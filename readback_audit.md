# Readback Audit – finalpool Review Branch

**Generated:** 2026-04-09 10:12 UTC  
**Repository:** `bugmaker00/BenchTasksCollv3-review`  
**Review branch:** `finalpool`  
**Live commit:** `531b8ecc7c8d351a11f828fb88b6b34be91c5857`  
**Source-of-truth:** `full_scope.csv`

---

## Summary

| Metric | Value |
|--------|-------|
| Tasks in scope | 77 |
| Files in scope (CSV) | 385 |
| Files observed live | 385 |
| Exact SHA matches | 385 |
| SHA mismatches | 0 |
| Missing from live | 0 |
| Unexpected extras in live | 0 |
| Audit result | ✅ PASS – live state matches saved scope 100% |

---

## Developer Contribution Summary

| Developer | Branch | Tasks | Files |
|-----------|--------|-------|-------|
| `fan` | `fan-dev` | 4 | 17 |
| `gyy` | `gyy` | 6 | 37 |
| `haoze` | `haoze` | 4 | 22 |
| `jl` | `jl_dev` | 5 | 25 |
| `junteng` | `junteng_dev` | 8 | 42 |
| `junxian` | `junxian_dev` | 3 | 18 |
| `lueyang` | `lueyang-dev` | 8 | 43 |
| `lv` | `lv` | 7 | 32 |
| `ruige` | `ruige` | 6 | 28 |
| `wenshuo` | `wenshuo-dev` | 4 | 22 |
| `xiaochen` | `xiaochen_dev` | 7 | 36 |
| `yuxuan` | `yuxuan-dev` | 5 | 23 |
| `yuzhen` | `yuzhen-dev` | 6 | 27 |
| `zhaochen` | `zhaochen` | 4 | 13 |

---

## Line-by-Line Audit: full_scope.csv vs Live State

Each row below corresponds to one entry in `full_scope.csv` and confirms whether the live file SHA on the `finalpool` branch matches the recorded value.

