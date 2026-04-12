# Render Contract — MCPBench Task File-Set Artifact

**Contract version:** 1.0.0  
**Repository snapshot:** `BenchTasksCollv3-review` @ `6ac0348` ("Add example task template")  
**Reviewed change set:** 8 files introduced in commit `6ac0348` (the example task template)  
**Scope:** This contract governs the serialised JSON representation of a fully-resolved  
`TaskConfig` object produced by `TaskConfig.to_dict()` in  
`utils/data_structures/task_config.py`.  
This JSON is the canonical **file-set artifact** exchanged between the benchmark  
runner, the evaluation harness, and any downstream tooling.

---

## 1. Field Catalogue and Field Order

Fields **must** appear in the JSON object in exactly the order listed below.  
No additional top-level fields are permitted.

| # | Field name | JSON type | Required | Default when absent |
|---|---|---|---|---|
| 1 | `task_dir` | string | **yes** | — |
| 2 | `id` | string | **yes** | derived |
| 3 | `needed_mcp_servers` | array of strings | **yes** | — |
| 4 | `needed_local_tools` | array of strings | **yes** | — |
| 5 | `task_root` | string | **yes** | derived |
| 6 | `task_str` | string | **yes** | read from `docs/task.md` |
| 7 | `log_file` | string | **yes** | derived |
| 8 | `agent_workspace` | string | **yes** | derived |
| 9 | `launch_time` | string | **yes** | runtime timestamp |
| 10 | `max_turns` | integer \| null | no | `null` |
| 11 | `max_steps_under_single_turn_mode` | integer \| null | no | `null` |
| 12 | `single_turn_mode` | boolean | **yes** | `false` |
| 13 | `cn_mode` | boolean | **yes** | `false` |
| 14 | `system_prompts` | object | **yes** | — |
| 15 | `initialization` | object | **yes** | — |
| 16 | `stop` | object | **yes** | — |
| 17 | `evaluation` | object | **yes** | — |
| 18 | `meta` | object | **yes** | `{}` |
| 19 | `local_token_key_session` | object \| null | no | `null` |

### 1.1 `system_prompts` sub-object (field 14)

Sub-fields must appear in this order:

| # | Field name | JSON type | Required |
|---|---|---|---|
| 1 | `agent` | string \| null | yes |
| 2 | `user` | string \| null | yes |

### 1.2 `initialization` sub-object (field 15)

Sub-fields must appear in this order:

| # | Field name | JSON type | Required |
|---|---|---|---|
| 1 | `workspace` | string \| null | yes |
| 2 | `process_command` | string \| null | yes |

### 1.3 `stop` sub-object (field 16)

Sub-fields must appear in this order:

| # | Field name | JSON type | Required |
|---|---|---|---|
| 1 | `user_phrases` | array of strings | yes |
| 2 | `tool_names` | array of strings | yes |

### 1.4 `evaluation` sub-object (field 17)

Sub-fields must appear in this order:

| # | Field name | JSON type | Required |
|---|---|---|---|
| 1 | `groundtruth_workspace` | string \| null | yes |
| 2 | `evaluation_command` | string \| null | yes |

---

## 2. Empty-Value Policy

| Condition | Representation in JSON |
|---|---|
| Optional field not configured | JSON `null` (never omitted) |
| Optional list not populated | `[]` (empty array) |
| Optional object not populated | `{}` (empty object) |
| Optional string not populated | `null` |
| `meta` when no metadata | `{}` |
| `local_token_key_session` when absent | `null` |
| `max_turns` when unlimited | `null` |
| `max_steps_under_single_turn_mode` when not in single-turn mode | `null` |

**Rule:** Fields that are optional and have no value are always serialised as `null` (or  
their empty-collection equivalent). They are **never omitted** from the JSON object,  
so that consumers can always rely on the presence of every declared key.

**Tie-breaking:** When `single_turn_mode` is `false` and  
`max_steps_under_single_turn_mode` would be unused, it is serialised as `null`.

---

## 3. Normalization Rules

### 3.1 Path fields (`task_root`, `log_file`, `agent_workspace`)
- All path strings must be **absolute POSIX paths** (no trailing slash).
- Produced by `os.path.abspath(…)` at serialisation time.

