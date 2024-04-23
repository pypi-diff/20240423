# Comparing `tmp/jaseci-1.4.2.5.tar.gz` & `tmp/jaseci-1.4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci-1.4.2.5.tar", last modified: Tue Jan  9 16:44:28 2024, max compression
+gzip compressed data, was "jaseci-1.4.2.6.tar", last modified: Tue Apr 23 19:42:44 2024, max compression
```

## Comparing `jaseci-1.4.2.5.tar` & `jaseci-1.4.2.6.tar`

### file list

```diff
@@ -1,218 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.458459 jaseci-1.4.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-09 16:44:28.458459 jaseci-1.4.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.422459 jaseci-1.4.2.5/jaseci/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.426459 jaseci-1.4.2.5/jaseci/cli_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/cli_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16103 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/cli_tools/book_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/cli_tools/jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.426459 jaseci-1.4.2.5/jaseci/cli_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/cli_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/cli_tools/tests/test_jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.426459 jaseci-1.4.2.5/jaseci/extens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.430459 jaseci-1.4.2.5/jaseci/extens/act_lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/jaseci.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/rand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/std.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/stripe.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.430459 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/std_test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_file_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_mail_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_net_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_std.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_std_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_webtool.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_zlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/webtool.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/act_lib/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.434459 jaseci-1.4.2.5/jaseci/extens/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/actions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/alias_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/architype_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/global_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/graph_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5816 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/jac_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/jsorc_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/logger_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/master_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5435 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/super_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.434459 jaseci-1.4.2.5/jaseci/extens/api/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_architype_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_global_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_graph_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_logger_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_object_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_uncommon.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/tests/test_walker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/walker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/api/webhook_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.438459 jaseci-1.4.2.5/jaseci/extens/svc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/elastic_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/kube_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/mail_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/prome_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/redis_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/storage_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/stripe_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/task_svc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/extens/svc/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.438459 jaseci-1.4.2.5/jaseci/jac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.438459 jaseci-1.4.2.5/jaseci/jac/interpreter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/interpreter/architype_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)    67272 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/interpreter/interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9414 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/interpreter/sentinel_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.438459 jaseci-1.4.2.5/jaseci/jac/interpreter/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/interpreter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/interpreter/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/interpreter/walker_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.442459 jaseci-1.4.2.5/jaseci/jac/ir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/ast_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/jac_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.442459 jaseci-1.4.2.5/jaseci/jac/ir/passes/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/ast_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/codegen_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/ir_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/printer_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/pt_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/ir/passes/stats_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jac.g4
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.442459 jaseci-1.4.2.5/jaseci/jac/jac_parse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jac_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34691 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jac_parse/jacLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    29031 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jac_parse/jacListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   334026 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jac_parse/jacParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jac_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.446459 jaseci-1.4.2.5/jaseci/jac/jsci_vm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jsci_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jsci_vm/disasm.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jsci_vm/inst_ptr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jsci_vm/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jsci_vm/op_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.446459 jaseci-1.4.2.5/jaseci/jac/jsci_vm/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jsci_vm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/jsci_vm/tests/test_codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.446459 jaseci-1.4.2.5/jaseci/jac/machine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/machine/jac_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/machine/jac_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/machine/machine_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.446459 jaseci-1.4.2.5/jaseci/jac/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/tests/book_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/tests/test_book.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jac/tests/test_lang_14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.446459 jaseci-1.4.2.5/jaseci/jsorc/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22563 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/jsorc_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/jsorc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/live_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.450459 jaseci-1.4.2.5/jaseci/jsorc/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/manifests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/manifests/database.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   484138 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/manifests/elastic.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    37855 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/manifests/prometheus.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/manifests/redis.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/remote_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.450459 jaseci-1.4.2.5/jaseci/jsorc/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/jsorc/tests/test_jsorc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.454459 jaseci-1.4.2.5/jaseci/prim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/ability.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/architype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/master.py
--rw-r--r--   0 runner    (1001) docker     (127)    18287 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/obj_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9531 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/super_master.py
--rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/prim/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.454459 jaseci-1.4.2.5/jaseci/svc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/svc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.454459 jaseci-1.4.2.5/jaseci/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/jac_test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    14672 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/jac_test_progs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    32750 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/test_jac.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    25401 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/test_progs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8911 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.454459 jaseci-1.4.2.5/jaseci/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.458459 jaseci-1.4.2.5/jaseci/utils/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/actions/actions_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    21564 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/actions/actions_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/actions/actions_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)   119142 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/gprof2dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/id_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/jaseci/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 16:44:28.458459 jaseci-1.4.2.5/jaseci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-01-09 16:44:28.000000 jaseci-1.4.2.5/jaseci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2024-01-09 16:44:28.000000 jaseci-1.4.2.5/jaseci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 16:44:28.000000 jaseci-1.4.2.5/jaseci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-09 16:44:28.000000 jaseci-1.4.2.5/jaseci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-09 16:44:28.000000 jaseci-1.4.2.5/jaseci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-09 16:44:28.000000 jaseci-1.4.2.5/jaseci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 16:44:28.458459 jaseci-1.4.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-01-09 16:44:10.000000 jaseci-1.4.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.556937 jaseci-1.4.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-23 19:42:44.556937 jaseci-1.4.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.520937 jaseci-1.4.2.6/jaseci/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.524937 jaseci-1.4.2.6/jaseci/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/cli_tools/book_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14869 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/cli_tools/jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.524937 jaseci-1.4.2.6/jaseci/cli_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/cli_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21548 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/cli_tools/tests/test_jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.524937 jaseci-1.4.2.6/jaseci/extens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.528936 jaseci-1.4.2.6/jaseci/extens/act_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/jaseci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/rand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8191 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.528936 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/std_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_mail_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_net_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_std_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_webtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_zlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/webtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/act_lib/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.532936 jaseci-1.4.2.6/jaseci/extens/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/alias_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/global_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/jsorc_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/master_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/share_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/super_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.536937 jaseci-1.4.2.6/jaseci/extens/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_global_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_uncommon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/tests/test_walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/api/webhook_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.536937 jaseci-1.4.2.6/jaseci/extens/svc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/elastic_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/kube_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12467 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/prome_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/redis_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/storage_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/stripe_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/extens/svc/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.540937 jaseci-1.4.2.6/jaseci/jac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.540937 jaseci-1.4.2.6/jaseci/jac/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/interpreter/architype_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67273 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/interpreter/interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/interpreter/sentinel_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.540937 jaseci-1.4.2.6/jaseci/jac/interpreter/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/interpreter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/interpreter/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8452 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/interpreter/walker_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.540937 jaseci-1.4.2.6/jaseci/jac/ir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/ast_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/jac_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.540937 jaseci-1.4.2.6/jaseci/jac/ir/passes/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/ast_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/codegen_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/ir_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/printer_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/pt_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/ir/passes/stats_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jac.g4
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.544937 jaseci-1.4.2.6/jaseci/jac/jac_parse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jac_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34691 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jac_parse/jacLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29031 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jac_parse/jacListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   334026 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jac_parse/jacParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jac_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.544937 jaseci-1.4.2.6/jaseci/jac/jsci_vm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jsci_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jsci_vm/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jsci_vm/inst_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jsci_vm/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jsci_vm/op_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.544937 jaseci-1.4.2.6/jaseci/jac/jsci_vm/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jsci_vm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/jsci_vm/tests/test_codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.544937 jaseci-1.4.2.6/jaseci/jac/machine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/machine/jac_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/machine/jac_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/machine/machine_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.544937 jaseci-1.4.2.6/jaseci/jac/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13323 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/tests/book_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13870 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/tests/test_book.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jac/tests/test_lang_14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.548936 jaseci-1.4.2.6/jaseci/jsorc/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22563 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/jsorc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/jsorc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12303 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/live_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.548936 jaseci-1.4.2.6/jaseci/jsorc/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/manifests/database.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   484420 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/manifests/elastic.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    37855 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/manifests/prometheus.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/manifests/redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/remote_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.548936 jaseci-1.4.2.6/jaseci/jsorc/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/jsorc/tests/test_jsorc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.552937 jaseci-1.4.2.6/jaseci/prim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/ability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/architype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18288 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/obj_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/super_master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/prim/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.552937 jaseci-1.4.2.6/jaseci/svc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/svc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.552937 jaseci-1.4.2.6/jaseci/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27903 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/jac_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14672 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/jac_test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32750 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/test_jac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25401 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.552937 jaseci-1.4.2.6/jaseci/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.556937 jaseci-1.4.2.6/jaseci/utils/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/actions/actions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21565 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/actions/actions_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/actions/actions_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119142 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/gprof2dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5401 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/id_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10454 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/jaseci/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:42:44.556937 jaseci-1.4.2.6/jaseci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-23 19:42:44.000000 jaseci-1.4.2.6/jaseci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2024-04-23 19:42:44.000000 jaseci-1.4.2.6/jaseci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:42:44.000000 jaseci-1.4.2.6/jaseci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 19:42:44.000000 jaseci-1.4.2.6/jaseci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-23 19:42:44.000000 jaseci-1.4.2.6/jaseci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 19:42:44.000000 jaseci-1.4.2.6/jaseci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:42:44.556937 jaseci-1.4.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-23 19:42:33.000000 jaseci-1.4.2.6/setup.py
```

### Comparing `jaseci-1.4.2.5/LICENSE` & `jaseci-1.4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/PKG-INFO` & `jaseci-1.4.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaseci
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
 License-File: LICENSE
 Requires-Dist: click<8.2.0,>=8.1.0
 Requires-Dist: click-shell<2.2,>=2.1
 Requires-Dist: numpy<1.24.0,>=1.23.0