| # | Task | Destination Path | Scope SHA (first 10) | Live SHA (first 10) | Status |
|---|------|-----------------|----------------------|---------------------|--------|
| 1 | `activity-logger` | `tasks/finalpool/activity-logger/docs/agent_system_prompt.md` | `7a82a562e4` | `7a82a562e4` | ✅ |
| 2 | `activity-logger` | `tasks/finalpool/activity-logger/docs/task.md` | `07edc9f1cf` | `07edc9f1cf` | ✅ |
| 3 | `activity-logger` | `tasks/finalpool/activity-logger/docs/user_system_prompt.md` | `da1a27fb93` | `da1a27fb93` | ✅ |
| 4 | `activity-logger` | `tasks/finalpool/activity-logger/evaluation/main.py` | `0f298beb21` | `0f298beb21` | ✅ |
| 5 | `activity-logger` | `tasks/finalpool/activity-logger/initial_workspace/readme.txt` | `452e4680c1` | `452e4680c1` | ✅ |
| 6 | `alert-system` | `tasks/finalpool/alert-system/docs/agent_system_prompt.md` | `daf846d28f` | `daf846d28f` | ✅ |
| 7 | `alert-system` | `tasks/finalpool/alert-system/docs/task.md` | `eac81c97cd` | `eac81c97cd` | ✅ |
| 8 | `alert-system` | `tasks/finalpool/alert-system/docs/user_system_prompt.md` | `4e3eea6832` | `4e3eea6832` | ✅ |
| 9 | `alert-system` | `tasks/finalpool/alert-system/evaluation/main.py` | `3ec09e6e52` | `3ec09e6e52` | ✅ |
| 10 | `alert-system` | `tasks/finalpool/alert-system/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 11 | `analytics-dashboard` | `tasks/finalpool/analytics-dashboard/docs/agent_system_prompt.md` | `af735f9c24` | `af735f9c24` | ✅ |
| 12 | `analytics-dashboard` | `tasks/finalpool/analytics-dashboard/docs/task.md` | `3e22a21e8d` | `3e22a21e8d` | ✅ |
| 13 | `analytics-dashboard` | `tasks/finalpool/analytics-dashboard/docs/user_system_prompt.md` | `f0cfee02e3` | `f0cfee02e3` | ✅ |
| 14 | `analytics-dashboard` | `tasks/finalpool/analytics-dashboard/evaluation/main.py` | `d3ec5c3f84` | `d3ec5c3f84` | ✅ |
| 15 | `asset-optimizer` | `tasks/finalpool/asset-optimizer/docs/agent_system_prompt.md` | `f804ede58f` | `f804ede58f` | ✅ |
| 16 | `asset-optimizer` | `tasks/finalpool/asset-optimizer/docs/task.md` | `3fe083333d` | `3fe083333d` | ✅ |
| 17 | `asset-optimizer` | `tasks/finalpool/asset-optimizer/evaluation/main.py` | `ac0fc2e202` | `ac0fc2e202` | ✅ |
| 18 | `asset-optimizer` | `tasks/finalpool/asset-optimizer/groundtruth_workspace/readme.txt` | `003bd96629` | `003bd96629` | ✅ |
| 19 | `asset-optimizer` | `tasks/finalpool/asset-optimizer/initial_workspace/readme.txt` | `037e22b77b` | `037e22b77b` | ✅ |
| 20 | `backup-utility` | `tasks/finalpool/backup-utility/docs/agent_system_prompt.md` | `860943ea76` | `860943ea76` | ✅ |
| 21 | `backup-utility` | `tasks/finalpool/backup-utility/docs/task.md` | `df94e32a20` | `df94e32a20` | ✅ |
| 22 | `backup-utility` | `tasks/finalpool/backup-utility/evaluation/main.py` | `c73ac7574c` | `c73ac7574c` | ✅ |
| 23 | `backup-utility` | `tasks/finalpool/backup-utility/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 24 | `blog-engine` | `tasks/finalpool/blog-engine/docs/agent_system_prompt.md` | `cadecba4bb` | `cadecba4bb` | ✅ |
| 25 | `blog-engine` | `tasks/finalpool/blog-engine/docs/task.md` | `11b5f36c57` | `11b5f36c57` | ✅ |
| 26 | `blog-engine` | `tasks/finalpool/blog-engine/evaluation/main.py` | `8ad8ad13c9` | `8ad8ad13c9` | ✅ |
| 27 | `blog-engine` | `tasks/finalpool/blog-engine/groundtruth_workspace/readme.txt` | `1de574c148` | `1de574c148` | ✅ |
| 28 | `blog-engine` | `tasks/finalpool/blog-engine/initial_workspace/readme.txt` | `2a1248ef26` | `2a1248ef26` | ✅ |
| 29 | `blog-engine` | `tasks/finalpool/blog-engine/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 30 | `booking-system` | `tasks/finalpool/booking-system/docs/agent_system_prompt.md` | `9f31a9f20a` | `9f31a9f20a` | ✅ |
| 31 | `booking-system` | `tasks/finalpool/booking-system/docs/task.md` | `7a39ea59fd` | `7a39ea59fd` | ✅ |
| 32 | `booking-system` | `tasks/finalpool/booking-system/docs/user_system_prompt.md` | `6db1275608` | `6db1275608` | ✅ |
| 33 | `booking-system` | `tasks/finalpool/booking-system/evaluation/main.py` | `6233aa8b1e` | `6233aa8b1e` | ✅ |
| 34 | `booking-system` | `tasks/finalpool/booking-system/groundtruth_workspace/readme.txt` | `4585d8e79e` | `4585d8e79e` | ✅ |
| 35 | `booking-system` | `tasks/finalpool/booking-system/initial_workspace/readme.txt` | `96007f01eb` | `96007f01eb` | ✅ |
| 36 | `booking-system` | `tasks/finalpool/booking-system/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 37 | `cache-optimizer` | `tasks/finalpool/cache-optimizer/docs/agent_system_prompt.md` | `e8a0f83716` | `e8a0f83716` | ✅ |
| 38 | `cache-optimizer` | `tasks/finalpool/cache-optimizer/docs/task.md` | `fe0ef157e9` | `fe0ef157e9` | ✅ |
| 39 | `cache-optimizer` | `tasks/finalpool/cache-optimizer/evaluation/main.py` | `92a32801de` | `92a32801de` | ✅ |
| 40 | `cache-optimizer` | `tasks/finalpool/cache-optimizer/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 41 | `calendar-sync` | `tasks/finalpool/calendar-sync/docs/agent_system_prompt.md` | `a9686f317d` | `a9686f317d` | ✅ |
| 42 | `calendar-sync` | `tasks/finalpool/calendar-sync/docs/task.md` | `9be622c990` | `9be622c990` | ✅ |
| 43 | `calendar-sync` | `tasks/finalpool/calendar-sync/docs/user_system_prompt.md` | `76b7f760ce` | `76b7f760ce` | ✅ |
| 44 | `calendar-sync` | `tasks/finalpool/calendar-sync/evaluation/main.py` | `9b8b9bea63` | `9b8b9bea63` | ✅ |
| 45 | `calendar-sync` | `tasks/finalpool/calendar-sync/groundtruth_workspace/readme.txt` | `a07ba1f362` | `a07ba1f362` | ✅ |
| 46 | `calendar-sync` | `tasks/finalpool/calendar-sync/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 47 | `canvas-automation` | `tasks/finalpool/canvas-automation/docs/agent_system_prompt.md` | `57542673b4` | `57542673b4` | ✅ |
| 48 | `canvas-automation` | `tasks/finalpool/canvas-automation/docs/task.md` | `c5909995cf` | `c5909995cf` | ✅ |
| 49 | `canvas-automation` | `tasks/finalpool/canvas-automation/evaluation/main.py` | `c0511c9c52` | `c0511c9c52` | ✅ |
| 50 | `canvas-automation` | `tasks/finalpool/canvas-automation/initial_workspace/readme.txt` | `da813cedf9` | `da813cedf9` | ✅ |
| 51 | `canvas-automation` | `tasks/finalpool/canvas-automation/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 52 | `canvas-grade-automation` | `tasks/finalpool/canvas-grade-automation/docs/agent_system_prompt.md` | `fc8abeded1` | `fc8abeded1` | ✅ |
| 53 | `canvas-grade-automation` | `tasks/finalpool/canvas-grade-automation/docs/task.md` | `b4bbfddfe6` | `b4bbfddfe6` | ✅ |
| 54 | `canvas-grade-automation` | `tasks/finalpool/canvas-grade-automation/evaluation/main.py` | `2e5b6f752e` | `2e5b6f752e` | ✅ |
| 55 | `canvas-grade-automation` | `tasks/finalpool/canvas-grade-automation/groundtruth_workspace/readme.txt` | `6e09110842` | `6e09110842` | ✅ |
| 56 | `certificate-manager` | `tasks/finalpool/certificate-manager/docs/agent_system_prompt.md` | `797cdb2e91` | `797cdb2e91` | ✅ |
| 57 | `certificate-manager` | `tasks/finalpool/certificate-manager/docs/task.md` | `45e0a04b00` | `45e0a04b00` | ✅ |
| 58 | `certificate-manager` | `tasks/finalpool/certificate-manager/evaluation/main.py` | `8a10dea710` | `8a10dea710` | ✅ |
| 59 | `chat-bot` | `tasks/finalpool/chat-bot/docs/agent_system_prompt.md` | `93526c8187` | `93526c8187` | ✅ |
| 60 | `chat-bot` | `tasks/finalpool/chat-bot/docs/task.md` | `333f77688b` | `333f77688b` | ✅ |
| 61 | `chat-bot` | `tasks/finalpool/chat-bot/docs/user_system_prompt.md` | `1655610d1a` | `1655610d1a` | ✅ |
| 62 | `chat-bot` | `tasks/finalpool/chat-bot/evaluation/main.py` | `c8b7543e0f` | `c8b7543e0f` | ✅ |
| 63 | `chat-bot` | `tasks/finalpool/chat-bot/initial_workspace/readme.txt` | `949b059ef5` | `949b059ef5` | ✅ |
| 64 | `chat-bot` | `tasks/finalpool/chat-bot/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 65 | `client-portal` | `tasks/finalpool/client-portal/docs/agent_system_prompt.md` | `1517f069a2` | `1517f069a2` | ✅ |
| 66 | `client-portal` | `tasks/finalpool/client-portal/docs/task.md` | `b2972de7e6` | `b2972de7e6` | ✅ |
| 67 | `client-portal` | `tasks/finalpool/client-portal/docs/user_system_prompt.md` | `b5798087f8` | `b5798087f8` | ✅ |
| 68 | `client-portal` | `tasks/finalpool/client-portal/evaluation/main.py` | `33542a0115` | `33542a0115` | ✅ |
| 69 | `client-portal` | `tasks/finalpool/client-portal/groundtruth_workspace/readme.txt` | `eb8eb29000` | `eb8eb29000` | ✅ |
| 70 | `client-portal` | `tasks/finalpool/client-portal/initial_workspace/readme.txt` | `612f91ae44` | `612f91ae44` | ✅ |
| 71 | `client-portal` | `tasks/finalpool/client-portal/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 72 | `cms-builder` | `tasks/finalpool/cms-builder/docs/agent_system_prompt.md` | `3fd93f4403` | `3fd93f4403` | ✅ |
| 73 | `cms-builder` | `tasks/finalpool/cms-builder/docs/task.md` | `3e0263be84` | `3e0263be84` | ✅ |
| 74 | `cms-builder` | `tasks/finalpool/cms-builder/docs/user_system_prompt.md` | `7193c26ca6` | `7193c26ca6` | ✅ |
| 75 | `cms-builder` | `tasks/finalpool/cms-builder/evaluation/main.py` | `84ccab21d4` | `84ccab21d4` | ✅ |
| 76 | `cms-builder` | `tasks/finalpool/cms-builder/groundtruth_workspace/readme.txt` | `ad6f4c0740` | `ad6f4c0740` | ✅ |
| 77 | `cms-builder` | `tasks/finalpool/cms-builder/initial_workspace/readme.txt` | `ecea21fcef` | `ecea21fcef` | ✅ |
| 78 | `cms-builder` | `tasks/finalpool/cms-builder/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 79 | `contact-manager` | `tasks/finalpool/contact-manager/docs/agent_system_prompt.md` | `37a564aaf9` | `37a564aaf9` | ✅ |
| 80 | `contact-manager` | `tasks/finalpool/contact-manager/docs/task.md` | `047e004f43` | `047e004f43` | ✅ |
| 81 | `contact-manager` | `tasks/finalpool/contact-manager/docs/user_system_prompt.md` | `f61c99cd04` | `f61c99cd04` | ✅ |
| 82 | `contact-manager` | `tasks/finalpool/contact-manager/evaluation/main.py` | `8f2296d2d0` | `8f2296d2d0` | ✅ |
| 83 | `contact-manager` | `tasks/finalpool/contact-manager/groundtruth_workspace/readme.txt` | `56ed915025` | `56ed915025` | ✅ |
| 84 | `contact-manager` | `tasks/finalpool/contact-manager/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 85 | `content-manager` | `tasks/finalpool/content-manager/docs/agent_system_prompt.md` | `3416a4b47d` | `3416a4b47d` | ✅ |
| 86 | `content-manager` | `tasks/finalpool/content-manager/docs/task.md` | `02802002d1` | `02802002d1` | ✅ |
| 87 | `content-manager` | `tasks/finalpool/content-manager/docs/user_system_prompt.md` | `3da6f47240` | `3da6f47240` | ✅ |
| 88 | `content-manager` | `tasks/finalpool/content-manager/evaluation/main.py` | `982a15a5b3` | `982a15a5b3` | ✅ |
| 89 | `content-manager` | `tasks/finalpool/content-manager/groundtruth_workspace/readme.txt` | `44cb789124` | `44cb789124` | ✅ |
| 90 | `content-manager` | `tasks/finalpool/content-manager/initial_workspace/readme.txt` | `b620fa6801` | `b620fa6801` | ✅ |
| 91 | `content-manager` | `tasks/finalpool/content-manager/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 92 | `content-scheduler` | `tasks/finalpool/content-scheduler/docs/agent_system_prompt.md` | `1e0c0a2799` | `1e0c0a2799` | ✅ |
| 93 | `content-scheduler` | `tasks/finalpool/content-scheduler/docs/task.md` | `de4bf4aad4` | `de4bf4aad4` | ✅ |
| 94 | `content-scheduler` | `tasks/finalpool/content-scheduler/docs/user_system_prompt.md` | `341037927a` | `341037927a` | ✅ |
| 95 | `content-scheduler` | `tasks/finalpool/content-scheduler/evaluation/main.py` | `1f76ffb0b2` | `1f76ffb0b2` | ✅ |
| 96 | `content-scheduler` | `tasks/finalpool/content-scheduler/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 97 | `coupon-manager` | `tasks/finalpool/coupon-manager/docs/agent_system_prompt.md` | `a4125f15ca` | `a4125f15ca` | ✅ |
| 98 | `coupon-manager` | `tasks/finalpool/coupon-manager/docs/task.md` | `d000140885` | `d000140885` | ✅ |
| 99 | `coupon-manager` | `tasks/finalpool/coupon-manager/evaluation/main.py` | `123fa3d7df` | `123fa3d7df` | ✅ |
| 100 | `coupon-manager` | `tasks/finalpool/coupon-manager/groundtruth_workspace/readme.txt` | `cb660dd46d` | `cb660dd46d` | ✅ |
| 101 | `crm-system` | `tasks/finalpool/crm-system/docs/agent_system_prompt.md` | `aed247732d` | `aed247732d` | ✅ |
| 102 | `crm-system` | `tasks/finalpool/crm-system/docs/task.md` | `e99bf9b1a7` | `e99bf9b1a7` | ✅ |
| 103 | `crm-system` | `tasks/finalpool/crm-system/docs/user_system_prompt.md` | `3200c3655e` | `3200c3655e` | ✅ |
| 104 | `crm-system` | `tasks/finalpool/crm-system/evaluation/main.py` | `b0218b569f` | `b0218b569f` | ✅ |
| 105 | `crm-system` | `tasks/finalpool/crm-system/groundtruth_workspace/readme.txt` | `fd607ce918` | `fd607ce918` | ✅ |
| 106 | `crm-system` | `tasks/finalpool/crm-system/initial_workspace/readme.txt` | `862860d2ef` | `862860d2ef` | ✅ |
| 107 | `crm-system` | `tasks/finalpool/crm-system/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 108 | `customer-feedback-processor` | `tasks/finalpool/customer-feedback-processor/docs/agent_system_prompt.md` | `157b0b4847` | `157b0b4847` | ✅ |
| 109 | `customer-feedback-processor` | `tasks/finalpool/customer-feedback-processor/docs/task.md` | `2f669aeb7f` | `2f669aeb7f` | ✅ |
| 110 | `customer-feedback-processor` | `tasks/finalpool/customer-feedback-processor/evaluation/main.py` | `f12b85da1b` | `f12b85da1b` | ✅ |
| 111 | `customer-feedback-processor` | `tasks/finalpool/customer-feedback-processor/groundtruth_workspace/readme.txt` | `4b0898f2c6` | `4b0898f2c6` | ✅ |
| 112 | `customer-feedback-processor` | `tasks/finalpool/customer-feedback-processor/initial_workspace/readme.txt` | `e3f4210010` | `e3f4210010` | ✅ |
| 113 | `data-analytics` | `tasks/finalpool/data-analytics/docs/agent_system_prompt.md` | `30f7f40b71` | `30f7f40b71` | ✅ |
| 114 | `data-analytics` | `tasks/finalpool/data-analytics/docs/task.md` | `fc59c3f6f7` | `fc59c3f6f7` | ✅ |
| 115 | `data-analytics` | `tasks/finalpool/data-analytics/evaluation/main.py` | `da13921e56` | `da13921e56` | ✅ |
| 116 | `data-analytics` | `tasks/finalpool/data-analytics/groundtruth_workspace/readme.txt` | `a75ccdc451` | `a75ccdc451` | ✅ |
| 117 | `data-analytics` | `tasks/finalpool/data-analytics/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 118 | `data-validator` | `tasks/finalpool/data-validator/docs/agent_system_prompt.md` | `4fdcc38500` | `4fdcc38500` | ✅ |
| 119 | `data-validator` | `tasks/finalpool/data-validator/docs/task.md` | `43c54ce05b` | `43c54ce05b` | ✅ |
| 120 | `data-validator` | `tasks/finalpool/data-validator/evaluation/main.py` | `ec160b52e6` | `ec160b52e6` | ✅ |
| 121 | `data-validator` | `tasks/finalpool/data-validator/initial_workspace/readme.txt` | `4613c754e3` | `4613c754e3` | ✅ |
| 122 | `data-validator` | `tasks/finalpool/data-validator/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 123 | `deal-manager` | `tasks/finalpool/deal-manager/docs/agent_system_prompt.md` | `822d0dce41` | `822d0dce41` | ✅ |
| 124 | `deal-manager` | `tasks/finalpool/deal-manager/docs/task.md` | `485125d053` | `485125d053` | ✅ |
| 125 | `deal-manager` | `tasks/finalpool/deal-manager/evaluation/main.py` | `ca2d0cdee4` | `ca2d0cdee4` | ✅ |
| 126 | `deal-manager` | `tasks/finalpool/deal-manager/groundtruth_workspace/readme.txt` | `771c7bea48` | `771c7bea48` | ✅ |
| 127 | `deal-manager` | `tasks/finalpool/deal-manager/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 128 | `deployment-tool` | `tasks/finalpool/deployment-tool/docs/agent_system_prompt.md` | `439254e7f3` | `439254e7f3` | ✅ |
| 129 | `deployment-tool` | `tasks/finalpool/deployment-tool/docs/task.md` | `d2ed062095` | `d2ed062095` | ✅ |
| 130 | `deployment-tool` | `tasks/finalpool/deployment-tool/docs/user_system_prompt.md` | `0f8ca4f49e` | `0f8ca4f49e` | ✅ |
| 131 | `deployment-tool` | `tasks/finalpool/deployment-tool/evaluation/main.py` | `f51f8d260c` | `f51f8d260c` | ✅ |
| 132 | `deployment-tool` | `tasks/finalpool/deployment-tool/groundtruth_workspace/readme.txt` | `059c7ef13b` | `059c7ef13b` | ✅ |
| 133 | `deployment-tool` | `tasks/finalpool/deployment-tool/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 134 | `discount-calculator` | `tasks/finalpool/discount-calculator/docs/agent_system_prompt.md` | `1bdcfd62f6` | `1bdcfd62f6` | ✅ |
| 135 | `discount-calculator` | `tasks/finalpool/discount-calculator/docs/task.md` | `3d8ecabfbc` | `3d8ecabfbc` | ✅ |
| 136 | `discount-calculator` | `tasks/finalpool/discount-calculator/evaluation/main.py` | `b9e4eef4c4` | `b9e4eef4c4` | ✅ |
| 137 | `discount-calculator` | `tasks/finalpool/discount-calculator/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 138 | `email-campaign` | `tasks/finalpool/email-campaign/docs/agent_system_prompt.md` | `b5571ff0b8` | `b5571ff0b8` | ✅ |
| 139 | `email-campaign` | `tasks/finalpool/email-campaign/docs/task.md` | `bfb291790b` | `bfb291790b` | ✅ |
| 140 | `email-campaign` | `tasks/finalpool/email-campaign/docs/user_system_prompt.md` | `d02fc5512a` | `d02fc5512a` | ✅ |
| 141 | `email-campaign` | `tasks/finalpool/email-campaign/evaluation/main.py` | `3ad9498d28` | `3ad9498d28` | ✅ |
| 142 | `email-campaign` | `tasks/finalpool/email-campaign/groundtruth_workspace/readme.txt` | `b594bff06f` | `b594bff06f` | ✅ |
| 143 | `email-campaign` | `tasks/finalpool/email-campaign/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 144 | `email-classification-system` | `tasks/finalpool/email-classification-system/docs/agent_system_prompt.md` | `7358c0e497` | `7358c0e497` | ✅ |
| 145 | `email-classification-system` | `tasks/finalpool/email-classification-system/docs/task.md` | `ef4d26b713` | `ef4d26b713` | ✅ |
| 146 | `email-classification-system` | `tasks/finalpool/email-classification-system/evaluation/main.py` | `d59a313242` | `d59a313242` | ✅ |
| 147 | `email-classification-system` | `tasks/finalpool/email-classification-system/groundtruth_workspace/readme.txt` | `1b84edb603` | `1b84edb603` | ✅ |
| 148 | `email-classification-system` | `tasks/finalpool/email-classification-system/initial_workspace/readme.txt` | `7403c7b29c` | `7403c7b29c` | ✅ |
| 149 | `email-classification-system` | `tasks/finalpool/email-classification-system/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 150 | `error-tracker` | `tasks/finalpool/error-tracker/docs/agent_system_prompt.md` | `7edfe1654a` | `7edfe1654a` | ✅ |
| 151 | `error-tracker` | `tasks/finalpool/error-tracker/docs/task.md` | `c405eeb6f1` | `c405eeb6f1` | ✅ |
| 152 | `error-tracker` | `tasks/finalpool/error-tracker/docs/user_system_prompt.md` | `9812415682` | `9812415682` | ✅ |
| 153 | `error-tracker` | `tasks/finalpool/error-tracker/evaluation/main.py` | `a5a871584a` | `a5a871584a` | ✅ |
| 154 | `error-tracker` | `tasks/finalpool/error-tracker/groundtruth_workspace/readme.txt` | `889635f3d8` | `889635f3d8` | ✅ |
| 155 | `expense-tracker` | `tasks/finalpool/expense-tracker/docs/agent_system_prompt.md` | `dd1527c8e1` | `dd1527c8e1` | ✅ |
| 156 | `expense-tracker` | `tasks/finalpool/expense-tracker/docs/task.md` | `2d04cc1787` | `2d04cc1787` | ✅ |
| 157 | `expense-tracker` | `tasks/finalpool/expense-tracker/docs/user_system_prompt.md` | `f33b43ddad` | `f33b43ddad` | ✅ |
| 158 | `expense-tracker` | `tasks/finalpool/expense-tracker/evaluation/main.py` | `aa44f7e511` | `aa44f7e511` | ✅ |
| 159 | `expense-tracker` | `tasks/finalpool/expense-tracker/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 160 | `feedback-collector` | `tasks/finalpool/feedback-collector/docs/agent_system_prompt.md` | `a2f93a5f68` | `a2f93a5f68` | ✅ |
| 161 | `feedback-collector` | `tasks/finalpool/feedback-collector/docs/task.md` | `0a80d28b35` | `0a80d28b35` | ✅ |
| 162 | `feedback-collector` | `tasks/finalpool/feedback-collector/docs/user_system_prompt.md` | `1dcd2febff` | `1dcd2febff` | ✅ |
| 163 | `feedback-collector` | `tasks/finalpool/feedback-collector/evaluation/main.py` | `987379d7c3` | `987379d7c3` | ✅ |
| 164 | `feedback-collector` | `tasks/finalpool/feedback-collector/initial_workspace/readme.txt` | `fb367d1db3` | `fb367d1db3` | ✅ |
| 165 | `file-manager` | `tasks/finalpool/file-manager/docs/agent_system_prompt.md` | `cbdafc0c17` | `cbdafc0c17` | ✅ |
| 166 | `file-manager` | `tasks/finalpool/file-manager/docs/task.md` | `e47e4d2eb2` | `e47e4d2eb2` | ✅ |
| 167 | `file-manager` | `tasks/finalpool/file-manager/evaluation/main.py` | `c212153783` | `c212153783` | ✅ |
| 168 | `file-manager` | `tasks/finalpool/file-manager/initial_workspace/readme.txt` | `39066d1c18` | `39066d1c18` | ✅ |
| 169 | `follow-up-reminder` | `tasks/finalpool/follow-up-reminder/docs/agent_system_prompt.md` | `1179aefbab` | `1179aefbab` | ✅ |
| 170 | `follow-up-reminder` | `tasks/finalpool/follow-up-reminder/docs/task.md` | `793f1e2b6b` | `793f1e2b6b` | ✅ |
| 171 | `follow-up-reminder` | `tasks/finalpool/follow-up-reminder/docs/user_system_prompt.md` | `da20647087` | `da20647087` | ✅ |
| 172 | `follow-up-reminder` | `tasks/finalpool/follow-up-reminder/evaluation/main.py` | `659cacbb0b` | `659cacbb0b` | ✅ |
| 173 | `follow-up-reminder` | `tasks/finalpool/follow-up-reminder/groundtruth_workspace/readme.txt` | `e53072f448` | `e53072f448` | ✅ |
| 174 | `form-builder` | `tasks/finalpool/form-builder/docs/agent_system_prompt.md` | `870eb246b0` | `870eb246b0` | ✅ |
| 175 | `form-builder` | `tasks/finalpool/form-builder/docs/task.md` | `c51655a9f8` | `c51655a9f8` | ✅ |
| 176 | `form-builder` | `tasks/finalpool/form-builder/evaluation/main.py` | `b0d50f2cb2` | `b0d50f2cb2` | ✅ |
| 177 | `health-monitor` | `tasks/finalpool/health-monitor/docs/agent_system_prompt.md` | `22489282fa` | `22489282fa` | ✅ |
| 178 | `health-monitor` | `tasks/finalpool/health-monitor/docs/task.md` | `c072e606de` | `c072e606de` | ✅ |
| 179 | `health-monitor` | `tasks/finalpool/health-monitor/evaluation/main.py` | `dee407e663` | `dee407e663` | ✅ |
| 180 | `health-monitor` | `tasks/finalpool/health-monitor/groundtruth_workspace/readme.txt` | `a7dabb5a68` | `a7dabb5a68` | ✅ |
| 181 | `health-monitor` | `tasks/finalpool/health-monitor/initial_workspace/readme.txt` | `3c1c546d8e` | `3c1c546d8e` | ✅ |
| 182 | `health-monitor` | `tasks/finalpool/health-monitor/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 183 | `help-desk` | `tasks/finalpool/help-desk/docs/agent_system_prompt.md` | `10fab205db` | `10fab205db` | ✅ |
| 184 | `help-desk` | `tasks/finalpool/help-desk/docs/task.md` | `75b6b54d90` | `75b6b54d90` | ✅ |
| 185 | `help-desk` | `tasks/finalpool/help-desk/docs/user_system_prompt.md` | `fb10b29717` | `fb10b29717` | ✅ |
| 186 | `help-desk` | `tasks/finalpool/help-desk/evaluation/main.py` | `6e609f0e62` | `6e609f0e62` | ✅ |
| 187 | `help-desk` | `tasks/finalpool/help-desk/groundtruth_workspace/readme.txt` | `a0b36c00ab` | `a0b36c00ab` | ✅ |
| 188 | `help-desk` | `tasks/finalpool/help-desk/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 189 | `image-processor` | `tasks/finalpool/image-processor/docs/agent_system_prompt.md` | `c738b9ebe1` | `c738b9ebe1` | ✅ |
| 190 | `image-processor` | `tasks/finalpool/image-processor/docs/task.md` | `6f13328b18` | `6f13328b18` | ✅ |
| 191 | `image-processor` | `tasks/finalpool/image-processor/docs/user_system_prompt.md` | `bbbda1442d` | `bbbda1442d` | ✅ |
| 192 | `image-processor` | `tasks/finalpool/image-processor/evaluation/main.py` | `1c08806918` | `1c08806918` | ✅ |
| 193 | `image-processor` | `tasks/finalpool/image-processor/initial_workspace/readme.txt` | `72e4d93956` | `72e4d93956` | ✅ |
| 194 | `image-processor` | `tasks/finalpool/image-processor/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 195 | `inventory-management` | `tasks/finalpool/inventory-management/docs/agent_system_prompt.md` | `56ee0a61c6` | `56ee0a61c6` | ✅ |
| 196 | `inventory-management` | `tasks/finalpool/inventory-management/docs/task.md` | `a07413add4` | `a07413add4` | ✅ |
| 197 | `inventory-management` | `tasks/finalpool/inventory-management/evaluation/main.py` | `640d082192` | `640d082192` | ✅ |
| 198 | `inventory-management` | `tasks/finalpool/inventory-management/groundtruth_workspace/readme.txt` | `4cf94c012f` | `4cf94c012f` | ✅ |
| 199 | `invoice-generator` | `tasks/finalpool/invoice-generator/docs/agent_system_prompt.md` | `c293d75e1e` | `c293d75e1e` | ✅ |
| 200 | `invoice-generator` | `tasks/finalpool/invoice-generator/docs/task.md` | `a474010b52` | `a474010b52` | ✅ |
| 201 | `invoice-generator` | `tasks/finalpool/invoice-generator/evaluation/main.py` | `3ee457d91f` | `3ee457d91f` | ✅ |
| 202 | `invoice-generator` | `tasks/finalpool/invoice-generator/initial_workspace/readme.txt` | `440f4424b1` | `440f4424b1` | ✅ |
| 203 | `load-balancer` | `tasks/finalpool/load-balancer/docs/agent_system_prompt.md` | `1c2b01c279` | `1c2b01c279` | ✅ |
| 204 | `load-balancer` | `tasks/finalpool/load-balancer/docs/task.md` | `7c0a385ca9` | `7c0a385ca9` | ✅ |
| 205 | `load-balancer` | `tasks/finalpool/load-balancer/evaluation/main.py` | `d052e55c9b` | `d052e55c9b` | ✅ |
| 206 | `load-balancer` | `tasks/finalpool/load-balancer/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 207 | `log-analyzer` | `tasks/finalpool/log-analyzer/docs/agent_system_prompt.md` | `787cac4c94` | `787cac4c94` | ✅ |
| 208 | `log-analyzer` | `tasks/finalpool/log-analyzer/docs/task.md` | `c1c6f84f98` | `c1c6f84f98` | ✅ |
| 209 | `log-analyzer` | `tasks/finalpool/log-analyzer/evaluation/main.py` | `9f2e006a08` | `9f2e006a08` | ✅ |
| 210 | `log-analyzer` | `tasks/finalpool/log-analyzer/initial_workspace/readme.txt` | `beee2d168a` | `beee2d168a` | ✅ |
| 211 | `log-analyzer` | `tasks/finalpool/log-analyzer/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 212 | `loyalty-program` | `tasks/finalpool/loyalty-program/docs/agent_system_prompt.md` | `6c9e7dd708` | `6c9e7dd708` | ✅ |
| 213 | `loyalty-program` | `tasks/finalpool/loyalty-program/docs/task.md` | `1eff915fad` | `1eff915fad` | ✅ |
| 214 | `loyalty-program` | `tasks/finalpool/loyalty-program/docs/user_system_prompt.md` | `a1414b9ada` | `a1414b9ada` | ✅ |
| 215 | `loyalty-program` | `tasks/finalpool/loyalty-program/evaluation/main.py` | `54242173a1` | `54242173a1` | ✅ |
| 216 | `loyalty-program` | `tasks/finalpool/loyalty-program/groundtruth_workspace/readme.txt` | `8b17eba8a7` | `8b17eba8a7` | ✅ |
| 217 | `media-organizer` | `tasks/finalpool/media-organizer/docs/agent_system_prompt.md` | `c0a5ad88b8` | `c0a5ad88b8` | ✅ |
| 218 | `media-organizer` | `tasks/finalpool/media-organizer/docs/task.md` | `52a6dba315` | `52a6dba315` | ✅ |
| 219 | `media-organizer` | `tasks/finalpool/media-organizer/docs/user_system_prompt.md` | `189aa16b1b` | `189aa16b1b` | ✅ |
| 220 | `media-organizer` | `tasks/finalpool/media-organizer/evaluation/main.py` | `5c84a130d7` | `5c84a130d7` | ✅ |
| 221 | `media-organizer` | `tasks/finalpool/media-organizer/groundtruth_workspace/readme.txt` | `312aa3e471` | `312aa3e471` | ✅ |
| 222 | `media-organizer` | `tasks/finalpool/media-organizer/initial_workspace/readme.txt` | `7706b80b1b` | `7706b80b1b` | ✅ |
| 223 | `media-organizer` | `tasks/finalpool/media-organizer/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 224 | `monitoring-agent` | `tasks/finalpool/monitoring-agent/docs/agent_system_prompt.md` | `f1d59a5d39` | `f1d59a5d39` | ✅ |
| 225 | `monitoring-agent` | `tasks/finalpool/monitoring-agent/docs/task.md` | `eece2322fe` | `eece2322fe` | ✅ |
| 226 | `monitoring-agent` | `tasks/finalpool/monitoring-agent/evaluation/main.py` | `3363334252` | `3363334252` | ✅ |
| 227 | `monitoring-agent` | `tasks/finalpool/monitoring-agent/groundtruth_workspace/readme.txt` | `34bcbbe1f6` | `34bcbbe1f6` | ✅ |
| 228 | `monitoring-agent` | `tasks/finalpool/monitoring-agent/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 229 | `network-analyzer` | `tasks/finalpool/network-analyzer/docs/agent_system_prompt.md` | `69f6a79bc9` | `69f6a79bc9` | ✅ |
| 230 | `network-analyzer` | `tasks/finalpool/network-analyzer/docs/task.md` | `474295ab9a` | `474295ab9a` | ✅ |
| 231 | `network-analyzer` | `tasks/finalpool/network-analyzer/evaluation/main.py` | `38306e8f69` | `38306e8f69` | ✅ |
| 232 | `order-processor` | `tasks/finalpool/order-processor/docs/agent_system_prompt.md` | `551b266784` | `551b266784` | ✅ |
| 233 | `order-processor` | `tasks/finalpool/order-processor/docs/task.md` | `80c3094dc4` | `80c3094dc4` | ✅ |
| 234 | `order-processor` | `tasks/finalpool/order-processor/evaluation/main.py` | `d7be8a2707` | `d7be8a2707` | ✅ |
| 235 | `order-processor` | `tasks/finalpool/order-processor/initial_workspace/readme.txt` | `9bc4c8c2f5` | `9bc4c8c2f5` | ✅ |
| 236 | `payment-processor` | `tasks/finalpool/payment-processor/docs/agent_system_prompt.md` | `2dac5ae103` | `2dac5ae103` | ✅ |
| 237 | `payment-processor` | `tasks/finalpool/payment-processor/docs/task.md` | `7ab01099d7` | `7ab01099d7` | ✅ |
| 238 | `payment-processor` | `tasks/finalpool/payment-processor/docs/user_system_prompt.md` | `fadb1bca67` | `fadb1bca67` | ✅ |
| 239 | `payment-processor` | `tasks/finalpool/payment-processor/evaluation/main.py` | `7b815ec12e` | `7b815ec12e` | ✅ |
| 240 | `payment-processor` | `tasks/finalpool/payment-processor/groundtruth_workspace/readme.txt` | `f0bbd0d0a6` | `f0bbd0d0a6` | ✅ |
| 241 | `pdf-report-generator` | `tasks/finalpool/pdf-report-generator/docs/agent_system_prompt.md` | `62db8dc075` | `62db8dc075` | ✅ |
| 242 | `pdf-report-generator` | `tasks/finalpool/pdf-report-generator/docs/task.md` | `2b55c6adc7` | `2b55c6adc7` | ✅ |
| 243 | `pdf-report-generator` | `tasks/finalpool/pdf-report-generator/docs/user_system_prompt.md` | `1c02cf84b8` | `1c02cf84b8` | ✅ |
| 244 | `pdf-report-generator` | `tasks/finalpool/pdf-report-generator/evaluation/main.py` | `d81995c4d2` | `d81995c4d2` | ✅ |
| 245 | `pdf-report-generator` | `tasks/finalpool/pdf-report-generator/groundtruth_workspace/readme.txt` | `11350ab189` | `11350ab189` | ✅ |
| 246 | `pdf-report-generator` | `tasks/finalpool/pdf-report-generator/initial_workspace/readme.txt` | `62aa6c0fa7` | `62aa6c0fa7` | ✅ |
| 247 | `permission-manager` | `tasks/finalpool/permission-manager/docs/agent_system_prompt.md` | `6ea4a757b1` | `6ea4a757b1` | ✅ |
| 248 | `permission-manager` | `tasks/finalpool/permission-manager/docs/task.md` | `fc0d74d29f` | `fc0d74d29f` | ✅ |
| 249 | `permission-manager` | `tasks/finalpool/permission-manager/evaluation/main.py` | `30f2138eb4` | `30f2138eb4` | ✅ |
| 250 | `permission-manager` | `tasks/finalpool/permission-manager/initial_workspace/readme.txt` | `01a1d34589` | `01a1d34589` | ✅ |
| 251 | `permission-manager` | `tasks/finalpool/permission-manager/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 252 | `personalization-service` | `tasks/finalpool/personalization-service/docs/agent_system_prompt.md` | `a5a746fd57` | `a5a746fd57` | ✅ |
| 253 | `personalization-service` | `tasks/finalpool/personalization-service/docs/task.md` | `6bdbf2bd28` | `6bdbf2bd28` | ✅ |
| 254 | `personalization-service` | `tasks/finalpool/personalization-service/evaluation/main.py` | `75683b4a6b` | `75683b4a6b` | ✅ |
| 255 | `personalization-service` | `tasks/finalpool/personalization-service/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 256 | `price-tracker` | `tasks/finalpool/price-tracker/docs/agent_system_prompt.md` | `4d38c4f2c9` | `4d38c4f2c9` | ✅ |
| 257 | `price-tracker` | `tasks/finalpool/price-tracker/docs/task.md` | `66908fff53` | `66908fff53` | ✅ |
| 258 | `price-tracker` | `tasks/finalpool/price-tracker/evaluation/main.py` | `b6c6f37202` | `b6c6f37202` | ✅ |
| 259 | `price-tracker` | `tasks/finalpool/price-tracker/groundtruth_workspace/readme.txt` | `1617067aea` | `1617067aea` | ✅ |
| 260 | `product-catalog` | `tasks/finalpool/product-catalog/docs/agent_system_prompt.md` | `d3a114a359` | `d3a114a359` | ✅ |
| 261 | `product-catalog` | `tasks/finalpool/product-catalog/docs/task.md` | `c246972a18` | `c246972a18` | ✅ |
| 262 | `product-catalog` | `tasks/finalpool/product-catalog/docs/user_system_prompt.md` | `b8e7ce47c5` | `b8e7ce47c5` | ✅ |
| 263 | `product-catalog` | `tasks/finalpool/product-catalog/evaluation/main.py` | `aa5ad4fee1` | `aa5ad4fee1` | ✅ |
| 264 | `product-catalog` | `tasks/finalpool/product-catalog/groundtruth_workspace/readme.txt` | `15a9147f45` | `15a9147f45` | ✅ |
| 265 | `product-catalog` | `tasks/finalpool/product-catalog/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 266 | `qr-generator` | `tasks/finalpool/qr-generator/docs/agent_system_prompt.md` | `8db26807ba` | `8db26807ba` | ✅ |
| 267 | `qr-generator` | `tasks/finalpool/qr-generator/docs/task.md` | `2b426d9a79` | `2b426d9a79` | ✅ |
| 268 | `qr-generator` | `tasks/finalpool/qr-generator/docs/user_system_prompt.md` | `e90d40478f` | `e90d40478f` | ✅ |
| 269 | `qr-generator` | `tasks/finalpool/qr-generator/evaluation/main.py` | `c973acb75e` | `c973acb75e` | ✅ |
| 270 | `qr-generator` | `tasks/finalpool/qr-generator/groundtruth_workspace/readme.txt` | `c732c9722d` | `c732c9722d` | ✅ |
| 271 | `qr-generator` | `tasks/finalpool/qr-generator/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 272 | `reminder-service` | `tasks/finalpool/reminder-service/docs/agent_system_prompt.md` | `e445c597a9` | `e445c597a9` | ✅ |
| 273 | `reminder-service` | `tasks/finalpool/reminder-service/docs/task.md` | `6d1f79bc7d` | `6d1f79bc7d` | ✅ |
| 274 | `reminder-service` | `tasks/finalpool/reminder-service/evaluation/main.py` | `463abec43d` | `463abec43d` | ✅ |
| 275 | `reminder-service` | `tasks/finalpool/reminder-service/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 276 | `robots-handler` | `tasks/finalpool/robots-handler/docs/agent_system_prompt.md` | `652e53d9c9` | `652e53d9c9` | ✅ |
| 277 | `robots-handler` | `tasks/finalpool/robots-handler/docs/task.md` | `8d146caf47` | `8d146caf47` | ✅ |
| 278 | `robots-handler` | `tasks/finalpool/robots-handler/docs/user_system_prompt.md` | `42b2943ce2` | `42b2943ce2` | ✅ |
| 279 | `robots-handler` | `tasks/finalpool/robots-handler/evaluation/main.py` | `e3d977afa8` | `e3d977afa8` | ✅ |
| 280 | `robots-handler` | `tasks/finalpool/robots-handler/groundtruth_workspace/readme.txt` | `66479d87a3` | `66479d87a3` | ✅ |
| 281 | `robots-handler` | `tasks/finalpool/robots-handler/initial_workspace/readme.txt` | `e15fb47910` | `e15fb47910` | ✅ |
| 282 | `robots-handler` | `tasks/finalpool/robots-handler/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 283 | `sales-pipeline` | `tasks/finalpool/sales-pipeline/docs/agent_system_prompt.md` | `2dd7a0dc2d` | `2dd7a0dc2d` | ✅ |
| 284 | `sales-pipeline` | `tasks/finalpool/sales-pipeline/docs/task.md` | `683835d028` | `683835d028` | ✅ |
| 285 | `sales-pipeline` | `tasks/finalpool/sales-pipeline/evaluation/main.py` | `bef059eca8` | `bef059eca8` | ✅ |
| 286 | `scheduler` | `tasks/finalpool/scheduler/docs/agent_system_prompt.md` | `edbe02a2f2` | `edbe02a2f2` | ✅ |
| 287 | `scheduler` | `tasks/finalpool/scheduler/docs/task.md` | `7d1a8c3db4` | `7d1a8c3db4` | ✅ |
| 288 | `scheduler` | `tasks/finalpool/scheduler/docs/user_system_prompt.md` | `5868c08845` | `5868c08845` | ✅ |
| 289 | `scheduler` | `tasks/finalpool/scheduler/evaluation/main.py` | `c389fb2e3a` | `c389fb2e3a` | ✅ |
| 290 | `scheduler` | `tasks/finalpool/scheduler/initial_workspace/readme.txt` | `d6508ec045` | `d6508ec045` | ✅ |
| 291 | `search-engine` | `tasks/finalpool/search-engine/docs/agent_system_prompt.md` | `ee8bd1152a` | `ee8bd1152a` | ✅ |
| 292 | `search-engine` | `tasks/finalpool/search-engine/docs/task.md` | `373d85d588` | `373d85d588` | ✅ |
| 293 | `search-engine` | `tasks/finalpool/search-engine/docs/user_system_prompt.md` | `920bda31ec` | `920bda31ec` | ✅ |
| 294 | `search-engine` | `tasks/finalpool/search-engine/evaluation/main.py` | `2bbc1fbf45` | `2bbc1fbf45` | ✅ |
| 295 | `search-engine` | `tasks/finalpool/search-engine/groundtruth_workspace/readme.txt` | `3a498c55ca` | `3a498c55ca` | ✅ |
| 296 | `search-engine` | `tasks/finalpool/search-engine/initial_workspace/readme.txt` | `82aad23677` | `82aad23677` | ✅ |
| 297 | `search-engine` | `tasks/finalpool/search-engine/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 298 | `security-scanner` | `tasks/finalpool/security-scanner/docs/agent_system_prompt.md` | `e745356d49` | `e745356d49` | ✅ |
| 299 | `security-scanner` | `tasks/finalpool/security-scanner/docs/task.md` | `1199f9a904` | `1199f9a904` | ✅ |
| 300 | `security-scanner` | `tasks/finalpool/security-scanner/evaluation/main.py` | `aa598887d3` | `aa598887d3` | ✅ |
| 301 | `security-scanner` | `tasks/finalpool/security-scanner/groundtruth_workspace/readme.txt` | `8c0812f9ac` | `8c0812f9ac` | ✅ |
| 302 | `security-scanner` | `tasks/finalpool/security-scanner/initial_workspace/readme.txt` | `7811929633` | `7811929633` | ✅ |
| 303 | `sentiment-analyzer` | `tasks/finalpool/sentiment-analyzer/docs/agent_system_prompt.md` | `15552e6fa7` | `15552e6fa7` | ✅ |
| 304 | `sentiment-analyzer` | `tasks/finalpool/sentiment-analyzer/docs/task.md` | `8fae54191c` | `8fae54191c` | ✅ |
| 305 | `sentiment-analyzer` | `tasks/finalpool/sentiment-analyzer/evaluation/main.py` | `e1d8d5a33a` | `e1d8d5a33a` | ✅ |
| 306 | `sentiment-analyzer` | `tasks/finalpool/sentiment-analyzer/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 307 | `shipment-tracker` | `tasks/finalpool/shipment-tracker/docs/agent_system_prompt.md` | `8ffb5d89c3` | `8ffb5d89c3` | ✅ |
| 308 | `shipment-tracker` | `tasks/finalpool/shipment-tracker/docs/task.md` | `514db2bd7b` | `514db2bd7b` | ✅ |
| 309 | `shipment-tracker` | `tasks/finalpool/shipment-tracker/evaluation/main.py` | `62b0f5dee4` | `62b0f5dee4` | ✅ |
| 310 | `social-connector` | `tasks/finalpool/social-connector/docs/agent_system_prompt.md` | `6677eb21c0` | `6677eb21c0` | ✅ |
| 311 | `social-connector` | `tasks/finalpool/social-connector/docs/task.md` | `556cef93dc` | `556cef93dc` | ✅ |
| 312 | `social-connector` | `tasks/finalpool/social-connector/docs/user_system_prompt.md` | `4ac3b3bce4` | `4ac3b3bce4` | ✅ |
| 313 | `social-connector` | `tasks/finalpool/social-connector/evaluation/main.py` | `f7a497dc80` | `f7a497dc80` | ✅ |
| 314 | `social-connector` | `tasks/finalpool/social-connector/groundtruth_workspace/readme.txt` | `507f1bb35e` | `507f1bb35e` | ✅ |
| 315 | `social-connector` | `tasks/finalpool/social-connector/initial_workspace/readme.txt` | `6e3d26684d` | `6e3d26684d` | ✅ |
| 316 | `social-connector` | `tasks/finalpool/social-connector/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 317 | `social-publisher` | `tasks/finalpool/social-publisher/docs/agent_system_prompt.md` | `9cd9ceb6a1` | `9cd9ceb6a1` | ✅ |
| 318 | `social-publisher` | `tasks/finalpool/social-publisher/docs/task.md` | `de9b502f70` | `de9b502f70` | ✅ |
| 319 | `social-publisher` | `tasks/finalpool/social-publisher/evaluation/main.py` | `9afe0bc2d3` | `9afe0bc2d3` | ✅ |
| 320 | `social-publisher` | `tasks/finalpool/social-publisher/initial_workspace/readme.txt` | `a85c0f309a` | `a85c0f309a` | ✅ |
| 321 | `social-publisher` | `tasks/finalpool/social-publisher/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 322 | `status-checker` | `tasks/finalpool/status-checker/docs/agent_system_prompt.md` | `b36bad0d78` | `b36bad0d78` | ✅ |
| 323 | `status-checker` | `tasks/finalpool/status-checker/docs/task.md` | `101ffe053a` | `101ffe053a` | ✅ |
| 324 | `status-checker` | `tasks/finalpool/status-checker/docs/user_system_prompt.md` | `a9306a9758` | `a9306a9758` | ✅ |
| 325 | `status-checker` | `tasks/finalpool/status-checker/evaluation/main.py` | `c2ba975d4a` | `c2ba975d4a` | ✅ |
| 326 | `status-checker` | `tasks/finalpool/status-checker/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 327 | `storage-manager` | `tasks/finalpool/storage-manager/docs/agent_system_prompt.md` | `d83b07e5e0` | `d83b07e5e0` | ✅ |
| 328 | `storage-manager` | `tasks/finalpool/storage-manager/docs/task.md` | `3534c551a2` | `3534c551a2` | ✅ |
| 329 | `storage-manager` | `tasks/finalpool/storage-manager/evaluation/main.py` | `9638a4f0c6` | `9638a4f0c6` | ✅ |
| 330 | `streaming-service` | `tasks/finalpool/streaming-service/docs/agent_system_prompt.md` | `5b6e38e19b` | `5b6e38e19b` | ✅ |
| 331 | `streaming-service` | `tasks/finalpool/streaming-service/docs/task.md` | `0a07c6b347` | `0a07c6b347` | ✅ |
| 332 | `streaming-service` | `tasks/finalpool/streaming-service/docs/user_system_prompt.md` | `321dc50395` | `321dc50395` | ✅ |
| 333 | `streaming-service` | `tasks/finalpool/streaming-service/evaluation/main.py` | `454d9cfac1` | `454d9cfac1` | ✅ |
| 334 | `streaming-service` | `tasks/finalpool/streaming-service/groundtruth_workspace/readme.txt` | `0fc39c49c7` | `0fc39c49c7` | ✅ |
| 335 | `subtitle-generator` | `tasks/finalpool/subtitle-generator/docs/agent_system_prompt.md` | `c966720ba6` | `c966720ba6` | ✅ |
| 336 | `subtitle-generator` | `tasks/finalpool/subtitle-generator/docs/task.md` | `650b51bb51` | `650b51bb51` | ✅ |
| 337 | `subtitle-generator` | `tasks/finalpool/subtitle-generator/docs/user_system_prompt.md` | `87759b2757` | `87759b2757` | ✅ |
| 338 | `subtitle-generator` | `tasks/finalpool/subtitle-generator/evaluation/main.py` | `f79bcbb1b0` | `f79bcbb1b0` | ✅ |
| 339 | `subtitle-generator` | `tasks/finalpool/subtitle-generator/groundtruth_workspace/readme.txt` | `76df0c8ad9` | `76df0c8ad9` | ✅ |
| 340 | `subtitle-generator` | `tasks/finalpool/subtitle-generator/initial_workspace/readme.txt` | `83a4d84b90` | `83a4d84b90` | ✅ |
| 341 | `survey-builder` | `tasks/finalpool/survey-builder/docs/agent_system_prompt.md` | `435baa2f8a` | `435baa2f8a` | ✅ |
| 342 | `survey-builder` | `tasks/finalpool/survey-builder/docs/task.md` | `fcca3086fd` | `fcca3086fd` | ✅ |
| 343 | `survey-builder` | `tasks/finalpool/survey-builder/evaluation/main.py` | `520d991dce` | `520d991dce` | ✅ |
| 344 | `survey-builder` | `tasks/finalpool/survey-builder/initial_workspace/readme.txt` | `f638bdb4d0` | `f638bdb4d0` | ✅ |
| 345 | `sync-service` | `tasks/finalpool/sync-service/docs/agent_system_prompt.md` | `e1c110f16b` | `e1c110f16b` | ✅ |
| 346 | `sync-service` | `tasks/finalpool/sync-service/docs/task.md` | `802dec9816` | `802dec9816` | ✅ |
| 347 | `sync-service` | `tasks/finalpool/sync-service/docs/user_system_prompt.md` | `394e058bf8` | `394e058bf8` | ✅ |
| 348 | `sync-service` | `tasks/finalpool/sync-service/evaluation/main.py` | `af455e2de5` | `af455e2de5` | ✅ |
| 349 | `sync-service` | `tasks/finalpool/sync-service/initial_workspace/readme.txt` | `070a1eb940` | `070a1eb940` | ✅ |
| 350 | `tag-manager` | `tasks/finalpool/tag-manager/docs/agent_system_prompt.md` | `3eacf7cb43` | `3eacf7cb43` | ✅ |
| 351 | `tag-manager` | `tasks/finalpool/tag-manager/docs/task.md` | `f555002f3b` | `f555002f3b` | ✅ |
| 352 | `tag-manager` | `tasks/finalpool/tag-manager/docs/user_system_prompt.md` | `34c7f0234d` | `34c7f0234d` | ✅ |
| 353 | `tag-manager` | `tasks/finalpool/tag-manager/evaluation/main.py` | `8bd4e95aff` | `8bd4e95aff` | ✅ |
| 354 | `tag-manager` | `tasks/finalpool/tag-manager/groundtruth_workspace/readme.txt` | `f3729197b2` | `f3729197b2` | ✅ |
| 355 | `tag-manager` | `tasks/finalpool/tag-manager/initial_workspace/readme.txt` | `76e79ade64` | `76e79ade64` | ✅ |
| 356 | `tag-manager` | `tasks/finalpool/tag-manager/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 357 | `task-scheduler` | `tasks/finalpool/task-scheduler/docs/agent_system_prompt.md` | `a23389721f` | `a23389721f` | ✅ |
| 358 | `task-scheduler` | `tasks/finalpool/task-scheduler/docs/task.md` | `0df5feb41d` | `0df5feb41d` | ✅ |
| 359 | `task-scheduler` | `tasks/finalpool/task-scheduler/evaluation/main.py` | `07f1544b37` | `07f1544b37` | ✅ |
| 360 | `template-engine` | `tasks/finalpool/template-engine/docs/agent_system_prompt.md` | `f8ebcb9a75` | `f8ebcb9a75` | ✅ |
| 361 | `template-engine` | `tasks/finalpool/template-engine/docs/task.md` | `639da1accc` | `639da1accc` | ✅ |
| 362 | `template-engine` | `tasks/finalpool/template-engine/evaluation/main.py` | `e8fc0443db` | `e8fc0443db` | ✅ |
| 363 | `territory-manager` | `tasks/finalpool/territory-manager/docs/agent_system_prompt.md` | `08376b399e` | `08376b399e` | ✅ |
| 364 | `territory-manager` | `tasks/finalpool/territory-manager/docs/task.md` | `ab21f2198d` | `ab21f2198d` | ✅ |
| 365 | `territory-manager` | `tasks/finalpool/territory-manager/docs/user_system_prompt.md` | `0fbe596d34` | `0fbe596d34` | ✅ |
| 366 | `territory-manager` | `tasks/finalpool/territory-manager/evaluation/main.py` | `1b0b35268d` | `1b0b35268d` | ✅ |
| 367 | `territory-manager` | `tasks/finalpool/territory-manager/groundtruth_workspace/readme.txt` | `74cde9fbcb` | `74cde9fbcb` | ✅ |
| 368 | `translation-api` | `tasks/finalpool/translation-api/docs/agent_system_prompt.md` | `0f764f4347` | `0f764f4347` | ✅ |
| 369 | `translation-api` | `tasks/finalpool/translation-api/docs/task.md` | `6e1f7dbd9f` | `6e1f7dbd9f` | ✅ |
| 370 | `translation-api` | `tasks/finalpool/translation-api/evaluation/main.py` | `9393c988c7` | `9393c988c7` | ✅ |
| 371 | `translation-api` | `tasks/finalpool/translation-api/initial_workspace/readme.txt` | `66f7f8d2aa` | `66f7f8d2aa` | ✅ |
| 372 | `translation-api` | `tasks/finalpool/translation-api/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 373 | `video-trimmer` | `tasks/finalpool/video-trimmer/docs/agent_system_prompt.md` | `61294abce5` | `61294abce5` | ✅ |
| 374 | `video-trimmer` | `tasks/finalpool/video-trimmer/docs/task.md` | `4175bc67f1` | `4175bc67f1` | ✅ |
| 375 | `video-trimmer` | `tasks/finalpool/video-trimmer/evaluation/main.py` | `16da2f5707` | `16da2f5707` | ✅ |
| 376 | `video-trimmer` | `tasks/finalpool/video-trimmer/initial_workspace/readme.txt` | `fe2b540b9b` | `fe2b540b9b` | ✅ |
| 377 | `voice-processor` | `tasks/finalpool/voice-processor/docs/agent_system_prompt.md` | `18f5747c45` | `18f5747c45` | ✅ |
| 378 | `voice-processor` | `tasks/finalpool/voice-processor/docs/task.md` | `4a07ed7213` | `4a07ed7213` | ✅ |
| 379 | `voice-processor` | `tasks/finalpool/voice-processor/docs/user_system_prompt.md` | `93cadbb437` | `93cadbb437` | ✅ |
| 380 | `voice-processor` | `tasks/finalpool/voice-processor/evaluation/main.py` | `2e91016fe6` | `2e91016fe6` | ✅ |
| 381 | `voice-processor` | `tasks/finalpool/voice-processor/preprocess/main.py` | `9b394352ca` | `9b394352ca` | ✅ |
| 382 | `web-crawler` | `tasks/finalpool/web-crawler/docs/agent_system_prompt.md` | `22e9cf6d87` | `22e9cf6d87` | ✅ |
| 383 | `web-crawler` | `tasks/finalpool/web-crawler/docs/task.md` | `a800d698b1` | `a800d698b1` | ✅ |
| 384 | `web-crawler` | `tasks/finalpool/web-crawler/evaluation/main.py` | `7a023f673f` | `7a023f673f` | ✅ |
| 385 | `web-crawler` | `tasks/finalpool/web-crawler/initial_workspace/readme.txt` | `ccd7abdb50` | `ccd7abdb50` | ✅ |

