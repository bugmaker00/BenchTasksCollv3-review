# Contract Checklist — `render_preview.json` vs `render_contract.md`

**Artifact under review:** `render_preview.json`  
**Contract version:** 1.0.0 (see `render_contract.md`)  
**Validation date:** 2025-09-01  
**Result: ALL 27 CHECKS PASS ✅**

---

## §1 — Field Catalogue and Field Order

| Check ID | Rule | Evidence in preview | Status |
|---|---|---|---|
| 1.0 | All 19 top-level fields present in declared order | Keys: `task_dir`, `id`, `needed_mcp_servers`, `needed_local_tools`, `task_root`, `task_str`, `log_file`, `agent_workspace`, `launch_time`, `max_turns`, `max_steps_under_single_turn_mode`, `single_turn_mode`, `cn_mode`, `system_prompts`, `initialization`, `stop`, `evaluation`, `meta`, `local_token_key_session` — exact order matches §1 table | ✅ PASS |
| 1.1 | `system_prompts` sub-fields: `agent` before `user` | `{"agent": "...", "user": "..."}` | ✅ PASS |
| 1.2 | `initialization` sub-fields: `workspace` before `process_command` | `{"workspace": "...", "process_command": "..."}` | ✅ PASS |
| 1.3 | `stop` sub-fields: `user_phrases` before `tool_names` | `{"user_phrases": [...], "tool_names": [...]}` | ✅ PASS |
| 1.4 | `evaluation` sub-fields: `groundtruth_workspace` before `evaluation_command` | `{"groundtruth_workspace": "...", "evaluation_command": "..."}` | ✅ PASS |

---

## §2 — Empty-Value Policy

| Check ID | Rule | Evidence in preview | Status |
|---|---|---|---|
| 2.1 | Optional `max_turns` serialised as `null` (not omitted) | `"max_turns": null` — key present | ✅ PASS |
| 2.2 | Optional `max_steps_under_single_turn_mode` serialised as `null` | `"max_steps_under_single_turn_mode": null` — key present | ✅ PASS |
| 2.3 | Optional `local_token_key_session` serialised as `null` | `"local_token_key_session": null` — key present | ✅ PASS |
| 2.4 | Unpopulated `meta` serialised as `{}` | `"meta": {}` | ✅ PASS |
| 2.5 | `single_turn_mode = false` → `max_steps_under_single_turn_mode = null` (tie-breaking rule) | `"single_turn_mode": false`, `"max_steps_under_single_turn_mode": null` | ✅ PASS |

---

## §3 — Normalization Rules

| Check ID | Rule | Evidence in preview | Status |
|---|---|---|---|
| 3.1a | `task_root` is absolute POSIX path (starts with `/`) | `"/opt/mcpbench/tasks/examples/example-task"` | ✅ PASS |
| 3.1b | `log_file` is absolute POSIX path | `"/opt/mcpbench/tasks/examples/example-task/log.json"` | ✅ PASS |
| 3.1c | `agent_workspace` is absolute POSIX path | `"/opt/mcpbench/tasks/examples/example-task/workspace"` | ✅ PASS |
| 3.1d | No trailing slash on `task_root` | value ends with `example-task` | ✅ PASS |
| 3.1e | No trailing slash on `log_file` | value ends with `log.json` | ✅ PASS |
| 3.1f | No trailing slash on `agent_workspace` | value ends with `workspace` | ✅ PASS |
| 3.2 | `task_dir` is a two-part relative path `<split>/<task_name>` with forward-slash only | `"examples/example-task"` — 2 parts, forward-slash, no leading/trailing slash | ✅ PASS |
| 3.3 | `id` = `task_dir` parts joined with `-` | `task_dir = "examples/example-task"` → `id = "examples-example-task"` ✓ | ✅ PASS |
| 3.4 | `launch_time` matches `YYYY-MM-DD HH:MM:SS <Weekday>` | `"2025-09-01 10:00:00 Monday"` — matches regex `\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2} \w+` | ✅ PASS |
| 3.5 | `initialization.process_command` = `"uv run -m <module>"` (preprocess/main.py exists) | `"uv run -m tasks.examples.example-task.preprocess.main"` | ✅ PASS |
| 3.6 | `evaluation.evaluation_command` = `"uv run -m <module>"` (evaluation/main.py exists) | `"uv run -m tasks.examples.example-task.evaluation.main"` | ✅ PASS |
| 3.7 | `system_prompts.agent` content reflects docs/agent_system_prompt.md (non-null, non-empty) | `"This file must be non-empty and all English (no Chinese)"` — sourced from tracked file | ✅ PASS |
| 3.8a | `needed_local_tools` is non-empty | `["python_execute", "claim_done"]` — length 2 | ✅ PASS |
| 3.8b | `needed_local_tools` contains `"claim_done"` | `"claim_done"` present at index 1 | ✅ PASS |
| 3.9 | `needed_mcp_servers` is non-empty | `["github"]` — length 1 | ✅ PASS |
| 3.10 | `stop.user_phrases` defaults to `["#### STOP"]` | `["#### STOP"]` | ✅ PASS |
| 3.11 | `stop.tool_names` defaults to `["local-claim_done"]` | `["local-claim_done"]` | ✅ PASS |
| 3.12 | `task_str` sourced from `docs/task.md` (non-empty) | `"This file must be non-empty and all English (no Chinese)"` — non-empty | ✅ PASS |

---

## §4 — Ordering Constraints

| Check ID | Rule | Evidence in preview | Status |
|---|---|---|---|
| 4.1 | Top-level field order strictly matches §1 (fields 1–19) | Confirmed by programmatic comparison against declared list | ✅ PASS |
| 4.2 | `single_turn_mode` is JSON boolean (not string or integer) | `false` (JSON boolean) | ✅ PASS |
| 4.3 | `cn_mode` is JSON boolean | `false` (JSON boolean) | ✅ PASS |
| 4.4 | `needed_local_tools` insertion order preserved; `"claim_done"` may appear at any position | `["python_execute", "claim_done"]` — `claim_done` at position 1 | ✅ PASS |

---

## §6 — Language Constraint

| Check ID | Rule | Evidence in preview | Status |
|---|---|---|---|
| 6.1 | `system_prompts.agent` non-empty and all English | Value is all-ASCII English text | ✅ PASS |
| 6.2 | `task_str` non-empty and all English (docs/task.md) | Value is all-ASCII English text | ✅ PASS |
| 6.3 | `system_prompts.user` non-null → must be all English | `"This file is optional, but if it is non-empty, is has to be all English"` — all-ASCII English text | ✅ PASS |

---

## Summary

| Contract section | Checks | Passed | Failed |
|---|---|---|---|
| §1 Field order | 5 | 5 | 0 |
| §2 Empty-value policy | 5 | 5 | 0 |
| §3 Normalization rules | 14 | 14 | 0 |
| §4 Ordering constraints | 4 | 4 | 0 |
| §6 Language constraint | 3 | 3 | 0 |
| **Total** | **31** | **31** | **0** |

**Conclusion:** `render_preview.json` is fully conformant with `render_contract.md` version 1.0.0.  
No violations were detected. The preview is approved as a valid representative of the  
MCPBench Task File-Set Artifact schema.