@@ -17,15 +17,15 @@
 Requires-Dist: flake8
 Requires-Dist: pep8-naming
 Requires-Dist: stripe
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: docstring-parser
 Requires-Dist: prometheus_api_client==0.5.1
 Requires-Dist: prometheus-client==0.14.1
-Requires-Dist: kubernetes==23.6.0
+Requires-Dist: kubernetes==21.7.0
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: pytest-cov
 Requires-Dist: validators==0.21.2
 Requires-Dist: psycopg2-binary==2.9.5
 Requires-Dist: pygls==1.0.2
 Requires-Dist: mock
```

### Comparing `jaseci-1.4.2.5/jaseci/__init__.py` & `jaseci-1.4.2.6/jaseci/__init__.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/cli_tools/book_tools.py` & `jaseci-1.4.2.6/jaseci/cli_tools/book_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,19 +201,19 @@
             auth_level = ""
             for j in Sm.all_apis(None, True):
                 if i == j["fname"]:
                     found = True
                     auth_level = (
                         "public"
                         if j in Sm._public_api
-                        else "user"
-                        if j in Sm._private_api
-                        else "admin"
-                        if j in Sm._admin_api
-                        else "cli_only"
+                        else (
+                            "user"
+                            if j in Sm._private_api
+                            else "admin" if j in Sm._admin_api else "cli_only"
+                        )
                     )
                     break
             if not found:
                 continue
             name = i.replace("_", " ")
             api = i.replace("_", "\\_")
             ret += (
@@ -434,19 +434,19 @@
             auth_level = ""
             for j in Sm.all_apis(None, True):
                 if i == j["fname"]:
                     found = True
                     auth_level = (
                         "public"
                         if j in Sm._public_api
-                        else "user"
-                        if j in Sm._private_api
-                        else "admin"
-                        if j in Sm._admin_api
-                        else "cli_only"
+                        else (
+                            "user"
+                            if j in Sm._private_api
+                            else "admin" if j in Sm._admin_api else "cli_only"
+                        )
                     )
                     break
             if not found:
                 continue
             name = i.replace("_", " ")
             api = i.replace("_", "\\_")
             ret += f"<div class='actionHeading'>{name}</div>\n\n"
```

### Comparing `jaseci-1.4.2.5/jaseci/cli_tools/jsctl.py` & `jaseci-1.4.2.6/jaseci/cli_tools/jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/cli_tools/tests/test_jsctl.py` & `jaseci-1.4.2.6/jaseci/cli_tools/tests/test_jsctl.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/date.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 from datetime import datetime, timedelta
 from jaseci.jsorc.live_actions import jaseci_action
 from dateutil.relativedelta import relativedelta
 
 
 @jaseci_action()
 def quantize_to_year(date: str):
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/elastic.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/file.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 from jaseci.jsorc.live_actions import jaseci_action
 import os
 import json
 import base64
 
 
 @jaseci_action()
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/file_handler.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/file_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 import mimetypes
 import magic
 from os import path
 from urllib.parse import urlparse
 from requests import get
 from jaseci.jsorc.live_actions import jaseci_action
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/jaseci.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/jaseci.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import master_from_meta, copy_func
 from jaseci.prim.super_master import SuperMaster
 import functools
 
 
 def interface_api(api_name, is_public, p_spec, *args, meta):
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/maths.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/maths.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/net.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/net.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This library of actions cover the standard operations that can be
 run on graph elements (nodes and edges). A number of these actions
 accept lists that are exclusively composed of instances of defined
 architype node and/or edges. Keep in mind that a \\lstinline{jac_set}
 is simply a list that only contains such elements.
 """
+
 from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import master_from_meta
 from jaseci.jac.jac_set import JacSet
 from jaseci.prim.node import Node
 from jaseci.prim.edge import Edge
 import uuid
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/rand.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/rand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 import random
 
 # import faker
 from datetime import datetime
 from datetime import timedelta
 from jaseci.jsorc.live_actions import jaseci_action
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/regex.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/request.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 import requests
 from jaseci.jsorc.live_actions import jaseci_action
 
 
 @jaseci_action()
 def get(url: str, data: dict = {}, header: dict = {}):
     """
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/std.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/std.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 from operator import itemgetter
 from jaseci.utils.utils import app_logger, json_out
 from datetime import datetime
 from jaseci.jac.machine.jac_value import jac_wrap_value as jwv
 from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import master_from_meta
 from jaseci.prim.element import Element
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/storage.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/storage.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/stripe.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/stripe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 import stripe as s
 
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.utils import logger
 from jaseci.extens.svc.stripe_svc import StripeService
 from jaseci.jsorc.live_actions import jaseci_action
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/std_test_code.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/std_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_date.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_elastic.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_elastic.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_file.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_file_lib.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_file_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_mail_lib.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_mail_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_maths.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_net_lib.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_net_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_regex.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_std.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_std.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_std_lib.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_std_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_url.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_vector.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_webtool.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_webtool.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/tests/test_zlib.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/tests/test_zlib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/url.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 from jaseci.jsorc.live_actions import jaseci_action
 from fastapi import HTTPException
 import base64
 import requests
 import urllib
 import validators
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/vector.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 import numpy as np
 from operator import itemgetter
 import pickle, base64
 
 from jaseci.jsorc.live_actions import jaseci_action
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/webtool.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/webtool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 import requests
 from jaseci.jsorc.live_actions import jaseci_action
 from bs4 import BeautifulSoup
 
 
 @jaseci_action()
 def get_page_meta(url: str, timeout: int = 3, parser: str = "lxml", headers: dict = {}):
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/act_lib/zip.py` & `jaseci-1.4.2.6/jaseci/extens/act_lib/zip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Built in actions for Jaseci"""
+
 from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import print_stack_to_log
 from base64 import b64decode, b64encode
 import zlib
 
 
 @jaseci_action()
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/actions_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/actions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Admin Global api functions as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 import jaseci.jsorc.live_actions as lact
 import json
 
 
 class ActionsApi:
     """
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/alias_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/alias_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Alias api as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 
 
 class AliasAPI:
     """
     Alias APIs for creating nicknames for UUIDs and other long strings
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/architype_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/architype_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Architype api functions as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.prim.architype import Architype
 from jaseci.prim.sentinel import Sentinel
 from jaseci.utils.utils import b64decode_str
 
 
 class ArchitypeApi:
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/config_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/config_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/global_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/global_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Admin Global api functions as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.prim.sentinel import Sentinel
 import uuid
 
 
 class GlobalApi:
     """
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/graph_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/graph_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Graph api functions as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.utils.id_list import IdList
 from jaseci.prim.graph import Graph
 from jaseci.prim.node import Node
 import uuid
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/interface.py` & `jaseci-1.4.2.6/jaseci/extens/api/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 General master interface engine for client interfaces as mixin
 """
+
 from inspect import signature, getdoc
 from jaseci.utils.utils import logger, is_jsonable, is_true, exc_stack_as_str_list
 from jaseci.prim.element import Element
 from jaseci.prim.walker import Walker
 import json
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/jac_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/jac_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Jac tools api functions as a mixin
 """
+
 from copy import deepcopy
 import json
 import os
 
 from jaseci.extens.api.interface import Interface
 from jaseci.jsorc.jsorc import JsOrc
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/jsorc_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/jsorc_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 JSORC APIs
 """
+
 import json
 from json import dumps
 from time import time
 
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.jsorc.jsorc_utils import convert_yaml_manifest, ManifestType
 from jaseci.utils.utils import logger
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/logger_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/logger_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Logger api as a mixin
 """
+
 import re
 from jaseci.extens.api.interface import Interface
 from jaseci.utils.log_utils import parse_logs
 from jaseci.utils.utils import logger, app_logger, logs
 from jaseci.utils.utils import connect_logger_handler
 from logging.handlers import HTTPHandler
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/master_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/master_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Master api as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.utils.id_list import IdList
 import uuid
 
 
 class MasterApi:
     """
@@ -68,15 +69,15 @@
             masts.append(i.serialize(detailed=detailed))
         return masts
 
     @Interface.private_api(cli_args=["name"])
     def master_active_set(self, name: str):
         """
         Sets the default master master should use
-        NOTE: Specail handler included in general_interface_to_api
+        NOTE: Special handler included in general_interface_to_api
         """
         mas = self.sub_master_ids.get_obj_by_name(name)
         if not mas:
             return {"response": f"{name} not found"}
         self.caller = mas.jid
         return {"response": f"You are now {mas.name}"}
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/object_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/object_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Object api as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.prim.element import Element
 
 
 class ObjectApi:
     """Object APIs for generalized operations on Jaseci objects
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/prometheus_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/prometheus_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Prometheus APIs
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.extens.svc.prome_svc import PrometheusService
 
 
 def prome():
     return JsOrc.svc("prome").poke(PrometheusService)
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/queue_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/queue_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Queue api functions as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.extens.svc.task_svc import TaskService
 
 
 class QueueApi:
     """
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/sentinel_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/sentinel_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Sentinel api functions as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.utils.id_list import IdList
 from jaseci.prim.sentinel import Sentinel
 from jaseci.utils.utils import b64decode_str
 import uuid
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/super_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/super_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Super (master) api as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.prim.master import Master
 
 
 class SuperApi:
     """Super APIs for creating nicknames for UUIDs and other long strings"""
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_architype_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_global_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_global_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_graph_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_logger_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_logger_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_object_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_object_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_sentinel_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_uncommon.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_uncommon.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_user_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/tests/test_walker_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/tests/test_walker_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/user_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/user_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 User API
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.jsorc.jsorc import JsOrc
 
 
 class UserApi:
     """
     User APIs for creating users (some functions should be override downstream)
@@ -138,7 +139,28 @@
         )
 
     def user_destroyer(self, name: str):
         """
         Permanently delete master with given id
         """
         pass