---

## Task Inventory (full_scope.csv source of truth)

| # | Task Name | Source Branch | Source Dev | Files |
|---|-----------|---------------|------------|-------|
| 1 | `activity-logger` | `lueyang-dev` | `lueyang` | 5 |
| 2 | `alert-system` | `yuzhen-dev` | `yuzhen` | 5 |
| 3 | `analytics-dashboard` | `lv` | `lv` | 4 |
| 4 | `asset-optimizer` | `yuxuan-dev` | `yuxuan` | 5 |
| 5 | `backup-utility` | `xiaochen_dev` | `xiaochen` | 4 |
| 6 | `blog-engine` | `gyy` | `gyy` | 6 |
| 7 | `booking-system` | `junteng_dev` | `junteng` | 7 |
| 8 | `cache-optimizer` | `wenshuo-dev` | `wenshuo` | 4 |
| 9 | `calendar-sync` | `junteng_dev` | `junteng` | 6 |
| 10 | `canvas-automation` | `ruige` | `ruige` | 5 |
| 11 | `canvas-grade-automation` | `jl_dev` | `jl` | 4 |
| 12 | `certificate-manager` | `zhaochen` | `zhaochen` | 3 |
| 13 | `chat-bot` | `lv` | `lv` | 6 |
| 14 | `client-portal` | `lueyang-dev` | `lueyang` | 7 |
| 15 | `cms-builder` | `gyy` | `gyy` | 7 |
| 16 | `contact-manager` | `junteng_dev` | `junteng` | 6 |
| 17 | `content-manager` | `yuxuan-dev` | `yuxuan` | 7 |
| 18 | `content-scheduler` | `gyy` | `gyy` | 5 |
| 19 | `coupon-manager` | `fan-dev` | `fan` | 4 |
| 20 | `crm-system` | `lueyang-dev` | `lueyang` | 7 |
| 21 | `customer-feedback-processor` | `jl_dev` | `jl` | 5 |
| 22 | `data-analytics` | `ruige` | `ruige` | 5 |
| 23 | `data-validator` | `yuzhen-dev` | `yuzhen` | 5 |
| 24 | `deal-manager` | `lueyang-dev` | `lueyang` | 5 |
| 25 | `deployment-tool` | `xiaochen_dev` | `xiaochen` | 6 |
| 26 | `discount-calculator` | `fan-dev` | `fan` | 4 |
| 27 | `email-campaign` | `lueyang-dev` | `lueyang` | 6 |
| 28 | `email-classification-system` | `jl_dev` | `jl` | 6 |
| 29 | `error-tracker` | `xiaochen_dev` | `xiaochen` | 5 |
| 30 | `expense-tracker` | `ruige` | `ruige` | 5 |
| 31 | `feedback-collector` | `lv` | `lv` | 5 |
| 32 | `file-manager` | `ruige` | `ruige` | 4 |
| 33 | `follow-up-reminder` | `lueyang-dev` | `lueyang` | 5 |
| 34 | `form-builder` | `yuzhen-dev` | `yuzhen` | 3 |
| 35 | `health-monitor` | `xiaochen_dev` | `xiaochen` | 6 |
| 36 | `help-desk` | `junteng_dev` | `junteng` | 6 |
| 37 | `image-processor` | `wenshuo-dev` | `wenshuo` | 6 |
| 38 | `inventory-management` | `jl_dev` | `jl` | 4 |
| 39 | `invoice-generator` | `yuzhen-dev` | `yuzhen` | 4 |
| 40 | `load-balancer` | `zhaochen` | `zhaochen` | 4 |
| 41 | `log-analyzer` | `ruige` | `ruige` | 5 |
| 42 | `loyalty-program` | `fan-dev` | `fan` | 5 |
| 43 | `media-organizer` | `haoze` | `haoze` | 7 |
| 44 | `monitoring-agent` | `xiaochen_dev` | `xiaochen` | 5 |
| 45 | `network-analyzer` | `yuxuan-dev` | `yuxuan` | 3 |
| 46 | `order-processor` | `junteng_dev` | `junteng` | 4 |
| 47 | `payment-processor` | `yuzhen-dev` | `yuzhen` | 5 |
| 48 | `pdf-report-generator` | `jl_dev` | `jl` | 6 |
| 49 | `permission-manager` | `yuzhen-dev` | `yuzhen` | 5 |
| 50 | `personalization-service` | `lv` | `lv` | 4 |
| 51 | `price-tracker` | `fan-dev` | `fan` | 4 |
| 52 | `product-catalog` | `junteng_dev` | `junteng` | 6 |
| 53 | `qr-generator` | `junxian_dev` | `junxian` | 6 |
| 54 | `reminder-service` | `junteng_dev` | `junteng` | 4 |
| 55 | `robots-handler` | `gyy` | `gyy` | 7 |
| 56 | `sales-pipeline` | `lueyang-dev` | `lueyang` | 3 |
| 57 | `scheduler` | `wenshuo-dev` | `wenshuo` | 5 |
| 58 | `search-engine` | `wenshuo-dev` | `wenshuo` | 7 |
| 59 | `security-scanner` | `xiaochen_dev` | `xiaochen` | 5 |
| 60 | `sentiment-analyzer` | `lv` | `lv` | 4 |
| 61 | `shipment-tracker` | `junteng_dev` | `junteng` | 3 |
| 62 | `social-connector` | `junxian_dev` | `junxian` | 7 |
| 63 | `social-publisher` | `gyy` | `gyy` | 5 |
| 64 | `status-checker` | `xiaochen_dev` | `xiaochen` | 5 |
| 65 | `storage-manager` | `zhaochen` | `zhaochen` | 3 |
| 66 | `streaming-service` | `haoze` | `haoze` | 5 |
| 67 | `subtitle-generator` | `haoze` | `haoze` | 6 |
| 68 | `survey-builder` | `lv` | `lv` | 4 |
| 69 | `sync-service` | `yuxuan-dev` | `yuxuan` | 5 |
| 70 | `tag-manager` | `gyy` | `gyy` | 7 |
| 71 | `task-scheduler` | `yuxuan-dev` | `yuxuan` | 3 |
| 72 | `template-engine` | `zhaochen` | `zhaochen` | 3 |
| 73 | `territory-manager` | `lueyang-dev` | `lueyang` | 5 |
| 74 | `translation-api` | `junxian_dev` | `junxian` | 5 |
| 75 | `video-trimmer` | `haoze` | `haoze` | 4 |
| 76 | `voice-processor` | `lv` | `lv` | 5 |
| 77 | `web-crawler` | `ruige` | `ruige` | 4 |

---

## Audit Conclusion

```
Scope entries: 385
Live matches:  385
Mismatches:    0
Missing:       0
Extra:         0

RESULT: PASS
```

> The `finalpool` branch live state is in full agreement with `full_scope.csv`.
> Every file's SHA matches its recorded value. No files are missing or unexpected.
