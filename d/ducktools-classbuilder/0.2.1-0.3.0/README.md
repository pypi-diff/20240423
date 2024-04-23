# Comparing `tmp/ducktools_classbuilder-0.2.1.tar.gz` & `tmp/ducktools_classbuilder-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktools_classbuilder-0.2.1.tar", last modified: Wed Apr 17 16:46:43 2024, max compression
+gzip compressed data, was "ducktools_classbuilder-0.3.0.tar", last modified: Tue Apr 23 13:34:43 2024, max compression
```

## Comparing `ducktools_classbuilder-0.2.1.tar` & `ducktools_classbuilder-0.3.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.453205 ducktools_classbuilder-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-17 16:46:43.453205 ducktools_classbuilder-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.441205 ducktools_classbuilder-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/approach_vs_tool.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    24506 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/extension_examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.445205 ducktools_classbuilder-0.2.1/docs/perf/
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/perf/performance_tests.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.445205 ducktools_classbuilder-0.2.1/docs/prefab/
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/docs/prefab/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:46:43.453205 ducktools_classbuilder-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.441205 ducktools_classbuilder-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.441205 ducktools_classbuilder-0.2.1/src/ducktools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.445205 ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/
--rw-r--r--   0 runner    (1001) docker     (127)    13747 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/prefab.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/prefab.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.453205 ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-17 16:46:43.000000 ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-17 16:46:43.000000 ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:46:43.000000 ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 16:46:43.000000 ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-17 16:46:43.000000 ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.441205 ducktools_classbuilder-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.441205 ducktools_classbuilder-0.2.1/tests/prefab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.445205 ducktools_classbuilder-0.2.1/tests/prefab/dynamic/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_compare_attrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_pre_post_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_slots_novalues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_slotted_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.449205 ducktools_classbuilder-0.2.1/tests/prefab/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.449205 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/creation_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/dunders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:46:43.453205 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/fails/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/fails/creation_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/fails/creation_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/fails/creation_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/fails/creation_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/fails/inheritance_1.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/fails/inheritance_2.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/frozen_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/funcs_prefabs.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/init_ex.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/repr_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_dunders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_frozen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_hint_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_kw_only.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-17 16:46:39.000000 ducktools_classbuilder-0.2.1/tests/prefab/shared/test_repr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/approach_vs_tool.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24506 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/extension_examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/docs/perf/
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/perf/performance_tests.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/docs/prefab/
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/docs/prefab/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.059505 ducktools_classbuilder-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.059505 ducktools_classbuilder-0.3.0/src/ducktools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29887 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 13:34:43.000000 ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.063505 ducktools_classbuilder-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.059505 ducktools_classbuilder-0.3.0/tests/prefab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.067505 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_compare_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_pre_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_slots_novalues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_slotted_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.067505 ducktools_classbuilder-0.3.0/tests/prefab/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/creation_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/dunders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:34:43.071505 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/creation_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/inheritance_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/fails/inheritance_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/frozen_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/funcs_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/init_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/repr_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_dunders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/prefab/shared/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-23 13:34:38.000000 ducktools_classbuilder-0.3.0/tests/test_core.py
```

### Comparing `ducktools_classbuilder-0.2.1/LICENSE.md` & `ducktools_classbuilder-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/PKG-INFO` & `ducktools_classbuilder-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.2.1
+Version: 0.3.0
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ducktools_classbuilder-0.2.1/README.md` & `ducktools_classbuilder-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/Makefile` & `ducktools_classbuilder-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/api.md` & `ducktools_classbuilder-0.3.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/approach_vs_tool.md` & `ducktools_classbuilder-0.3.0/docs/approach_vs_tool.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/conf.py` & `ducktools_classbuilder-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/extension_examples.md` & `ducktools_classbuilder-0.3.0/docs/extension_examples.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/index.md` & `ducktools_classbuilder-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/make.bat` & `ducktools_classbuilder-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/perf/performance_tests.md` & `ducktools_classbuilder-0.3.0/docs/perf/performance_tests.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/docs/prefab/index.md` & `ducktools_classbuilder-0.3.0/docs/prefab/index.md`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/pyproject.toml` & `ducktools_classbuilder-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/__init__.py` & `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,20 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-__version__ = "v0.2.1"
+__version__ = "v0.3.0"
 
 # Change this name if you make heavy modifications
 INTERNALS_DICT = "__classbuilder_internals__"
 
 
-def get_internals(cls):
-    """
-    Utility function to get the internals dictionary
-    or return None.
-
-    As generated classes will always have 'fields'
-    and 'local_fields' attributes this will always
-    evaluate as 'truthy' if this is a generated class.
-
-    Generally you should use the helper get_flags and
-    get_fields methods.
-
-    Usage:
-       if internals := get_internals(cls):
-           ...
-
-    :param cls: generated class
-    :return: internals dictionary of the class or None
-    """
-    return getattr(cls, INTERNALS_DICT, None)
-
-
 def get_fields(cls, *, local=False):
     """
     Utility function to gather the fields dictionary
     from the class internals.
 
     :param cls: generated class
     :param local: get only fields that were not inherited
@@ -67,15 +45,17 @@
 
     :param cls: generated class
     :return: dictionary of keys and flag values
     """
     return getattr(cls, INTERNALS_DICT)["flags"]
 
 
-def get_inst_fields(inst):
+def _get_inst_fields(inst):
+    # This is an internal helper for constructing new
+    # 'Field' instances from existing ones.
     return {
         k: getattr(inst, k)
         for k in get_fields(type(inst))
     }
 
 
 # As 'None' can be a meaningful default we need a sentinel value
@@ -101,15 +81,15 @@
         :param funcname: name of the generated function eg `__init__`
         :param code_generator: code generator function to operate on a class.
         """
         self.funcname = funcname
         self.code_generator = code_generator
 
     def __repr__(self):
-        return f"<MethodMaker for {self.funcname} method>"
+        return f"<MethodMaker for {self.funcname!r} method>"
 
     def __get__(self, instance, cls):
         local_vars = {}
         code, globs = self.code_generator(cls)
         exec(code, globs, local_vars)
         method = local_vars.get(self.funcname)
         method.__qualname__ = f"{cls.__qualname__}.{self.funcname}"
@@ -118,15 +98,15 @@
         setattr(cls, self.funcname, method)
 
         # Use 'get' to return the generated function as a bound method
         # instead of as a regular function for first usage.
         return method.__get__(instance, cls)
 
 
-def init_maker(cls, *, null=NOTHING):
+def init_maker(cls, *, null=NOTHING, extra_code=None):
     fields = get_fields(cls)
     flags = get_flags(cls)
 
     arglist = []
     assignments = []
     globs = {}
 
@@ -146,16 +126,25 @@
             arg = f"{k}"
             assignment = f"self.{k} = {k}"
 
         arglist.append(arg)
         assignments.append(assignment)
 
     args = ", ".join(arglist)
-    assigns = "\n    ".join(assignments)
-    code = f"def __init__(self, {args}):\n" f"    {assigns}\n"
+    assigns = "\n    ".join(assignments) if assignments else "pass\n"
+    code = (
+        f"def __init__(self, {args}):\n" 
+        f"    {assigns}\n"
+    )
+    # Handle additional function calls
+    # Used for validate_field on fieldclasses
+    if extra_code:
+        for line in extra_code:
+            code += f"    {line}\n"
+
     return code, globs
 
 
 def repr_maker(cls):
     fields = get_fields(cls)
     content = ", ".join(
         f"{name}={{self.{name}!r}}"
@@ -296,15 +285,15 @@
         This is intended to be used to convert a base 
         Field into a subclass.
         
         :param fld: field class to convert
         :param kwargs: Additional keyword arguments for subclasses
         :return: new field subclass instance
         """
-        argument_dict = {**get_inst_fields(fld), **kwargs}
+        argument_dict = {**_get_inst_fields(fld), **kwargs}
 
         return cls(**argument_dict)
 
 
 # Use the builder to generate __repr__ and __eq__ methods
 # and pretend `Field` was a built class all along.
 _field_internal = {
@@ -403,36 +392,33 @@
                     )
             else:
                 used_default = True
 
     return cls
 
 
+def _field_init_func(cls):
+    # Fields need a different Nothing for their __init__ generation
+    # And an extra call to validate_field
+    field_nothing = _NothingType()
+    extra_calls = ["self.validate_field()"]
+    return init_maker(cls, null=field_nothing, extra_code=extra_calls)
+
+
 def fieldclass(cls):
     """
     This is a special decorator for making Field subclasses using __slots__.
     This works by forcing the __init__ method to treat NOTHING as a regular
     value. This means *all* instance attributes always have defaults.
 
     :param cls: Field subclass
     :return: Modified subclass
     """
 
-    # Fields need a way to call their validate method
-    # So append it to the code from __init__.
-    def field_init_func(cls_):
-        code, globs = init_maker(cls_, null=field_nothing)
-        code += "    self.validate_field()\n"
-        return code, globs
-
-    field_nothing = _NothingType()
-    field_init_desc = MethodMaker(
-        "__init__",
-        field_init_func,
-    )
+    field_init_desc = MethodMaker("__init__", _field_init_func)
     field_methods = frozenset({field_init_desc, repr_desc, eq_desc})
 
     cls = builder(
         cls,
         gatherer=slot_gatherer,
         methods=field_methods,
         flags={"slotted": True, "kw_only": True}
```