+
+    @Interface.private_api()
+    def user_search(
+        self,
+        name: str,
+        detailed: bool = False,
+        create_if_not_exist: bool = False,
+        create_fields: dict = {},
+    ):
+        """
+        Search for user and returns its master jid.
+        Create new one if the user doesn't already exist, optionally.
+        create_fields will be forwarded to the user create endpoint, including
+            password
+            global_init
+            global_init_ctx
+            other_fields
+            send_email
+        See the user_create API for more details.
+        """
+        pass
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/walker_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/walker_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Walker api functions as a mixin
 """
+
 from jaseci.extens.api.interface import Interface
 from jaseci.prim.walker import Walker
 from jaseci.prim.node import Node
 from jaseci.prim.sentinel import Sentinel
 from jaseci.utils.id_list import IdList
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/api/webhook_api.py` & `jaseci-1.4.2.6/jaseci/extens/api/webhook_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Webhook API
 """
+
 from jaseci.extens.api.interface import Interface
 from fastapi import HTTPException
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.extens.svc.stripe_svc import StripeService
 
 import stripe as _stripe
 
@@ -51,17 +52,19 @@
                 payload_meta.get("sentinel")
                 or customer_meta.get("sentinel")
                 or master.active_snt_id
                 or self._h.get_glob("GLOB_SENTINEL")
             )
             sentinel = self._h.get_obj(
                 master_id,
-                self._h.get_glob("GLOB_SENTINEL")
-                if sentinel_id == "global"
-                else sentinel_id,
+                (
+                    self._h.get_glob("GLOB_SENTINEL")
+                    if sentinel_id == "global"
+                    else sentinel_id
+                ),
             )
 
             payload = {"event": req_body}
             self.seek_committer(master)
 
             wlk = stripe_service.get_walker(req_body["type"])
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/elastic_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/elastic_svc.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
 
                 if not self.config.get("auth"):
                     auth = kube.get_secret(
                         f'{metadata.get("name")}-es-elastic-user',
                         "elastic",
                         metadata.get("namespace"),
                     )
