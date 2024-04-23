# Comparing `tmp/forta_bot_sdk-0.2.2.tar.gz` & `tmp/forta_bot_sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forta_bot_sdk-0.2.2.tar", last modified: Tue Apr  9 10:42:00 2024, max compression
+gzip compressed data, was "forta_bot_sdk-0.2.3.tar", last modified: Tue Apr 23 09:14:19 2024, max compression
```

## Comparing `forta_bot_sdk-0.2.2.tar` & `forta_bot_sdk-0.2.3.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.879994 forta_bot_sdk-0.2.2/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1073 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.2/LICENSE
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      844 2024-04-09 10:42:00.879922 forta_bot_sdk-0.2.2/PKG-INFO
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      118 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.2/README.md
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      103 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.2/pyproject.toml
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      747 2024-04-09 10:42:00.880266 forta_bot_sdk-0.2.2/setup.cfg
--rw-r--r--   0 haseebrabbani   (501) staff       (20)       69 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.2/setup.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.861064 forta_bot_sdk-0.2.2/src/
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.863366 forta_bot_sdk-0.2.2/src/forta_bot_sdk/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2512 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/__init__.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.865622 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      349 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     5098 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/alert.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      994 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/alert_event.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      175 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/alert_subscription.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      305 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/create_alert_event.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1312 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1355 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/get_alert.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     7941 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/get_alerts.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     3114 2024-04-09 10:25:29.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/send_alerts.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.866419 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      265 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1570 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/block.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      479 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/block_event.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      361 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/create_block_event.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      938 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1601 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/get_block_with_transactions.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1236 2024-04-05 11:40:50.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/get_latest_block_number.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.867190 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)       56 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1332 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/cache.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2430 2024-04-09 10:01:39.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     3028 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/disk_cache.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1315 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/get_json_rpc_cache_provider.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1398 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/is_cache_healthy.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     4960 2024-04-05 11:43:22.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/json_rpc_cache.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.868339 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)       71 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1653 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      683 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_alert.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      833 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_block.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      954 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_block_range.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     3757 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_cli_command.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      742 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_transaction.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.869341 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      341 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      144 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/handle_alert.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      182 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/handle_block.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      206 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/handle_transaction.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)       87 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/health_check.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      287 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/initialize.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      145 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/scan_alerts_options.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      419 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/common/scan_evm_options.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     5367 2024-04-08 11:41:16.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/di.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.869881 forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      112 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1908 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/finding.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      143 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/finding_severity.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2147 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/finding_source.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      147 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/finding_type.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.870476 forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      207 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2386 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2267 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/run_handlers_on_alert.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     6369 2024-04-07 07:34:41.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/run_handlers_on_block.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2645 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/run_handlers_on_transaction.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.870817 forta_bot_sdk-0.2.2/src/forta_bot_sdk/health/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)       76 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/health/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      709 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/health/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1554 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/health/run_health_check.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.871688 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      207 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      432 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/constants.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      606 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/decode_jwt.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1690 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1728 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/get_rpc_jwt.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1176 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/get_scanner_jwt.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      566 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/get_token_exchange_url.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2357 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/verify_jwt.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.872429 forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      133 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      511 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     4269 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/get_labels.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1900 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/label.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      130 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/label_entity_type.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      691 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/label_source.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.872975 forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      156 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      496 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2778 2024-04-09 10:33:36.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/filter_logs.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1077 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/get_logs_for_block.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1277 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/log.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.873681 forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      152 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2721 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/constants.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      341 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     9542 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/metrics_helper.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      976 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/metrics_manager.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      150 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/types.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.874333 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      171 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/__init__.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.874678 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/alerts/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)        0 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/alerts/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     3085 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/alerts/get_alerts_for_subscriptions.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     3642 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/alerts/scan_alerts.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)       24 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/constants.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     4170 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/di.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.875170 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/evm/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)        0 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/evm/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      403 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/evm/get_block_time.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     4109 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/evm/get_provider.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     6152 2024-04-08 11:26:35.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/evm/scan_evm.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      431 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/should_stop_on_errors.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1673 2024-04-08 11:25:12.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/should_submit_findings.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.875756 forta_bot_sdk-0.2.2/src/forta_bot_sdk/traces/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      123 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/traces/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      401 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/traces/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1597 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/traces/get_trace_data.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1791 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/traces/trace.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.876527 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      285 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2248 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/create_transaction_event.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      585 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/di.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1147 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/get_transaction_receipt.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      987 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/receipt.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      793 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/transaction.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     3430 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/transaction_event.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.879344 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1663 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/__init__.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      440 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/address.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1189 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/assertions.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2429 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/bloom_filter.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      118 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/file_system.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      102 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/format_exception.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      647 2024-04-09 10:28:54.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_aiohttp_session.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      834 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_bot_id.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      198 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_bot_owner.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      578 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_chain_id.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      755 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_forta_api_headers.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      888 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_forta_api_url.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      314 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_forta_chain_id.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2197 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_forta_config.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      375 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_json_file.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     1080 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/json_encoder.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      686 2024-04-09 10:34:18.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/logger.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      137 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/now.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      198 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/sleep.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      444 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/snake_to_camel_case.py
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     2622 2024-04-08 11:30:03.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/with_retry.py
-drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-09 10:42:00.879544 forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      844 2024-04-09 10:42:00.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/PKG-INFO
--rw-r--r--   0 haseebrabbani   (501) staff       (20)     5211 2024-04-09 10:42:00.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 haseebrabbani   (501) staff       (20)        1 2024-04-09 10:42:00.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 haseebrabbani   (501) staff       (20)      119 2024-04-09 10:42:00.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/requires.txt
--rw-r--r--   0 haseebrabbani   (501) staff       (20)       14 2024-04-09 10:42:00.000000 forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.334755 forta_bot_sdk-0.2.3/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1073 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.3/LICENSE
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      844 2024-04-23 09:14:19.334669 forta_bot_sdk-0.2.3/PKG-INFO
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      118 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.3/README.md
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      103 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.3/pyproject.toml
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      747 2024-04-23 09:14:19.335048 forta_bot_sdk-0.2.3/setup.cfg
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)       69 2024-01-22 07:36:59.000000 forta_bot_sdk-0.2.3/setup.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.307530 forta_bot_sdk-0.2.3/src/
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.310171 forta_bot_sdk-0.2.3/src/forta_bot_sdk/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2512 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/__init__.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.313582 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      349 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     5098 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/alert.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      994 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/alert_event.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      175 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/alert_subscription.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      305 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/create_alert_event.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1312 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1355 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/get_alert.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     7941 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/get_alerts.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     3114 2024-04-09 10:25:29.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/send_alerts.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.314872 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      265 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1570 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/block.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      479 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/block_event.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      361 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/create_block_event.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      938 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1601 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/get_block_with_transactions.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1236 2024-04-05 11:40:50.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/get_latest_block_number.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.316456 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)       56 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1332 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/cache.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2430 2024-04-09 10:01:39.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     3028 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/disk_cache.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1315 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/get_json_rpc_cache_provider.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1398 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/is_cache_healthy.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     4960 2024-04-05 11:43:22.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/json_rpc_cache.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.318026 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)       71 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1653 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      683 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_alert.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      833 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_block.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      954 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_block_range.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     3757 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_cli_command.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      742 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_transaction.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.319363 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      341 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      144 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/handle_alert.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      182 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/handle_block.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      206 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/handle_transaction.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)       87 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/health_check.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      287 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/initialize.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      145 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/scan_alerts_options.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      419 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/common/scan_evm_options.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     5367 2024-04-08 11:41:16.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/di.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.320176 forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      112 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1908 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/finding.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      143 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/finding_severity.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2147 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/finding_source.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      147 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/finding_type.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.321273 forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      207 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2386 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2267 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/run_handlers_on_alert.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     6369 2024-04-07 07:34:41.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/run_handlers_on_block.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2645 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/run_handlers_on_transaction.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.321792 forta_bot_sdk-0.2.3/src/forta_bot_sdk/health/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)       76 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/health/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      709 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/health/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1554 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/health/run_health_check.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.323217 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      207 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      432 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/constants.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      606 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/decode_jwt.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1690 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1728 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/get_rpc_jwt.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1176 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/get_scanner_jwt.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      566 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/get_token_exchange_url.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2357 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/verify_jwt.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.324304 forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      133 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      511 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     4269 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/get_labels.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1900 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/label.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      130 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/label_entity_type.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      691 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/label_source.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.325331 forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      156 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      496 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2778 2024-04-09 10:33:36.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/filter_logs.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1077 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/get_logs_for_block.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1277 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/log.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.326479 forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      152 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2721 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/constants.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      341 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     9542 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/metrics_helper.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      976 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/metrics_manager.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      150 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/types.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.327470 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      171 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/__init__.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.328046 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/alerts/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)        0 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/alerts/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     3085 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/alerts/get_alerts_for_subscriptions.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     3642 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/alerts/scan_alerts.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)       24 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/constants.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     4170 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/di.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.328852 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/evm/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)        0 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/evm/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      403 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/evm/get_block_time.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     4109 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/evm/get_provider.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     6152 2024-04-08 11:26:35.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/evm/scan_evm.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      431 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/should_stop_on_errors.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1673 2024-04-08 11:25:12.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/should_submit_findings.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.329779 forta_bot_sdk-0.2.3/src/forta_bot_sdk/traces/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      123 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/traces/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      401 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/traces/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1597 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/traces/get_trace_data.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1791 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/traces/trace.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.331134 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      285 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2248 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/create_transaction_event.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      585 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/di.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1147 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/get_transaction_receipt.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      987 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/receipt.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      793 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/transaction.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     3430 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/transaction_event.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.334119 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1667 2024-04-23 09:04:55.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/__init__.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      440 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/address.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1189 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/assertions.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2429 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/bloom_filter.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      118 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/file_system.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      102 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/format_exception.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      647 2024-04-09 10:28:54.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_aiohttp_session.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      834 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_bot_id.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      198 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_bot_owner.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      578 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_chain_id.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      755 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_forta_api_headers.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      888 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_forta_api_url.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      314 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_forta_chain_id.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2197 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_forta_config.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      375 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_json_file.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     1080 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/json_encoder.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      686 2024-04-09 10:34:18.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/logger.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      137 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/now.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      198 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/sleep.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      444 2024-04-04 11:13:57.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/snake_to_camel_case.py
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     2622 2024-04-08 11:30:03.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/with_retry.py
+drwxr-xr-x   0 haseebrabbani   (501) staff       (20)        0 2024-04-23 09:14:19.334343 forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      844 2024-04-23 09:14:19.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)     5211 2024-04-23 09:14:19.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)        1 2024-04-23 09:14:19.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)      119 2024-04-23 09:14:19.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/requires.txt
+-rw-r--r--   0 haseebrabbani   (501) staff       (20)       14 2024-04-23 09:14:19.000000 forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/top_level.txt
```

### Comparing `forta_bot_sdk-0.2.2/LICENSE` & `forta_bot_sdk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/PKG-INFO` & `forta_bot_sdk-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forta_bot_sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Forta Detection Bot Python SDK
 Home-page: https://forta.org/
 Project-URL: Source, https://github.com/forta-network/forta-bot-sdk-v2
 Project-URL: Documentation, https://docs.forta.network/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forta_bot_sdk-0.2.2/setup.cfg` & `forta_bot_sdk-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forta_bot_sdk
