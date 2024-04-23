# Comparing `tmp/reqless-0.13.3.tar.gz` & `tmp/reqless-1.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqless-0.13.3.tar", last modified: Fri Apr 19 14:19:01 2024, max compression
+gzip compressed data, was "reqless-1.0.0a0.tar", last modified: Tue Apr 23 13:33:15 2024, max compression
```

## Comparing `reqless-0.13.3.tar` & `reqless-1.0.0a0.tar`

### file list

```diff
@@ -1,103 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.253136 reqless-0.13.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.233136 reqless-0.13.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.237136 reqless-0.13.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-19 14:17:58.000000 reqless-0.13.3/.github/workflows/main-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-19 14:17:58.000000 reqless-0.13.3/.github/workflows/other-branch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-19 14:17:58.000000 reqless-0.13.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-19 14:17:58.000000 reqless-0.13.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 14:17:58.000000 reqless-0.13.3/.gitmodules
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.233136 reqless-0.13.3/.meta/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.237136 reqless-0.13.3/.meta/coverage/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 14:18:58.000000 reqless-0.13.3/.meta/coverage/badge.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-19 14:18:57.000000 reqless-0.13.3/.meta/coverage/report.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-19 14:17:58.000000 reqless-0.13.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-19 14:17:58.000000 reqless-0.13.3/.safety-policy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-19 14:17:58.000000 reqless-0.13.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-19 14:17:58.000000 reqless-0.13.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-19 14:19:01.253136 reqless-0.13.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20220 2024-04-19 14:17:58.000000 reqless-0.13.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 14:17:58.000000 reqless-0.13.3/Vagrantfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.237136 reqless-0.13.3/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-19 14:17:58.000000 reqless-0.13.3/bin/reqless-py-worker
--rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-04-19 14:17:58.000000 reqless-0.13.3/forgetful-bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 14:17:58.000000 reqless-0.13.3/provision.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-19 14:17:58.000000 reqless-0.13.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.241136 reqless-0.13.3/reqless/
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_job_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_job_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_throttles.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/abstract/abstract_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16598 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/lua/
--rw-r--r--   0 runner    (1001) docker     (127)    98606 2024-04-19 14:18:51.000000 reqless-0.13.3/reqless/lua/qless-lib.lua
--rw-r--r--   0 runner    (1001) docker     (127)    72558 2024-04-19 14:18:51.000000 reqless-0.13.3/reqless/lua/qless.lua
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/proctitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/qmore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/qmore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/qmore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.245136 reqless-0.13.3/reqless/queue_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/queue_resolvers/transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.249136 reqless-0.13.3/reqless/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless/workers/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.253136 reqless-0.13.3/reqless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22180 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 14:19:01.000000 reqless-0.13.3/reqless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:01.249136 reqless-0.13.3/reqless_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_job_processor_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_qmore_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14394 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15107 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-19 14:17:58.000000 reqless-0.13.3/reqless_test/test_worker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-19 14:18:33.000000 reqless-0.13.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:19:01.253136 reqless-0.13.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-19 14:17:58.000000 reqless-0.13.3/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.204605 reqless-1.0.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.184605 reqless-1.0.0a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.188605 reqless-1.0.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-23 13:32:05.000000 reqless-1.0.0a0/.github/workflows/main-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-23 13:32:05.000000 reqless-1.0.0a0/.github/workflows/other-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-23 13:32:05.000000 reqless-1.0.0a0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 13:32:05.000000 reqless-1.0.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 13:32:05.000000 reqless-1.0.0a0/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.184605 reqless-1.0.0a0/.meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.188605 reqless-1.0.0a0/.meta/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-23 13:33:11.000000 reqless-1.0.0a0/.meta/coverage/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-23 13:33:11.000000 reqless-1.0.0a0/.meta/coverage/report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-23 13:32:05.000000 reqless-1.0.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 13:32:05.000000 reqless-1.0.0a0/.safety-policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 13:32:05.000000 reqless-1.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 13:32:05.000000 reqless-1.0.0a0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-23 13:33:15.204605 reqless-1.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-04-23 13:32:05.000000 reqless-1.0.0a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 13:32:05.000000 reqless-1.0.0a0/Vagrantfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.188605 reqless-1.0.0a0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-23 13:32:05.000000 reqless-1.0.0a0/bin/reqless-py-worker
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5394 2024-04-23 13:32:05.000000 reqless-1.0.0a0/forgetful-bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-23 13:32:05.000000 reqless-1.0.0a0/provision.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-23 13:32:05.000000 reqless-1.0.0a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.188605 reqless-1.0.0a0/reqless/
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 13:33:15.000000 reqless-1.0.0a0/reqless/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.192605 reqless-1.0.0a0/reqless/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_job_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_queue_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_throttles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/abstract/abstract_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16623 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.192605 reqless-1.0.0a0/reqless/lua/
+-rw-r--r--   0 runner    (1001) docker     (127)    98606 2024-04-23 13:33:04.000000 reqless-1.0.0a0/reqless/lua/qless-lib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    72558 2024-04-23 13:33:04.000000 reqless-1.0.0a0/reqless/lua/qless.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/proctitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.192605 reqless-1.0.0a0/reqless/qmore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/qmore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/qmore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9022 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.196605 reqless-1.0.0a0/reqless/queue_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/queue_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/queue_resolvers/transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.196605 reqless-1.0.0a0/reqless/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/base_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/forking_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/main_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/serial_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless/workers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.200605 reqless-1.0.0a0/reqless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22221 2024-04-23 13:33:15.000000 reqless-1.0.0a0/reqless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-23 13:33:15.000000 reqless-1.0.0a0/reqless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:33:15.000000 reqless-1.0.0a0/reqless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-23 13:33:15.000000 reqless-1.0.0a0/reqless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 13:33:15.000000 reqless-1.0.0a0/reqless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.196605 reqless-1.0.0a0/reqless_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.196605 reqless-1.0.0a0/reqless_test/qmore/
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/qmore/test_qmore_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.196605 reqless-1.0.0a0/reqless_test/queue_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/queue_resolvers/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/queue_resolvers/test_qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/queue_resolvers/test_transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15456 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_job_processor_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:33:15.200605 reqless-1.0.0a0/reqless_test/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/workers/test_base_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/workers/test_forking_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/workers/test_gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/workers/test_main_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/workers/test_serial_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-23 13:32:05.000000 reqless-1.0.0a0/reqless_test/workers/test_worker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-23 13:32:45.000000 reqless-1.0.0a0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:33:15.204605 reqless-1.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-23 13:32:05.000000 reqless-1.0.0a0/whitelist.txt
```

### Comparing `reqless-0.13.3/.github/workflows/main-branch.yaml` & `reqless-1.0.0a0/.github/workflows/main-branch.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -52,16 +52,14 @@
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
           make test-with-coverage
-          coverage report | tee .meta/coverage/report.txt
-          coverage-badge -f -o .meta/coverage/badge.svg
           python -m build
 
       - name: Checkout tdg5/github-action-pack
         uses: actions/checkout@v4
         with:
           path: .github/actions/tdg5/github-action-pack
           ref: v0.0.5
```

### Comparing `reqless-0.13.3/.github/workflows/other-branch.yaml` & `reqless-1.0.0a0/.github/workflows/other-branch.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -47,9 +47,8 @@
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
           make test-with-coverage
-          coverage report
           python -m build
```

### Comparing `reqless-0.13.3/.github/workflows/release.yaml` & `reqless-1.0.0a0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/.meta/coverage/badge.svg` & `reqless-1.0.0a0/.meta/coverage/badge.svg`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/.meta/coverage/report.txt` & `reqless-1.0.0a0/.meta/coverage/report.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Name                                                                              Stmts   Miss  Cover
 -----------------------------------------------------------------------------------------------------
-reqless/__init__.py                                                                 146      1    99%
+reqless/__init__.py                                                                 145      1    99%
 reqless/abstract/__init__.py                                                         15      0   100%
-reqless/abstract/abstract_client.py                                                  23      0   100%
+reqless/abstract/abstract_client.py                                                  24      0   100%
 reqless/abstract/abstract_config.py                                                  18      0   100%
 reqless/abstract/abstract_job.py                                                     56      0   100%
 reqless/abstract/abstract_job_data.py                                                 6      0   100%
 reqless/abstract/abstract_job_processor.py                                           20      1    95%
 reqless/abstract/abstract_jobs.py                                                    10      0   100%
 reqless/abstract/abstract_queue.py                                                   27      0   100%
 reqless/abstract/abstract_queue_identifiers_transformer.py                            4      0   100%
@@ -28,15 +28,17 @@
 reqless/queue.py                                                                     91      0   100%
 reqless/queue_resolvers/__init__.py                                                   4      0   100%
 reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py       50      0   100%
 reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py      61      0   100%
 reqless/queue_resolvers/transforming_queue_resolver.py                               13      0   100%
 reqless/throttle.py                                                                  29      0   100%
 reqless/util.py                                                                       7      0   100%
-reqless/workers/__init__.py                                                           2      0   100%
-reqless/workers/forking.py                                                           55      2    96%
-reqless/workers/greenlet.py                                                          50      0   100%
-reqless/workers/serial.py                                                            29      0   100%
+reqless/workers/__init__.py                                                           5      0   100%
+reqless/workers/base_worker.py                                                       65      2    97%
+reqless/workers/forking_worker.py                                                    58      3    95%
+reqless/workers/gevent_worker.py                                                     53      0   100%
+reqless/workers/main_worker.py                                                       13      0   100%
+reqless/workers/serial_worker.py                                                     27      0   100%
+reqless/workers/signals.py                                                           13      0   100%
 reqless/workers/util.py                                                              39      1    97%
-reqless/workers/worker.py                                                            78      3    96%
 -----------------------------------------------------------------------------------------------------
-TOTAL                                                                              1340     24    98%
+TOTAL                                                                              1360     24    98%
```

### Comparing `reqless-0.13.3/.pre-commit-config.yaml` & `reqless-1.0.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/LICENSE` & `reqless-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/Makefile` & `reqless-1.0.0a0/Makefile`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 	make -C reqless/qless-core/
 	cp reqless/qless-core/qless.lua reqless/lua/
 	cp reqless/qless-core/qless-lib.lua reqless/lua/
 
 .PHONY: test-with-coverage
 test-with-coverage: qless-core
 	coverage run -m pytest