-                    self.config[
-                        "auth"
-                    ] = f'basic {b64encode(f"elastic:{auth}".encode()).decode()}'
+                    self.config["auth"] = (
+                        f'basic {b64encode(f"elastic:{auth}".encode()).decode()}'
+                    )
 
         self.app = Elastic(self.config)
         self.app.health("timeout=1s")
 
     def post_run(self):
         if multiprocessing.current_process().name == "MainProcess":
             under_test = self.config.get("under_test", False)
```

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/kube_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/kube_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/mail_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/mail_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/prome_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/prome_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/redis_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/redis_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/storage_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/storage_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/stripe_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/stripe_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/task_svc.py` & `jaseci-1.4.2.6/jaseci/extens/svc/task_svc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/extens/svc/tasks.py` & `jaseci-1.4.2.6/jaseci/extens/svc/tasks.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/interpreter/architype_interp.py` & `jaseci-1.4.2.6/jaseci/jac/interpreter/architype_interp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Sentinel interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
+
 from jaseci.prim.node import Node
 from jaseci.prim.edge import Edge
 from jaseci.prim.walker import Walker
 from jaseci.jac.interpreter.interp import Interp
 from jaseci.jac.machine.jac_scope import JacScope
 from jaseci.jac.machine.jac_value import JacValue
 
@@ -202,13 +203,17 @@
         for i in self.super_archs:
             super_jac_ast = (
                 self.parent()
                 .arch_ids.get_obj_by_name(name=i, kind=item.kind)
                 .get_jac_ast()
                 .kid[-1]
             )
-            self.run_attr_block(super_jac_ast, item) if not isinstance(
-                item, Walker
-            ) else self.run_walker_block(super_jac_ast, item)
-        self.run_attr_block(jac_ast, item) if not isinstance(
-            item, Walker
-        ) else self.run_walker_block(jac_ast, item)
+            (
+                self.run_attr_block(super_jac_ast, item)
+                if not isinstance(item, Walker)
+                else self.run_walker_block(super_jac_ast, item)
+            )
+        (
+            self.run_attr_block(jac_ast, item)
+            if not isinstance(item, Walker)
+            else self.run_walker_block(jac_ast, item)
+        )
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/interpreter/interp.py` & `jaseci-1.4.2.6/jaseci/jac/interpreter/interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
+
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.extens.svc.task_svc import TaskService
 from jaseci.utils.utils import is_jsonable, parse_str_token, uuid_re
 from jaseci.prim.element import Element
 from jaseci.prim.node import Node
 from jaseci.prim.edge import Edge
 from jaseci.jac.jac_set import JacSet
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/interpreter/sentinel_interp.py` & `jaseci-1.4.2.6/jaseci/jac/interpreter/sentinel_interp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Sentinel interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
+
 from jaseci.prim.architype import Architype
 from jaseci.jac.interpreter.interp import Interp
 from jaseci.utils.utils import parse_str_token
 from jaseci.jac.ir.jac_code import jac_ast_to_ir
 from jaseci.jac.machine.jac_scope import JacScope
 from jaseci.prim.ability import Ability
 
@@ -211,16 +212,18 @@
                 | KW_GRAPH graph_block
             ) KW_BY (
                 (walker_ref spawn_ctx? (code_block | SEMI))
                 | KW_WALKER walker_block
             );
         """
         kid = self.set_cur_ast(jac_ast)
-        self.run_multistring(kid[2]) if kid[1].name == "NAME" else self.run_multistring(
-            kid[1]
+        (
+            self.run_multistring(kid[2])
+            if kid[1].name == "NAME"
+            else self.run_multistring(kid[1])
         )
         testcase = {
             "name": kid[1].token_text() if kid[1].name == "NAME" else "",
             "title": self.pop().value,
             "graph_ref": None,
             "graph_block": None,
             "walker_ref": None,
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/interpreter/tests/test_interp.py` & `jaseci-1.4.2.6/jaseci/jac/interpreter/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/interpreter/walker_interp.py` & `jaseci-1.4.2.6/jaseci/jac/interpreter/walker_interp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Walker interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
+
 from jaseci.prim.node import Node
 from jaseci.jac.interpreter.interp import Interp
 from jaseci.jac.jac_set import JacSet
 from jaseci.jac.machine.jac_scope import JacScope
 from jaseci.jac.ir.jac_code import jac_ir_to_ast
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/ast.py` & `jaseci-1.4.2.6/jaseci/jac/ir/ast.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/ast_builder.py` & `jaseci-1.4.2.6/jaseci/jac/ir/ast_builder.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/jac_code.py` & `jaseci-1.4.2.6/jaseci/jac/ir/jac_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Mix in for jac code object in Jaseci
 """
+
 import json
 from jaseci.utils.utils import logger
 from jaseci.jac.ir.ast_builder import JacAstBuilder
 from jaseci.jac.ir.passes.schedule import multi_pass_optimizer
 from jaseci.jac.ir.ast import Ast
 import hashlib
 from pathlib import Path
@@ -89,17 +90,15 @@
             self.is_active = False
 
     def apply_ir(self, ir):
         """Apply's IR to object"""
         self.code_ir = (
             ir.strip()
             if (isinstance(ir, str))
-            else json.dumps(ir)
-            if (isinstance(ir, dict))
-            else jac_ast_to_ir(ir)
+            else json.dumps(ir) if (isinstance(ir, dict)) else jac_ast_to_ir(ir)
         )
         self.code_sig = hashlib.md5(self.code_ir.encode()).hexdigest()
         JacCode.refresh(self)  # should disregard overloaded versions
 
     def compile_jac(self, code, dir, start_rule="start", opt_level=4):
         """Generate AST tree from Jac code text"""
         tree = JacAstBuilder(
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/passes/codegen_pass.py` & `jaseci-1.4.2.6/jaseci/jac/ir/passes/codegen_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/passes/ir_pass.py` & `jaseci-1.4.2.6/jaseci/jac/ir/passes/ir_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/passes/printer_pass.py` & `jaseci-1.4.2.6/jaseci/jac/ir/passes/printer_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/passes/pt_prune_pass.py` & `jaseci-1.4.2.6/jaseci/jac/ir/passes/pt_prune_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/ir/passes/schedule.py` & `jaseci-1.4.2.6/jaseci/jac/ir/passes/schedule.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jac.g4` & `jaseci-1.4.2.6/jaseci/jac/jac.g4`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jac_parse/jacLexer.py` & `jaseci-1.4.2.6/jaseci/jac/jac_parse/jacLexer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jac_parse/jacListener.py` & `jaseci-1.4.2.6/jaseci/jac/jac_parse/jacListener.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jac_parse/jacParser.py` & `jaseci-1.4.2.6/jaseci/jac/jac_parse/jacParser.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jac_set.py` & `jaseci-1.4.2.6/jaseci/jac/jac_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Jac's set class for Jaseci
 
 Adds relevant operators to id_list for operations on sets of nodes and edges
 """
+
 # from jaseci.utils.id_list import id_list
 from jaseci.utils.utils import logger
 from jaseci.prim.element import Element
 
 
 class JacSet(list):
     """
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/jsci_vm/disasm.py` & `jaseci-1.4.2.6/jaseci/jac/jsci_vm/disasm.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jsci_vm/inst_ptr.py` & `jaseci-1.4.2.6/jaseci/jac/jsci_vm/inst_ptr.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jsci_vm/machine.py` & `jaseci-1.4.2.6/jaseci/jac/jsci_vm/machine.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jsci_vm/op_codes.py` & `jaseci-1.4.2.6/jaseci/jac/jsci_vm/op_codes.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/jsci_vm/tests/test_codegen.py` & `jaseci-1.4.2.6/jaseci/jac/jsci_vm/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/machine/jac_scope.py` & `jaseci-1.4.2.6/jaseci/jac/machine/jac_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Variable scope manager for Jac
 
 Utility for all runtime interaction with variables in different scopes
 """
+
 from jaseci.jac.machine.jac_value import JacValue
 from jaseci.jsorc.live_actions import get_global_actions
 
 
 class JacScope:
     def __init__(self, parent, name, has_obj=None, here=None, visitor=None):
         self.parent = parent
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/machine/jac_value.py` & `jaseci-1.4.2.6/jaseci/jac/machine/jac_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Variable manager for Jac
 
 Representations for all jac runtime variables
 """