-version = 0.2.2
+version = 0.2.3
 description = Forta Detection Bot Python SDK
 url = https://forta.org/
 project_urls = 
 	Source = https://github.com/forta-network/forta-bot-sdk-v2
 	Documentation =  https://docs.forta.network/
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/__init__.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/alert.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/alert.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/alert_event.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/alert_event.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/get_alert.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/get_alert.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/get_alerts.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/get_alerts.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/alerts/send_alerts.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/alerts/send_alerts.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/block.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/block.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/get_block_with_transactions.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/get_block_with_transactions.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/blocks/get_latest_block_number.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/blocks/get_latest_block_number.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/cache.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/cache.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/disk_cache.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/disk_cache.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/get_json_rpc_cache_provider.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/get_json_rpc_cache_provider.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/is_cache_healthy.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/is_cache_healthy.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cache/json_rpc_cache.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cache/json_rpc_cache.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_alert.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_alert.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_block.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_block.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_block_range.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_block_range.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_cli_command.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_cli_command.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/cli/run_transaction.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/cli/run_transaction.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/finding.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/finding.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/findings/finding_source.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/findings/finding_source.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/run_handlers_on_alert.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/run_handlers_on_alert.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/run_handlers_on_block.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/run_handlers_on_block.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/handlers/run_handlers_on_transaction.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/handlers/run_handlers_on_transaction.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/health/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/health/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/health/run_health_check.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/health/run_health_check.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/decode_jwt.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/decode_jwt.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/get_rpc_jwt.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/get_rpc_jwt.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/get_scanner_jwt.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/get_scanner_jwt.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/get_token_exchange_url.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/get_token_exchange_url.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/jwt/verify_jwt.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/jwt/verify_jwt.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/get_labels.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/get_labels.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/label.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/label.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/labels/label_source.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/labels/label_source.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/filter_logs.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/filter_logs.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/get_logs_for_block.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/get_logs_for_block.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/logs/log.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/logs/log.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/constants.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/constants.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/metrics_helper.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/metrics_helper.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/metrics/metrics_manager.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/metrics/metrics_manager.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/alerts/get_alerts_for_subscriptions.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/alerts/get_alerts_for_subscriptions.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/alerts/scan_alerts.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/alerts/scan_alerts.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/evm/get_provider.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/evm/get_provider.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/evm/scan_evm.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/evm/scan_evm.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/scanning/should_submit_findings.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/scanning/should_submit_findings.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/traces/get_trace_data.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/traces/get_trace_data.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/traces/trace.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/traces/trace.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/create_transaction_event.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/create_transaction_event.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/di.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/di.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/get_transaction_receipt.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/get_transaction_receipt.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/receipt.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/receipt.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/transaction.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/transactions/transaction_event.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/transactions/transaction_event.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/__init__.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .json_encoder import JSONEncoder, JSONable
 from .now import now
 from .snake_to_camel_case import snake_to_camel_case
 from .format_exception import format_exception
 
 
 def hex_to_int(val: str | int) -> Optional[int]:
-    if not val:
+    if val is None:
         return None
     if type(val) == int:
         return val
     return int(val, 0)
 
 
 def get_dict_val(d: dict, key: str) -> Optional[Any]:
```

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/assertions.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/assertions.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/bloom_filter.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/bloom_filter.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_aiohttp_session.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_aiohttp_session.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_bot_id.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_bot_id.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_chain_id.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_chain_id.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_forta_api_headers.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_forta_api_headers.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_forta_api_url.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_forta_api_url.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/get_forta_config.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/get_forta_config.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/json_encoder.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/logger.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/logger.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk/utils/with_retry.py` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk/utils/with_retry.py`

 * *Files identical despite different names*

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/PKG-INFO` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forta_bot_sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Forta Detection Bot Python SDK
 Home-page: https://forta.org/
 Project-URL: Source, https://github.com/forta-network/forta-bot-sdk-v2
 Project-URL: Documentation, https://docs.forta.network/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forta_bot_sdk-0.2.2/src/forta_bot_sdk.egg-info/SOURCES.txt` & `forta_bot_sdk-0.2.3/src/forta_bot_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

