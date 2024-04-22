# Comparing `tmp/pyzdd-0.2.6.tar.gz` & `tmp/pyzdd-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzdd-0.2.6.tar", last modified: Fri Dec 23 06:20:46 2022, max compression
+gzip compressed data, was "pyzdd-0.2.8.tar", last modified: Mon Apr 22 22:29:34 2024, max compression
```

## Comparing `pyzdd-0.2.6.tar` & `pyzdd-0.2.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.766921 pyzdd-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.762921 pyzdd-0.2.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.762921 pyzdd-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.github/workflows/cpp.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2022-12-23 06:20:29.000000 pyzdd-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2022-12-23 06:20:29.000000 pyzdd-0.2.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2022-12-23 06:20:29.000000 pyzdd-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-23 06:20:29.000000 pyzdd-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2022-12-23 06:20:46.766921 pyzdd-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2022-12-23 06:20:29.000000 pyzdd-0.2.6/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      370 2022-12-23 06:20:29.000000 pyzdd-0.2.6/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.762921 pyzdd-0.2.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2022-12-23 06:20:29.000000 pyzdd-0.2.6/docs/frontier.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-23 06:20:29.000000 pyzdd-0.2.6/docs/glossary.md
--rw-r--r--   0 runner    (1001) docker     (123)      881 2022-12-23 06:20:29.000000 pyzdd-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2022-12-23 06:20:46.770921 pyzdd-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2022-12-23 06:20:29.000000 pyzdd-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.762921 pyzdd-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.762921 pyzdd-0.2.6/src/pyzdd/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2022-12-23 06:20:29.000000 pyzdd-0.2.6/src/pyzdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2022-12-23 06:20:29.000000 pyzdd-0.2.6/src/pyzdd/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-23 06:20:29.000000 pyzdd-0.2.6/src/pyzdd/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2022-12-23 06:20:29.000000 pyzdd-0.2.6/src/pyzdd/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.762921 pyzdd-0.2.6/src/pyzdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2022-12-23 06:20:46.000000 pyzdd-0.2.6/src/pyzdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2022-12-23 06:20:46.000000 pyzdd-0.2.6/src/pyzdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 06:20:46.000000 pyzdd-0.2.6/src/pyzdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 06:20:46.000000 pyzdd-0.2.6/src/pyzdd.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-23 06:20:46.000000 pyzdd-0.2.6/src/pyzdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-23 06:20:46.000000 pyzdd-0.2.6/src/pyzdd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.766921 pyzdd-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2022-12-23 06:20:29.000000 pyzdd-0.2.6/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2022-12-23 06:20:29.000000 pyzdd-0.2.6/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2022-12-23 06:20:29.000000 pyzdd-0.2.6/tests/test_sro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2022-12-23 06:20:29.000000 pyzdd-0.2.6/tests/test_structure_enumeration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.766921 pyzdd-0.2.6/xtal_tdzdd/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.766921 pyzdd-0.2.6/xtal_tdzdd/example/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/example/AB.dot
--rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/example/AB_1stNN.dot
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/example/example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/example/full.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23064 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      445 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/iterator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14402 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/permutation.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14764 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/short_range_order.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.766921 pyzdd-0.2.6/xtal_tdzdd/spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/choice.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/combination.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/induced_subgraph.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/isomorphism.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/simpath.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/spanning_forest.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8509 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/stpath.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/superperiodic.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/spec/universe.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/structure_enumeration.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 06:20:46.766921 pyzdd-0.2.6/xtal_tdzdd/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_choice.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_combination.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_induced_graph.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11434 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_permutation.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_simpath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_spanning_forest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_sro.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_stpath.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16915 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_structure_enumeration.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_superperiodic.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      890 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/test/test_universe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      293 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/type.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      512 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2022-12-23 06:20:29.000000 pyzdd-0.2.6/xtal_tdzdd/wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.182790 pyzdd-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.174790 pyzdd-0.2.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.174790 pyzdd-0.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.github/workflows/cpp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-22 22:29:24.000000 pyzdd-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-22 22:29:24.000000 pyzdd-0.2.8/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-22 22:29:24.000000 pyzdd-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 22:29:24.000000 pyzdd-0.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-22 22:29:34.182790 pyzdd-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-22 22:29:24.000000 pyzdd-0.2.8/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      370 2024-04-22 22:29:24.000000 pyzdd-0.2.8/clean.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.174790 pyzdd-0.2.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-22 22:29:24.000000 pyzdd-0.2.8/docs/frontier.md
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-22 22:29:24.000000 pyzdd-0.2.8/docs/glossary.md
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-22 22:29:24.000000 pyzdd-0.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-22 22:29:34.182790 pyzdd-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-22 22:29:24.000000 pyzdd-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.170790 pyzdd-0.2.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.174790 pyzdd-0.2.8/src/pyzdd/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-22 22:29:24.000000 pyzdd-0.2.8/src/pyzdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-22 22:29:24.000000 pyzdd-0.2.8/src/pyzdd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-22 22:29:24.000000 pyzdd-0.2.8/src/pyzdd/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-22 22:29:24.000000 pyzdd-0.2.8/src/pyzdd/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.182790 pyzdd-0.2.8/src/pyzdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-22 22:29:34.000000 pyzdd-0.2.8/src/pyzdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-22 22:29:34.000000 pyzdd-0.2.8/src/pyzdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:29:34.000000 pyzdd-0.2.8/src/pyzdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:29:34.000000 pyzdd-0.2.8/src/pyzdd.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 22:29:34.000000 pyzdd-0.2.8/src/pyzdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-22 22:29:34.000000 pyzdd-0.2.8/src/pyzdd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.174790 pyzdd-0.2.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-22 22:29:24.000000 pyzdd-0.2.8/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-22 22:29:24.000000 pyzdd-0.2.8/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-22 22:29:24.000000 pyzdd-0.2.8/tests/test_sro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-22 22:29:24.000000 pyzdd-0.2.8/tests/test_structure_enumeration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.178790 pyzdd-0.2.8/xtal_tdzdd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.178790 pyzdd-0.2.8/xtal_tdzdd/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/example/AB.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/example/AB_1stNN.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/example/example.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/example/full.dot
+-rw-r--r--   0 runner    (1001) docker     (127)    23064 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/iterator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/permutation.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/short_range_order.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.178790 pyzdd-0.2.8/xtal_tdzdd/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/choice.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/combination.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/induced_subgraph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/isomorphism.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/simpath.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/spanning_forest.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/stpath.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/superperiodic.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/spec/universe.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17072 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/structure_enumeration.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:29:34.182790 pyzdd-0.2.8/xtal_tdzdd/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_choice.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_combination.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_induced_graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11434 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_permutation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_simpath.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_spanning_forest.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_sro.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_stpath.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16915 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_structure_enumeration.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_superperiodic.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/test/test_universe.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-04-22 22:29:24.000000 pyzdd-0.2.8/xtal_tdzdd/wrapper.cpp
```

### Comparing `pyzdd-0.2.6/.github/workflows/deploy.yml` & `pyzdd-0.2.8/.github/workflows/deploy.yml`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
           - [macos-12, macosx_x86_64]
           # No Github-Actions hosted runner for M1 mac for now...
           # https://github.com/actions/runner-images/issues/2187
           # - [macos-12, macosx_arm64]
         python: ["cp38", "cp39", "cp310", "cp311"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Install MacOS dependencies
         if: ${{ startsWith(matrix.buildplat[0], 'macos') }}
         # https://github.com/bluesheeptoken/CPT/blob/master/CI/github/build_wheels.sh
         # https://github.com/scikit-learn/scikit-learn/blob/main/build_tools/github/build_wheels.sh
@@ -40,52 +40,55 @@
           echo CC=/usr/bin/clang >> $GITHUB_ENV
           echo CXX=/usr/bin/clang++ >> $GITHUB_ENV
           echo CFLAGS="${CFLAGS} -I${PREFIX}/opt/libomp/include" >> $GITHUB_ENV
           echo CXXFLAGS="${CXXFLAGS} -I${PREFIX}/opt/libomp/include" >> $GITHUB_ENV
           echo LDFLAGS="${LDFLAGS} -Wl,-rpath,${PREFIX}/opt/libomp/lib -L${PREFIX}/opt/libomp/lib -lomp" >> $GITHUB_ENV
 
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.11.3
+        uses: pypa/cibuildwheel@v2.17.0
         env:
           CIBW_BUILD: ${{ matrix.python }}-${{ matrix.buildplat[1] }}
         with:
           config-file: "{package}/pyproject.toml"
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: pypi-${{ matrix.python }}-${{ matrix.buildplat[1] }}
           path: ./wheelhouse/*.whl
 
   build_sdist:
     if: ${{ github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags') }}
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Install dependencies
         run: |
           sudo apt-get install -y make cmake gcc g++
 
       - name: Build sdist
         run: pipx run build --sdist
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
+          name: pypi-sdist
           path: dist/*.tar.gz
 
   deploy-pypi:
 
     runs-on: ubuntu-latest
     needs: [build_wheels, build_sdist]
 
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: artifact
+          pattern: pypi-*
+          merge-multiple: true
           path: dist
 
       - name: Publish package to TestPyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.TESTPYPI_API_TOKEN }}
```