+
 from jaseci.prim.element import Element
 from jaseci.prim.obj_mixins import Anchored
 from jaseci.prim.node import Node
 from jaseci.prim.edge import Edge
 from jaseci.prim.graph import Graph
 from jaseci.jac.jac_set import JacSet
 import uuid
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/machine/machine_state.py` & `jaseci-1.4.2.6/jaseci/jac/machine/machine_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
+
 from copy import copy
 from jaseci.utils.utils import logger, exc_stack_as_str_list, generate_stack_as_str_list
 from jaseci.jsorc.live_actions import live_actions, load_preconfig_actions
 
 # from jaseci.actions.find_action import find_action
 from jaseci.prim.element import Element
 
@@ -95,17 +96,19 @@
             name = self.call_name()
             if name not in self._mast._jac_profile:
                 self._mast._jac_profile[name] = {
                     "calls": 1,
                     "u_calls": 0 if name in MachineState.recur_detect_set else 1,
                     "tot_time": self._jac_scope._total_time
                     + (time.time() - self._jac_scope._start_time),
-                    "cum_time": 0
-                    if name in MachineState.recur_detect_set
-                    else time.time() - self._jac_scope._cum_start_time,
+                    "cum_time": (
+                        0
+                        if name in MachineState.recur_detect_set
+                        else time.time() - self._jac_scope._cum_start_time
+                    ),
                 }
             else:
                 c = self._mast._jac_profile[name]["calls"]
                 u = self._mast._jac_profile[name]["u_calls"]
                 t = self._mast._jac_profile[name]["tot_time"]
                 p = self._mast._jac_profile[name]["cum_time"]
                 self._mast._jac_profile[name]["calls"] = c + 1
