# Comparing `tmp/psrpcore-0.2.2.tar.gz` & `tmp/psrpcore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psrpcore-0.2.2.tar", last modified: Tue Feb 28 22:06:04 2023, max compression
+gzip compressed data, was "psrpcore-0.3.0.tar", last modified: Tue Apr 23 00:06:50 2024, max compression
```

## Comparing `psrpcore-0.2.2.tar` & `psrpcore-0.3.0.tar`

### file list

```diff
@@ -1,78 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.968561 psrpcore-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-28 22:05:55.000000 psrpcore-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-28 22:05:55.000000 psrpcore-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-02-28 22:05:55.000000 psrpcore-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-28 22:05:55.000000 psrpcore-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-28 22:05:55.000000 psrpcore-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-02-28 22:06:04.968561 psrpcore-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-28 22:05:55.000000 psrpcore-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.960560 psrpcore-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.960560 psrpcore-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/_static/.keep
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/_static/ConvertTo-PythonClass.ps1
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/protocol.md
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/scenarios.md
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/transport.md
--rw-r--r--   0 runner    (1001) docker     (123)    30358 2023-02-28 22:05:55.000000 psrpcore-0.2.2/docs/types.md
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-02-28 22:05:55.000000 psrpcore-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-28 22:05:55.000000 psrpcore-0.2.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-28 22:05:55.000000 psrpcore-0.2.2/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 22:06:04.968561 psrpcore-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.956560 psrpcore-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.964561 psrpcore-0.2.2/src/psrpcore/
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21509 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25040 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    42065 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    75252 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28828 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/_server.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.964561 psrpcore-0.2.2/src/psrpcore/types/
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39766 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9823 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    52505 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    29785 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_host.py
--rw-r--r--   0 runner    (1001) docker     (123)    45203 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    34053 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_psrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    38134 2023-02-28 22:05:55.000000 psrpcore-0.2.2/src/psrpcore/types/_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.964561 psrpcore-0.2.2/src/psrpcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-02-28 22:06:04.000000 psrpcore-0.2.2/src/psrpcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-02-28 22:06:04.000000 psrpcore-0.2.2/src/psrpcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 22:06:04.000000 psrpcore-0.2.2/src/psrpcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-28 22:06:04.000000 psrpcore-0.2.2/src/psrpcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-28 22:06:04.000000 psrpcore-0.2.2/src/psrpcore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.968561 psrpcore-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19921 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    71463 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    55475 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_host_call.py
--rw-r--r--   0 runner    (1001) docker     (123)    36387 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_integration_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52850 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_integration_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    17874 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 22:06:04.968561 psrpcore-0.2.2/tests/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31330 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    40850 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_complex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15553 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_host.py
--rw-r--r--   0 runner    (1001) docker     (123)    52834 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_primitive.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_psrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11422 2023-02-28 22:05:55.000000 psrpcore-0.2.2/tests/types/test_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.347411 psrpcore-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-23 00:06:44.000000 psrpcore-0.3.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 00:06:44.000000 psrpcore-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-23 00:06:44.000000 psrpcore-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-23 00:06:44.000000 psrpcore-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-23 00:06:44.000000 psrpcore-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-23 00:06:50.347411 psrpcore-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-23 00:06:44.000000 psrpcore-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.335410 psrpcore-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.335410 psrpcore-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/_static/.keep
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/_static/ConvertTo-PythonClass.ps1
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/minishell.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/protocol.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/psrpcore.md
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/psrpcore.types.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11837 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/scenarios.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/transport.md
+-rw-r--r--   0 runner    (1001) docker     (127)    29055 2024-04-23 00:06:44.000000 psrpcore-0.3.0/docs/types.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-23 00:06:44.000000 psrpcore-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 00:06:44.000000 psrpcore-0.3.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 00:06:44.000000 psrpcore-0.3.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 00:06:50.347411 psrpcore-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.331411 psrpcore-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.339410 psrpcore-0.3.0/src/psrpcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24950 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13083 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_clixml_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42064 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72138 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28526 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.339410 psrpcore-0.3.0/src/psrpcore/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39371 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51877 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28835 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43051 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32430 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_psrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43799 2024-04-23 00:06:44.000000 psrpcore-0.3.0/src/psrpcore/types/_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.347411 psrpcore-0.3.0/src/psrpcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-23 00:06:50.000000 psrpcore-0.3.0/src/psrpcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-23 00:06:50.000000 psrpcore-0.3.0/src/psrpcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:06:50.000000 psrpcore-0.3.0/src/psrpcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 00:06:50.000000 psrpcore-0.3.0/src/psrpcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 00:06:50.000000 psrpcore-0.3.0/src/psrpcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.343411 psrpcore-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/clixml_shell_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19984 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71463 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_clixml_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12010 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55475 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_host_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36387 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_integration_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52844 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_integration_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17874 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:50.343411 psrpcore-0.3.0/tests/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31329 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40850 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52834 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_primitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19095 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_psrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_serialize_clixml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17382 2024-04-23 00:06:44.000000 psrpcore-0.3.0/tests/types/test_serializer.py
```

### Comparing `psrpcore-0.2.2/LICENSE` & `psrpcore-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/PKG-INFO` & `psrpcore-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrpcore
-Version: 0.2.2
+Version: 0.3.0
 Summary: Core components for the PowerShell Remoting Protocol
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,22 +27,23 @@
         
 Project-URL: homepage, https://github.com/jborean93/psrpcore
 Project-URL: documentation, https://psrpcore.readthedocs.io/
 Keywords: psrp,pwsh,powershell,remoting
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
 
 # psrpcore - Python PowerShell Remoting Protocol Core Library
 
 [![Test workflow](https://github.com/jborean93/psrpcore/actions/workflows/ci.yml/badge.svg)](https://github.com/jborean93/psrpcore/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/jborean93/psrpcore/branch/main/graph/badge.svg?token=UEA7VoocS5)](https://codecov.io/gh/jborean93/psrpcore)
 [![PyPI version](https://badge.fury.io/py/psrpcore.svg)](https://badge.fury.io/py/psrpcore)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/jborean93/PSAccessToken/blob/main/LICENSE)
@@ -56,15 +57,15 @@
 ## Documentation
 
 Documentation is available at https://psrpcore.readthedocs.io/.
 
 
 ## Requirements
 
-* CPython 3.7+
+* CPython 3.8+
 * [cryptography](https://github.com/pyca/cryptography)
 
 
 ## Install
 
 ### From PyPI
```

### Comparing `psrpcore-0.2.2/README.md` & `psrpcore-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ## Documentation
 
 Documentation is available at https://psrpcore.readthedocs.io/.
 
 
 ## Requirements
 
-* CPython 3.7+
+* CPython 3.8+
 * [cryptography](https://github.com/pyca/cryptography)
 
 
 ## Install
 
 ### From PyPI
```

### Comparing `psrpcore-0.2.2/docs/Makefile` & `psrpcore-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/docs/_static/ConvertTo-PythonClass.ps1` & `psrpcore-0.3.0/docs/_static/ConvertTo-PythonClass.ps1`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/docs/conf.py` & `psrpcore-0.3.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
+import re
 import sys
 import typing
 
 from sphinx.application import Sphinx
 
 sys.path.insert(0, os.path.abspath(".."))
 
-import re
 
 from psrpcore.types import PSEnumBase, PSFlagBase, PSObject
 from psrpcore.types._base import _UnsetValue
 
 _PARAM_PATTERN = re.compile(r":param (\w*):")
 
 # -- Project information -----------------------------------------------------
@@ -37,21 +37,24 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "myst_parser",
     "sphinx_rtd_theme",
     "sphinx.ext.autodoc",
-    "sphinx.ext.coverage",
+    "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
-    "sphinxcontrib.apidoc",
 ]
 
-apidoc_module_dir = "../src/psrpcore"
-apidoc_output_dir = "source"
+# Uses type hints for class/func defs
+autodoc_typehints = "both"
+autodoc_typehints_description_target = "documented"
+
+# Allows linking to Python types
+intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = [
     "_templates",
 ]
 
 # List of patterns, relative to source directory, that match files and
@@ -124,21 +127,17 @@
     insertion_offset = 0
     for idx, param_name in insertions:
         prop = prop_entries.get(param_name)
         if not prop:
             continue
 
         param_type = prop.ps_type if prop.ps_type is not None else PSObject
-        if param_type.__module__ == "builtins":
-            param_type_str = param_type.__name__
-
-        else:
-            param_type_str = f"{param_type.__module__}.{param_type.__name__}"
-
-        type_line = f":type {param_name}: :obj:`{param_type.__name__} " f"<{param_type_str}>`"
+        type_line = f":type {param_name}: {param_type.__name__}"
+        if not prop.mandatory:
+            type_line += " | None"
         lines.insert(idx + insertion_offset, type_line)
         insertion_offset += 1
 
 
 def autodoc_process_signature(
     app: Sphinx,
     what: str,
@@ -177,15 +176,15 @@
             entry = f"{prop.name}: {ps_type_str}"
 
         else:
             default_value = prop._value
             if prop._value == _UnsetValue:
                 default_value = None
 
-            entry = f"{prop.name}: Optional[{ps_type_str}] = {default_value!r}"
+            entry = f"{prop.name}: {ps_type_str} | None = {default_value!r}"
 
         kwargs.append(entry)
 
     signature = f'({", ".join(kwargs)})' if kwargs else None
 
     return signature, return_annotations
 
@@ -194,15 +193,14 @@
     app: Sphinx,
     what: str,
     name: str,
     obj: typing.Any,
     skip: bool,
     options: typing.Dict[str, typing.Any],
 ) -> bool:
-    a = ""
     return (
         skip
         # This is a metadata class for all PSObject types, end users don't need
         # to know about this for every single class in the codebase.
         or (name == "PSObject" and (obj != PSObject and obj != PSObject.PSObject))
         or name
         in [
@@ -214,11 +212,10 @@
         ]
     )
 
 
 def setup(
     app: Sphinx,
 ) -> None:
-
     app.connect("autodoc-process-docstring", autodoc_process_docstring)
     app.connect("autodoc-process-signature", autodoc_process_signature)
     app.connect("autodoc-skip-member", autodoc_skip_member_handler)
```

### Comparing `psrpcore-0.2.2/docs/index.rst` & `psrpcore-0.3.0/docs/index.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-PSRP Core: Python Implementation of the PowerShell Remoting Protocol
-====================================================================
+# PSRP Core: Python Implementation of the PowerShell Remoting Protocol
 
 PowerShell Remoting Protocol is a protocol used by PowerShell to invoke commands
 across the network just different processes. This library is designed around
 the Sans-IO concept and focuses entirely on the protocol itself. It is up to
 the user of this module to provide the IO using their desired mechanism.
 
 This module is brand new and is still in development so the docs are very
 brief and will be expanded upon in the future.
 
+```{eval-rst}
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    protocol
+   minishell
    scenarios
    transport
    types
-   source/modules
 
-Indices and tables
-==================
+.. toctree::
+   :maxdepth: 1
+   :caption: API:
 
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+   psrpcore
+   psrpcore.types
+```
```

### Comparing `psrpcore-0.2.2/docs/make.bat` & `psrpcore-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/docs/protocol.md` & `psrpcore-0.3.0/docs/protocol.md`

 * *Files 25% similar despite different names*

```diff
@@ -7,55 +7,58 @@
 
 ## Glossary
 
 Here are some of the key terms used in PSRP and this library:
 
 ### Runspace Pool
 
-A runspace pool is a collection of [runspaces](./protocol.html/#runspace).
+A runspace pool is a collection of [runspaces](#protocol-runspace).
 This is the primary interface that a client and server used to communicate with each other.
 A runspace pool is represented by the following classes:
 
-+ [ClientRunspacePool](./source/psrpcore.html#psrpcore.ClientRunspacePool)
-+ [ServerRunspacePool](./source/psrpcore.html#psrpcore.ServerRunspacePool)
++ [ClientRunspacePool](psrpcore.ClientRunspacePool)
++ [ServerRunspacePool](psrpcore.ServerRunspacePool)
 
+(protocol-runspace)=
 ### Runspace
 
-A runspace is an entity that is able to run a [pipeline](./protocol.html/#pipeline) (only 1 concurrently) and also contains session state information, like variables.
+A runspace is an entity that is able to run a [pipeline](#protocol-pipeline) (only 1 concurrently) and also contains session state information, like variables.
 There is no specific runspace class in this library as the same functionality is offered by using a runspace pool with a min and max count of 1.
 
+(protocol-pipeline)=
 ### Pipeline
 
-A pipeline contains an ordered list of [commands](./protocol.html/#command) to be run.
+A pipeline contains an ordered list of [commands](#protocol-command) to be run.
 The output of the first command becomes the input to the next command in the list until all commands have been run.
 A pipeline is represented by the following classes:
 
-+ [ClientPowerShell](./source/psrpcore.html#psrpcore.ClientPowerShell)
++ [ClientPowerShell](psrpcore.ClientPowerShell)
   + Main pipeline used by a client to run a collection of PowerShell commands
-+ [ClientGetCommandMetadata](./source/psrpcore.html#psrpcore.ClientGetCommandMetadata)
++ [ClientGetCommandMetadata](psrpcore.ClientGetCommandMetadata)
   + Pipeline used by a client to extract command metadata of the connected runspace
-+ [ServerPipeline](./source/psrpcore.html#psrpcore.ServerPipeline)
++ [ServerPipeline](psrpcore.ServerPipeline)
   + Pipeline used by a server to represent the client pipeline requested
 
+(protocol-command)=
 ### Command
 
 A command is process that can be executed by the server.
 It contains the necessary instructions to tell the server what to run.
 A command is represent by the following class:
 
-+ [Command](./source/psrpcore.html#psrpcore.Command)
++ [Command](psrpcore.Command)
 
 ### PSHost
 
 A PSHost is the interface that is used by the runspace/pipeline to communicate with the user.
 This communication is typically, but not limited to, in the form of a console/terminal window.
 A PSHost is represented by the following classes:
 
-+ [ClientHostResponder](./source/psrpcore.html#psrpcore.ClientHostResponder)
-+ [ServerHostRequestor](./source/psrpcore.html#psrpcore.ServerHostRequestor)
++ [ClientHostResponder](psrpcore.ClientHostResponder)
++ [ServerHostRequestor](psrpcore.ServerHostRequestor)
 
 ### Fragment
 
 A fragment contains a message, or part of, that is the fundamental message streamed between the client and the server.
 The size of the fragment is defined by the underlying transport used.
 
 ### CLIXML
```

### Comparing `psrpcore-0.2.2/docs/scenarios.md` & `psrpcore-0.3.0/docs/scenarios.md`

 * *Files 10% similar despite different names*

```diff
@@ -42,19 +42,19 @@
                 raise Exception(f"Open failed {event.reason}")
 ```
 
 ### Exchanged Events
 
 |Message|Role|Purpose|
 |-|-|-|
-|[SessionCapability](./source/psrpcore.html#psrpcore.SessionCapabilityEvent)|Server|States the protocol versions offered by the client|
-|[InitRunspacePool](./source/psrpcore.html#psrpcore.InitRunspacePoolEvent)|Server|Runspace Pool configuration settings|
-|[SessionCapability](./source/psrpcore.html#psrpcore.SessionCapabilityEvent)|Client|States the protocol versions offered by the server|
-|[ApplicationPrivateData](./source/psrpcore.html#psrpcore.ApplicationPrivateDataEvent)|Client|Server provided data not processed by the PSRP layer.|
-|[RunspacePoolState](./source/psrpcore.html#psrpcore.RunspacePoolStateEvent)|Client|The final state which should be ``Opened``|
+|[SessionCapability](psrpcore.SessionCapabilityEvent)|Server|States the protocol versions offered by the client|
+|[InitRunspacePool](psrpcore.InitRunspacePoolEvent)|Server|Runspace Pool configuration settings|
+|[SessionCapability](psrpcore.SessionCapabilityEvent)|Client|States the protocol versions offered by the server|
+|[ApplicationPrivateData](psrpcore.ApplicationPrivateDataEvent)|Client|Server provided data not processed by the PSRP layer.|
+|[RunspacePoolState](psrpcore.RunspacePoolStateEvent)|Client|The final state which should be ``Opened``|
 
 
 ## Closing a Runspace Pool
 
 Closing a Runspace Pool is done by a transport specific message and is not covered by PSRP itself.
 
 ```python
@@ -79,22 +79,22 @@
 Before closing a Runspace Pool, all pipelines must be stopped or completed.
 Failure to do so could result in an indefinite hang until they have stopped naturally.
 
 ### Exchanged Events
 
 |Message|Role|Purpose|
 |-|-|-|
-|[RunspacePoolState](./source/psrpcore.html#psrpcore.RunspacePoolStateEvent)|Client|Final state to denote the pool has been closed|
+|[RunspacePoolState](psrpcore.RunspacePoolStateEvent)|Client|Final state to denote the pool has been closed|
 
 _Note: This message is not guaranteed to be sent and merely a formality. Actually closing the pool should be signaled by the transport protocol._
 
 
 ## Exchange a Session Key
 
-To serialize a [Secure String](./source/psrpcore.types.html#psrpcore.types.PSSecureString) the client must first perform a session key exchange.
+To serialize a [Secure String](psrpcore.types.PSSecureString) the client must first perform a session key exchange.
 This exchange has the client generate a public key unique to that runspace pool, send that to the server, and await the encrypted key response.
 Once the key has been exchange the client is able to send and decrypt secure strings.
 
 ```python
 import psrpcore
 
 client_pool = psrpcore.ClientRunspacePool()
@@ -110,23 +110,23 @@
 server_pool.next_event()
 
 # Send the encrypted session key back to the client and process the msg
 client_pool.receive_data(server_pool.data_to_send())
 client_pool.next_event()
 ```
 
-Older PowerShell versions could have the server request the key exchange by sending a [PublicKeyRequest](./source/psrpcore.html#psrpcore.PublicKeyRequestEvent) message.
+Older PowerShell versions could have the server request the key exchange by sending a [PublicKeyRequest](psrpcore.PublicKeyRequestEvent) message.
 When receiving this message the client is expected to perform this exchange like normal.
 
 ### Exchanged Events
 
 |Message|Role|Purpose|
 |-|-|-|
-|[PublicKey](./source/psrpcore.html#psrpcore.PublicKeyEvent)|Server|Base64 encoded public key generated by the client|
-|[EncryptedSessionKey](./source/psrpcore.html#psrpcore.EncryptedSessionKeyEvent)|Client|Encrypted session key generated by the server|
+|[PublicKey](psrpcore.PublicKeyEvent)|Server|Base64 encoded public key generated by the client|
+|[EncryptedSessionKey](psrpcore.EncryptedSessionKeyEvent)|Client|Encrypted session key generated by the server|
 
 
 ## Adjusting Runspace Count
 
 Once the Runspace Pool has been created it is possible to adjust the minimum and maximum runspace count in the pool.
 This is done by sending the request to adjust the count and awaiting the response from the server as to whether that was successful or not.
 
@@ -156,17 +156,17 @@
 assert avail_resp.success
 ```
 
 ### Exchanged Events
 
 |Message|Role|Purpose|
 |-|-|-|
-|[SetMinRunspaces](./source/psrpcore.html#psrpcore.SetMinRunspacesEvent)|Server|Request to adjust the min runspace count|
-|[SetMaxRunspaces](./source/psrpcore.html#psrpcore.SetMaxRunspacesEvent)|Server|Request to adjust the max runspace count|
-|[RunspaceAvailability](./source/psrpcore.html#psrpcore.SetRunspaceAvailabilityEvent)|Client|Whether the count was adjusted or not|
+|[SetMinRunspaces](psrpcore.SetMinRunspacesEvent)|Server|Request to adjust the min runspace count|
+|[SetMaxRunspaces](psrpcore.SetMaxRunspacesEvent)|Server|Request to adjust the max runspace count|
+|[RunspaceAvailability](psrpcore.SetRunspaceAvailabilityEvent)|Client|Whether the count was adjusted or not|
 
 
 ## Running a PowerShell Pipeline
 
 ```python
 import psrpcore
 
@@ -228,37 +228,38 @@
 One key thing to note is that the data is still exchanged on the underlying Runspace Pool.
 A call to ``data_to_send()`` is guaranteed to not mix messages targeted towards different pipelines or the pool in general.
 
 ### Exchanged Events
 
 |Message|Role|Purpose|
 |-|-|-|
-|[CreatePipeline](./source/psrpcore.html#psrpcore.CreatePipelineEvent)|Server|Contains the PowerShell pipeline details to invoke|
-|[PipelineInput](./source/psrpcore.html#psrpcore.PipelineInputEvent)|Server|Data to be sent as input to the first command in the pipeline|
-|[EndOfPipelineInput](./source/psrpcore.html#psrpcore.EndOfPipelineInputEvent)|Server|Signals no more input is expected|
-|[PipelineOutput](./source/psrpcore.html#psrpcore.PipelineOutputEvent)|Client|Output from the running pipeline|
-|[ErrorRecordMsg](./source/psrpcore.html#psrpcore.ErrorRecordEvent)|Client|Error record from the running pipeline|
-|[WarningRecordMsg](./source/psrpcore.html#psrpcore.WarningRecordEvent)|Client|Warning record from the running pipeline|
-|[VerboseRecordMsg](./source/psrpcore.html#psrpcore.VerboseRecordEvent)|Client|Verbose record from the running pipeline|
-|[DebugRecordMsg](./source/psrpcore.html#psrpcore.DebugRecordEvent)|Client|Debug record from the running pipeline|
-|[InformationRecordMsg](./source/psrpcore.html#psrpcore.InformationRecordEvent)|Client|Information record from the running pipeline|
-|[ProgressRecordMsg](./source/psrpcore.html#psrpcore.ProgressRecordEvent)|Client|Progress record from the running pipeline|
-|[PipelineState](./source/psrpcore.html#psrpcore.PipelineStateEvent)|Client|The pipeline state and optional error message if it failed|
+|[CreatePipeline](psrpcore.CreatePipelineEvent)|Server|Contains the PowerShell pipeline details to invoke|
+|[PipelineInput](psrpcore.PipelineInputEvent)|Server|Data to be sent as input to the first command in the pipeline|
+|[EndOfPipelineInput](psrpcore.EndOfPipelineInputEvent)|Server|Signals no more input is expected|
+|[PipelineOutput](psrpcore.PipelineOutputEvent)|Client|Output from the running pipeline|
+|[ErrorRecordMsg](psrpcore.ErrorRecordEvent)|Client|Error record from the running pipeline|
+|[WarningRecordMsg](psrpcore.WarningRecordEvent)|Client|Warning record from the running pipeline|
+|[VerboseRecordMsg](psrpcore.VerboseRecordEvent)|Client|Verbose record from the running pipeline|
+|[DebugRecordMsg](psrpcore.DebugRecordEvent)|Client|Debug record from the running pipeline|
+|[InformationRecordMsg](psrpcore.InformationRecordEvent)|Client|Information record from the running pipeline|
+|[ProgressRecordMsg](psrpcore.ProgressRecordEvent)|Client|Progress record from the running pipeline|
+|[PipelineState](psrpcore.PipelineStateEvent)|Client|The pipeline state and optional error message if it failed|
 
 The ``InformationRecordMsg`` is only used when talking to a PowerShell v5.1 or newer server.
 
-_Note: While running a pipeline can send a ``PipelineHostCall`` message as per [Sending a Host Call](./scenarios.html#sending-a-host-call)._
+_Note: While running a pipeline can send a ``PipelineHostCall`` message as per [Sending a Host Call](#scenarios-sending-a-host-call)._
 
 
+(scenarios-sending-a-host-call)=
 ## Sending a Host Call
 
 Interacting directly with the user is typically done through a host call.
 There are strict set of host calls defined in PSRP and the methods available depend on the host information that was defined on the Runspace Pool or Pipeline.
 Host calls are initiated by the server and, depending on the method invoked, can block further processing until a response is received.
-The [ClientHostResponder](./source/psrpcore.html#psrpcore.ClientHostResponder) and [ServerHostRequestor](./source/psrpcore.html#psrpcore.ServerHostRequestor) classes can be used to request and respond to host calls using well defined types.
+The [ClientHostResponder](psrpcore.ClientHostResponder) and [ServerHostRequestor](psrpcore.ServerHostRequestor) classes can be used to request and respond to host calls using well defined types.
 
 ```python
 import psrpcore
 import sys
 
 client_pool = psrpcore.ClientRunspacePool()
 client_host = psrpcore.ClientHostResponder(client_pool)
@@ -291,11 +292,11 @@
 
 _Note: While it is possible to send a host call as defined on the Runspace Pool it is typically done through a running Pipeline._
 
 ### Exchanged Events
 
 |Message|Role|Purpose|
 |-|-|-|
-|[RunspacePoolHostCall](./source/psrpcore.html#psrpcore.RunspacePoolHostCallEvent)|Client|The requested call to run on the client Runspace Pool host|
-|[PipelineHostCall](./source/psrpcore.html#psrpcore.PipelineHostCallEvent)|Client|The requested call to run on the client Pipeline host|
-|[RunspacePoolHostResponse](./source/psrpcore.html#psrpcore.RunspacePoolHostResponseEvent)|Server|The response, if any, of the Runspace Pool host call|
-|[PipelineHostResponse](./source/psrpcore.html#psrpcore.PipelineHostResponseEvent)|Server|The response, if any, of the Pipeline host call|
+|[RunspacePoolHostCall](psrpcore.RunspacePoolHostCallEvent)|Client|The requested call to run on the client Runspace Pool host|
+|[PipelineHostCall](psrpcore.PipelineHostCallEvent)|Client|The requested call to run on the client Pipeline host|
+|[RunspacePoolHostResponse](psrpcore.RunspacePoolHostResponseEvent)|Server|The response, if any, of the Runspace Pool host call|
+|[PipelineHostResponse](psrpcore.PipelineHostResponseEvent)|Server|The response, if any, of the Pipeline host call|
```

### Comparing `psrpcore-0.2.2/docs/transport.md` & `psrpcore-0.3.0/docs/transport.md`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/docs/types.md` & `psrpcore-0.3.0/docs/types.md`

 * *Files 8% similar despite different names*

```diff
@@ -120,46 +120,47 @@
 
 In [MS-PSRP](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/602ee78e-9a19-45ad-90fa-bb132b7cecec) there are three different type classes:
 
 * [Primitive types](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c8c85974-ffd7-4455-84a8-e49016c20683)
 * [Complex types](https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/406ad572-1ede-43e0-b063-e7291cda3e63)
 * Enum types - they are complex types but we consider them separate here
 
+(types-primitive-types)=
 ### Primitive Types
 
 Primitive types are the fundamental types that contain a value and optional properties.
 When it comes to working with primitive types for PSRP in Python, there exists a Python class for each primitive in `psrpcore.types` that subclasses both `PSObject` as well as the Python type it closely resembles.
 Here is the mapping of the primitive types:
 
 | .NET | psrpcore.type | Python Type | Native |
 |-|-|-|-|
-| [System.String](https://docs.microsoft.com/en-us/dotnet/api/system.string) | [PSString](./source/psrpcore.types.html#psrpcore.types.PSString) | str | Y |
-| [System.Char](https://docs.microsoft.com/en-us/dotnet/api/system.char) | [PSChar](./source/psrpcore.types.html#psrpcore.types.PSChar) | int¹ | N |
-| [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean) | [PSBool](./source/psrpcore.types.html#psrpcore.types.PSBool)² | bool | Y |
-| [System.DateTime](https://docs.microsoft.com/en-us/dotnet/api/system.datetime) | [PSDateTime](./source/psrpcore.types.html#psrpcore.types.PSDateTime) | datetime.datetime | Y |
-| [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/system.timespan) | [PSDuration](./source/psrpcore.types.html#psrpcore.types.PSDuration) | str | N |
-| [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/system.byte) | [PSByte](./source/psrpcore.types.html#psrpcore.types.PSByte) | int | N |
-| [System.SByte](https://docs.microsoft.com/en-us/dotnet/api/system.sbyte) | [PSSByte](./source/psrpcore.types.html#psrpcore.types.PSSByte) | int | N |
-| [System.UInt16](https://docs.microsoft.com/en-us/dotnet/api/system.uint16) | [PSUInt16](./source/psrpcore.types.html#psrpcore.types.PSUInt16) | int | N |
-| [System.Int16](https://docs.microsoft.com/en-us/dotnet/api/system.int16) | [PSInt16](./source/psrpcore.types.html#psrpcore.types.PSInt16) | int | N |
-| [System.UInt32](https://docs.microsoft.com/en-us/dotnet/api/system.uint32) | [PSUInt](./source/psrpcore.types.html#psrpcore.types.PSUInt) | int | N |
-| [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/system.int32) | [PSInt](./source/psrpcore.types.html#psrpcore.types.PSInt) | int | Y |
-| [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/system.uint64) | [PSUInt64](./source/psrpcore.types.html#psrpcore.types.PSUInt64) | int | N |
-| [System.Int64](https://docs.microsoft.com/en-us/dotnet/api/system.int64) | [PSInt64](./source/psrpcore.types.html#psrpcore.types.PSInt64) | int | N |
-| [System.Single](https://docs.microsoft.com/en-us/dotnet/api/system.single) | [PSSingle](./source/psrpcore.types.html#psrpcore.types.PSSingle) | float | Y |
-| [System.Double](https://docs.microsoft.com/en-us/dotnet/api/system.double) | [PSDouble](./source/psrpcore.types.html#psrpcore.types.PSDouble) | float | N |
-| [System.Decimal](https://docs.microsoft.com/en-us/dotnet/api/system.decimal) | [PSDecimal](./source/psrpcore.types.html#psrpcore.types.PSDecimal) | decimal.Decimal | Y |
-| `System.Byte[]` - Array | [PSByteArray](./source/psrpcore.types.html#psrpcore.types.PSByteArray) | bytes | Y |
-| [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/system.guid) | [PSGuid](./source/psrpcore.types.html#psrpcore.types.PSGuid) | uuid.UUID | Y |
-| [System.Uri](https://docs.microsoft.com/en-us/dotnet/api/system.uri) | [PSUri](./source/psrpcore.types.html#psrpcore.types.PSUri) | str | N |
+| [System.String](https://docs.microsoft.com/en-us/dotnet/api/system.string) | [PSString](psrpcore.types.PSString) | str | Y |
+| [System.Char](https://docs.microsoft.com/en-us/dotnet/api/system.char) | [PSChar](psrpcore.types.PSChar) | int¹ | N |
+| [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/system.boolean) | [PSBool](psrpcore.types.PSBool)² | bool | Y |
+| [System.DateTime](https://docs.microsoft.com/en-us/dotnet/api/system.datetime) | [PSDateTime](psrpcore.types.PSDateTime) | datetime.datetime | Y |
+| [System.TimeSpan](https://docs.microsoft.com/en-us/dotnet/api/system.timespan) | [PSDuration](psrpcore.types.PSDuration) | str | N |
+| [System.Byte](https://docs.microsoft.com/en-us/dotnet/api/system.byte) | [PSByte](psrpcore.types.PSByte) | int | N |
+| [System.SByte](https://docs.microsoft.com/en-us/dotnet/api/system.sbyte) | [PSSByte](psrpcore.types.PSSByte) | int | N |
+| [System.UInt16](https://docs.microsoft.com/en-us/dotnet/api/system.uint16) | [PSUInt16](psrpcore.types.PSUInt16) | int | N |
+| [System.Int16](https://docs.microsoft.com/en-us/dotnet/api/system.int16) | [PSInt16](psrpcore.types.PSInt16) | int | N |
+| [System.UInt32](https://docs.microsoft.com/en-us/dotnet/api/system.uint32) | [PSUInt](psrpcore.types.PSUInt) | int | N |
+| [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/system.int32) | [PSInt](psrpcore.types.PSInt) | int | Y |
+| [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/system.uint64) | [PSUInt64](psrpcore.types.PSUInt64) | int | N |
+| [System.Int64](https://docs.microsoft.com/en-us/dotnet/api/system.int64) | [PSInt64](psrpcore.types.PSInt64) | int | N |
+| [System.Single](https://docs.microsoft.com/en-us/dotnet/api/system.single) | [PSSingle](psrpcore.types.PSSingle) | float | Y |
+| [System.Double](https://docs.microsoft.com/en-us/dotnet/api/system.double) | [PSDouble](psrpcore.types.PSDouble) | float | N |
+| [System.Decimal](https://docs.microsoft.com/en-us/dotnet/api/system.decimal) | [PSDecimal](psrpcore.types.PSDecimal) | decimal.Decimal | Y |
+| `System.Byte[]` - Array | [PSByteArray](psrpcore.types.PSByteArray) | bytes | Y |
+| [System.Guid](https://docs.microsoft.com/en-us/dotnet/api/system.guid) | [PSGuid](psrpcore.types.PSGuid) | uuid.UUID | Y |
+| [System.Uri](https://docs.microsoft.com/en-us/dotnet/api/system.uri) | [PSUri](psrpcore.types.PSUri) | str | N |
 | `$null` | `PSNull`² | None | Y |
-| [System.Version](https://docs.microsoft.com/en-us/dotnet/api/system.version) | [PSVersion](./source/psrpcore.types.html#psrpcore.types.PSVersion) | N/A | N |
-| [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/system.xml.xmldocument) | [PSXml](./source/psrpcore.types.html#psrpcore.types.PSXml) | str | N |
-| [System.Management.Automation.ScriptBlock](https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.scriptblock) | [PSScriptBlock](./source/psrpcore.types.html#psrpcore.types.PSScriptBlock) | str | N |
-| [System.Security.SecureString](https://docs.microsoft.com/en-us/dotnet/api/system.security.securestring) | [PSSecureString](./source/psrpcore.types.html#psrpcore.types.PSSecureString)³ | N/A | N |
+| [System.Version](https://docs.microsoft.com/en-us/dotnet/api/system.version) | [PSVersion](psrpcore.types.PSVersion) | N/A | N |
+| [System.Xml.XmlDocument](https://docs.microsoft.com/en-us/dotnet/api/system.xml.xmldocument) | [PSXml](psrpcore.types.PSXml) | str | N |
+| [System.Management.Automation.ScriptBlock](https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.scriptblock) | [PSScriptBlock](psrpcore.types.PSScriptBlock) | str | N |
+| [System.Security.SecureString](https://docs.microsoft.com/en-us/dotnet/api/system.security.securestring) | [PSSecureString](psrpcore.types.PSSecureString)³ | N/A | N |
 
 ¹ - While the base Python type is an `int`, doing `PSChar('1')` will get the char based on the string value. Do `PSChar(1)` if you want the `PSChar` to represent `\u0001`
 
 ² - While there is a `psrpcore.types` class for these .NET types, they do not inherit `PSObject` so they cannot handle extended properties
 
 ³ - A `PSSecureString` can be used to encrypt strings that traverse across the wire but the string in Python is not encrypted in memory
 
@@ -188,19 +189,19 @@
 A complex object typically is a class instance that contains both adapted and extended properties.
 They can also include container like object such as a dict, list, stack, queue, etc.
 
 While `psrpcore` supports (de)serialization of effectively any complex object, there are a few important .NET complex types that are good to remember:
 
 | .NET | psrpcore.type | Python Type | Native |
 |-|-|-|-|
-| [System.Collections.ArrayList](https://docs.microsoft.com/en-us/dotnet/api/system.collections.arraylist)¹ | [PSList](./source/psrpcore.types.html#psrpcore.types.PSList) | list | Y |
-| [System.Collections.Hashtable](https://docs.microsoft.com/en-us/dotnet/api/system.collections.hashtable)¹ | [PSDict](./source/psrpcore.types.html#psrpcore.types.PSDict) | dict | Y |
-| [System.Collections.Stack](https://docs.microsoft.com/en-us/dotnet/api/system.collections.stack)¹ | [PSStack](./source/psrpcore.types.html#psrpcore.types.PSStack) | list | N |
-| [System.Collections.Queue](https://docs.microsoft.com/en-us/dotnet/api/system.collections.queue)¹ | [PSQueue](./source/psrpcore.types.html#psrpcore.types.PSQueue) | queue.Queue | Y |
-| [System.Management.Automation.PSCustomObject](https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscustomobject) | [PSCustomObject](./source/psrpcore.types.html#psrpcore.types.PSCustomObject) | type² | Y |
+| [System.Collections.ArrayList](https://docs.microsoft.com/en-us/dotnet/api/system.collections.arraylist)¹ | [PSList](psrpcore.types.PSList) | list | Y |
+| [System.Collections.Hashtable](https://docs.microsoft.com/en-us/dotnet/api/system.collections.hashtable)¹ | [PSDict](psrpcore.types.PSDict) | dict | Y |
+| [System.Collections.Stack](https://docs.microsoft.com/en-us/dotnet/api/system.collections.stack)¹ | [PSStack](psrpcore.types.PSStack) | list | N |
+| [System.Collections.Queue](https://docs.microsoft.com/en-us/dotnet/api/system.collections.queue)¹ | [PSQueue](psrpcore.types.PSQueue) | queue.Queue | Y |
+| [System.Management.Automation.PSCustomObject](https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscustomobject) | [PSCustomObject](psrpcore.types.PSCustomObject) | type² | Y |
 
 ¹ - Other .NET types that are similar to this type are always deserialized to this .NET type, `psrpcore` acts the same, e.g. an` [Object[]]` will become a `PSList`
 
 ² - Unless the Python type hash been marked as a specific .NET type, it will automatically be serialized as a `PSCustomObject`
 
 Like a primitive object, when `Native` is `Y`, those Python types are automatically serialized to the .NET type it represents.
 If you wish to use a specific .NET type that does not natively do this, you need to use the `psrpcore.types.*` class that represents the .NET type you desire or create your own.
@@ -208,16 +209,16 @@
 ### Enum Types
 
 While technically a complex type I consider enums in PSRP to be a separate type of object that straddles both a primitive and complex type.
 Because of its uniqueness they are implemented slightly differently and have a few caveats in Python.
 
 There are 2 base enum types that can be used
 
-* [psrpcore.types.PSEnumBase](./source/psrpcore.types.html#psrpcore.types.PSEnumBase): Inherits `PSObject`, used for enum types that should be set with a single value
-* [psrpcore.types.PSFlagBase](./source/psrpcore.types.html#psrpcore.types.PSFlagBase): Same as `PSEnumBase` but has special behaviour to allow multiple values to be set
+* [psrpcore.types.PSEnumBase](psrpcore.types.PSEnumBase): Inherits `PSObject`, used for enum types that should be set with a single value
+* [psrpcore.types.PSFlagBase](psrpcore.types.PSFlagBase): Same as `PSEnumBase` but has special behaviour to allow multiple values to be set
 
 Like with .NET enums, the enums that inherit `PSEnumBase` or `PSFlagBase` must represent one of the [numeric types](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/integral-numeric-types) like:
 
 * `psrpcore.types.PSByte`
 * `psrpcore.types.PSSByte`
 * `psrpcore.types.PSUInt16`
 * `psrpcore.types.PSInt16`
@@ -285,34 +286,34 @@
 ## Implementing .NET Type in Python
 
 When implementing your own Python class to represent a .NET type there are few things you need to consider/understand:
 
 + The property names of the .NET class must match up with the ones defined on the Python class
 + When an object is serialized, property values are sourced from the property object inside `PSObject`
   + Using a `@property` decorator to generate a calculated property value won't work
-  + The workaround is to use a [PSAliasProperty](./source/psrpcore.types.html#psrpcore.types.PSAliasProperty) or [PSScriptProperty](./source/psrpcore.types.html#psrpcore.types.PSScriptProperty) that is automatically called during the serialization process
+  + The workaround is to use a [PSAliasProperty](psrpcore.types.PSAliasProperty) or [PSScriptProperty](psrpcore.types.PSScriptProperty) that is automatically called during the serialization process
 + Methods defined on the Python class are not transferred to PowerShell, only properties are
 + Whether you want the type to be rehydrated on deserialization or not
 
-All custom .NET types in PowerShell that you implement *SHOULD* inherit from [psrpcore.types.PSObject](./source/psrpcore.types.html#psrpcore.types.PSObject) and use the [psrpcore.types.PSType](./source/psrpcore.types.html#psrpcore.types.PSType) decorator to define the .NET metadata.
+All custom .NET types in PowerShell that you implement *SHOULD* inherit from [psrpcore.types.PSObject](psrpcore.types.PSObject) and use the [psrpcore.types.PSType](psrpcore.types.PSType) decorator to define the .NET metadata.
 Any classes that do not do this will be treated as a `PSCustomObject` which is explained a bit later.
 The `PSType` decorator accepts the following arguments:
 
 + `type_names`: A list of .NET types the object implements, i.e. `['System.String']`
-+ `adapted_properties`: A list of [psrpcore.types.PSPropertyInfo](./source/psrpcore.types.html#psrpcore.types.PSPropertyInfo) instances that define the adapted properties of the object
-+ `extended_properties`: A list of [psrpcore.types.PSPropertyInfo](./source/psrpcore.types.html#psrpcore.types.PSPropertyInfo) instances that define the extended properties of the object
++ `adapted_properties`: A list of [psrpcore.types.PSPropertyInfo](psrpcore.types.PSPropertyInfo) instances that define the adapted properties of the object
++ `extended_properties`: A list of [psrpcore.types.PSPropertyInfo](psrpcore.types.PSPropertyInfo) instances that define the extended properties of the object
 + `skip_inheritance`: Do not inherit the type names and properties of the base class
 + `rehydrate`: Whether this type can be rehydrated (deserialized to this type) or not (default: `True`)
 + `tag`: The CLIXML tag element value to use, this should not be used for end users as all complex types are `Obj`
 
 The type names and properties of the base object will also be inherited onto the defined class.
 For example `PSObject` defines the type names as `["System.Object"]` and thus anything that inherits `PSObject` will have those types appended on it's custom types, e.g. `["System.MyType", "System.Object"]`.
 To skip this behaviour and have a blank starting slate, set `skip_inheritance=True`.
 
-The `adapted_properties` and `extended_properties` kwargs take a list of [PSPropertyInfo](./source/psrpcore.types.html#psrpcore.types.PSPropertyInfo) objects that define the properties of the object itself.
+The `adapted_properties` and `extended_properties` kwargs take a list of [PSPropertyInfo](psrpcore.types.PSPropertyInfo) objects that define the properties of the object itself.
 Once a property has been defined on the object it is immediately gettable/settable like a normal attribute of an instance.
 
 The `rehydrate` kwarg is used during serialization to determine the Python type that is used for the deserialized value.
 If `True` then any .NET objects that implement the same `type_names` will be a Python instance of the actual type.
 If `False` then the returned Python object will be a `psrpcore.types.PSCustomObject` with all the same properties set and the `obj.PSObject.type_names` will have `Deserialized.<type name>` on them.
 The main benefit `rehydrate=True` offers is it allows you do an `isinstance(obj, MyType)` check and call methods defined on that object.
 
@@ -431,15 +432,15 @@
 
 ps_custom_object = MyPSCustomObject('name', 1)
 ```
 
 The first example is a lot simpler and works in a similar way to how `[PSCustomObject]$hash` works but the latter allows you to control more aspect when generating the object such as mandatory arguments, calculated properties, custom methods on the Python side, etc.
 When the serializer detects an object that does not contain any of the .NET type metadata it does the following:
 
-* If it's a known native type like `str`, `int`, it will serialize it as the [primitive type it maps to](#primitive-types)
+* If it's a known native type like `str`, `int`, it will serialize it as the [primitive type it maps to](#types-primitive-types)
 * Otherwise is creates a `PSObject` with it's properties set to all the instances properties and attributes
 
 When it comes to deserializing a `PSCustomObject`, there is no rehydration behaviour. It will always be deserialized as a `psrpcore.types.PSCustomObject`.
 
 
 ## Deserialization Behaviour
 
@@ -452,23 +453,23 @@
   + If the type is not registered, or the init above failed, a blank `PSObject` is created
   + In the latter case the `PSTypeNames` for the next object are prefixed with `Deserialized.<TypeName>`
 + If the CLIXML contains a `<ToString>` value, that is registered to the object's metadata so `str(obj)` outputs that value
 + It will scan all adapted and extended properties in the CLIXML and add them to the value
   + Even if a rehydrated object was used and did not have that property in the class metadata it will still be added to the new instance
   + This also applies to enums and extended primitive objects
 + If the object wraps a dictionary (XML tag == `DCT`)
-  + The value becomes [psrpcore.types.PSDict](./source/psrpcore.types.html#psrpcore.types.PSDict) and is populated with the dict elements
+  + The value becomes [psrpcore.types.PSDict](psrpcore.types.PSDict) and is populated with the dict elements
 + If the object wraps a stack (XML tag == `STK`)
-  + The value becomes [psrpcore.types.PSStack](./source/psrpcore.types.html#psrpcore.types.PSStack) and is populated with the stack elements
+  + The value becomes [psrpcore.types.PSStack](psrpcore.types.PSStack) and is populated with the stack elements
 + If the object wraps a queue (XML tag == `QUE`)
-  + The value becomes [psrpcore.types.PSQueue](./source/psrpcore.types.html#psrpcore.types.PSQueue) and is populated with the queue elements
+  + The value becomes [psrpcore.types.PSQueue](psrpcore.types.PSQueue) and is populated with the queue elements
 + If the object wraps a list (XML tag == `LST`)
-  + The value becomes [psrpcore.types.PSList](./source/psrpcore.types.html#psrpcore.types.PSList) and is populated with the list elements
+  + The value becomes [psrpcore.types.PSList](psrpcore.types.PSList) and is populated with the list elements
 + If the object wraps a IEnumerable (XML tag == `IE`)
-  + The value becomes [psrpcore.types.PSIEnumerable](./source/psrpcore.types.html#psrpcore.types.PSIEnumerable) and is populated with the enumerable elements
+  + The value becomes [psrpcore.types.PSIEnumerable](psrpcore.types.PSIEnumerable) and is populated with the enumerable elements
 + If the object contains a remaining value
   + If the type names match a *registered rehydratable* enum, the enum value is set to this primitive value
   + Else the value now becomes an instance of the primitive value specified instead of a `PSObject`
 
 The end result is:
 
 + Primitive objects are returned as primitive objects with any extra extended properties that may be present
@@ -493,18 +494,18 @@
 ## Add-Member and Update-TypeData
 
 In PowerShell you can add extra properties to an existing object using the [Add-Member](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/add-member?view=powershell-7) cmdlet.
 The [Update-TypeData](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/update-typedata?view=powershell-7) does a similar thing but applies the type information to the type itself rather than a specific object.
 
 You can achieve a similar thing in `psrpcore` by using one of the following methods:
 
-+ [add_member](./source/psrpcore.types.html#psrpcore.types.add_member)
-+ [add_alias_property](./source/psrpcore.types.html#psrpcore.types.add_alias_property)
-+ [add_note_property](./source/psrpcore.types.html#psrpcore.types.add_note_property)
-+ [add_script_property](./source/psrpcore.types.html#psrpcore.types.add_script_property)
++ [add_member](psrpcore.types.add_member)
++ [add_alias_property](psrpcore.types.add_alias_property)
++ [add_note_property](psrpcore.types.add_note_property)
++ [add_script_property](psrpcore.types.add_script_property)
 
 ```python
 import psrpcore.types
 
 
 # The property only applies to the object passed in
 obj = psrpcore.types.PSString("testing")
```

### Comparing `psrpcore-0.2.2/pyproject.toml` & `psrpcore-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 requires = [
     "setuptools >= 61.0.0"  # Support for setuptools config in pyproject.toml
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psrpcore"
-version = "0.2.2"
+version = "0.3.0"
 description = "Core components for the PowerShell Remoting Protocol"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     { name = "Jordan Borean", email = "jborean93@gmail.com" }
 ]
 keywords = ["psrp", "pwsh", "powershell", "remoting"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
     "cryptography",
 ]
 
 [project.urls]
 homepage = "https://github.com/jborean93/psrpcore"
@@ -85,15 +85,15 @@
 [tool.pytest.ini_options]
 testpaths = "tests"
 junit_family = "xunit2"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = sanity,py37,py38,py39,py310,py311
+envlist = sanity,py38,py39,py310,py311,py312
 skip_missing_interpreters = true
 isolated_build = True
 
 [testenv]
 deps =
     -r{toxinidir}/requirements-dev.txt
```

### Comparing `psrpcore-0.2.2/src/psrpcore/__init__.py` & `psrpcore-0.3.0/src/psrpcore/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 
 import psrpcore.types as types
 from psrpcore._client import (
     ClientGetCommandMetadata,
     ClientPowerShell,
     ClientRunspacePool,
 )
+from psrpcore._clixml_shell import ClixmlOutput, ClixmlShell
 from psrpcore._command import Command
+from psrpcore._crypto import PSRemotingCrypto
 from psrpcore._events import (
     ApplicationPrivateDataEvent,
     ConnectRunspacePoolEvent,
     CreatePipelineEvent,
     DebugRecordEvent,
     EncryptedSessionKeyEvent,
     EndOfPipelineInputEvent,
@@ -64,14 +66,16 @@
 
 __all__ = [
     "ApplicationPrivateDataEvent",
     "ClientGetCommandMetadata",
     "ClientHostResponder",
     "ClientPowerShell",
     "ClientRunspacePool",
+    "ClixmlOutput",
+    "ClixmlShell",
     "Command",
     "ConnectRunspacePoolEvent",
     "CreatePipelineEvent",
     "DebugRecordEvent",
     "EncryptedSessionKeyEvent",
     "EndOfPipelineInputEvent",
     "ErrorRecordEvent",
@@ -91,18 +95,17 @@
     "PipelineHostCallEvent",
     "PipelineHostResponseEvent",
     "PipelineInputEvent",
     "PipelineOutputEvent",
     "PipelineStateEvent",
     "PowerShell",
     "ProgressRecordEvent",
-    "ps_data_packet",
-    "ps_guid_packet",
     "PublicKeyEvent",
     "PublicKeyRequestEvent",
+    "PSRemotingCrypto",
     "ResetRunspaceStateEvent",
     "RunspacePoolHostCallEvent",
     "RunspacePoolHostResponseEvent",
     "RunspacePoolInitDataEvent",
     "RunspacePoolStateEvent",
     "ServerHostRequestor",
     "ServerPipeline",
```

### Comparing `psrpcore-0.2.2/src/psrpcore/_base.py` & `psrpcore-0.3.0/src/psrpcore/_base.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/src/psrpcore/_client.py` & `psrpcore-0.3.0/src/psrpcore/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,39 +64,35 @@
 
 class ClientRunspacePool(RunspacePool["_ClientPipeline"]):
     """Client Runspace Pool.
 
     Represents a Runspace Pool on a remote host which can contain one or more
     running pipelines. This is a non blocking connection object that handles
     the incoming and outgoing PSRP packets without worrying about the IO. This
-    model is inspired by `Sans-IO model`_ where this object deals with only
-    the PSRP protocol and needs to be combined with an IO transport separately.
+    model is inspired by `Sans-IO model <https://sans-io.readthedocs.io/>`_
+    where this object deals with only the PSRP protocol and needs to be
+    combined with an IO transport separately.
 
     This is meant to be a close representation of the
-    `System.Management.Automation.Runspaces.RunspacePool`_ .NET class.
+    `System.Management.Automation.Runspaces.RunspacePool <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.runspacepool>`_
+    .NET class.
 
     Args:
         application_arguments: Arguments that are sent to the server and
             accessible through `$PSSenderInfo.ApplicationArguments` of a
             pipeline that runs in this Runspace Pool.
         apartment_state: The apartment state of the thread used to execute
             commands within this Runspace Pool.
         host: The HostInfo that describes the client hosting application.
         thread_options: Determines whether a new thread is created for each
             invocation.
         min_runspaces: The minimum number of Runspaces a pool can hold.
         max_runspaces: The maximum number of Runspaces a pool can hold.
         runspace_pool_id: Manually set the Runspace Pool ID, used when
             reconnecting to an existing Runspace Pool.
-
-    .. _System.Management.Automation.Runspaces.RunspacePool:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.runspacepool
-
-    .. _Sans-IO model:
-        https://sans-io.readthedocs.io/
     """
 
     def __init__(
         self,
         application_arguments: typing.Optional[typing.Dict[str, typing.Any]] = None,
         apartment_state: ApartmentState = ApartmentState.Unknown,
         host: typing.Optional[HostInfo] = None,
```

### Comparing `psrpcore-0.2.2/src/psrpcore/_command.py` & `psrpcore-0.3.0/src/psrpcore/_command.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/src/psrpcore/_crypto.py` & `psrpcore-0.3.0/src/psrpcore/_crypto.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # Copyright: (c) 2021, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
+import base64
 import struct
 import typing
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.hazmat.primitives.padding import PKCS7
@@ -108,37 +109,41 @@
 class PSRemotingCrypto(PSCryptoProvider):
     """PSCryptoProvider used by PSRP for serializing SecureStrings."""
 
     def __init__(self) -> None:
         self._cipher: typing.Optional[Cipher] = None
         self._padding = PKCS7(algorithms.AES.block_size)
 
-    def decrypt(self, value: bytes) -> bytes:
+    def decrypt(self, value: str) -> str:
         if not self._cipher:
             raise MissingCipherError()
 
+        b_enc = base64.b64decode(value)
+
         decryptor = self._cipher.decryptor()
-        b_dec = decryptor.update(value) + decryptor.finalize()
+        b_padded = decryptor.update(b_enc) + decryptor.finalize()
 
         unpadder = self._padding.unpadder()
-        plaintext = unpadder.update(b_dec) + unpadder.finalize()
+        b_dec = unpadder.update(b_padded) + unpadder.finalize()
 
-        return plaintext
+        return b_dec.decode("utf-16-le", errors="surrogatepass")
 
-    def encrypt(self, value: bytes) -> bytes:
+    def encrypt(self, value: str) -> str:
         if not self._cipher:
             raise MissingCipherError()
 
+        b_value = value.encode("utf-16-le", errors="surrogatepass")
+
         padder = self._padding.padder()
-        b_padded = padder.update(value) + padder.finalize()
+        b_padded = padder.update(b_value) + padder.finalize()
 
         encryptor = self._cipher.encryptor()
         b_enc = encryptor.update(b_padded) + encryptor.finalize()
 
-        return b_enc
+        return base64.b64encode(b_enc).decode()
 
     def register_key(
         self,
         key: bytes,
     ) -> None:
         algorithm = algorithms.AES(key)
         mode = modes.CBC(b"\x00" * 16)  # PSRP doesn't use an IV
```

### Comparing `psrpcore-0.2.2/src/psrpcore/_events.py` & `psrpcore-0.3.0/src/psrpcore/_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,14 @@
         return parameters
 
 
 def _unpack_multi_dimensional_array(
     obj: PSObject,
     unpack_obj: typing.Callable[[PSObject], typing.Any],
 ) -> typing.List:
-
     final_list: typing.List[typing.Any] = [unpack_obj(o) for o in obj.mae]
     for count in reversed(obj.mal):
         to_enumerate = final_list
         final_list = []
 
         entries: typing.Any = []
         for entry in to_enumerate:
```

### Comparing `psrpcore-0.2.2/src/psrpcore/_exceptions.py` & `psrpcore-0.3.0/src/psrpcore/_exceptions.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/src/psrpcore/_host.py` & `psrpcore-0.3.0/src/psrpcore/_host.py`

 * *Files 4% similar despite different names*

```diff
@@ -649,162 +649,148 @@
     ) -> int:
         """GetName Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.GetName` host
         call that requests the human friendly host name identifier.
         human friendly host name identifier.
 
-        This corresponds to the `PSHost.Name Property`_.
+        This corresponds to the
+        `PSHost.Name Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.name>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHost.Name Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.name
         """
         return self._connection.host_call(HostMethodIdentifier.GetName)
 
     def get_version(
         self,
     ) -> int:
         """GetVersion Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.GetVersion` host
         call that requests the version of the hosting application.
 
-        This corresponds to the `PSHost.Version Property`_.
+        This corresponds to the
+        `PSHost.Version Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.version>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHost.Version Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.version
         """
         return self._connection.host_call(HostMethodIdentifier.GetVersion)
 
     def get_instance_id(
         self,
     ) -> int:
         """GetInstanceId Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.GetInstanceId`
         host call that requests the identifier of the hosting application.
 
-        This corresponds to the `PSHost.InstanceId Property`_.
+        This corresponds to the
+        `PSHost.InstanceId Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.instanceid>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHost.InstanceId Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.instanceid
         """
         return self._connection.host_call(HostMethodIdentifier.GetInstanceId)
 
     def get_current_culture(
         self,
     ) -> int:
         """GetCurrentCulture Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetCurrentCulture` host
         call that requests the current culture of the host.
 
-        This corresponds to the `PSHost.CurrentCulture Property`_.
+        This corresponds to the
+        `PSHost.CurrentCulture Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.currentculture>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHost.CurrentCulture Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.currentculture
         """
         return self._connection.host_call(HostMethodIdentifier.GetCurrentCulture)
 
     def get_current_ui_culture(
         self,
     ) -> int:
         """GetCurrentUICulture Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetCurrentUICulture` host
         call that requests the current UI culture of the host.
 
-        This corresponds to the `PSHost.CurrentUICulture Property`_.
+        This corresponds to the
+        `PSHost.CurrentUICulture Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.currentuiculture>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHost.CurrentUICulture Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.currentuiculture
         """
         return self._connection.host_call(HostMethodIdentifier.GetCurrentUICulture)
 
     def set_should_exit(
         self,
         exit_code: int,
     ) -> None:
         """SetShouldExit Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetShouldExit` host
         call that requests the current engine runspace to shut down and
         terminate the host's root runspace.
 
-        This corresponds to the `PSHost.SetShouldExit Method`_.
+        This corresponds to the
+        `PSHost.SetShouldExit Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.setshouldexit>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             exit_code: The exit code accompanying the exit keyword.
-
-        .. _PSHost.SetShouldExit Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.setshouldexit
         """
         self._connection.host_call(HostMethodIdentifier.SetShouldExit, [exit_code])
 
     def enter_nested_prompt(
         self,
     ) -> None:
         """EnterNestedPrompt Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.EnterNestedPrompt` host
         call that instructs the host to interrupt the currently running
         pipeline and start a new, "nested" input loop, where an input loop is
         the cycle of prompt, input, execute.
 
-        This corresponds to the `PSHost.EnterNestedPrompt Method`_.
+        This corresponds to the
+        `PSHost.EnterNestedPrompt Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.enternestedprompt>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
-
-        .. _PSHost.EnterNestedPrompt Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.enternestedprompt
         """
         self._connection.host_call(HostMethodIdentifier.EnterNestedPrompt)
 
     def exit_nested_prompt(
         self,
     ) -> None:
         """ExitNestedPrompt Request.
@@ -813,22 +799,20 @@
         :class:`psrpcore.types.HostMethodIdentifier.ExitNestedPrompt` host
         call that causes the host to end the currently running input loop. If
         the input loop was created by a prior call to EnterNestedPrompt, the
         enclosing pipeline will be resumed. If the current input loop is the
         top-most loop, then the host will act as though
         :meth:`set_should_exit()` was called.
 
-        This corresponds to the `PSHost.ExitNestedPrompt Method`_.
+        This corresponds to the
+        `PSHost.ExitNestedPrompt Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.exitnestedprompt>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
-
-        .. _PSHost.ExitNestedPrompt Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.exitnestedprompt
         """
         self._connection.host_call(HostMethodIdentifier.ExitNestedPrompt)
 
     def notify_begin_application(
         self,
     ) -> None:
         """NotifyBeginApplication Request.
@@ -843,22 +827,20 @@
             * reads from stdin
             * writes to stdout
             * writes to stderr
 
         The engine will always call this method and
         :meth:`notify_end_application()` in pairs.
 
-        This corresponds to the `PSHost.NotifyBeginApplication Method`_.
+        This corresponds to the
+        `PSHost.NotifyBeginApplication Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.notifybeginapplication>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
-
-        .. _PSHost.NotifyBeginApplication Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.notifybeginapplication
         """
         self._connection.host_call(HostMethodIdentifier.NotifyBeginApplication)
 
     def notify_end_application(
         self,
     ) -> None:
         """NotifyEndApplication Request.
@@ -867,22 +849,20 @@
         :class:`psrpcore.types.HostMethodIdentifier.NotifyEndApplication`
         host call that is called by the engine to notify the host that the
         execution of a legacy command has completed.
 
         The engine will always call this method and
         :meth:`notify_begin_application()` in pairs.
 
-        This corresponds to the `PSHost.NotifyEndApplication Method`_.
+        This corresponds to the
+        `PSHost.NotifyEndApplication Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.notifyendapplication>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
-
-        .. _PSHost.NotifyEndApplication Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshost.notifyendapplication
         """
         self._connection.host_call(HostMethodIdentifier.NotifyEndApplication)
 
     # I don't think this is actually possible to do.
     # def push_runspace(self, runspace) -> None:
     #     self._connection.host_call(HostMethodIdentifier.PushRunspace, [runspace])
 
@@ -891,45 +871,41 @@
     ) -> None:
         """PopRunspace Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.PopRunspace` host
         call that is called by the engine to notify the host that a Runspace
         pop has been requested.
 
-        This corresponds to the `IHostSupportsInteractiveSession.PopRunspace Method`_.
+        This corresponds to the
+        `IHostSupportsInteractiveSession.PopRunspace Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.ihostsupportsinteractivesession.poprunspace>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
-
-        .. _IHostSupportsInteractiveSession.PopRunspace Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.ihostsupportsinteractivesession.poprunspace
         """
         self._connection.host_call(HostMethodIdentifier.PopRunspace)
 
     def get_is_runspace_pushed(
         self,
     ) -> int:
         """GetIsRunspacePushed Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetIsRunspacePushed` host
         call to check if the runspace is pushed or not.
 
-        This corresponds to the `IHostSupportsInteractiveSession.IsRunspacePushed Property`_.
+        This corresponds to the
+        `IHostSupportsInteractiveSession.IsRunspacePushed Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.ihostsupportsinteractivesession.isrunspacepushed>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _IHostSupportsInteractiveSession.IsRunspacePushed Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.ihostsupportsinteractivesession.isrunspacepushed
         """
         return self._connection.host_call(HostMethodIdentifier.GetIsRunspacePushed)
 
     # Also don't think this is possible remotely.
     # def get_runspace(self) -> int:
     #     return self._connection.host_call(HostMethodIdentifier.GetRunspace, [])
 
@@ -938,48 +914,44 @@
     ) -> int:
         """ReadLine Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.ReadLine` host
         call to read characters from the console until a newline is
         encountered.
 
-        This corresponds to the `PSHostUserInterface.ReadLine Method`_.
+        This corresponds to the
+        `PSHostUserInterface.ReadLine Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.readline>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostUserInterface.ReadLine Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.readline
         """
         return self._connection.host_call(HostMethodIdentifier.ReadLine)
 
     def read_line_as_secure_string(
         self,
     ) -> int:
         """ReadLineAsSecureString Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.ReadLineAsSecureString` host
         call to read characters from the console until a newline is
         encountered without echoing the input back to the user.
 
-        This corresponds to the `PSHostUserInterface.ReadLineAsSecureString Method`_.
+        This corresponds to the
+        `PSHostUserInterface.ReadLineAsSecureString Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.readlineassecurestring>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostUserInterface.ReadLineAsSecureString Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.readlineassecurestring
         """
         return self._connection.host_call(HostMethodIdentifier.ReadLineAsSecureString)
 
     def write(
         self,
         value: str,
         foreground_color: typing.Optional[ConsoleColor] = None,
@@ -987,27 +959,25 @@
     ) -> None:
         """Write Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.Write1` or
         :class:`psrpcore.types.HostMethodIdentifier.Write2` host call that
         writes the characters to the screen buffer.
 
-        This corresponds to the `PSHostUserInterface.Write Method`_.
+        This corresponds to the
+        `PSHostUserInterface.Write Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.write>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             value: The characters to write.
             foreground_color: The color to display the text with.
             background_color: The color to display the background with.
-
-        .. _PSHostUserInterface.Write Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.write
         """
         mi = HostMethodIdentifier.Write1
         mp: typing.List[typing.Union[str, int]] = [value]
 
         if not (foreground_color is None and background_color is None):
             mi = HostMethodIdentifier.Write2
             mp.insert(0, foreground_color.value if foreground_color is not None else 0)
@@ -1024,27 +994,25 @@
         """WriteLine Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.WriteLine1`,
         :class:`psrpcore.types.HostMethodIdentifier.WriteLine2`, or
         :class:`psrpcore.types.HostMethodIdentifier.WriteLine2` host call that
         writes the characters with a newline to the screen buffer.
 
-        This corresponds to the `PSHostUserInterface.WriteLine Method`_.
+        This corresponds to the
+        `PSHostUserInterface.WriteLine Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeline>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             line: The line to write, if not set then just a newline is written.
             foreground_color: The color to display the line with.
             background_color: The color to display the background with.
-
-        .. _PSHostUserInterface.WriteLine Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeline
         """
         mi = HostMethodIdentifier.WriteLine1
         mp: typing.List[typing.Union[str, int]] = []
 
         if line is not None:
             mi = HostMethodIdentifier.WriteLine2
             mp.append(line)
@@ -1064,48 +1032,44 @@
         line: str,
     ) -> None:
         """WriteErrorLine Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.WriteErrorLine`
         host call that writes the line to the error display of the host.
 
-        This corresponds to the `PSHostUserInterface.WriteErrorLine Method`_.
+        This corresponds to the
+        `PSHostUserInterface.WriteErrorLine Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeerrorline>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             line: The line to write to the error display.
-
-        .. _PSHostUserInterface.WriteErrorLine Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeerrorline
         """
         self._connection.host_call(HostMethodIdentifier.WriteErrorLine, [line])
 
     def write_debug_line(
         self,
         line: str,
     ) -> None:
         """WriteDebugLine Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.WriteDebugLine`
         host call that writes a debugging message to the host.
 
-        This corresponds to the `PSHostUserInterface.WriteDebugLine Method`_.
+        This corresponds to the
+        `PSHostUserInterface.WriteDebugLine Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writedebugline>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             line: The debug line to write to the display.
-
-        .. _PSHostUserInterface.WriteDebugLine Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writedebugline
         """
         self._connection.host_call(HostMethodIdentifier.WriteDebugLine, [line])
 
     def write_progress(
         self,
         source_id: int,
         activity_id: int,
@@ -1118,15 +1082,16 @@
         seconds_remaining: int = -1,
     ) -> None:
         """WriteProgress Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.WriteProgress`
         host call that writes a progress record to be displayed on the host.
 
-        This corresponds to the `PSHostUserInterface.WriteProgress Method`_.
+        This corresponds to the
+        `PSHostUserInterface.WriteProgress Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeprogress>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             source_id: Unique identifier of the source of the record.
@@ -1144,17 +1109,14 @@
             percent_complete: The estimate of the percentage of total work for
                 the activity that is completed. Set to a negative value to
                 indicate that the percentage completed should not be displayed.
             record_type: The type of record represented.
             seconds_remaining: The estimate of time remaining until this
                 activity is completed. Set to a negative value to indicate that
                 the seconds remaining should not be displayed.
-
-        .. _PSHostUserInterface.WriteProgress Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeprogress
         """
         # ProgressRecord serialized here is like a PSRP ProgressRecordMsg object.
         self._connection.host_call(
             HostMethodIdentifier.WriteProgress,
             [
                 source_id,
                 ProgressRecordMsg(
@@ -1175,48 +1137,44 @@
         line: str,
     ) -> None:
         """WriteVerboseLine Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.WriteVerboseLine`
         host call that writes a verbose message to the host.
 
-        This corresponds to the `PSHostUserInterface.WriteVerboseLine Method`_.
+        This corresponds to the
+        `PSHostUserInterface.WriteVerboseLine Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeverboseline>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             line: The verbose line to write to the display.
-
-        .. _PSHostUserInterface.WriteVerboseLine Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writeverboseline
         """
         self._connection.host_call(HostMethodIdentifier.WriteVerboseLine, [line])
 
     def write_warning_line(
         self,
         line: str,
     ) -> None:
         """WriteWarningLine Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.WriteWarningLine`
         host call that writes a warning message to the host.
 
-        This corresponds to the `PSHostUserInterface.WriteWarningLine Method`_.
+        This corresponds to the
+        `PSHostUserInterface.WriteWarningLine Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writewarningline>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             line: The warning line to write to the display.
-
-        .. _PSHostUserInterface.WriteWarningLine Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.writewarningline
         """
         self._connection.host_call(HostMethodIdentifier.WriteWarningLine, [line])
 
     def prompt(
         self,
         caption: str,
         message: str,
@@ -1224,30 +1182,28 @@
     ) -> int:
         """Prompt Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.Prompt`
         host call prompts the user with a number of fields for which to supply
         values.
 
-        This corresponds to the `PSHostUserInterface.Prompt Method`_.
+        This corresponds to the
+        `PSHostUserInterface.Prompt Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.prompt>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Args:
             caption: The caption or title for the prompt.
             message: The message describing the set of fields.
             descriptions: A list of fields to display.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostUserInterface.Prompt Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.prompt
         """
         fields = [FieldDescription.ToPSObjectForRemoting(f, for_host=True) for f in descriptions]
 
         return self._connection.host_call(HostMethodIdentifier.Prompt, [caption, message, fields])
 
     def prompt_for_credential(
         self,
@@ -1261,15 +1217,16 @@
         """PromptForCredential Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.PromptForCredential1`, or
         :class:`psrpcore.types.HostMethodIdentifier.PromptForCredential2` host
         call prompts the user for a credential.
 
-        This corresponds to the `PSHostUserInterface.PromptForCredential Method`_.
+        This corresponds to the
+        `PSHostUserInterface.PromptForCredential Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.promptforcredential>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Args:
             caption: The caption or title for the prompt.
@@ -1279,17 +1236,14 @@
             target_name: The domain part of the username if set.
             allowed_credential_types: The types of credential that is being
                 requested.
             options: Options to control the UI behaviour.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostUserInterface.PromptForCredential Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.promptforcredential
         """
         mi = HostMethodIdentifier.PromptForCredential1
         mp: typing.List[typing.Any] = [caption, message, username, target_name or ""]
         if not (allowed_credential_types is None and options is None):
             mi = HostMethodIdentifier.PromptForCredential2
             mp.append(
                 PSCredentialTypes.Default.value if allowed_credential_types is None else allowed_credential_types.value
@@ -1306,15 +1260,16 @@
         default_choice: int = -1,
     ) -> int:
         """PromptForChoice Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.PromptForChoice`
         host call prompts the user to choose an option from a set list.
 
-        This corresponds to the `PSHostUserInterface.PromptForChoice Method`_.
+        This corresponds to the
+        `PSHostUserInterface.PromptForChoice Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.promptforchoice>`_.
         See :meth:`prompt_for_multiple_choice()` for a way to allow the user to
         select multiple choices.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
@@ -1323,17 +1278,14 @@
             message: The message describing the set of choices.
             choices: A list of choices.
             default_choice: The default choice that correspond to the index of
                 choices, ``-1`` means no default.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostUserInterface.PromptForChoice Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostuserinterface.promptforchoice
         """
         converted_choices = [ChoiceDescription.ToPSObjectForRemoting(c, for_host=True) for c in choices]
 
         return self._connection.host_call(
             HostMethodIdentifier.PromptForChoice, [caption, message, converted_choices, default_choice]
         )
 
@@ -1347,32 +1299,29 @@
         """PromptForChoiceMultipleSelection Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.PromptForChoiceMultipleSelection`
         host call prompts the user to choose multiple options from a set list.
 
         This corresponds to the
-        `IHostUISupportsMultipleChoiceSelection.PromptForChoice Method`_.
+        `IHostUISupportsMultipleChoiceSelection.PromptForChoice Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.ihostuisupportsmultiplechoiceselection.promptforchoice>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Args:
             caption: The caption or title for the prompt.
             message: The message describing the set of choices.
             choices: A list of choices.
             default_choices: A list of default choice that correspond to the index of
                 choices.
 
         Returns:
             int: The call id for the request.
-
-        .. _IHostUISupportsMultipleChoiceSelection.PromptForChoice Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.ihostuisupportsmultiplechoiceselection.promptforchoice
         """
         converted_choices = [ChoiceDescription.ToPSObjectForRemoting(c, for_host=True) for c in choices]
 
         return self._connection.host_call(
             HostMethodIdentifier.PromptForChoiceMultipleSelection,
             [caption, message, converted_choices, default_choices or []],
         )
@@ -1383,123 +1332,108 @@
         """GetForegroundColor Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetForegroundColor` host
         call to request the foreground color of the host.
 
         This corresponds to the
-        `PSHostRawUserInterface.ForegroundColor Property`_.
+        `PSHostRawUserInterface.ForegroundColor Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.foregroundcolor>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.ForegroundColor Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.foregroundcolor
         """
         return self._connection.host_call(HostMethodIdentifier.GetForegroundColor)
 
     def set_foreground_color(
         self,
         color: ConsoleColor,
     ) -> None:
         """SetForegroundColor Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetForegroundColor` host
         call to change the foreground color of the host.
 
         This corresponds to the
-        `PSHostRawUserInterface.ForegroundColor Property`_.
+        `PSHostRawUserInterface.ForegroundColor Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.foregroundcolor>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             color: The color to set the foreground color to.
-
-        .. _PSHostRawUserInterface.ForegroundColor Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.foregroundcolor
         """
         self._connection.host_call(HostMethodIdentifier.SetForegroundColor, [color.value])
 
     def get_background_color(
         self,
     ) -> int:
         """GetBackgroundColor Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetBackgroundColor` host
         call to request the background color of the host.
 
         This corresponds to the
-        `PSHostRawUserInterface.BackgroundColor Property`_.
+        `PSHostRawUserInterface.BackgroundColor Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.backgroundcolor>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.BackgroundColor Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.backgroundcolor
         """
         return self._connection.host_call(HostMethodIdentifier.GetBackgroundColor)
 
     def set_background_color(
         self,
         color: ConsoleColor,
     ) -> None:
         """SetBackgroundColor Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetBackgroundColor` host
         call to change the background color of the host.
 
         This corresponds to the
-        `PSHostRawUserInterface.BackgroundColor Property`_.
+        `PSHostRawUserInterface.BackgroundColor Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.backgroundcolor>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             color: The color to set the background color to.
-
-        .. _PSHostRawUserInterface.BackgroundColor Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.backgroundcolor
         """
         self._connection.host_call(HostMethodIdentifier.SetBackgroundColor, [color.value])
 
     def get_cursor_position(
         self,
     ) -> int:
         """GetCursorPosition Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetCursorPosition` host
         call to get the position of the cursor on the screen buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.CursorPosition Property`_.
+        `PSHostRawUserInterface.CursorPosition Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorposition>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.CursorPosition Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorposition
         """
         return self._connection.host_call(HostMethodIdentifier.GetCursorPosition)
 
     def set_cursor_position(
         self,
         x: int,
         y: int,
@@ -1507,26 +1441,23 @@
         """SetCursorPosition Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetCursorPosition` host
         call to change the position of the cursor on the screen buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.CursorPosition Property`_.
+        `PSHostRawUserInterface.CursorPosition Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorposition>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             x: The horizontal location to set the cursor to.
             y: The vertical location to set the cursor to.
-
-        .. _PSHostRawUserInterface.CursorPosition Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorposition
         """
         self._connection.host_call(
             HostMethodIdentifier.SetCursorPosition,
             [Coordinates.ToPSObjectForRemoting(Coordinates(x, y), for_host=True)],
         )
 
     def get_window_position(
@@ -1536,25 +1467,22 @@
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetWindowPosition` host
         call to get the position of the view window relative to the screen
         buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.WindowPosition Property`_.
+        `PSHostRawUserInterface.WindowPosition Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowposition>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.WindowPosition Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowposition
         """
         return self._connection.host_call(HostMethodIdentifier.GetWindowPosition)
 
     def set_window_position(
         self,
         x: int,
         y: int,
@@ -1563,26 +1491,23 @@
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetWindowPosition` host
         call to change the position of the view window relative to the screen
         buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.WindowPosition Property`_.
+        `PSHostRawUserInterface.WindowPosition Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowposition>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             x: The horizontal location to set the window to.
             y: The vertical location to set the window to.
-
-        .. _PSHostRawUserInterface.WindowPosition Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowposition
         """
         self._connection.host_call(
             HostMethodIdentifier.SetWindowPosition,
             [Coordinates.ToPSObjectForRemoting(Coordinates(x, y), for_host=True)],
         )
 
     def get_cursor_size(
@@ -1591,74 +1516,65 @@
         """GetCursorSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetCursorSize` host
         call to get the size of the cursor as a percentage.
 
         This corresponds to the
-        `PSHostRawUserInterface.CursorSize Property`_.
+        `PSHostRawUserInterface.CursorSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorsize>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.CursorSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorsize
         """
         return self._connection.host_call(HostMethodIdentifier.GetCursorSize)
 
     def set_cursor_size(
         self,
         size: int,
     ) -> None:
         """SetCursorSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetCursorSize` host
         call to set the size of the cursor as a percentage.
 
         This corresponds to the
-        `PSHostRawUserInterface.CursorSize Property`_.
+        `PSHostRawUserInterface.CursorSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorsize>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             size: The cursor size as a percentage.
-
-        .. _PSHostRawUserInterface.CursorSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.cursorsize
         """
         self._connection.host_call(HostMethodIdentifier.SetCursorSize, [size])
 
     def get_buffer_size(
         self,
     ) -> int:
         """GetBufferSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetBufferSize` host
         call to get the size of the screen buffer as measured by cells.
 
         This corresponds to the
-        `PSHostRawUserInterface.BufferSize Property`_.
+        `PSHostRawUserInterface.BufferSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.buffersize>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.BufferSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.buffersize
         """
         return self._connection.host_call(HostMethodIdentifier.GetBufferSize)
 
     def set_buffer_size(
         self,
         width: int,
         height: int,
@@ -1666,26 +1582,23 @@
         """SetBufferSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetBufferSize` host
         call to change the size of the screen buffer as measured by cells.
 
         This corresponds to the
-        `PSHostRawUserInterface.BufferSize Property`_.
+        `PSHostRawUserInterface.BufferSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.buffersize>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             width: The number of cells in the buffer width.
             height: The number of cells in the buffer height.
-
-        .. _PSHostRawUserInterface.BufferSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.buffersize
         """
         self._connection.host_call(
             HostMethodIdentifier.SetBufferSize, [Size.ToPSObjectForRemoting(Size(width, height), for_host=True)]
         )
 
     def get_window_size(
         self,
@@ -1693,25 +1606,22 @@
         """GetWindowSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetWindowSize` host
         call to get the size of the view window as measured by cells.
 
         This corresponds to the
-        `PSHostRawUserInterface.WindowSize Property`_.
+        `PSHostRawUserInterface.WindowSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowsize>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.WindowSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowsize
         """
         return self._connection.host_call(HostMethodIdentifier.GetWindowSize)
 
     def set_window_size(
         self,
         width: int,
         height: int,
@@ -1719,26 +1629,23 @@
         """SetWindowSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetWindowSize` host
         call to change the size of the view window size as measured by cells.
 
         This corresponds to the
-        `PSHostRawUserInterface.WindowSize Property`_.
+        `PSHostRawUserInterface.WindowSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowsize>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             width: The number of cells in the view window width.
             height: The number of cells in the view window height.
-
-        .. _PSHostRawUserInterface.WindowSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowsize
         """
         self._connection.host_call(
             HostMethodIdentifier.SetWindowSize, [Size.ToPSObjectForRemoting(Size(width, height), for_host=True)]
         )
 
     def get_window_title(
         self,
@@ -1746,171 +1653,150 @@
         """GetWindowTitle Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetWindowTitle` host
         call to get the window title.
 
         This corresponds to the
-        `PSHostRawUserInterface.WindowTitle Property`_.
+        `PSHostRawUserInterface.WindowTitle Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowtitle>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.WindowTitle Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowtitle
         """
         return self._connection.host_call(HostMethodIdentifier.GetWindowTitle)
 
     def set_window_title(
         self,
         title: str,
     ) -> None:
         """SetWindowTitle Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetWindowTitle` host
         call to change the title of the host window
 
         This corresponds to the
-        `PSHostRawUserInterface.WindowTitle Property`_.
+        `PSHostRawUserInterface.WindowTitle Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowtitle>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             title: The title to set the host window to.
-
-        .. _PSHostRawUserInterface.WindowTitle Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.windowtitle
         """
         self._connection.host_call(HostMethodIdentifier.SetWindowTitle, [title])
 
     def get_max_window_size(
         self,
     ) -> int:
         """GetMaxWindowSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetMaxWindowSize` host
         call to get largest possible window size that can fit in the current
         buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.MaxWindowSize Property`_.
+        `PSHostRawUserInterface.MaxWindowSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.maxwindowsize>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.MaxWindowSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.maxwindowsize
         """
         return self._connection.host_call(HostMethodIdentifier.GetMaxWindowSize)
 
     def get_max_physical_window_size(
         self,
     ) -> int:
         """GetMaxPhysicalWindowSize Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetMaxPhysicalWindowSize`
         host call to get largest possible window size that can be set.
 
         This corresponds to the
-        `PSHostRawUserInterface.MaxPhysicalWindowSize Property`_.
+        `PSHostRawUserInterface.MaxPhysicalWindowSize Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.maxphysicalwindowsize>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.MaxPhysicalWindowSize Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.maxphysicalwindowsize
         """
         return self._connection.host_call(HostMethodIdentifier.GetMaxPhysicalWindowSize)
 
     def get_key_available(
         self,
     ) -> int:
         """GetKeyAvailable Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetKeyAvailable` host
         call to examine if a keystroke is waiting in the input buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.KeyAvailable Property`_.
+        `PSHostRawUserInterface.KeyAvailable Property <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.keyavailable>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.KeyAvailable Property:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.keyavailable
         """
         return self._connection.host_call(HostMethodIdentifier.GetKeyAvailable)
 
     def read_key(
         self,
         options: ReadKeyOptions = ReadKeyOptions.IncludeKeyDown,
     ) -> int:
         """ReadKey Request.
 
         Sends the :class:`psrpcore.types.HostMethodIdentifier.ReadKey` host
         call to request read a key stroke.
 
         This corresponds to the
-        `PSHostRawUserInterface.ReadKey Method`_.
+        `PSHostRawUserInterface.ReadKey Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.readkey>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Args:
             options: Further options to control the read key operation.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.ReadKey Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.readkey
         """
         return self._connection.host_call(HostMethodIdentifier.ReadKey, [options.value])
 
     def flush_input_buffer(
         self,
     ) -> None:
         """FlushInputBuffer Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.FlushInputBuffer` host
         call to reset the keyboard input buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.FlushInputBuffer Method`_.
+        `PSHostRawUserInterface.FlushInputBuffer Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.flushinputbuffer>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
-
-        .. _PSHostRawUserInterface.FlushInputBuffer Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.flushinputbuffer
         """
         self._connection.host_call(HostMethodIdentifier.FlushInputBuffer)
 
     def set_buffer_cells(
         self,
         left: int,
         top: int,
@@ -1923,17 +1809,17 @@
         """SetBufferContents Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.SetBufferContents1` host
         call to set the contents of the host buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.SetBufferContents Method`_. See
-        :meth:`set_buffer_contents()` to set the buffer contents by individual
-        cells.
+        `PSHostRawUserInterface.SetBufferContents Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.setbuffercontents>`_.
+        See :meth:`set_buffer_contents()` to set the buffer contents by
+        individual cells.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             left: The left margin of the region to set the cell to.
@@ -1942,17 +1828,14 @@
             bottom: The bottom margin of the region to set the cell to.
             character: The character used to fill the cells in the region
                 specified.
             foreground: The foreground (text) color to fill the cells in the
                 region specified.
             background: The background color to fill the cells in the region
                 specified.
-
-        .. _PSHostRawUserInterface.SetBufferContents Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.setbuffercontents
         """
         rectangle = Rectangle.ToPSObjectForRemoting(Rectangle(left, top, right, bottom), for_host=True)
         cell = BufferCell.ToPSObjectForRemoting(
             BufferCell(character, foreground, background, BufferCellType.Complete), for_host=True
         )
         self._connection.host_call(HostMethodIdentifier.SetBufferContents1, [rectangle, cell])
 
@@ -1969,30 +1852,28 @@
         call to set the contents of the host buffer.
 
         The ``contents`` value is a list of a list of
         :class:`psrpcore.types.BufferCell` where the first list dimension
         represents each row and the 2nd dimension is each column of that row.
 
         This corresponds to the
-        `PSHostRawUserInterface.SetBufferContents Method`_. See
-        :meth:`set_buffer_cells()` to set an individual cell across a region.
+        `PSHostRawUserInterface.SetBufferContents Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.setbuffercontents>`_.
+        See :meth:`set_buffer_cells()` to set an individual cell across a
+        region.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             x: The horizontal location of the upper left corner of the region
                 to write the cells from.
             y: The vertical location of the upper left corner of the region to
                 write the cells from.
             contents: A list of a list of cells that should be written.
-
-        .. _PSHostRawUserInterface.SetBufferContents Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.setbuffercontents
         """
         coordinates = Coordinates.ToPSObjectForRemoting(Coordinates(x, y), for_host=True)
         wrap_cell = functools.partial(BufferCell.ToPSObjectForRemoting, for_host=True)
         host_contents = _create_multi_dimensional_array(contents, wrap_cell)
         self._connection.host_call(HostMethodIdentifier.SetBufferContents2, [coordinates, host_contents])
 
     def get_buffer_contents(
@@ -2005,15 +1886,15 @@
         """GetBufferContents Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.GetBufferContents` host
         call to request the contents of the screen region specified.
 
         This corresponds to the
-        `PSHostRawUserInterface.GetBufferContents Method`_.
+        `PSHostRawUserInterface.GetBufferContents Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.getbuffercontents>`_.
 
         Note:
             The server should wait for the host response before continuing the
             pipeline that created this request.
 
         Note:
             PowerShell does not implement this call for security reasons.
@@ -2024,17 +1905,14 @@
             left: The left margin of the buffer region.
             top: The top margin of the buffer region.
             right: The right margin of the buffer region.
             bottom: The bottom margin of the buffer region.
 
         Returns:
             int: The call id for the request.
-
-        .. _PSHostRawUserInterface.GetBufferContents Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.getbuffercontents
         """
         return self._connection.host_call(
             HostMethodIdentifier.GetBufferContents,
             [
                 Rectangle.ToPSObjectForRemoting(Rectangle(left, top, right, bottom), for_host=True),
             ],
         )
@@ -2058,15 +1936,15 @@
         """ScrollBufferContents Request.
 
         Sends the
         :class:`psrpcore.types.HostMethodIdentifier.ScrollBufferContents` host
         call to scoll a region of the screen buffer.
 
         This corresponds to the
-        `PSHostRawUserInterface.ScrollBufferContents Method`_.
+        `PSHostRawUserInterface.ScrollBufferContents Method <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.scrollbuffercontents>`_.
 
         Note:
             This is a void method and the server should continue pipeline
             execution and expect no response from the client.
 
         Args:
             source_left: The left margin of the screen to be scrolled.
@@ -2083,17 +1961,14 @@
             clip_bottom: The bottom margin of the clipped region.
             character: The character used to fill the cells intersecting the
                 source and clip region.
             foreground: The foreground (text) color to fill the cells
                 intersecting the source and clip region.
             background: The background color to fill the cells intersecting
                 the source and clip region.
-
-        .. _PSHostRawUserInterface.ScrollBufferContents Method:
-            https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.pshostrawuserinterface.scrollbuffercontents
         """
         source = Rectangle.ToPSObjectForRemoting(
             Rectangle(source_left, source_top, source_right, source_bottom), for_host=True
         )
         dest = Coordinates.ToPSObjectForRemoting(Coordinates(x, y), for_host=True)
         clip = Rectangle.ToPSObjectForRemoting(Rectangle(clip_left, clip_top, clip_right, clip_bottom), for_host=True)
         fill = BufferCell.ToPSObjectForRemoting(
```

### Comparing `psrpcore-0.2.2/src/psrpcore/_payload.py` & `psrpcore-0.3.0/src/psrpcore/_payload.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/src/psrpcore/_pipeline.py` & `psrpcore-0.3.0/src/psrpcore/_pipeline.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/src/psrpcore/_server.py` & `psrpcore-0.3.0/src/psrpcore/_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 # Copyright: (c) 2021, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 import base64
 import datetime
-import getpass
 import os
 import platform
-import threading
 import typing
 import uuid
 
 from psrpcore._base import Pipeline, RunspacePool
 from psrpcore._crypto import encrypt_session_key
 from psrpcore._events import (
     ConnectRunspacePoolEvent,
@@ -41,14 +39,15 @@
     DebugRecord,
     EncryptedSessionKey,
     ErrorCategory,
     ErrorCategoryInfo,
     ErrorDetails,
     ErrorRecord,
     HostMethodIdentifier,
+    InformationRecord,
     InformationRecordMsg,
     InvocationInfo,
     NETException,
     PipelineHostCall,
     PipelineState,
     ProgressRecordMsg,
     ProgressRecordType,
@@ -734,42 +733,35 @@
         required_version = ProtocolVersion.Pwsh5.value
         if their_version < required_version:
             raise InvalidProtocolVersion("writing information record", their_version, required_version)
 
         if self.state != PSInvocationState.Running:
             raise InvalidPipelineState("write pipeline information", self.state, [PSInvocationState.Running])
 
-        time_generated = PSDateTime.now() if time_generated is None else time_generated
-        if not tags:
-            tags = []
-
-        if user is None:
-            try:
-                # getuser on Windows relies on env vars that may not may not be set. Just fallback gracefully.
-                user = getpass.getuser()
-
-            except ModuleNotFoundError:  # pragma: no cover
-                user = "Unknown"
-
-        computer = platform.node() if computer is None else computer
-        process_id = os.getpid() if process_id is None else process_id
-
-        # get_native_id isn't available until 3.8, default to 0.
-        native_thread_id = getattr(threading, "get_native_id", lambda: 0)()
-
+        record = InformationRecord.create(
+            message_data=message_data,
+            source=source,
+            time_generated=time_generated,
+            tags=tags,
+            user=user,
+            computer=computer,
+            process_id=process_id,
+            native_thread_id=native_thread_id,
+            managed_thread_id=managed_thread_id,
+        )
         value = InformationRecordMsg(
-            MessageData=message_data,
-            Source=source,
-            TimeGenerated=time_generated,
-            Tags=tags,
-            User=user,
-            Computer=computer,
-            ProcessId=process_id or 0,
-            NativeThreadId=native_thread_id or 0,
-            ManagedThreadId=managed_thread_id or 0,
+            MessageData=record.MessageData,
+            Source=record.Source,
+            TimeGenerated=record.TimeGenerated,
+            Tags=record.Tags,
+            User=record.User,
+            Computer=record.Computer,
+            ProcessId=record.ProcessId,
+            NativeThreadId=record.NativeThreadId,
+            ManagedThreadId=record.ManagedThreadId,
         )
         self.prepare_message(value, message_type=PSRPMessageType.InformationRecord)
 
     def _change_state(
         self,
         state: PSInvocationState,
         error: typing.Optional[ErrorRecord] = None,
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/__init__.py` & `psrpcore-0.3.0/src/psrpcore/types/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -140,24 +140,31 @@
     SessionCapability,
     SetMaxRunspaces,
     SetMinRunspaces,
     UserEvent,
     VerboseRecordMsg,
     WarningRecordMsg,
 )
-from psrpcore.types._serializer import deserialize, serialize
+from psrpcore.types._serializer import (
+    ClixmlStream,
+    deserialize,
+    deserialize_clixml,
+    serialize,
+    serialize_clixml,
+)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __all__ = [
     "ApartmentState",
     "ApplicationPrivateData",
     "BufferCell",
     "BufferCellType",
     "ChoiceDescription",
+    "ClixmlStream",
     "CommandMetadataCount",
     "CommandOrigin",
     "CommandTypes",
     "ConnectRunspacePool",
     "ConsoleColor",
     "ControlKeyStates",
     "Coordinates",
@@ -268,10 +275,12 @@
     "WarningRecord",
     "WarningRecordMsg",
     "add_alias_property",
     "add_member",
     "add_note_property",
     "add_script_property",
     "deserialize",
+    "deserialize_clixml",
     "ps_isinstance",
     "serialize",
+    "serialize_clixml",
 ]
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_base.py` & `psrpcore-0.3.0/src/psrpcore/types/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -420,35 +420,33 @@
 
 
 class PSAliasProperty(PSPropertyInfo):
     """Alias Property
 
     This is a property that gets a value based on another property or attribute
     of the PSObject. It is designed to replicate the functionality of
-    `PSAliasProperty`_. During serialization the alias property will just copy
-    the value of the target it is pointing to. You cannot set a value to an
-    alias property, see :class:`PSScriptProperty` which allows the caller
-    to define a way to get and set properties on an object dynamically.
+    `PSAliasProperty <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psaliasproperty>`_.
+    During serialization the alias property will just copy the value of the
+    target it is pointing to. You cannot set a value to an alias property, see
+    :class:`PSScriptProperty` which allows the caller to define a way to get
+    and set properties on an object dynamically.
 
     Note:
         When an object that has an alias property is deserialized, the property
         is converted to a :class:`PSNoteProperty` and the alias will no longer
         exist.
 
     Args:
         name: The name of the property.
         alias: The name of the property or attribute to point to.
         ps_type: If set, the property value will be casted to this PSObject
             type.
 
     Attributes:
         alias (str): The target of the alias.
-
-    .. _PSAliasProperty:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psaliasproperty
     """
 
     def __init__(
         self,
         name: str,
         alias: str,
         ps_type: typing.Optional[type] = None,
@@ -460,29 +458,27 @@
         return PSAliasProperty(self.name, self.alias, self.ps_type)
 
 
 class PSNoteProperty(PSPropertyInfo):
     """Note Property
 
     This is a property that stores a value as a name-value pair. Is is designed
-    to replicate the functionality of `PSNoteProperty`_ and is typically the
-    type of property to use when creating a PSObject.
+    to replicate the functionality of
+    `PSNoteProperty <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psnoteproperty>`_
+    and is typically the type of property to use when creating a PSObject.
 
     Note:
         See :class:`PSPropertyInfo` for more information on the `mandatory`
         argument.
 
     Args:
         name: The name of the property.
         value: The property value to set, if omitted the default is `None`.
         mandatory: The property must be defined when creating a PSObject.
         ps_type: If set, the property value will be casted to this PSObject type.
-
-    .. _PSNoteProperty:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psnoteproperty
     """
 
     def __init__(
         self,
         name: str,
         value: typing.Optional[typing.Any] = _UnsetValue,
         mandatory: bool = False,
@@ -495,15 +491,16 @@
 
 
 class PSScriptProperty(PSPropertyInfo):
     """Script Property
 
     This is a property that can get and optionally set another property or
     attribute of a PSObject at runtime. It is designed to replicate the
-    functionality of `PSScriptProperty`_.
+    functionality of
+    `PSScriptProperty <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psscriptproperty>`_.
 
     The getter callable must be a callable that has only 1 argument that is the
     PSObject the property is a member of. This allows the caller to retrieve a
     property of the PSObject at runtime or any other source as needed.
 
     The setter callable must be a callable that has only 2 arguments, the first
     being the value that needs to be set and the second is the PSObject the
@@ -513,17 +510,14 @@
     Args:
         name: The name of the property.
         getter: The callable to run when getting a value for this property.
         setter: The callable to run when setting a value for this property.
         mandatory: The property must be defined when creating a PSObject.
         ps_type: If set, the property value will be casted to this PSObjec
              type.
-
-    .. _PSScriptProperty:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psscriptproperty
     """
 
     def __init__(
         self,
         name: str,
         getter: typing.Callable[["PSObject"], typing.Any],
         setter: typing.Optional[typing.Callable[["PSObject", typing.Any], None]] = None,
@@ -798,93 +792,75 @@
 
         if self.tag is not None and self.tag not in registry.element_registry:
             registry.element_registry[self.tag] = cls
 
         return cls
 
 
-class PSCryptoProvider(metaclass=abc.ABCMeta):
-    """PSRemoting crypto provider
+class PSCryptoProvider:
+    """Serizliation crypto provider
 
-    The CryptoProvider used by PSRemoting that can encrypt and decrypt secure
-    exchanged in that PSSession. The key must be registered once it has been
-    generated using :meth:`PSCryptoProvider.register_key`.
+    The CryptoProvider used by the serializer to encrypt and decrypt
+    :class:`psrpcore.types.PSSecureString` values. The method used to encrypt
+    and decrypt these values differs across implementations.
     """
 
-    @abc.abstractmethod
-    def decrypt(self, value: bytes) -> bytes:
-        """Decrypts the encrypted bytes.
+    def decrypt(self, value: str) -> str:
+        """Decrypts the encrypted value.
 
-        Decrypts the encrypted bytes passed in.
+        Decrypts the encrypted value passed in. The value provided is the raw
+        XML element text of the ``<SS>`` element to decrypt.
 
         Args:
-            value: The encrypted bytes to decrypt.
+            value: The encrypted XML text element to decrypt.
 
         Returns:
-            bytes: The decrypted bytes.
+            str: The decrypted value.
         """
-        pass  # pragma: no cover
+        raise NotImplementedError()
 
-    @abc.abstractmethod
-    def encrypt(self, value: bytes) -> bytes:
+    def encrypt(self, value: str) -> str:
         """Encrypted the bytes.
 
-        Encrypts the bytes passed in.
+        Encrypts the value passed in and returns the raw XML ``<SS>`` element
+        for serialization.
 
         Args:
-            value: The bytes to encrypt.
+            value: The string to encrypt.
 
         Returns:
-            bytes: The encrypted bytes.
-        """
-        pass  # pragma: no cover
-
-    @abc.abstractmethod
-    def register_key(
-        self,
-        key: bytes,
-    ) -> None:
-        """Registers the session key.
-
-        Registers the session key that is used to encrypt and decrypt secure
-        strings for PSRP.
-
-        Args:
-            key: The session key negotiated between the client and server.
+            str: The encrypted and encoded XML text element.
         """
-        pass  # pragma: no cover
+        raise NotImplementedError()
 
 
 def add_member(
     obj: typing.Union[PSObject, typing.Type[PSObject]],
     prop: PSPropertyInfo,
     force: bool = False,
 ) -> None:
     """Add an extended property.
 
     This can add an extended property to a PSObject class or a specific
     instance of a class. This replicates some of the functionality in
-    `Update-TypeData`_ and `Add-Member`_ in PowerShell. If a property under the
-    same name already exists under that PSObject then `force=True` is required
-    to replace it. The same applies if there is an existing adapted property on
-    the object.
+    `Update-TypeData <https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/update-typedata>`_
+    and
+    `Add-Member <https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/add-member>`_
+    in PowerShell. If a property under the same name already exists under that
+    PSObject then `force=True` is required to replace it. The same applies if
+    there is an existing adapted property on the object.
 
     See :meth:`add_alias_property`, :meth:`add_note_property`, and
     :meth:`add_script_property` for simplified versions of this function.
 
     Args:
         obj: The PSObject class or an instance of a PSObject class to add the
             extended property to.
         prop: The property to add to the object or class.
         force: Overwrite the existing property ``True`` or fail ``False``.
-
-    .. _Update-TypeData:
-        https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/update-typedata
-    .. _Add-Member:
-        https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/add-member
     """
     ps_object = getattr(obj, "PSObject", None)
     if not ps_object:
         raise ValueError("The passing in object does not contain the required PSObject attribute")
 
     prop_name = prop.name
     adapted_properties = {p.name: i for i, p in enumerate(ps_object.adapted_properties)}
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_collection.py` & `psrpcore-0.3.0/src/psrpcore/types/_collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,19 +21,17 @@
     should inherit from. It cannot be instantiated directly and is meant to be
     used as a base class for any .NET dictionary types.
 
     Note:
         While you can implement your own custom dictionary .NET type like
         `System.Collections.Generic.Dictionary<TKey, TValue>`, any dictionary
         based .NET types will be deserialized by the remote PowerShell runspace
-        as `System.Collections.Hashtable`_. This .NET type is represented by
-        :class:`PSDict`.
-
-    .. _System.Collections.Hashtable:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.hashtable?view=net-5.0
+        as
+        `System.Collections.Hashtable <https://docs.microsoft.com/en-us/dotnet/api/system.collections.hashtable?view=net-5.0>`_.
+        This .NET type is represented by :class:`PSDict`.
     """
 
     def __new__(cls, *args: typing.Any, **kwargs: typing.Any) -> "PSDictBase":
         if cls == PSDictBase:
             raise TypeError(
                 f"Type {cls.__qualname__} cannot be instantiated; it can be used only as a base class for "
                 f"dictionary types."
@@ -100,38 +98,32 @@
     inherit from. It cannot be instantiated directly and is meant to be used as
     a base class for any .NET list types.
 
     Note:
         While you can implement your own custom list .NET type like
         `System.Collections.Generic.List<T>`, any list based .NET types will be
         deserialized by the remote PowerShell runspace as
-        `System.Collections.ArrayList`_. This .NET type is represented by
-        :class:`PSList`.
-
-    .. _System.Collections.ArrayList:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.arraylist?view=net-5.0
+        `System.Collections.ArrayList <https://docs.microsoft.com/en-us/dotnet/api/system.collections.arraylist?view=net-5.0>`_.
+        This .NET type is represented by :class:`PSList`.
     """
 
 
 class PSQueueBase(PSObject, queue.Queue):
     """The base queue type.
 
     This is the base queue PSObject type that all queue like objects should
     inherit from. It cannot be instantiated directly and is meant to be used as
     a base class for any .NET queue types.
 
     Note:
         While you can implement your own custom queue .NET type like
         `System.Collections.Generic.Queue<T>`, any queue based .NET types will
         be deserialized by the remote PowerShell runspace as
-        `System.Collections.Queue`_. This .NET type is represented by
-        :class:`PSQueue`.
-
-    .. _System.Collections.Queue:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.queue?view=net-5.0
+        `System.Collections.Queue <https://docs.microsoft.com/en-us/dotnet/api/system.collections.queue?view=net-5.0>`_.
+        This .NET type is represented by :class:`PSQueue`.
     """
 
     def __new__(cls, *args: typing.Any, **kwargs: typing.Any) -> "PSQueueBase":
         if cls == PSQueueBase:
             raise TypeError(
                 f"Type {cls.__qualname__} cannot be instantiated; it can be used only as a base class for "
                 f"queue types."
@@ -164,66 +156,51 @@
     collection but Python does not have a native stack type so this just
     replicates the a Python list.
 
     Note:
         While you can implement your own custom stack .NET type like
         `System.Collections.Generic.Stack<T>`, any stack based .NET types will
         be deserialized by the remote PowerShell runspace as
-        `System.Collections.Stack`_. This .NET type is represented by
-        :class:`PSStack`.
-
-    .. System.Collections.Stack:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.stack?view=net-5.0
+        `System.Collections.Stack <https://docs.microsoft.com/en-us/dotnet/api/system.collections.stack?view=net-5.0>`_.
+        This .NET type is represented by :class:`PSStack`.
     """
 
 
 @PSType(["System.Collections.Stack"], tag="STK")
 class PSStack(PSStackBase):
     """The Stack complex type.
 
     This is the stack complex type which represents the following types:
 
         Python: :class:`list`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.2.6.1 Stack`_
+        PSRP: `[MS-PSRP] 2.2.5.2.6.1 Stack <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e9cf648e-38fe-42ba-9ca3-d89a9e0a856a>`_
 
-        .NET: `System.Collections.Stack`_
+        .NET: `System.Collections.Stack <https://docs.microsoft.com/en-us/dotnet/api/system.collections.stack?view=net-5.0>`_
 
     A stack is a last-in, first-out setup but Python does not have a native
     stack type so this just uses a :class:`list`.
-
-    .. _[MS-PSRP] 2.2.5.2.6.1 Stack:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e9cf648e-38fe-42ba-9ca3-d89a9e0a856a
-
-    .. _System.Collections.Stack:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.stack?view=net-5.0
     """
 
 
 @PSType(["System.Collections.Queue"], tag="QUE")
 class PSQueue(PSQueueBase):
     """The Queue complex type.
 
     This is the queue complex type which represents the following types:
 
         Python: :class:`queue.Queue`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.2.6.2 Queue`_
-
-        .NET: `System.Collections.Queue`_
+        PSRP: `[MS-PSRP] 2.2.5.2.6.2 Queue <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ade9f023-ac30-4b7e-be17-900c02a6f837>`_
 
-    .. _[MS-PSRP] 2.2.5.2.6.2 Queue:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ade9f023-ac30-4b7e-be17-900c02a6f837
-
-    .. _System.Collections.Queue:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.queue?view=net-5.0
+        .NET: `System.Collections.Queue <https://docs.microsoft.com/en-us/dotnet/api/system.collections.queue?view=net-5.0>`_
     """
 
 
 # Would prefer an Generic.List<T> but regardless of the type a list is always deserialized by PowerShell as an
 # ArrayList so just do that here.
 @PSType(["System.Collections.ArrayList"], tag="LST")
 class PSList(PSListBase):
@@ -231,45 +208,33 @@
 
     This is the queue complex type which represents the following types:
 
         Python: :class:`list`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.2.6.3 List`_
-
-        .NET: `System.Collections.ArrayList`_
-
-    .. _[MS-PSRP] 2.2.5.2.6.3 List:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/f4bdb166-cefc-4d49-848c-7d08680ae0a7
+        PSRP: `[MS-PSRP] 2.2.5.2.6.3 List <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/f4bdb166-cefc-4d49-848c-7d08680ae0a7>`_
 
-    .. _System.Collections.ArrayList:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.arraylist?view=net-5.0
+        .NET: `System.Collections.ArrayList <https://docs.microsoft.com/en-us/dotnet/api/system.collections.arraylist?view=net-5.0>`_
     """
 
 
 @PSType(["System.Collections.Hashtable"], tag="DCT")
 class PSDict(PSDictBase):
     """The Dictionary complex type.
 
     This is the dictionary complex type which represents the following types:
 
         Python: :class:`dict`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.2.6.4 Dictionaries`_
+        PSRP: `[MS-PSRP] 2.2.5.2.6.4 Dictionaries <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c4e000a2-21d8-46c0-a71b-0051365d8273>`_
 
-        .NET: `System.Collections.Hashtable`_
-
-    .. _[MS-PSRP] 2.2.5.2.6.4 Dictionaries:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c4e000a2-21d8-46c0-a71b-0051365d8273
-
-    .. _System.Collections.Hashtable:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.hashtable?view=net-5.0
+        .NET: `System.Collections.Hashtable <https://docs.microsoft.com/en-us/dotnet/api/system.collections.hashtable?view=net-5.0>`_
     """
 
 
 @PSType(["System.Collections.IEnumerable"], tag="IE")
 class PSIEnumerable(_PSListBase):
     """The IEnumerable complex type.
 
@@ -277,12 +242,9 @@
 
         Python: :class:`list`
 
         Native Serialization: no
 
         PSRP: N/A - Mentioned in :class:`PSList`
 
-        .NET `System.Collections.IEnumerable`_
-
-    .. _System.Collections.IEnumerable:
-        https://docs.microsoft.com/en-us/dotnet/api/system.collections.ienumerable?view=net-5.0
+        .NET `System.Collections.IEnumerable <https://docs.microsoft.com/en-us/dotnet/api/system.collections.ienumerable?view=net-5.0>`_
     """
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_complex.py` & `psrpcore-0.3.0/src/psrpcore/types/_complex.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 # Copyright: (c) 2021, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
 """PSRP/.NET Complex Types.
 
 The PSRP/.NET Complex Type class definitions. A complex type is pretty much
 anything that isn't a primitive type as known to the protocol. Most of the
-types defined here are defined in `MS-PSRP 2.2.3 Other Object Types`_ but some
-are also just other .NET objects that are used in the PSRP protocol. Some types
-are a PSRP specific representation of an actual .NET type but with a few minor
-differences. These types are prefixed with `PSRP` to differentiate between the
-PSRP specific ones and the actual .NET types.
-
-.. _MS-PSRP 2.2.3 Other Object Types:
-    https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e41c4a38-a821-424b-bc1c-89f8478c39ae
+types defined here are defined in
+`MS-PSRP 2.2.3 Other Object Types <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e41c4a38-a821-424b-bc1c-89f8478c39ae>`_
+but some are also just other .NET objects that are used in the PSRP protocol.
+Some types are a PSRP specific representation of an actual .NET type but with
+a few minor differences. These types are prefixed with `PSRP` to differentiate
+between the PSRP specific ones and the actual .NET types.
 """
 
 import collections
+import datetime
+import getpass
 import ntpath
+import os
+import platform
 import posixpath
+import threading
 import typing
 
 from psrpcore.types._base import (
     PSAliasProperty,
     PSNoteProperty,
     PSObject,
     PSScriptProperty,
@@ -82,26 +85,22 @@
 
 
 @PSType(["System.ConsoleColor"])
 class ConsoleColor(PSEnumBase):
     """System.ConsoleColor enum.
 
     Specifies constants that define foreground and background colors for the
-    console. This is also documented under `[MS-PSRP] 2.2.3.3 Color`_ but in
-    the :class:`HostInfo` default data format.
+    console. This is also documented under
+    `[MS-PSRP] 2.2.3.3 Color <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d7edefec-41b1-465d-bc07-2a8ec9d727a1>`_
+    but in the :class:`HostInfo` default data format.
 
     Note:
-        This is an auto-generated Python class for the `System.ConsoleColor`_
+        This is an auto-generated Python class for the
+        `System.ConsoleColor <https://docs.microsoft.com/en-us/dotnet/api/system.consolecolor?view=net-5.0>`_
         .NET class.
-
-    .. _System.ConsoleColor:
-        https://docs.microsoft.com/en-us/dotnet/api/system.consolecolor?view=net-5.0
-
-    .. _[MS-PSRP] 2.2.3.3 Color:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d7edefec-41b1-465d-bc07-2a8ec9d727a1
     """
 
     Black = 0
     DarkBlue = 1
     DarkGreen = 2
     DarkCyan = 3
     DarkRed = 4
@@ -123,18 +122,16 @@
     """System.Management.Automation.ProgressRecordType enum.
 
     Defines two types of progress record that refer to the beginning
     (or middle) and end of an operation.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.ProgressRecordType`_ .NET class.
-
-    .. _System.Management.Automation.ProgressRecordType:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.progressrecordtype
+        `System.Management.Automation.ProgressRecordType <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.progressrecordtype>`_
+        .NET class.
     """
 
     Processing = 0  #: Operation just started or is not yet complete.
     Completed = 1  #: Operation is complete.
 
 
 @PSType(["System.Management.Automation.PSCredentialTypes"])
@@ -142,18 +139,16 @@
     """System.Management.Automation.PSCredentialTypes enum flags.
 
     Defines the valid types of credentials. Used by
     :class:`HostMethodIdentifier.PromptForCredential2` calls.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.PSCredentialTypes`_ .NET class.
-
-    .. _System.Management.Automation.PSCredentialTypes:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscredentialtypes
+        `System.Management.Automation.PSCredentialTypes <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscredentialtypes>`_
+        .NET class.
     """
 
     Generic = 1  #: Generic credentials.
     Domain = 2  #: Credentials valid for a domain.
     Default = Generic | Domain  #: Default credentials (Generic | Domain).
 
 
@@ -162,18 +157,16 @@
     """System.Management.Automation.PSCredentialUIOptions enum flags.
 
     Defines the options available when prompting for credentials. Used by
     :class:`HostMethodIdentifier.PromptForCredential2` calls.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.PSCredentialUIOptions`_ .NET class.
-
-    .. _System.Management.Automation.PSCredentialUIOptions:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscredentialuioptions
+        `System.Management.Automation.PSCredentialUIOptions <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscredentialuioptions>`_
+        .NET class.
     """
 
     none = 0  #: Performs no validation.
     ValidateUserNameSyntax = 1  #: Validates the username, but not its existence or correctness.
     AlwaysPrompt = 2  #: Always prompt, even if a persisted credential was available.
     ReadOnlyUsername = 3  #: Username is read-only, and the user may not modify it.
     Default = ValidateUserNameSyntax  #: Validates the username, but not its existence or correctness.
@@ -183,40 +176,33 @@
 class SessionStateEntryVisibility(PSEnumBase):
     """System.Management.Automation.SessionStateEntryVisibility enum.
 
     Defines the visibility of execution environment elements.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.SessionStateEntryVisibility`_ .NET class.
-
-    .. _System.Management.Automation.SessionStateEntryVisibility:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.sessionstateentryvisibility
+        `System.Management.Automation.SessionStateEntryVisibility <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.sessionstateentryvisibility>`_
+        .NET class.
     """
 
     Public = 0  #: Entries are visible to requests from outside the runspace.
     Private = 1  #: Entries are not visible to requests from outside the runspace.
 
 
 @PSType(["System.Management.Automation.Runspaces.RunspacePoolState"])
 class RunspacePoolState(PSEnumBase):
     """RunspacePoolState enum.
 
     Defines the current state of the Runspace Pool. It is documented in PSRP
-    under `[MS-PSRP] 2.2.3.4 RunspacePoolState`_ and while it shares the same
-    name as the .NET type
-    `System.Management.Automation.Runspaces.RunspacePoolState`_ it has a few
-    extra names and some values that do not match. The .NET enum is used here
-    as that's what PowerShell uses internally.
-
-    .. _[MS-PSRP] 2.2.3.4 RunspacePoolState:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/b05495bc-a9b2-4794-9f43-4bf1f3633900
-
-    .. _System.Management.Automation.Runspaces.RunspacePoolState:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.runspacepoolstate
+    under
+    `[MS-PSRP] 2.2.3.4 RunspacePoolState <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/b05495bc-a9b2-4794-9f43-4bf1f3633900>`_
+    and while it shares the same name as the .NET type
+    `System.Management.Automation.Runspaces.RunspacePoolState <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.runspacepoolstate>`_
+    it has a few extra names and some values that do not match. The .NET enum
+    is used here as that's what PowerShell uses internally.
     """
 
     BeforeOpen = 0  #: Beginning state upon creation.
     Opening = 1  #: A RunspacePool is being created.
     Opened = 2  #: The RunspacePool is created and valid.
     Closed = 3  #: The RunspacePool is closed.
     Closing = 4  #: The RunspacePool is being closed.
@@ -227,25 +213,20 @@
 
 
 @PSType(["System.Management.Automation.PSInvocationState"])
 class PSInvocationState(PSEnumBase):
     """PSInvocationState enum.
 
     Defines the current state of the Pipeline. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.5 PSInvocationState`_.
+    `[MS-PSRP] 2.2.3.5 PSInvocationState <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/acaa253a-29be-45fd-911c-6715515a28b9>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.PSInvocationState`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.5 PSInvocationState:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/acaa253a-29be-45fd-911c-6715515a28b9
-
-    .. _System.Management.Automation.PSInvocationState:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psinvocationstate
+        `System.Management.Automation.PSInvocationState <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.psinvocationstate>`_
+        .NET class.
     """
 
     NotStarted = 0  #: Pipeline has not been started
     Running = 1  #: Pipeline is executing.
     Stopping = 2  #: Pipeline is stopping execution.
     Stopped = 3  #: Pipeline is completed due to a stop request.
     Completed = 4  #: Pipeline has completed executing a command.
@@ -255,74 +236,60 @@
 
 @PSType(["System.Management.Automation.Runspaces.PSThreadOptions"])
 class PSThreadOptions(PSEnumBase):
     """System.Management.Automation.Runspaces.PSThreadOptions enum.
 
     Control whether a new thread is created when a command is executed within a
     Runspace. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.6 PSThreadOptions`_.
+    `[MS-PSRP] 2.2.3.6 PSThreadOptions <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/bfc63adb-d6f1-4ccc-9bd8-73de6cc78dda>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Runspaces.PSThreadOptions`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.6 PSThreadOptions:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/bfc63adb-d6f1-4ccc-9bd8-73de6cc78dda
-
-    .. _System.Management.Automation.Runspaces.PSThreadOptions:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.psthreadoptions
+        `System.Management.Automation.Runspaces.PSThreadOptions <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.psthreadoptions>`_
+        .NET class.
     """
 
     Default = 0  #: Use the server thread option settings.
     UseNewThread = 1  #: Creates a new thread for each invocation.
     ReuseThread = 2
     """ Creates a new thread for the first invocation and then re-uses that thread in subsequent invocations. """
     UseCurrentThread = 3  #: Doesn't create a new thread; the execution occurs on the thread that called Invoke.
 
 
 @PSType(["System.Threading.ApartmentState"])
 class ApartmentState(PSEnumBase):
     """System.Management.Automation.Runspaces.ApartmentState enum.
 
     Specifies the apartment state of a Thread. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.7 ApartmentState`_.
+    `[MS-PSRP] 2.2.3.7 ApartmentState <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/6845133d-7503-450d-a74e-388cdd3b2386>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Threading.ApartmentState`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.7 ApartmentState:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/6845133d-7503-450d-a74e-388cdd3b2386
-
-    .. _System.Threading.ApartmentState:
-        https://docs.microsoft.com/en-us/dotnet/api/system.threading.apartmentstate?view=net-5.0
+        `System.Threading.ApartmentState <https://docs.microsoft.com/en-us/dotnet/api/system.threading.apartmentstate?view=net-5.0>`_
+        .NET class.
     """
 
     STA = 0  #: The thread will create and enter a multi-threaded apartment.
     MTA = 1  #: The thread will create and enter a single-threaded apartment.
     Unknown = 2  #: The ApartmentState property has not been set.
 
 
 @PSType(["System.Management.Automation.RemoteStreamOptions"])
 class RemoteStreamOptions(PSFlagBase):
     """System.Management.Automation.RemoteStreamOptions enum flags.
 
     Control whether InvocationInfo is added to items in the Error, Warning,
     Verbose and Debug streams during remote calls. It is documented in PSRP
-    under `[MS-PSRP] 2.2.3.8 RemoteStreamOptions`_.
+    under
+    `[MS-PSRP] 2.2.3.8 RemoteStreamOptions <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4941e59c-ce01-4549-8eb5-372b8eb6dd12>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.RemoteStreamOptions`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.8 RemoteStreamOptions:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4941e59c-ce01-4549-8eb5-372b8eb6dd12
-
-    .. _System.Management.Automation.RemoteStreamOptions:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.remotestreamoptions
+        `System.Management.Automation.RemoteStreamOptions <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.remotestreamoptions>`_
+        .NET class.
     """
 
     none = 0  #: InvocationInfo is not added to any stream record.
     AddInvocationInfoToErrorRecord = 1  #: InvocationInfo is added to any :class:`ErrorRecord`.
     AddInvocationInfoToWarningRecord = 2  #: InvocationInfo is added to any `Warning` :class:`InformationalRecord`.
     AddInvocationInfoToDebugRecord = 4  #: InvocationInfo is added to any `Debug` :class:`InformationalRecord`.
     AddInvocationInfoToVerboseRecord = 8  #: InvocationInfo is added to any `Verbose` :class:`InformationalRecord`.
@@ -330,25 +297,21 @@
 
 
 @PSType(["System.Management.Automation.ErrorCategory"])
 class ErrorCategory(PSEnumBase):
     """System.Management.Automation.ErrorCategory enum.
 
     Errors reported by PowerShell will be in one of these categories. It is
-    documented in PSRP under `[MS-PSRP] 2.2.3.9 ErrorCategory`_.
+    documented in PSRP under
+    `[MS-PSRP] 2.2.3.9 ErrorCategory <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ae7d6061-15c8-4184-a05e-1033dbb7228b>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.ErrorCategory`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.9 ErrorCategory:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ae7d6061-15c8-4184-a05e-1033dbb7228b
-
-    .. _System.Management.Automation.ErrorCategory:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errorcategory
+        `System.Management.Automation.ErrorCategory <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errorcategory>`_
+        .NET class.
     """
 
     NotSpecified = 0  #: No error category is specified, or the error category is invalid.
     OpenError = 1
     CloseError = 2
     DeviceError = 3
     DeadlockDetected = 4
@@ -382,25 +345,21 @@
 
 
 @PSType(["System.Management.Automation.CommandTypes"])
 class CommandTypes(PSFlagBase):
     """System.Management.Automation.CommandTypes enum flags.
 
     Defines the types of commands that PowerShell can execute. It is documented
-    in PSRP under `[MS-PSRP] 2.2.3.19 CommandType`_.
+    in PSRP under
+    `[MS-PSRP] 2.2.3.19 CommandType <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/a038c5c9-a220-4064-aa78-ed9cf5a2893c>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.CommandTypes`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.19 CommandType:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/a038c5c9-a220-4064-aa78-ed9cf5a2893c
-
-    .. _System.Management.Automation.CommandTypes:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.commandtypes
+        `System.Management.Automation.CommandTypes <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.commandtypes>`_
+        .NET class.
     """
 
     Alias = 1  #: Aliases create a name that refers to other command types.
     Function = 2  #: Script functions that are defined by a script block.
     Filter = 4  #: Script filters that are defined by a script block.
     Cmdlet = 8  #: A cmdlet.
     ExternalScript = 16  #: A PowerShell script (`*.ps1` file).
@@ -411,51 +370,42 @@
 
 
 @PSType(["System.Management.Automation.CommandOrigin"])
 class CommandOrigin(PSEnumBase):
     """System.Management.Automation.CommandOrigin enum.
 
     Defines the dispatch origin of a command. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.30 CommandOrigin`_.
+    `[MS-PSRP] 2.2.3.30 CommandOrigin <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/6c35a5de-d063-4097-ace5-002a0c5e452d>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.CommandOrigin`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.30 CommandOrigin:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/6c35a5de-d063-4097-ace5-002a0c5e452d
-
-    .. _System.Management.Automation.CommandOrigin:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.commandorigin
+        `System.Management.Automation.CommandOrigin <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.commandorigin>`_
+        .NET class.
     """
 
     Runspace = 0  #: The command was submited via a runspace.
     Internal = 1  #: The command was dispatched by the PowerShell engine.
 
 
 @PSType(["System.Management.Automation.Runspaces.PipelineResultTypes"])
 class PipelineResultTypes(PSFlagBase):
     """System.Management.Automation.Runspaces.PipelineResultTypes enum flags.
 
     Defines the types of streams coming out of a pipeline. It is documented in
-    PSRP under `[MS-PSRP] 2.2.3.31 PipelineResultTypes`_. .NET and MS-PSRP have
-    separate values but .NET is used as it is the correct source.
-    Technically the values are not designed as flags but there are some older
-    APIs that combine Output | Error together.
+    PSRP under
+    `[MS-PSRP] 2.2.3.31 PipelineResultTypes <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/efdce0ba-531e-4904-9cab-b65c476c649a>`_.
+    .NET and MS-PSRP have
+    separate values but .NET is used as it is the correct source. Technically
+    the values are not designed as flags but there are some older APIs that
+    combine Output | Error together.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Runspaces.PipelineResultTypes`_ .NET
-        class.
-
-    .. _[MS-PSRP] 2.2.3.31 PipelineResultTypes:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/efdce0ba-531e-4904-9cab-b65c476c649a
-
-    .. _System.Management.Automation.Runspaces.PipelineResultTypes:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.pipelineresulttypes
+        `System.Management.Automation.Runspaces.PipelineResultTypes <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.runspaces.pipelineresulttypes>`_
+        .NET class.
     """
 
     none = 0  #: Default streaming behaviour.
     Output = 1  #: Output stream.
     Error = 2  #: Error stream.
     Warning = 3  #: Warning stream.
     Verbose = 4  #: Verbose stream.
@@ -478,30 +428,27 @@
     ],
 )
 class ScriptPosition(PSObject):
     """ScriptPosition.
 
     Represents a single point in a script. This script may come from a file or
     interactive input. This is the actual .NET type
-    `System.Management.Automation.Language.ScriptPosition`_.
+    `System.Management.Automation.Language.ScriptPosition <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.language.scriptposition>`_.
 
     Args:
         File: The name of the file, or if the script did not come from a file,
             then null.
         LineNumber: The line number of the position, with the value 1 being the
             first line.
         ColumnNumber: The column number of the position, with the value 1 being
             the first column.
         Line: The complete text of the line that this position is included on.
 
     Attributes:
         Offset (:class:`PSInt`): Not used in pwsh.
-
-    .. _System.Management.Automation.Language.ScriptPosition:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.language.scriptposition
     """
 
 
 @PSType(
     type_names=[
         "System.Management.Automation.Language.ScriptExtent",
     ],
@@ -519,22 +466,19 @@
     ],
 )
 class ScriptExtent(PSObject):
     """ScriptExtent.
 
     A script extend used to customize the display of error location
     information. This is the actual .NET type
-    `System.Management.Automation.Language.ScriptExtent`_.
+    `System.Management.Automation.Language.ScriptExtent <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.language.scriptextent>`_.
 
     Args:
         StartPosition: The position beginning the extent.
         EndPosition: The position ending the extent.
-
-    .. _System.Management.Automation.Language.ScriptExtent:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.language.scriptextent
     """
 
     def __init__(
         self,
         StartPosition: ScriptPosition,
         EndPosition: ScriptPosition,
     ):
@@ -610,15 +554,16 @@
         PSNoteProperty("UnboundArguments", ps_type=PSList),
     ],
 )
 class InvocationInfo(PSObject):
     """InvocationInfo.
 
     Describes how and where this command was invoked. This is the actual .NET
-    type `System.Management.Automation.InvocationInfo`_.
+    type
+    `System.Management.Automation.InvocationInfo <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.invocationinfo>`_.
 
     Args:
         BoundParameters: Dictionary of parameters that were bound for this
             script or command.
         CommandOrigin: Command was being invoked inside the runspace or if it
             was an external request.
         DisplayScriptPosition: The position for the invocation or error.
@@ -640,17 +585,14 @@
             invoked.
         PSScriptRoot: The directory from where the command was being invoked.
         ScriptLineNumber: The line number in the executing script that contains
             this cmdlet.
         ScriptName: The name of the script containing the cmdlet.
         UnboundArguments: The list of arguments that were not bound to any
             parameter.
-
-    .. _System.Management.Automation.InvocationInfo:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.invocationinfo
     """
 
 
 def _invocation_info_from_ps_object(
     obj: PSObject,
 ) -> InvocationInfo:
     """Used by ErrorRecord and InformationalRecord to deserialize the invocation info details."""
@@ -762,25 +704,23 @@
         PSNoteProperty("TargetType", ps_type=PSString),
     ],
 )
 class ErrorCategoryInfo(PSObject):
     """ErrorCategoryInfo.
 
     Contains auxiliary information about an ErrorRecord. This is the actual
-    .NET type `System.Management.Automation.ErrorCategoryInfo`_.
+    .NET type
+    `System.Management.Automation.ErrorCategoryInfo <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errorcategoryinfo>`_.
 
     Args:
         Category: The error category.
         Activity: Description of the operation which encountered the error.
         Reason: Description of the error.
         TargetName: Description of the target object.
         TargetType: Description of the type of the target object.
-
-    .. _System.Management.Automation.ErrorCategoryInfo:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errorcategoryinfo
     """
 
     def __str__(self) -> str:
         return (
             f'{self.Category.name!s} ({self.TargetName or ""}:{self.TargetType or ""}) '
             f'[{self.Activity or ""}], {self.Reason or ""}'
         )
@@ -799,23 +739,21 @@
     """ErrorDetails.
 
     ErrorDetails represents additional details about an :class:`ErrorRecord`,
     starting with a replacement Message. Clients can use ErrorDetails when they
     want to display a more specific message than the one contained in a
     particular Exception, without having to create a new Exception or define a
     new Exception class. This is the actual
-    .NET type `System.Management.Automation.ErrorDetails`_.
+    .NET type
+    `System.Management.Automation.ErrorDetails <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errordetails>`_.
 
     Args:
         Message: Message with replaces Message in Exception.
         RecommendedAction: Describes the recommended action in the event this
             error occurs. This can be empty if not applicable.
-
-    .. _System.Management.Automation.ErrorDetails:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errordetails
     """
 
 
 @PSType(
     type_names=[
         "System.Management.Automation.ErrorRecord",
     ],
@@ -830,17 +768,20 @@
         PSNoteProperty("ScriptStackTrace", ps_type=PSString),
     ],
 )
 class ErrorRecord(PSObject):
     """ErrorRecord.
 
     The data type that represents information about an error. It is documented
-    in PSRP under `[MS-PSRP] 2.2.3.15 ErrorRecord`_. The invocation specific
-    properties are documented under `[MS-PSRP] 2.2.3.15.1 InvocationInfo`_.
-    This is the actual .NET type `System.Management.Automation.ErrorRecord`_
+    in PSRP under
+    `[MS-PSRP] 2.2.3.15 ErrorRecord <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/0fe855a7-d13c-44e2-aa88-291e2054ae3a>`_.
+    The invocation specific properties are documented under
+    `[MS-PSRP] 2.2.3.15.1 InvocationInfo <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/000363b7-e2f9-4a34-94f5-d540a15aee7b>`_.
+    This is the actual .NET type
+    `System.Management.Automation.ErrorRecord <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errorrecord>`_
 
     Args:
         Exception: An exception describing the error.
         TargetObject: The object against which the error occurred.
         FullyQualifiedErrorId: String which uniquely identifies this error
             condition.
         CategoryInfo: Information regarding the ErrorCategory associated with
@@ -848,23 +789,14 @@
         ErrorDetails: Additional information about the error.
         InvocationInfo: Identifies the cmdlet, script, or other command which
             caused the error.
         PipelineIterationInfo: The status of the pipeline when this record was
             created. Each entry represents the number of inputs the command[i]
             in the statement has processed when the record was created.
         ScriptStackTrace: The object against which the error occurred.
-
-    .. _[MS-PSRP] 2.2.3.15 ErrorRecord:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/0fe855a7-d13c-44e2-aa88-291e2054ae3a
-
-    .. _[MS-PSRP] 2.2.3.15.1 InvocationInfo:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/000363b7-e2f9-4a34-94f5-d540a15aee7b
-
-    .. _System.Management.Automation.ErrorRecord:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.errorrecord
     """
 
     def __init__(
         self,
         *args: typing.Any,
         **kwargs: typing.Any,
     ) -> None:
@@ -974,34 +906,27 @@
 )
 class InformationalRecord(PSObject):
     """PowerShell InformationalRecord.
 
     InformationalRecord (that is Debug, Warning, or Verbose) is a structure
     that contains additional information that a pipeline can output in addition
     to the regular data output. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.16 InformationalRecord`_. The invocation specific
-    properties are documented under `[MS-PSRP] 2.2.3.15.1 InvocationInfo`_.
+    `[MS-PSRP] 2.2.3.16 InformationalRecord <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/97cad2dc-c34a-4db6-bfa1-cbf196853937>`_.
+    The invocation specific properties are documented under
+    `[MS-PSRP] 2.2.3.15.1 InvocationInfo <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/000363b7-e2f9-4a34-94f5-d540a15aee7b>`_.
     This also represents the
-    `System.Management.Automation.InformationalRecord`_ .NET type.
+    `System.Management.Automation.InformationalRecord <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.informationalrecord>`_
+    .NET type.
 
     Args:
         Message: The message writen by the command that created this record.
         InvocationInfo: The invocation info of the command that created this
             record.
         PipelineIterationInfo: The status of the pipeline when this record was
             created.
-
-    .. _[MS-PSRP] 2.2.3.16 InformationalRecord:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/97cad2dc-c34a-4db6-bfa1-cbf196853937
-
-    .. _[MS-PSRP] 2.2.3.15.1 InvocationInfo:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/000363b7-e2f9-4a34-94f5-d540a15aee7b
-
-    .. _System.Management.Automation.InformationalRecord:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.informationalrecord
     """
 
     def __init__(
         self,
         *args: typing.Any,
         **kwargs: typing.Any,
     ) -> None:
@@ -1028,15 +953,15 @@
         record.serialize_extended_info = obj.InformationalRecord_SerializeInvocationInfo
 
         return record
 
     @classmethod
     def ToPSObjectForRemoting(
         cls,
-        instance: "ErrorRecord",
+        instance: "InformationalRecord",
         **kwargs: typing.Any,
     ) -> PSObject:
         obj = PSObject()
         add_note_property(obj, "InformationalRecord_Message", instance.Message)
 
         if instance.serialize_extended_info and instance.InvocationInfo:
             add_note_property(obj, "InformationalRecord_SerializeInvocationInfo", True)
@@ -1050,42 +975,36 @@
 
 
 @PSType(["System.Management.Automation.DebugRecord"])
 class DebugRecord(InformationalRecord):
     """DebugRecord.
 
     A debug record in the PSInformationalBuffers. This represents the
-    `System.Management.Automation.DebugRecord`_ .NET type.
-
-    .. _System.Management.Automation.DebugRecord:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.debugrecord?view=powershellsdk-7.0.0
+    `System.Management.Automation.DebugRecord <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.debugrecord?view=powershellsdk-7.0.0>`_
+    .NET type.
     """
 
 
 @PSType(["System.Management.Automation.VerboseRecord"])
 class VerboseRecord(InformationalRecord):
     """VerboseRecord.
 
     A verbose record in the PSInformationalBuffers. This represents the
-    `System.Management.Automation.VerboseRecord`_ .NET type.
-
-    .. _System.Management.Automation.VerboseRecord:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.verboserecord?view=powershellsdk-7.0.0
+    `System.Management.Automation.VerboseRecord <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.verboserecord?view=powershellsdk-7.0.0>`_
+    .NET type.
     """
 
 
 @PSType(["System.Management.Automation.WarningRecord"])
 class WarningRecord(InformationalRecord):
     """WarningRecord.
 
     A warning record in the PSInformationalBuffers. This represents the
-    `System.Management.Automation.WarningRecord`_ .NET type.
-
-    .. _System.Management.Automation.WarningRecord:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.warningrecord?view=powershellsdk-7.0.0
+    `System.Management.Automation.WarningRecord <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.warningrecord?view=powershellsdk-7.0.0>`_
+    .NET type.
     """
 
 
 @PSType(
     type_names=["System.Management.Automation.ProgressRecord"],
     adapted_properties=[
         PSNoteProperty("ActivityId", mandatory=True, ps_type=PSInt),
@@ -1100,15 +1019,16 @@
     tag="PR",
 )
 class ProgressRecord(PSObject):
     """ProgressRecord.
 
     Defines a data structure used to represent the status of an ongoing
     operation at a point in time. This represents the
-    `System.Management.Automation.ProgressRecord`_ .NET type.
+    `System.Management.Automation.ProgressRecord <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.progressrecord?view=powershellsdk-7.0.0>`_
+    .NET type.
 
     Args:
         Activity: Description of the activity.
         ActivityId: Id of the activity, used as a key for the linking of
             subordinate activities.
 
         CurrentOperation: Current operation of the many required to accomplish
@@ -1117,17 +1037,14 @@
         PercentComplete: Percentage of total work for the activity that is
             completed.
         RecordType: Type of record represented by this instance.
         SecondsRemaining: Estimated time remaining until the activity is
             complete.
         StatusDescription: Current status of the operation, e.g. "35 of 50
             items copied".
-
-    .. _System.Management.Automation.ProgressRecord:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.progressrecord?view=powershellsdk-7.0.0
     """
 
 
 @PSType(
     ["System.Management.Automation.InformationRecord"],
     adapted_properties=[
         PSNoteProperty("MessageData"),
@@ -1142,98 +1059,134 @@
     ],
 )
 class InformationRecord(PSObject):
     """InformationRecord.
 
     Defines a data structure used to represent informational context destined
     for the host or user. This represents the
-    `System.Management.Automation.InformationRecord`_ .NET type.
+    `System.Management.Automation.InformationRecord <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.informationrecord?view=powershellsdk-7.0.0>`_
+    .NET type.
 
     Args:
         MessageData: The message data for the informational record.
         Source: The source of the information record (script path, function
             name, etc.).
         TimeGenerated: The time the informational record was generated.
         Tags: The tags associated with this informational record.
-        User: THe user that generated the informational record.
+        User: The user that generated the informational record.
         Computer: THe computer that generated the informational record.
         ProcessId: The process that generated the informational record.
         NativeThreadId: The native thread that generated the informational
             record.
         ManagedThreadId: The managed thread that generated the informational
             record.
-
-    .. _System.Management.Automation.InformationRecord:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.informationrecord?view=powershellsdk-7.0.0
     """
 
+    @classmethod
+    def create(
+        cls,
+        message_data: typing.Any,
+        source: str,
+        *,
+        time_generated: typing.Optional[datetime.datetime] = None,
+        tags: typing.Optional[typing.List[str]] = None,
+        user: typing.Optional[str] = None,
+        computer: typing.Optional[str] = None,
+        process_id: typing.Optional[int] = None,
+        native_thread_id: typing.Optional[int] = None,
+        managed_thread_id: typing.Optional[int] = None,
+    ) -> "InformationRecord":
+        """Helper class for creating InformationRecords with defaults."""
+
+        time_generated = PSDateTime.now() if time_generated is None else time_generated
+        if not tags:
+            tags = PSList([])
+
+        if user is None:
+            try:
+                # getuser on Windows relies on env vars that may not may not be set. Just fallback gracefully.
+                user = getpass.getuser()
+
+            except ModuleNotFoundError:  # pragma: no cover
+                user = "Unknown"
+
+        computer = PSString(platform.node()) if computer is None else computer
+        process_id = os.getpid() if process_id is None else process_id
+
+        # get_native_id isn't available until 3.8, default to 0.
+        native_thread_id = threading.get_native_id() if native_thread_id is None else native_thread_id
+
+        return InformationRecord(
+            MessageData=message_data,
+            Source=source,
+            TimeGenerated=time_generated,
+            Tags=tags,
+            User=user,
+            Computer=computer,
+            ProcessId=process_id,
+            NativeThreadId=native_thread_id,
+            ManagedThreadId=managed_thread_id or 0,
+        )
+
 
 @PSType(type_names=["System.Management.Automation.PSPrimitiveDictionary"])
 class PSPrimitiveDictionary(PSDict):
     """Primitive Dictionary.
 
     A primitive dictionary represents a dictionary which contains only objects
     that are primitive types. While Python does not place any limitations on
     the types this object can contain, trying to serialize a
     PSPrimitiveDictionary with complex types to PowerShell will fail. The types
-    that are allowed can be found at `[MS-PSRP] 2.2.3.18 Primitive Dictionary`_.
-
-    .. _[MS-PSRP] 2.2.3.18 Primitive Dictionary:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/7779aa42-6927-4225-b31c-2771fd869546
+    that are allowed can be found at
+    `[MS-PSRP] 2.2.3.18 Primitive Dictionary <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/7779aa42-6927-4225-b31c-2771fd869546>`_.
     """
 
 
 @PSType(
     type_names=["Selected.Microsoft.PowerShell.Commands.GenericMeasureInfo"],
     extended_properties=[
         PSNoteProperty("Count", mandatory=True, ps_type=PSInt),
     ],
 )
 class CommandMetadataCount(PSCustomObject):
     """CommandMetadataCount.
 
     Special data type used by the command metadata messages. It is documented
-    in PSRP under `[MS-PSRP] 2.2.3.21 CommandMetadataCount`_.
+    in PSRP under
+    `[MS-PSRP] 2.2.3.21 CommandMetadataCount <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4647da0c-18e6-496c-9d9e-c669d40dc1db>`_.
 
     Args:
         Count: The count.
-
-    .. _[MS-PSRP] 2.2.3.21 CommandMetadataCount:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4647da0c-18e6-496c-9d9e-c669d40dc1db
     """
 
 
 @PSType(
     type_names=["System.Management.Automation.PSCredential"],
     adapted_properties=[
         PSNoteProperty("UserName", mandatory=True, ps_type=PSString),
         PSNoteProperty("Password", mandatory=True, ps_type=PSSecureString),
     ],
 )
 class PSCredential(PSObject):
     """PSCredential.
 
     Represents a username and a password. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.25 PSCredential`_. It also represents the
-    `System.Management.Automation.PSCredential`_ .NET type.
+    `[MS-PSRP] 2.2.3.25 PSCredential <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/a7c91a93-ee59-4af0-8a67-a9361af9870e>`_.
+    It also represents the
+    `System.Management.Automation.PSCredential <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscredential>`_
+    .NET type.
 
     Note:
         To be able to serialize this object, a session key is exchanged between
         the host and the peer. If the peer does not support the session key
         exchange then this cannot be serialized.
 
     Args:
         UserName: The username for the credential.
         Password: The password for the credential.
-
-    .. _[MS-PSRP] 2.2.3.25 PSCredential:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/a7c91a93-ee59-4af0-8a67-a9361af9870e
-
-    .. _System.Management.Automation.PSCredential:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.pscredential
     """
 
 
 @PSType(
     type_names=[
         "System.Exception",
     ],
@@ -1247,24 +1200,22 @@
         PSNoteProperty("StackTrace", ps_type=PSString),
         PSNoteProperty("TargetSite", ps_type=PSString),
     ],
 )
 class NETException(PSObject):
     """.NET Exception.
 
-    Represents a .NET `System.Exception`_ type. It isn't documented in
-    MS-PSRP but is used when creating an ErrorRecord or just as a base of
-    another exception type.
+    Represents a .NET
+    `System.Exception <https://docs.microsoft.com/en-us/dotnet/api/system.exception?view=net-5.0>`_
+    type. It isn't documented in MS-PSRP but is used when creating an
+    ErrorRecord or just as a base of another exception type.
 
     Args:
         Message: Message that describes the current exception.
         Data: User defined information about the exception.
         HelpLink: A link to the help file associated with this exception.
         HResult: A coded numerical value that is assigned to a specific exception.
         InnerException: Exception instance that caused the current exception.
         Source: Name of the application or the object that causes the error.
         StackTrace: String representation of the immediate frames on the call stack.
         TargetSite: Method that throws the current exception.
-
-    .. _System.Exception:
-        https://docs.microsoft.com/en-us/dotnet/api/system.exception?view=net-5.0
     """
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_enum.py` & `psrpcore-0.3.0/src/psrpcore/types/_enum.py`

 * *Files 9% similar despite different names*

```diff
@@ -144,30 +144,30 @@
             return enum.IntFlag._missing_.__func__(cls, value)  # type: ignore[attr-defined]
 
         @classmethod
         def _create_pseudo_member_(cls, value):  # type: ignore[no-untyped-def]
             return enum.IntFlag._create_pseudo_member_.__func__(cls, value)  # type: ignore[attr-defined]
 
     def __or__(self, other):  # type: ignore[no-untyped-def]
-        return enum.IntFlag.__or__(self, other)
+        return enum.IntFlag.__or__(self, other)  # type: ignore[type-var]
 
     def __and__(self, other):  # type: ignore[no-untyped-def]
-        return enum.IntFlag.__and__(self, other)
+        return enum.IntFlag.__and__(self, other)  # type: ignore[type-var]
 
     def __xor__(self, other):  # type: ignore[no-untyped-def]
-        return enum.IntFlag.__xor__(self, other)
+        return enum.IntFlag.__xor__(self, other)  # type: ignore[type-var]
 
     def __ror__(self, other):  # type: ignore[no-untyped-def]
-        return enum.IntFlag.__or__(self, other)
+        return enum.IntFlag.__or__(self, other)  # type: ignore[type-var]
 
     def __rand__(self, other):  # type: ignore[no-untyped-def]
-        return enum.IntFlag.__and__(self, other)
+        return enum.IntFlag.__and__(self, other)  # type: ignore[type-var]
 
     def __rxor__(self, other):  # type: ignore[no-untyped-def]
-        return enum.IntFlag.__xor__(self, other)
+        return enum.IntFlag.__xor__(self, other)  # type: ignore[type-var]
 
     def __invert__(self):  # type: ignore[no-untyped-def]
         return enum.IntFlag.__invert__(self)
 
     def __repr__(self) -> str:
         return enum.IntFlag.__repr__(self)
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_host.py` & `psrpcore-0.3.0/src/psrpcore/types/_host.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,20 @@
 
 @PSType(["System.Management.Automation.Remoting.RemoteHostMethodId"])
 class HostMethodIdentifier(PSEnumBase):
     """Host Method Identifier enum.
 
     This is an enum class for the
     System.Management.Automation.Remoting.RemoteHostMethodId .NET class. It is
-    documented in PSRP under `[MS-PSRP] 2.2.3.17 Host Method Identifier`_.
+    documented in PSRP under
+    `[MS-PSRP] 2.2.3.17 Host Method Identifier <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ddd2a4d1-797d-4d73-8372-7a77a62fb204>`_.
 
     The values are used in :class:`psrpcore.types.RunspacePoolHostCall` and
     :class:`psrpcore.types.PipelineHostCall` to identify what method should be
     invoked.
-
-    .. _[MS-PSRP] 2.2.3.17 Host Method Identifier:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ddd2a4d1-797d-4d73-8372-7a77a62fb204
     """
 
     GetName = 1
     GetVersion = 2
     GetInstanceId = 3
     GetCurrentCulture = 4
     GetCurrentUICulture = 5
@@ -126,25 +124,20 @@
 
 
 @PSType(["System.Management.Automation.Host.ControlKeyStates"])
 class ControlKeyStates(PSFlagBase):
     """System.Management.Automation.Host.ControlKeyStates enum flags.
 
     Defines the state of the control key. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.27 ControlKeyStates`_.
+    `[MS-PSRP] 2.2.3.27 ControlKeyStates <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/bd7241a2-4ba0-4db1-a2b3-77ea1a8a4cbf>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.ControlKeyStates`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.27 ControlKeyStates:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/bd7241a2-4ba0-4db1-a2b3-77ea1a8a4cbf
-
-    .. _System.Management.Automation.Host.ControlKeyStates:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.controlkeystates
+        `System.Management.Automation.Host.ControlKeyStates <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.controlkeystates>`_
+        .NET class.
     """
 
     none = 0  #: No control key state.
     RightAltPressed = 1  #: The right alt key is pressed.
     LeftAltPressed = 2  #: The left alt key is pressed.
     RightCtrlPressed = 4  #: The right ctrl key is pressed.
     LeftCtrlPressed = 8  #: The left ctrl key is pressed.
@@ -158,25 +151,20 @@
 @PSType(["System.Management.Automation.Host.ControlKeyStates"])
 class BufferCellType(PSFlagBase):
     """System.Management.Automation.Host.BufferCellType enum flags.
 
     Defines three types of BufferCells to accommodate for hosts that use up to
     two cells to display a character in some languages such as Chinese and
     Japanese. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.29 BufferCellType`_.
+    `[MS-PSRP] 2.2.3.29 BufferCellType <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/99938ede-6d84-422e-b75d-ace93ea85ea2>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.BufferCellType`_ .NET class.
-
-    .. _[MS-PSRP] 2.2.3.29 BufferCellType:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/99938ede-6d84-422e-b75d-ace93ea85ea2
-
-    .. _System.Management.Automation.Host.BufferCellType:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.buffercelltype
+        `System.Management.Automation.Host.BufferCellType <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.buffercelltype>`_
+        .NET class.
     """
 
     Complete = 0  #: Character occupies one BufferCell.
     Leading = 1  #: Character occupies two BufferCells and this is the leading one.
     Trailing = 2  #: Preceded by a Leading BufferCell.
 
 
@@ -184,18 +172,16 @@
 class ReadKeyOptions(PSFlagBase):
     """System.Management.Automation.Host.ReadKeyOptions enum flags.
 
     Governs the behavior of :class:`HostMethodIdentifier.ReadKey`.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.ReadKeyOptions`_ .NET class.
-
-    .. _System.Management.Automation.Host.ReadKeyOptions:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.readkeyoptions
+        `System.Management.Automation.Host.ReadKeyOptions <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.readkeyoptions>`_
+        .NET class.
     """
 
     AllowCtrlC = 1  #: Allow Ctrl-C to be processed as a keystroke, as opposed to causing a break event.
     NoEcho = 2  #: Do not display the character for the key in the window when pressed.
     IncludeKeyDown = 4  #: Include key down events. One of IncludeKeyDown and IncludeKeyUp or both must be specified.
     IncludeKeyUp = 8  #: Include key up events. One of IncludeKeyDown and IncludeKeyUp or both must be specified.
 
@@ -212,33 +198,29 @@
         PSNoteProperty("BufferCellType", ps_type=BufferCellType),
     ],
 )
 class BufferCell(PSObject):
     """BufferCell.
 
     Represents the contents of a cell of a host's screen buffer. It is
-    documented in PSRP under `[MS-PSRP] 2.2.3.28 BufferCell`_. but the PSRP
-    documentation represents how this value is serialized under
+    documented in PSRP under
+    `[MS-PSRP] 2.2.3.28 BufferCell <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d6270c27-8855-46b6-834c-5a5d188bfe70>`_.
+    but the PSRP documentation represents how this value is serialized under
     host method invocations not the .NET type.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.BufferCell`_ .NET class.
+        `System.Management.Automation.Host.BufferCell <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.buffercell>`_
+        .NET class.
 
     Args:
         Character: Character visible in the cell.
         ForegroundColor: Foreground color.
         BackgroundColor: Background color.
         BufferCellType: Type of the buffer cell.
-
-    .. _[MS-PSRP] 2.2.3.28 BufferCell:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d6270c27-8855-46b6-834c-5a5d188bfe70
-
-    .. _System.Management.Automation.Host.BufferCell:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.buffercell
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -284,22 +266,20 @@
     """ChoiceDescription.
 
     Provides a description of a choice for use by
     :class:`HostMethodIdentifier.PromptForChoice`.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.ChoiceDescription`_ .NET class.
+        `System.Management.Automation.Host.ChoiceDescription <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.choicedescription>`_
+        .NET class.
 
     Args:
         Label: Human friendly message to describe the choice.
         HelpMessage: Help details of the choice.
-
-    .. _System.Management.Automation.Host.ChoiceDescription:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.choicedescription
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -337,30 +317,26 @@
         PSNoteProperty("Y", mandatory=True, ps_type=PSInt),
     ],
 )
 class Coordinates(PSObject):
     """Coordinates
 
     Represents an x,y coordinate pair. It is documented under
-    `[MS-PSRP] 2.2.3.1 Coordinates`_ but the PSRP documentation represents how
-    this value is serialized under :class:`HostDefaultData` not the .NET type.
+    `[MS-PSRP] 2.2.3.1 Coordinates <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/05db8994-ec5c-485c-9e91-3a398e461d38>`_
+    but the PSRP documentation represents how this value is serialized under
+    :class:`HostDefaultData` not the .NET type.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.Coordinates`_ .NET class.
+        `System.Management.Automation.Host.Coordinates <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.coordinates>`_
+        .NET class.
 
     Args:
         X: X coordinate (0 is the leftmost column).
         Y: Y coordinate (0 is the topmost row).
-
-    .. _[MS-PSRP] 2.2.3.1 Coordinates:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/05db8994-ec5c-485c-9e91-3a398e461d38
-
-    .. _System.Management.Automation.Host.Coordinates:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.coordinates
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -406,29 +382,27 @@
     """FieldDescription.
 
     Provides a description of a field for use by
     :class:`HostMethodIdentifier.Prompt`.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.FieldDescription`_ .NET class.
+        `System.Management.Automation.Host.FieldDescription <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.fielddescription>`_
+        .NET class.
 
     Args:
         Name: The name of the field.
         ParameterTypeName: Short name of the field value type.
         ParameterTypeFullName: Full name of the field value type.
         ParameterAssemblyFullName: .NET assembly name of the field value type.
         Label: Human friendly message to describe the field.
         HelpMessage: Help details of the field.
         IsMandatory: The value must be supplied for this field.
         DefaultValue: The default value, if any, for the field.
         Attributes: List of attributes that apply to the field.
-
-    .. _System.Management.Automation.Host.FieldDescription:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.fielddescription
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -482,32 +456,27 @@
         PSNoteProperty("KeyDown", ps_type=PSBool),
     ],
 )
 class KeyInfo(PSObject):
     """KeyInfo.
 
     Represents information of a keystroke. It is documented in PSRP under
-    `[MS-PSRP] 2.2.3.26 KeyInfo`_.
+    `[MS-PSRP] 2.2.3.26 KeyInfo <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/481442e2-5304-4679-b16d-6e53c351339d>`_.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.KeyInfo`_ .NET class.
+        `System.Management.Automation.Host.KeyInfo <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.keyinfo>`_
+        .NET class.
 
     Args:
         VirtualKeyCode: A virtual key code that identifies the given key in a
             device-independent manner.
         Character: Character corresponding to the pressed keys.
         ControlKeyState: State of the control keys.
         KeyDown: True if the event was generated when a key was pressed.
-
-    .. _[MS-PSRP] 2.2.3.26 KeyInfo:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/481442e2-5304-4679-b16d-6e53c351339d
-
-    .. _System.Management.Automation.Host.KeyInfo:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.keyinfo
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -557,24 +526,22 @@
 class Rectangle(PSObject):
     """Rectangle.
 
     Represents a rectangular region of the screen.
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.Rectangle`_ .NET class.
+        `System.Management.Automation.Host.Rectangle <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.rectangle>`_
+        .NET class.
 
     Args:
         Left: Gets and sets the left side of the rectangle.
         Top: Gets and sets the top of the rectangle.
         Right: Gets and sets the right side of the rectangle.
         Bottom: Gets and sets the bottom of the rectanngle.
-
-    .. _System.Management.Automation.Host.Rectangle:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.rectangle
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -614,31 +581,27 @@
         PSNoteProperty("Height", mandatory=True, ps_type=PSInt),
     ],
 )
 class Size(PSObject):
     """Size
 
     Represents a width and height pair. It is documented under
-    `[MS-PSRP] 2.2.3.2 Size`_ but the PSRP documentation represents how this
-    value is serialized under :class:`HostDefaultData` not the .NET type.
+    `[MS-PSRP] 2.2.3.2 Size <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/98cd950f-cc12-4ab4-955d-c389e3089856>`_
+    but the PSRP documentation represents how this value is serialized under
+    :class:`HostDefaultData` not the .NET type.
 
 
     Note:
         This is an auto-generated Python class for the
-        `System.Management.Automation.Host.Size`_ .NET class.
+        `System.Management.Automation.Host.Size <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.size>`_
+        .NET class.
 
     Args:
         Width: The width of an area.
         Height: The height of an area.
-
-    .. _[MS-PSRP] 2.2.3.2 Size:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/98cd950f-cc12-4ab4-955d-c389e3089856
-
-    .. _System.Management.Automation.Host.Size:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.host.size
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -683,15 +646,16 @@
 )
 class HostDefaultData(PSObject):
     """HostInfo default data.
 
     This defines the default data for a PSHost when creating a RunspacePool or
     Pipeline. This does not represent an actual .NET type but is an internal
     object representation used by PSRP itself. This type represents the
-    `hostDefaultData` property documented at `[MS-PSRP] 2.2.3.14 HostInfo`_.
+    `hostDefaultData` property documented at
+    `[MS-PSRP] 2.2.3.14 HostInfo <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/510fd8f3-e3ac-45b4-b622-0ad5508a5ac6>`_.
 
     Args:
         ForegroundColor: Color of the character on the screen buffer.
         BackgroundColor: Color behind characters on the screen buffer.
         CursorPosition: Cursor position in the screen buffer.
         WindowPosition: Position of the view window relative to the screen
             buffer.
@@ -700,17 +664,14 @@
             cells.
         WindowSize: Current view window size, measured in character cells.
         MaxWindowSize:  Size of the largest window position for the current
             buffer.
         MaxPhysicalWindowSize: Largest window possible ignoring the current
             buffer dimensions.
         WindowTitle: The titlebar text of the current view window.
-
-    .. _[MS-PSRP] 2.2.3.14 HostInfo:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/510fd8f3-e3ac-45b4-b622-0ad5508a5ac6
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -776,29 +737,26 @@
     ],
     skip_inheritance=True,
 )
 class HostInfo(PSObject):
     """HostInfo.
 
     Defines the PSHost information. Message is defined in
-    `[MS-PSRP] 2.2.3.14 HostInfo`_.
+    `[MS-PSRP] 2.2.3.14 HostInfo <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/510fd8f3-e3ac-45b4-b622-0ad5508a5ac6>`_.
 
     Args:
         IsHostNull: Whether there is a PSHost ``False`` or not ``True``.
         IsHostUINull: Whether the PSHost implements the `UI` implementation
             methods ``False`` or not ``True``.
         IsHostRawUINull: Whether the PSHost UI implements the ``RawUI``
             implementation methods ``False`` or not ``True``.
         UseRunspaceHost: When creating a pipeline, set this to ``True`` to get
             it to use the associated RunspacePool host.
         HostDefaultData: Host default data associated with the PSHost
             implementation. Can be ``None`` if not implemented.
-
-    .. _[MS-PSRP] 2.2.3.14 HostInfo:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/510fd8f3-e3ac-45b4-b622-0ad5508a5ac6
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_primitive.py` & `psrpcore-0.3.0/src/psrpcore/types/_primitive.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,17 @@
 
 """PSRP/.NET Primitive Types.
 
 The PSRP/.NET Primitive Type class definitions. A primitive type is a
 fundamental type, like strings, ints, etc, that typically only represent a
 single value. Some of the lines are blurred with certain types but the ones
 defined here are what is documented under
-`MS-PSRP 2.2.5.1 Serialization of Primitive Type Objects`_ with the exception
-of the Progress and Information records which are complex types.
-
-.. _MS-PSRP 2.2.5.1 Serialization of Primitive Type Objects:
-    https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c8c85974-ffd7-4455-84a8-e49016c20683
+`MS-PSRP 2.2.5.1 Serialization of Primitive Type Objects <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c8c85974-ffd7-4455-84a8-e49016c20683>`_
+with the exception of the Progress and Information records which are complex
+types.
 """
 
 import base64
 import datetime
 import decimal
 import enum
 import operator
@@ -231,55 +229,43 @@
 
     This is the string primitive type which represents the following types:
 
         Python: :class:`str`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.1 String`_
-
-        .NET: `System.String`_
+        PSRP: `[MS-PSRP] 2.2.5.1.1 String <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/052b8c32-735b-49c0-8c24-bb32a5c871ce>`_
 
-    .. _[MS-PSRP] 2.2.5.1.1 String:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/052b8c32-735b-49c0-8c24-bb32a5c871ce
-
-    .. _System.String:
-        https://docs.microsoft.com/en-us/dotnet/api/system.string?view=net-5.0
+        .NET: `System.String <https://docs.microsoft.com/en-us/dotnet/api/system.string?view=net-5.0>`_
     """
 
 
 @PSType(["System.Char", "System.ValueType"], tag="C")
 class PSChar(PSObject, int):
     """The Char primitive type.
 
     This is the char primitive type which represents the following types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.2 Character`_
+        PSRP: `[MS-PSRP] 2.2.5.1.2 Character <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ff6f9767-a0a5-4cca-b091-4f15afc6e6d8>`_
 
-        .NET: `System.Char`_
+        .NET: `System.Char <https://docs.microsoft.com/en-us/dotnet/api/system.char?view=net-5.0>`_
 
     A char in .NET represents a UTF-16 codepoint from `u0000` to `uFFFF`.
     The codepoint may represent an invalid unicode character, say it's 1 half
     of a surrogate pair, but it's still a valid Char. A PSChar can be
     initialized just like an `int()` as long as the value is from `0` to
     `65535` inclusive. A PSChar can also be initialized from a single string
     character like `PSChar('a')`, any byte strings will be encoded as UTF-8
     when getting the character. If a decimal value is used as a string then the
     PSChar instance will be the value of that codepoint of the character and
     not the decimal value itself.
-
-    .. _[MS-PSRP] 2.2.5.1.2 Character:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ff6f9767-a0a5-4cca-b091-4f15afc6e6d8
-
-    .. _System.Char:
-        https://docs.microsoft.com/en-us/dotnet/api/system.char?view=net-5.0
     """
 
     def __new__(cls, *args: typing.Any, **kwargs: typing.Any) -> "PSChar":
         raw_args = list(args)
 
         if isinstance(raw_args[0], bytes):
             raw_args[0] = raw_args[0].decode("utf-8")
@@ -314,54 +300,41 @@
 
 This is the bool primitive type which represents the following types:
 
     Python: :class:`bool`
 
     Native Serialization: yes
 
-    PSRP: `[MS-PSRP] 2.2.5.1.3 Boolean`_
+    PSRP: `[MS-PSRP] 2.2.5.1.3 Boolean <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/8b4b1067-4b58-46d5-b1c9-b881b6e7a0aa>`_
 
-    .NET: `System.Boolean`_
+    .NET: `System.Boolean <https://docs.microsoft.com/en-us/dotnet/api/system.boolean?view=net-5.0>`_
 
 Cannot subclass bool due to a limitation on Python. This unfortunately means
 we can't represent an extended primitive object of this type in Python as well.
-
-.. _[MS-PSRP] 2.2.5.1.3 Boolean:
-    https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/8b4b1067-4b58-46d5-b1c9-b881b6e7a0aa
-
-.. _System.Boolean:
-    https://docs.microsoft.com/en-us/dotnet/api/system.boolean?view=net-5.0
 """
 
 
 @PSType(["System.DateTime", "System.ValueType"], tag="DT")
 class PSDateTime(PSObject, datetime.datetime):
     """The Date/Time primitive type.
 
     This is the datetime primitive type which represents the following types:
 
         Python: obj:`datetime.datetime`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.4 Date/Time`_
-
-        .NET: `System.DateTime`_
+        PSRP: `[MS-PSRP] 2.2.5.1.4 Date/Time <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/a3b75b8d-ad7e-4649-bb82-cfa70f54fb8c>`_
 
+        .NET: `System.DateTime <https://docs.microsoft.com/en-us/dotnet/api/system.datetime?view=net-5.0>`_
 
     This extends the Python datetime.datetime class and adds a `nanosecond`
     attribute to track the nanoseconds. While the class can have a nanosecond
     precision, a serialized DateTime object can only go up to a .NET Tick which
     is 100s of nanoseconds.
-
-    .. _[MS-PSRP] 2.2.5.1.4 Date/Time:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/a3b75b8d-ad7e-4649-bb82-cfa70f54fb8c
-
-    .. _System.DateTime:
-        https://docs.microsoft.com/en-us/dotnet/api/system.datetime?view=net-5.0
     """
 
     def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
         super().__init__()
         self.nanosecond = getattr(self, "nanosecond", None) or 0
 
     def __new__(cls, *args: typing.Any, **kwargs: typing.Any) -> "PSDateTime":
@@ -459,28 +432,22 @@
 
     This is the duration primitive type which represents the following types:
 
         Python: :class:`datetime.timedelta`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.5 Duration`_
+        PSRP: `[MS-PSRP] 2.2.5.1.5 Duration <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/434cd15d-8fb3-462c-a004-bcd0d3a60201>`_
 
-        .NET: `System.TimeSpan`_
+        .NET: `System.TimeSpan <https://docs.microsoft.com/en-us/dotnet/api/system.timespan?view=net-5.0>`_
 
     This extends the Python datetime.timespan class and adds a `nanoseconds`
     attribute to track the nanoseconds. While the class can have a nanosecond
     precision, a serialized Duration object can only go up to a .NET Tick which
     is 100s of nanoseconds.
-
-    .. _[MS-PSRP] 2.2.5.1.5 Duration:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/434cd15d-8fb3-462c-a004-bcd0d3a60201
-
-    .. _System.TimeSpan:
-        https://docs.microsoft.com/en-us/dotnet/api/system.timespan?view=net-5.0
     """
 
     def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
         super().__init__()
         self.nanoseconds = getattr(self, "nanoseconds", None) or 0
 
     def __new__(cls, *args: typing.Any, **kwargs: typing.Any) -> "PSDuration":
@@ -622,26 +589,20 @@
     This is the unsigned byte primitive type which represents the following
     types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.6 Unsigned Byte`_
+        PSRP: `[MS-PSRP] 2.2.5.1.6 Unsigned Byte <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/6e25153d-77b6-4e21-b5fa-6f986895171a>`_
 
-        .NET: `System.Byte`_
+        .NET: `System.Byte <https://docs.microsoft.com/en-us/dotnet/api/system.byte?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between 0 and 255 like a Byte on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.6 Unsigned Byte:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/6e25153d-77b6-4e21-b5fa-6f986895171a
-
-    .. _System.Byte:
-        https://docs.microsoft.com/en-us/dotnet/api/system.byte?view=net-5.0
     """
 
     MinValue = 0
     MaxValue = 255
 
 
 @PSType(["System.SByte", "System.ValueType"], tag="SB")
@@ -651,26 +612,20 @@
     This is the signed byte primitive type which represents the following
     types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.7 Signed Byte`_
+        PSRP: `[MS-PSRP] 2.2.5.1.7 Signed Byte <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/8046c418-1531-4c43-9b9d-fb9bceace0db>`_
 
-        .NET: `System.SByte`_
+        .NET: `System.SByte <https://docs.microsoft.com/en-us/dotnet/api/system.sbyte?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between -128 and 127 like an SByte on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.7 Signed Byte:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/8046c418-1531-4c43-9b9d-fb9bceace0db
-
-    .. _System.SByte:
-        https://docs.microsoft.com/en-us/dotnet/api/system.sbyte?view=net-5.0
     """
 
     MinValue = -128
     MaxValue = 127
 
 
 @PSType(["System.UInt16", "System.ValueType"], tag="U16")
@@ -680,26 +635,20 @@
     This is the unsigned short primitive type which represents the following
     types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.8 Unsigned Short`_
+        PSRP: `[MS-PSRP] 2.2.5.1.8 Unsigned Short <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/33751ca7-90d0-4b5e-a04f-2d8798cfb419>`_
 
-        .NET: `System.UInt16`_
+        .NET: `System.UInt16 <https://docs.microsoft.com/en-us/dotnet/api/system.uint16?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between 0 and 65535 like a UInt16 on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.8 Unsigned Short:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/33751ca7-90d0-4b5e-a04f-2d8798cfb419
-
-    .. _System.UInt16:
-        https://docs.microsoft.com/en-us/dotnet/api/system.uint16?view=net-5.0
     """
 
     MinValue = 0
     MaxValue = 65535
 
 
 @PSType(["System.Int16", "System.ValueType"], tag="I16")
@@ -709,26 +658,20 @@
     This is the signed short primitive type which represents the following
     types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.9 Signed Short`_
+        PSRP: `[MS-PSRP] 2.2.5.1.9 Signed Short <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e0ed596d-0aea-40bb-a254-285b71188214>`_
 
-        .NET: `System.Int16`_
+        .NET: `System.Int16 <https://docs.microsoft.com/en-us/dotnet/api/system.int16?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between -32768 and 32767 like an Int16 on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.9 Signed Short:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e0ed596d-0aea-40bb-a254-285b71188214
-
-    .. _System.Int16:
-        https://docs.microsoft.com/en-us/dotnet/api/system.int16?view=net-5.0
     """
 
     MinValue = -32768
     MaxValue = 32767
 
 
 @PSType(["System.UInt32", "System.ValueType"], tag="U32")
@@ -738,26 +681,20 @@
     This is the unsigned integer primitive type which represents the following
     types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.10 Unsigned Int`_
+        PSRP: `[MS-PSRP] 2.2.5.1.10 Unsigned Int <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/7b904471-3519-4a6a-900b-8053ad975c08>`_
 
-        .NET: `System.UInt32`_
+        .NET: `System.UInt32 <https://docs.microsoft.com/en-us/dotnet/api/system.uint32?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between 0 and 4294967295 like a UInt32 on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.10 Unsigned Int:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/7b904471-3519-4a6a-900b-8053ad975c08
-
-    .. _System.UInt32:
-        https://docs.microsoft.com/en-us/dotnet/api/system.uint32?view=net-5.0
     """
 
     MinValue = 0
     MaxValue = 4294967295
 
 
 @PSType(["System.Int32", "System.ValueType"], tag="I32")
@@ -766,26 +703,20 @@
 
     This is the signed int primitive type which represents the following types:
 
         Python: :class:`int`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.11 Signed Int`_
+        PSRP: `[MS-PSRP] 2.2.5.1.11 Signed Int <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9eef96ba-1876-427b-9450-75a1b28f5668>`_
 
-        .NET: `System.Int32`_
+        .NET: `System.Int32 <https://docs.microsoft.com/en-us/dotnet/api/system.int32?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between -2147483648 and 2147483647 like an Int32 on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.11 Signed Int:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9eef96ba-1876-427b-9450-75a1b28f5668
-
-    .. _System.Int32:
-        https://docs.microsoft.com/en-us/dotnet/api/system.int32?view=net-5.0
     """
 
     MinValue = -2147483648
     MaxValue = 2147483647
 
 
 @PSType(["System.UInt64", "System.ValueType"], tag="U64")
@@ -795,26 +726,20 @@
     This is the unsigned long primitive type which represents the following
     types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.12 Unsigned Long`_
+        PSRP: `[MS-PSRP] 2.2.5.1.12 Unsigned Long <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d92cd5d2-59c6-4a61-b517-9fc48823cb4d>`_
 
-        .NET: `System.UInt64`_
+        .NET: `System.UInt64 <https://docs.microsoft.com/en-us/dotnet/api/system.uint64?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between 0 and 18446744073709551615 like a UInt64 on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.12 Unsigned Long:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d92cd5d2-59c6-4a61-b517-9fc48823cb4d
-
-    .. _System.UInt64:
-        https://docs.microsoft.com/en-us/dotnet/api/system.uint64?view=net-5.0
     """
 
     MinValue = 0
     MaxValue = 18446744073709551615
 
 
 @PSType(["System.Int64", "System.ValueType"], tag="I64")
@@ -824,26 +749,20 @@
     This is the signed long primitive type which represents the following
     types:
 
         Python: :class:`int`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.13 Signed Long`_
+        PSRP: `[MS-PSRP] 2.2.5.1.13 Signed Long <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/de124e86-3f8c-426a-ab75-47fdb4597c62>`_
 
-        .NET: `System.Int64`_
+        .NET: `System.Int64 <https://docs.microsoft.com/en-us/dotnet/api/system.int64?view=net-5.0>`_
 
     While this represents an int in Python it is artificially limited to values
     between -9223372036854775808 and 9223372036854775807 like an Int64 on .NET.
-
-    .. _[MS-PSRP] 2.2.5.1.13 Signed Long:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/de124e86-3f8c-426a-ab75-47fdb4597c62
-
-    .. _System.Int64:
-        https://docs.microsoft.com/en-us/dotnet/api/system.int64?view=net-5.0
     """
 
     MinValue = -9223372036854775808
     MaxValue = 9223372036854775807
 
 
 @PSType(["System.Single", "System.ValueType"], tag="Sg")
@@ -852,23 +771,17 @@
 
     This is the single primitive type which represents the following types:
 
         Python: :class:`float`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.14 Float`_
+        PSRP: `[MS-PSRP] 2.2.5.1.14 Float <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d8a5a9ab-5f52-4175-96a3-c29afb7b82b8>`_
 
-        .NET: `System.Single`_
-
-    .. _[MS-PSRP] 2.2.5.1.14 Float:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d8a5a9ab-5f52-4175-96a3-c29afb7b82b8
-
-    .. _System.Single:
-        https://docs.microsoft.com/en-us/dotnet/api/system.single?view=net-5.0
+        .NET: `System.Single <https://docs.microsoft.com/en-us/dotnet/api/system.single?view=net-5.0>`_
     """
 
     def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
         super().__init__()
 
     def __repr__(self) -> str:
         return float.__repr__(self)
@@ -883,23 +796,17 @@
 
     This is the double primitive type which represents the following types:
 
         Python: :class:`float`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.15 Double`_
-
-        .NET: `System.Single`_
+        PSRP: `[MS-PSRP] 2.2.5.1.15 Double <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/02fa08c5-139c-4e98-a13e-45784b4eabde>`_
 
-    .. _[MS-PSRP] 2.2.5.1.15 Double:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/02fa08c5-139c-4e98-a13e-45784b4eabde
-
-    .. _System.Double:
-        https://docs.microsoft.com/en-us/dotnet/api/system.double?view=net-5.0
+        .NET: `System.Double <https://docs.microsoft.com/en-us/dotnet/api/system.double?view=net-5.0>`_
     """
 
     def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
         super().__init__()
 
     def __repr__(self) -> str:
         return float.__repr__(self)
@@ -914,23 +821,17 @@
 
     This is the decimal primitive type which represents the following types:
 
         Python: :class:`decimal.Decimal`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.16 Decimal`_
-
-        .NET: `System.Decimal`_
-
-    .. _[MS-PSRP] 2.2.5.1.16 Decimal:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/0f760f90-fa46-49bd-8868-001e2c29eb50
+        PSRP: `[MS-PSRP] 2.2.5.1.16 Decimal <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/0f760f90-fa46-49bd-8868-001e2c29eb50>`_
 
-    .. _System.Decimal:
-        https://docs.microsoft.com/en-us/dotnet/api/system.decimal?view=net-5.0
+        .NET: `System.Decimal <https://docs.microsoft.com/en-us/dotnet/api/system.decimal?view=net-5.0>`_
     """
 
     def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
         super().__init__()
 
     def __repr__(self) -> str:
         return decimal.Decimal.__repr__(self)
@@ -945,20 +846,17 @@
 
     This is the byte array primitive type which represents the following types:
 
         Python: :class:`bytes`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.17 Array of Bytes`_
+        PSRP: `[MS-PSRP] 2.2.5.1.17 Array of Bytes <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/489ed886-34d2-4306-a2f5-73843c219b14>`_
 
         .NET: System.Byte[]
-
-    .. _[MS-PSRP] 2.2.5.1.17 Array of Bytes:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/489ed886-34d2-4306-a2f5-73843c219b14
     """
 
     def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
         super().__init__()
 
     def __getitem__(  # type: ignore[override]  # The __mro__ is confusing mypy
         self,
@@ -985,23 +883,17 @@
 
     This is the GUID/UUID primitive type which represents the following types:
 
         Python: :class:`uuid.UUID`
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.18 GUID`_
-
-        .NET: `System.Guid`_
-
-    .. _[MS-PSRP] 2.2.5.1.18 GUID:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c30c37fa-692d-49c7-bb86-b3179a97e106
+        PSRP: `[MS-PSRP] 2.2.5.1.18 GUID <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c30c37fa-692d-49c7-bb86-b3179a97e106>`_
 
-    .. _System.Guid:
-        https://docs.microsoft.com/en-us/dotnet/api/system.guid?view=net-5.0
+        .NET: `System.Guid <https://docs.microsoft.com/en-us/dotnet/api/system.guid?view=net-5.0>`_
     """
 
     def __new__(cls, *args: typing.Any, **kwargs: typing.Any) -> "PSGuid":
         return super().__new__(cls)
 
     def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
         super().__init__()
@@ -1042,63 +934,54 @@
 
     This is the URI primitive type which represents the following types:
 
         Python: :class:`str`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.19 URI`_
+        PSRP: `[MS-PSRP] 2.2.5.1.19 URI <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4ac73ac2-5cf7-4669-b4de-c8ba19a13186>`_
 
-        .NET: `System.Uri`_
+        .NET: `System.Uri <https://docs.microsoft.com/en-us/dotnet/api/system.uri?view=net-5.0>`_
 
     While the primitive type represents a URI, this is merely a URI as a string
     in Python. You will need need to use a separate function to parse this URI
     like :func:`urllib.parse.urlparse`.
-
-    .. _[MS-PSRP] 2.2.5.1.19 URI:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4ac73ac2-5cf7-4669-b4de-c8ba19a13186
-
-    .. _System.Uri:
-        https://docs.microsoft.com/en-us/dotnet/api/system.uri?view=net-5.0
     """
 
 
 PSNull = None
 """The Null Value primitive type.
 
 This is the Null Value primitive type which represents the following types:
 
     Python: None
 
     Native Serialization: yes
 
-    PSRP: `[MS-PSRP] 2.2.5.1.20 Null Value`_
+    PSRP: `[MS-PSRP] 2.2.5.1.20 Null Value <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/402f2a78-5771-45ae-bf33-59f6e57767ca>`_
 
     .NET: null/$null
 
 This isn't a type but rather just a placeholder for `None` in PSRP.
-
-.. _[MS-PSRP] 2.2.5.1.20 Null Value:
-    https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/402f2a78-5771-45ae-bf33-59f6e57767ca
 """
 
 
 @PSType(["System.Version"], tag="Version")
 class PSVersion(PSObject):
     """The Version primitive type.
 
     This is the Version primitive type which represents the following types:
 
         Python: N/A
 
         Native Serialization: yes
 
-        PSRP: `[MS-PSRP] 2.2.5.1.21 Version`_
+        PSRP: `[MS-PSRP] 2.2.5.1.21 Version <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/390db910-e035-4f97-80fd-181a008ff6f8>`_
 
-        .NET: `System.Version`_
+        .NET: `System.Version <https://docs.microsoft.com/en-us/dotnet/api/system.version?view=net-5.0>`_
 
     This is a custom implementation of a basic Version structure that matches
     the .NET System.Version class. A valid .NET Version must have the major and
     minor values defined as an integer and the build and revision are optional
     integer values.
 
     This class is able to sort multiple PSVersions but not with other Python
@@ -1113,20 +996,14 @@
         revision: The optional revision when not using version_str.
 
     Attributes:
         major (:class:`int`): See parameters.
         minor (:class:`int`): See parameters.
         build (:class:`int`, optional): See parameters.
         revision (:class:`int`, optional): See parameters.
-
-    .. _[MS-PSRP] 2.2.5.1.21 Version:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/390db910-e035-4f97-80fd-181a008ff6f8
-
-    .. _System.Version:
-        https://docs.microsoft.com/en-us/dotnet/api/system.version?view=net-5.0
     """
 
     def __init__(
         self,
         version_str: typing.Optional[str] = None,
         major: typing.Optional[int] = None,
         minor: typing.Optional[int] = None,
@@ -1243,72 +1120,60 @@
     This is the XML Document primitive type which represents the following
     types:
 
         Python: :class:`str`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.22 XML Document`_
+        PSRP: `[MS-PSRP] 2.2.5.1.22 XML Document <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/df5908ab-bb4d-45e4-8adc-7258e5a9f537>`_
 
-        .NET: `System.Xml.XmlDocument`_
+        .NET: `System.Xml.XmlDocument <https://docs.microsoft.com/en-us/dotnet/api/system.xml.xmldocument?view=net-5.0>`_
 
     While the primitive type represents an XML Document, this is merely an XML
     value as a string in Python. You will still need to use an XML library to
     parse the value.
-
-    .. _[MS-PSRP] 2.2.5.1.22 XML Document:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/df5908ab-bb4d-45e4-8adc-7258e5a9f537
-
-    .. _System.Xml.XmlDocument:
-        https://docs.microsoft.com/en-us/dotnet/api/system.xml.xmldocument?view=net-5.0
     """
 
 
 @PSType(["System.Management.Automation.ScriptBlock"], tag="SBK")
 class PSScriptBlock(PSStringBase):
     """The ScriptBlock primitive type.
 
     This is the PowerShell ScriptBlock primitive type which represents the
     following types:
 
         Python: :class:`str`
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.23 ScriptBlock`_
+        PSRP: `[MS-PSRP] 2.2.5.1.23 ScriptBlock <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/306af1be-6be5-4074-acc9-e29bd32f3206>`_
 
-        .NET: `System.Management.Automation.ScriptBlock`_
+        .NET: `System.Management.Automation.ScriptBlock <https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.scriptblock?view=powershellsdk-7.0.0>`_
 
     While the primitive type represents a ScriptBlock in PowerShell there are
     some limitations when it comes to sending a scriptblock over a remote
     PSSession. The PSRP server will automatically convert the instance to a
     string so this type is mostly useless.
-
-    .. _[MS-PSRP] 2.2.5.1.23 ScriptBlock:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/306af1be-6be5-4074-acc9-e29bd32f3206
-
-    .. _System.Management.Automation.ScriptBlock:
-        https://docs.microsoft.com/en-us/dotnet/api/system.management.automation.scriptblock?view=powershellsdk-7.0.0
     """
 
 
 @PSType(["System.Security.SecureString"], tag="SS")
 class PSSecureString(PSObject):
     """The Secure String primitive type.
 
     This is the PowerShell secure string primitive type which represents the
     following types:
 
         Python: N/A
 
         Native Serialization: no
 
-        PSRP: `[MS-PSRP] 2.2.5.1.24 Secure String`_
+        PSRP: `[MS-PSRP] 2.2.5.1.24 Secure String <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/69b9dc01-a843-4f91-89f8-0205f021a7dd>`_
 
-        .NET: `System.Security.SecureString`_
+        .NET: `System.Security.SecureString <https://docs.microsoft.com/en-us/dotnet/api/system.security.securestring?view=net-5.0>`_
 
     It is designed to mark a string as a secure string which will be encrypted
     as it is serialized. The plaintext value can be retrieved using the
     :meth:`PSSecureString.decrypt` function.
 
     Note:
         Before a `PSSecureString` can be created or decrypted from the peer,
@@ -1324,20 +1189,14 @@
     Args:
         value: The plaintext value to encrypt (when `cipher` is `None`) or the
             encrypted value (when `cipher` is not `None`).
         cipher: The :class:`PSCryptoProvider` cipher used to encrypt or decrypt
             the secure string. If omitted then the `value` specified is
             treated as the plaintext and will be encrypted during
             serialization.
-
-    .. _[MS-PSRP] 2.2.5.1.24 Secure String:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/69b9dc01-a843-4f91-89f8-0205f021a7dd
-
-    .. _System.Security.SecureString:
-        https://docs.microsoft.com/en-us/dotnet/api/system.security.securestring?view=net-5.0
     """
 
     def __init__(
         self,
         value: str,
         cipher: typing.Optional[PSCryptoProvider] = None,
     ) -> None:
@@ -1345,17 +1204,15 @@
         self._value: str = value
         self._cipher = cipher
         self._encrypted = cipher is not None
 
     def decrypt(self) -> PSString:
         """Decrypts a PSSecureString into the plaintext string."""
         if self._cipher:
-            b_enc = base64.b64decode(self._value)
-            b_dec = self._cipher.decrypt(b_enc)
-            raw = b_dec.decode("utf-16-le", errors="surrogatepass")
+            raw = self._cipher.decrypt(self._value)
 
         else:
             raw = self._value
 
         dec_str = PSString(raw)
         dec_str.PSObject = self.PSObject
         return dec_str
@@ -1372,15 +1229,11 @@
         instance: "PSSecureString",
         cipher: PSCryptoProvider,
         **kwargs: typing.Any,
     ) -> PSObject:
         if not instance._encrypted:
             # The value was provided by the user without a cipher. Use the one passed in by the serializer to encrypt
             # the value and return that for serialization.
-            b_value = instance._value.encode("utf-16-le", errors="surrogatepass")
-            b_enc = cipher.encrypt(b_value)
-            enc_value = base64.b64encode(b_enc).decode()
-
-            return cls(enc_value, cipher)
+            return cls(cipher.encrypt(instance._value), cipher)
 
         else:
             return instance
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_psrp.py` & `psrpcore-0.3.0/src/psrpcore/types/_psrp.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,29 +123,23 @@
         PSNoteProperty("TimeZone", ps_type=PSByteArray),
     ],
 )
 class SessionCapability(PSObject):
     """SESSION_CAPABILITY Message.
 
     Defines the session capability and protocol versions. Message is defined in
-    `MS-PSRP 2.2.2.1 SESSION_CAPABILITY`_. The TimeZone property is a .NET type
-    serialized to bytes as defined by
-    `MS-PSRP 2.2.3.10.1 CurrentSystemTimeZone`_.
+    `MS-PSRP 2.2.2.1 SESSION_CAPABILITY <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2f41abfb-7e30-4fb1-b286-527e9d67ad30>`_.
+    The TimeZone property is a .NET type serialized to bytes as defined by
+    `MS-PSRP 2.2.3.10.1 CurrentSystemTimeZone <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/5e6263c5-358a-459b-a49e-0707e383eb55>`_.
 
     Args:
         PSVersion: The version of the higher-layer application.
         protocolversion: The version of the PowerShell Remoting Protocol.
         SerializationVersion: The version of the serialization system.
         TimeZone: The time zone of the client.
-
-    .. _MS-PSRP 2.2.2.1 SESSION_CAPABILITY:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2f41abfb-7e30-4fb1-b286-527e9d67ad30
-
-    .. _MS-PSRP 2.2.3.10.1 CurrentSystemTimeZone:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/5e6263c5-358a-459b-a49e-0707e383eb55
     """
 
     @classmethod
     def ToPSObjectForRemoting(
         cls,
         instance: "SessionCapability",
         **kwargs: typing.Any,
@@ -172,48 +166,42 @@
         PSNoteProperty("ApplicationArguments", mandatory=True, ps_type=PSPrimitiveDictionary),
     ],
 )
 class InitRunspacePool(PSObject):
     """INIT_RUNSPACEPOOL Message.
 
     Defines the Runspace Pool initialization data. Message is defined in
-    `MS-PSRP 2.2.2.2 INIT_RUNSPACEPOOL`_.
+    `MS-PSRP 2.2.2.2 INIT_RUNSPACEPOOL <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c867589a-0b43-47bd-9abf-7477699ff6c9>`_.
 
     Args:
         MinRunspaces: The minimum number of runspaces in the Runspace Pool.
         MaxRunspaces: The maximum number of runspaces in the Runspace Pool.
         PSThreadOptions: Thread options provided by the higher layer.
         ApartmentState: Apart state provided by the higher layer.
         HostInfo: Host information.
         ApplicationArguments: Application arguments provided by the higher
             layer.
-
-    .. _MS-PSRP 2.2.2.2 INIT_RUNSPACEPOOL:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c867589a-0b43-47bd-9abf-7477699ff6c9
-
     """
 
 
 @PSMessageType(
     PSRPMessageType.PublicKey,
     extended_properties=[
         PSNoteProperty("PublicKey", mandatory=True, ps_type=PSString),
     ],
 )
 class PublicKey(PSObject):
     """PUBLIC_KEY Message.
 
     Defines the public key created by the client used in the session key
-    exchange. Message is defined in `MS-PSRP 2.2.2.3 - PUBLIC_KEY`_.
+    exchange. Message is defined in
+    `MS-PSRP 2.2.2.3 - PUBLIC_KEY <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/3efa4b90-c089-432b-91db-76a3deb175bc>`_.
 
     Args:
         PublicKey: The base64 encoding of the PKCS1 formatted public key.
-
-    .. _MS-PSRP 2.2.2.3 - PUBLIC_KEY:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/3efa4b90-c089-432b-91db-76a3deb175bc
     """
 
 
 @PSMessageType(
     PSRPMessageType.EncryptedSessionKey,
     extended_properties=[
         PSNoteProperty("EncryptedSessionKey", mandatory=True, ps_type=PSString),
@@ -221,83 +209,71 @@
 )
 class EncryptedSessionKey(PSObject):
     """ENCRYPTED_SESSION_KEY Message.
 
     Defines the encrypted session key calculated by the server. The value is
     encrypted using the public key that was sent by the client in the
     :class:`PublicKey` message. Message is defined in
-    `MS-PSRP 2.2.2.4 - ENCRYPTED_SESSION_KEY`_.
+    `MS-PSRP 2.2.2.4 - ENCRYPTED_SESSION_KEY <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e3e155af-b379-40cf-80c0-14a124145147>`_.
 
     Note:
         The session key is encrypted using the RSAES-PKCS-v1_5 encryption
         scheme.
 
     Args:
         EncryptedSessionKey: The base64 encoding of the 256-bit AES encrypted
             session key.
-
-    .. _MS-PSRP 2.2.2.4 - ENCRYPTED_SESSION_KEY:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e3e155af-b379-40cf-80c0-14a124145147
     """
 
 
 @PSMessageType(PSRPMessageType.PublicKeyRequest)
 class PublicKeyRequest(PSStringBase):
     """PUBLIC_KEY_REQUEST Message.
 
     This is a message that the server sends the client when it wants to start
     the encryption key exchange. Message is defined in
-    `MS-PSRP 2.2.2.5 - PUBLIC_KEY_REQUEST`_.
-
-    .. _MS-PSRP 2.2.2.5 - PUBLIC_KEY_REQUEST:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9ff2857d-a7cb-4da6-81f1-65d08b3dbe63
+    `MS-PSRP 2.2.2.5 - PUBLIC_KEY_REQUEST <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9ff2857d-a7cb-4da6-81f1-65d08b3dbe63>`_.
     """
 
 
 @PSMessageType(
     PSRPMessageType.SetMaxRunspaces,
     extended_properties=[
         PSNoteProperty("MaxRunspaces", mandatory=True, ps_type=PSInt),
         PSNoteProperty("ci", mandatory=True, ps_type=PSInt64),
     ],
 )
 class SetMaxRunspaces(PSObject):
     """SET_MAX_RUNSPACES Message.
 
     Set maximum runspaces in a RunspacePool. Message is defined in
-    `MS-PSRP 2.2.2.6 - SET_MAX_RUNSPACES`_.
+    `MS-PSRP 2.2.2.6 - SET_MAX_RUNSPACES <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/92037046-043a-4962-8e7e-2d457249548b>`_.
 
     Args:
         MaxRunspaces: The maximum runspaces in a pool.
         ci: The Call ID the message is related to.
-
-    .. _MS-PSRP 2.2.2.6 - SET_MAX_RUNSPACES:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/92037046-043a-4962-8e7e-2d457249548b
     """
 
 
 @PSMessageType(
     PSRPMessageType.SetMinRunspaces,
     extended_properties=[
         PSNoteProperty("MinRunspaces", mandatory=True, ps_type=PSInt),
         PSNoteProperty("ci", mandatory=True, ps_type=PSInt64),
     ],
 )
 class SetMinRunspaces(PSObject):
     """SET_MIN_RUNSPACES Message.
 
     Set minimum runspaces in a RunspacePool. Message is defined in
-    `MS-PSRP 2.2.2.7 - SET_MIN_RUNSPACES`_.
+    `MS-PSRP 2.2.2.7 - SET_MIN_RUNSPACES <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2d425c82-ead1-4888-911a-b11f545ca441>`_.
 
     Args:
         MinRunspaces: The minimum runspaces in a pool.
         ci: The Call ID the message is related to.
-
-    .. _MS-PSRP 2.2.2.7 - SET_MIN_RUNSPACES:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2d425c82-ead1-4888-911a-b11f545ca441
     """
 
 
 @PSMessageType(
     PSRPMessageType.RunspaceAvailability,
     extended_properties=[
         PSNoteProperty("SetMinMaxRunspacesResponse", mandatory=True),
@@ -305,47 +281,42 @@
     ],
 )
 class RunspaceAvailability(PSObject):
     """RUNSPACE_AVAILABILITY Message.
 
     A response to either set maximum runspaces or set minimum runspaces in a
     RunspacePool or request for available runspaces in a RunspacePool. Message
-    is defined in `MS-PSRP 2.2.2.8 - RUNSPACE_AVAILABILITY`_.
+    is defined in
+    `MS-PSRP 2.2.2.8 - RUNSPACE_AVAILABILITY <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/bcab75d9-31a8-4fdc-a8c4-00f41e5985d2>`_.
 
     Args:
         SetMinMaxRunspacesResponse: A :class:`PSBool` for a set min/max response
             or a :class:`PSInt64` for a get available response.
         ci: The Call ID the message is related to.
-
-    .. _MS-PSRP 2.2.2.8 - RUNSPACE_AVAILABILITY:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/bcab75d9-31a8-4fdc-a8c4-00f41e5985d2
     """
 
 
 @PSMessageType(
     PSRPMessageType.RunspacePoolState,
     extended_properties=[
         PSNoteProperty("RunspaceState", mandatory=True, ps_type=PSInt),
         PSNoteProperty("ExceptionAsErrorRecord", ps_type=ErrorRecord),
     ],
 )
 class RunspacePoolStateMsg(PSObject):
     """RUNSPACEPOOL_STATE Message.
 
     Defines the state of the RunspacePool. Message is defined in
-    `MS-PSRP 2.2.2.9 RUNSPACEPOOL_STATE`_. The raw RunspaceState values
-    correlate to :class:`RunspacePoolState`.
+    `MS-PSRP 2.2.2.9 RUNSPACEPOOL_STATE <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/0a5d8ef3-3b2c-4e16-9f2c-16efdaf16925>`_.
+    The raw RunspaceState values correlate to :class:`RunspacePoolState`.
 
     Args:
         RunspaceState: The RunspacePool state information as an integer.
         ExceptionAsErrorRecord: The optional error record associated with the
             RunspacePool error.
-
-    .. _MS-PSRP 2.2.2.9 RUNSPACEPOOL_STATE:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/0a5d8ef3-3b2c-4e16-9f2c-16efdaf16925
     """
 
     @classmethod
     def ToPSObjectForRemoting(
         cls,
         instance: "RunspacePoolStateMsg",
         **kwargs: typing.Any,
@@ -370,50 +341,46 @@
         PSNoteProperty("IsNested", mandatory=True, ps_type=PSBool),
     ],
 )
 class CreatePipeline(PSObject):
     """CREATE_PIPELINE Message.
 
     Creates a command pipeline and invoke it in the specified RunspacePool.
-    Message is defined in `MS-PSRP 2.2.2.10 CREATE_PIPELINE`_.
+    Message is defined in
+    `MS-PSRP 2.2.2.10 CREATE_PIPELINE <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2cf8cccb-63ab-404a-82df-caef0c41717a>`_.
 
     Args:
         NoInput: Whether the pipeline will take input.
         ApartmentState: Apartment state provided by the higher layer.
         RemoteStreamOptions: Stream options that indicate how an application
             must treat messages from the PowerShell streams.
         AddToHistory: Whether the higher layer is to add the pipeline to the
             history field of the runspace.
         HostInfo: The host information.
         PowerShell: The pipeline information to create.
         IsNested: Whether the higher layer is to run the pipeline in nested or
             steppable mode.
-
-    .. _MS-PSRP 2.2.2.10 CREATE_PIPELINE:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2cf8cccb-63ab-404a-82df-caef0c41717a
     """
 
 
 @PSMessageType(
     PSRPMessageType.GetAvailableRunspaces,
     extended_properties=[
         PSNoteProperty("ci", mandatory=True, ps_type=PSInt64),
     ],
 )
 class GetAvailableRunspaces(PSObject):
     """GET_AVAILABLE_RUNSPACES Message.
 
     Get the number of available runspaces in a RunspacePool. Message is defined
-    in `MS-PSRP 2.2.2.11 GET_AVAILABLE_RUNSPACES`_.
+    in
+    `MS-PSRP 2.2.2.11 GET_AVAILABLE_RUNSPACES <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/3f4d5a5c-9e7f-4ea2-8fea-253ddd394638>`_.
 
     Args:
         ci: The Call ID associated with this operation.
-
-    .. _MS-PSRP 2.2.2.11 GET_AVAILABLE_RUNSPACES:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/3f4d5a5c-9e7f-4ea2-8fea-253ddd394638
     """
 
 
 @PSMessageType(
     PSRPMessageType.UserEvent,
     extended_properties=[
         PSNoteProperty("EventIdentifier", ps_type=PSInt),
@@ -426,28 +393,25 @@
         PSNoteProperty("RunspaceId", ps_type=PSGuid),
     ],
 )
 class UserEvent(PSObject):
     """USER_EVENT Message.
 
     Report a user-defined event from a remote runspace. Message is defined in
-    `MS-PSRP 2.2.2.12 USER_EVENT`_.
+    `MS-PSRP 2.2.2.12 USER_EVENT <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c5a79f22-715d-4221-ae4d-47c685197b3b>`_.
 
     Args:
         EventIdentifier: The event identifier.
         SourceIdentifier: The source identifier.
         TimeGenerated: The time when the event was generated.
         Sender: The sender of the event.
         SourceArgs: Event arguments.
         MessageData: Message data associated with the event.
         ComputerName: Name of the computer where the event was fired.
         RunspaceId: The ID of the runspace.
-
-    .. _MS-PSRP 2.2.2.12 USER_EVENT:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c5a79f22-715d-4221-ae4d-47c685197b3b
     """
 
     @classmethod
     def FromPSObjectForRemoting(
         cls,
         obj: PSObject,
         **kwargs: typing.Any,
@@ -491,22 +455,19 @@
 )
 class ApplicationPrivateData(PSObject):
     """APPLICATION_PRIVATE_DATA Message.
 
     Data private to the application using the PowerShell Remoting Protocol on
     the server and client, which is passed by the protocol without
     interpretation. Message is defined in
-    `MS-PSRP 2.2.2.13 APPLICATION_PRIVATE_DATA`_.
+    `MS-PSRP 2.2.2.13 APPLICATION_PRIVATE_DATA <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/f0e105d4-4242-429f-b63b-a600111fb27e>`_.
 
     Args:
         ApplicationPrivateData: Private data that the higher layer provides to
             the server when a RunspacePool is created.
-
-    .. _MS-PSRP 2.2.2.13 APPLICATION_PRIVATE_DATA:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/f0e105d4-4242-429f-b63b-a600111fb27e
     """
 
 
 @PSMessageType(
     PSRPMessageType.GetCommandMetadata,
     extended_properties=[
         PSNoteProperty("Name", ps_type=PSList),
@@ -515,27 +476,25 @@
         PSNoteProperty("ArgumentList", ps_type=PSList),
     ],
 )
 class GetCommandMetadata(PSObject):
     """GET_COMMAND_METADATA Message.
 
     Get command metadata for commands available in a RunspacePool. Message is
-    defined in `MS-PSRP 2.2.2.14 GET_COMMAND_METADATA`_.
+    defined in
+    `MS-PSRP 2.2.2.14 GET_COMMAND_METADATA <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/b634ddef-93a0-4d3b-9e63-a630d01f233a>`_.
 
     Args:
         Name: List of wildcard patterns specifying the command names that the
             server SHOULD return.
         CommandType: The command types to search for.
         Namespace: The command namespaces containing the commands that the
             server SHOULD return.
         ArgumentList: Extra arguments passed to the higher layer above the
             PowerShell Remoting Protocol.
-
-    .. _MS-PSRP 2.2.2.14 GET_COMMAND_METADATA:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/b634ddef-93a0-4d3b-9e63-a630d01f233a
     """
 
 
 @PSMessageType(
     PSRPMessageType.RunspacePoolHostCall,
     extended_properties=[
         PSNoteProperty("ci", mandatory=True, ps_type=PSInt64),
@@ -543,23 +502,21 @@
         PSNoteProperty("mp", mandatory=True, ps_type=PSList),
     ],
 )
 class RunspacePoolHostCall(PSObject):
     """RUNSPACEPOOL_HOST_CALL Message.
 
     Method call on the host associated with the RunspacePool on the server.
-    Message is defined in `MS-PSRP 2.2.2.15 RUNSPACEPOOL_HOST_CALL`_.
+    Message is defined in
+    `MS-PSRP 2.2.2.15 RUNSPACEPOOL_HOST_CALL <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4623540b-4dd3-440e-a54b-e0fb87dd92c8>`_.
 
     Args:
         ci: The Call ID associated with this operation.
         mi: The host method identifier.
         mp: The parameters for the method.
-
-    .. _MS-PSRP 2.2.2.15 RUNSPACEPOOL_HOST_CALL:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/4623540b-4dd3-440e-a54b-e0fb87dd92c8
     """
 
 
 @PSMessageType(
     PSRPMessageType.RunspacePoolHostResponse,
     extended_properties=[
         PSNoteProperty("ci", mandatory=True, ps_type=PSInt64),
@@ -568,24 +525,22 @@
         PSNoteProperty("me", ps_type=ErrorRecord),
     ],
 )
 class RunspacePoolHostResponse(PSObject):
     """RUNSPACEPOOL_HOST_RESPONSE Message.
 
     Response from a host call executed on the client RunspacePool's host.
-    Message is defined in `MS-PSRP 2.2.2.16 RUNSPACEPOOL_HOST_RESPONSE`_.
+    Message is defined in
+    `MS-PSRP 2.2.2.16 RUNSPACEPOOL_HOST_RESPONSE <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9bcdf122-ad6b-45c3-9960-68d22627cdb5>`_.
 
     Args:
         ci: The Call ID associated with this operation.
         mi: The host method identifier.
         mr: The return value of the method.
         me: Exception thrown by a host method invocation.
-
-    .. _MS-PSRP 2.2.2.16 RUNSPACEPOOL_HOST_RESPONSE:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9bcdf122-ad6b-45c3-9960-68d22627cdb5
     """
 
     @classmethod
     def ToPSObjectForRemoting(
         cls,
         instance: "RunspacePoolHostResponse",
         **kwargs: typing.Any,
@@ -604,80 +559,67 @@
 
 
 @PSMessageType(PSRPMessageType.PipelineInput)
 class PipelineInput(PSObject):
     """PIPELINE_INPUT Message.
 
     Input to a command pipeline on the server. Message is defined in
-    `MS-PSRP 2.2.2.17 PIPELINE_INPUT`_. The actual object is the serialized
-    object that is being sent as input.
-
-    .. _MS-PSRP 2.2.2.17 PIPELINE_INPUT:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2c08acdd-3443-48c2-bf87-8fe2808d96ea
+    `MS-PSRP 2.2.2.17 PIPELINE_INPUT <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/2c08acdd-3443-48c2-bf87-8fe2808d96ea>`_.
+    The actual object is the serialized object that is being sent as input.
     """
 
 
 @PSMessageType(PSRPMessageType.EndOfPipelineInput)
 class EndOfPipelineInput(PSObject):
     """END_OF_PIPELINE_INPUT Message.
 
     Close the input collection for the command pipeline on the server. Message
-    is defined in `MS-PSRP 2.2.2.18 END_OF_PIPELINE_INPUT`_.
-
-    .. _MS-PSRP 2.2.2.18 END_OF_PIPELINE_INPUT:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e616e6fd-0241-4823-b415-7dfc247646f1
+    is defined in
+    `MS-PSRP 2.2.2.18 END_OF_PIPELINE_INPUT <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/e616e6fd-0241-4823-b415-7dfc247646f1>`_.
     """
 
 
 @PSMessageType(PSRPMessageType.PipelineOutput)
 class PipelineOutput(PSObject):
     """PIPELINE_OUTPUT Message.
 
     Output of a command pipeline on the server. Message is defined in
-    `MS-PSRP 2.2.2.19 PIPELINE_OUTPUT`_. The actual object is the serialized
-    object that is being outputted from the server.
-
-    .. _MS-PSRP 2.2.2.19 PIPELINE_OUTPUT:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/3b2c1076-c435-4aef-bdfe-3179bc452723
+    `MS-PSRP 2.2.2.19 PIPELINE_OUTPUT <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/3b2c1076-c435-4aef-bdfe-3179bc452723>`_.
+    The actual object is the serialized object that is being outputted from
+    the server.
     """
 
 
 @PSMessageType(PSRPMessageType.ErrorRecord, skip_inheritance=False)
 class ErrorRecordMsg(ErrorRecord):
     """ERROR_RECORD Message.
 
     Error record from a command pipeline on the server.. Message is defined in
-    `MS-PSRP 2.2.2.20 ERROR_RECORD`_.
-
-    .. _MS-PSRP 2.2.2.20 ERROR_RECORD:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c527797a-d017-4755-8a81-9f58280a7135
+    `MS-PSRP 2.2.2.20 ERROR_RECORD <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/c527797a-d017-4755-8a81-9f58280a7135>`_.
     """
 
 
 @PSMessageType(
     PSRPMessageType.PipelineState,
     extended_properties=[
         PSNoteProperty("PipelineState", mandatory=True, ps_type=PSInt),
         PSNoteProperty("ExceptionAsErrorRecord", ps_type=ErrorRecord),
     ],
 )
 class PipelineState(PSObject):
     """PIPELINE_STATE Message.
 
     State information of a command pipeline on the server. Message is defined
-    in `MS-PSRP 2.2.2.21 PIPELINE_STATE`_. The raw PipelineState values
-    correlate to :class:`PSInvocationState`.
+    in `MS-PSRP 2.2.2.21 PIPELINE_STATE <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/932f0c9d-845a-4883-8efd-b49a593578b8>`_.
+    The raw PipelineState values correlate to :class:`PSInvocationState`.
 
     Args:
         PipelineState: State information of the command pipeline.
         ExceptionAsErrorRecord: The optional error record associated with the
             Pipeline state error.
-
-    .. _MS-PSRP 2.2.2.21 PIPELINE_STATE:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/932f0c9d-845a-4883-8efd-b49a593578b8
     """
 
     @classmethod
     def ToPSObjectForRemoting(
         cls,
         instance: "PipelineState",
         **kwargs: typing.Any,
@@ -691,42 +633,33 @@
 
 
 @PSMessageType(PSRPMessageType.DebugRecord, skip_inheritance=False)
 class DebugRecordMsg(DebugRecord):
     """DEBUG_RECORD Message.
 
     Debug record from a command pipeline on the server. Message is defined in
-    `MS-PSRP 2.2.2.22 DEBUG_RECORD`_.
-
-    .. _MS-PSRP 2.2.2.22 DEBUG_RECORD:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/43b4cb30-6b14-498b-9325-c60339838a22
+    `MS-PSRP 2.2.2.22 DEBUG_RECORD <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/43b4cb30-6b14-498b-9325-c60339838a22>`_.
     """
 
 
 @PSMessageType(PSRPMessageType.VerboseRecord, skip_inheritance=False)
 class VerboseRecordMsg(VerboseRecord):
     """VERBOSE_RECORD Message.
 
     Verbose record from a command pipeline on the server. Message is defined in
-    `MS-PSRP 2.2.2.23 VERBOSE_RECORD`_.
-
-    .. _MS-PSRP 2.2.2.23 VERBOSE_RECORD:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/f94b18f5-0bd4-4817-8184-eb72767cce94
+    `MS-PSRP 2.2.2.23 VERBOSE_RECORD <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/f94b18f5-0bd4-4817-8184-eb72767cce94>`_.
     """
 
 
 @PSMessageType(PSRPMessageType.WarningRecord, skip_inheritance=False)
 class WarningRecordMsg(WarningRecord):
     """WARNING_RECORD Message.
 
     Warning record from a command pipeline on the server. Message is defined in
-    `MS-PSRP 2.2.2.24 WARNING_RECORD`_.
-
-    .. _MS-PSRP 2.2.2.24 WARNING_RECORD:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/31c10c51-b831-475c-ae62-603426e6a617
+    `MS-PSRP 2.2.2.24 WARNING_RECORD <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/31c10c51-b831-475c-ae62-603426e6a617>`_.
     """
 
 
 # While this looks similar to the ProgressRecord type the PSRP message is different and cannot inherit from
 # ProgressRecord.
 @PSMessageType(
     PSRPMessageType.ProgressRecord,
@@ -741,15 +674,15 @@
         PSNoteProperty("SecondsRemaining", ps_type=PSInt),
     ],
 )
 class ProgressRecordMsg(PSObject):
     """PROGRESS_RECORD Message.
 
     Progress record from a command pipeline on the server. Message is defined
-    in `MS-PSRP 2.2.2.25 PROGRESS_RECORD`_.
+    in `MS-PSRP 2.2.2.25 PROGRESS_RECORD <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/435ab824-1069-43eb-8146-7c50593a47ac>`_.
 
     Args:
         Activity: Description of the activity.
         ActivityId: Id of the activity, used as a key for the linking of
             subordinate activities.
         StatusDescription: Current status of the operation, e.g. "35 of 50
             items copied".
@@ -757,17 +690,14 @@
             the activity, e.g. "copying foo.txt".
         ParentActivityId: Id of the activity for which this is a subordinate.
         PercentComplete: Percentage of total work for the activity that is
             completed.
         Type: Type of record represented by this instance.
         SecondsRemaining: Estimated time remaining until the activity is
             complete.
-
-    .. _MS-PSRP 2.2.2.25 PROGRESS_RECORD:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/435ab824-1069-43eb-8146-7c50593a47ac
     """
 
 
 # While this has the same props as InformationRecord it is serialized as extended props and without types.
 @PSMessageType(
     PSRPMessageType.InformationRecord,
     extended_properties=[
@@ -782,15 +712,15 @@
         PSNoteProperty("ManagedThreadId", ps_type=PSUInt),
     ],
 )
 class InformationRecordMsg(PSObject):
     """INFORMATION_RECORD Message.
 
     Information record from a command pipeline on the server. Message is
-    defined in `MS-PSRP 2.2.2.26 INFORMATION_RECORD`_.
+    defined in `MS-PSRP 2.2.2.26 INFORMATION_RECORD <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/5a3ec5f0-4654-4d87-830c-d3e07c4717c9>`_.
 
     Note:
         This message is only used in ProtocolVersion>=2.3 (PowerShell v5.1+).
 
     Args:
         MessageData: The message data for the informational record.
         Source: The source of the information record (script path, function
@@ -800,77 +730,66 @@
         User: THe user that generated the informational record.
         Computer: THe computer that generated the informational record.
         ProcessId: The process that generated the informational record.
         NativeThreadId: The native thread that generated the informational
             record.
         ManagedThreadId: The managed thread that generated the informational
             record.
-
-    .. _MS-PSRP 2.2.2.26 INFORMATION_RECORD:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/5a3ec5f0-4654-4d87-830c-d3e07c4717c9
     """
 
 
 @PSMessageType(PSRPMessageType.PipelineHostCall, skip_inheritance=False)
 class PipelineHostCall(RunspacePoolHostCall):
     """PIPELINE_HOST_CALL Message.
 
     Method call on the host associated with the pipeline invocation settings on
-    the server. Message is defined in `MS-PSRP 2.2.2.27 PIPELINE_HOST_CALL`_.
+    the server. Message is defined in
+    `MS-PSRP 2.2.2.27 PIPELINE_HOST_CALL <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/16947dfb-99b5-461f-b556-dec1beb33da8>`_.
 
     Args:
         ci: The Call ID associated with this operation.
         mi: The host method identifier.
         mp: The parameters for the method.
-
-    .. _MS-PSRP 2.2.2.27 PIPELINE_HOST_CALL:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/16947dfb-99b5-461f-b556-dec1beb33da8
     """
 
 
 @PSMessageType(PSRPMessageType.PipelineHostResponse, skip_inheritance=False)
 class PipelineHostResponse(RunspacePoolHostResponse):
     """PIPELINE_HOST_RESPONSE Message.
 
     Response from a host call executed on the client's host. Message is defined
-    in `MS-PSRP 2.2.2.28 PIPELINE_HOST_RESPONSE`_.
+    in `MS-PSRP 2.2.2.28 PIPELINE_HOST_RESPONSE <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d4298dce-ee0d-417d-a73a-b4ad26524e3b>`_.
 
     Args:
         ci: The Call ID associated with this operation.
         mi: The host method identifier.
         mr: The return value of the method.
         me: Exception thrown by a host method invocation.
-
-    .. _MS-PSRP 2.2.2.28 PIPELINE_HOST_RESPONSE:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/d4298dce-ee0d-417d-a73a-b4ad26524e3b
     """
 
 
 @PSMessageType(
     PSRPMessageType.ConnectRunspacePool,
     extended_properties=[
         PSNoteProperty("MinRunspaces", ps_type=PSInt),
         PSNoteProperty("MaxRunspaces", ps_type=PSInt),
     ],
 )
 class ConnectRunspacePool(PSObject):
     """CONNECT_RUNSPACEPOOL Message.
 
     Connect to a RunspacePool. Message is defined in
-    `MS-PSRP 2.2.2.29 CONNECT_RUNSPACEPOOL`_.
+    `MS-PSRP 2.2.2.29 CONNECT_RUNSPACEPOOL <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9192146c-81b5-4abd-9b20-a56df272b95e>`_.
 
     Note:
         This message is only used in ProtocolVersion>=2.2 (PowerShell v3.0+).
 
     Args:
         MinRunspaces: Minimum number of runspaces in the Runspace Pool.
         MaxRunspaces: Maximum number of runspaces in the RUnspace Pool.
-
-    .. _MS-PSRP 2.2.2.29 CONNECT_RUNSPACEPOOL:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/9192146c-81b5-4abd-9b20-a56df272b95e
     """
 
     @classmethod
     def ToPSObjectForRemoting(
         cls,
         instance: "ConnectRunspacePool",
         **kwargs: typing.Any,
@@ -897,42 +816,36 @@
         PSNoteProperty("MaxRunspaces", mandatory=True, ps_type=PSInt),
     ],
 )
 class RunspacePoolInitData(PSObject):
     """RUNSPACEPOOL_INIT_DATA Message.
 
     RunspacePool initialization data. Message is defined in
-    `MS-PSRP 2.2.2.30 RUNSPACEPOOL_INIT_DATA`_.
+    `MS-PSRP 2.2.2.30 RUNSPACEPOOL_INIT_DATA <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ee0ce0cb-2523-4d43-b8e8-049bb89112ad>`_.
 
     Note:
         This message is only used in ProtocolVersion>=2.2 (PowerShell v3.0+).
 
     Args:
         MinRunspaces: Minimum number of runspaces in the Runspace Pool.
         MaxRunspaces: Maximum number of runspaces in the RUnspace Pool.
-
-    .. _MS-PSRP 2.2.2.30 RUNSPACEPOOL_INIT_DATA:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/ee0ce0cb-2523-4d43-b8e8-049bb89112ad
     """
 
 
 @PSMessageType(
     PSRPMessageType.ResetRunspaceState,
     extended_properties=[
         PSNoteProperty("ci", mandatory=True, ps_type=PSInt64),
     ],
 )
 class ResetRunspaceState(PSObject):
     """RESET_RUNSPACE_STATE Message.
 
     Reset RunspacePool Runspace state. Message is defined in
-    `MS-PSRP 2.2.2.31 RESET_RUNSPACE_STATE`_.
+    `MS-PSRP 2.2.2.31 RESET_RUNSPACE_STATE <https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/dc353f4b-c2e1-4172-a6ea-f72d7ef7c6bd>`_.
 
     Note:
         This message is only used in ProtocolVersion>=2.3 (PowerShell v5.1+).
 
     Args:
         ci: The Call ID associated with this operation.
-
-    .. _MS-PSRP 2.2.2.31 RESET_RUNSPACE_STATE:
-        https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-psrp/dc353f4b-c2e1-4172-a6ea-f72d7ef7c6bd
     """
```

### Comparing `psrpcore-0.2.2/src/psrpcore/types/_serializer.py` & `psrpcore-0.3.0/src/psrpcore/types/_serializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 # Copyright: (c) 2021, Jordan Borean (@jborean93) <jborean93@gmail.com>
 # MIT License (see LICENSE or https://opensource.org/licenses/MIT)
 
+from __future__ import annotations
+
 import base64
 import binascii
 import datetime
 import decimal
 import enum
 import logging
 import queue
@@ -119,14 +121,95 @@
 
     Returns:
         Optional[Union[bool, PSObject]]: The CLIXML as an XML Element object.
     """
     return _Serializer(cipher, **kwargs).deserialize(value)
 
 
+@typing.overload
+def deserialize_clixml(
+    clixml: str,
+    cipher: PSCryptoProvider,
+    preserve_streams: typing.Literal[False] = False,
+) -> list[typing.Any]: ...  # pragma: nocover
+
+
+@typing.overload
+def deserialize_clixml(
+    clixml: str,
+    cipher: PSCryptoProvider,
+    preserve_streams: typing.Literal[True] = True,
+) -> list[tuple[typing.Any, ClixmlStream]]: ...  # pragma: nocover
+
+
+def deserialize_clixml(
+    clixml: str,
+    cipher: PSCryptoProvider,
+    preserve_streams: bool = False,
+) -> list[typing.Union[typing.Any, tuple[typing.Any, ClixmlStream]]]:
+    """Deserialize a CLIXML string to Python objects.
+
+    Deserializes a CLIXML CML string produced by pwsh -OutputFormat xml into
+    the Python objects they represent. The string can start with the known
+    CLIXML prefix '#< CLIXML\\n' as the code will strip it out if present.
+
+    The raw CLIXML string can be from stdout of ``pwsh -OutputFormat xml``
+    or from output of:
+
+    .. code-block:: powershell
+
+        [System.Management.Automation.PSSerialize]::Serialize($value)
+
+    When ``preserve_streams=True``, the stream name is denoted by the ``S``
+    XML attribute. If the attribute does not exist or is set to an unknown
+    value it will be automatically converted to ``OUTPUT``.
+
+    Args:
+        clixml: The CLIXML string from PowerShell.
+        cipher: The Runspace Pool cipher to use for SecureStrings.
+        preserve_stream: Output each object as a tuple with the first value
+            being the deserialized object and the second value being the
+            :class:`ClixmlStream` as annotated by the ``S`` XML attribute.
+
+    Returns:
+        list[typing.Any]: The list of Python objects that were created from the
+        CLIXML string. Each entry will be a tuple if ``preserve_streams=True``.
+    """
+    serializer = _Serializer(cipher)
+
+    # Strip out the CLIXML header if it is present
+    if clixml.startswith("#< CLIXML"):
+        clixml = clixml[9:].lstrip("\r\n")
+
+    # ElementTree will process the xmlns value and apply it to each element
+    # breaking our parser. It is easier to just strip it from the root Objs
+    # element.
+    objs_header_end_idx = clixml.find(">")
+    clixml = "<Objs" + clixml[objs_header_end_idx:]
+
+    raw_clixml = ElementTree.fromstring(clixml)
+    values = []
+    for raw in raw_clixml:
+        v = serializer.deserialize(raw)
+
+        if preserve_streams:
+            stream_type = ClixmlStream.OUTPUT
+            if stream_attr := raw.attrib.get("S", None):
+                try:
+                    stream_type = ClixmlStream(stream_attr.lower())
+                except ValueError:
+                    pass
+
+            v = (v, stream_type)
+
+        values.append(v)
+
+    return values
+
+
 def serialize(
     value: typing.Optional[typing.Any],
     cipher: PSCryptoProvider,
     **kwargs: typing.Any,
 ) -> ElementTree.Element:
     """Serialize the Python object to CLIXML.
 
@@ -140,14 +223,89 @@
 
     Returns:
         ElementTree.Element: The CLIXML as an XML Element object.
     """
     return _Serializer(cipher, **kwargs).serialize(value)
 
 
+def serialize_clixml(
+    value: typing.Any | tuple[typing.Any | None, ClixmlStream] | None,
+    cipher: PSCryptoProvider,
+) -> str:
+    """Serializes the Python object(s) to a CLIXML string.
+
+    Serializes the provided value to a CLIXML string that can be used
+    independently to PSRemoting. The value provided can be used with:
+
+    .. code-block:: powershell
+
+        [System.Management.Automation.PSSerialize]::Deserialize($value)
+
+    If the provided value is a list each entry will be appended to the root
+    ``Objs`` element. To serialize the list as a PowerShell list/array object
+    in the ``Objs`` element, wrap the value inside another list.
+
+    .. code-block:: python
+
+        value = [1, 2, 3]
+        serialize_clixml([value], cipher)
+
+    Each value provided can also be a tuple of 2 elements where the first
+    elements is the value to serialize and the second element is the stream
+    to associate it with based on the :class:`psrpcore.types.ClixmlStream`
+    value. PowerShell accepts the following types with each stream:
+
+        OUTPUT - Any
+
+        ERROR - :class:`psrpcore.types.ErrorRecord` or :class:`str`
+
+        DEBUG, VERBOSE, WARNING - :class:`str`
+
+        INFORMATION - :class:`psrpcore.types.InformationRecord` or :class:`str`
+
+        PROGRESS - :class:`psrpcore.types.ProgressRecord`
+
+    Using a string with he ``ERROR``, ``DEBUG``, ``VERBOSE``, ``WARNING``,
+    and ``INFORMATION`` CLIXML stream will result in a record with that string
+    message. Using other types will result in the object being casted to a
+    string or undefined behaviour.
+
+    Args:
+        value: The value(s) to serialize.
+        cipher: The Runspace Pool cipher to use for SecureStrings.
+
+    Returns:
+        str: The CLIXML string.
+    """
+    objs = ElementTree.Element(
+        "Objs",
+        attrib={
+            "Version": "1.1.0.1",
+            "xmlns": "http://schemas.microsoft.com/powershell/2004/04",
+        },
+    )
+
+    serializer = _Serializer(cipher)
+    if not isinstance(value, list):
+        value = [value]
+
+    for v in value:
+        if isinstance(v, tuple) and len(v) == 2 and isinstance(v[1], ClixmlStream):
+            serialized_value = serializer.serialize(v[0])
+            serialized_value.attrib["S"] = v[1].value
+        else:
+            serialized_value = serializer.serialize(v)
+
+        objs.append(serialized_value)
+
+    clixml = ElementTree.tostring(objs, encoding="unicode")
+
+    return clixml
+
+
 def _deserialize_datetime(
     value: str,
 ) -> PSDateTime:
     """Deserializes a CLIXML DateTime string.
 
     DateTime values from PowerShell are in the format
     'YYYY-MM-DDTHH:MM-SS[.100's of nanoseconds]Z'. Unfortunately Python's
@@ -456,14 +614,26 @@
     # make sure we escape _X as well as _x.
     value = re.sub(_STRING_SERIAL_ESCAPE_ESCAPE, "_x005F_\\1", value)
     value = re.sub(_STRING_SERIAL_ESCAPE, rplcr, value)
 
     return value
 
 
+class ClixmlStream(str, enum.Enum):
+    """Signifies what stream the object is associated with in :meth:`serialize_clixml`."""
+
+    OUTPUT = "output"  #: Output stream
+    ERROR = "error"  #: Error stream
+    DEBUG = "debug"  #: Debug stream
+    VERBOSE = "verbose"  #: Verbose stream
+    WARNING = "warning"  #: Warning stream
+    PROGRESS = "progress"  #: Progress stream
+    INFORMATION = "information"  #: Information stream
+
+
 class _Serializer:
     """The Python object serializer.
 
     This is used to encapsulate the (de)serialization of Python objects to and
     from CLIXML. An instance of this class should only be used once as it
     contains a reference map to objects that are serialized in that message.
     Use the :meth:`serialize` and :meth:`deserialize` instead of calling this
@@ -784,15 +954,15 @@
                         prop == "PSObject"
                         or prop.startswith("__")
                         or prop.startswith(private_prefix)
                         or callable(prop_value)
                     ):
                         continue
 
-                    elif not attr_element:
+                    elif attr_element is None:
                         attr_element = ElementTree.SubElement(element, "MS")
 
                     sub_element = self.serialize(prop_value)
                     sub_element.attrib["N"] = _serialize_string(prop)
                     attr_element.append(sub_element)
 
         return element
```

### Comparing `psrpcore-0.2.2/src/psrpcore.egg-info/PKG-INFO` & `psrpcore-0.3.0/src/psrpcore.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psrpcore
-Version: 0.2.2
+Version: 0.3.0
 Summary: Core components for the PowerShell Remoting Protocol
 Author-email: Jordan Borean <jborean93@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Jordan Borean, Red Hat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,22 +27,23 @@
         
 Project-URL: homepage, https://github.com/jborean93/psrpcore
 Project-URL: documentation, https://psrpcore.readthedocs.io/
 Keywords: psrp,pwsh,powershell,remoting
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cryptography
 
 # psrpcore - Python PowerShell Remoting Protocol Core Library
 
 [![Test workflow](https://github.com/jborean93/psrpcore/actions/workflows/ci.yml/badge.svg)](https://github.com/jborean93/psrpcore/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/jborean93/psrpcore/branch/main/graph/badge.svg?token=UEA7VoocS5)](https://codecov.io/gh/jborean93/psrpcore)
 [![PyPI version](https://badge.fury.io/py/psrpcore.svg)](https://badge.fury.io/py/psrpcore)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/jborean93/PSAccessToken/blob/main/LICENSE)
@@ -56,15 +57,15 @@
 ## Documentation
 
 Documentation is available at https://psrpcore.readthedocs.io/.
 
 
 ## Requirements
 
-* CPython 3.7+
+* CPython 3.8+
 * [cryptography](https://github.com/pyca/cryptography)
 
 
 ## Install
 
 ### From PyPI
```

### Comparing `psrpcore-0.2.2/src/psrpcore.egg-info/SOURCES.txt` & `psrpcore-0.3.0/src/psrpcore.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,29 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements-docs.txt
 docs/Makefile
 docs/conf.py
-docs/index.rst
+docs/index.md
 docs/make.bat
+docs/minishell.md
 docs/protocol.md
+docs/psrpcore.md
+docs/psrpcore.types.md
 docs/scenarios.md
 docs/transport.md
 docs/types.md
 docs/_static/.keep
 docs/_static/ConvertTo-PythonClass.ps1
 src/psrpcore/__init__.py
 src/psrpcore/_base.py
 src/psrpcore/_client.py
+src/psrpcore/_clixml_shell.py
 src/psrpcore/_command.py
 src/psrpcore/_crypto.py
 src/psrpcore/_events.py
 src/psrpcore/_exceptions.py
 src/psrpcore/_host.py
 src/psrpcore/_payload.py
 src/psrpcore/_pipeline.py
@@ -40,17 +44,19 @@
 src/psrpcore/types/_complex.py
 src/psrpcore/types/_enum.py
 src/psrpcore/types/_host.py
 src/psrpcore/types/_primitive.py
 src/psrpcore/types/_psrp.py
 src/psrpcore/types/_serializer.py
 tests/__init__.py
+tests/clixml_shell_runner.py
 tests/conftest.py
 tests/test_base.py
 tests/test_client.py
+tests/test_clixml_shell.py
 tests/test_command.py
 tests/test_crypto.py
 tests/test_events.py
 tests/test_exceptions.py
 tests/test_host_call.py
 tests/test_integration_client.py
 tests/test_integration_server.py
@@ -60,8 +66,9 @@
 tests/types/test_base.py
 tests/types/test_collection.py
 tests/types/test_complex.py
 tests/types/test_enum.py
 tests/types/test_host.py
 tests/types/test_primitive.py
 tests/types/test_psrp.py
+tests/types/test_serialize_clixml.py
 tests/types/test_serializer.py
```

### Comparing `psrpcore-0.2.2/tests/conftest.py` & `psrpcore-0.3.0/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,19 @@
     return
 
 
 PWSH_PATH = which("pwsh.exe" if os.name == "nt" else "pwsh")
 
 
 class FakeCryptoProvider(psrpcore.types.PSCryptoProvider):
-    def decrypt(self, value: bytes) -> bytes:
-        return value
+    def decrypt(self, value: str) -> str:
+        return base64.b64decode(value).decode("utf-16-le", errors="surrogatepass")
 
-    def encrypt(self, value: bytes) -> bytes:
-        return value
-
-    def register_key(self, key: bytes) -> None:
-        pass
+    def encrypt(self, value: str) -> str:
+        return base64.b64encode(value.encode("utf-16-le", errors="surrogatepass")).decode()
 
 
 class OutOfProcTransport(typing.Generic[T]):
     def __init__(self, runspace: T) -> None:
         self.runspace = runspace
         self._incoming: queue.Queue[typing.Union[Exception, OutOfProcPacket]] = queue.Queue()
         self._listen_task = threading.Thread(target=self._read_task)
```

### Comparing `psrpcore-0.2.2/tests/test_base.py` & `psrpcore-0.3.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_client.py` & `psrpcore-0.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_command.py` & `psrpcore-0.3.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_crypto.py` & `psrpcore-0.3.0/tests/test_crypto.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     enc_session_key = crypto.encrypt_session_key(public, session_key)
     assert isinstance(enc_session_key, bytes)
     assert enc_session_key.startswith(b"\x01\x02\x00\x00\x10\x66\x00\x00\x00\xa4\x00\x00")
 
     actual_session_key = crypto.decrypt_session_key(private, enc_session_key)
     assert actual_session_key == session_key
 
-    data = b"abc"
+    data = "abc"
     encryptor = crypto.PSRemotingCrypto()
     encryptor.register_key(actual_session_key)
     enc_data = encryptor.encrypt(data)
     assert enc_data != data
 
     dec_data = encryptor.decrypt(enc_data)
     assert dec_data == data
```

### Comparing `psrpcore-0.2.2/tests/test_events.py` & `psrpcore-0.3.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_exceptions.py` & `psrpcore-0.3.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_host_call.py` & `psrpcore-0.3.0/tests/test_host_call.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_integration_client.py` & `psrpcore-0.3.0/tests/test_integration_client.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_integration_server.py` & `psrpcore-0.3.0/tests/test_integration_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,14 @@
 
     with BackgroundPipeline(
         client_opened_pwsh,
         cmd,
         Name=server_pwsh.pipe_name,
         Script="my script",
     ) as ps:
-
         runspace = server_pwsh.runspace
         open_runspace(server_pwsh)
 
         command = server_pwsh.next_payload()
         assert command.action == "Command"
         assert command.ps_guid is not None
         server_pwsh.command_ack(command.ps_guid)
@@ -289,15 +288,14 @@
     """
 
     with BackgroundPipeline(
         client_opened_pwsh,
         cmd,
         Name=server_pwsh.pipe_name,
     ):
-
         runspace = server_pwsh.runspace
         open_runspace(server_pwsh)
 
         command = server_pwsh.next_payload()
         assert command.action == "Command"
         server_pwsh.command_ack(command.ps_guid)
 
@@ -379,15 +377,14 @@
     """
 
     with BackgroundPipeline(
         client_opened_pwsh,
         cmd,
         Name=server_pwsh.pipe_name,
     ):
-
         runspace = server_pwsh.runspace
         open_runspace(server_pwsh)
 
         command = server_pwsh.next_payload()
         assert command.action == "Command"
         server_pwsh.command_ack(command.ps_guid)
 
@@ -450,15 +447,14 @@
     """
 
     with BackgroundPipeline(
         client_opened_pwsh,
         cmd,
         Name=server_pwsh.pipe_name,
     ) as ps:
-
         runspace = server_pwsh.runspace
         open_runspace(server_pwsh)
 
         command = server_pwsh.next_payload()
         assert command.action == "Command"
         server_pwsh.command_ack(command.ps_guid)
 
@@ -535,15 +531,14 @@
     """
 
     with BackgroundPipeline(
         client_opened_pwsh,
         cmd,
         Name=server_pwsh.pipe_name,
     ):
-
         runspace = server_pwsh.runspace
         open_runspace(server_pwsh)
 
         command = server_pwsh.next_payload()
         assert command.action == "Command"
         server_pwsh.command_ack(command.ps_guid)
 
@@ -621,15 +616,14 @@
     """
 
     with BackgroundPipeline(
         client_opened_pwsh,
         cmd,
         Name=server_pwsh.pipe_name,
     ) as ps:
-
         runspace = server_pwsh.runspace
         open_runspace(server_pwsh)
 
         command = server_pwsh.next_payload()
         assert command.action == "Command"
         server_pwsh.command_ack(command.ps_guid)
```

### Comparing `psrpcore-0.2.2/tests/test_payload.py` & `psrpcore-0.3.0/tests/test_payload.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/test_server.py` & `psrpcore-0.3.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/types/test_base.py` & `psrpcore-0.3.0/tests/types/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -842,15 +842,14 @@
     assert ps_base.ps_isinstance(obj, MyDeserialized1)
     assert ps_base.ps_isinstance(obj, MyDeserialized2)
     assert not ps_base.ps_isinstance(obj, Serialized)
     assert ps_base.ps_isinstance(obj, Serialized, ignore_deserialized=True)
 
 
 def test_fail_to_create_ps_type_without_ps_object():
-
     with pytest.raises(TypeError, match=r"PSType class [\w_\.<>]+ must be a subclass of PSObject"):
 
         @ps_base.PSType()
         class MyClass:
             pass
```

### Comparing `psrpcore-0.2.2/tests/types/test_collection.py` & `psrpcore-0.3.0/tests/types/test_collection.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/types/test_complex.py` & `psrpcore-0.3.0/tests/types/test_complex.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/types/test_enum.py` & `psrpcore-0.3.0/tests/types/test_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 @pytest.mark.parametrize("rehydrate", [True, False])
 def test_ps_enum(rehydrate):
     type_name = "MyEnumRehydrated" if rehydrate else "MyEnum"
 
     @PSType(type_names=[f"System.{type_name}"], rehydrate=rehydrate)
     class EnumTest(ps_enum.PSEnumBase):
-
         none = 0
         Value1 = 1
         Value2 = 2
         Value3 = 3
 
     assert str(EnumTest.none) == "EnumTest.none"
     assert repr(EnumTest.none) == "<EnumTest.none: 0>"
@@ -96,15 +95,14 @@
 
 @pytest.mark.parametrize("rehydrate", [True, False])
 def test_ps_enum_unsigned_type(rehydrate):
     type_name = "EnumUIntRehydrated" if rehydrate else "EnumUInt"
 
     @PSType(type_names=[f"System.{type_name}"], rehydrate=rehydrate)
     class EnumTest(ps_enum.PSEnumBase, base_type=PSUInt):
-
         none = 0
         Value1 = 1
         Value2 = 2
         Value3 = 3
 
     assert str(EnumTest.none) == "EnumTest.none"
     assert repr(EnumTest.none) == "<EnumTest.none: 0>"
@@ -167,15 +165,14 @@
 
 @pytest.mark.parametrize("rehydrate", [True, False])
 def test_ps_enum_extended_properties(rehydrate):
     type_name = "EnumExtendedRehydrated" if rehydrate else "EnumExtended"
 
     @PSType(type_names=[f"System.{type_name}"], rehydrate=rehydrate)
     class EnumTest(ps_enum.PSEnumBase, base_type=PSInt64):
-
         none = 0
         Value1 = 1
         Value2 = 2
         Value3 = 3
 
     assert str(EnumTest.none) == "EnumTest.none"
     assert repr(EnumTest.none) == "<EnumTest.none: 0>"
@@ -245,15 +242,14 @@
 
 @pytest.mark.parametrize("rehydrate", [True, False])
 def test_ps_flags(rehydrate):
     type_name = "FlagHydrated" if rehydrate else "Flag"
 
     @PSType(type_names=[f"System.{type_name}"], rehydrate=rehydrate)
     class FlagTest(ps_enum.PSFlagBase):
-
         none = 0
         Flag1 = 1
         Flag2 = 2
         Flag3 = 4
 
     if sys.version_info[:2] < (3, 11):
         assert str(FlagTest.none) == "FlagTest.none"
@@ -359,15 +355,14 @@
     )
 
 
 @pytest.mark.skipif(sys.version_info[:2] >= (3, 11), reason="Change in enum behaviour")
 def test_ps_flags_operators_pre_py311():
     @PSType(type_names=["System.FlagTest"])
     class FlagTest(ps_enum.PSFlagBase):
-
         none = 0
         Flag1 = 1
         Flag2 = 2
         Flag3 = 4
         Flag4 = 8
 
     val = FlagTest.none
@@ -413,15 +408,14 @@
     assert val.value == -3
 
 
 @pytest.mark.skipif(sys.version_info[:2] < (3, 11), reason="Change in enum behaviour")
 def test_ps_flags_operators_py311():
     @PSType(type_names=["System.FlagTest"])
     class FlagTest(ps_enum.PSFlagBase):
-
         none = 0
         Flag1 = 1
         Flag2 = 2
         Flag3 = 4
         Flag4 = 8
 
     val = FlagTest.none
@@ -469,15 +463,14 @@
         class InvalidEnum(ps_enum.PSEnumBase, base_type=PSString):
             none = 0
 
 
 def test_ps_enum_to_ps_ps_baseint():
     @PSType(type_names=["System.EnumToInt"])
     class EnumToInt(ps_enum.PSEnumBase):
-
         none = 0
         Value1 = 1
 
     value = PSInt(EnumToInt.Value1)
     assert isinstance(value, PSInt)
     assert value == 1
```

### Comparing `psrpcore-0.2.2/tests/types/test_host.py` & `psrpcore-0.3.0/tests/types/test_host.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/types/test_primitive.py` & `psrpcore-0.3.0/tests/types/test_primitive.py`

 * *Files identical despite different names*

### Comparing `psrpcore-0.2.2/tests/types/test_psrp.py` & `psrpcore-0.3.0/tests/types/test_psrp.py`

 * *Files identical despite different names*