+	coverage report | tee .meta/coverage/report.txt
+	coverage-badge -f -o .meta/coverage/badge.svg
 
 requirements:
 	pip freeze | grep -v -e reqless > requirements.txt
 
 .PHONY: test
 test:
 	pytest
```

### Comparing `reqless-0.13.3/PKG-INFO` & `reqless-1.0.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.3
-Summary: Redis-based Queue Management
+Version: 1.0.0a0
+Summary: Queue Management built on remote data structure stores like redis and valkey
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
-Keywords: job,qless,qmore,redis,reqless
+Keywords: job,qless,qmore,redis,reqless,valkey
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
@@ -33,34 +33,33 @@
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pre-commit~=2.20.0; extra == "dev"
 Requires-Dist: removestar~=1.3.1; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
 Requires-Dist: setproctitle~=1.3.3; extra == "dev"
 Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: types-decorator~=5.1.8.4; extra == "dev"
-Requires-Dist: types-mock~=5.1.0.2; extra == "dev"
 Requires-Dist: types-redis~=4.6.0.11; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: coverage-badge~=1.1.0; extra == "test"
-Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest~=7.4.0; extra == "test"
 Requires-Dist: setuptools>=69; extra == "test"
 Provides-Extra: all
 Requires-Dist: reqless[dev,test]; extra == "all"
 
 [![code coverage](https://github.com/tdg5/reqless-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/reqless-py/main/.meta/coverage/report.txt)
 [![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
 
 # reqless
 
 This is a fork of [seomoz/qless-py](https://github.com/seomoz/qless-py) that
 includes significant type improvements and support for throttles.
 
-`qless` is a powerful `Redis`-based job queueing system inspired by
+`qless` is a powerful job queueing system based on remote dictionary servers
+(like `redis` and `valkey`) inspired by
 [resque](https://github.com/defunkt/resque#readme), but built on a collection
 of Lua scripts, maintained in the
 [qless-core](https://github.com/tdg5/qless-core) repo.
 
 ## Philosophy and Nomenclature
 
 A `job` is a unit of work identified by a job id or `jid`. A `queue` can
@@ -459,19 +458,19 @@
 # Wait 5 minutes
 len(queue.pop(10))
 # => 5 jobs got popped
 ```
 
 ### Configuration Options
 
-You can get and set global (read: in the context of the same Redis instance)
-configuration to change the behavior for heartbeating, and so forth. There
-aren't a tremendous number of configuration options, but an important one is
-how long job data is kept around. Job data is expired after it has been
-completed for `jobs-history` seconds, but is limited to the last
+You can get and set global (in the context of the same remote dictionary
+server instance) configuration to change the behavior for heartbeating, and so
+forth. There aren't a tremendous number of configuration options, but an
+important one is how long job data is kept around. Job data is expired after it
+has been completed for `jobs-history` seconds, but is limited to the last
 `jobs-history-count` completed jobs. These default to 50k jobs, and 30 days,
 but depending on volume, your needs may change. To only keep the last 500 jobs
 for up to 7 days:
 
 ```python
 client.config["jobs-history"] = 7 * 86400
 client.config["jobs-history-count"] = 500
@@ -606,17 +605,17 @@
 Frankly, these are best viewed using the web app.
 
 ### Lua
 
 `qless` is a set of client language bindings, but the majority of the work is
 done in a collection of Lua scripts that comprise the
 [core](https://github.com/tdg5/qless-core) functionality. These scripts run
-on the Redis 2.6+ server atomically and allow for portability with the same
-functionality guarantees. Consult the documentation for `qless-core` to learn
-more about its internals.
+on `redis` and `valkey` 7.0+ server atomically and allow for portability with
+the same functionality guarantees. Consult the documentation for `qless-core`
+to learn more about its internals.
 
 ### Web App
 
 `qless` also comes with a web app for administrative tasks, like keeping tabs
 on the progress of jobs, tracking specific jobs, retrying failed jobs, etc.
 It's available in the [`qless`](https://github.com/tdg5/qless) library as a
 mountable [`Sinatra`](http://www.sinatrarb.com/) app. The web app is language
```

### Comparing `reqless-0.13.3/README.md` & `reqless-1.0.0a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 [![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
 
 # reqless
 
 This is a fork of [seomoz/qless-py](https://github.com/seomoz/qless-py) that
 includes significant type improvements and support for throttles.
 
-`qless` is a powerful `Redis`-based job queueing system inspired by
+`qless` is a powerful job queueing system based on remote dictionary servers
+(like `redis` and `valkey`) inspired by
 [resque](https://github.com/defunkt/resque#readme), but built on a collection
 of Lua scripts, maintained in the
 [qless-core](https://github.com/tdg5/qless-core) repo.
 
 ## Philosophy and Nomenclature
 
 A `job` is a unit of work identified by a job id or `jid`. A `queue` can
@@ -409,19 +410,19 @@
 # Wait 5 minutes
 len(queue.pop(10))
 # => 5 jobs got popped
 ```
 
 ### Configuration Options
 
-You can get and set global (read: in the context of the same Redis instance)
-configuration to change the behavior for heartbeating, and so forth. There
-aren't a tremendous number of configuration options, but an important one is
-how long job data is kept around. Job data is expired after it has been
-completed for `jobs-history` seconds, but is limited to the last
+You can get and set global (in the context of the same remote dictionary
+server instance) configuration to change the behavior for heartbeating, and so
+forth. There aren't a tremendous number of configuration options, but an
+important one is how long job data is kept around. Job data is expired after it
+has been completed for `jobs-history` seconds, but is limited to the last
 `jobs-history-count` completed jobs. These default to 50k jobs, and 30 days,
 but depending on volume, your needs may change. To only keep the last 500 jobs
 for up to 7 days:
 
 ```python
 client.config["jobs-history"] = 7 * 86400
 client.config["jobs-history-count"] = 500
@@ -556,17 +557,17 @@
 Frankly, these are best viewed using the web app.
 
 ### Lua
 
 `qless` is a set of client language bindings, but the majority of the work is
 done in a collection of Lua scripts that comprise the
 [core](https://github.com/tdg5/qless-core) functionality. These scripts run
-on the Redis 2.6+ server atomically and allow for portability with the same
-functionality guarantees. Consult the documentation for `qless-core` to learn
-more about its internals.
+on `redis` and `valkey` 7.0+ server atomically and allow for portability with
+the same functionality guarantees. Consult the documentation for `qless-core`
+to learn more about its internals.
 
 ### Web App
 
 `qless` also comes with a web app for administrative tasks, like keeping tabs
 on the progress of jobs, tracking specific jobs, retrying failed jobs, etc.
 It's available in the [`qless`](https://github.com/tdg5/qless) library as a
 mountable [`Sinatra`](http://www.sinatrarb.com/) app. The web app is language
```

### Comparing `reqless-0.13.3/bin/reqless-py-worker` & `reqless-1.0.0a0/bin/reqless-py-worker`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/forgetful-bench.py` & `reqless-1.0.0a0/forgetful-bench.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,22 +19,22 @@
     type=float,
     help="What portion of jobs should be randomly dropped by workers",
 )
 parser.add_argument(
     "--host",
     dest="host",
     default="localhost",
-    help="The host to connect to as the Redis server",
+    help="The host to use when connecting to the remote data structure server",
 )
 parser.add_argument(
     "--port",
     dest="port",
     default=6379,
     type=int,
-    help="The port to connect on as the Redis server",
+    help="The port to use when connecting to the remote data structure server",
 )
 parser.add_argument(
     "--stages",
     dest="stages",
     default=1,
     type=int,
     help="How many times to requeue jobs",
@@ -68,15 +68,15 @@
     help="Reduce all the output",
 )
 parser.add_argument(
     "--no-flush",
     dest="flush",
     default=True,
     action="store_false",
-    help="Don't flush Redis after running",
+    help="Don't flush the remote data structure server after running",
 )
 
 args = parser.parse_args()
 
 
 logger = logging.getLogger("reqless-bench")
 formatter = logging.Formatter("[%(asctime)s] %(threadName)s => %(message)s")
@@ -119,22 +119,24 @@
                 job["stages"] -= 1
                 if job["stages"] > 0:
                     job.complete("testing")
                 else:
                     job.complete()
 
 
-# Make sure that the redis instance is empty first
-if len(client.redis.keys("*")):
-    print("Must begin on an empty Redis instance")
+# Make sure that the data structure server instance is empty first
+if len(client.database.keys("*")):
+    print("Must begin with empty data structure server")
     exit(1)
 
 client.config.set("heartbeat", 1)
-# This is how much CPU Redis had used /before/
-cpu_before = client.redis.info()["used_cpu_user"] + client.redis.info()["used_cpu_sys"]
+# This is how much CPU the data structure server had used /before/
+cpu_before = (
+    client.database.info()["used_cpu_user"] + client.database.info()["used_cpu_sys"]
+)
 # This is how long it took to add the jobs
 put_time = -time.time()
 # Alright, let's make a bunch of jobs
 testing = client.queue("testing")
 jids = [
     testing.put(
         reqless.Job,
@@ -183,16 +185,19 @@
 print("\tSDev : %f" % stats["run"]["std"])
 print("\tCompletion Time Histogram:")
 histo(stats["run"]["histogram"])
 
 print("=" * 50)
 print("Put jobs : %fs" % put_time)
 print("Do jobs  : %fs" % work_time)
-info = client.redis.info()
-print("Redis Mem: %s" % info["used_memory_human"])
-print("Redis Lua: %s" % info["used_memory_lua"])
-print("Redis CPU: %fs" % (info["used_cpu_user"] + info["used_cpu_sys"] - cpu_before))
+info = client.database.info()
+print("Data Structure Server Mem: %s" % info["used_memory_human"])
+print("Data Structure Server Lua: %s" % info["used_memory_lua"])
+print(
+    "Data Structure Server CPU: %fs"
+    % (info["used_cpu_user"] + info["used_cpu_sys"] - cpu_before)
+)
 
 # Flush the database when we're done
 if args.flush:
     print("Flushing")
-    client.redis.flushdb()
+    client.database.flushdb()
```

### Comparing `reqless-0.13.3/provision.sh` & `reqless-1.0.0a0/provision.sh`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/pyproject.toml` & `reqless-1.0.0a0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 dependencies = [
   "argparse",
   "decorator",
   "hiredis",
   "redis",
   "typing_extensions>=4.8.0",
 ]
-description = "Redis-based Queue Management"
+description = "Queue Management built on remote data structure stores like redis and valkey"
 dynamic = ["version"]
 keywords = [
     "job",
     "qless",
     "qmore",
     "redis",
     "reqless",
+    "valkey",
 ]
 license = {text = "MIT"}
 name = "reqless"
 readme = "README.md"
 requires-python = ">3.9.0"
 
 [project.optional-dependencies]
@@ -48,21 +49,19 @@
   "mypy~=1.8.0",
   "pre-commit~=2.20.0",
   "removestar~=1.3.1",
   "safety==2.3.4",
   "setproctitle~=1.3.3",
   "twine~=4.0.2",
   "types-decorator~=5.1.8.4",
-  "types-mock~=5.1.0.2",
   "types-redis~=4.6.0.11",
 ]
 test = [
     "coverage",
     "coverage-badge~=1.1.0",
-    "mock",
     "pytest~=7.4.0",
     "setuptools>=69",
 ]
 all = ["reqless[dev,test]"]
 
 [project.urls]
 Homepage = "https://github.com/tdg5/reqless-py"
```

### Comparing `reqless-0.13.3/reqless/__init__.py` & `reqless-1.0.0a0/reqless/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import json
 import pkgutil
 import socket
 import time
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import decorator
-import redis
-from redis import Redis
+from redis import Redis, ResponseError
 from redis.commands.core import Script
 
 from reqless.abstract import (
     AbstractClient,
     AbstractConfig,
     AbstractJob,
     AbstractJobs,
@@ -161,45 +160,46 @@
         url: str = "redis://localhost:6379",
         hostname: Optional[str] = None,
         **kwargs: Any,
     ):
         # This is our unique identifier as a worker
         self._worker_name: str = hostname or socket.gethostname()
         kwargs["decode_responses"] = True
-        # This is just the redis instance we're connected to conceivably
-        # someone might want to work with multiple instances simultaneously.
-        self._redis: Redis = redis.Redis.from_url(url, **kwargs)
+        # This is just the data structure server instance we're connected to
+        # conceivably someone might want to work with multiple instances
+        # simultaneously.
+        self._database: Redis = Redis.from_url(url, **kwargs)
         self._jobs: AbstractJobs = Jobs(self)
         self._queues: AbstractQueues = Queues(self)
         self._throttles: AbstractThrottles = Throttles(self)
         self._config: AbstractConfig = Config(self)
         self._workers: AbstractWorkers = Workers(self)
         self._events: Optional[Events] = None
 
         # We now have a single unified core script.
         data = pkgutil.get_data("reqless", "lua/qless.lua")
         if data is None:
             raise RuntimeError("Failed to load reqless lua!")
-        self._lua: Script = self.redis.register_script(data)
+        self._lua: Script = self.database.register_script(data)
 
     @property
     def config(self) -> AbstractConfig:
         return self._config
 
     @property
     def jobs(self) -> AbstractJobs:
         return self._jobs
 
     @property
     def queues(self) -> AbstractQueues:
         return self._queues
 
     @property
-    def redis(self) -> Redis:
-        return self._redis
+    def database(self) -> Redis:
+        return self._database
 
     @property
     def throttles(self) -> AbstractThrottles:
         return self._throttles
 
     @property
     def workers(self) -> AbstractWorkers:
@@ -212,23 +212,23 @@
     @worker_name.setter
     def worker_name(self, value: str) -> None:
         self._worker_name = value
 
     @property
     def events(self) -> Events:
         if self._events is None:
-            self._events = Events(self.redis)
+            self._events = Events(self.database)
         return self._events
 
     def __call__(self, command: str, *args: Any) -> Any:
         lua_args = [command, repr(time.time())]
         lua_args.extend(args)
         try:
             return self._lua(keys=[], args=lua_args)
-        except redis.ResponseError as exc:
+        except ResponseError as exc:
             raise ReqlessError(str(exc))
 
     def track(self, jid: str) -> bool:
         """Begin tracking this job"""
         response: str = self("track", "track", jid)
         return response == "1"
```

### Comparing `reqless-0.13.3/reqless/abstract/__init__.py` & `reqless-1.0.0a0/reqless/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/abstract/abstract_client.py` & `reqless-1.0.0a0/reqless/abstract/abstract_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any
+from typing import Any
+
+from redis import Redis
 
 from reqless.abstract.abstract_config import AbstractConfig
 from reqless.abstract.abstract_jobs import AbstractJobs
 from reqless.abstract.abstract_queues import AbstractQueues
 from reqless.abstract.abstract_throttles import AbstractThrottles
 from reqless.abstract.abstract_workers import AbstractWorkers
 
 
-if TYPE_CHECKING:  # pragma: no cover
-    from redis import Redis
-
-
 class AbstractClient(ABC):
     @abstractmethod
     def __call__(self, command: str, *args: Any) -> Any:  # pragma: no cover
         pass
 
     @property
     @abstractmethod
@@ -30,15 +28,15 @@
     @property
     @abstractmethod
     def queues(self) -> AbstractQueues:  # pragma: no cover
         pass
 
     @property
     @abstractmethod
-    def redis(self) -> "Redis":  # pragma: no cover
+    def database(self) -> Redis:  # pragma: no cover
         pass
 
     @property
     @abstractmethod
     def throttles(self) -> AbstractThrottles:  # pragma: no cover
         pass
```

### Comparing `reqless-0.13.3/reqless/abstract/abstract_config.py` & `reqless-1.0.0a0/reqless/abstract/abstract_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/abstract/abstract_job.py` & `reqless-1.0.0a0/reqless/abstract/abstract_job.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/abstract/abstract_job_processor.py` & `reqless-1.0.0a0/reqless/abstract/abstract_job_processor.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/abstract/abstract_jobs.py` & `reqless-1.0.0a0/reqless/abstract/abstract_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/abstract/abstract_queue.py` & `reqless-1.0.0a0/reqless/abstract/abstract_queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/abstract/abstract_queue_jobs.py` & `reqless-1.0.0a0/reqless/abstract/abstract_queue_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/abstract/abstract_throttle.py` & `reqless-1.0.0a0/reqless/abstract/abstract_throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/config.py` & `reqless-1.0.0a0/reqless/config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/importer.py` & `reqless-1.0.0a0/reqless/importer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/job.py` & `reqless-1.0.0a0/reqless/job.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,15 +500,17 @@
         name = value.__module__ + "." + value.__name__
         self.client("recur.update", self.jid, "klass", name)
         self._klass = value
         self._klass_name = name
 
     @property
     def next(self) -> Optional[float]:
-        return self.client.redis.zscore("ql:q:" + self.queue_name + "-recur", self.jid)
+        return self.client.database.zscore(
+            "ql:q:" + self.queue_name + "-recur", self.jid
+        )
 
     def move(self, queue: str) -> bool:
         """Make this recurring job attached to another queue"""
         response: bool = self.client("recur.update", self.jid, "queue", queue)
         return response
 
     def cancel(self) -> List[str]:
```

### Comparing `reqless-0.13.3/reqless/listener.py` & `reqless-1.0.0a0/reqless/listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 from contextlib import contextmanager
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple
 
 from redis import Redis
 from redis.client import PubSub
 
 
-# Our logger
 logger = logging.getLogger("reqless")
 
 
 class Listener:
     """A class that listens to pubsub channels and can unlisten"""
 
-    def __init__(self, redis: Redis, channels: List[str]):
-        self._pubsub: PubSub = redis.pubsub()
+    def __init__(self, database: Redis, channels: List[str]):
+        self._pubsub: PubSub = database.pubsub()
         self._channels: List[str] = channels
 
     def listen(self) -> Generator[Dict[str, Any], None, None]:
         """Listen for events as they come in"""
         try:
             self._pubsub.subscribe(*self._channels)
             for message in self._pubsub.listen():  # type: ignore[no-untyped-call]
@@ -46,18 +45,18 @@
         "popped",
         "put",
         "stalled",
         "track",
         "untrack",
     )
 
-    def __init__(self, redis: Redis):
+    def __init__(self, database: Redis):
         self._listener = Listener(
             channels=[self.namespace + event for event in self.events],
-            redis=redis,
+            database=database,
         )
         self._callbacks: Dict[str, Optional[Callable]] = {k: None for k in self.events}
 
     def listen(self) -> None:
         """Listen for events"""
         for message in self._listener.listen():
             logger.debug("Message: %s", message)
```

### Comparing `reqless-0.13.3/reqless/lua/qless-lib.lua` & `reqless-1.0.0a0/reqless/lua/qless-lib.lua`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/lua/qless.lua` & `reqless-1.0.0a0/reqless/lua/qless.lua`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/profile.py` & `reqless-1.0.0a0/reqless/profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Some utilities for profiling"""
 
 from collections import defaultdict
 from types import TracebackType
 from typing import Any, Dict, Optional, Type
 
-import redis
 from redis import Redis
+from redis.connection import ConnectionPool, DefaultParser
 
 from reqless.abstract import AbstractClient
 
 
 class Profiler:
     """Profiling a series of requests. Initialized with a Reqless client"""
 
     @staticmethod
     def clone(client: AbstractClient) -> Redis:
-        """Clone the redis client to be slowlog-compatible"""
-        kwargs = client.redis.connection_pool.connection_kwargs
-        kwargs["parser_class"] = redis.connection.DefaultParser
-        pool = redis.connection.ConnectionPool(**kwargs)
-        return redis.Redis(connection_pool=pool)
+        """Clone the data structure server client to be slowlog-compatible"""
+        kwargs = client.database.connection_pool.connection_kwargs
+        kwargs["parser_class"] = DefaultParser
+        pool = ConnectionPool(**kwargs)
+        return Redis(connection_pool=pool)
 
     @staticmethod
     def pretty(timings: Dict, label: str) -> None:
         """Print timing stats"""
         results = [(sum(values), len(values), key) for key, values in timings.items()]
         print(label)
         print("=" * 65)
@@ -35,32 +35,32 @@
         for total, length, key in sorted(results, reverse=True):
             print(
                 "%20s => %10.5f us | %8i | %10i us"
                 % (key, float(total) / length, length, total)
             )
 
     def __init__(self, client: AbstractClient):
-        self._client: Redis = self.clone(client)
+        self._database: Redis = self.clone(client)
         self._configs: Optional[Dict] = None
         self._timings: Dict = defaultdict(list)
         self._commands: Dict = {}
 
     def start(self) -> None:
         """Get ready for a profiling run"""
-        self._configs = self._client.config_get("slow-*")
-        self._client.config_set("slowlog-max-len", 100000)
-        self._client.config_set("slowlog-log-slower-than", 0)
-        self._client.execute_command("slowlog", "reset")
+        self._configs = self._database.config_get("slow-*")
+        self._database.config_set("slowlog-max-len", 100000)
+        self._database.config_set("slowlog-log-slower-than", 0)
+        self._database.execute_command("slowlog", "reset")
 
     def stop(self) -> None:
         """Set everything back to normal and collect our data"""
         if self._configs:
             for key, value in self._configs.items():
-                self._client.config_set(key, value)
-        logs = self._client.execute_command("slowlog", "get", 100000)
+                self._database.config_set(key, value)
+        logs = self._database.execute_command("slowlog", "get", 100000)
         current: Dict[str, Any] = {"name": None, "accumulated": defaultdict(list)}
         for _, _, duration, request in logs:
             command = request[0]
             if command == "slowlog":
                 continue
             if "eval" in command.lower():
                 subcommand = request[3]
@@ -80,15 +80,15 @@
             if current["name"] not in self._commands:
                 self._commands[current["name"]] = defaultdict(list)
             for key, values in current["accumulated"].items():
                 self._commands[current["name"]][key].extend(values)
 
     def display(self) -> None:
         """Print the results of this profiling"""
-        self.pretty(self._timings, "Raw Redis Commands")
+        self.pretty(self._timings, "Raw Data Structure Server Commands")
         print()
         for key, value in self._commands.items():
             self.pretty(value, 'Reqless "%s" Command' % key)
             print()
 
     def __enter__(self) -> "Profiler":
         self.start()
```

### Comparing `reqless-0.13.3/reqless/qmore/client.py` & `reqless-1.0.0a0/reqless/qmore/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         return (
             f"<QueuePriorityPattern patterns={self.patterns}"
             f" should_distribute_fairly={self.should_distribute_fairly}>"
         )
 
 
 class QmoreClient:
-    def __init__(self, redis: Redis):
-        self.redis: Redis = redis
+    def __init__(self, database: Redis):
+        self.database: Redis = database
 
     def get_queue_identifier_patterns(self) -> Dict[str, List[str]]:
-        serialized_patterns = self.redis.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
+        serialized_patterns = self.database.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
         patterns = {
             identifier: json.loads(json_patterns)
             for identifier, json_patterns in serialized_patterns.items()
         }
         if "default" not in patterns:
             patterns["default"] = "*"
         return patterns
@@ -42,22 +42,22 @@
         self,
         identifier_patterns: Dict[str, List[str]],
     ) -> None:
         json_patterns: Mapping[Union[bytes, str], Union[bytes, float, int, str]] = {
             identifier: json.dumps(patterns)
             for identifier, patterns in identifier_patterns.items()
         }
-        pipeline = self.redis.pipeline()
+        pipeline = self.database.pipeline()
         pipeline.delete(QUEUE_IDENTIFIER_PATTERNS_KEY)
         if json_patterns:
             pipeline.hset(QUEUE_IDENTIFIER_PATTERNS_KEY, mapping=json_patterns)
         pipeline.execute()
 
     def get_queue_priority_patterns(self) -> List[QueuePriorityPattern]:
-        serialized_priority_patterns = self.redis.lrange(
+        serialized_priority_patterns = self.database.lrange(
             QUEUE_PRIORITY_PATTERNS_KEY, 0, -1
         )
         queue_priority_patterns: List[QueuePriorityPattern] = []
         for serialized_priority_pattern in serialized_priority_patterns:
             priority_pattern_data = json.loads(serialized_priority_pattern)
             queue_priority_pattern = QueuePriorityPattern(
                 patterns=[
@@ -71,15 +71,15 @@
             queue_priority_patterns.append(queue_priority_pattern)
         return queue_priority_patterns
 
     def set_queue_priority_patterns(
         self,
         queue_priority_patterns: List[QueuePriorityPattern],
     ) -> None:
-        pipeline = self.redis.pipeline()
+        pipeline = self.database.pipeline()
         pipeline.delete(QUEUE_PRIORITY_PATTERNS_KEY)
         for queue_priority_pattern in queue_priority_patterns:
             serialized_queue_priority_pattern = json.dumps(
                 {
                     "fairly": queue_priority_pattern.should_distribute_fairly,
                     "pattern": ",".join(queue_priority_pattern.patterns),
                 }
```

### Comparing `reqless-0.13.3/reqless/queue.py` & `reqless-1.0.0a0/reqless/queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/queue_resolvers/__init__.py` & `reqless-1.0.0a0/reqless/queue_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-1.0.0a0/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 ):
     def __init__(
         self,
         client: Client,
         dynamic_queue_mapping_refresh_frequency_milliseconds: Optional[int] = None,
     ):
         self.reqless_client: Client = client
-        self.qmore_client: QmoreClient = QmoreClient(redis=self.reqless_client.redis)
+        self.qmore_client: QmoreClient = QmoreClient(
+            database=self.reqless_client.database
+        )
 
         self._dynamic_queue_mapping: Optional[Dict[str, List[str]]] = None
         self._dynamic_queue_mapping_ttl_time_delta: timedelta = timedelta(
             milliseconds=(
                 dynamic_queue_mapping_refresh_frequency_milliseconds or 5 * 60 * 1000
             ),
         )
```

### Comparing `reqless-0.13.3/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-1.0.0a0/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 ):
     def __init__(
         self,
         client: Client,
         dynamic_queue_priorities_refresh_frequency_milliseconds: Optional[int] = None,
     ):
         self.reqless_client: Client = client
-        self.qmore_client: QmoreClient = QmoreClient(redis=self.reqless_client.redis)
+        self.qmore_client: QmoreClient = QmoreClient(
+            database=self.reqless_client.database
+        )
 
         self._dynamic_queue_priorities: Optional[List[QueuePriorityPattern]] = None
         self._dynamic_queue_priorities_ttl_time_delta: timedelta = timedelta(
             milliseconds=(
                 dynamic_queue_priorities_refresh_frequency_milliseconds or 5 * 60 * 1000
             ),
         )
```

### Comparing `reqless-0.13.3/reqless/queue_resolvers/transforming_queue_resolver.py` & `reqless-1.0.0a0/reqless/queue_resolvers/transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/throttle.py` & `reqless-1.0.0a0/reqless/throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/workers/forking.py` & `reqless-1.0.0a0/reqless/workers/forking_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 from reqless import logger, util
 from reqless.abstract import (
     AbstractClient,
     AbstractJob,
     AbstractQueue,
     AbstractQueueResolver,
 )
-from reqless.workers.serial import SerialWorker
+from reqless.workers.base_worker import BaseWorker
+from reqless.workers.serial_worker import SerialWorker
+from reqless.workers.signals import register_signal_handler
 from reqless.workers.util import create_sandbox, divide
-from reqless.workers.worker import Worker
 
 
 try:
     NUM_CPUS = multiprocessing.cpu_count()
 except NotImplementedError:
     NUM_CPUS = 1
 
 
-class ForkingWorker(Worker):
+class ForkingWorker(BaseWorker):
     """A worker that forks child processes"""
 
     def __init__(
         self,
         queues: Union[Iterable[Union[str, AbstractQueue]], AbstractQueueResolver],
         client: AbstractClient,
         interval: Optional[float] = None,
@@ -40,15 +41,15 @@
             client,
             interval,
             resume,
             **kwargs,
         )
         # Worker class to use
         _klass = self.kwargs.pop("klass", SerialWorker)
-        self.klass: Type[Worker] = (
+        self.klass: Type[BaseWorker] = (
             util.import_class(_klass) if isinstance(_klass, str) else _klass
         )
         # How many children to launch
         self.count: int = self.kwargs.pop("workers", 0) or NUM_CPUS
         # A dictionary of child pids to information about them
         self.sandboxes: Dict[int, str] = {}
 
@@ -69,23 +70,29 @@
                 pid, status = os.waitpid(cpid, 0)
                 logger.warning("%i stopped with status %i" % (pid, status >> 8))
             except OSError:  # pragma: no cover
                 logger.exception("Error waiting for %i..." % cpid)
             finally:
                 self.sandboxes.pop(cpid, None)
 
-    def spawn(self, **kwargs: Any) -> Worker:
+    def spawn(self, **kwargs: Any) -> BaseWorker:
         """Return a new worker for a child process"""
         copy = dict(self.kwargs)
         copy.update(kwargs)
         return self.klass(self.queues, self.client, **copy)
 
+    def before_run(self) -> None:
+        register_signal_handler(
+            handler=self.signal_handler,
+            signals=("TERM", "INT", "QUIT"),
+        )
+
     def run(self) -> None:
         """Run this worker"""
-        self.signals(("TERM", "INT", "QUIT"))
+        self.before_run()
         # Divide up the jobs that we have to divy up between the workers. This
         # produces evenly-sized groups of jobs
         resume = divide(self.resume, self.count)
         for index in range(self.count):
             # The sandbox for the child worker
             sandbox = os.path.join(
                 os.getcwd(), "reqless-py-workers", "sandbox-%s" % index
@@ -125,14 +132,14 @@
                         except Exception:
                             logger.exception("Exception in spawned worker")
                         finally:
                             os._exit(0)
         finally:
             self.stop(signal.SIGKILL)
 
-    def handler(
+    def signal_handler(
         self, signum: int, frame: Optional[FrameType]
     ) -> None:  # pragma: no cover
         """Signal handler for this process"""
         if signum in (signal.SIGTERM, signal.SIGINT, signal.SIGQUIT):
             self.stop(signum)
             os._exit(0)
```

### Comparing `reqless-0.13.3/reqless/workers/greenlet.py` & `reqless-1.0.0a0/reqless/workers/gevent_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from reqless import logger
 from reqless.abstract import (
     AbstractClient,
     AbstractJob,
     AbstractQueue,
     AbstractQueueResolver,
 )
+from reqless.workers.base_worker import BaseWorker
+from reqless.workers.signals import basic_signal_handler, register_signal_handler
 from reqless.workers.util import create_sandbox
-from reqless.workers.worker import Worker
 
 
-class GeventWorker(Worker):
+class GeventWorker(BaseWorker):
     """A Gevent-based worker"""
 
     def __init__(
         self,
         queues: Union[Iterable[Union[str, AbstractQueue]], AbstractQueueResolver],
         client: AbstractClient,
         interval: Optional[float] = None,
@@ -58,25 +59,27 @@
                 job.sandbox = sandbox
                 job.process()
         finally:
             # Delete its entry from our greenlets mapping
             self.greenlets.pop(job.jid, None)
             self.sandboxes.append(sandbox)
 
-    def kill(self, jid: str) -> None:
+    def halt_job_processing(self, jid: str) -> None:
         """Stop the greenlet processing the provided jid"""
         greenlet = self.greenlets.get(jid)
         if greenlet is not None:
             logger.warning("Lost ownership of %s" % jid)
             greenlet.kill()
 
+    def before_run(self) -> None:
+        register_signal_handler(handler=basic_signal_handler(on_quit=self.stop))
+
     def run(self) -> None:
         """Work on jobs"""
-        # Register signal handlers
-        self.signals()
+        self.before_run()
 
         # Start listening
         with self.listener():
             try:
                 generator = self.jobs()
                 while not self.shutdown:
                     self.pool.wait_available()
```

### Comparing `reqless-0.13.3/reqless/workers/serial.py` & `reqless-1.0.0a0/reqless/workers/serial_worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from reqless.abstract import (
     AbstractClient,
     AbstractJob,
     AbstractQueue,
     AbstractQueueResolver,
 )
+from reqless.workers.base_worker import BaseWorker
 from reqless.workers.util import create_sandbox, set_title
-from reqless.workers.worker import Worker
 
 
-class SerialWorker(Worker):
+class SerialWorker(BaseWorker):
     """A worker that just does serial work"""
 
     def __init__(
         self,
         queues: Union[Iterable[Union[str, AbstractQueue]], AbstractQueueResolver],
         client: AbstractClient,
         interval: Optional[float] = None,
@@ -35,24 +35,26 @@
         # The jid that we're working on at the moment
         self.jid: Optional[str] = None
         # This is the sandbox we use
         self._sandbox: str = kwargs.pop(
             "sandbox", os.path.join(os.getcwd(), "reqless-py-workers")
         )
 
-    def kill(self, jid: str) -> None:
-        """The best way to do this is to fall on our sword"""
-        if jid == self.jid:
-            exit(1)
+    def halt_job_processing(self, jid: str) -> None:
+        """Since this method is most likely to be called by the listener, and
+        the worker is definitely running in a different thread from the
+        listenter, there's not a lot we can reliably do here. Trying to exit
+        would only kill the listener thread, while the thread doing the actual
+        work continued. So, in this scenario, we have to depend on the job
+        doing a good job of heartbeating since that's the best way for the job
+        to learn that it should halt. As such, do nothing."""
+        pass
 
     def run(self) -> None:
         """Run jobs, popping one after another"""
-        # Register our signal handlers
-        self.signals()
-
         with self.listener():
             for job in self.jobs():
                 # If there was no job to be had, we should sleep a little bit
                 if not job:
                     self.jid = None
                     set_title("Sleeping for %fs" % self.interval)
                     time.sleep(self.interval)
```

### Comparing `reqless-0.13.3/reqless/workers/util.py` & `reqless-1.0.0a0/reqless/workers/util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless/workers/worker.py` & `reqless-1.0.0a0/reqless/workers/base_worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 """Our base worker"""
 
 import json
-import os
-import signal
-import sys
 import threading
-import traceback
-from code import InteractiveConsole
 from contextlib import contextmanager
-from types import FrameType
-from typing import Any, Dict, Generator, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Generator, Iterable, List, Optional, Union
 
 from reqless import exceptions, logger
 from reqless.abstract import (
     AbstractClient,
     AbstractJob,
     AbstractQueue,
     AbstractQueueResolver,
 )
 from reqless.listener import Listener
 from reqless.queue_resolvers import TransformingQueueResolver
 
 
-class Worker:
-    """Worker. For doing work"""
+class BaseWorker:
+    """Base worker, for doing work"""
 
     def __init__(
         self,
         queues: Union[Iterable[Union[str, AbstractQueue]], AbstractQueueResolver],
         client: AbstractClient,
         interval: Optional[float] = None,
         resume: Optional[Union[bool, List[AbstractJob]]] = None,
@@ -106,67 +100,37 @@
             if not seen:
                 yield None
 
     @contextmanager
     def listener(self) -> Generator[None, None, None]:
         """Listen for pubsub messages relevant to this worker in a thread"""
         channels = ["ql:w:" + self.client.worker_name]
-        listener = Listener(self.client.redis, channels)
+        listener = Listener(self.client.database, channels)
         thread = threading.Thread(target=self.listen, args=(listener,))
         thread.start()
         try:
             yield
         finally:
             listener.unlisten()
             thread.join()
 
     def listen(self, listener: Listener) -> None:
         """Listen for events that affect our ownership of a job"""
         for message in listener.listen():
             try:
                 data = json.loads(message["data"])
                 if data["event"] in ("canceled", "lock_lost", "put"):
-                    self.kill(data["jid"])
+                    self.halt_job_processing(data["jid"])
             except Exception:
                 logger.exception("Pubsub error")
 
-    def kill(self, jid: str) -> None:
+    def halt_job_processing(self, jid: str) -> None:  # pragma: no cover
         """Stop processing the provided jid"""
-        raise NotImplementedError('Derived classes must override "kill"')
+        raise NotImplementedError('Derived classes must override "halt_job_processing"')
 
-    def run(self) -> None:
+    def run(self) -> None:  # pragma: no cover
         """Run this worker"""
         raise NotImplementedError('Derived classes must override "run"')
 
-    def signals(self, signals: Tuple[str, ...] = ("QUIT", "USR1", "USR2")) -> None:
-        """Register our signal handler"""
-        for sig in signals:
-            signal.signal(getattr(signal, "SIG" + sig), self.handler)
-
     def stop(self) -> None:
         """Mark this for shutdown"""
         self.shutdown = True
-
-    def handler(
-        self, signum: int, frame: Optional[FrameType]
-    ) -> None:  # pragma: no cover
-        """Signal handler for this process"""
-        if signum == signal.SIGQUIT:
-            # QUIT - Finish processing, but don't do any more work after that
-            self.stop()
-        elif signum == signal.SIGUSR1:
-            # USR1 - Print the backtrace
-            message = "".join(traceback.format_stack(frame))
-            message = "Signaled traceback for %s:\n%s" % (os.getpid(), message)
-            print(message, file=sys.stderr)
-            logger.warning(message)
-        elif signum == signal.SIGUSR2:
-            # USR2 - Enter a debugger
-            # Much thanks to http://stackoverflow.com/questions/132058
-            data = {"_frame": frame}  # Allow access to frame object.
-            if frame:
-                data.update(frame.f_globals)  # Unless shadowed by global
-                data.update(frame.f_locals)
-                # Build up a message with a traceback
-                message = "".join(traceback.format_stack(frame))
-            message = "Traceback:\n%s" % message
-            InteractiveConsole(data).interact(message)
```

### Comparing `reqless-0.13.3/reqless.egg-info/PKG-INFO` & `reqless-1.0.0a0/reqless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.3
-Summary: Redis-based Queue Management
+Version: 1.0.0a0
+Summary: Queue Management built on remote data structure stores like redis and valkey
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
-Keywords: job,qless,qmore,redis,reqless
+Keywords: job,qless,qmore,redis,reqless,valkey
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
@@ -33,34 +33,33 @@
 Requires-Dist: mypy~=1.8.0; extra == "dev"
 Requires-Dist: pre-commit~=2.20.0; extra == "dev"
 Requires-Dist: removestar~=1.3.1; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
 Requires-Dist: setproctitle~=1.3.3; extra == "dev"
 Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: types-decorator~=5.1.8.4; extra == "dev"
-Requires-Dist: types-mock~=5.1.0.2; extra == "dev"
 Requires-Dist: types-redis~=4.6.0.11; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
 Requires-Dist: coverage-badge~=1.1.0; extra == "test"
-Requires-Dist: mock; extra == "test"
 Requires-Dist: pytest~=7.4.0; extra == "test"
 Requires-Dist: setuptools>=69; extra == "test"
 Provides-Extra: all
 Requires-Dist: reqless[dev,test]; extra == "all"
 
 [![code coverage](https://github.com/tdg5/reqless-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/reqless-py/main/.meta/coverage/report.txt)
 [![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
 
 # reqless
 
 This is a fork of [seomoz/qless-py](https://github.com/seomoz/qless-py) that
 includes significant type improvements and support for throttles.
 
-`qless` is a powerful `Redis`-based job queueing system inspired by
+`qless` is a powerful job queueing system based on remote dictionary servers
+(like `redis` and `valkey`) inspired by
 [resque](https://github.com/defunkt/resque#readme), but built on a collection
 of Lua scripts, maintained in the
 [qless-core](https://github.com/tdg5/qless-core) repo.
 
 ## Philosophy and Nomenclature
 
 A `job` is a unit of work identified by a job id or `jid`. A `queue` can
@@ -459,19 +458,19 @@
 # Wait 5 minutes
 len(queue.pop(10))
 # => 5 jobs got popped
 ```
 
 ### Configuration Options
 
-You can get and set global (read: in the context of the same Redis instance)
-configuration to change the behavior for heartbeating, and so forth. There
-aren't a tremendous number of configuration options, but an important one is
-how long job data is kept around. Job data is expired after it has been
-completed for `jobs-history` seconds, but is limited to the last
+You can get and set global (in the context of the same remote dictionary
+server instance) configuration to change the behavior for heartbeating, and so
+forth. There aren't a tremendous number of configuration options, but an
+important one is how long job data is kept around. Job data is expired after it
+has been completed for `jobs-history` seconds, but is limited to the last
 `jobs-history-count` completed jobs. These default to 50k jobs, and 30 days,
 but depending on volume, your needs may change. To only keep the last 500 jobs
 for up to 7 days:
 
 ```python
 client.config["jobs-history"] = 7 * 86400
 client.config["jobs-history-count"] = 500
@@ -606,17 +605,17 @@
 Frankly, these are best viewed using the web app.
 
 ### Lua
 
 `qless` is a set of client language bindings, but the majority of the work is
 done in a collection of Lua scripts that comprise the
 [core](https://github.com/tdg5/qless-core) functionality. These scripts run
-on the Redis 2.6+ server atomically and allow for portability with the same
-functionality guarantees. Consult the documentation for `qless-core` to learn
-more about its internals.
+on `redis` and `valkey` 7.0+ server atomically and allow for portability with
+the same functionality guarantees. Consult the documentation for `qless-core`
+to learn more about its internals.
 
 ### Web App
 
 `qless` also comes with a web app for administrative tasks, like keeping tabs
 on the progress of jobs, tracking specific jobs, retrying failed jobs, etc.
 It's available in the [`qless`](https://github.com/tdg5/qless) library as a
 mountable [`Sinatra`](http://www.sinatrarb.com/) app. The web app is language
```

### Comparing `reqless-0.13.3/reqless.egg-info/SOURCES.txt` & `reqless-1.0.0a0/reqless.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -56,32 +56,35 @@
 reqless/qmore/__init__.py
 reqless/qmore/client.py
 reqless/queue_resolvers/__init__.py
 reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
 reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
 reqless/queue_resolvers/transforming_queue_resolver.py
 reqless/workers/__init__.py
-reqless/workers/forking.py
-reqless/workers/greenlet.py
-reqless/workers/serial.py
+reqless/workers/base_worker.py
+reqless/workers/forking_worker.py
+reqless/workers/gevent_worker.py
+reqless/workers/main_worker.py
+reqless/workers/serial_worker.py
+reqless/workers/signals.py
 reqless/workers/util.py
-reqless/workers/worker.py
 reqless_test/__init__.py
 reqless_test/common.py
 reqless_test/py.typed
 reqless_test/test_client.py
 reqless_test/test_config.py
 reqless_test/test_events.py
-reqless_test/test_forking.py
-reqless_test/test_greenlet.py
 reqless_test/test_importer.py
 reqless_test/test_job.py
 reqless_test/test_job_processor_api.py
 reqless_test/test_listener.py
-reqless_test/test_qmore_client.py
-reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
-reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
 reqless_test/test_queue.py
-reqless_test/test_serial.py
-reqless_test/test_transforming_queue_resolver.py
-reqless_test/test_worker.py
-reqless_test/test_worker_util.py
+reqless_test/qmore/test_qmore_client.py
+reqless_test/queue_resolvers/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
+reqless_test/queue_resolvers/test_qmore_dynamic_priority_queue_identifiers_transformer.py
+reqless_test/queue_resolvers/test_transforming_queue_resolver.py
+reqless_test/workers/test_base_worker.py
+reqless_test/workers/test_forking_worker.py
+reqless_test/workers/test_gevent_worker.py
+reqless_test/workers/test_main_worker.py
+reqless_test/workers/test_serial_worker.py
+reqless_test/workers/test_worker_util.py
```

### Comparing `reqless-0.13.3/reqless_test/common.py` & `reqless-1.0.0a0/reqless_test/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,60 @@
 """A base class for all of our common tests"""
 
+import json
 import logging
+import time
 import unittest
+from os import path
 from typing import List
 
-import redis
+from redis import Redis
 
 import reqless
+from reqless import logger
 from reqless.abstract import AbstractJob
 
 
+class BlockingJob:
+    """Job that can block until a given file is removed from the file system"""
+
+    @staticmethod
+    def process(job: AbstractJob) -> None:
+        """Dummy job"""
+        data_dict = json.loads(job.data)
+        blocker_file = data_dict.get("blocker_file")
+        if blocker_file:
+            while path.exists(blocker_file):
+                time.sleep(0.1)
+        try:
+            job.complete()
+        except Exception:
+            logger.exception("Unable to complete job %s" % job.jid)
+
+
 class NoopJob:
     @staticmethod
     def process(job: AbstractJob) -> None:
         job.complete()
 
 
 class TestReqless(unittest.TestCase):
     """Base class for all of our tests"""
 
-    redis: redis.Redis
+    database: Redis
 
     @classmethod
     def setUpClass(cls) -> None:
         reqless.logger.setLevel(logging.CRITICAL)
-        cls.redis = redis.Redis()
+        cls.database = Redis()
         # Clear the script cache, and nuke everything
-        cls.redis.execute_command("script", "flush")
+        cls.database.execute_command("script", "flush")
 
     def setUp(self) -> None:
-        all_keys: List = self.redis.keys("*")
+        all_keys: List = self.database.keys("*")
         assert len(all_keys) == 0
         # The reqless client we're using
         self.client = reqless.Client()
 
     def ensure_queues_exist(self, queue_names: List[str]) -> None:
         for queue_name in queue_names:
             queue = self.client.queues[queue_name]
@@ -41,8 +62,8 @@
                 jid = queue.put(NoopJob, "{}")
                 job = self.client.jobs[jid]
                 if job:
                     job.cancel()
 
     def tearDown(self) -> None:
         # Ensure that we leave no keys behind, and that we've unfrozen time
-        self.redis.flushdb()
+        self.database.flushdb()
```

### Comparing `reqless-0.13.3/reqless_test/test_client.py` & `reqless-1.0.0a0/reqless_test/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Basic tests about the client"""
 
 from typing import List
 
 from reqless import retry
 from reqless.abstract import AbstractClient, AbstractJob
-from reqless.workers.worker import Worker
+from reqless.workers.base_worker import BaseWorker
 from reqless_test.common import TestReqless
 
 
 def pop_one(client: AbstractClient, queue_name: str) -> AbstractJob:
     job = client.queues[queue_name].pop()
     assert job is not None and not isinstance(job, List)
     return job
@@ -190,15 +190,15 @@
 
 class TestWorkers(TestReqless):
     """Test the Workers class"""
 
     def setUp(self) -> None:
         TestReqless.setUp(self)
         self.client.worker_name = "worker"
-        self.worker = Worker(["foo"], self.client)
+        self.worker = BaseWorker(["foo"], self.client)
 
     def test_individual(self) -> None:
         """Gives us access to individual workers"""
         self.client.queues["foo"].put("reqless_test.common.NoopJob", "{}", jid="jid")
         self.assertEqual(self.client.workers["worker"], {"jobs": [], "stalled": []})
         job = next(self.worker.jobs())
         assert job is not None
```

### Comparing `reqless-0.13.3/reqless_test/test_config.py` & `reqless-1.0.0a0/reqless_test/test_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless_test/test_events.py` & `reqless-1.0.0a0/reqless_test/test_events.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless_test/test_forking.py` & `reqless-1.0.0a0/reqless_test/workers/test_forking_worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Test the forking worker"""
 
 import json
 import os
 import signal
 import time
 from threading import Thread
-from typing import Optional, Tuple
+from typing import Optional
 
 from reqless.abstract import AbstractJob
-from reqless.workers.forking import ForkingWorker
-from reqless.workers.worker import Worker
+from reqless.workers.base_worker import BaseWorker
+from reqless.workers.forking_worker import ForkingWorker
 from reqless_test.common import TestReqless
 
 
 class Foo:
     """Dummy class"""
 
     @staticmethod
@@ -34,20 +34,20 @@
         job.complete()
         os.kill(os.getpid(), signal.SIGKILL)
 
 
 class PatchedForkingWorker(ForkingWorker):
     """A forking worker that doesn't register signal handlers"""
 
-    def signals(self, signals: Tuple[str, ...] = ()) -> None:
+    def before_run(self) -> None:
         """Do not actually register signal handlers"""
         pass
 
 
-class TestWorker(TestReqless):
+class TestForkingWorker(TestReqless):
     """Test the worker"""
 
     def setUp(self) -> None:
         TestReqless.setUp(self)
         self.client.worker_name = "worker"
         self.worker = PatchedForkingWorker(["foo"], self.client, workers=1, interval=1)
         self.queue = self.client.queues["foo"]
@@ -82,15 +82,15 @@
         assert isinstance(job, AbstractJob)
         self.assertEqual(json.loads(job.data)["cwd"], expected)
 
     def test_spawn_klass_string(self) -> None:
         """Should be able to import by class string"""
         worker = PatchedForkingWorker(
             client=self.client,
-            klass="reqless.workers.serial.SerialWorker",
+            klass="reqless.workers.serial_worker.SerialWorker",
             queues=["foo"],
         )
-        self.assertIsInstance(worker.spawn(), Worker)
+        self.assertIsInstance(worker.spawn(), BaseWorker)
 
     def test_spawn(self) -> None:
         """It gives us back a worker instance"""
-        self.assertIsInstance(self.worker.spawn(), Worker)
+        self.assertIsInstance(self.worker.spawn(), BaseWorker)
```

### Comparing `reqless-0.13.3/reqless_test/test_greenlet.py` & `reqless-1.0.0a0/reqless_test/workers/test_gevent_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from threading import Thread
 from typing import Generator, Optional
 
 import gevent
 
 from reqless.abstract import AbstractJob, AbstractQueue
 from reqless.listener import Listener
-from reqless.workers.greenlet import GeventWorker
+from reqless.workers.gevent_worker import GeventWorker
 from reqless_test.common import TestReqless
 
 
 class GeventJob:
     """Dummy class"""
 
     @staticmethod
@@ -40,15 +40,15 @@
             yield next(generator)
 
     def listen(self, listener: Listener) -> None:
         """Don't actually listen for pubsub events"""
         pass
 
 
-class TestWorker(TestReqless):
+class TestGeventWorker(TestReqless):
     """Test the worker"""
 
     def setUp(self) -> None:
         TestReqless.setUp(self)
         self.worker = PatchedGeventWorker(
             ["foo"], self.client, greenlets=1, interval=0.2
         )
@@ -82,20 +82,20 @@
         """Make sure the client sleeps if there aren't jobs to be had"""
         for _ in range(4):
             self.queue.put(GeventJob, "{}")
         before = time.time()
         self.worker.run()
         self.assertGreater(time.time() - before, 0.2)
 
-    def test_kill(self) -> None:
-        """Can kill greenlets when it loses its lock"""
+    def test_halt_job_processing(self) -> None:
+        """Can halt_job_processing greenlets when it loses its lock"""
         worker = PatchedGeventWorker(["foo"], self.client)
         greenlet = gevent.spawn(gevent.sleep, 1)
         worker.greenlets["foo"] = greenlet
-        worker.kill("foo")
+        worker.halt_job_processing("foo")
         greenlet.join()
         self.assertIsInstance(greenlet.value, gevent.GreenletExit)
 
-    def test_kill_dead(self) -> None:
+    def test_halt_job_processing_dead(self) -> None:
         """Does not panic if the greenlet handling a job is no longer around"""
         # This test succeeds if it finishes without an exception
-        self.worker.kill("foo")
+        self.worker.halt_job_processing("foo")
```

### Comparing `reqless-0.13.3/reqless_test/test_importer.py` & `reqless-1.0.0a0/reqless_test/test_importer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import mock
+from unittest import mock
 
 from reqless.importer import Importer
 from reqless_test.common import TestReqless
 
 
 class ImporterTestClass:
     pass
```

### Comparing `reqless-0.13.3/reqless_test/test_job.py` & `reqless-1.0.0a0/reqless_test/test_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             "reqless_test.test_job.Foo", "{}", jid="c", depends=["a"]
         )
         job = self.get_job("c")
         self.assertEqual(job.dependencies, ["a"])
         job.depend("b")
         job = self.get_job("c")
         actual_dependencies = job.dependencies
-        # Redis sets have an undefined order
+        # DB server sets have an undefined order
         actual_dependencies.sort()
         self.assertEqual(actual_dependencies, ["a", "b"])
         job.undepend("a")
         job = self.get_job("c")
         self.assertEqual(job.dependencies, ["b"])
         job.undepend(all=True)
         job = self.get_job("c")
```

### Comparing `reqless-0.13.3/reqless_test/test_job_processor_api.py` & `reqless-1.0.0a0/reqless_test/test_job_processor_api.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless_test/test_listener.py` & `reqless-1.0.0a0/reqless_test/test_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         def func(message: Dict) -> None:
             nonlocal count
             count += 1
             self.assertEqual("ql:popped", message["channel"])
             self.assertEqual("message", message["type"])
             self.assertEqual("jid", message["data"])
 
-        listener = Listener(channels=["ql:popped"], redis=self.client.redis)
+        listener = Listener(channels=["ql:popped"], database=self.client.database)
 
         def publish() -> None:
             for message in listener.listen():
                 func(message)
 
         thread = Thread(target=publish)
         thread.start()
```

### Comparing `reqless-0.13.3/reqless_test/test_qmore_client.py` & `reqless-1.0.0a0/reqless_test/qmore/test_qmore_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,49 +9,49 @@
 )
 from reqless_test.common import TestReqless
 
 
 class TestQmoreClient(TestReqless):
     def setUp(self) -> None:
         TestReqless.setUp(self)
-        self.redis = self.client.redis
-        self.subject = QmoreClient(redis=self.client.redis)
+        self.database = self.client.database
+        self.subject = QmoreClient(database=self.client.database)
 
     def test_get_queue_identifier_patterns(self) -> None:
         """It fetches the expected queue identifier patterns"""
         mapping = {"one": ["one", "two*", "!three"], "four": ["four", "five"]}
         json_mapping: Mapping[Union[bytes, str], Union[bytes, float, int, str]] = {
             key: json.dumps(value) for key, value in mapping.items()
         }
-        self.redis.hset(QUEUE_IDENTIFIER_PATTERNS_KEY, mapping=json_mapping)
+        self.database.hset(QUEUE_IDENTIFIER_PATTERNS_KEY, mapping=json_mapping)
         fetched_mapping = self.subject.get_queue_identifier_patterns()
         self.assertEqual({"default": "*", **mapping}, fetched_mapping)
 
     def test_set_queue_identifier_patterns(self) -> None:
         """It sets the expected queue identifier patterns"""
         mapping = {"not_three": ["one", "two*", "!three"], "five": ["four", "five"]}
         self.subject.set_queue_identifier_patterns(mapping)
-        serialized_patterns = self.redis.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
+        serialized_patterns = self.database.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
         patterns = {
             identifier: json.loads(json_patterns)
             for identifier, json_patterns in serialized_patterns.items()
         }
         self.assertEqual(mapping, patterns)
 
     def test_set_queue_identifier_patterns_with_no_patterns(self) -> None:
         """It clears any existing patterns and does not try to hset without a mapping"""
         # Make sure there's something there to clear out
         mapping = {"not_three": ["one", "two*", "!three"], "five": ["four", "five"]}
         self.subject.set_queue_identifier_patterns(mapping)
-        serialized_patterns = self.redis.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
+        serialized_patterns = self.database.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
         self.assertEqual(2, len(serialized_patterns))
 
         empty_mapping: Dict[str, List[str]] = {}
         self.subject.set_queue_identifier_patterns(empty_mapping)
-        serialized_patterns = self.redis.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
+        serialized_patterns = self.database.hgetall(QUEUE_IDENTIFIER_PATTERNS_KEY)
         patterns = {
             identifier: json.loads(json_patterns)
             for identifier, json_patterns in serialized_patterns.items()
         }
         self.assertEqual(empty_mapping, patterns)
 
     def test_get_queue_priority_patterns(self) -> None:
@@ -64,15 +64,15 @@
                 {
                     "fairly": queue_priority.should_distribute_fairly,
                     "pattern": ",".join(queue_priority.patterns),
                 }
             )
             for queue_priority in given_queue_priorities
         ]
-        pipeline = self.redis.pipeline()
+        pipeline = self.database.pipeline()
         pipeline.delete(QUEUE_PRIORITY_PATTERNS_KEY)
         for serialized_queue_priority in serialized_queue_priorities:
             pipeline.rpush(QUEUE_PRIORITY_PATTERNS_KEY, serialized_queue_priority)
         pipeline.execute()
         queue_priorities = self.subject.get_queue_priority_patterns()
         zipped_queue_priorities = zip(given_queue_priorities, queue_priorities)
         for given_queue_priority, queue_priority in zipped_queue_priorities:
@@ -84,15 +84,15 @@
 
     def test_set_queue_priority_patterns(self) -> None:
         """It sets the expected queue identifier patterns"""
         given_queue_priorities = [
             QueuePriorityPattern(patterns=["*"], should_distribute_fairly=True),
         ]
         self.subject.set_queue_priority_patterns(given_queue_priorities)
-        serialized_queue_priorities = self.redis.lrange(
+        serialized_queue_priorities = self.database.lrange(
             QUEUE_PRIORITY_PATTERNS_KEY, 0, -1
         )
         queue_priorities = []
         for serialized_queue_priority in serialized_queue_priorities:
             queue_priority_data = json.loads(serialized_queue_priority)
             patterns = [
                 pattern.strip() for pattern in queue_priority_data["pattern"].split(",")
```

### Comparing `reqless-0.13.3/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-1.0.0a0/reqless_test/queue_resolvers/test_qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from reqless_test.common import TestReqless
 
 
 class TestQmoreDynamicMappingQueueIdentifiersTransformer(TestReqless):
     def setUp(self) -> None:
         TestReqless.setUp(self)
-        self.qmore_client = QmoreClient(redis=self.client.redis)
+        self.qmore_client = QmoreClient(database=self.client.database)
 
     def set_dynamic_queues(self, mapping: Dict[str, List[str]]) -> None:
         self.qmore_client.set_queue_identifier_patterns(mapping)
 
     def collect_queue_names(
         self,
         dynamic_queue_mapping: Dict[str, List[str]],
```

### Comparing `reqless-0.13.3/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-1.0.0a0/reqless_test/queue_resolvers/test_qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from reqless_test.common import TestReqless
 
 
 class TestQmoreDynamicPriorityQueueIdentifiersTransformer(TestReqless):
     def setUp(self) -> None:
         TestReqless.setUp(self)
-        self.qmore_client = QmoreClient(redis=self.client.redis)
+        self.qmore_client = QmoreClient(database=self.client.database)
         # We use many queues to reduce the chances that we shuffle a list into
         # the same order.
         # Identifiers are [a1a, a2a, a3a, ... g1g, g2g, g3g]  # noqa: SC100
         self.queue_identifiers: List[str] = [
             f"{chr(97 + ascii_offset)}{index}{chr(97 + ascii_offset)}"
             for ascii_offset in range(7)
             for index in range(1, 4)
```

### Comparing `reqless-0.13.3/reqless_test/test_queue.py` & `reqless-1.0.0a0/reqless_test/test_queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless_test/test_serial.py` & `reqless-1.0.0a0/reqless_test/workers/test_serial_worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,135 +1,107 @@
 """Test the serial worker"""
 
 import json
 import time
-from os import path
 from tempfile import NamedTemporaryFile
 from threading import Thread
-from typing import Generator, Optional, Tuple
+from typing import Generator, Optional
 
-from reqless import logger
 from reqless.abstract import AbstractJob
 from reqless.listener import Listener
-from reqless.workers.serial import SerialWorker
-from reqless_test.common import TestReqless
+from reqless.workers.serial_worker import SerialWorker
+from reqless_test.common import BlockingJob, TestReqless
 
 
-class SerialJob:
-    """Dummy class"""
-
-    @staticmethod
-    def foo(job: AbstractJob) -> None:
-        """Dummy job"""
-        data_dict = json.loads(job.data)
-        blocker_file = data_dict.get("blocker_file")
-        if blocker_file:
-            while path.exists(blocker_file):
-                time.sleep(0.1)
-        try:
-            job.complete()
-        except Exception:
-            logger.exception("Unable to complete job %s" % job.jid)
-
-
-class Worker(SerialWorker):
-    """A worker that limits the number of jobs it runs"""
-
+class ShortLivedSerialWorker(SerialWorker):
     def jobs(self) -> Generator[Optional[AbstractJob], None, None]:
-        """Yield only a few jobs"""
         generator = SerialWorker.jobs(self)
         for _ in range(5):
             yield next(generator)
 
-    def kill(self, jid: str) -> None:
-        """We'll push a message to redis instead of falling on our sword"""
-        self.client.redis.rpush("foo", jid)
-        raise KeyboardInterrupt()
-
-    def signals(self, signals: Tuple[str, ...] = ()) -> None:
-        """Do not set any signal handlers"""
-        pass
-
+    def halt_job_processing(self, jid: str) -> None:
+        self.client.database.rpush("foo", jid)
 
-class NoListenWorker(Worker):
-    """A worker that just won't listen"""
 
+class NoListenSerialWorker(ShortLivedSerialWorker):
     def listen(self, listener: Listener) -> None:
-        """Don't listen for lost locks"""
         pass
 
 
-class TestWorker(TestReqless):
+class TestSerialWorker(TestReqless):
     """Test the worker"""
 
     def setUp(self) -> None:
         TestReqless.setUp(self)
         self.queue = self.client.queues["foo"]
         self.thread: Optional[Thread] = None
 
     def tearDown(self) -> None:
         if self.thread:
             self.thread.join()
         TestReqless.tearDown(self)
 
     def test_basic(self) -> None:
         """Can complete jobs in a basic way"""
-        jids = [self.queue.put(SerialJob, "{}") for _ in range(5)]
-        NoListenWorker(["foo"], self.client, interval=0.2).run()
+        jids = [self.queue.put(BlockingJob, "{}") for _ in range(5)]
+        NoListenSerialWorker(["foo"], self.client, interval=0.2).run()
         states = []
         for jid in jids:
             job = self.client.jobs[jid]
             assert job is not None and isinstance(job, AbstractJob)
             states.append(job.state)
         self.assertEqual(states, ["complete"] * 5)
 
     def test_jobs(self) -> None:
         """The jobs method yields None if there are no jobs"""
-        worker = NoListenWorker(["foo"], self.client, interval=0.2)
+        worker = NoListenSerialWorker(["foo"], self.client, interval=0.2)
         self.assertEqual(next(worker.jobs()), None)
 
     def test_sleeps(self) -> None:
         """Make sure the client sleeps if there aren't jobs to be had"""
         for _ in range(4):
-            self.queue.put(SerialJob, "{}")
+            self.queue.put(BlockingJob, "{}")
         before = time.time()
-        NoListenWorker(["foo"], self.client, interval=0.2).run()
+        NoListenSerialWorker(["foo"], self.client, interval=0.2).run()
         self.assertGreater(time.time() - before, 0.2)
 
     def test_lost_locks(self) -> None:
         """The worker should be able to stop processing if need be"""
         temp_file = NamedTemporaryFile()
-        jid = self.queue.put(SerialJob, json.dumps({"blocker_file": temp_file.name}))
-        self.thread = Thread(target=Worker(["foo"], self.client, interval=0.2).run)
+        jid = self.queue.put(BlockingJob, json.dumps({"blocker_file": temp_file.name}))
+        self.thread = Thread(
+            target=ShortLivedSerialWorker(["foo"], self.client, interval=0.2).run
+        )
         self.thread.start()
         job = self.client.jobs[jid]
         assert job is not None and isinstance(job, AbstractJob)
-        # Now, we'll timeout one of the jobs and ensure that kill is invoked
+        # Now, we'll timeout one of the jobs and ensure that
+        # halt_job_processing is invoked
         while job.state != "running":
             time.sleep(0.01)
             job = self.client.jobs[jid]
             assert job is not None and isinstance(job, AbstractJob)
         job.timeout()
         temp_file.close()
-        self.assertEqual(self.client.redis.brpop(["foo"], 1), ("foo", jid))
+        self.assertEqual(self.client.database.brpop(["foo"], 1), ("foo", jid))
 
-    def test_kill(self) -> None:
+    def test_halt_job_processing(self) -> None:
         """Should be able to fall on its sword if need be"""
         worker = SerialWorker([], self.client)
         worker.jid = "foo"
-        thread = Thread(target=worker.kill, args=(worker.jid,))
+        thread = Thread(target=worker.halt_job_processing, args=(worker.jid,))
         thread.start()
         thread.join()
         self.assertFalse(thread.is_alive())
 
-    def test_kill_dead(self) -> None:
+    def test_halt_job_processing_dead(self) -> None:
         """If we've moved on to another job, say so"""
         # If this tests runs to completion, it has succeeded
         worker = SerialWorker([], self.client)
-        worker.kill("foo")
+        worker.halt_job_processing("foo")
 
     def test_shutdown(self) -> None:
         """We should be able to shutdown a serial worker"""
         # If this test finishes, it passes
         worker = SerialWorker([], self.client, interval=0.1)
         worker.stop()
         worker.run()
```

### Comparing `reqless-0.13.3/reqless_test/test_transforming_queue_resolver.py` & `reqless-1.0.0a0/reqless_test/queue_resolvers/test_transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/reqless_test/test_worker.py` & `reqless-1.0.0a0/reqless_test/workers/test_base_worker.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,80 +3,80 @@
 from typing import List
 
 import reqless
 from reqless.abstract import AbstractClient, AbstractJob
 from reqless.queue_resolvers.transforming_queue_resolver import (
     TransformingQueueResolver,
 )
-from reqless.workers.worker import Worker
+from reqless.workers.base_worker import BaseWorker
 from reqless_test.common import TestReqless
 
 
-class TestWorker(TestReqless):
+class TestBaseWorker(TestReqless):
     """Test the worker"""
 
     def setUp(self) -> None:
         TestReqless.setUp(self)
         self.client.worker_name = "worker"
-        self.worker = Worker(["foo"], self.client)
+        self.worker = BaseWorker(["foo"], self.client)
 
-    def test_kill(self) -> None:
-        """The base worker class' kill method should raise an exception"""
-        self.assertRaises(NotImplementedError, self.worker.kill, 1)
+    def test_halt_job_processing(self) -> None:
+        """The base worker class' halt_job_processing method should raise an
+        exception"""
+        self.assertRaises(NotImplementedError, self.worker.halt_job_processing, 1)
 
     def test_resume(self) -> None:
         """We should be able to resume jobs"""
         queue = self.worker.client.queues["foo"]
         queue.put("reqless_test.common.NoopJob", "{}")
-        job = self.client.queues["foo"].peek()
-        assert isinstance(job, AbstractJob)
+        job = self.pop_one(self.client, "foo")
         # Now, we'll create a new worker and make sure it gets that job first
-        worker = Worker(["foo"], self.client, resume=[job])
+        worker = BaseWorker(["foo"], self.client, resume=[job])
         job_from_worker = next(worker.jobs())
         assert job_from_worker is not None and isinstance(job_from_worker, AbstractJob)
         self.assertEqual(job_from_worker.jid, job.jid)
 
     def test_unresumable(self) -> None:
         """If we can't heartbeat jobs, we should not try to resume it"""
         queue = self.worker.client.queues["foo"]
         queue.put("reqless_test.common.NoopJob", "{}")
         # Pop from another worker
         other = reqless.Client(hostname="other")
         job = self.pop_one(other, "foo")
         # Now, we'll create a new worker and make sure it gets that job first
         job_again = self.client.jobs[job.jid]
         assert job_again is not None and isinstance(job_again, AbstractJob)
-        worker = Worker(["foo"], self.client, resume=[job_again])
+        worker = BaseWorker(["foo"], self.client, resume=[job_again])
         self.assertEqual(next(worker.jobs()), None)
 
     def test_resumable(self) -> None:
         """We should be able to find all the jobs that can be resumed"""
         # We're going to put some jobs into some queues, and pop them.
         jid = self.client.queues["foo"].put("reqless_test.common.NoopJob", "{}")
         self.client.queues["bar"].put("reqless_test.common.NoopJob", "{}")
         self.pop_one(self.client, "foo")
         self.pop_one(self.client, "bar")
 
         # Now, we should be able to see a resumable job in 'foo', but we should
         # not see the job that we popped from 'bar'
-        worker = Worker(["foo"], self.client, resume=True)
+        worker = BaseWorker(["foo"], self.client, resume=True)
         jids = [job.jid for job in worker.resume]
         self.assertEqual(jids, [jid])
 
     def test_queue_resolver_when_list_of_queues_given(self) -> None:
         """When given a list of queues, it wraps them in a queue resolver"""
         queue_names = ["foo"]
-        worker = Worker(queue_names, self.client)
+        worker = BaseWorker(queue_names, self.client)
         self.assertEqual(queue_names, worker.queue_resolver.resolve())
 
     def test_queue_resolver_when_queue_resolver_given(self) -> None:
         """When given a queue resolver, it takes it without modification"""
         queue_names = ["foo"]
         queue_resolver = TransformingQueueResolver(queue_identifiers=queue_names)
-        worker = Worker(client=self.client, queues=queue_resolver)
+        worker = BaseWorker(client=self.client, queues=queue_resolver)
         self.assertEqual(queue_resolver, worker.queue_resolver)
         self.assertEqual(queue_names, worker.queue_resolver.resolve())
 
     def pop_one(self, client: AbstractClient, queue_name: str) -> AbstractJob:
         job = client.queues[queue_name].pop()
         assert job is not None and not isinstance(job, List)
         return job
```

### Comparing `reqless-0.13.3/reqless_test/test_worker_util.py` & `reqless-1.0.0a0/reqless_test/workers/test_worker_util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.3/requirements.txt` & `reqless-1.0.0a0/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 isort==5.8.0
 jaraco.classes==3.3.0
 jeepney==0.8.0
 keyring==24.3.0
 markdown-it-py==3.0.0
 mccabe==0.7.0
 mdurl==0.1.2
-mock==1.3.0
 more-itertools==10.1.0
 mypy==1.8.0
 mypy-extensions==1.0.0
 nh3==0.2.15
 nodeenv==1.8.0
 packaging==23.2
 pathspec==0.11.2
@@ -64,15 +63,14 @@
 SecretStorage==3.3.3
 setproctitle==1.3.3
 six==1.16.0
 toml==0.10.2
 tomli==2.0.1
 twine==4.0.2
 types-decorator==5.1.8.4
-types-mock==5.1.0.2
 types-pyOpenSSL==24.0.0.20240311
 types-redis==4.6.0.11
 typing_extensions==4.8.0
 urllib3==2.1.0
 virtualenv==20.24.7
 zipp==3.17.0
 zope.event==5.0
```

### Comparing `reqless-0.13.3/whitelist.txt` & `reqless-1.0.0a0/whitelist.txt`

 * *Files identical despite different names*