### Comparing `ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/__init__.pyi` & `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,19 @@
 from collections.abc import Callable
 
 _py_type = type  # Alias for type where it is used as a name
 
 __version__: str
 INTERNALS_DICT: str
 
-def get_internals(cls) -> dict[str, typing.Any] | None: ...
-
 def get_fields(cls: type, *, local: bool = False) -> dict[str, Field]: ...
 
 def get_flags(cls:type) -> dict[str, bool]: ...
 
-def get_inst_fields(inst: typing.Any) -> dict[str, typing.Any]: ...
+def _get_inst_fields(inst: typing.Any) -> dict[str, typing.Any]: ...
 
 class _NothingType:
     ...
 NOTHING: _NothingType
 
 # Stub Only
 _codegen_type = Callable[[type], tuple[str, dict[str, typing.Any]]]
@@ -28,14 +26,15 @@
     def __repr__(self) -> str: ...
     def __get__(self, instance, cls) -> Callable: ...
 
 def init_maker(
     cls: type,
     *,
     null: _NothingType = NOTHING,
+    extra_code: None | list[str] = None
 ) -> tuple[str, dict[str, typing.Any]]: ...
 def repr_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 def eq_maker(cls: type) -> tuple[str, dict[str, typing.Any]]: ...
 
 init_desc: MethodMaker
 repr_desc: MethodMaker
 eq_desc: MethodMaker
