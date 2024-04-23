# Comparing `tmp/alibabacloud_dingtalk-2.0.96.tar.gz` & `tmp/alibabacloud_dingtalk-2.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.96.tar", last modified: Thu Apr 18 04:15:40 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.0.97.tar", last modified: Mon Apr 22 10:35:35 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.0.96.tar` & `alibabacloud_dingtalk-2.0.97.tar`

### file list

```diff
@@ -1,429 +1,429 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/
--rw-r--r--   0 root         (0) root         (0)   121863 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2565 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2650 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8552 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15045 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21346 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23757 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38246 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    50325 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9980 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22974 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58254 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   168107 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12444 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    19284 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25166 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45004 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25682 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26721 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95304 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   142688 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   204138 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   393347 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45240 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    60886 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5222 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4059 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250270 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   651992 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71584 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   101499 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9614 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9792 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161860 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   394680 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27976 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41039 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78198 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   236838 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6044 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71632 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119949 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143706 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   201494 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58616 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   122524 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   334068 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   418722 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21270 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    41482 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33392 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44364 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17934 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30172 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19630 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8944 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14272 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5652 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10226 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   257462 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   615355 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4810 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7215 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32170 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    45878 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   391978 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   499475 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112278 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   148230 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13874 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15755 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56946 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    54091 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    64765 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    80337 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259804 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   315211 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   213190 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   379351 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19496 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   140210 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   190495 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   557050 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   850115 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72708 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113146 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    86294 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120009 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18589 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   378556 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   527163 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161906 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   305557 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17280 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28173 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35856 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52698 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4825 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4965 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10562 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9402 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80133 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   134962 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17059 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18223 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68862 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   119612 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136761 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   208587 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   303006 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   368637 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24693 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33051 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90230 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    89450 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   671658 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   913856 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62348 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152590 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63194 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105975 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91118 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   131540 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9852 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5150 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4229 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16181 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22736 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148979 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   170469 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52227 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    52481 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25614 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    31620 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34360 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42471 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8962 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7167 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89094 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   161460 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77488 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   120360 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56344 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    57967 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29226 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68049 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   265120 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   409387 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17983 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5368 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4409 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43482 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   135300 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   169147 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94300 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   103368 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93324 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   146182 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39248 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44633 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   386598 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   538012 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31508 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25740 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44726 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94517 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   187612 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   346388 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58076 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    94327 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13910 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28049 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70520 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152094 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14284 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15723 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14192 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21167 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13676 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17009 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    77172 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133813 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75904 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   107789 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33103 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40753 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8278 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20146 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66210 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   128063 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5370 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8155 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41320 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42730 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   198336 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413640 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4774 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494302 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   751756 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5452 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4320 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3853 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14206 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-04-18 04:15:40.000000 alibabacloud_dingtalk-2.0.96/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/
+-rw-r--r--   0 root         (0) root         (0)   123399 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2565 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8552 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15045 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21346 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23757 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38246 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    50325 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22974 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58254 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   168107 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    19568 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45004 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25682 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26721 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95304 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   142688 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   204138 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   393347 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45240 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    60886 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5222 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4059 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250270 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   651992 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71584 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   101499 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9614 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161860 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   394680 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27976 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41039 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78198 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   236838 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71632 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119949 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143706 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   201494 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58616 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   122524 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334068 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   418722 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21270 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    41482 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33392 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44364 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17934 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30172 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19630 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14272 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5652 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   257462 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   615355 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4810 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7215 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32170 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    45878 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   391978 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   499475 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112278 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   148230 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13874 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15755 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56946 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    54091 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    64765 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259804 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   315211 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   213190 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   379351 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19496 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   140210 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   190495 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   557050 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   850115 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72708 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113146 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    86294 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120009 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18589 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   378556 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   527163 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   161906 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   305557 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17280 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28173 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35856 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52698 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4825 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10562 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9402 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80133 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   134962 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17059 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18223 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68862 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   119612 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136761 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   208587 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   303006 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   368637 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24693 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33051 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90230 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    89450 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   671658 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   913856 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62348 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152590 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63194 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105975 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91118 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   131540 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4229 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22736 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148979 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   170469 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52227 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    52481 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25614 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    31620 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34360 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42471 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7167 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89094 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   162124 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77488 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   120360 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    56344 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    57967 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29226 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68049 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   265120 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   409387 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17983 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5368 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4409 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43482 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   135300 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   169147 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    94300 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   103368 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93324 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   146182 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39248 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44633 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   386598 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   538012 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31508 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25740 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44726 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94517 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   187612 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   346388 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58076 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    94327 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13910 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28049 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70520 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152094 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14284 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15723 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14192 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21167 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13676 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17009 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77172 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133813 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75904 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   107789 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33103 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40753 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8278 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20146 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66210 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   128063 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5370 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8155 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41320 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42730 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   198336 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413640 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4774 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494302 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   751756 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5452 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3853 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14206 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-04-22 10:35:35.000000 alibabacloud_dingtalk-2.0.97/setup.py
```