### Comparing `pyzdd-0.2.6/.github/workflows/testing.yml` & `pyzdd-0.2.8/.github/workflows/testing.yml`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,26 @@
   tests:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: ["3.8", "3.9", "3.10"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Install dependencies
         run: |
           sudo apt-get install -y make cmake gcc g++
 
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       # https://github.com/actions/cache/blob/main/examples.md#python---pip
-      - uses: actions/cache@v3
+      - uses: actions/cache@v4
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-${{ matrix.python-version }}-pip-${{ hashFiles('**/setup.py') }}
           restore-keys: |
             ${{ runner.os }}-${{ matrix.python-version }}-pip-
 
       - name: Install
```

### Comparing `pyzdd-0.2.6/.gitignore` & `pyzdd-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/.pre-commit-config.yaml` & `pyzdd-0.2.8/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 ci:
     skip: [clang-format]
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-yaml
 
   # formatter
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 24.4.0
     hooks:
     - id: black
   # linter
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: 7.0.0
     hooks:
     - id: flake8
       exclude: ^docs/
   # type annotation
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.9.0
     hooks:
     - id: mypy
       exclude: ^docs/
   # isort
   - repo: https://github.com/pycqa/isort
-    rev: v5.11.3
+    rev: 5.13.2
     hooks:
       - id: isort
         name: isort (python)
         args: ["--profile", "black"]
         exclude: ^setup.py
       - id: isort
         name: isort (cython)
         types: [cython]
       - id: isort
         name: isort (pyi)
         types: [pyi]
   # Upgrade syntax
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
   - repo: https://github.com/pocc/pre-commit-hooks
     rev: v1.3.5
     hooks:
       - id: clang-format
         args: [-i, --style=file]
```

### Comparing `pyzdd-0.2.6/CMakeLists.txt` & `pyzdd-0.2.8/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/LICENSE` & `pyzdd-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/README.md` & `pyzdd-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/docs/frontier.md` & `pyzdd-0.2.8/docs/frontier.md`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/pyproject.toml` & `pyzdd-0.2.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 manylinux-x86_64-image = "manylinux2014"
 
 [tool.cibuildwheel.linux]
 # Note that manylinux_2_24 builds occur inside a Debian9 docker, where manylinux2010 and manylinux2014 builds occur inside a CentOS one. So for manylinux_2_24 the CIBW_BEFORE_ALL_LINUX command must use apt-get -y instead.
 before-build = "yum install -y make cmake gcc gcc-c++"
 
 [tool.cibuildwheel.macos]
-archs = ["x86_64", "arm64"]
+# archs = ["x86_64", "arm64"]
 
 [tool.black]
 line-length = 99
 target-version = ['py38', 'py39', 'py310']
 include = '\.pyi?$'
 exclude = '''
 /(
```

### Comparing `pyzdd-0.2.6/setup.py` & `pyzdd-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 with open(Path(__file__).resolve().parent / "README.md") as f:
     long_description = "\n" + f.read()
 
 
 # Adapted from https://github.com/pybind/cmake_example
 
+
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
     def __init__(self, name, sourcedir=""):
         Extension.__init__(self, name, sources=[])
         self.sourcedir = os.path.abspath(sourcedir)
```

### Comparing `pyzdd-0.2.6/src/pyzdd/__init__.py` & `pyzdd-0.2.8/src/pyzdd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/src/pyzdd/graph.py` & `pyzdd-0.2.8/src/pyzdd/graph.py`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/src/pyzdd/structure.py` & `pyzdd-0.2.8/src/pyzdd/structure.py`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/src/pyzdd.egg-info/SOURCES.txt` & `pyzdd-0.2.8/src/pyzdd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/tests/test_graph.py` & `pyzdd-0.2.8/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/tests/test_spec.py` & `pyzdd-0.2.8/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/tests/test_sro.py` & `pyzdd-0.2.8/tests/test_sro.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         dd2,
         num_sites,
         num_types,
         vertex_order,
         automorphism,
         composition_constraints,
     )