```

### Comparing `jaseci-1.4.2.5/jaseci/jac/tests/book_code.py` & `jaseci-1.4.2.6/jaseci/jac/tests/book_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/tests/test_book.py` & `jaseci-1.4.2.6/jaseci/jac/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jac/tests/test_lang_14.py` & `jaseci-1.4.2.6/jaseci/jac/tests/test_lang_14.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/jsorc.py` & `jaseci-1.4.2.6/jaseci/jsorc/jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/jsorc_settings.py` & `jaseci-1.4.2.6/jaseci/jsorc/jsorc_settings.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/jsorc_utils.py` & `jaseci-1.4.2.6/jaseci/jsorc/jsorc_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/live_actions.py` & `jaseci-1.4.2.6/jaseci/jsorc/live_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 General action base class with automation for hot loading
 """
+
 from importlib.util import spec_from_file_location, module_from_spec
 from jaseci.utils.utils import logger
 from jaseci.jsorc.remote_actions import ACTIONS_SPEC_LOC
 from jaseci.jsorc.remote_actions import serv_actions, mark_as_remote, mark_as_endpoint
 import requests
 import os
 import sys
```

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/manifests/database.yaml` & `jaseci-1.4.2.6/jaseci/jsorc/manifests/database.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/manifests/elastic.yaml` & `jaseci-1.4.2.6/jaseci/jsorc/manifests/elastic.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -5635,14 +5635,15 @@
       labels:
         control-plane: elastic-operator
     spec:
       terminationGracePeriodSeconds: 10
       serviceAccountName: elastic-operator
       securityContext:
         runAsNonRoot: true
+        fsGroup: 65534
       containers:
       - image: "docker.elastic.co/eck/eck-operator:2.7.0"
         imagePullPolicy: IfNotPresent
         name: manager
         args:
         - "manager"
         - "--config=/conf/eck.yaml"
@@ -5996,14 +5997,18 @@
 spec:
   version: 8.6.2
   nodeSets:
   - name: default
     count: 1
     config:
       node.store.allow_mmap: false
+      http.cors.enabled: true
+      http.cors.allow-origin: "*"
+      http.cors.allow-methods: OPTIONS, POST, GET
+      http.cors.allow-headers: X-Requested-With, X-Auth-Token, Content-Type, Content-Length, Authorization, Access-Control-Allow-Headers, Accept
     volumeClaimTemplates:
     - metadata:
         name: elasticsearch-data
         namespace: elastic
       spec:
         accessModes:
         - ReadWriteOnce
```

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/manifests/prometheus.yaml` & `jaseci-1.4.2.6/jaseci/jsorc/manifests/prometheus.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/manifests/redis.yaml` & `jaseci-1.4.2.6/jaseci/jsorc/manifests/redis.yaml`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/memory.py` & `jaseci-1.4.2.6/jaseci/jsorc/memory.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/redis.py` & `jaseci-1.4.2.6/jaseci/jsorc/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module includes code related to hooking Jaseci's Redis to the
 core engine.
 """
+
 import json
 
 import jaseci as core_mod
 from jaseci.utils.json_handler import JaseciJsonDecoder, jsci_dict_normalize
 from jaseci.jsorc.memory import MemoryHook
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.extens.svc.redis_svc import RedisService
```

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/remote_actions.py` & `jaseci-1.4.2.6/jaseci/jsorc/remote_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 General action base class with automation for hot loading
 """
+
 from jaseci.utils.utils import logger, ColCodes as Cc
 from fastapi import FastAPI
 from fastapi.responses import RedirectResponse
 from pydantic import validate_arguments
 from time import time
 import inspect
 import uvicorn
```

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/tests/test_actions.py` & `jaseci-1.4.2.6/jaseci/jsorc/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/jsorc/tests/test_jsorc.py` & `jaseci-1.4.2.6/jaseci/jsorc/tests/test_jsorc.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/prim/ability.py` & `jaseci-1.4.2.6/jaseci/prim/ability.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Action class for Jaseci
 
 Each action has an id, name, timestamp and it's set of edges.
 """
+
 from jaseci.prim.element import Element
 from jaseci.jsorc.live_actions import live_actions
 from jaseci.jac.jac_set import JacSet
 import inspect
 import time
 
 from jaseci.jsorc.jsorc import JsOrc
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/architype.py` & `jaseci-1.4.2.6/jaseci/prim/architype.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Architype class for Jaseci
 
 Each architype is a registered templatized version of instances of any Jaseci
 abstractions or collections of instances (e.g., subgraphs, etc)
 """