```

### Comparing `ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/prefab.py` & `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/src/ducktools/classbuilder/prefab.pyi` & `ducktools_classbuilder-0.3.0/src/ducktools/classbuilder/prefab.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing_extensions import dataclass_transform
 
 from collections.abc import Callable
 
 from . import (
     INTERNALS_DICT, NOTHING,
     Field, MethodMaker, SlotFields as SlotFields,
-    builder, fieldclass, get_internals, slot_gatherer
+    builder, fieldclass, get_flags, get_fields, slot_gatherer
 )
 
 # noinspection PyUnresolvedReferences
 from . import _NothingType
 
 PREFAB_FIELDS: str
 PREFAB_INIT_FUNC: str
```

### Comparing `ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/PKG-INFO` & `ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ducktools-classbuilder
-Version: 0.2.1
+Version: 0.3.0
 Summary: Toolkit for creating class boilerplate generators
 Author: David C Ellis
 License: MIT License
         
         Copyright (c) 2024 David C Ellis
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ducktools_classbuilder-0.2.1/src/ducktools_classbuilder.egg-info/SOURCES.txt` & `ducktools_classbuilder-0.3.0/src/ducktools_classbuilder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/ducktools/classbuilder/prefab.pyi
 src/ducktools/classbuilder/py.typed
 src/ducktools_classbuilder.egg-info/PKG-INFO
 src/ducktools_classbuilder.egg-info/SOURCES.txt
 src/ducktools_classbuilder.egg-info/dependency_links.txt
 src/ducktools_classbuilder.egg-info/requires.txt
 src/ducktools_classbuilder.egg-info/top_level.txt
+tests/test_core.py
 tests/prefab/dynamic/test_compare_attrib.py
 tests/prefab/dynamic/test_construction.py
 tests/prefab/dynamic/test_internals.py
 tests/prefab/dynamic/test_pre_post_init.py
 tests/prefab/dynamic/test_slots_novalues.py
 tests/prefab/dynamic/test_slotted_class.py
 tests/prefab/shared/conftest.py
```

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_construction.py` & `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_construction.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_internals.py` & `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_internals.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_pre_post_init.py` & `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_pre_post_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/dynamic/test_slotted_class.py` & `ducktools_classbuilder-0.3.0/tests/prefab/dynamic/test_slotted_class.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/creation.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/creation.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/dunders.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/inheritance.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/init_ex.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/init_ex.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/kw_only.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/examples/repr_func.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/examples/repr_func.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_creation.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_creation.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_dunders.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_dunders.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_frozen.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_frozen.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_funcs.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_funcs.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_hint_syntax.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_hint_syntax.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_inheritance.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_init.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_init.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_kw_only.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_kw_only.py`

 * *Files identical despite different names*

### Comparing `ducktools_classbuilder-0.2.1/tests/prefab/shared/test_repr.py` & `ducktools_classbuilder-0.3.0/tests/prefab/shared/test_repr.py`

 * *Files identical despite different names*