-    for (graph, target) in zip(graphs, targets):
+    for graph, target in zip(graphs, targets):
         restrict_pair_correlation(
             dd2,
             num_sites,
             num_types,
             vertex_order,
             graph,
             target,
```

### Comparing `pyzdd-0.2.6/tests/test_structure_enumeration.py` & `pyzdd-0.2.8/tests/test_structure_enumeration.py`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/CMakeLists.txt` & `pyzdd-0.2.8/xtal_tdzdd/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/example/AB.dot` & `pyzdd-0.2.8/xtal_tdzdd/example/AB.dot`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/example/AB_1stNN.dot` & `pyzdd-0.2.8/xtal_tdzdd/example/AB_1stNN.dot`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/example/example.cpp` & `pyzdd-0.2.8/xtal_tdzdd/example/example.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/example/full.dot` & `pyzdd-0.2.8/xtal_tdzdd/example/full.dot`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/graph.hpp` & `pyzdd-0.2.8/xtal_tdzdd/graph.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/iterator.hpp` & `pyzdd-0.2.8/xtal_tdzdd/iterator.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/permutation.hpp` & `pyzdd-0.2.8/xtal_tdzdd/permutation.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/short_range_order.hpp` & `pyzdd-0.2.8/xtal_tdzdd/short_range_order.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/choice.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/choice.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/combination.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/combination.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/induced_subgraph.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/induced_subgraph.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/isomorphism.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/isomorphism.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/simpath.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/simpath.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/spanning_forest.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/spanning_forest.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/stpath.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/stpath.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/superperiodic.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/superperiodic.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/spec/universe.hpp` & `pyzdd-0.2.8/xtal_tdzdd/spec/universe.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/structure_enumeration.hpp` & `pyzdd-0.2.8/xtal_tdzdd/structure_enumeration.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/CMakeLists.txt` & `pyzdd-0.2.8/xtal_tdzdd/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_choice.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_choice.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_combination.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_combination.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_induced_graph.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_induced_graph.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_permutation.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_permutation.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_simpath.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_simpath.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_spanning_forest.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_spanning_forest.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_sro.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_sro.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_stpath.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_stpath.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_structure_enumeration.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_structure_enumeration.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_superperiodic.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_superperiodic.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/test/test_universe.cpp` & `pyzdd-0.2.8/xtal_tdzdd/test/test_universe.cpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/utils.hpp` & `pyzdd-0.2.8/xtal_tdzdd/utils.hpp`

 * *Files identical despite different names*

### Comparing `pyzdd-0.2.6/xtal_tdzdd/wrapper.cpp` & `pyzdd-0.2.8/xtal_tdzdd/wrapper.cpp`

 * *Files identical despite different names*