+
 from jaseci.prim.element import Element
 from jaseci.jac.interpreter.architype_interp import ArchitypeInterp
 from jaseci.jac.ir.jac_code import JacCode
 from jaseci.utils.id_list import IdList
 
 
 class Architype(Element, JacCode, ArchitypeInterp):
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/edge.py` & `jaseci-1.4.2.6/jaseci/prim/edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Edge class for Jaseci
 
 Each edge has an id, name, timestamp, the from node at the element of the edge
 and the to node it is pointing to.
 """
+
 from jaseci.prim.element import Element
 from jaseci.prim.obj_mixins import Anchored
 from jaseci.utils.utils import logger
 import uuid
 import sys
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/element.py` & `jaseci-1.4.2.6/jaseci/prim/element.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/prim/graph.py` & `jaseci-1.4.2.6/jaseci/prim/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Graph  class for Jaseci
 
 """
+
 from jaseci.prim.node import Node
 from jaseci.utils.id_list import IdList
 
 
 class Graph(Node):
     """Graph class for Jaseci"""
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/master.py` & `jaseci-1.4.2.6/jaseci/prim/master.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from jaseci.extens.api.config_api import ConfigApi
 from jaseci.extens.api.interface import Interface
 from jaseci.extens.api.master_api import MasterApi
 from jaseci.extens.api.jac_api import JacApi
 from jaseci.extens.api.user_api import UserApi
 from jaseci.extens.api.queue_api import QueueApi
 from jaseci.extens.api.webhook_api import WebhookApi
+from jaseci.extens.api.share_api import ShareApi
 from jaseci.extens.api.health_api import HealthApi
 from jaseci.jsorc.jsorc import JsOrc
 
 
 @JsOrc.context(name="master")
 class Master(
     Element,
@@ -32,14 +33,15 @@
     SentinelApi,
     WalkerApi,
     ArchitypeApi,
     JacApi,
     UserApi,
     QueueApi,
     WebhookApi,
+    ShareApi,
     HealthApi,
 ):
     """Main class for master functions for user"""
 
     def __init__(self, head_master=None, *args, **kwargs):
         kwargs["m_id"] = None
 
@@ -47,14 +49,15 @@
         MasterApi.__init__(self, head_master)
         AliasAPI.__init__(self)
         ConfigApi.__init__(self)
         ObjectApi.__init__(self)
         GraphApi.__init__(self)
         WalkerApi.__init__(self)
         SentinelApi.__init__(self)
+        ShareApi.__init__(self)
         Interface.__init__(self)
 
     def destroy(self):
         """
         Destroys self from memory and persistent storage
         """
         GraphApi.destroy(self)
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/node.py` & `jaseci-1.4.2.6/jaseci/prim/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Node class for Jaseci
 
 Each node has an id, name, timestamp and it's set of edges.
 First node in list of 'member_node_ids' is designated root node
 """
+
 from collections import OrderedDict
 from jaseci.prim.element import Element
 from jaseci.prim.obj_mixins import Anchored
 from jaseci.prim.edge import Edge
 from jaseci.utils.id_list import IdList
 from jaseci.utils.utils import logger
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/obj_mixins.py` & `jaseci-1.4.2.6/jaseci/prim/obj_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Jaseci object mixins
 
 Various mixins to define properties of Jaseci objects
 """
+
 from jaseci.utils.id_list import IdList
 from jaseci.utils.utils import logger
 import uuid
 
 
 class Anchored:
     """Utility class for objects that hold anchor values"""
@@ -76,17 +77,19 @@
     """Utility class for objects that are sharable between users"""
 
     def __init__(self, m_id, mode=None, **kwargs):
         self.set_master(m_id)
         self.j_access = (
             mode
             if mode is not None
-            else self._h.get_obj(self._m_id, self._m_id).perm_default
-            if self._h.has_obj(self._m_id)
-            else "private"
+            else (
+                self._h.get_obj(self._m_id, self._m_id).perm_default
+                if self._h.has_obj(self._m_id)
+                else "private"
+            )
         )
         self.j_r_acc_ids = IdList(self)
         self.j_rw_acc_ids = IdList(self)
 
     @property
     def _m_id(self) -> str:
         return self.j_master
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/sentinel.py` & `jaseci-1.4.2.6/jaseci/prim/sentinel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Sentinel class for Jaseci
 
 Each sentinel has an id, name, timestamp and it's set of walkers.
 """
+
 from jaseci.prim.element import Element
 from jaseci.prim.obj_mixins import Anchored
 from jaseci.utils.utils import (
     logger,
     ColCodes as Cc,
     is_true,
     perf_test_start,
```

### Comparing `jaseci-1.4.2.5/jaseci/prim/super_master.py` & `jaseci-1.4.2.6/jaseci/prim/super_master.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/prim/walker.py` & `jaseci-1.4.2.6/jaseci/prim/walker.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/infer.py` & `jaseci-1.4.2.6/jaseci/tests/infer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/jac_test_code.py` & `jaseci-1.4.2.6/jaseci/tests/jac_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/jac_test_progs.py` & `jaseci-1.4.2.6/jaseci/tests/jac_test_progs.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/test_core.py` & `jaseci-1.4.2.6/jaseci/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/test_jac.py` & `jaseci-1.4.2.6/jaseci/tests/test_jac.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/test_node.py` & `jaseci-1.4.2.6/jaseci/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/test_progs.py` & `jaseci-1.4.2.6/jaseci/tests/test_progs.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/test_stack.py` & `jaseci-1.4.2.6/jaseci/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/tests/test_stripe.py` & `jaseci-1.4.2.6/jaseci/tests/test_stripe.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
         config = JsOrc.settings("STRIPE_CONFIG")
         config["enabled"] = True
-        config[
-            "api_key"
-        ] = "sk_test_51JWUIeCZO78n7fsZnPvualWhmJg1DcCI332kKnWF3q2sKGwnPADjEmNblfFWi4pWAWPuJwHxpeSoJGc0J5ButHN900Q2xBz1se"
+        config["api_key"] = (
+            "sk_test_51JWUIeCZO78n7fsZnPvualWhmJg1DcCI332kKnWF3q2sKGwnPADjEmNblfFWi4pWAWPuJwHxpeSoJGc0J5ButHN900Q2xBz1se"
+        )
         config["webhook_key"] = "test_webhook_key"
 
         JsOrc.svc_reset("stripe")
 
         super(StripeTests, cls).setUpClass()
         stripe.Product.create = Mock()
         stripe.Price.create = Mock()
```

### Comparing `jaseci-1.4.2.5/jaseci/utils/actions/actions_manager.py` & `jaseci-1.4.2.6/jaseci/utils/actions/actions_manager.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/utils/actions/actions_optimizer.py` & `jaseci-1.4.2.6/jaseci/utils/actions/actions_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module that manage and optimizes the actions configuration of Jaseci
 """
