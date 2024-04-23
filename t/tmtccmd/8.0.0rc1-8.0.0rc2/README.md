# Comparing `tmp/tmtccmd-8.0.0rc1.tar.gz` & `tmp/tmtccmd-8.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmtccmd-8.0.0rc1.tar", last modified: Wed Jan 24 15:32:53 2024, max compression
+gzip compressed data, was "tmtccmd-8.0.0rc2.tar", last modified: Tue Apr 23 12:14:21 2024, max compression
```

## Comparing `tmtccmd-8.0.0rc1.tar` & `tmtccmd-8.0.0rc2.tar`

### file list

```diff
@@ -1,265 +1,244 @@
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.175665 tmtccmd-8.0.0rc1/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    20743 2024-01-24 15:28:28.000000 tmtccmd-8.0.0rc1/CHANGELOG.md
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11359 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/LICENSE-APACHE
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1061 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/LICENSE-MIT
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      227 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/MANIFEST.in
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      177 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/NOTICE
--rw-r--r--   0 rmueller  (1000) rmueller  (1000)     6575 2024-01-24 15:32:53.175665 tmtccmd-8.0.0rc1/PKG-INFO
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5118 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.151665 tmtccmd-8.0.0rc1/docs/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        5 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/docs/.gitignore
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.151665 tmtccmd-8.0.0rc1/docs/.pytest_cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-11-10 16:41:10.000000 tmtccmd-8.0.0rc1/docs/.pytest_cache/.gitignore
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-11-10 16:41:10.000000 tmtccmd-8.0.0rc1/docs/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-11-10 16:41:10.000000 tmtccmd-8.0.0rc1/docs/.pytest_cache/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.143665 tmtccmd-8.0.0rc1/docs/.pytest_cache/v/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.151665 tmtccmd-8.0.0rc1/docs/.pytest_cache/v/cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-10 16:41:10.000000 tmtccmd-8.0.0rc1/docs/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-10 16:41:10.000000 tmtccmd-8.0.0rc1/docs/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      634 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/docs/Makefile
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.151665 tmtccmd-8.0.0rc1/docs/api/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      168 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/docs/api/cfdp.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1546 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/api/com.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1435 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/docs/api/config.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      741 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/api/core.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      239 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/api/fsfw.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      212 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/api/logging.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4120 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/api/pus.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      640 2023-11-29 16:48:58.000000 tmtccmd-8.0.0rc1/docs/api/tc.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      497 2024-01-24 12:12:43.000000 tmtccmd-8.0.0rc1/docs/api/tm.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1440 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/docs/api/util.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      127 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/api/version.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1263 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/docs/api.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      356 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/docs/cfdp.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5275 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/communication.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3261 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/docs/conf.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8477 2023-11-29 17:07:41.000000 tmtccmd-8.0.0rc1/docs/gettingstarted.rst
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.151665 tmtccmd-8.0.0rc1/docs/images/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    13571 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/docs/images/example_system.drawio
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   148156 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/docs/images/example_system.png
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   116372 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/docs/images/tmtccmd_usage.PNG
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   268138 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/docs/images/tmtccmd_usage.graphml
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   198496 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/docs/images/tmtccmd_usage.pdf
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1134 2024-01-24 15:05:22.000000 tmtccmd-8.0.0rc1/docs/index.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3192 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/docs/introduction.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      760 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/docs/make.bat
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       24 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/docs/requirements.txt
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.143665 tmtccmd-8.0.0rc1/examples/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.151665 tmtccmd-8.0.0rc1/examples/app/
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)    13742 2023-11-29 16:35:49.000000 tmtccmd-8.0.0rc1/examples/app/tmtcc.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.151665 tmtccmd-8.0.0rc1/misc/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8164 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/misc/logo-tiny.png
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    55175 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/misc/logo_medium.png
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1651 2024-01-24 15:32:43.000000 tmtccmd-8.0.0rc1/pyproject.toml
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       12 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/requirements.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       38 2024-01-24 15:32:53.175665 tmtccmd-8.0.0rc1/setup.cfg
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.155665 tmtccmd-8.0.0rc1/tests/
--rw-r--r--   0 rmueller  (1000) rmueller  (1000)    69632 2023-10-08 21:43:09.000000 tmtccmd-8.0.0rc1/tests/.coverage
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        4 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/.gitignore
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.155665 tmtccmd-8.0.0rc1/tests/.pytest_cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-10-02 08:23:01.000000 tmtccmd-8.0.0rc1/tests/.pytest_cache/.gitignore
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-10-02 08:23:01.000000 tmtccmd-8.0.0rc1/tests/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-10-02 08:23:01.000000 tmtccmd-8.0.0rc1/tests/.pytest_cache/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.143665 tmtccmd-8.0.0rc1/tests/.pytest_cache/v/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.155665 tmtccmd-8.0.0rc1/tests/.pytest_cache/v/cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1496 2023-11-20 22:09:47.000000 tmtccmd-8.0.0rc1/tests/.pytest_cache/v/cache/lastfailed
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    16899 2023-11-20 22:09:47.000000 tmtccmd-8.0.0rc1/tests/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-20 22:09:47.000000 tmtccmd-8.0.0rc1/tests/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/__init__.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.155665 tmtccmd-8.0.0rc1/tests/com/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/com/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      822 2024-01-24 11:59:01.000000 tmtccmd-8.0.0rc1/tests/com/test_dummy.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2448 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/com/test_serial_cobs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2320 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/com/test_serial_dle.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3754 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/com/test_tcp.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1638 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/com/test_udp.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1930 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/com/test_utils.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.155665 tmtccmd-8.0.0rc1/tests/config/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.155665 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-11-16 22:59:45.000000 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/.gitignore
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-11-16 22:59:45.000000 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-11-16 22:59:45.000000 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.143665 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/v/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/v/cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-20 21:26:01.000000 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/v/cache/lastfailed
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2247 2023-11-20 21:26:01.000000 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-20 21:26:01.000000 tmtccmd-8.0.0rc1/tests/config/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/config/__init__.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/config/log/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      860 2023-11-16 22:57:04.000000 tmtccmd-8.0.0rc1/tests/config/log/tmtccmd_raw_pus_2023-11-16.log
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      590 2023-11-16 22:57:04.000000 tmtccmd-8.0.0rc1/tests/config/log/tmtccmd_raw_pus_2023-11-16.log.1
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8348 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tests/config/test_args_conversion.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2744 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tests/config/test_args_parsing.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3644 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tests/config/test_cfdp_conversions.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    16512 2023-11-29 16:35:49.000000 tmtccmd-8.0.0rc1/tests/config/test_cmd_def_tree.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4409 2023-11-29 16:35:49.000000 tmtccmd-8.0.0rc1/tests/config/test_prompt.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      286 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tests/hook_obj_mock.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/pus/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-10-16 20:55:49.000000 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/.gitignore
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-10-16 20:55:49.000000 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-10-16 20:55:49.000000 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.147665 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/v/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/v/cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      843 2023-10-16 20:55:49.000000 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-10-16 20:55:49.000000 tmtccmd-8.0.0rc1/tests/pus/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/pus/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    10964 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/pus/test_srv20.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/tc/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/tc/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1121 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/tc/test_srv20.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8807 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tests/test_backend.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1905 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tests/test_printer.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6925 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/test_pus_verif_log.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4927 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tests/test_queue.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9187 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tests/test_seq_sender.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2676 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/test_tm_handler.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2200 2024-01-24 14:54:50.000000 tmtccmd-8.0.0rc1/tests/test_util.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/tm/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-10-16 20:55:58.000000 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/.gitignore
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-10-16 20:55:58.000000 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-10-16 20:55:58.000000 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.147665 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/v/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/v/cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       64 2023-10-16 21:03:56.000000 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/v/cache/lastfailed
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      485 2023-10-16 21:07:53.000000 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-10-16 21:07:53.000000 tmtccmd-8.0.0rc1/tests/tm/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tests/tm/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1395 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/tm/test_srv1.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1295 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/tm/test_srv17.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1593 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/tm/test_srv20.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      532 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/tm/test_srv200.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1491 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tests/tm/test_srv5.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.159665 tmtccmd-8.0.0rc1/tmtccmd/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8693 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/__init__.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.163665 tmtccmd-8.0.0rc1/tmtccmd/cfdp/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      320 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/cfdp/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1054 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/cfdp/request.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.163665 tmtccmd-8.0.0rc1/tmtccmd/com/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3180 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5242 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/com/dummy.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    19386 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/qemu.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7949 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/ser_utils.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2469 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/serial_base.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3768 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/serial_cobs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4239 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/serial_dle.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8127 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/tcp.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6977 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/tcpip_utils.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2980 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/udp.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2551 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/com/utils.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      187 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tmtccmd/com_if.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.163665 tmtccmd-8.0.0rc1/tmtccmd/config/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4677 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/config/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    29707 2023-11-29 16:35:49.000000 tmtccmd-8.0.0rc1/tmtccmd/config/args.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3181 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/config/cfdp.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9279 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/config/com.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3223 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/config/defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6001 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/config/globals.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3335 2023-11-29 16:40:50.000000 tmtccmd-8.0.0rc1/tmtccmd/config/hook.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      550 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tmtccmd/config/objects.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12235 2023-11-29 17:31:16.000000 tmtccmd-8.0.0rc1/tmtccmd/config/prompt.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    17106 2024-01-24 14:59:14.000000 tmtccmd-8.0.0rc1/tmtccmd/config/tmtc.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.167665 tmtccmd-8.0.0rc1/tmtccmd/core/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      140 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tmtccmd/core/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      409 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/core/backend_base.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      938 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/core/backend_state.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1484 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/core/base.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9444 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/core/ccsds_backend.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1830 2023-11-18 11:25:43.000000 tmtccmd-8.0.0rc1/tmtccmd/core/globals_manager.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.167665 tmtccmd-8.0.0rc1/tmtccmd/fsfw/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3097 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/fsfw/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7301 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/fsfw/tmtc_printer.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.167665 tmtccmd-8.0.0rc1/tmtccmd/gui/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       35 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tmtccmd/gui/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6971 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/gui/buttons.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4802 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/gui/cmd_select.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2153 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/gui/defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12835 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/gui/frontend.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6835 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/gui/worker.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.167665 tmtccmd-8.0.0rc1/tmtccmd/logging/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4654 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/logging/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7494 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/logging/pus.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.171665 tmtccmd-8.0.0rc1/tmtccmd/pus/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6983 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      100 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s11_tc_sched.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1854 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s11_tc_sched_defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       92 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s17_test.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       75 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s17_test_defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      130 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s1_verification.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      161 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s200_fsfw_mode.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      259 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s200_fsfw_mode_defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      108 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s201_fsfw_health.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      148 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s201_fsfw_health_defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      155 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s20_fsfw_param.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    15855 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s20_fsfw_param_defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       94 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s3_fsfw_hk.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      234 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s5_fsfw_event.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      621 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s5_fsfw_event_defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      194 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s5_satrs_event.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      657 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s5_satrs_event_defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      244 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s8_fsfw_action.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      104 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/s8_fsfw_action_defs.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.171665 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2779 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s11_tc_sched.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      681 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s17_test.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2106 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s200_fsfw_mode.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      311 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s201_fsfw_health.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6537 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s20_fsfw_param.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5750 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s3_fsfw_hk.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1242 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s5_event.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1128 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s8_fsfw_action.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.171665 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      510 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s1_verification.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5865 2024-01-24 11:55:16.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s200_fsfw_mode.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4605 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s20_fsfw_param.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5339 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s23_filemgmt.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1982 2023-11-29 17:07:41.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s2_rawcmd.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7832 2023-11-29 17:07:41.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s3_fsfw_hk.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1809 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s3_hk_base.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4898 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s5_fsfw_event.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4211 2023-11-29 17:07:41.000000 tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s8_fsfw_action.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.175665 tmtccmd-8.0.0rc1/tmtccmd/tmtc/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      820 2023-11-29 17:07:41.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7928 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/ccsds_seq_sender.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2108 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/ccsds_tm_listener.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3819 2023-11-29 17:07:41.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/common.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1074 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/decorator.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4016 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/handler.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2993 2023-11-22 15:09:09.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/procedure.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9432 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/queue.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4740 2023-11-29 17:07:41.000000 tmtccmd-8.0.0rc1/tmtccmd/tmtc/tm_base.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.175665 tmtccmd-8.0.0rc1/tmtccmd/util/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      118 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/util/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2911 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/util/conf_util.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      227 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/util/countdown.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      500 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/util/exit.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12446 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/util/hammingcode.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2333 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/util/json.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3338 2023-11-29 16:35:49.000000 tmtccmd-8.0.0rc1/tmtccmd/util/obj_id.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      448 2023-10-01 22:30:50.000000 tmtccmd-8.0.0rc1/tmtccmd/util/retval.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      310 2024-01-24 15:27:49.000000 tmtccmd-8.0.0rc1/tmtccmd/util/seqcnt.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      209 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/util/tmtc_printer.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      243 2023-11-17 17:24:21.000000 tmtccmd-8.0.0rc1/tmtccmd/version.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.175665 tmtccmd-8.0.0rc1/tmtccmd.egg-info/
--rw-r--r--   0 rmueller  (1000) rmueller  (1000)     6575 2024-01-24 15:32:53.000000 tmtccmd-8.0.0rc1/tmtccmd.egg-info/PKG-INFO
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5755 2024-01-24 15:32:53.000000 tmtccmd-8.0.0rc1/tmtccmd.egg-info/SOURCES.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        1 2024-01-24 15:32:53.000000 tmtccmd-8.0.0rc1/tmtccmd.egg-info/dependency_links.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      197 2024-01-24 15:32:53.000000 tmtccmd-8.0.0rc1/tmtccmd.egg-info/requires.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       53 2024-01-24 15:32:53.000000 tmtccmd-8.0.0rc1/tmtccmd.egg-info/top_level.txt
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.147665 tmtccmd-8.0.0rc1/venv/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 15:32:53.175665 tmtccmd-8.0.0rc1/venv/bin/
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      626 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2html.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      746 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2html4.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)     1114 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2html5.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      823 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2latex.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      631 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2man.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      796 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2odt.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)     1758 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2odt_prepstyles.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      633 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2pseudoxml.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      669 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2s5.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      903 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2xetex.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      634 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rst2xml.py
--rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)      702 2023-11-18 11:15:35.000000 tmtccmd-8.0.0rc1/venv/bin/rstpep2html.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.153295 tmtccmd-8.0.0rc2/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    21611 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/CHANGELOG.md
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11359 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/LICENSE-APACHE
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1061 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/LICENSE-MIT
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      227 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/MANIFEST.in
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      177 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/NOTICE
+-rw-r--r--   0 rmueller  (1000) rmueller  (1000)     6581 2024-04-23 12:14:21.153295 tmtccmd-8.0.0rc2/PKG-INFO
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5118 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/README.md
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.117296 tmtccmd-8.0.0rc2/docs/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        5 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/docs/.gitignore
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      634 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/docs/Makefile
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.121296 tmtccmd-8.0.0rc2/docs/api/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      168 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/api/cfdp.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1546 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/docs/api/com.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1435 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/api/config.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      741 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/docs/api/core.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      239 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/docs/api/fsfw.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      212 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/docs/api/logging.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4120 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/docs/api/pus.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      640 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/docs/api/tc.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      497 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/api/tm.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1440 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/api/util.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      127 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/docs/api/version.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1263 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/api.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      356 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/cfdp.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5278 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/docs/communication.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3261 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/conf.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8477 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/gettingstarted.rst
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.125295 tmtccmd-8.0.0rc2/docs/images/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    13571 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/images/example_system.drawio
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   148156 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/images/example_system.png
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   116372 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/docs/images/tmtccmd_usage.PNG
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   268138 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/docs/images/tmtccmd_usage.graphml
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)   198496 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/docs/images/tmtccmd_usage.pdf
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1134 2023-11-02 16:40:37.000000 tmtccmd-8.0.0rc2/docs/index.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3192 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/docs/introduction.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      760 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/docs/make.bat
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       24 2023-10-06 13:10:57.000000 tmtccmd-8.0.0rc2/docs/requirements.txt
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.113296 tmtccmd-8.0.0rc2/examples/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.125295 tmtccmd-8.0.0rc2/examples/app/
+-rwxrwxr-x   0 rmueller  (1000) rmueller  (1000)    14096 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/examples/app/tmtcc.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.125295 tmtccmd-8.0.0rc2/misc/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8164 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/misc/logo-tiny.png
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    55175 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/misc/logo_medium.png
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1670 2024-04-23 12:13:27.000000 tmtccmd-8.0.0rc2/pyproject.toml
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       12 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/requirements.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       38 2024-04-23 12:14:21.153295 tmtccmd-8.0.0rc2/setup.cfg
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.125295 tmtccmd-8.0.0rc2/tests/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        4 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/.gitignore
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.125295 tmtccmd-8.0.0rc2/tests/.pytest_cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-10-09 10:18:13.000000 tmtccmd-8.0.0rc2/tests/.pytest_cache/.gitignore
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-10-09 10:18:13.000000 tmtccmd-8.0.0rc2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-10-09 10:18:13.000000 tmtccmd-8.0.0rc2/tests/.pytest_cache/README.md
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.113296 tmtccmd-8.0.0rc2/tests/.pytest_cache/v/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.125295 tmtccmd-8.0.0rc2/tests/.pytest_cache/v/cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12122 2024-04-23 12:13:32.000000 tmtccmd-8.0.0rc2/tests/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2024-04-23 12:13:32.000000 tmtccmd-8.0.0rc2/tests/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/__init__.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.113296 tmtccmd-8.0.0rc2/tests/cfdp/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.129295 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-10-09 10:16:06.000000 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/.gitignore
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-10-09 10:16:06.000000 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-10-09 10:16:06.000000 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/README.md
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.113296 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/v/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.129295 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/v/cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       40 2023-11-02 11:44:57.000000 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/v/cache/lastfailed
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2497 2023-11-02 11:45:04.000000 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-02 11:45:04.000000 tmtccmd-8.0.0rc2/tests/cfdp/.pytest_cache/v/cache/stepwise
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.129295 tmtccmd-8.0.0rc2/tests/cfdp/log/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      863 2023-10-09 10:18:12.000000 tmtccmd-8.0.0rc2/tests/cfdp/log/tmtccmd_raw_pus_2023-10-09.log
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      590 2023-10-09 10:18:12.000000 tmtccmd-8.0.0rc2/tests/cfdp/log/tmtccmd_raw_pus_2023-10-09.log.1
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      860 2023-10-17 14:07:19.000000 tmtccmd-8.0.0rc2/tests/cfdp/log/tmtccmd_raw_pus_2023-10-17.log
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      590 2023-10-17 14:07:19.000000 tmtccmd-8.0.0rc2/tests/cfdp/log/tmtccmd_raw_pus_2023-10-17.log.1
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.129295 tmtccmd-8.0.0rc2/tests/com/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/com/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      833 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/com/test_dummy.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2448 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/com/test_serial_cobs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2320 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/com/test_serial_dle.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3881 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/com/test_tcp.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1640 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/com/test_udp.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1930 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/com/test_utils.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.129295 tmtccmd-8.0.0rc2/tests/config/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.129295 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-11-16 14:41:30.000000 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/.gitignore
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-11-16 14:41:30.000000 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-11-16 14:41:30.000000 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/README.md
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.113296 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/v/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/v/cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-16 14:54:26.000000 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/v/cache/lastfailed
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      115 2023-11-16 14:56:15.000000 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-11-16 14:56:15.000000 tmtccmd-8.0.0rc2/tests/config/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/config/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8346 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/config/test_args_conversion.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2782 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/config/test_args_parsing.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3644 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tests/config/test_cfdp_conversions.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    16512 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tests/config/test_cmd_def_tree.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4409 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tests/config/test_prompt.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      286 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tests/hook_obj_mock.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tests/pus/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/pus/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    10964 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/pus/test_srv20.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tests/tc/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/tc/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1127 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/tc/test_srv20.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9080 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/test_backend.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1956 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/test_printer.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7462 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/test_pus_verif_log.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5009 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/test_queue.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9234 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/test_seq_sender.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2851 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/test_tm_handler.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2200 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/test_util.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tests/tm/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2023-10-17 09:55:37.000000 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/.gitignore
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2023-10-17 09:55:37.000000 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2023-10-17 09:55:37.000000 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/README.md
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.113296 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/v/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/v/cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      375 2023-10-17 09:55:37.000000 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2023-10-17 09:55:37.000000 tmtccmd-8.0.0rc2/tests/tm/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tests/tm/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1445 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/tm/test_srv1.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1227 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/tm/test_srv17.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1590 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/tm/test_srv20.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      535 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/tm/test_srv200.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1540 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tests/tm/test_srv5.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tmtccmd/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8699 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/__init__.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.133295 tmtccmd-8.0.0rc2/tmtccmd/cfdp/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      321 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/cfdp/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1054 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/cfdp/request.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.137295 tmtccmd-8.0.0rc2/tmtccmd/com/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3183 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/com/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5249 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/com/dummy.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    19386 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/com/qemu.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7949 2023-10-06 13:10:57.000000 tmtccmd-8.0.0rc2/tmtccmd/com/ser_utils.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2469 2023-10-06 13:10:57.000000 tmtccmd-8.0.0rc2/tmtccmd/com/serial_base.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3731 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/com/serial_cobs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4202 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/com/serial_dle.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8094 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/com/tcp.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6977 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/com/tcpip_utils.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2945 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/com/udp.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2551 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/com/utils.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      187 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/com_if.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.137295 tmtccmd-8.0.0rc2/tmtccmd/config/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3916 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/config/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    28683 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/config/args.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3181 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/config/cfdp.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9282 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/config/com.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2868 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/config/defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6001 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/config/globals.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3335 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/config/hook.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      550 2023-11-28 14:57:36.000000 tmtccmd-8.0.0rc2/tmtccmd/config/objects.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12235 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/config/prompt.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    17106 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/config/tmtc.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.137295 tmtccmd-8.0.0rc2/tmtccmd/core/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      140 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/core/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      409 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/core/backend_base.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      938 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/core/backend_state.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1484 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/core/base.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9444 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/core/ccsds_backend.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1830 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/core/globals_manager.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.137295 tmtccmd-8.0.0rc2/tmtccmd/fsfw/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3097 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/fsfw/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7302 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/fsfw/tmtc_printer.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.141295 tmtccmd-8.0.0rc2/tmtccmd/gui/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       35 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/gui/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6971 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/gui/buttons.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4802 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/gui/cmd_select.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2153 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/gui/defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12836 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/gui/frontend.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6835 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/gui/worker.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.141295 tmtccmd-8.0.0rc2/tmtccmd/logging/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4655 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/logging/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7494 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/logging/pus.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.145295 tmtccmd-8.0.0rc2/tmtccmd/pus/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6984 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      100 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s11_tc_sched.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1854 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s11_tc_sched_defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       92 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s17_test.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       75 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s17_test_defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      130 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s1_verification.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      161 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s200_fsfw_mode.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      259 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s200_fsfw_mode_defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      108 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s201_fsfw_health.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      148 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s201_fsfw_health_defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      155 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s20_fsfw_param.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    15855 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s20_fsfw_param_defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       94 2023-11-16 11:30:22.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s3_fsfw_hk.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      235 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s5_fsfw_event.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      621 2023-10-17 12:07:31.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s5_fsfw_event_defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      195 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s5_satrs_event.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      657 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s5_satrs_event_defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      245 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s8_fsfw_action.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      104 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/s8_fsfw_action_defs.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.145295 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2779 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s11_tc_sched.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      681 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s17_test.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2107 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s200_fsfw_mode.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      311 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s201_fsfw_health.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6428 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s20_fsfw_param.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5751 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s3_fsfw_hk.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1242 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s5_event.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1128 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s8_fsfw_action.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.149295 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      510 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s1_verification.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5866 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s200_fsfw_mode.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4385 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s20_fsfw_param.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5339 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s23_filemgmt.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1983 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s2_rawcmd.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7832 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s3_fsfw_hk.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1809 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s3_hk_base.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4740 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s5_fsfw_event.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4212 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s8_fsfw_action.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.149295 tmtccmd-8.0.0rc2/tmtccmd/tmtc/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      823 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     7929 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/ccsds_seq_sender.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2109 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/ccsds_tm_listener.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3874 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/common.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1080 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/decorator.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4016 2023-11-02 11:40:27.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/handler.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3092 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/procedure.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9713 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/queue.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4740 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/tmtc/tm_base.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.153295 tmtccmd-8.0.0rc2/tmtccmd/util/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      118 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/util/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2911 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/util/conf_util.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      227 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/util/countdown.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      500 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/util/exit.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12447 2024-04-23 11:36:50.000000 tmtccmd-8.0.0rc2/tmtccmd/util/hammingcode.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2333 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/util/json.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3338 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/util/obj_id.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      448 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/util/retval.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      310 2024-04-12 15:20:11.000000 tmtccmd-8.0.0rc2/tmtccmd/util/seqcnt.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      209 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/util/tmtc_printer.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      243 2023-10-04 13:06:23.000000 tmtccmd-8.0.0rc2/tmtccmd/version.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 12:14:21.153295 tmtccmd-8.0.0rc2/tmtccmd.egg-info/
+-rw-r--r--   0 rmueller  (1000) rmueller  (1000)     6581 2024-04-23 12:14:21.000000 tmtccmd-8.0.0rc2/tmtccmd.egg-info/PKG-INFO
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5366 2024-04-23 12:14:21.000000 tmtccmd-8.0.0rc2/tmtccmd.egg-info/SOURCES.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        1 2024-04-23 12:14:21.000000 tmtccmd-8.0.0rc2/tmtccmd.egg-info/dependency_links.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      203 2024-04-23 12:14:21.000000 tmtccmd-8.0.0rc2/tmtccmd.egg-info/requires.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       47 2024-04-23 12:14:21.000000 tmtccmd-8.0.0rc2/tmtccmd.egg-info/top_level.txt
```

### Comparing `tmtccmd-8.0.0rc1/CHANGELOG.md` & `tmtccmd-8.0.0rc2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,40 @@
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/).
 
 Starting from v4.0.0, this project adheres to [Semantic Versioning](http://semver.org/).
 
 # [unreleased]
 
+# [v8.0.0rc2] 2024-04-23
+
+- Bumped `spacepackets` to release range >=0.24, <0.25.
+- Bumped `cfdp-py` to v0.1.1.
+
+## Changed
+
+- Renamed `DefaultProcedureParams` to `TreeCommandingParams`.
+- Renamed `TcParams` to `CommandingParams`.
+- Renamed `DefaultProcedureInfo` to `TreeCommandingProcedure`.
+- Renamed `add_default_procedure_arguments` to `add_tree_commanding_arguments`.
+- Renamed `TcProcedureType.DEFAULT` to `TcProcedureType.TREE_COMMANDING`.
+- Replaced `TelemetryListT` by `List[bytes]`.
+- Renamed `TcpSpacePacketsComIF` to `TcpSpacePacketsClient`.
+- Renamed `UdpComIF` to `UdpClient`.
+
+## Removed
+
+- `CoreServiceList` enumeration.
+- `DEFAULT_APID` and `DEBUG_MODE` globals.
+
+## Fixed
+
+- TCP client implementation re-worked to be thread-safe. Also added more graceful shut-down
+  handling. Consequently, the thread spawned by the TCP client is not daemonic anymore.
+
 # [v8.0.0rc1] 2024-01-24
 
 ## Fixed
 
 - Fixed bug for acknowledged file transfer cancellation in the destination handler.
 
 ## Removed
@@ -250,15 +276,15 @@
 
 `spacepackets` version 0.14.0
 
 ## Fixed
 
 - `config.args`: Assigning of the COM interface in the args to setup converters is now done in
   the `args_to_params_generic` function. Otherwise, this feature does not work for the conversion
-  of CFDP arguments. 
+  of CFDP arguments.
 
 ## Changed
 
 - Remove `setup.cfg` and move to `pyproject.toml`. Create new `.flake8` file accordingly.
 
 ## Added
 
@@ -272,15 +298,15 @@
 
 ### Logging
 
 The usage of the `logging` library now is a lot more pythonic and more
 aligned to the recommended way to use the logger. The `get_console_logger` has become deprecated.
 Users are encouraged to create custom application loggers using `logging.getLogger(__name__)`.
 It is also possible to apply the library log format to an application logger using
-`tmtccmd.logging.add_colorlog_console_logger`. 
+`tmtccmd.logging.add_colorlog_console_logger`.
 
 - Mark `get_console_logger` as deprecated.
 - New `tmtccmd.init_logger` method to set up library logger.
 - The logging default init function does not set up an error file logger anymore.
 - (breaking) Rename `set_up_colorlog_logger` to `add_colorlog_console_logger`.
 
 ## Added
@@ -311,15 +337,15 @@
 ### Argument parsing and Core modules
 
 - (breaking): `tmtccmd.config.hook.TmTcCfgHookBase` renamed to `tmtccmd.config.hook.HookBase`.
 - (breaking): The `PostArgsParsingWrapper` constructor now expects a `SetupParams` parameter and
   caches it.
   All `set_*` methods now do not expect the `SetupParams` to be passed explicitely anymore.
 - (breaking): The `PreArgsParsingWrapper` now expects a `setup_params` parameter to be passed to the
-  `parse` method. The parameter helper will be cached in the created `PostArgsParsingWrapper`. 
+  `parse` method. The parameter helper will be cached in the created `PostArgsParsingWrapper`.
 - `args_to_params_tmtc` now expects an `assign_com_if` method and can assign a COM interface
   when it is passed. It oftentimes makes sense to determine a valid COM interface
   (and prompt applicable parameters from the user) before prompting procedure parameters.
   The new behaviour is the default when using the `PostArgsParsingWrapper`.
 
 ### PUS modules
 
@@ -338,15 +364,15 @@
 - `tmtccmd.tc.pus_20_params.py`: Create new `crate_fsfw_load_param_cmd` and
   deprecate the former `pack_fsfw_load_param_cmd` function.
 
 ### Other
 
 - (breaking): `DefaultPusQueueHelper`: `seq_cnt_provider`, `pus_verificator`
   and `default_pus_apid` (formerly `pus_apid`) do not have default values anymore
-  and need to be specified explicitely. 
+  and need to be specified explicitely.
 - (breaking): Renamed `tmtccmd.config.com.ComIfCfgBase` to `ComCfgBase`
 - (breaking): `tmtccmd.com.ComInterface`: Change `get_id` to `id` property.
 - (breaking): TCP (`tmtccmd.com.TcpSpacePacketsComIF`) and `tmtccmd.com.UdpComIF`:
    Remove `max_recv_size` argument and replace it with 4096 where it was used.
 - (breaking): TCP: Renamed `tmtccmd.com.TcpComIF` to `tmtccmd.com.TcpSpacePacketsComIF` to better
   reflect this interface sends and expects space packets.
 - (breaking) TCP: The TCP communication interface now expects a generic `Sequence[PacketId]`
@@ -468,15 +494,15 @@
   - Separate functions to set the internal mode
   - Moved mode enum outside of class scope
 - Call user send callback for both queue commands and regular telecommands
 
 ## TmTcHandler
 
 - Added a cached `SequentialCommandSenderReceiver`
-- Added `CONTINUOUS` mode which will start the receiver thread in the 
+- Added `CONTINUOUS` mode which will start the receiver thread in the
   `SequentialCommandSenderReceiver` instance and only send one TC
 
 ## Runner module
 
 - Added argument in `__start_tmtc_commander_cli` to defer sending of command
 - Added two functions, `init_and_start_daemons` and `performOperation`, to allow
   separate calls to initiate the TmTcHandler and send TCs
```

### Comparing `tmtccmd-8.0.0rc1/LICENSE-APACHE` & `tmtccmd-8.0.0rc2/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/LICENSE-MIT` & `tmtccmd-8.0.0rc2/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/PKG-INFO` & `tmtccmd-8.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmtccmd
-Version: 8.0.0rc1
+Version: 8.0.0rc2
 Summary: TMTC Commander Core
 Author-email: Robin Mueller <robin.mueller.m@gmail.com>
 License: Apache-2.0 or MIT
 Project-URL: Homepage, https://github.com/robamu-org/tmtccmd
 Keywords: ccsds,ecss,space,communication,packet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,16 +27,16 @@
 Requires-Dist: colorama~=0.4.0
 Requires-Dist: colorlog~=6.6
 Requires-Dist: cobs~=1.2
 Requires-Dist: prompt-toolkit~=3.0
 Requires-Dist: Deprecated~=1.2
 Requires-Dist: pyserial~=3.5
 Requires-Dist: dle-encoder~=0.2.3
-Requires-Dist: spacepackets~=0.23.0
-Requires-Dist: cfdp-py~=0.1.0
+Requires-Dist: spacepackets<0.25,>=0.24.0
+Requires-Dist: cfdp-py~=0.1.1
 Provides-Extra: gui
 Requires-Dist: PyQt6~=6.6; extra == "gui"
 Provides-Extra: test
 Requires-Dist: pyfakefs~=4.5; extra == "test"
 
 <p align="center"> <img src="misc/logo.png" width="40%"> </p>
```

### Comparing `tmtccmd-8.0.0rc1/README.md` & `tmtccmd-8.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/Makefile` & `tmtccmd-8.0.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/api/com.rst` & `tmtccmd-8.0.0rc2/docs/api/com.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/api/config.rst` & `tmtccmd-8.0.0rc2/docs/api/config.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/api/core.rst` & `tmtccmd-8.0.0rc2/docs/api/core.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/api/pus.rst` & `tmtccmd-8.0.0rc2/docs/api/pus.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/api/tc.rst` & `tmtccmd-8.0.0rc2/docs/api/tc.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/api/util.rst` & `tmtccmd-8.0.0rc2/docs/api/util.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/api.rst` & `tmtccmd-8.0.0rc2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/communication.rst` & `tmtccmd-8.0.0rc2/docs/communication.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 
 The use of a communication abstraction allows to use the same TMTC specification
 independently of the used communication interface. For example, it might be possible to build
 an on-board software both for a remote MCU and for a hosted system. The MCU might expect the
 same command data to be exchanged via a specific transport layer, while the hosted version
 might just use a UDP socket.
 
-The following example shows how to use the :py:class:`tmtccmd.com.udp.UdpComIF` to send
+The following example shows how to use the :py:class:`tmtccmd.com.udp.UdpClient` to send
 PUS packets (a subtype of CCSDS space packets) to a UDP server
 
 .. testcode:: udp_com
 
     import socket
 
     from tmtccmd.com import ComInterface
-    from tmtccmd.com.udp import UdpComIF, EthAddr
+    from tmtccmd.com.udp import UdpClient, EthAddr
     from spacepackets.ecss.tc import PusTelecommand
 
     def send_my_telecommand(tc: PusTelecommand, com_if: ComInterface):
     	com_if.send(tc.pack())
 
     simulated_udp_server = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     # Let the OS assign an appropriate port.
     addr = ("127.0.0.1", 0)
     simulated_udp_server.bind(addr)
     addr = simulated_udp_server.getsockname()
 
-    udp_client = UdpComIF("udp", send_address=EthAddr.from_tuple(addr))
+    udp_client = UdpClient("udp", send_address=EthAddr.from_tuple(addr))
     udp_client.initialize()
     udp_client.open()
 
     ping_tc = PusTelecommand(service=17, subservice=1, apid=0x020)
     send_my_telecommand(ping_tc, udp_client)
 
     recvd_data, sender_addr = simulated_udp_server.recvfrom(4096)
```

### Comparing `tmtccmd-8.0.0rc1/docs/conf.py` & `tmtccmd-8.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/gettingstarted.rst` & `tmtccmd-8.0.0rc2/docs/gettingstarted.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/images/example_system.drawio` & `tmtccmd-8.0.0rc2/docs/images/example_system.drawio`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/images/example_system.png` & `tmtccmd-8.0.0rc2/docs/images/example_system.png`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/images/tmtccmd_usage.PNG` & `tmtccmd-8.0.0rc2/docs/images/tmtccmd_usage.PNG`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/images/tmtccmd_usage.graphml` & `tmtccmd-8.0.0rc2/docs/images/tmtccmd_usage.graphml`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/images/tmtccmd_usage.pdf` & `tmtccmd-8.0.0rc2/docs/images/tmtccmd_usage.pdf`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/index.rst` & `tmtccmd-8.0.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/introduction.rst` & `tmtccmd-8.0.0rc2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/docs/make.bat` & `tmtccmd-8.0.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/examples/app/tmtcc.py` & `tmtccmd-8.0.0rc2/examples/app/tmtcc.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     QueueWrapper,
     SendCbParams,
     SpecificApidHandlerBase,
     TcHandlerBase,
     TcProcedureType,
     TcQueueEntryType,
 )
-from tmtccmd.util import FileSeqCountProvider, ObjectIdDictT, PusFileSeqCountProvider
+from tmtccmd.util import ObjectIdDictT
+from spacepackets.seqcount import FileSeqCountProvider, PusFileSeqCountProvider
 
 _LOGGER = logging.getLogger()
 
 EXAMPLE_PUS_APID = 0xEF
 EXAMPLE_CFDP_APID = 0xF0
 
 CFDP_LOCAL_ENTITY_ID = UnsignedByteField(byte_len=2, val=1)
@@ -139,25 +140,25 @@
         self.printer = printer
         self.verif_wrapper = verif_wrapper
         assert self.printer.file_logger is not None
 
     def handle_tm(self, packet: bytes, _user_args: Any):
         try:
             tm_packet = PusTelemetry.unpack(
-                packet, time_reader=CdsShortTimestamp.empty()
+                packet, timestamp_len=CdsShortTimestamp.TIMESTAMP_SIZE
             )
         except ValueError as e:
             _LOGGER.warning("Could not generate PUS TM object from raw data")
             _LOGGER.warning(f"Raw Packet: [{packet.hex(sep=',')}], REPR: {packet!r}")
             raise e
         service = tm_packet.service
         dedicated_handler = False
         if service == 1:
             verif_tm = Service1Tm.unpack(
-                data=packet, params=UnpackParams(CdsShortTimestamp.empty(), 1, 2)
+                data=packet, params=UnpackParams(CdsShortTimestamp.TIMESTAMP_SIZE, 1, 2)
             )
             res = self.verif_wrapper.add_tm(verif_tm)
             if res is None:
                 _LOGGER.info(
                     f"Received Verification TM[{tm_packet.service},"
                     f" {tm_packet.subservice}] with Request ID"
                     f" {verif_tm.tc_req_id.as_u32():#08x}"
@@ -166,34 +167,38 @@
                     f"No matching telecommand found for {verif_tm.tc_req_id}"
                 )
             else:
                 self.verif_wrapper.log_to_console(verif_tm, res)
                 self.verif_wrapper.log_to_file(verif_tm, res)
             dedicated_handler = True
         if service == 5:
-            event_tm = Service5Tm.unpack(packet, time_reader=CdsShortTimestamp.empty())
+            event_tm = Service5Tm.unpack(
+                packet, timestamp_len=CdsShortTimestamp.TIMESTAMP_SIZE
+            )
             _LOGGER.info(
                 f"Received event packet TM [{event_tm.service}, {event_tm.subservice}]"
             )
         if service == 17:
-            ping_tm = Service17Tm.unpack(packet, time_reader=CdsShortTimestamp.empty())
+            ping_tm = Service17Tm.unpack(
+                packet, timestamp_len=CdsShortTimestamp.TIMESTAMP_SIZE
+            )
             dedicated_handler = True
             if ping_tm.subservice == 2:
                 _LOGGER.info("Received Ping Reply TM[17,2]")
             else:
                 _LOGGER.info(
                     "Received Test Packet with unknown subservice"
                     f" {tm_packet.subservice}"
                 )
         if tm_packet is None:
             _LOGGER.info(
                 f"The service {service} is not implemented in Telemetry Factory"
             )
             tm_packet = PusTelemetry.unpack(
-                packet, time_reader=CdsShortTimestamp.empty()
+                packet, timestamp_len=CdsShortTimestamp.TIMESTAMP_SIZE
             )
         # TODO: Insert this into a DB instead. Maybe use sqlite for first variant.
         # self.raw_logger.log_tm(tm_packet)
         if not dedicated_handler:
             _LOGGER.info(
                 f"Received PUS TM [{tm_packet.service}, {tm_packet.subservice}] with not dedicated "
                 f"handler"
@@ -230,35 +235,37 @@
                 _LOGGER.info(f"Sending {pus_tc_wrapper.pus_tc}")
                 send_params.com_if.send(raw_tc)
         elif entry_helper.entry_type == TcQueueEntryType.LOG:
             log_entry = entry_helper.to_log_entry()
             _LOGGER.info(log_entry.log_str)
 
     def queue_finished_cb(self, helper: ProcedureWrapper):
-        if helper.proc_type == TcProcedureType.DEFAULT:
-            def_proc = helper.to_def_procedure()
+        if helper.proc_type == TcProcedureType.TREE_COMMANDING:
+            def_proc = helper.to_tree_commanding_procedure()
             _LOGGER.info(f"Queue handling finished for command {def_proc.cmd_path}")
 
     def feed_cb(self, helper: ProcedureWrapper, wrapper: FeedWrapper):
         self.queue_helper.queue_wrapper = wrapper.queue_wrapper
-        if helper.proc_type == TcProcedureType.DEFAULT:
-            def_proc = helper.to_def_procedure()
+        if helper.proc_type == TcProcedureType.TREE_COMMANDING:
+            def_proc = helper.to_tree_commanding_procedure()
             cmd_path = def_proc.cmd_path
             assert cmd_path is not None
             # Path starts with / so the first entry of the list will be an empty string. We cut
             # off that string.
             cmd_path_list = cmd_path.split("/")[1:]
             if cmd_path_list[0] == "ping":
                 return self.queue_helper.add_pus_tc(
-                    PusTelecommand(service=17, subservice=1)
+                    PusTelecommand(apid=EXAMPLE_PUS_APID, service=17, subservice=1)
                 )
             elif cmd_path_list[0] == "test":
                 if cmd_path_list[1] == "event":
                     return self.queue_helper.add_pus_tc(
-                        PusTelecommand(service=17, subservice=128)
+                        PusTelecommand(
+                            apid=EXAMPLE_PUS_APID, service=17, subservice=128
+                        )
                     )
 
 
 # Note about lint disable: I could split up the function but I prefer to have the whole
 # running main in one block for the example.
 def main():  # noqa: C901
     # Apply the library logger formatting to the own root logger. Library logs will be propagated
@@ -274,16 +281,16 @@
     post_args_wrapper = parser_wrapper.parse(hook_obj=hook_obj, setup_params=params)
     proc_wrapper = ProcedureParamsWrapper()
     if post_args_wrapper.use_gui:
         post_args_wrapper.set_params_without_prompts(proc_wrapper)
     else:
         post_args_wrapper.set_params_with_prompts(proc_wrapper)
     params.apid = EXAMPLE_PUS_APID
-    if params.app_params.print_tree:
-        perform_tree_printout(params.app_params, hook_obj.get_command_definitions())
+    if params.tc_params.print_tree:
+        perform_tree_printout(params.tc_params, hook_obj.get_command_definitions())
         sys.exit(0)
     setup_args = SetupWrapper(
         hook_obj=hook_obj, setup_params=params, proc_param_wrapper=proc_wrapper
     )
     # Create console logger helper and file loggers
     tmtc_logger = RegularTmtcLogWrapper()
     printer = FsfwTmTcPrinter(tmtc_logger.logger)
@@ -308,26 +315,28 @@
         init_procedure=init_proc,
     )
     tmtccmd.start(tmtc_backend=tmtc_backend, hook_obj=hook_obj)
     try:
         while True:
             state = tmtc_backend.periodic_op(None)
             if state.request == BackendRequest.TERMINATION_NO_ERROR:
+                tmtc_backend.close_com_if()
                 sys.exit(0)
             elif state.request == BackendRequest.DELAY_IDLE:
                 _LOGGER.info("TMTC Client in IDLE mode")
                 time.sleep(3.0)
             elif state.request == BackendRequest.DELAY_LISTENER:
                 time.sleep(0.8)
             elif state.request == BackendRequest.DELAY_CUSTOM:
                 if state.next_delay.total_seconds() <= 0.4:
                     time.sleep(state.next_delay.total_seconds())
                 else:
                     time.sleep(0.4)
             elif state.request == BackendRequest.CALL_NEXT:
                 pass
     except KeyboardInterrupt:
+        tmtc_backend.close_com_if()
         sys.exit(0)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `tmtccmd-8.0.0rc1/misc/logo-tiny.png` & `tmtccmd-8.0.0rc2/misc/logo-tiny.png`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/misc/logo_medium.png` & `tmtccmd-8.0.0rc2/misc/logo_medium.png`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/pyproject.toml` & `tmtccmd-8.0.0rc2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tmtccmd"
 description = "TMTC Commander Core"
 readme = "README.md"
-version = "8.0.0rc1"
+version = "8.0.0rc.2"
 requires-python = ">=3.8"
 license = {text = "Apache-2.0 or MIT" }
 authors = [
     {name = "Robin Mueller", email = "robin.mueller.m@gmail.com"}
 ]
 keywords = ["ccsds", "ecss", "space", "communication", "packet"]
 classifiers = [
@@ -32,16 +32,16 @@
     "colorama~=0.4.0",
     "colorlog~=6.6",
     "cobs~=1.2",
     "prompt-toolkit~=3.0",
     "Deprecated~=1.2",
     "pyserial~=3.5",
     "dle-encoder~=0.2.3",
-    "spacepackets~=0.23.0",
-    "cfdp-py~=0.1.0"
+    "spacepackets>=0.24.0, <0.25",
+    "cfdp-py~=0.1.1",
     # "spacepackets @ git+https://github.com/us-irs/spacepackets-py@main"
 ]
 
 [project.optional-dependencies]
 gui = [
     "PyQt6~=6.6",
 ]
@@ -52,11 +52,11 @@
 [project.urls]
 "Homepage" = "https://github.com/robamu-org/tmtccmd"
 
 # Auto-Discovery is problematic for some reason, so use custom-discovery
 [tool.setuptools.packages]
 find = {}
 
-[tool.ruff]
+[tool.ruff.lint]
 ignore = ["E501"]
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `tmtccmd-8.0.0rc1/tests/.pytest_cache/v/cache/nodeids` & `tmtccmd-8.0.0rc2/tests/.pytest_cache/v/cache/nodeids`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6652173913043479%*

 * *Differences: {'delete': '[214, 213, 183, 153, 101, 100, 99, 98, 97, 94, 93, 81, 72, 69, 67, 66, 65, 64, 63, 62, '*

 * *           '61, 60, 59, 58, 57, 56, 55, 54, 53, 52, 51, 50, 41, 40, 39, 38, 37, 36, 35, 34, 33, '*

 * *           '32, 31, 30, 29, 28, 27, 26, 25, 24, 23, 22, 21, 20, 19, 18, 17, 16, 15, 14, 13, 12, '*

 * *           '11, 1, 0]',*

 * * 'insert': "[(79, 'config/test_cmd_def_tree.py::TestCmdDefTree::test_extract_node_invalid_input'), "*

 * *           "(80, 'config/test_cmd_def_tree.py::TestCmdDefTree::test_extract_node_not_conta […]*

```diff
@@ -1,110 +1,49 @@
 [
-    "cfdp/test_checksum.py::TestChecksumHelper::test_modular_checksum",
-    "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_check_timer_mechanism",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_empty_file_reception",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_empty_file_reception_with_closure",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_file_data_pdu_before_metadata_is_discarded",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_file_is_overwritten",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_larger_file_reception",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_permission_error",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_remote_cfg_does_not_exist",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_small_file_reception",
     "cfdp/test_dest_handler.py::TestCfdpDestHandler::test_small_file_reception_with_closure",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_acked_empty_transfer",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_acked_small_file_transfer",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_basic",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_deferred_lost_segment_handling_after_timeout",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_deferred_lost_segment_handling_after_timeout_activity_reset",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_deferred_missing_file_segment_handling",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_immediate_missing_file_seg_handling_0",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_immediate_missing_file_seg_handling_1",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_immediate_missing_segment_also_rerequested_after_eof",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_immediate_multi_missing_segment_handling",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_metadata_eof_only_missing_metadata",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_metadata_only_transfer",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_missing_file_segment_is_rerequested",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_missing_metadata_pdu",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_multi_segment_missing_deferred_handling",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_positive_ack_procedure_finished_pdu",
-    "cfdp/test_dest_handler_acked.py::TestDestHandlerAcked::test_stuff",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_check_limit_reached",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_check_timer_mechanism",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_empty_file_reception",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_empty_file_reception_with_closure",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_file_data_pdu_before_metadata_is_discarded",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_file_is_overwritten",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_larger_file_reception",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_larger_file_reception_with_closure",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_metadata_only_transfer",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_permission_error",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_remote_cfg_does_not_exist",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_small_file_reception",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_small_file_reception_no_closure",
-    "cfdp/test_dest_handler_naked.py::TestCfdpDestHandler::test_small_file_reception_with_closure",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_create_dir",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_creation",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_list_dir",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_read_file",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_read_opened_file",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_rename",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_replace_file",
     "cfdp/test_filestore.py::TestCfdpHostFilestore::test_write_file",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_basic",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_coalesence_0",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_coalesence_1",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_coalesence_2",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_invalid_removal_0",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_invalid_removal_1",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_noop_removal_0",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_noop_removal_1",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_noop_removal_2",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_removal_0",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_removal_1",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_removal_2",
-    "cfdp/test_lost_seg_tracker.py::TestLostSegmentTracker::test_removal_3",
-    "cfdp/test_request.py::TestRequest::test_printout_0",
-    "cfdp/test_request.py::TestRequest::test_printout_1",
-    "cfdp/test_request.py::TestRequest::test_printout_2",
-    "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_ack_limit_reached",
-    "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_ack_procedure_success",
     "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_empty_file_transfer",
-    "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_large_missing_chunk_retransmission",
     "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_missing_filedata_pdu_retransmission",
     "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_missing_metadata_pdu_retransmission",
-    "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_positive_ack_procedure",
     "cfdp/test_src_handler_acked.py::TestSourceHandlerAcked::test_small_file_transfer",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerNackedWithClosure::test_cancelled_transaction",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerNackedWithClosure::test_empty_file_pdu_generation",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerNackedWithClosure::test_invalid_dest_id_pdu_passed",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerNackedWithClosure::test_invalid_dir_pdu_passed",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerNackedWithClosure::test_invalid_source_id_pdu_passed",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerNackedWithClosure::test_small_file_pdu_generation",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_cancelled_transaction",
-    "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_empty_file_pdu_generation",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_empty_file_pdu_generation_nacked_by_remote_cfg",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_empty_file_pdu_generation_nacked_explicitely",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_invalid_dest_id_pdu_passed",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_invalid_dir_pdu_passed",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_invalid_source_id_pdu_passed",
     "cfdp/test_src_handler_nak_closure.py::TestCfdpSourceHandlerWithClosure::test_small_file_pdu_generation",
     "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_empty_file",
     "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_empty_file_explicit_nacked",
     "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_empty_file_nacked_by_def_config",
     "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_perfectly_segmented_file_pdu_generation",
     "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_proxy_get_request",
-    "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_proxy_put_response_no_originating_id",
-    "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_put_req_by_proxy_op",
     "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_segmented_file_pdu_generation",
     "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNackedNoClosure::test_small_file_pdu_generation",
-    "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNoClosure::test_empty_file",
-    "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNoClosure::test_perfectly_segmented_file_pdu_generation",
-    "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNoClosure::test_proxy_get_request",
-    "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNoClosure::test_segmented_file_pdu_generation",
-    "cfdp/test_src_handler_nak_no_closure.py::TestCfdpSourceHandlerNoClosure::test_small_file_pdu_generation",
     "com/test_dummy.py::TestDummy::test_dummy_if",
     "com/test_serial_cobs.py::TestSerialCobsInterface::test_recv",
     "com/test_serial_cobs.py::TestSerialCobsInterface::test_send",
     "com/test_serial_cobs.py::TestSerialCobsInterface::test_state",
     "com/test_serial_dle.py::TestSerialDleInterface::test_recv",
     "com/test_serial_dle.py::TestSerialDleInterface::test_send",
     "com/test_serial_dle.py::TestSerialDleInterface::test_state",
@@ -135,28 +74,39 @@
     "config/test_args_parsing.py::TestArgsParsing::test_valid_argument_0",
     "config/test_args_parsing.py::TestArgsParsing::test_valid_argument_1",
     "config/test_cfdp_conversions.py::TestCfdpParamsConversion::test_generic_conversion_function",
     "config/test_cfdp_conversions.py::TestCfdpParamsConversion::test_generic_put_request_generation",
     "config/test_cfdp_conversions.py::TestCfdpParamsConversion::test_get_request_put_request_generation",
     "config/test_cfdp_conversions.py::TestCfdpParamsConversion::test_invalid_conversion_for_proxy_op",
     "config/test_cfdp_conversions.py::TestCfdpParamsConversion::test_put_request_generation",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_extract_node_invalid_input",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_extract_node_not_contained",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_extract_subnode_relativ_path_by_list",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_extract_subnode_relative_path",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_extract_subnode_simple",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_named_dict",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_path_contained",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_path_contained_acs",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_path_contained_acs_ctrl",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_path_contained_invalid_input",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_path_contained_tcs",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_prinout_one_sublevel",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_prinout_two_sublevels",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_3",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_4",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_5",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_empty",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_hidden_children",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_hidden_override",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_suppressed_leaves",
+    "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_suppressed_leaves_print_override",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_printout_two_sublevels_one_cutoff",
     "config/test_cmd_def_tree.py::TestCmdDefTree::test_state",
+    "config/test_prompt.py::TestPromptFunc::test_cmd_history",
     "config/test_prompt.py::TestPromptFunc::test_prompt_cmd_path_full_print",
-    "config/test_prompt.py::TestPromptFunc::test_prompt_cmd_path_retry",
     "config/test_prompt.py::TestPromptFunc::test_prompt_cmd_path_retry_explicit",
     "config/test_prompt.py::TestPromptFunc::test_prompt_cmd_path_retry_prompted",
     "config/test_prompt.py::TestPromptFunc::test_prompt_cmd_path_simple_print",
     "config/test_prompt.py::TestPromptFunc::test_prompt_help_reprint",
     "pus/test_srv20.py::TestSrv20::test_basic_boolean_param",
     "pus/test_srv20.py::TestSrv20::test_double_matrix",
     "pus/test_srv20.py::TestSrv20::test_double_param",
@@ -178,15 +128,14 @@
     "tc/test_srv20.py::TestSrv20Tc::test_unpack",
     "test_backend.py::TestBackend::test_basic_ops",
     "test_backend.py::TestBackend::test_idle",
     "test_backend.py::TestBackend::test_multi_queue_ops",
     "test_backend.py::TestBackend::test_one_queue_multi_entry_ops",
     "test_backend.py::TestBackend::test_procedure_handling",
     "test_cd.py::CountdownTest::test_basic",
-    "test_countdown.py::CountdownTest::test_basic",
     "test_printer.py::TestPrintersLoggers::test_print_functions",
     "test_printer.py::TestPrintersLoggers::test_pus_loggers",
     "test_pus_verif_log.py::TestPusVerifLog::test_console_log_acc_failure",
     "test_pus_verif_log.py::TestPusVerifLog::test_console_log_acc_failure_without_colors",
     "test_pus_verif_log.py::TestPusVerifLog::test_console_log_start_failure",
     "test_pus_verif_log.py::TestPusVerifLog::test_console_log_success",
     "test_pus_verif_log.py::TestPusVerifLog::test_console_log_success_without_colors",
@@ -208,13 +157,11 @@
     "test_util.py::TestObjectId::test_basic",
     "test_util.py::TestObjectId::test_diff_types",
     "tm/test_srv1.py::TestVerif1TmWrapper::test_basic",
     "tm/test_srv17.py::TestTelemetry::test_generic_pus_c",
     "tm/test_srv20.py::TestSrv20Tm::test_dump_wrapper",
     "tm/test_srv20.py::TestSrv20Tm::test_state",
     "tm/test_srv20.py::TestSrv20Tm::test_unpack",
-    "tm/test_srv200.py::TestSrv200Tm::test_deserialization",
-    "tm/test_srv200.py::TestSrv200Tm::test_serialization",
     "tm/test_srv5.py::TestSrv5Tm::test_basic",
     "tm/test_srv5.py::TestSrv5Tm::test_packed",
     "tm/test_srv5.py::TestSrv5Tm::test_unpack"
 ]
```

### Comparing `tmtccmd-8.0.0rc1/tests/com/test_dummy.py` & `tmtccmd-8.0.0rc2/tests/com/test_dummy.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,12 +10,12 @@
         self.assertFalse(dummy_com_if.is_open())
         dummy_com_if.open()
         self.assertTrue(dummy_com_if.is_open())
         self.assertFalse(dummy_com_if.initialized)
         dummy_com_if.initialize()
         self.assertTrue(dummy_com_if.initialized)
         self.assertFalse(dummy_com_if.data_available())
-        dummy_com_if.send(PusTelecommand(service=17, subservice=1).pack())
+        dummy_com_if.send(PusTelecommand(apid=0x02, service=17, subservice=1).pack())
         self.assertTrue(dummy_com_if.data_available())
         replies = dummy_com_if.receive()
         # Full verification set (acceptance, start and completion) and ping reply
         self.assertEqual(len(replies), 4)
```

### Comparing `tmtccmd-8.0.0rc1/tests/com/test_serial_cobs.py` & `tmtccmd-8.0.0rc2/tests/com/test_serial_cobs.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/com/test_serial_dle.py` & `tmtccmd-8.0.0rc2/tests/com/test_serial_dle.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/com/test_tcp.py` & `tmtccmd-8.0.0rc2/tests/com/test_tcp.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 from collections import deque
 from typing import Optional
 from unittest import TestCase
 
 from spacepackets import PacketType
 from spacepackets.ccsds import PacketId
 from spacepackets.ecss import PusTelecommand, PusTelemetry
-from tmtccmd.com.tcp import TcpSpacePacketsComIF
+from tmtccmd.com.tcp import TcpSpacePacketsClient
 from tmtccmd.com.tcpip_utils import EthAddr
 
 
 LOCALHOST = "127.0.0.1"
-START_ADDR = 7777
 
 
 class TestTcpIf(TestCase):
     def setUp(self) -> None:
         self.tcp_server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.tcp_server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-        self.addr = (LOCALHOST, 7777)
+        # Let the OS assign a port.
+        self.addr = (LOCALHOST, 0)
         self.tcp_server.bind(self.addr)
+        # Update the address for the client.
+        self.addr = self.addr[0], self.tcp_server.getsockname()[1]
         self.tcp_server.listen()
         self.expected_packet_id = PacketId(
             apid=0x22, sec_header_flag=True, ptype=PacketType.TM
         )
         self.base_data = bytes([0, 1, 2, 3])
         self.ping_cmd = PusTelecommand(service=17, subservice=1, apid=0x22)
         self.ping_reply = PusTelemetry(
-            service=17, subservice=2, apid=0x22, time_provider=None
+            service=17, subservice=2, apid=0x22, timestamp=bytes()
         )
-        self.tcp_client = TcpSpacePacketsComIF(
+        self.tcp_client = TcpSpacePacketsClient(
             "tcp",
             space_packet_ids=[self.expected_packet_id],
             target_address=EthAddr.from_tuple(self.addr),
-            tm_polling_freqency=0.05,
+            inner_thread_delay=0.05,
         )
         self.conn_socket: Optional[socket.socket] = None
         self.server_received_packets = deque()
         self.tcp_client.initialize()
 
     def test_monolithic(self):
         self._open()
```

### Comparing `tmtccmd-8.0.0rc1/tests/com/test_udp.py` & `tmtccmd-8.0.0rc2/tests/com/test_udp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import time
 import select
 import socket
 from typing import Any
 from unittest import TestCase
 
 from tmtccmd.com.tcpip_utils import EthAddr
-from tmtccmd.com.udp import UdpComIF
+from tmtccmd.com.udp import UdpClient
 
 LOCALHOST = "127.0.0.1"
 
 
 class TestUdpIf(TestCase):
     def setUp(self) -> None:
         self.udp_server = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         self.addr = (LOCALHOST, 7777)
         self.udp_server.bind(self.addr)
-        self.udp_client = UdpComIF("udp", send_address=EthAddr.from_tuple(self.addr))
+        self.udp_client = UdpClient("udp", send_address=EthAddr.from_tuple(self.addr))
         self.udp_client.initialize()
 
     def test_basic(self):
         self.assertEqual(self.udp_client.id, "udp")
         self._open()
 
     def test_send(self):
```

### Comparing `tmtccmd-8.0.0rc1/tests/com/test_utils.py` & `tmtccmd-8.0.0rc2/tests/com/test_utils.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/config/log/tmtccmd_raw_pus_2023-11-16.log` & `tmtccmd-8.0.0rc2/tests/cfdp/log/tmtccmd_raw_pus_2023-10-17.log`

 * *Files 12% similar despite different names*

```diff
@@ -1,3 +1,3 @@
-2023-11-16 23:57:04.101: tm 1 [1, 3] repr: PusTelemetry.from_composite_fields(PusTelemetry(sp_header=SpacePacketHeader(packet_version=0, packet_type=<PacketType.TM: 0>, apid=0, seq_cnt=0, data_len=19, sec_header_flag=True, seq_flags=<SequenceFlags.UNSEGMENTED: 3>), sec_header=PusTmSecondaryHeader(service=<PusService.S1_VERIFICATION: 1>, subservice=<Subservice.TM_START_SUCCESS: 3>, time=CdsShortTimestamp(ccsds_days=24060, ms_of_day=82624101), message_counter=0, dest_id=0, spacecraft_time_ref=0, pus_version=<PusVersion.PUS_C: 2>), tm_data=bytearray(b'\x18\x00\xc0\x00')
-2023-11-16 23:57:04.102: tm 1 [1, 3] raw readable hex: [08,00,c0,00,00,13,20,01,03,00,00,00,00,40,5d,fc,04,ec,be,65,18,00,c0,00,60,1b]
-2023-11-16 23:57:04.102: tm 1 [1, 3] raw repr: bytearray(b'\x08\x00\xc0\x00\x00\x13 \x01\x03\x00\x00\x00\x00@]\xfc\x04\xec\xbee\x18\x00\xc0\x00`\x1b')
+2023-10-17 16:07:19.249: tm 1 [1, 3] repr: PusTelemetry.from_composite_fields(PusTelemetry(sp_header=SpacePacketHeader(packet_version=0, packet_type=<PacketType.TM: 0>, apid=0, seq_cnt=0, data_len=19, sec_header_flag=True, seq_flags=<SequenceFlags.UNSEGMENTED: 3>), sec_header=PusTmSecondaryHeader(service=<PusService.S1_VERIFICATION: 1>, subservice=<Subservice.TM_START_SUCCESS: 3>, time=CdsShortTimestamp(ccsds_days=24030, ms_of_day=50839249), message_counter=0, dest_id=0, spacecraft_time_ref=0, pus_version=<PusVersion.PUS_C: 2>), tm_data=bytearray(b'\x18\x00\xc0\x00')
+2023-10-17 16:07:19.250: tm 1 [1, 3] raw readable hex: [08,00,c0,00,00,13,20,01,03,00,00,00,00,40,5d,de,03,07,be,d1,18,00,c0,00,32,6c]
+2023-10-17 16:07:19.250: tm 1 [1, 3] raw repr: bytearray(b'\x08\x00\xc0\x00\x00\x13 \x01\x03\x00\x00\x00\x00@]\xde\x03\x07\xbe\xd1\x18\x00\xc0\x002l')
```

### Comparing `tmtccmd-8.0.0rc1/tests/config/log/tmtccmd_raw_pus_2023-11-16.log.1` & `tmtccmd-8.0.0rc2/tests/cfdp/log/tmtccmd_raw_pus_2023-10-09.log.1`

 * *Files 12% similar despite different names*

```diff
@@ -1,3 +1,3 @@
-2023-11-16 23:57:04.101: tc 0 [17, 1] repr: PusTelecommand.from_composite_fields(sp_header=SpacePacketHeader(packet_version=0, packet_type=<PacketType.TC: 1>, apid=0, seq_cnt=0, data_len=6, sec_header_flag=True, seq_flags=<SequenceFlags.UNSEGMENTED: 3>), sec_header=PusTcDataFieldHeader(service=<PusService.S17_TEST: 17>, subservice=<Subservice.TC_PING: 1>, ack_flags=15 , app_data=b'')
-2023-11-16 23:57:04.101: tc 0 [17, 1] raw readable hex: [18,00,c0,00,00,06,2f,11,01,00,00,79,58]
-2023-11-16 23:57:04.101: tc 0 [17, 1] raw repr: bytearray(b'\x18\x00\xc0\x00\x00\x06/\x11\x01\x00\x00yX')
+2023-10-09 12:18:12.778: tc 0 [17, 1] repr: PusTelecommand.from_composite_fields(sp_header=SpacePacketHeader(packet_version=0, packet_type=<PacketType.TC: 1>, apid=0, seq_cnt=0, data_len=6, sec_header_flag=True, seq_flags=<SequenceFlags.UNSEGMENTED: 3>), sec_header=PusTcDataFieldHeader(service=<PusService.S17_TEST: 17>, subservice=<Subservice.TC_PING: 1>, ack_flags=15 , app_data=b'')
+2023-10-09 12:18:12.778: tc 0 [17, 1] raw readable hex: [18,00,c0,00,00,06,2f,11,01,00,00,79,58]
+2023-10-09 12:18:12.778: tc 0 [17, 1] raw repr: bytearray(b'\x18\x00\xc0\x00\x00\x06/\x11\x01\x00\x00yX')
```

### Comparing `tmtccmd-8.0.0rc1/tests/config/test_args_conversion.py` & `tmtccmd-8.0.0rc2/tests/config/test_args_conversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 from spacepackets.cfdp import TransmissionMode
 
 from tests.hook_obj_mock import create_hook_mock
 from tmtccmd import CoreModeConverter, CoreModeList
 from tmtccmd.config import CfdpParams
 from tmtccmd.config.args import (
-    AppParams,
-    DefaultProcedureParams,
+    CommandingParams,
+    TreeCommandingParams,
     SetupParams,
     args_to_all_params_tmtc,
     cfdp_args_to_cfdp_params,
     perform_tree_printout,
 )
 from tmtccmd.config.tmtc import CmdTreeNode, TreePart
 
@@ -48,15 +48,15 @@
         # For some reason, those fields need to be reset manually
         self.params.backend_params.mode = ""
         self.params.backend_params.com_if_id = ""
         self.simple_pargs_cli_set()
         self.assertEqual(self.params.tc_params.delay, 0)
         self.assertEqual(self.params.backend_params.mode, "")
         self.assertEqual(self.params.backend_params.com_if_id, "")
-        def_params = DefaultProcedureParams(None)
+        def_params = TreeCommandingParams(None)
         args_to_all_params_tmtc(
             pargs=self.pargs,
             params=self.params,
             hook_obj=self.hook_mock,
             use_prompts=False,
             def_tmtc_params=def_params,
             assign_com_if=False,
@@ -74,15 +74,15 @@
         )
         self.assertEqual(self.params.backend_params.listener, False)
         self.assertEqual(self.params.backend_params.com_if_id, "dummy")
 
     def test_delay_set(self):
         self.simple_pargs_cli_set()
         self.pargs.delay = 2.0
-        def_params = DefaultProcedureParams(None)
+        def_params = TreeCommandingParams(None)
         args_to_all_params_tmtc(
             pargs=self.pargs,
             params=self.params,
             hook_obj=self.hook_mock,
             use_prompts=False,
             def_tmtc_params=def_params,
             assign_com_if=False,
@@ -111,15 +111,15 @@
         self.pargs.type = "ack"
         cfdp_params = CfdpParams()
         cfdp_args_to_cfdp_params(self.pargs, cfdp_params)
         self.assertEqual(cfdp_params.transmission_mode, TransmissionMode.ACKNOWLEDGED)
 
     def test_auto_listener_mode(self):
         self.auto_listener_cli_set()
-        def_params = DefaultProcedureParams(None)
+        def_params = TreeCommandingParams(None)
         args_to_all_params_tmtc(
             pargs=self.pargs,
             params=self.params,
             hook_obj=self.hook_mock,
             use_prompts=False,
             def_tmtc_params=def_params,
             assign_com_if=False,
@@ -134,81 +134,81 @@
             self.params.mode, CoreModeConverter.get_str(CoreModeList.LISTENER_MODE)
         )
         self.params = SetupParams()
 
     def test_tree_printout_conversion_default(self):
         self.base_cli_set()
         self.pargs.print_tree = []
-        def_params = DefaultProcedureParams(None)
+        def_params = TreeCommandingParams(None)
         args_to_all_params_tmtc(
             pargs=self.pargs,
             params=self.params,
             hook_obj=self.hook_mock,
             use_prompts=False,
             def_tmtc_params=def_params,
             assign_com_if=False,
         )
-        self.assertTrue(self.params.app_params.print_tree)
-        self.assertTrue(self.params.app_params.tree_print_with_description)
-        self.assertIsNone(self.params.app_params.tree_print_max_depth)
+        self.assertTrue(self.params.tc_params.print_tree)
+        self.assertTrue(self.params.tc_params.tree_print_with_description)
+        self.assertIsNone(self.params.tc_params.tree_print_max_depth)
 
     def test_tree_printout_conversion_with_custom_args(self):
         self.base_cli_set()
         self.pargs.print_tree = ["b", "2"]
-        def_params = DefaultProcedureParams(None)
+        def_params = TreeCommandingParams(None)
         args_to_all_params_tmtc(
             pargs=self.pargs,
             params=self.params,
             hook_obj=self.hook_mock,
             use_prompts=False,
             def_tmtc_params=def_params,
             assign_com_if=False,
         )
-        self.assertTrue(self.params.app_params.print_tree)
-        self.assertFalse(self.params.app_params.tree_print_with_description)
-        self.assertEqual(self.params.app_params.tree_print_max_depth, 2)
+        self.assertTrue(self.params.tc_params.print_tree)
+        self.assertFalse(self.params.tc_params.tree_print_with_description)
+        self.assertEqual(self.params.tc_params.tree_print_max_depth, 2)
 
     @patch("builtins.print")
     def test_tree_printout_0(self, print_mock: MagicMock):
         root_node_only = CmdTreeNode.root_node()
-        app_params = AppParams()
-        app_params.print_tree = True
-        perform_tree_printout(app_params, root_node_only)
+        tc_params = CommandingParams()
+        tc_params.print_tree = True
+        perform_tree_printout(tc_params, root_node_only)
         self.assertEqual(len(print_mock.call_args_list), 2)
         self.assertEqual(
             print_mock.call_args_list[0],
             call("Printing command tree with full descriptions:"),
         )
         printout = print_mock.call_args_list[1].args[0]
         self.assertTrue("/" in printout)
         self.assertTrue("[ Root Node ]" in printout)
 
     @patch("builtins.print")
     def test_tree_printout_1(self, print_mock: MagicMock):
         root_node_only = CmdTreeNode.root_node()
-        app_params = AppParams()
-        app_params.print_tree = True
-        app_params.tree_print_with_description = False
-        perform_tree_printout(app_params, root_node_only)
+        tc_params = CommandingParams()
+        tc_params.print_tree = True
+        tc_params.tree_print_with_description = False
+        perform_tree_printout(tc_params, root_node_only)
         self.assertEqual(len(print_mock.call_args_list), 2)
         self.assertEqual(
             print_mock.call_args_list[0],
             call("Printing command tree without descriptions:"),
         )
         self.assertEqual(print_mock.call_args_list[1], call(f"/{os.linesep}"))
 
     @patch("builtins.print")
     def test_tree_printout_2(self, print_mock: MagicMock):
         root_node_only = CmdTreeNode.root_node()
         root_node_only.add_child(CmdTreeNode("acs", "ACS Subsystem"))
-        app_params = AppParams()
-        app_params.print_tree = True
-        app_params.tree_print_with_description = False
-        app_params.tree_print_max_depth = 0
-        perform_tree_printout(app_params, root_node_only)
+        tc_params = CommandingParams()
+        tc_params.print_tree = True
+        tc_params.tree_print_with_description = False
+        tc_params.tree_print_max_depth = 0
+        perform_tree_printout(tc_params, root_node_only)
         self.assertEqual(len(print_mock.call_args_list), 2)
         self.assertEqual(
             print_mock.call_args_list[0],
             call("Printing command tree without descriptions and maximum depth 0:"),
         )
         self.assertEqual(
             print_mock.call_args_list[1],
```

### Comparing `tmtccmd-8.0.0rc1/tests/config/test_args_parsing.py` & `tmtccmd-8.0.0rc2/tests/config/test_args_parsing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 from unittest import TestCase
 
 from tmtccmd.config.args import (
     add_tmtc_mode_arguments,
     add_generic_arguments,
     add_default_com_if_arguments,
-    add_default_procedure_arguments,
+    add_tree_commanding_arguments,
 )
 
 
 class TestArgsParsing(TestCase):
     def setUp(self) -> None:
         self.arg_parser = argparse.ArgumentParser()
 
@@ -25,22 +25,23 @@
 
     def test_valid_argument_1(self):
         add_tmtc_mode_arguments(self.arg_parser)
         args = self.arg_parser.parse_args(["--mode", "one-q"])
         self.assertEqual(args.mode, "one-q")
 
     def test_def_proc_argument_empty(self):
-        add_default_procedure_arguments(self.arg_parser)
+        add_tree_commanding_arguments(self.arg_parser)
         args = self.arg_parser.parse_args([])
         self.assertIsNone(args.cmd_path)
 
     def test_def_proc_argument_valid(self):
-        add_default_procedure_arguments(self.arg_parser)
+        add_tree_commanding_arguments(self.arg_parser)
         args = self.arg_parser.parse_args(["-p", "/PING"])
         self.assertEqual(args.cmd_path, "/PING")
+        self.assertEqual(args.print_tree, None)
 
     def test_generic_arguments_empty(self):
         add_generic_arguments(self.arg_parser)
         args = self.arg_parser.parse_args([])
         self.assertIsNone(args.delay)
         self.assertFalse(args.gui)
 
@@ -57,19 +58,19 @@
 
     def test_com_if_arguments_valid(self):
         add_default_com_if_arguments(self.arg_parser)
         args = self.arg_parser.parse_args(["-c", "udp"])
         self.assertEqual(args.com_if, "udp")
 
     def test_tree_print_args_0(self):
-        add_default_procedure_arguments(self.arg_parser)
+        add_tree_commanding_arguments(self.arg_parser)
         args = self.arg_parser.parse_args(["-T"])
         self.assertEqual(args.print_tree, [])
         args = self.arg_parser.parse_args(["--print-tree"])
         self.assertEqual(args.print_tree, [])
         args = self.arg_parser.parse_args(["--pt"])
         self.assertEqual(args.print_tree, [])
 
     def test_tree_print_args_1(self):
-        add_default_procedure_arguments(self.arg_parser)
+        add_tree_commanding_arguments(self.arg_parser)
         args = self.arg_parser.parse_args(["-T", "b", "2"])
         self.assertEqual(args.print_tree, ["b", "2"])
```

### Comparing `tmtccmd-8.0.0rc1/tests/config/test_cfdp_conversions.py` & `tmtccmd-8.0.0rc2/tests/config/test_cfdp_conversions.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/config/test_cmd_def_tree.py` & `tmtccmd-8.0.0rc2/tests/config/test_cmd_def_tree.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/config/test_prompt.py` & `tmtccmd-8.0.0rc2/tests/config/test_prompt.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/pus/test_srv20.py` & `tmtccmd-8.0.0rc2/tests/pus/test_srv20.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/tc/test_srv20.py` & `tmtccmd-8.0.0rc2/tests/tc/test_srv20.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class TestSrv20Tc(TestCase):
     def setUp(self):
         self.obj_id = bytes([0x01, 0x02, 0x03, 0x04])
         self.boolean_param = create_scalar_boolean_parameter(
             object_id=self.obj_id, domain_id=1, unique_id=5, parameter=True
         )
-        self.tc = create_load_param_cmd(self.boolean_param)
+        self.tc = create_load_param_cmd(0x05, self.boolean_param)
 
     def test_basic(self):
         # 12 bytes of generic parameter header + 1 byte parameter itself
         self.assertEqual(len(self.tc.app_data), 13)
         self.assertEqual(self.tc.service, PusService.S20_PARAMETER)
         self.assertEqual(self.tc.subservice, CustomSubservice.TC_LOAD)
```

### Comparing `tmtccmd-8.0.0rc1/tests/test_backend.py` & `tmtccmd-8.0.0rc2/tests/test_backend.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from spacepackets.ecss import PusTelecommand
 from tmtccmd import CcsdsTmtcBackend, CcsdsTmListener, TcHandlerBase
 from tmtccmd.com.dummy import DummyComIF
 from tmtccmd.core import TcMode, TmMode, BackendRequest
 from tmtccmd.core.ccsds_backend import NoValidProcedureSet
 from tmtccmd.tmtc import (
     TcProcedureBase,
-    DefaultProcedureInfo,
     TcProcedureType,
     ProcedureWrapper,
 )
 from tmtccmd.tmtc.handler import FeedWrapper, SendCbParams
+from tmtccmd.tmtc.procedure import TreeCommandingProcedure
 from tmtccmd.tmtc.queue import DefaultPusQueueHelper, QueueWrapper
 
 
 class TcHandlerMock(TcHandlerBase):
-    def __init__(self):
+    def __init__(self, apid: int):
         super().__init__()
+        self.apid = apid
         self.is_feed_cb_valid = False
         self.feed_cb_call_count = 0
         self.feed_cb_def_proc_count = 0
         self.send_cb_call_count = 0
         self.queue_helper = DefaultPusQueueHelper(
             queue_wrapper=QueueWrapper.empty(),
             tc_sched_timestamp_len=4,
@@ -44,38 +45,39 @@
 
     def feed_cb(self, info: ProcedureWrapper, wrapper: FeedWrapper):
         self.queue_helper.queue_wrapper = wrapper.queue_wrapper
         self.feed_cb_call_count += 1
         self.send_cb_cmd_path_arg = None
         self.send_cb_op_code_arg = None
         if info is not None:
-            if info.proc_type == TcProcedureType.DEFAULT:
+            if info.proc_type == TcProcedureType.TREE_COMMANDING:
                 self.feed_cb_def_proc_count += 1
-                def_info = info.to_def_procedure()
+                def_info = info.to_tree_commanding_procedure()
                 if def_info.cmd_path != "/ping":
                     self.is_feed_cb_valid = False
                 self.send_cb_cmd_path_arg = def_info.cmd_path
                 if def_info.cmd_path == "/ping":
                     self.queue_helper.add_pus_tc(
-                        PusTelecommand(service=17, subservice=1)
+                        PusTelecommand(apid=self.apid, service=17, subservice=1)
                     )
                 elif def_info.cmd_path == "/event":
                     self.queue_helper.add_pus_tc(
-                        PusTelecommand(service=17, subservice=1)
+                        PusTelecommand(apid=self.apid, service=17, subservice=1)
                     )
                     self.queue_helper.add_pus_tc(
-                        PusTelecommand(service=5, subservice=1)
+                        PusTelecommand(apid=self.apid, service=5, subservice=1)
                     )
 
 
 class TestBackend(TestCase):
     def setUp(self) -> None:
         self.com_if = DummyComIF()
         self.tm_listener = MagicMock(specs=CcsdsTmListener)
-        self.tc_handler = TcHandlerMock()
+        self.apid = 0x06
+        self.tc_handler = TcHandlerMock(self.apid)
         self.backend = CcsdsTmtcBackend(
             tc_mode=TcMode.IDLE,
             tm_mode=TmMode.IDLE,
             com_if=self.com_if,
             tm_listener=self.tm_listener,
             tc_handler=self.tc_handler,
         )
@@ -112,36 +114,38 @@
         self.backend.poll_tm()
         self.assertEqual(self.tm_listener.operation.call_count, 2)
         self.assertEqual(res.request, BackendRequest.DELAY_LISTENER)
         self.backend.tm_mode = TmMode.IDLE
         self.backend.tc_mode = TcMode.ONE_QUEUE
         with self.assertRaises(NoValidProcedureSet):
             self.backend.periodic_op()
-        self.backend.current_procedure = DefaultProcedureInfo(cmd_path="/ping")
+        self.backend.current_procedure = TreeCommandingProcedure(cmd_path="/ping")
 
         res = self.backend.periodic_op()
         # Only one queue entry which is handled immediately
         self.assertEqual(res.request, BackendRequest.TERMINATION_NO_ERROR)
         self.assertEqual(self.tc_handler.feed_cb_def_proc_count, 1)
         self.assertEqual(self.tc_handler.feed_cb_call_count, 1)
         self.assertEqual(self.tc_handler.send_cb_call_count, 1)
         assert self.tc_handler.send_cb_call_args is not None
         self.assertIsNotNone(self.tc_handler.send_cb_call_args.info)
         self.assertIsNotNone(self.tc_handler.send_cb_call_args.entry)
         self.assertEqual(self.tc_handler.send_cb_call_args.com_if, self.com_if)
         cast_wrapper = self.tc_handler.send_cb_call_args.entry
         pus_entry = cast_wrapper.to_pus_tc_entry()
-        self.assertEqual(pus_entry.pus_tc, PusTelecommand(service=17, subservice=1))
+        self.assertEqual(
+            pus_entry.pus_tc, PusTelecommand(apid=self.apid, service=17, subservice=1)
+        )
         self.backend.close_com_if()
         self.assertFalse(self.com_if.is_open())
 
     def test_one_queue_multi_entry_ops(self):
         self.backend.tm_mode = TmMode.IDLE
         self.backend.tc_mode = TcMode.ONE_QUEUE
-        self.backend.current_procedure = DefaultProcedureInfo(cmd_path="/event")
+        self.backend.current_procedure = TreeCommandingProcedure(cmd_path="/event")
         res = self.backend.periodic_op()
         self.assertEqual(res.request, BackendRequest.CALL_NEXT)
         self.assertEqual(self.tc_handler.feed_cb_def_proc_count, 1)
         self.assertEqual(self.tc_handler.feed_cb_call_count, 1)
         self.assertEqual(self.tc_handler.send_cb_call_count, 1)
         self._check_tc_req_recvd(17, 1)
         res = self.backend.periodic_op()
@@ -150,45 +154,46 @@
         self.assertEqual(self.tc_handler.send_cb_call_count, 2)
         self._check_tc_req_recvd(5, 1)
         self.assertEqual(res.request, BackendRequest.TERMINATION_NO_ERROR)
 
     def test_multi_queue_ops(self):
         self.backend.tm_mode = TmMode.IDLE
         self.backend.tc_mode = TcMode.MULTI_QUEUE
-        self.backend.current_procedure = DefaultProcedureInfo(cmd_path="/ping")
+        self.backend.current_procedure = TreeCommandingProcedure(cmd_path="/ping")
         res = self.backend.periodic_op()
         self.assertEqual(res.request, BackendRequest.CALL_NEXT)
         self.assertEqual(self.backend.request, BackendRequest.CALL_NEXT)
         self.assertEqual(self.backend.tc_mode, TcMode.IDLE)
         self.assertEqual(self.tc_handler.feed_cb_def_proc_count, 1)
         self.assertEqual(self.tc_handler.feed_cb_call_count, 1)
         self.assertEqual(self.tc_handler.send_cb_call_count, 1)
         self._check_tc_req_recvd(17, 1)
         res = self.backend.periodic_op()
         self.assertEqual(self.tc_handler.feed_cb_call_count, 1)
         self.assertEqual(res.request, BackendRequest.DELAY_IDLE)
         self.backend.tc_mode = TcMode.MULTI_QUEUE
-        self.backend.current_procedure = DefaultProcedureInfo(cmd_path="/ping")
+        self.backend.current_procedure = TreeCommandingProcedure(cmd_path="/ping")
         res = self.backend.periodic_op()
         self.assertEqual(res.request, BackendRequest.CALL_NEXT)
         self.assertEqual(self.backend.request, BackendRequest.CALL_NEXT)
         self.assertEqual(self.tc_handler.feed_cb_def_proc_count, 2)
         self.assertEqual(self.tc_handler.feed_cb_call_count, 2)
 
     def test_procedure_handling(self):
-        def_proc = DefaultProcedureInfo(cmd_path="/ping")
+        def_proc = TreeCommandingProcedure(cmd_path="/ping")
         self.backend.current_procedure = def_proc
         self.assertEqual(
-            self.backend.current_procedure.proc_type, TcProcedureType.DEFAULT
+            self.backend.current_procedure.proc_type, TcProcedureType.TREE_COMMANDING
         )
         proc_helper = self.backend.current_procedure
-        def_proc = proc_helper.to_def_procedure()
+        def_proc = proc_helper.to_tree_commanding_procedure()
         self.assertIsNotNone(def_proc)
         self.assertEqual(def_proc.cmd_path, "/ping")
 
     def _check_tc_req_recvd(self, service: int, subservice: int):
         self.assertEqual(self.tc_handler.send_cb_call_args.com_if, self.com_if)
         cast_wrapper = self.tc_handler.send_cb_call_args.entry
         pus_entry = cast_wrapper.to_pus_tc_entry()
         self.assertEqual(
-            pus_entry.pus_tc, PusTelecommand(service=service, subservice=subservice)
+            pus_entry.pus_tc,
+            PusTelecommand(apid=self.apid, service=service, subservice=subservice),
         )
```

### Comparing `tmtccmd-8.0.0rc1/tests/test_printer.py` & `tmtccmd-8.0.0rc2/tests/test_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,29 +17,31 @@
     RawTmtcRotatingLogWrapper,
 )
 
 
 # TODO: Use temp files to test loggers?
 class TestPrintersLoggers(TestCase):
     def setUp(self):
+        self.apid = 0x07
         self.log_path = Path(LOG_DIR)
         if not self.log_path.exists():
             self.log_path.mkdir()
         self.regular_file_name = Path(
             RegularTmtcLogWrapper.get_current_tmtc_file_name()
         )
 
     def test_pus_loggers(self):
         regular_tmtc_logger = RegularTmtcLogWrapper(self.regular_file_name)
         raw_tmtc_log = RawTmtcRotatingLogWrapper(max_bytes=1024, backup_count=10)
         pus_tc = create_service_17_ping_command()
         raw_tmtc_log.log_tc(pus_tc)
         pus_tm = Service1Tm(
+            apid=self.apid,
             subservice=Subservice.TM_START_SUCCESS,
-            time_provider=CdsShortTimestamp.from_now(),
+            timestamp=CdsShortTimestamp.now().pack(),
             verif_params=VerificationParams(
                 req_id=RequestId(pus_tc.packet_id, pus_tc.packet_seq_control)
             ),
         )
         raw_tmtc_log.log_tm(pus_tm.pus_tm)
         self.assertTrue(Path(self.regular_file_name).exists())
         regular_tmtc_logger.logger.info("Test")
```

### Comparing `tmtccmd-8.0.0rc1/tests/test_queue.py` & `tmtccmd-8.0.0rc2/tests/test_queue.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,41 +3,42 @@
 from typing import cast
 from unittest import TestCase
 from unittest.mock import MagicMock
 
 from spacepackets.ecss import PusTelecommand
 from spacepackets.seqcount import ProvidesSeqCount
 
-from tmtccmd import DefaultProcedureInfo
 
 # Required for eval calls
 # noinspection PyUnresolvedReferences
 from tmtccmd.tmtc import (  # noqa: F401
     LogQueueEntry,
     QueueEntryHelper,
     RawTcEntry,
     WaitEntry,
 )
+from tmtccmd.tmtc.procedure import TreeCommandingProcedure
 from tmtccmd.tmtc.queue import DefaultPusQueueHelper, QueueWrapper
 
 
 class TestTcQueue(TestCase):
     def setUp(self) -> None:
+        self.apid = 0x11
         self.queue_wrapper = QueueWrapper(
-            info=DefaultProcedureInfo.empty(), queue=deque()
+            info=TreeCommandingProcedure.empty(), queue=deque()
         )
         self.assertEqual(self.queue_wrapper.queue, deque())
         self.queue_helper = DefaultPusQueueHelper(
             self.queue_wrapper,
             tc_sched_timestamp_len=4,
             seq_cnt_provider=None,
             default_pus_apid=None,
             pus_verificator=None,
         )
-        self.pus_cmd = PusTelecommand(service=17, subservice=1)
+        self.pus_cmd = PusTelecommand(apid=self.apid, service=17, subservice=1)
 
     def test_wait_entry(self):
         self.queue_helper.add_wait(timedelta(seconds=2))
         self.assertEqual(len(self.queue_wrapper.queue), 1)
         wait_entry = cast(WaitEntry, self.queue_wrapper.queue.pop())
         self.assertTrue(wait_entry)
         self.assertFalse(wait_entry.is_tc())
@@ -67,52 +68,52 @@
         pus_entry = cast_wrapper.to_pus_tc_entry()
         self.assertEqual(pus_entry.pus_tc, self.pus_cmd)
         self.assertTrue(pus_entry)
         with self.assertRaises(TypeError):
             cast_wrapper.to_wait_entry()
 
     def test_multi_entry(self):
-        pus_cmd = PusTelecommand(service=17, subservice=1)
+        pus_cmd = PusTelecommand(apid=self.apid, service=17, subservice=1)
         self.queue_helper.add_pus_tc(pus_cmd)
         self.assertEqual(len(self.queue_wrapper.queue), 1)
         self.queue_helper.add_log_cmd("Test String")
         self.queue_helper.add_raw_tc(bytes([0, 1, 2]))
         self.queue_helper.add_ccsds_tc(pus_cmd.to_space_packet())
         self.queue_helper.add_packet_delay(timedelta(seconds=3.0))
         self.assertEqual(len(self.queue_wrapper.queue), 5)
         pus_entry = self.queue_wrapper.queue.popleft()
         cast_wrapper = QueueEntryHelper(pus_entry)
         pus_entry = cast_wrapper.to_pus_tc_entry()
         self.assertEqual(pus_entry.pus_tc, pus_cmd)
         self.assertTrue(pus_entry)
         log_entry = self.queue_wrapper.queue.popleft()
         self.assertFalse(log_entry.is_tc())
-        cast_wrapper.base = log_entry
+        cast_wrapper.entry = log_entry
         log_entry = cast_wrapper.to_log_entry()
         self.assertTrue(log_entry)
         with self.assertRaises(TypeError):
             cast_wrapper.to_raw_tc_entry()
         self.assertEqual(log_entry.log_str, "Test String")
         test_obj = eval(f"{log_entry!r}")
         self.assertEqual(test_obj.log_str, log_entry.log_str)
 
         raw_entry = self.queue_wrapper.queue.popleft()
         self.assertTrue(raw_entry.is_tc())
-        cast_wrapper.base = raw_entry
+        cast_wrapper.entry = raw_entry
         raw_entry = cast_wrapper.to_raw_tc_entry()
         self.assertTrue(raw_entry)
         self.assertEqual(raw_entry.tc, bytes([0, 1, 2]))
         test_obj = eval(f"{raw_entry!r}")
         self.assertEqual(raw_entry.tc, test_obj.tc)
 
         space_packet_entry = self.queue_wrapper.queue.popleft()
         self.assertTrue(space_packet_entry.is_tc())
-        cast_wrapper.base = space_packet_entry
+        cast_wrapper.entry = space_packet_entry
         space_packet_entry = cast_wrapper.to_space_packet_entry()
         self.assertTrue(space_packet_entry)
         self.assertTrue(space_packet_entry.space_packet, pus_cmd.to_space_packet())
 
         packet_delay = self.queue_wrapper.queue.pop()
         self.assertFalse(packet_delay.is_tc())
-        cast_wrapper.base = packet_delay
+        cast_wrapper.entry = packet_delay
         packet_delay = cast_wrapper.to_packet_delay_entry()
         self.assertEqual(packet_delay.delay_time.total_seconds(), 3.0)
```

### Comparing `tmtccmd-8.0.0rc1/tests/test_seq_sender.py` & `tmtccmd-8.0.0rc2/tests/test_seq_sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 from datetime import timedelta
 from unittest.mock import MagicMock, ANY
 
 from spacepackets.ecss import PusTelecommand
 from tmtccmd.com import ComInterface
 from tmtccmd.tmtc.ccsds_seq_sender import SequentialCcsdsSender, SenderMode
 from tmtccmd.tmtc.handler import TcHandlerBase, SendCbParams
-from tmtccmd.tmtc.procedure import DefaultProcedureInfo
+from tmtccmd.tmtc.procedure import TreeCommandingProcedure
 from tmtccmd.tmtc.queue import QueueWrapper, DefaultPusQueueHelper
 
 
 class TestSendReceive(TestCase):
     def setUp(self) -> None:
+        self.apid = 0x22
         self.queue_wrapper = QueueWrapper.empty()
         self.queue_helper = DefaultPusQueueHelper(
             self.queue_wrapper,
             tc_sched_timestamp_len=4,
             pus_verificator=None,
             default_pus_apid=None,
             seq_cnt_provider=None,
@@ -41,15 +42,15 @@
         # Is busy now, so does not accept new queue unless forced
         with self.assertRaises(ValueError):
             self.seq_sender.queue_wrapper = self.queue_wrapper
         self.seq_sender.operation(self.com_if)
         self.tc_handler_mock.send_cb.assert_called_with(ANY)
         call_args = self.tc_handler_mock.send_cb.call_args
         send_cb_params = cast(SendCbParams, call_args.args[0])
-        self.assertEqual(send_cb_params.info.procedure, DefaultProcedureInfo.empty())
+        self.assertEqual(send_cb_params.info.procedure, TreeCommandingProcedure.empty())
         raw_tc_entry = send_cb_params.entry.to_raw_tc_entry()
         self.assertEqual(raw_tc_entry.tc, bytes([0, 1, 2]))
         # Queue should be empty now
         # Called twice for each operation call
         self.assertEqual(self.tc_handler_mock.queue_finished_cb.call_count, 2)
         self.assertFalse(self.queue_wrapper.queue)
         self.assertEqual(self.seq_sender.mode, SenderMode.DONE)
@@ -106,15 +107,15 @@
         call_args = self.tc_handler_mock.send_cb.call_args
         send_cb_params = cast(SendCbParams, call_args.args[0])
         self.assertEqual(send_cb_params.entry.to_raw_tc_entry().tc, bytes([1, 2, 3]))
 
     def test_interpacket_delay(self):
         delay_ms = 20
         inter_packet_delay = timedelta(milliseconds=delay_ms)
-        ping_cmd = PusTelecommand(service=17, subservice=1)
+        ping_cmd = PusTelecommand(apid=self.apid, service=17, subservice=1)
         self.queue_helper.add_pus_tc(ping_cmd)
         self.queue_helper.add_packet_delay_ms(delay_ms)
         self.queue_helper.add_ccsds_tc(ping_cmd.to_space_packet())
         self.queue_helper.add_raw_tc(bytes([0, 1, 2]))
         # Send first TC, assert delay of 10 ms, then send last packet
         res = self.seq_sender.operation(self.com_if)
         self.assertEqual(res.longest_rem_delay, timedelta())
```

### Comparing `tmtccmd-8.0.0rc1/tests/test_tm_handler.py` & `tmtccmd-8.0.0rc2/tests/test_tm_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,29 +24,38 @@
         if not self.was_called:
             self.was_called = True
         self.called_times += 1
         self.packet_queue.appendleft(packet)
 
 
 class TestTmHandler(TestCase):
+    def setUp(self) -> None:
+        self.apid = 0x33
+
     def test_basic(self):
         tm_handler = ApidHandler(0x01)
         com_if = MagicMock(specs=ComInterface)
         unknown_handler = MagicMock(specs=GenericApidHandlerBase)
         ccsds_handler = CcsdsTmHandler(unknown_handler)
         ccsds_handler.add_apid_handler(tm_handler)
         tm_listener = CcsdsTmListener(tm_handler=ccsds_handler)
         handled_packets = tm_listener.operation(com_if)
         self.assertEqual(handled_packets, 0)
         self.assertTrue(ccsds_handler.has_apid(0x01))
         tm0_raw = PusTelemetry(
-            service=1, subservice=12, apid=0x01, time_provider=CdsShortTimestamp.empty()
+            service=1,
+            subservice=12,
+            apid=0x01,
+            timestamp=CdsShortTimestamp.empty().pack(),
         ).pack()
         tm1_raw = PusTelemetry(
-            service=5, subservice=1, apid=0x01, time_provider=CdsShortTimestamp.empty()
+            service=5,
+            subservice=1,
+            apid=0x01,
+            timestamp=CdsShortTimestamp.empty().pack(),
         ).pack()
         com_if.receive.return_value = [tm0_raw]
         handled_packets = tm_listener.operation(com_if)
         self.assertEqual(handled_packets, 1)
         self.assertTrue(tm_handler.was_called)
         self.assertEqual(tm_handler.called_times, 1)
         self.assertEqual(tm_handler.packet_queue.pop(), tm0_raw)
@@ -54,13 +63,16 @@
         handled_packets = tm_listener.operation(com_if)
         self.assertEqual(handled_packets, 2)
         self.assertEqual(tm_handler.called_times, 3)
         self.assertEqual(handled_packets, 2)
         self.assertEqual(tm_handler.packet_queue.pop(), tm0_raw)
         self.assertEqual(tm_handler.packet_queue.pop(), tm1_raw)
         unknown_apid = PusTelemetry(
-            service=1, subservice=12, apid=0x02, time_provider=CdsShortTimestamp.empty()
+            service=1,
+            subservice=12,
+            apid=0x02,
+            timestamp=CdsShortTimestamp.empty().pack(),
         ).pack()
         com_if.receive.return_value = [unknown_apid]
         handled_packets = tm_listener.operation(com_if)
         self.assertEqual(handled_packets, 1)
         unknown_handler.handle_tm.assert_called_once()
```

### Comparing `tmtccmd-8.0.0rc1/tests/test_util.py` & `tmtccmd-8.0.0rc2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tests/tm/test_srv1.py` & `tmtccmd-8.0.0rc2/tests/tm/test_srv1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import struct
 from unittest import TestCase
 
-from spacepackets.ecss import RequestId, PusTelecommand, PacketFieldU8
+from spacepackets.ecss import RequestId, PusTc, PacketFieldU8
 from spacepackets.ecss.pus_1_verification import (
     Service1Tm,
     Subservice,
     VerificationParams,
     FailureNotice,
 )
 from tmtccmd.pus.tm.s1_verification import Service1FsfwWrapper
 
 
 class TestVerif1TmWrapper(TestCase):
     def setUp(self) -> None:
-        self.ping_tc = PusTelecommand(service=17, subservice=1)
+        self.apid = 0x01
+        self.ping_tc = PusTc(apid=self.apid, service=17, subservice=1)
         pass
 
     def test_basic(self):
         context_param_1 = bytearray([0x10, 0x20, 0x30, 0x40])
         context_param_1_as_int = struct.unpack("!I", context_param_1)[0]
         context_param_2 = bytearray([0x40, 0x30, 0x20, 0x10])
         context_param_2_as_int = struct.unpack("!I", context_param_2)[0]
         failure_notice = FailureNotice(
             code=PacketFieldU8(1), data=context_param_1 + context_param_2
         )
         service_1_tm = Service1Tm(
+            apid=self.apid,
             subservice=Subservice.TM_START_FAILURE,
-            time_provider=None,
+            timestamp=bytes(),
             verif_params=VerificationParams(
                 step_id=None,
                 req_id=RequestId.from_pus_tc(self.ping_tc),
                 failure_notice=failure_notice,
             ),
         )
         wrapper = Service1FsfwWrapper(service_1_tm)
```

### Comparing `tmtccmd-8.0.0rc1/tests/tm/test_srv20.py` & `tmtccmd-8.0.0rc2/tests/tm/test_srv20.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,28 +13,28 @@
     def setUp(self):
         self.obj_id = bytes([0x01, 0x02, 0x03, 0x04])
         self.boolean_param = create_scalar_boolean_parameter(
             object_id=self.obj_id, domain_id=1, unique_id=5, parameter=True
         )
         self.tm = Service20FsfwTm(
             subservice=CustomSubservice.TM_DUMP_REPLY,
-            time_provider=None,
+            timestamp=bytes(),
             source_data=self.boolean_param.pack(),
         )
 
     def test_state(self):
-        self.assertEqual(self.tm.time_provider, None)
+        self.assertEqual(self.tm.timestamp, bytes())
         self.assertEqual(self.tm.service, PusService.S20_PARAMETER)
         self.assertEqual(self.tm.subservice, CustomSubservice.TM_DUMP_REPLY)
         self.assertEqual(self.tm.source_data, self.boolean_param.pack())
         self.assertEqual(self.tm.object_id, self.obj_id)
 
     def test_unpack(self):
         tm_raw = self.tm.pack()
-        tm_unpacked = Service20FsfwTm.unpack(raw_telemetry=tm_raw, time_reader=None)
+        tm_unpacked = Service20FsfwTm.unpack(raw_telemetry=tm_raw, timestamp_len=0)
         self.assertEqual(self.tm, tm_unpacked)
         param_unpacked = Parameter.unpack(tm_unpacked.source_data)
         self.assertEqual(param_unpacked, self.boolean_param)
 
     def test_dump_wrapper(self):
         self.dump_wrapper = Service20ParamDumpWrapper(param_tm=self.tm)
         param = self.dump_wrapper.get_param()
```

### Comparing `tmtccmd-8.0.0rc1/tests/tm/test_srv200.py` & `tmtccmd-8.0.0rc2/tests/tm/test_srv200.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 class TestSrv200Tm(TestCase):
     def setUp(self):
         self.app_data = bytearray()
         self.app_data.extend(bytes([0x01, 0x02, 0x03, 0x04]))
         self.srv_200_tm = PusTelemetry(
             service=200,
             subservice=Subservice.TM_MODE_REPLY,
-            time_provider=CdsShortTimestamp.empty(),
+            timestamp=CdsShortTimestamp.empty().pack(),
             apid=0x02,
         )
```

### Comparing `tmtccmd-8.0.0rc1/tests/tm/test_srv5.py` & `tmtccmd-8.0.0rc2/tests/tm/test_srv5.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import struct
 from unittest import TestCase
 from tmtccmd.pus.s5_fsfw_event import Service5Tm, Subservice, EventDefinition
 
 
 class TestSrv5Tm(TestCase):
     def setUp(self):
+        self.apid = 0x08
         self.obj_id = bytes([0x00, 0x01, 0x02, 0x03])
         self.event_def = EventDefinition(
             event_id=5, reporter_id=self.obj_id, param1=22, param2=942
         )
         self.srv5_tm = Service5Tm(
+            apid=self.apid,
             subservice=Subservice.TM_INFO_EVENT,
             event=self.event_def,
-            time_provider=None,
+            timestamp=bytes(),
         )
 
     def test_basic(self):
         self.assertEqual(
             self.srv5_tm.sp_header, self.srv5_tm.pus_tm.space_packet_header
         )
         self.assertEqual(self.srv5_tm.service, 5)
@@ -30,10 +32,10 @@
         self.assertEqual(struct.unpack("!H", raw_tm[13:15])[0], 5)
         self.assertEqual(raw_tm[15:19], self.obj_id)
         self.assertEqual(struct.unpack("!I", raw_tm[19:23])[0], 22)
         self.assertEqual(struct.unpack("!I", raw_tm[23:27])[0], 942)
 
     def test_unpack(self):
         raw_tm = self.srv5_tm.pack()
-        unpacked = Service5Tm.unpack(raw_tm, None)
+        unpacked = Service5Tm.unpack(raw_tm, 0)
         self.assertEqual(self.srv5_tm, unpacked)
         self.assertEqual(unpacked.event_definition, self.event_def)
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/__init__.py` & `tmtccmd-8.0.0rc2/tmtccmd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains core methods called by entry point files to setup and start a tmtccmd application.
 It also re-exports commonly used classes and functions.
 """
+
 import logging
 import sys
 import os
 from datetime import timedelta
 from typing import Union, cast, Optional
 
 from tmtccmd.config.args import ProcedureParamsWrapper
@@ -15,21 +16,21 @@
     HookBase,
     backend_mode_conversion,
     SetupWrapper,
     SetupParams,
     PreArgsParsingWrapper,
     CoreModeConverter,
     CoreModeList,
-    DefaultProcedureParams,
+    TreeCommandingParams,
 )
 from tmtccmd.core.ccsds_backend import BackendBase
 from tmtccmd.tmtc import TmTypes, TmHandlerBase, CcsdsTmHandler
 from tmtccmd.core import ModeWrapper
 from tmtccmd.tmtc import (
-    DefaultProcedureInfo,
+    TreeCommandingProcedure,
     TcProcedureBase,
     ProcedureWrapper,
     TcHandlerBase,
 )
 
 
 __TMTCCMD_LOGGER = logging.getLogger(__name__)
@@ -232,11 +233,11 @@
     )
     if init_procedure is not None:
         tmtc_backend.current_procedure = init_procedure.procedure
     return tmtc_backend
 
 
 def setup_backend_def_procedure(
-    backend: CcsdsTmtcBackend, tmtc_params: DefaultProcedureParams
+    backend: CcsdsTmtcBackend, tmtc_params: TreeCommandingProcedure
 ):
     assert tmtc_params.cmd_path is not None
-    backend.current_procedure = DefaultProcedureInfo(tmtc_params.cmd_path)
+    backend.current_procedure = TreeCommandingProcedure(tmtc_params.cmd_path)
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/cfdp/request.py` & `tmtccmd-8.0.0rc2/tmtccmd/cfdp/request.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/__init__.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """Communication module. Provides generic abstraction for communication and commonly used
 concrete implementations."""
 from abc import abstractmethod, ABC
-from typing import Any, Optional
+from typing import Any, List, Optional
 
 from tmtccmd.tmtc.common import TelemetryListT
 
 
 class ReceptionDecodeError(Exception):
     """Generic decode error which can also wrap the exception thrown by other libraries."""
 
@@ -63,15 +63,15 @@
     def send(self, data: bytes):
         """Send raw data.
 
         :raises SendError: Sending failed for some reason.
         """
 
     @abstractmethod
-    def receive(self, parameters: Any = 0) -> TelemetryListT:
+    def receive(self, parameters: Any = 0) -> List[bytes]:
         """Returns a list of received packets. The child class can use a separate thread to poll for
         the packets or use some other mechanism and container like a deque to store packets
         to be returned here.
 
         :param parameters:
         :raises ReceptionDecodeError: If the underlying COM interface uses encoding and
             decoding and the decoding fails, this exception will be returned.
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/dummy.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/dummy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Dummy Virtual Communication Interface. Currently serves to use the TMTC program without needing
 external hardware or an extra socket
 """
-from typing import Optional
+
+from typing import List, Optional
 
 from deprecated.sphinx import deprecated
 from spacepackets.ccsds.time import CdsShortTimestamp
 from spacepackets.ecss.pus_1_verification import (
     RequestId,
     Service1Tm,
     VerificationParams,
@@ -41,64 +42,64 @@
 
     def generate_reply_package(self):
         """Generate a reply package. Currently, this only generates a reply for a ping
         telecommand."""
         assert self.last_tc is not None
         if self.last_tc.service == 17:
             if self.last_tc.subservice == 1:
-                current_time_stamp = CdsShortTimestamp.from_now()
+                current_time_stamp = CdsShortTimestamp.now()
                 tm_packer = Service1Tm(
                     subservice=Pus1Subservice.TM_ACCEPTANCE_SUCCESS,
                     apid=self.last_tc.apid,
                     seq_count=self.current_ssc,
                     verif_params=VerificationParams(
                         req_id=RequestId(
                             self.last_tc.packet_id, self.last_tc.packet_seq_control
                         )
                     ),
-                    time_provider=current_time_stamp,
+                    timestamp=current_time_stamp.pack(),
                 )
 
                 self.current_ssc += 1
                 tm_packet_raw = tm_packer.pack()
                 self.next_telemetry_package.append(tm_packet_raw)
                 tm_packer = Service1Tm(
                     subservice=Pus1Subservice.TM_START_SUCCESS,
                     apid=self.last_tc.apid,
                     seq_count=self.current_ssc,
                     verif_params=VerificationParams(
                         req_id=RequestId(
                             self.last_tc.packet_id, self.last_tc.packet_seq_control
                         )
                     ),
-                    time_provider=current_time_stamp,
+                    timestamp=current_time_stamp.pack(),
                 )
                 tm_packet_raw = tm_packer.pack()
                 self.next_telemetry_package.append(tm_packet_raw)
                 self.current_ssc += 1
 
                 tm_packer = Service17Tm(
                     subservice=Pus17Subservice.TM_REPLY,
                     apid=self.last_tc.apid,
-                    time_provider=current_time_stamp,
+                    timestamp=current_time_stamp.pack(),
                 )
                 tm_packet_raw = tm_packer.pack()
                 self.next_telemetry_package.append(tm_packet_raw)
                 self.current_ssc += 1
 
                 tm_packer = Service1Tm(
                     subservice=Pus1Subservice.TM_COMPLETION_SUCCESS,
                     apid=self.last_tc.apid,
                     seq_count=self.current_ssc,
                     verif_params=VerificationParams(
                         req_id=RequestId(
                             self.last_tc.packet_id, self.last_tc.packet_seq_control
                         )
                     ),
-                    time_provider=current_time_stamp,
+                    timestamp=current_time_stamp.pack(),
                 )
                 tm_packet_raw = tm_packer.pack()
                 self.next_telemetry_package.append(tm_packet_raw)
                 self.current_ssc += 1
 
     def receive_reply_package(self) -> TelemetryListT:
         if self.reply_pending:
@@ -134,13 +135,13 @@
         self._open = False
 
     def data_available(self, timeout: float = 0, parameters: any = 0):
         if self.dummy_handler.reply_pending:
             return True
         return False
 
-    def receive(self, parameters: any = 0) -> TelemetryListT:
+    def receive(self, parameters: any = 0) -> List[bytes]:
         return self.dummy_handler.receive_reply_package()
 
-    def send(self, data: bytearray):
+    def send(self, data: bytes):
         if data is not None:
             self.dummy_handler.insert_telecommand(data)
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/qemu.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/qemu.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/ser_utils.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/ser_utils.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/serial_base.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/serial_base.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/serial_cobs.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/serial_cobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import collections
 import logging
 import threading
-from typing import Optional
+from typing import List, Optional
 
 from tmtccmd.com import ComInterface, ReceptionDecodeError
 from tmtccmd.com.serial_base import SerialComBase, SerialCfg, SerialCommunicationType
-from tmtccmd.tmtc import TelemetryListT
 from cobs import cobs
 
 
 class SerialCobsComIF(SerialComBase, ComInterface):
     """Serial communication interface which uses the
     `COBS protocol <https://pypi.org/project/cobs/>`_ to encode and decode packets.
 
@@ -54,15 +53,15 @@
 
     def send(self, data: bytes):
         encoded = bytearray([0])
         encoded.extend(cobs.encode(data))
         encoded.append(0)
         self.serial.write(encoded)
 
-    def receive(self, parameters: any = 0) -> TelemetryListT:
+    def receive(self, parameters: any = 0) -> List[bytes]:
         packet_list = []
         while self.__reception_buffer:
             data = self.__reception_buffer.pop()
             try:
                 packet_list.append(cobs.decode(data))
             except cobs.DecodeError as e:
                 raise ReceptionDecodeError(f"COBS decoding error: {e}", e)
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/serial_dle.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/serial_dle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import dataclasses
 import logging
 import threading
 from collections import deque
-from typing import Optional
+from typing import List, Optional
 
 import serial
 from dle_encoder import DleEncoder, STX_CHAR, ETX_CHAR, DleErrorCodes
 
 from tmtccmd.com import ComInterface
 from tmtccmd.com.serial_base import SerialComBase, SerialCfg, SerialCommunicationType
-from tmtccmd.tmtc import TelemetryListT
 
 
 @dataclasses.dataclass
 class DleCfg:
     dle_queue_len: Optional[int] = None
     dle_max_frame: Optional[int] = None
     encode_cr: bool = True
@@ -90,15 +89,15 @@
         self.__reception_thread.join(0.4)
         super().close_port()
 
     def send(self, data: bytes):
         encoded_data = self.__encoder.encode(source_packet=data, add_stx_etx=True)
         self.serial.write(encoded_data)
 
-    def receive(self, parameters: any = 0) -> TelemetryListT:
+    def receive(self, parameters: any = 0) -> List[bytes]:
         packet_list = []
         while self.__reception_buffer:
             data = self.__reception_buffer.pop()
             dle_retval, decoded_packet, read_len = self.__encoder.decode(
                 source_packet=data
             )
             if dle_retval == DleErrorCodes.OK:
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/tcp.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/tcp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,72 +1,70 @@
 """TCP communication interface"""
+
 import logging
 import queue
 import socket
 import time
 import enum
 import threading
 import select
 from collections import deque
-from typing import Optional, Sequence
+from typing import List, Optional, Sequence
 
 from spacepackets.ccsds.spacepacket import parse_space_packets, PacketId
 
 from tmtccmd.com import ComInterface, SendError
-from tmtccmd.tmtc import TelemetryListT
 from tmtccmd.com.tcpip_utils import EthAddr
 
 _LOGGER = logging.getLogger(__name__)
 
 TCP_RECV_WIRETAPPING_ENABLED = False
 TCP_SEND_WIRETAPPING_ENABLED = False
 
 
 class TcpCommunicationType(enum.Enum):
     """Parse for space packets in the TCP stream, using the space packet header."""
 
     SPACE_PACKETS = 0
 
 
-class TcpSpacePacketsComIF(ComInterface):
+class TcpSpacePacketsClient(ComInterface):
     """Communication interface for TCP communication. This particular interface expects
     raw space packets to be sent via TCP and uses a list of passed packet IDs to parse for them.
     """
 
     def __init__(
         self,
         com_if_id: str,
         space_packet_ids: Sequence[PacketId],
-        tm_polling_freqency: float,
+        inner_thread_delay: float,
         target_address: EthAddr,
         max_packets_stored: Optional[int] = None,
     ):
         """Initialize a communication interface to send and receive TMTC via TCP.
 
         :param com_if_id:
         :param space_packet_ids: Valid packet IDs for CCSDS space packets. Those will be used
             to parse for space packets inside the TCP stream.
-        :param tm_polling_freqency: Polling frequency in seconds
+        :param inner_thread_delay: Polling frequency of TCP thread in seconds.
         """
         self.com_if_id = com_if_id
         self.com_type = TcpCommunicationType.SPACE_PACKETS
         self.space_packet_ids = space_packet_ids
-        self.tm_polling_frequency = tm_polling_freqency
+        self.__inner_thread_delay = inner_thread_delay
         self.target_address = target_address
         self.max_packets_stored = max_packets_stored
-        self.connected = False
-
-        self.__tcp_socket: Optional[socket.socket] = None
-        self.__last_connection_time = 0
-        self.__tm_thread_kill_signal = threading.Event()
+        self.__conn_lock = threading.Lock()
+        self.__connected = False
+        self.__tcp_socket = None
+        self.__thread_kill_signal = threading.Event()
         # Separate thread to request TM packets periodically if no TCs are being sent
-        self.__tcp_conn_thread: Optional[threading.Thread] = threading.Thread(
-            target=self.__tcp_tm_client, daemon=True
-        )
+        self.__tcp_thread = None
         self.__tm_queue = queue.Queue()
+        self.__tc_queue = queue.Queue()
         self.__analysis_queue = deque()
         self.tm_packet_list = []
 
     @property
     def id(self) -> str:
         return self.com_if_id
 
@@ -76,81 +74,64 @@
         except IOError:
             _LOGGER.warning("Could not close TCP communication interface!")
 
     def initialize(self, args: any = None) -> any:
         pass
 
     def open(self, args: any = None):
-        self.__tm_thread_kill_signal.clear()
+        if self.is_open():
+            return
+        self.__thread_kill_signal.clear()
         try:
-            self.set_up_socket()
+            self.__init_socket()
+            self.__connect_socket()
         except IOError as e:
             _LOGGER.exception("Issues setting up the TCP socket")
             raise e
-        self.set_up_tcp_thread()
-        self.__tcp_conn_thread.start()
+        if self.__tcp_thread is None:
+            self.__tcp_thread = threading.Thread(target=self.__tcp_task)
+            self.__tcp_thread.start()
+            with self.__conn_lock:
+                self.__connected = True
 
     def is_open(self) -> bool:
-        return self.connected
+        with self.__conn_lock:
+            return self.__connected
 
-    def set_up_socket(self):
+    def __init_socket(self):
         if self.__tcp_socket is None:
             self.__tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            try:
-                self.__tcp_socket.settimeout(2.0)
-                self.__tcp_socket.connect(self.target_address.to_tuple)
-                self.connected = True
-            except socket.timeout as e:
-                _LOGGER.warning(
-                    "Could not connect to socket with address"
-                    f" {self.target_address}: {e}"
-                )
-            finally:
-                self.__tcp_socket.settimeout(None)
+            self.__tcp_socket.settimeout(2.0)
 
-    def set_up_tcp_thread(self):
-        if self.__tcp_conn_thread is None:
-            self.__tcp_conn_thread = threading.Thread(
-                target=self.__tcp_tm_client, daemon=True
+    def __connect_socket(self):
+        assert self.__tcp_socket is not None
+        try:
+            self.__tcp_socket.connect(self.target_address.to_tuple)
+        except socket.timeout as e:
+            _LOGGER.warning(
+                "Could not connect to socket with address"
+                f" {self.target_address}: {e}"
             )
+        finally:
+            self.__tcp_socket.settimeout(None)
 
     def close(self, args: any = None) -> None:
-        self.__tm_thread_kill_signal.set()
-        socket_was_closed = False
-        if self.__tcp_conn_thread is not None:
-            if self.__tcp_conn_thread.is_alive():
-                self.__tcp_conn_thread.join(self.tm_polling_frequency)
-            if self.connected:
-                try:
-                    self.__tcp_socket.shutdown(socket.SHUT_RDWR)
-                except OSError:
-                    _LOGGER.warning(
-                        "TCP socket endpoint was already closed or not connected"
-                    )
-                self.__tcp_socket.close()
-                socket_was_closed = True
-        if self.__tcp_socket is not None and not socket_was_closed:
-            self.__tcp_socket.close()
+        if not self.is_open():
+            return
+        self.__thread_kill_signal.set()
+        if self.__tcp_thread is not None:
+            self.__tcp_thread.join(self.__inner_thread_delay)
+            with self.__conn_lock:
+                self.__connected = False
         self.__tcp_socket = None
-        self.__tcp_conn_thread = None
 
     def send(self, data: bytes):
-        try:
-            if not self.connected:
-                self.set_up_socket()
-            self.__tcp_socket.sendto(data, self.target_address.to_tuple)
-        except BrokenPipeError as e:
-            raise SendError(f"{e}", e)
-        except ConnectionRefusedError or OSError as e:
-            self.connected = False
-            self.__tcp_socket.close()
-            self.__tcp_socket = None
-            raise SendError(f"TCP connection attempt failed with exception: {e}", e)
+        self.__tc_queue.put(data)
 
-    def receive(self, poll_timeout: float = 0) -> TelemetryListT:
+    def receive(self, poll_timeout: float = 0) -> List[bytes]:
         self.__tm_queue_to_packet_list()
         tm_packet_list = self.tm_packet_list
         self.tm_packet_list = []
         return tm_packet_list
 
     def __tm_queue_to_packet_list(self):
         while self.__tm_queue.qsize() > 0:
@@ -164,54 +145,80 @@
                     packet_ids=self.space_packet_ids,
                 )
             )
         else:
             while self.__analysis_queue:
                 self.tm_packet_list.append(self.__analysis_queue.popleft())
 
-    def __tcp_tm_client(self):
-        while True and not self.__tm_thread_kill_signal.is_set():
-            if self.connected:
-                try:
-                    self.__receive_tm_packets()
-                except ConnectionRefusedError:
-                    _LOGGER.warning("TCP connection attempt failed..")
-            time.sleep(self.tm_polling_frequency)
+    def __tcp_task(self):
+        while True and not self.__thread_kill_signal.is_set():
+            try:
+                self.__tmtc_event_loop()
+            except ConnectionRefusedError:
+                _LOGGER.warning("TCP connection attempt failed..")
+            time.sleep(self.__inner_thread_delay)
 
-    def __receive_tm_packets(self):
+    def __tmtc_event_loop(self):
+        assert self.__tcp_socket is not None
         try:
             while True:
-                ready = select.select([self.__tcp_socket], [], [], 0)
-                if not ready[0]:
+                outputs = []
+                queue_size = self.__tc_queue.qsize()
+                if queue_size > 0:
+                    outputs.append(self.__tcp_socket)
+                (readable, writable, _) = select.select(
+                    [self.__tcp_socket], outputs, [], self.__inner_thread_delay
+                )
+                if self.__thread_kill_signal.is_set():
+                    self.__tcp_socket.close()
                     break
-                bytes_recvd = self.__tcp_socket.recv(4096)
-                if bytes_recvd == b"":
-                    self.__close_tcp_socket()
-                    _LOGGER.info("TCP server has been closed")
-                    return
-                else:
-                    self.connected = True
-                if (
-                    self.max_packets_stored is not None
-                    and self.__tm_queue.qsize() >= self.max_packets_stored
-                ):
-                    _LOGGER.warning(
-                        "Number of packets in TCP queue too large. "
-                        "Overwriting old packets.."
-                    )
-                    self.__tm_queue.get()
-                    # TODO: If segments are received but the receiver is unable to parse packets
-                    #       properly, it might make sense to have a timeout which then also
-                    #       logs that there might be an issue reading packets
-                self.__tm_queue.put(bytes(bytes_recvd))
+                if queue_size > 0 and writable and writable[0]:
+                    self.__tc_handling(queue_size)
+                if readable and readable[0]:
+                    self.__tm_handling()
+        except KeyboardInterrupt:
+            _LOGGER.info("Keyboard interrupt, shutting down TCP task")
+            self.__force_shutdown()
         except ConnectionResetError:
-            self.__close_tcp_socket()
+            self.__force_shutdown()
             _LOGGER.exception("ConnectionResetError. TCP server might not be up")
 
+    def __tc_handling(self, queue_size: int):
+        try:
+            self.__tcp_socket.sendto(
+                self.__tc_queue.get(), self.target_address.to_tuple
+            )
+            queue_size -= 1
+        except BrokenPipeError as e:
+            raise SendError(f"{e}", e)
+        except ConnectionRefusedError or OSError as e:
+            self.__force_shutdown()
+            raise SendError(f"TCP connection attempt failed with exception: {e}", e)
+
+    def __tm_handling(self):
+        bytes_recvd = self.__tcp_socket.recv(4096)
+        if bytes_recvd == b"":
+            self.__force_shutdown()
+            _LOGGER.info("TCP server has been closed")
+            return
+        if (
+            self.max_packets_stored is not None
+            and self.__tm_queue.qsize() >= self.max_packets_stored
+        ):
+            _LOGGER.warning(
+                "Number of packets in TCP queue too large. " "Overwriting old packets.."
+            )
+            self.__tm_queue.get()
+            # TODO: If segments are received but the receiver is unable to parse packets
+            #       properly, it might make sense to have a timeout which then also
+            #       logs that there might be an issue reading packets
+        self.__tm_queue.put(bytes(bytes_recvd))
+
     def data_available(self, timeout: float = 0, parameters: any = 0) -> int:
         self.__tm_queue_to_packet_list()
         return len(self.tm_packet_list)
 
-    def __close_tcp_socket(self):
-        self.connected = False
+    def __force_shutdown(self):
+        assert self.__tcp_socket is not None
         self.__tcp_socket.close()
-        self.__tcp_socket = None
+        with self.__conn_lock:
+            self.__connected = False
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/tcpip_utils.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/tcpip_utils.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/udp.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/udp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """UDP Communication Interface"""
+
 import logging
 import select
 import socket
-from typing import Optional
+from typing import List, Optional
 
 from tmtccmd.com import ComInterface
-from tmtccmd.tmtc import TelemetryListT
 from tmtccmd.com.tcpip_utils import EthAddr
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class UdpComIF(ComInterface):
+class UdpClient(ComInterface):
     """Communication interface for UDP communication"""
 
     def __init__(
         self,
         com_if_id: str,
         send_address: EthAddr,
         recv_addr: Optional[EthAddr] = None,
@@ -76,15 +76,15 @@
         if self.udp_socket is None:
             return False
         ready = select.select([self.udp_socket], [], [], timeout)
         if ready[0]:
             return True
         return False
 
-    def receive(self, poll_timeout: float = 0) -> TelemetryListT:
+    def receive(self, poll_timeout: float = 0) -> List[bytes]:
         packet_list = []
         if self.udp_socket is None:
             return packet_list
         try:
             while self.data_available(poll_timeout):
                 data, sender_addr = self.udp_socket.recvfrom(4096)
                 packet_list.append(bytearray(data))
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/com/utils.py` & `tmtccmd-8.0.0rc2/tmtccmd/com/utils.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/__init__.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,95 +3,69 @@
 Submodules:
 
 * :py:mod:`tmtccmd.config.hook` - Base hook class which should be implemented by user and is used
   by the framework to retrieve certain configuration from the user.
 * :py:mod:`tmtccmd.config.args` - Various helper methods and classes to create the argument parsers
   and arguments converts to create the data structures expected by this library from passed CLI
   arguments."""
+
 import logging
 from pathlib import Path
 from typing import Optional
 
 from cfdppy.request import PutRequest
 from spacepackets.cfdp import CfdpLv
 from spacepackets.cfdp.tlv import ProxyPutRequest, ProxyPutRequestParams
 from spacepackets.util import UnsignedByteField
 
 from tmtccmd.cfdp.request import PutRequestCfgWrapper
 from tmtccmd.core import TcMode, TmMode
 from tmtccmd.core.base import ModeWrapper
 from tmtccmd.tmtc.procedure import (
-    CfdpProcedureInfo,
-    DefaultProcedureInfo,
+    CfdpProcedure,
+    TreeCommandingProcedure,
     ProcedureWrapper,
     TcProcedureType,
 )
 
 from .args import (
-    DefaultProcedureParams,
+    TreeCommandingParams,
     PreArgsParsingWrapper,
     ProcedureParamsWrapper,
     SetupParams,
     add_default_tmtccmd_args,
     create_default_args_parser,
     parse_default_tmtccmd_input_arguments,
 )
 from .defs import (
     CORE_COM_IF_DICT,
     CfdpParams,
     ComIfDictT,
     CoreComInterfaces,
     CoreModeConverter,
     CoreModeList,
-    CoreServiceList,
     default_json_path,
 )
 from .hook import HookBase
 from .prompt import prompt_op_code, prompt_service
 from .tmtc import CmdTreeNode, OpCodeEntry, OpCodeOptionBase, TmtcDefinitionWrapper
 
-_LOGGER = logging.getLogger(__name__)
-
 
 def backend_mode_conversion(mode: str, mode_wrapper: ModeWrapper):
     if mode == CoreModeConverter.get_str(CoreModeList.LISTENER_MODE):
         mode_wrapper.tm_mode = TmMode.LISTENER
         mode_wrapper.tc_mode = TcMode.IDLE
     elif mode == CoreModeConverter.get_str(CoreModeList.ONE_QUEUE_MODE):
         mode_wrapper.tm_mode = TmMode.LISTENER
         mode_wrapper.tc_mode = TcMode.ONE_QUEUE
     elif mode == CoreModeConverter.get_str(CoreModeList.MULTI_INTERACTIVE_QUEUE_MODE):
         mode_wrapper.tc_mode = TcMode.MULTI_QUEUE
         mode_wrapper.tm_mode = TmMode.LISTENER
 
 
-def get_global_hook_obj() -> Optional[HookBase]:
-    """This function can be used to get the handle to the global hook object.
-    :return:
-    """
-
-    try:
-        from typing import cast
-
-        from tmtccmd.config.definitions import CoreGlobalIds
-        from tmtccmd.core.globals_manager import get_global
-
-        hook_obj_raw = get_global(CoreGlobalIds.TMTC_HOOK)
-        if hook_obj_raw is None:
-            _LOGGER.error("Hook object is invalid!")
-            return None
-        return cast(HookBase, hook_obj_raw)
-    except ImportError:
-        _LOGGER.exception("Issues importing modules to get global hook handle!")
-        return None
-    except AttributeError:
-        _LOGGER.exception("Attribute error when trying to get global hook handle!")
-        return None
-
-
 class SetupWrapper:
     """This class encapsulates various important setup parameters required by tmtccmd components"""
 
     def __init__(
         self,
         hook_obj: HookBase,
         setup_params: SetupParams,
@@ -111,28 +85,30 @@
             self.json_cfg_path = default_json_path()
 
     @property
     def params(self):
         return self._params
 
 
-def tmtc_params_to_procedure(params: DefaultProcedureParams) -> DefaultProcedureInfo:
-    return DefaultProcedureInfo(cmd_path=params.cmd_path)
+def tmtc_params_to_procedure(params: TreeCommandingParams) -> TreeCommandingProcedure:
+    return TreeCommandingProcedure(cmd_path=params.cmd_path)
 
 
-def cfdp_put_req_params_to_procedure(params: CfdpParams) -> CfdpProcedureInfo:
-    proc_info = CfdpProcedureInfo()
+def cfdp_put_req_params_to_procedure(params: CfdpParams) -> CfdpProcedure:
+    proc_info = CfdpProcedure()
     proc_info.request_wrapper.base = PutRequestCfgWrapper(params)
     return proc_info
 
 
 def params_to_procedure_conversion(
     param_wrapper: ProcedureParamsWrapper,
 ) -> ProcedureWrapper:
     proc_wrapper = ProcedureWrapper(None)
-    if param_wrapper.ptype == TcProcedureType.DEFAULT:
-        proc_wrapper.procedure = tmtc_params_to_procedure(param_wrapper.def_params())  # type: ignore
+    if param_wrapper.ptype == TcProcedureType.TREE_COMMANDING:
+        tree_cmd_params = param_wrapper.tree_commanding_params()
+        assert tree_cmd_params is not None
+        proc_wrapper.procedure = tmtc_params_to_procedure(tree_cmd_params)
     elif param_wrapper.ptype == TcProcedureType.CFDP:
         proc_wrapper.procedure = cfdp_put_req_params_to_procedure(
             param_wrapper.cfdp_params()  # type: ignore
         )
     return proc_wrapper
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/args.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/args.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """Argument parser module."""
+
 from __future__ import annotations
 
 import argparse
 import logging
 import os
 import sys
 from dataclasses import dataclass
 from typing import List, Optional, Sequence, Tuple, Union
 
-from deprecated.sphinx import deprecated
 from prompt_toolkit.shortcuts import CompleteStyle
 from spacepackets.cfdp import TransmissionMode
 
 from tmtccmd.com import ComInterface
 from tmtccmd.com.utils import determine_com_if
-from tmtccmd.config.prompt import prompt_cmd_path, prompt_op_code, prompt_service
+from tmtccmd.config.prompt import prompt_cmd_path
 from tmtccmd.config.tmtc import CmdTreeNode
 from tmtccmd.tmtc.procedure import TcProcedureType
 
 from .defs import (
     CfdpParams,
     CoreComInterfaces,
     CoreModeConverter,
     CoreModeList,
-    DefaultProcedureParams,
+    TreeCommandingParams,
 )
 from .hook import HookBase
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def get_default_descript_txt() -> str:
@@ -58,37 +58,40 @@
         self._ptype = TcProcedureType.CUSTOM
         self._params = None
 
     @property
     def ptype(self):
         return self._ptype
 
-    def set_params(self, params: Union[DefaultProcedureParams, CfdpParams]):
-        if isinstance(params, DefaultProcedureParams):
+    def set_params(self, params: Union[TreeCommandingParams, CfdpParams]):
+        if isinstance(params, TreeCommandingParams):
             self._params = params
-            self._ptype = TcProcedureType.DEFAULT
+            self._ptype = TcProcedureType.TREE_COMMANDING
         elif isinstance(params, CfdpParams):
             self._params = params
             self._ptype = TcProcedureType.CFDP
 
-    def def_params(self) -> Optional[DefaultProcedureParams]:
-        if self._ptype == TcProcedureType.DEFAULT:
+    def tree_commanding_params(self) -> Optional[TreeCommandingParams]:
+        if self._ptype == TcProcedureType.TREE_COMMANDING:
             return self._params
         return None
 
     def cfdp_params(self) -> Optional[CfdpParams]:
         if self._ptype == TcProcedureType.CFDP:
             return self._params
         return None
 
 
 @dataclass
-class TcParams:
+class CommandingParams:
     delay: float = 0.0
     apid: int = 0
+    print_tree: bool = False
+    tree_print_with_description: bool = True
+    tree_print_max_depth: Optional[int] = None
 
 
 @dataclass
 class BackendParams:
     mode: str = ""
     com_if_id: str = ""
     listener: bool = False
@@ -96,31 +99,28 @@
 
 
 @dataclass
 class AppParams:
     use_gui: bool = False
     reduced_printout: bool = False
     use_ansi_colors: bool = True
-    print_tree: bool = False
-    tree_print_with_description: bool = True
-    tree_print_max_depth: Optional[int] = None
     compl_style: CompleteStyle = CompleteStyle.READLINE_LIKE
 
 
 class SetupParams:
     def __init__(
         self,
         com_if: Optional[ComInterface] = None,
-        tc_params: Optional[TcParams] = None,
+        tc_params: Optional[CommandingParams] = None,
         backend_params: Optional[BackendParams] = None,
         app_params: Optional[AppParams] = None,
     ):
         self.com_if = com_if
         if tc_params is None:
-            self.tc_params = TcParams()
+            self.tc_params = CommandingParams()
         if backend_params is None:
             self.backend_params = BackendParams()
         if app_params is None:
             self.app_params = AppParams()
 
     @property
     def apid(self):
@@ -155,15 +155,15 @@
         self.backend_params.com_if_id = com_if_id
 
 
 def add_default_tmtccmd_args(parser: argparse.ArgumentParser):
     add_tmtc_mode_arguments(parser)
     add_default_com_if_arguments(parser)
     add_generic_arguments(parser)
-    add_default_procedure_arguments(parser)
+    add_tree_commanding_arguments(parser)
     add_ethernet_arguments(parser)
 
 
 def parse_default_tmtccmd_input_arguments(
     args: Sequence[str],
     parser: argparse.ArgumentParser,
     print_known_args: bool = False,
@@ -195,28 +195,29 @@
             _LOGGER.info(argument)
 
     if len(unknown) > 0:
         print(f"Unknown arguments detected: {unknown}")
     return args, unknown
 
 
-def add_default_procedure_arguments(parser_or_subparser: argparse.ArgumentParser):
+def add_tree_commanding_arguments(parser_or_subparser: argparse.ArgumentParser):
     parser_or_subparser.add_argument(
         "-p",
         "--path",
         dest="cmd_path",
         help="Command tree path, used to uniquely identify command or command stack to be sent.",
         default=None,
     )
     parser_or_subparser.add_argument(
         "-T",
         "--pt",
         "--print-tree",
         dest="print_tree",
         nargs="*",
+        default=None,
         help=(
             f"Optional arguments [b] [p] [<numMaxDepth>]. Print the command definition tree. You "
             f"can{os.linesep}optionally add b to omit descriptions, p to display hidden nodes, "
             f"and a maximum print depth."
         ),
     )
     add_tmtc_mode_arguments(parser_or_subparser)
@@ -366,49 +367,17 @@
 def add_ethernet_arguments(arg_parser: argparse.ArgumentParser):
     arg_parser.add_argument("--h-ip", help="Host (Computer) IP. Default:''", default="")
     arg_parser.add_argument(
         "--t-ip", help="Target IP. Default: Localhost 127.0.0.1", default="127.0.0.1"
     )
 
 
-@deprecated(
-    version="8.0.0",
-    reason="use determine_cmd_path instead",
-)
-def find_service_and_op_code(
-    params: SetupParams,
-    def_params: DefaultProcedureParams,
-    hook_obj: HookBase,
-    pargs: argparse.Namespace,
-    use_prompts: bool,
-):
-    tmtc_defs = hook_obj.get_tmtc_definitions()
-    if pargs.service is None:
-        if use_prompts:
-            print("No service argument (-s) specified, prompting from user")
-            # Try to get the service list from the hook base and prompt service
-            # from user
-            def_params.service = prompt_service(
-                tmtc_defs, params.app_params.compl_style
-            )
-    else:
-        def_params.service = pargs.service
-    if pargs.op_code is None:
-        current_service = def_params.service
-        if use_prompts:
-            def_params.op_code = prompt_op_code(
-                tmtc_defs, current_service, params.app_params.compl_style
-            )
-    else:
-        def_params.op_code = pargs.op_code
-
-
 def determine_cmd_path(
     params: SetupParams,
-    def_params: DefaultProcedureParams,
+    def_params: TreeCommandingParams,
     hook_obj: HookBase,
     pargs: argparse.Namespace,
     use_prompts: bool,
 ):
     cmd_defs = hook_obj.get_command_definitions()
     if pargs.cmd_path is None:
         if use_prompts:
@@ -430,23 +399,14 @@
     use_prompts: bool,
     assign_com_if: bool,
 ):
     if pargs.gui is None:
         params.app_params.use_gui = False
     else:
         params.app_params.use_gui = pargs.gui
-    if pargs.print_tree is not None:
-        params.app_params.print_tree = True
-        for arg in pargs.print_tree:
-            if "b" in arg:
-                params.app_params.tree_print_with_description = False
-            if arg.isdigit():
-                params.app_params.tree_print_max_depth = int(arg)
-    else:
-        params.app_params.print_tree = False
     if pargs.com_if is None or pargs.com_if == CoreComInterfaces.UNSPECIFIED.value:
         assert hook_obj.cfg_path is not None
         params.com_if_id = determine_com_if(
             hook_obj.get_com_if_dict(), hook_obj.cfg_path, use_prompts
         )
     else:
         params.com_if_id = pargs.com_if
@@ -502,15 +462,15 @@
     else:
         params.tc_params.delay = float(pargs.delay)
 
 
 def args_to_all_params_tmtc(
     pargs: argparse.Namespace,
     params: SetupParams,
-    def_tmtc_params: DefaultProcedureParams,
+    def_tmtc_params: TreeCommandingParams,
     hook_obj: HookBase,
     use_prompts: bool,
     assign_com_if: bool = True,
 ):
     """This function converts command line arguments to the internalized setup parameters.
 
     It is recommended to use the :py:class:`PostArgsParsingHelper` class to do this instead of
@@ -532,14 +492,22 @@
     args_to_params_generic(
         pargs=pargs,
         params=params,
         hook_obj=hook_obj,
         use_prompts=use_prompts,
         assign_com_if=assign_com_if,
     )
+    params.tc_params.print_tree = False
+    if pargs.print_tree is not None:
+        params.tc_params.print_tree = True
+        for arg in pargs.print_tree:
+            if "b" in arg:
+                params.tc_params.tree_print_with_description = False
+            if arg.isdigit():
+                params.tc_params.tree_print_max_depth = int(arg)
     mode_set_explicitely = False
     if pargs.mode is None:
         params.mode = CoreModeConverter.get_str(CoreModeList.ONE_QUEUE_MODE)
     else:
         mode_set_explicitely = True
         params.mode = pargs.mode
     if (
@@ -556,37 +524,37 @@
             params.tc_params.delay = 4.0
         else:
             params.tc_params.delay = 0.0
     else:
         params.tc_params.delay = float(pargs.delay)
     if (
         params.mode != CoreModeConverter.get_str(CoreModeList.LISTENER_MODE)
-        and not params.app_params.print_tree
+        and not params.tc_params.print_tree
     ):
         determine_cmd_path(
             params=params,
             hook_obj=hook_obj,
             use_prompts=use_prompts,
             pargs=pargs,
             def_params=def_tmtc_params,
         )
 
 
-def perform_tree_printout(app_params: AppParams, cmd_def_tree: CmdTreeNode):
-    if app_params.tree_print_with_description:
+def perform_tree_printout(tc_params: CommandingParams, cmd_def_tree: CmdTreeNode):
+    if tc_params.tree_print_with_description:
         info_str = "with full descriptions"
     else:
         info_str = "without descriptions"
-    if app_params.tree_print_max_depth is not None:
-        info_str += f" and maximum depth {app_params.tree_print_max_depth}"
+    if tc_params.tree_print_max_depth is not None:
+        info_str += f" and maximum depth {tc_params.tree_print_max_depth}"
     print(f"Printing command tree {info_str}:")
     print(
         cmd_def_tree.str_for_tree(
-            app_params.tree_print_with_description,
-            app_params.tree_print_max_depth,
+            tc_params.tree_print_with_description,
+            tc_params.tree_print_max_depth,
         )
     )
 
 
 class PreArgsParsingWrapper:
     """This class can be used to simplify parsing all tmtccmd CLI arguments.
 
@@ -674,15 +642,15 @@
         )
 
     def add_def_proc_args(self):
         """Add the default tmtc procedure parameters to the default parser. This includes
         the service and operation code flags."""
         self._check_arg_parser()
         assert self.args_parser is not None
-        add_default_procedure_arguments(self.args_parser)
+        add_tree_commanding_arguments(self.args_parser)
 
     def add_cfdp_args(self):
         """Add the default CFDP procedure parameters to the default parser."""
         self._check_arg_parser()
         assert self.args_parser is not None
         add_cfdp_procedure_arguments(self.args_parser)
 
@@ -708,15 +676,15 @@
             description=(
                 "Default TMTC Procedure Mode using a Service and Operation "
                 "Code Command Tuple to dispatch commands"
             ),
             formatter_class=argparse.RawTextHelpFormatter,
             parents=[self.parent_parser],
         )
-        add_default_procedure_arguments(tmtc_parser)
+        add_tree_commanding_arguments(tmtc_parser)
         cfdp_descrip = "CCSDS CFDP File Transfer"
         cfdp_parser = subparser.add_parser(
             "cfdp",
             help=cfdp_descrip,
             description=cfdp_descrip,
             formatter_class=argparse.RawTextHelpFormatter,
             parents=[self.parent_parser],
@@ -758,35 +726,35 @@
     def use_gui(self):
         """This only yields valid values if :py:meth:`parse` was called once"""
         return self.args_raw.gui
 
     def request_type_from_args(self) -> TcProcedureType:
         if hasattr(self.args_raw, "proc_type"):
             if self.args_raw.proc_type == "tmtc":
-                return TcProcedureType.DEFAULT
+                return TcProcedureType.TREE_COMMANDING
             elif self.args_raw.proc_type == "cfdp":
                 return TcProcedureType.CFDP
             else:
                 raise ValueError(
                     'Procedure type argument destination unknown, should be "tmtc" or'
                     ' "cfdp"'
                 )
         else:
-            return TcProcedureType.DEFAULT
+            return TcProcedureType.TREE_COMMANDING
 
     def set_params_with_prompts(self, proc_base: ProcedureParamsWrapper):
         self._set_params(proc_base, True)
 
     def set_params_without_prompts(self, proc_wrapper: ProcedureParamsWrapper):
         self._set_params(proc_wrapper, False)
 
     def _set_params(self, proc_base: ProcedureParamsWrapper, with_prompts: bool):
         param_type = self.request_type_from_args()
-        if param_type == TcProcedureType.DEFAULT:
-            def_proc_params = DefaultProcedureParams(None)
+        if param_type == TcProcedureType.TREE_COMMANDING:
+            def_proc_params = TreeCommandingParams(None)
             if with_prompts:
                 self.set_tmtc_params_with_prompts(def_proc_params)
             else:
                 self.set_tmtc_params_without_prompts(def_proc_params)
             proc_base.set_params(def_proc_params)
         elif param_type == TcProcedureType.CFDP:
             cfdp_params = CfdpParams()
@@ -798,28 +766,28 @@
 
     def set_cfdp_params_with_prompts(self, cfdp_params: CfdpParams):
         self._set_cfdp_params(cfdp_params, True)
 
     def set_cfdp_params_without_prompts(self, cfdp_params: CfdpParams):
         self._set_cfdp_params(cfdp_params, False)
 
-    def set_tmtc_params_with_prompts(self, tmtc_params: DefaultProcedureParams):
+    def set_tmtc_params_with_prompts(self, tmtc_params: TreeCommandingParams):
         self._set_tmtc_params(tmtc_params, True)
 
-    def set_tmtc_params_without_prompts(self, tmtc_params: DefaultProcedureParams):
+    def set_tmtc_params_without_prompts(self, tmtc_params: TreeCommandingParams):
         """Set up the parameter object from the parsed arguments. This call auto-determines whether
         prompts should be used depending on whether the GUI flag was passed or not.
 
         :raise Value Error: Parse function call missing
         """
         self._set_tmtc_params(tmtc_params, False)
 
     def _set_tmtc_params(
         self,
-        def_tmtc_params: DefaultProcedureParams,
+        def_tmtc_params: TreeCommandingParams,
         use_prompts: bool,
     ):
         try:
             args_to_all_params_tmtc(
                 pargs=self.args_raw,
                 params=self.params,
                 hook_obj=self.hook_obj,
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/cfdp.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/cfdp.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/com.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/com.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 )
 
 from tmtccmd.com.serial_dle import SerialDleComIF
 from tmtccmd.com.serial_cobs import SerialCobsComIF
 
 from tmtccmd.com.ser_utils import determine_com_port, determine_baud_rate
 from tmtccmd.com.tcpip_utils import TcpIpType, EthAddr
-from tmtccmd.com.udp import UdpComIF
-from tmtccmd.com.tcp import TcpSpacePacketsComIF
+from tmtccmd.com.udp import UdpClient
+from tmtccmd.com.tcp import TcpSpacePacketsClient
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ComCfgBase:
     def __init__(
         self,
@@ -208,25 +208,25 @@
     :py:func:`default_tcpip_cfg_setup` for more details.
 
     :param tcpip_cfg: Configuration parameters
     :return:
     """
     communication_interface = None
     if tcpip_cfg.com_if_key == CoreComInterfaces.UDP.value:
-        communication_interface = UdpComIF(
+        communication_interface = UdpClient(
             com_if_id=tcpip_cfg.com_if_key,
             send_address=tcpip_cfg.send_addr,
             recv_addr=tcpip_cfg.recv_addr,
         )
     elif tcpip_cfg.com_if_key == CoreComInterfaces.TCP.value:
         assert tcpip_cfg.space_packet_ids is not None
-        communication_interface = TcpSpacePacketsComIF(
+        communication_interface = TcpSpacePacketsClient(
             com_if_id=tcpip_cfg.com_if_key,
             space_packet_ids=tcpip_cfg.space_packet_ids,
-            tm_polling_freqency=0.5,
+            inner_thread_delay=0.5,
             target_address=tcpip_cfg.send_addr,
         )
     return communication_interface
 
 
 def create_default_serial_interface(
     com_if_key: str, json_cfg_path: str, serial_cfg: SerialCfg
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/defs.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Com Interface Types
 ComIfValueT = Tuple[str, Any]
 ComIfDictT = Dict[str, ComIfValueT]
 
 
 @dataclass
-class DefaultProcedureParams:
+class TreeCommandingParams:
     cmd_path: Optional[str]
 
 
 @dataclass
 class CfdpParams:
     """Simplified dataclass to model the most important CFDP parameters. This can for example
     be used to internalize CFDP CLI or GUI options."""
@@ -27,16 +27,14 @@
 
 
 def default_json_path() -> str:
     return "tmtc_conf.json"
 
 
 class CoreComInterfaces(str, enum.Enum):
-    value: str
-
     DUMMY = "dummy"
     UDP = "udp"
     TCP = "tcp"
     SERIAL_COBS = "serial_cobs"
     SERIAL_DLE = "serial_dle"
     SERIAL_QEMU = "serial_qemu"
     UNSPECIFIED = "unspec"
@@ -85,26 +83,7 @@
             return "one-q"
         elif mode == CoreModeList.MULTI_INTERACTIVE_QUEUE_MODE:
             return "multi-q"
         elif mode == CoreModeList.IDLE:
             return "idle"
         else:
             return ""
-
-
-class CoreServiceList(str, enum.Enum):
-    value: str
-    SERVICE_2 = "2"
-    SERVICE_3 = "3"
-    SERVICE_5 = "5"
-    SERVICE_8 = "8"
-    SERVICE_9 = "9"
-    SERVICE_11 = "11"
-    SERVICE_17 = "17"
-    SERVICE_17_ALT = "test"
-    SERVICE_20 = "20"
-    SERVICE_23 = "23"
-    SERVICE_200 = "200"
-
-
-DEFAULT_APID = 0xEF
-DEBUG_MODE = False
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/globals.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/globals.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/hook.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/hook.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/objects.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/objects.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/prompt.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/prompt.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/config/tmtc.py` & `tmtccmd-8.0.0rc2/tmtccmd/config/tmtc.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/core/backend_state.py` & `tmtccmd-8.0.0rc2/tmtccmd/core/backend_state.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/core/base.py` & `tmtccmd-8.0.0rc2/tmtccmd/core/base.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/core/ccsds_backend.py` & `tmtccmd-8.0.0rc2/tmtccmd/core/ccsds_backend.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/core/globals_manager.py` & `tmtccmd-8.0.0rc2/tmtccmd/core/globals_manager.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/fsfw/__init__.py` & `tmtccmd-8.0.0rc2/tmtccmd/fsfw/__init__.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/fsfw/tmtc_printer.py` & `tmtccmd-8.0.0rc2/tmtccmd/fsfw/tmtc_printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Contains classes and functions that perform all printing functionalities.
 """
+
 import logging
 import enum
 from typing import List, Optional
 
 from spacepackets.util import get_printable_data_string, PrintFormats
 
 from tmtccmd.pus.s8_fsfw_action import Service8FsfwTm
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/gui/buttons.py` & `tmtccmd-8.0.0rc2/tmtccmd/gui/buttons.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/gui/cmd_select.py` & `tmtccmd-8.0.0rc2/tmtccmd/gui/cmd_select.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/gui/defs.py` & `tmtccmd-8.0.0rc2/tmtccmd/gui/defs.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/gui/frontend.py` & `tmtccmd-8.0.0rc2/tmtccmd/gui/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """PyQt front end components for the tmtccmd framework.
 @author         R. Mueller, P. Scheurenbrand, D. Nguyen
 """
+
 import os
 import sys
 import webbrowser
 from multiprocessing import Process
 from pathlib import Path
 from typing import Any, Tuple
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/gui/worker.py` & `tmtccmd-8.0.0rc2/tmtccmd/gui/worker.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/logging/__init__.py` & `tmtccmd-8.0.0rc2/tmtccmd/logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 @brief      This module is used to set up the global loggers
 """
+
 from tmtccmd.version import get_version
 import logging
 import os
 import sys
 from datetime import datetime
 
 from deprecated.sphinx import deprecated
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/logging/pus.py` & `tmtccmd-8.0.0rc2/tmtccmd/logging/pus.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/__init__.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module contains PUS data structures and helpers common for both PUS telemetry and
 telecommands.
 
 Content:
 
 * :py:class:`tmtccmd.pus.VerificationWrapper` helper class
 """
+
 from enum import IntEnum
 from typing import Optional
 
 from spacepackets.ecss import PusTelecommand
 from spacepackets.ecss.pus_1_verification import RequestId
 import spacepackets.ecss.pus_1_verification as pus_1
 from spacepackets.ecss.pus_verificator import (
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/s11_tc_sched_defs.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/s11_tc_sched_defs.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/s20_fsfw_param_defs.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/s20_fsfw_param_defs.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/s5_fsfw_event_defs.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/s5_fsfw_event_defs.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/s5_satrs_event_defs.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/s5_satrs_event_defs.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s11_tc_sched.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s11_tc_sched.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s17_test.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s17_test.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s200_fsfw_mode.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s200_fsfw_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Core components for mode commanding (custom PUS service)."""
+
 import enum
 import struct
 from typing import Union
 
 from deprecated.sphinx import deprecated
 from spacepackets.ecss import PusTelecommand
 from tmtccmd.pus import CustomFsfwPusService
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s20_fsfw_param.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s20_fsfw_param.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Contains definitions and functions related to PUS Service 20 Telecommands.
 """
+
 from __future__ import annotations
 
 import struct
 from typing import Optional
 
 from deprecated.sphinx import deprecated
 from spacepackets.ecss import PusService
@@ -26,47 +27,42 @@
     create_scalar_u16_parameter,
     create_scalar_u32_parameter,
     create_vector_double_parameter,
     create_vector_float_parameter,
 )
 
 
-def create_load_param_cmd(parameter: Parameter) -> PusTelecommand:
+def create_load_param_cmd(apid: int, parameter: Parameter) -> PusTelecommand:
     return PusTelecommand(
+        apid=apid,
         service=PusService.S20_PARAMETER,
         subservice=CustomSubservice.TC_LOAD,
         app_data=parameter.pack(),
     )
 
 
-def create_dump_param_cmd(param_fsfw_id: FsfwParamId) -> PusTelecommand:
+def create_dump_param_cmd(apid: int, param_fsfw_id: FsfwParamId) -> PusTelecommand:
     return PusTelecommand(
+        apid=apid,
         service=PusService.S20_PARAMETER,
         subservice=CustomSubservice.TC_LOAD,
         app_data=param_fsfw_id.pack(),
     )
 
 
-def create_load_param_cmd_from_raw(parameter_raw: bytes) -> PusTelecommand:
+def create_load_param_cmd_from_raw(apid: int, parameter_raw: bytes) -> PusTelecommand:
     return PusTelecommand(
+        apid=apid,
         service=PusService.S20_PARAMETER,
         subservice=CustomSubservice.TC_LOAD,
         app_data=parameter_raw,
     )
 
 
 @deprecated(
-    version="4.0.0a3",
-    reason="use crate_fsfw_load_param_cmd instead",
-)
-def pack_fsfw_load_param_cmd(app_data: bytes) -> PusTelecommand:
-    return create_load_param_cmd(app_data)
-
-
-@deprecated(
     version="3.1.0",
     reason="use create_scalar_boolean_parameter instead",
 )
 def pack_boolean_parameter_app_data(
     object_id: bytes, domain_id: int, unique_id: int, parameter: bool
 ) -> Optional[bytearray]:
     return pack_scalar_boolean_parameter_app_data(
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s3_fsfw_hk.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s3_fsfw_hk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Contains definitions and functions related to PUS Service 3 Telecommands.
 """
+
 import struct
 from typing import Tuple
 
 from deprecated.sphinx import deprecated
 from spacepackets.ecss.tc import PusTelecommand
 from spacepackets.ecss.pus_3_hk import Subservice
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s5_event.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s5_event.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tc/s8_fsfw_action.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tc/s8_fsfw_action.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s200_fsfw_mode.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s200_fsfw_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Base class for Service 200 mode commanding reply handling.
 """
+
 from __future__ import annotations
 
 import struct
 from typing import Optional
 
 from deprecated.sphinx import deprecated
 from spacepackets.ccsds.time import CcsdsTimeProvider
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s20_fsfw_param.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s20_fsfw_param.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from __future__ import annotations
 
-from typing import Optional
-
 from spacepackets import SpacePacketHeader
 from spacepackets.ccsds.spacepacket import PacketId, PacketSeqCtrl
-from spacepackets.ccsds.time import CdsShortTimestamp, CcsdsTimeProvider
 from spacepackets.ecss import (
     Ptc,
     PusTelemetry,
 )
 from spacepackets.ecss.defs import PusService
 from spacepackets.ecss.tm import AbstractPusTm
 
@@ -58,41 +55,39 @@
 
 
 class Service20FsfwTm(AbstractPusTm):
     def __init__(
         self,
         subservice: int,
         source_data: bytes,
-        time_provider: Optional[CcsdsTimeProvider],
+        timestamp: bytes,
         apid: int = 0,
     ):
         self.pus_tm = PusTelemetry(
             service=PusService.S20_PARAMETER,
             subservice=subservice,
             source_data=source_data,
-            time_provider=time_provider,
+            timestamp=timestamp,
             apid=apid,
         )
 
     @staticmethod
     def __common_checks(tm: PusTelemetry):
         if tm.service != 20:
             raise ValueError("service ID is not 20")
         if len(tm.source_data) < 4:
             raise ValueError(
                 "source data must include object ID (4 bytes) as minimal data"
             )
 
     @classmethod
-    def unpack(
-        cls, raw_telemetry: bytes, time_reader: Optional[CcsdsTimeProvider]
-    ) -> Service20FsfwTm:
+    def unpack(cls, raw_telemetry: bytes, timestamp_len: int) -> Service20FsfwTm:
         instance = cls.empty()
         instance.pus_tm = PusTelemetry.unpack(
-            data=raw_telemetry, time_reader=time_reader
+            data=raw_telemetry, timestamp_len=timestamp_len
         )
         Service20FsfwTm.__common_checks(instance.pus_tm)
         return instance
 
     @classmethod
     def from_tm(cls, tm: PusTelemetry):
         instance = cls.empty()
@@ -100,16 +95,16 @@
         Service20FsfwTm.__common_checks(instance.pus_tm)
         return instance
 
     def pack(self) -> bytearray:
         return self.pus_tm.pack()
 
     @property
-    def time_provider(self) -> Optional[CcsdsTimeProvider]:
-        return self.pus_tm.time_provider
+    def timestamp(self) -> bytes:
+        return self.pus_tm.timestamp
 
     @property
     def object_id(self) -> bytes:
         return bytes(self.source_data[0:4])
 
     @property
     def service(self) -> int:
@@ -123,17 +118,17 @@
     def source_data(self) -> bytes:
         return self.pus_tm.source_data
 
     @classmethod
     def empty(cls) -> Service20FsfwTm:
         return cls(
             subservice=0,
-            time_provider=CdsShortTimestamp.empty(),
             apid=0,
             source_data=bytes([0, 0, 0, 0]),
+            timestamp=bytes(),
         )
 
     @property
     def sp_header(self) -> SpacePacketHeader:
         return self.pus_tm.space_packet_header
 
     @property
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s23_filemgmt.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s23_filemgmt.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s2_rawcmd.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s2_rawcmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Base class for implementation of PUS Service 2 handling.
 """
+
 from __future__ import annotations
 
 from typing import Optional
 
 from deprecated.sphinx import deprecated
 from spacepackets.ccsds.time import CcsdsTimeProvider
 from spacepackets.ecss.tm import CdsShortTimestamp, PusTelemetry
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s3_fsfw_hk.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s3_fsfw_hk.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s3_hk_base.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s3_hk_base.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s5_fsfw_event.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s5_fsfw_event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 """Contains classes and functions to deserialize PUS Service 5 Telemetry
 """
 from __future__ import annotations
 
 import dataclasses
 import struct
-from typing import Optional
 
 from spacepackets import SpacePacketHeader
 from spacepackets.ccsds.spacepacket import PacketId, PacketSeqCtrl
-from spacepackets.ccsds.time import CcsdsTimeProvider
 from spacepackets.ecss.defs import PusService
 from spacepackets.ecss.pus_5_event import Subservice
 from spacepackets.ecss.tm import CdsShortTimestamp, AbstractPusTm, PusTelemetry
 from tmtccmd.pus.s5_fsfw_event_defs import Severity
 
 
 @dataclasses.dataclass
@@ -48,46 +46,46 @@
         param2 = struct.unpack("!I", data[10:14])[0]
         return cls(event_id, object_id, param1, param2)
 
 
 class Service5Tm(AbstractPusTm):
     def __init__(
         self,
+        apid: int,
         subservice: Subservice,
         event: EventDefinition,
-        time_provider: Optional[CdsShortTimestamp],
+        timestamp: bytes,
         ssc: int = 0,
-        apid: int = -1,
         packet_version: int = 0b000,
         space_time_ref: int = 0b0000,
         destination_id: int = 0,
     ):
         """Create a FSFW tailored Event Service 5 telemetry instance.
         Use the unpack function to create an instance from a raw bytestream instead.
         :raises ValueError: Invalid input arguments
         """
         self.pus_tm = PusTelemetry(
             service=PusService.S5_EVENT,
             subservice=subservice,
-            time_provider=time_provider,
+            timestamp=timestamp,
             seq_count=ssc,
             source_data=event.pack(),
             apid=apid,
             packet_version=packet_version,
             space_time_ref=space_time_ref,
             destination_id=destination_id,
         )
 
     @property
     def sp_header(self) -> SpacePacketHeader:
         return self.pus_tm.space_packet_header
 
     @property
-    def time_provider(self) -> Optional[CcsdsTimeProvider]:
-        return self.pus_tm.time_provider
+    def timestamp(self) -> bytes:
+        return self.pus_tm.timestamp
 
     def pack(self) -> bytearray:
         return self.pus_tm.pack()
 
     @property
     def service(self) -> int:
         return self.pus_tm.service
@@ -111,31 +109,30 @@
     @property
     def source_data(self) -> bytes:
         return self.pus_tm.source_data
 
     @classmethod
     def __empty(cls) -> Service5Tm:
         return cls(
+            apid=0x0,
             subservice=Subservice.TM_INFO_EVENT,
             event=EventDefinition.empty(),
-            time_provider=CdsShortTimestamp.empty(),
+            timestamp=CdsShortTimestamp.empty().pack(),
         )
 
     @classmethod
     def from_tm(cls, pus_tm: PusTelemetry) -> Service5Tm:
         instance = cls.__empty()
         instance.pus_tm = pus_tm
         return instance
 
     @classmethod
-    def unpack(
-        cls, data: bytes, time_reader: Optional[CcsdsTimeProvider]
-    ) -> Service5Tm:
+    def unpack(cls, data: bytes, timestamp_len: int) -> Service5Tm:
         instance = cls.__empty()
-        instance.pus_tm = PusTelemetry.unpack(data=data, time_reader=time_reader)
+        instance.pus_tm = PusTelemetry.unpack(data=data, timestamp_len=timestamp_len)
         return instance
 
     @property
     def severity(self) -> Severity:
         if self.subservice == Subservice.TM_INFO_EVENT:
             return Severity.INFO
         elif self.subservice == Subservice.TM_LOW_SEVERITY_EVENT:
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/pus/tm/s8_fsfw_action.py` & `tmtccmd-8.0.0rc2/tmtccmd/pus/tm/s8_fsfw_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Contains classes and functions to handle PUS Service 8 telemetry.
 """
+
 from __future__ import annotations
 import struct
 from typing import Optional
 from deprecated.sphinx import deprecated
 
 from spacepackets.ccsds.time import CcsdsTimeProvider
 from spacepackets.ecss import PusService
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/__init__.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     RawTcEntry,
     PacketDelayEntry,
     LogQueueEntry,
 )
 from .procedure import (
     TcProcedureBase,
     TcProcedureType,
-    DefaultProcedureInfo,
+    TreeCommandingProcedure,
     CustomProcedureInfo,
     ProcedureWrapper,
 )
 
 from .handler import FeedWrapper, TcHandlerBase, SendCbParams
 from .decorator import service_provider, route_to_registered_service_handlers
 from .common import *  # noqa re-export
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/ccsds_seq_sender.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/ccsds_seq_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Used to send multiple TCs in sequence"""
+
 import enum
 import logging
 from datetime import timedelta
 from typing import Optional
 
 from spacepackets.countdown import Countdown
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/ccsds_tm_listener.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/ccsds_tm_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the TmListener which can be used to listen to Telemetry in the background"""
+
 from typing import Dict, List, Tuple
 
 from spacepackets.ccsds.spacepacket import get_apid_from_raw_space_packet
 
 from tmtccmd.tmtc.common import TelemetryQueueT, CcsdsTmHandler
 from tmtccmd.com import ComInterface
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/common.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import enum
 import abc
 import logging
 from typing import Deque, List, Any, Dict, Optional
 from spacepackets.ecss.tm import PusTelemetry
 
 
-TelemetryListT = List[bytes]
+TelemetryList = List[bytes]
+# Deprecated type alias.
+TelemetryListT = TelemetryList
 TelemetryQueueT = Deque[bytes]
 
 PusTmQueue = Deque[PusTelemetry]
 PusTmListT = List[PusTelemetry]
 
 PusTmQueueT = Deque[PusTmListT]
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/decorator.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/decorator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import dataclasses
 import functools
 
 from tmtccmd.tmtc import TcHandlerBase
-from tmtccmd.tmtc.procedure import DefaultProcedureInfo
+from tmtccmd.tmtc.procedure import TreeCommandingProcedure
 from tmtccmd.tmtc.queue import DefaultPusQueueHelper
 
 SERVICE_HANDLER_DICT = dict()
 
 
 @dataclasses.dataclass
 class ServiceProviderParams:
     handler_base: TcHandlerBase
-    info: DefaultProcedureInfo
+    info: TreeCommandingProcedure
     queue_helper: DefaultPusQueueHelper
     op_code: str
 
 
 def service_provider(service: str):
     """Decorator. TODO: Documentation"""
     global SERVICE_HANDLER_DICT
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/handler.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/handler.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/procedure.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/procedure.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import enum
 from typing import Any, cast, Type, Optional
 
 from tmtccmd.cfdp import CfdpRequestWrapper
 
 
 class TcProcedureType(enum.Enum):
-    DEFAULT = 0
+    TREE_COMMANDING = 0
     CFDP = 1
     CUSTOM = 2
 
 
 class TcProcedureBase:
     def __init__(self, ptype: TcProcedureType):
         self.ptype = ptype
@@ -21,35 +21,37 @@
         super().__init__(TcProcedureType.CUSTOM)
         self.procedure = procedure
 
     def __repr__(self):
         return f"{self.__class__.__name__}(info={self.procedure!r}"
 
 
-class DefaultProcedureInfo(TcProcedureBase):
+class TreeCommandingProcedure(TcProcedureBase):
     """Generic abstraction for procedures. A procedure can be a single command or a sequence
     of commands. Generally, one procedure is mapped to a specific TC queue which is packed
     during run-time"""
 
     def __init__(self, cmd_path: Optional[str]):
-        super().__init__(TcProcedureType.DEFAULT)
+        super().__init__(TcProcedureType.TREE_COMMANDING)
         self.cmd_path = cmd_path
 
     @classmethod
     def empty(cls):
         return cls(None)
 
     def __repr__(self):
         return f"CmdInfo(cmd_path={self.cmd_path!r})"
 
-    def __eq__(self, other: DefaultProcedureInfo) -> bool:
-        return self.cmd_path == other.cmd_path
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, TreeCommandingProcedure):
+            return self.cmd_path == other.cmd_path
+        return False
 
 
-class CfdpProcedureInfo(TcProcedureBase):
+class CfdpProcedure(TcProcedureBase):
     def __init__(self):
         super().__init__(TcProcedureType.CFDP)
         self.request_wrapper = CfdpRequestWrapper(None)
 
     @property
     def cfdp_request_type(self):
         return self.request_wrapper.request
@@ -77,24 +79,24 @@
         expected_type: TcProcedureType,
     ) -> Any:
         assert self.procedure is not None
         if obj.ptype != expected_type:
             raise TypeError(f"Invalid object {obj} for type {self.procedure.ptype}")
         return cast(obj_type, obj)
 
-    def to_def_procedure(self) -> DefaultProcedureInfo:
+    def to_tree_commanding_procedure(self) -> TreeCommandingProcedure:
         assert self.procedure is not None
         return self.__cast_internally(
-            DefaultProcedureInfo, self.procedure, TcProcedureType.DEFAULT
+            TreeCommandingProcedure, self.procedure, TcProcedureType.TREE_COMMANDING
         )
 
-    def to_cfdp_procedure(self) -> CfdpProcedureInfo:
+    def to_cfdp_procedure(self) -> CfdpProcedure:
         assert self.procedure is not None
         return self.__cast_internally(
-            CfdpProcedureInfo, self.procedure, TcProcedureType.CFDP
+            CfdpProcedure, self.procedure, TcProcedureType.CFDP
         )
 
     def to_custom_procedure(self) -> CustomProcedureInfo:
         assert self.procedure is not None
         return self.__cast_internally(
             CustomProcedureInfo, self.procedure, TcProcedureType.CUSTOM
         )
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/queue.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/queue.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from spacepackets.ccsds import SpacePacket
 from spacepackets.ecss import PusService, PusVerificator, check_pus_crc
 from spacepackets.ecss.tc import PusTelecommand
 from spacepackets.seqcount import ProvidesSeqCount
 
 from tmtccmd.pus.s11_tc_sched import Subservice as Pus11Subservice
-from tmtccmd.tmtc.procedure import DefaultProcedureInfo, TcProcedureBase
+from tmtccmd.tmtc.procedure import TreeCommandingProcedure, TcProcedureBase
 
 
 class TcQueueEntryType(Enum):
     PUS_TC = "pus-tc"
     CCSDS_TC = "ccsds-tc"
     RAW_TC = "raw-tc"
     CUSTOM = "custom"
@@ -106,32 +106,35 @@
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.delay_time!r})"
 
 
 class QueueEntryHelper:
     def __init__(self, base: Optional[TcQueueEntryBase]):
-        self.base = base
+        self.entry = base
 
     @property
     def is_tc(self) -> bool:
-        return self.base.is_tc()
+        assert self.entry is not None
+        return self.entry.is_tc()
 
     @property
     def entry_type(self) -> TcQueueEntryType:
-        return self.base.etype
+        assert self.entry is not None
+        return self.entry.etype
 
     def __cast_internally(
         self,
         obj_type: Type[TcQueueEntryBase],
         expected_type: TcQueueEntryType,
     ) -> Any:
-        if self.base.etype != expected_type:
-            raise TypeError(f"Invalid object {self.base} for type {expected_type}")
-        return cast(obj_type, self.base)
+        assert self.entry is not None
+        if self.entry.etype != expected_type:
+            raise TypeError(f"Invalid object {self.entry} for type {expected_type}")
+        return cast(obj_type, self.entry)
 
     def to_log_entry(self) -> LogQueueEntry:
         return self.__cast_internally(LogQueueEntry, TcQueueEntryType.LOG)
 
     def to_pus_tc_entry(self) -> PusTcEntry:
         return self.__cast_internally(PusTcEntry, TcQueueEntryType.PUS_TC)
 
@@ -157,15 +160,15 @@
     ):
         self.info = info
         self.queue = queue
         self.inter_cmd_delay = inter_cmd_delay
 
     @classmethod
     def empty(cls):
-        return cls(DefaultProcedureInfo.empty(), deque())
+        return cls(TreeCommandingProcedure.empty(), deque())
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}(info={self.info!r}, queue={self.queue!r}, "
             f"inter_cmd_delay={self.inter_cmd_delay!r})"
         )
 
@@ -247,22 +250,25 @@
                 pus_entry.pus_tc.service == PusService.S11_TC_SCHED
                 and pus_entry.pus_tc.subservice == Pus11Subservice.TC_INSERT
             ):
                 self._handle_time_tagged_tc(pus_entry.pus_tc)
             self._pus_packet_handler(pus_entry.pus_tc)
 
     def _handle_time_tagged_tc(self, pus_tc: PusTelecommand):
-        pus_tc_raw = pus_tc.app_data[self.tc_sched_timestamp_len :]
+        new_pus_tc_app_data = bytearray()
+        new_pus_tc_app_data.extend(pus_tc.app_data[: self.tc_sched_timestamp_len])
+        pus_tc_raw = new_pus_tc_app_data[self.tc_sched_timestamp_len :]
         if not check_pus_crc(pus_tc_raw):
             raise ValueError(
                 f"crc check on contained PUS TC with length {len(pus_tc_raw)} failed"
             )
         time_tagged_tc = PusTelecommand.unpack(pus_tc_raw)
         self._pus_packet_handler(time_tagged_tc)
-        pus_tc.app_data[self.tc_sched_timestamp_len :] = time_tagged_tc.pack()
+        new_pus_tc_app_data.extend(time_tagged_tc.pack())
+        pus_tc._app_data = new_pus_tc_app_data
 
     def _pus_packet_handler(self, pus_tc: PusTelecommand):
         recalc_crc = False
         if self.pus_apid is not None:
             recalc_crc = True
             pus_tc.apid = self.pus_apid
         if self.seq_cnt_provider is not None:
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/tmtc/tm_base.py` & `tmtccmd-8.0.0rc2/tmtccmd/tmtc/tm_base.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/util/conf_util.py` & `tmtccmd-8.0.0rc2/tmtccmd/util/conf_util.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/util/hammingcode.py` & `tmtccmd-8.0.0rc2/tmtccmd/util/hammingcode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Hamming Code Implementation
 Hamming codes belong to the family of linear error correcting codes.
 Documentation: https://en.wikipedia.org/wiki/Hamming_code
 They can be used to identify up to two bit errors and correct one bit error per 256 byte block.
 """
+
 import logging
 from enum import Enum
 
 # Translated from ATMEL C library.
 # /* ----------------------------------------------------------------------------
 # *         ATMEL Microcontroller Software Support
 # * ----------------------------------------------------------------------------
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/util/json.py` & `tmtccmd-8.0.0rc2/tmtccmd/util/json.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd/util/obj_id.py` & `tmtccmd-8.0.0rc2/tmtccmd/util/obj_id.py`

 * *Files identical despite different names*

### Comparing `tmtccmd-8.0.0rc1/tmtccmd.egg-info/PKG-INFO` & `tmtccmd-8.0.0rc2/tmtccmd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmtccmd
-Version: 8.0.0rc1
+Version: 8.0.0rc2
 Summary: TMTC Commander Core
 Author-email: Robin Mueller <robin.mueller.m@gmail.com>
 License: Apache-2.0 or MIT
 Project-URL: Homepage, https://github.com/robamu-org/tmtccmd
 Keywords: ccsds,ecss,space,communication,packet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,16 +27,16 @@
 Requires-Dist: colorama~=0.4.0
 Requires-Dist: colorlog~=6.6
 Requires-Dist: cobs~=1.2
 Requires-Dist: prompt-toolkit~=3.0
 Requires-Dist: Deprecated~=1.2
 Requires-Dist: pyserial~=3.5
 Requires-Dist: dle-encoder~=0.2.3
-Requires-Dist: spacepackets~=0.23.0
-Requires-Dist: cfdp-py~=0.1.0
+Requires-Dist: spacepackets<0.25,>=0.24.0
+Requires-Dist: cfdp-py~=0.1.1
 Provides-Extra: gui
 Requires-Dist: PyQt6~=6.6; extra == "gui"
 Provides-Extra: test
 Requires-Dist: pyfakefs~=4.5; extra == "test"
 
 <p align="center"> <img src="misc/logo.png" width="40%"> </p>
```

### Comparing `tmtccmd-8.0.0rc1/tmtccmd.egg-info/SOURCES.txt` & `tmtccmd-8.0.0rc2/tmtccmd.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,19 +13,14 @@
 docs/communication.rst
 docs/conf.py
 docs/gettingstarted.rst
 docs/index.rst
 docs/introduction.rst
 docs/make.bat
 docs/requirements.txt
-docs/.pytest_cache/.gitignore
-docs/.pytest_cache/CACHEDIR.TAG
-docs/.pytest_cache/README.md
-docs/.pytest_cache/v/cache/nodeids
-docs/.pytest_cache/v/cache/stepwise
 docs/api/cfdp.rst
 docs/api/com.rst
 docs/api/config.rst
 docs/api/core.rst
 docs/api/fsfw.rst
 docs/api/logging.rst
 docs/api/pus.rst
@@ -37,31 +32,39 @@
 docs/images/example_system.png
 docs/images/tmtccmd_usage.PNG
 docs/images/tmtccmd_usage.graphml
 docs/images/tmtccmd_usage.pdf
 examples/app/tmtcc.py
 misc/logo-tiny.png
 misc/logo_medium.png
-tests/.coverage
 tests/.gitignore
 tests/__init__.py
 tests/hook_obj_mock.py
 tests/test_backend.py
 tests/test_printer.py
 tests/test_pus_verif_log.py
 tests/test_queue.py
 tests/test_seq_sender.py
 tests/test_tm_handler.py
 tests/test_util.py
 tests/.pytest_cache/.gitignore
 tests/.pytest_cache/CACHEDIR.TAG
 tests/.pytest_cache/README.md
-tests/.pytest_cache/v/cache/lastfailed
 tests/.pytest_cache/v/cache/nodeids
 tests/.pytest_cache/v/cache/stepwise
+tests/cfdp/.pytest_cache/.gitignore
+tests/cfdp/.pytest_cache/CACHEDIR.TAG
+tests/cfdp/.pytest_cache/README.md
+tests/cfdp/.pytest_cache/v/cache/lastfailed
+tests/cfdp/.pytest_cache/v/cache/nodeids
+tests/cfdp/.pytest_cache/v/cache/stepwise
+tests/cfdp/log/tmtccmd_raw_pus_2023-10-09.log
+tests/cfdp/log/tmtccmd_raw_pus_2023-10-09.log.1
+tests/cfdp/log/tmtccmd_raw_pus_2023-10-17.log
+tests/cfdp/log/tmtccmd_raw_pus_2023-10-17.log.1
 tests/com/__init__.py
 tests/com/test_dummy.py
 tests/com/test_serial_cobs.py
 tests/com/test_serial_dle.py
 tests/com/test_tcp.py
 tests/com/test_udp.py
 tests/com/test_utils.py
@@ -73,35 +76,27 @@
 tests/config/test_prompt.py
 tests/config/.pytest_cache/.gitignore
 tests/config/.pytest_cache/CACHEDIR.TAG
 tests/config/.pytest_cache/README.md
 tests/config/.pytest_cache/v/cache/lastfailed
 tests/config/.pytest_cache/v/cache/nodeids
 tests/config/.pytest_cache/v/cache/stepwise
-tests/config/log/tmtccmd_raw_pus_2023-11-16.log
-tests/config/log/tmtccmd_raw_pus_2023-11-16.log.1
 tests/pus/__init__.py
 tests/pus/test_srv20.py
-tests/pus/.pytest_cache/.gitignore
-tests/pus/.pytest_cache/CACHEDIR.TAG
-tests/pus/.pytest_cache/README.md
-tests/pus/.pytest_cache/v/cache/nodeids
-tests/pus/.pytest_cache/v/cache/stepwise
 tests/tc/__init__.py
 tests/tc/test_srv20.py
 tests/tm/__init__.py
 tests/tm/test_srv1.py
 tests/tm/test_srv17.py
 tests/tm/test_srv20.py
 tests/tm/test_srv200.py
 tests/tm/test_srv5.py
 tests/tm/.pytest_cache/.gitignore
 tests/tm/.pytest_cache/CACHEDIR.TAG
 tests/tm/.pytest_cache/README.md
-tests/tm/.pytest_cache/v/cache/lastfailed
 tests/tm/.pytest_cache/v/cache/nodeids
 tests/tm/.pytest_cache/v/cache/stepwise
 tmtccmd/__init__.py
 tmtccmd/com_if.py
 tmtccmd/version.py
 tmtccmd.egg-info/PKG-INFO
 tmtccmd.egg-info/SOURCES.txt
@@ -199,20 +194,8 @@
 tmtccmd/util/countdown.py
 tmtccmd/util/exit.py
 tmtccmd/util/hammingcode.py
 tmtccmd/util/json.py
 tmtccmd/util/obj_id.py
 tmtccmd/util/retval.py
 tmtccmd/util/seqcnt.py
-tmtccmd/util/tmtc_printer.py
-venv/bin/rst2html.py
-venv/bin/rst2html4.py
-venv/bin/rst2html5.py
-venv/bin/rst2latex.py
-venv/bin/rst2man.py
-venv/bin/rst2odt.py
-venv/bin/rst2odt_prepstyles.py
-venv/bin/rst2pseudoxml.py
-venv/bin/rst2s5.py
-venv/bin/rst2xetex.py
-venv/bin/rst2xml.py
-venv/bin/rstpep2html.py
+tmtccmd/util/tmtc_printer.py
```