### Comparing `alibabacloud_dingtalk-2.0.96/ChangeLog.md` & `alibabacloud_dingtalk-2.0.97/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-04-18 Version: 2.0.96
+- Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-04-15 Version: 2.0.95
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-09 Version: 2.0.94
 - Generated python activity_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-04-02 Version: 2.0.93
```

### Comparing `alibabacloud_dingtalk-2.0.96/LICENSE` & `alibabacloud_dingtalk-2.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/PKG-INFO` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dingtalk
-Version: 2.0.96
+Name: alibabacloud-dingtalk
+Version: 2.0.97
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.96/README-CN.md` & `alibabacloud_dingtalk-2.0.97/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/README.md` & `alibabacloud_dingtalk-2.0.97/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AmdpOrganizationDataPush',
             version='amdp_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/amdp/organizations/datas/push',
+            pathname=f'/v1.0/amdp/organizations/departments/datas/push',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
@@ -255,15 +255,15 @@
             headers=real_headers,
             body=OpenApiUtilClient.parse_to_map(body)
         )
         params = open_api_models.Params(
             action='AmdpOrganizationDataPush',
             version='amdp_1.0',
             protocol='HTTP',
-            pathname=f'/v1.0/amdp/organizations/datas/push',
+            pathname=f'/v1.0/amdp/organizations/departments/datas/push',
             method='POST',
             auth_type='AK',
             style='ROA',
             req_body_type='none',
             body_type='json'
         )
         return TeaCore.from_map(
```

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,20 +250,22 @@
 
 class AmdpJobPositionDataPushRequestParam(TeaModel):
     def __init__(
         self,
         dept_id: str = None,
         dept_leader: str = None,
         is_delete: str = None,
+        leader_dept_id: str = None,
         order_number: str = None,
         user_id: str = None,
     ):
         self.dept_id = dept_id
         self.dept_leader = dept_leader
         self.is_delete = is_delete
+        self.leader_dept_id = leader_dept_id
         self.order_number = order_number
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -274,28 +276,32 @@
         result = dict()
         if self.dept_id is not None:
             result['deptId'] = self.dept_id
         if self.dept_leader is not None:
             result['deptLeader'] = self.dept_leader
         if self.is_delete is not None:
             result['isDelete'] = self.is_delete