### 3.2 `task_dir`
- Must be a two-part relative path of the form `<split>/<task_name>`  
  (e.g., `examples/example-task`).
- Forward-slash separator only; no leading or trailing slash.

### 3.3 `id`
- Derived from `task_dir` by joining its two path components with `-`  
  (e.g., `task_dir = "examples/example-task"` → `id = "examples-example-task"`).

### 3.4 `launch_time`
- Format: `YYYY-MM-DD HH:MM:SS <weekday>` (e.g., `"2025-09-01 10:00:00 Monday"`).
- Produced by `datetime.now().strftime("%Y-%m-%d %H:%M:%S %A")`.

### 3.5 `initialization.process_command`
- If `preprocess/main.py` exists: `"uv run -m <dot.separated.module.path>"`.
- If absent: `null`.

### 3.6 `evaluation.evaluation_command`
- If `evaluation/main.py` exists: `"uv run -m <dot.separated.module.path>"`.
- If absent: `null`.

### 3.7 `system_prompts.agent`
- Template placeholders replaced at runtime before serialisation:
  - `!!<<<<||||current_working_dir||||>>>>!!` → `os.getcwd()`
  - `!!<<<<||||workspace_dir||||>>>>!!` → absolute path of `agent_workspace`
  - `!!<<<<||||workspace_dir_rela||||>>>>!!` → relative path of `agent_workspace`
  - `!!<<<<||||time||||>>>>!!` → `launch_time`

### 3.8 `needed_local_tools`
- Must be a **non-empty** array.
- Must contain the string `"claim_done"` as one of its elements.
- Elements are plain strings; no deduplication or sorting is applied.

### 3.9 `needed_mcp_servers`
- Must be a **non-empty** array.
- Elements are plain strings; order reflects dependency priority (no forced sort).

### 3.10 `stop.user_phrases` default
- When not overridden in `task_config.json`, defaults to `["#### STOP"]`.

### 3.11 `stop.tool_names` default
- When not overridden in `task_config.json`, defaults to `["local-claim_done"]`.

### 3.12 `task_str`
- Content of `docs/task.md` read verbatim (UTF-8, no trimming).
- In `cn_mode`, read from `docs/task_cn.md` instead.

---

## 4. Ordering Constraints

| Constraint | Rule |
|---|---|
| Top-level fields | Strictly ordered as listed in §1 (fields 1–19). |
| `system_prompts` sub-fields | `agent` before `user`. |
| `initialization` sub-fields | `workspace` before `process_command`. |
| `stop` sub-fields | `user_phrases` before `tool_names`. |
| `evaluation` sub-fields | `groundtruth_workspace` before `evaluation_command`. |
| `needed_mcp_servers` elements | Insertion order preserved; no forced sort. |
| `needed_local_tools` elements | Insertion order preserved; `"claim_done"` may appear at any position. |
| `meta` keys | Insertion order preserved; no forced sort. |
| `stop.user_phrases` elements | Insertion order preserved. |
| `stop.tool_names` elements | Insertion order preserved. |

---

## 5. Validated Source Files (Reviewed Change Set — commit 6ac0348)

The following 8 files were introduced in the reviewed change set and define  
the authoritative example task that this contract describes:

```
tasks/examples/example-task/readme.txt
tasks/examples/example-task/docs/agent_system_prompt.md
tasks/examples/example-task/docs/task.md
tasks/examples/example-task/docs/user_system_prompt.md
tasks/examples/example-task/evaluation/main.py
tasks/examples/example-task/groundtruth_workspace/readme.txt
tasks/examples/example-task/initial_workspace/readme.txt
tasks/examples/example-task/preprocess/main.py
```

Additionally, `tasks/examples/example-task/task_config.json` (not tracked in the  
reviewed commit) must satisfy these rules when present:
- `needed_mcp_servers`: non-empty array of strings.
- `needed_local_tools`: non-empty array containing `"claim_done"`.

---

## 6. Language Constraint

- `docs/agent_system_prompt.md` must be non-empty and written entirely in English.
- `docs/task.md` must be non-empty and written entirely in English.
- `docs/user_system_prompt.md` is optional; if non-empty it must be written entirely in English.
- Update-log entries and Chinese-mode (`cn_mode`) variants are exempt from this rule.