+
 from jaseci.jsorc.jsorc import JsOrc
 from jaseci.extens.svc.kube_svc import KubeService
 from jaseci.jsorc.remote_actions import ACTIONS_SPEC_LOC
 from jaseci.utils.utils import logger
 from jaseci.jsorc.live_actions import (
     load_module_actions,
     unload_module,
```

### Comparing `jaseci-1.4.2.5/jaseci/utils/actions/actions_state.py` & `jaseci-1.4.2.6/jaseci/utils/actions/actions_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/utils/file_handler.py` & `jaseci-1.4.2.6/jaseci/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/utils/gprof2dot.py` & `jaseci-1.4.2.6/jaseci/utils/gprof2dot.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/utils/id_list.py` & `jaseci-1.4.2.6/jaseci/utils/id_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ID list class for Jaseci
 
 Generalized functions for managing '_ids' convention for lists of Jaseci
 objects
 
 parent_obj is the instance that the list belongs to
 """
+
 from jaseci.utils.utils import logger
 
 
 class IdList(list):
     """
     ID list class for tracking lists of objects in Jaseci
```

### Comparing `jaseci-1.4.2.5/jaseci/utils/json_handler.py` & `jaseci-1.4.2.6/jaseci/utils/json_handler.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/utils/log_utils.py` & `jaseci-1.4.2.6/jaseci/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/utils/test_core.py` & `jaseci-1.4.2.6/jaseci/utils/test_core.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci/utils/utils.py` & `jaseci-1.4.2.6/jaseci/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.2.5/jaseci.egg-info/PKG-INFO` & `jaseci-1.4.2.6/jaseci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaseci
-Version: 1.4.2.5
+Version: 1.4.2.6
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
 License-File: LICENSE
 Requires-Dist: click<8.2.0,>=8.1.0
 Requires-Dist: click-shell<2.2,>=2.1
 Requires-Dist: numpy<1.24.0,>=1.23.0
@@ -17,15 +17,15 @@
 Requires-Dist: flake8
 Requires-Dist: pep8-naming
 Requires-Dist: stripe
 Requires-Dist: pydantic<2.0.0
 Requires-Dist: docstring-parser
 Requires-Dist: prometheus_api_client==0.5.1
 Requires-Dist: prometheus-client==0.14.1
-Requires-Dist: kubernetes==23.6.0
+Requires-Dist: kubernetes==21.7.0
 Requires-Dist: pytest
 Requires-Dist: pytest-xdist
 Requires-Dist: pytest-cov
 Requires-Dist: validators==0.21.2
 Requires-Dist: psycopg2-binary==2.9.5
 Requires-Dist: pygls==1.0.2
 Requires-Dist: mock
```

### Comparing `jaseci-1.4.2.5/jaseci.egg-info/SOURCES.txt` & `jaseci-1.4.2.6/jaseci.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 jaseci/extens/api/jsorc_api.py
 jaseci/extens/api/logger_api.py
 jaseci/extens/api/master_api.py
 jaseci/extens/api/object_api.py
 jaseci/extens/api/prometheus_api.py
 jaseci/extens/api/queue_api.py
 jaseci/extens/api/sentinel_api.py
+jaseci/extens/api/share_api.py
 jaseci/extens/api/super_api.py
 jaseci/extens/api/user_api.py
 jaseci/extens/api/walker_api.py
 jaseci/extens/api/webhook_api.py
 jaseci/extens/api/tests/__init__.py
 jaseci/extens/api/tests/test_architype_api.py
 jaseci/extens/api/tests/test_global_api.py
```

### Comparing `jaseci-1.4.2.5/jaseci.egg-info/requires.txt` & `jaseci-1.4.2.6/jaseci.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 flake8
 pep8-naming
 stripe
 pydantic<2.0.0
 docstring-parser
 prometheus_api_client==0.5.1
 prometheus-client==0.14.1
-kubernetes==23.6.0
+kubernetes==21.7.0
 pytest
 pytest-xdist
 pytest-cov
 validators==0.21.2
 psycopg2-binary==2.9.5
 pygls==1.0.2
 mock
```

### Comparing `jaseci-1.4.2.5/setup.py` & `jaseci-1.4.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         "flake8",
         "pep8-naming",
         "stripe",
         "pydantic<2.0.0",
         "docstring-parser",
         "prometheus_api_client==0.5.1",
         "prometheus-client==0.14.1",
-        "kubernetes==23.6.0",
+        "kubernetes==21.7.0",
         "pytest",
         "pytest-xdist",
         "pytest-cov",
         "validators==0.21.2",
         "psycopg2-binary==2.9.5",
         "pygls==1.0.2",
         "mock",
```