+        if self.leader_dept_id is not None:
+            result['leaderDeptId'] = self.leader_dept_id
         if self.order_number is not None:
             result['orderNumber'] = self.order_number
         if self.user_id is not None:
             result['userId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('deptId') is not None:
             self.dept_id = m.get('deptId')
         if m.get('deptLeader') is not None:
             self.dept_leader = m.get('deptLeader')
         if m.get('isDelete') is not None:
             self.is_delete = m.get('isDelete')
+        if m.get('leaderDeptId') is not None:
+            self.leader_dept_id = m.get('leaderDeptId')
         if m.get('orderNumber') is not None:
             self.order_number = m.get('orderNumber')
         if m.get('userId') is not None:
             self.user_id = m.get('userId')
         return self
```

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 
 class OpenUserDTO(TeaModel):
     def __init__(
         self,
         ding_user_id: str = None,
         name: str = None,
         user_uid: str = None,
+        work_no: str = None,
     ):
         self.ding_user_id = ding_user_id
         self.name = name
         self.user_uid = user_uid
+        self.work_no = work_no
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -26,24 +28,28 @@
         result = dict()
         if self.ding_user_id is not None:
             result['dingUserId'] = self.ding_user_id
         if self.name is not None:
             result['name'] = self.name
         if self.user_uid is not None:
             result['userUid'] = self.user_uid
+        if self.work_no is not None:
+            result['workNo'] = self.work_no
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('dingUserId') is not None:
             self.ding_user_id = m.get('dingUserId')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('userUid') is not None:
             self.user_uid = m.get('userUid')
+        if m.get('workNo') is not None:
+            self.work_no = m.get('workNo')
         return self
 
 
 class TitleMention(TeaModel):
     def __init__(
         self,
         length: int = None,
@@ -89,21 +95,23 @@
         self,
         kr_id: str = None,
         progress: int = None,
         status: int = None,
         title: str = None,
         title_mentions: List[TitleMention] = None,
         type: int = None,
+        weight: float = None,
     ):
         self.kr_id = kr_id
         self.progress = progress
         self.status = status
         self.title = title
         self.title_mentions = title_mentions
         self.type = type
+        self.weight = weight
 
     def validate(self):
         if self.title_mentions:
             for k in self.title_mentions:
                 if k:
                     k.validate()
 
@@ -123,14 +131,16 @@
             result['title'] = self.title
         result['titleMentions'] = []
         if self.title_mentions is not None:
             for k in self.title_mentions:
                 result['titleMentions'].append(k.to_map() if k else None)
         if self.type is not None:
             result['type'] = self.type
+        if self.weight is not None:
+            result['weight'] = self.weight
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('krId') is not None:
             self.kr_id = m.get('krId')
         if m.get('progress') is not None:
@@ -142,14 +152,16 @@
         self.title_mentions = []
         if m.get('titleMentions') is not None:
             for k in m.get('titleMentions'):
                 temp_model = TitleMention()
                 self.title_mentions.append(temp_model.from_map(k))
         if m.get('type') is not None:
             self.type = m.get('type')
+        if m.get('weight') is not None:
+            self.weight = m.get('weight')
         return self
 
 
 class OpenPeriodDTO(TeaModel):
     def __init__(
         self,
         end_date: int = None,
@@ -252,23 +264,25 @@
         key_results: List[OpenKeyResultDTO] = None,
         objective_id: str = None,
         period: OpenPeriodDTO = None,
         progress: int = None,
         status: int = None,
         teams: List[OpenTeamDTO] = None,
         title: str = None,
+        weight: float = None,
     ):
         self.executor = executor
         self.key_results = key_results
         self.objective_id = objective_id
         self.period = period
         self.progress = progress
         self.status = status
         self.teams = teams
         self.title = title
+        self.weight = weight
 
     def validate(self):
         if self.executor:
             self.executor.validate()
         if self.key_results:
             for k in self.key_results:
                 if k:
@@ -302,14 +316,16 @@
             result['status'] = self.status
         result['teams'] = []
         if self.teams is not None:
             for k in self.teams:
                 result['teams'].append(k.to_map() if k else None)
         if self.title is not None:
             result['title'] = self.title
+        if self.weight is not None:
+            result['weight'] = self.weight
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('executor') is not None:
             temp_model = OpenUserDTO()
             self.executor = temp_model.from_map(m['executor'])
@@ -330,14 +346,16 @@
         self.teams = []
         if m.get('teams') is not None:
             for k in m.get('teams'):
                 temp_model = OpenTeamDTO()
                 self.teams.append(temp_model.from_map(k))
         if m.get('title') is not None:
             self.title = m.get('title')
+        if m.get('weight') is not None:
+            self.weight = m.get('weight')
         return self
 
 
 class AlignObjectiveHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
```

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.0.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dingtalk
-Version: 2.0.96
+Name: alibabacloud_dingtalk
+Version: 2.0.97
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.0.96/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.0.97/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.0.96/setup.py` & `alibabacloud_dingtalk-2.0.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 18/04/2024
+Created on 22/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

