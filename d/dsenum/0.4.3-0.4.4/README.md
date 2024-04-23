# Comparing `tmp/dsenum-0.4.3.tar.gz` & `tmp/dsenum-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsenum-0.4.3.tar", last modified: Mon Apr 22 23:28:54 2024, max compression
+gzip compressed data, was "dsenum-0.4.4.tar", last modified: Tue Apr 23 08:22:19 2024, max compression
```

## Comparing `dsenum-0.4.3.tar` & `dsenum-0.4.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.121437 dsenum-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 23:28:46.000000 dsenum-0.4.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.109437 dsenum-0.4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-22 23:28:46.000000 dsenum-0.4.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.109437 dsenum-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-22 23:28:46.000000 dsenum-0.4.3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-22 23:28:46.000000 dsenum-0.4.3/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-22 23:28:46.000000 dsenum-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-22 23:28:46.000000 dsenum-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-22 23:28:46.000000 dsenum-0.4.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-22 23:28:46.000000 dsenum-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-22 23:28:46.000000 dsenum-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-22 23:28:54.121437 dsenum-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-22 23:28:46.000000 dsenum-0.4.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-04-22 23:28:46.000000 dsenum-0.4.3/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.109437 dsenum-0.4.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.109437 dsenum-0.4.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/developer_note.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.109437 dsenum-0.4.3/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/examples/basic.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/examples/constraints.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   158042 2024-04-22 23:28:47.000000 dsenum-0.4.3/docs/examples/performance.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-22 23:28:46.000000 dsenum-0.4.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 23:28:47.000000 dsenum-0.4.3/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-22 23:28:47.000000 dsenum-0.4.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-22 23:28:47.000000 dsenum-0.4.3/docs/supercell.rst
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-22 23:28:47.000000 dsenum-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-22 23:28:54.121437 dsenum-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-22 23:28:47.000000 dsenum-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.105437 dsenum-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.113437 dsenum-0.4.3/src/dsenum/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.117437 dsenum-0.4.3/src/dsenum/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/cluster/point_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/coloring_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)   296279 2024-04-22 23:28:53.000000 dsenum-0.4.3/src/dsenum/core.c
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/core.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/derivative_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/enumerate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/permutation_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/polya.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/site.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/superlattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-22 23:28:47.000000 dsenum-0.4.3/src/dsenum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.117437 dsenum-0.4.3/src/dsenum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-22 23:28:54.000000 dsenum-0.4.3/src/dsenum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-22 23:28:54.000000 dsenum-0.4.3/src/dsenum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:28:54.000000 dsenum-0.4.3/src/dsenum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:28:54.000000 dsenum-0.4.3/src/dsenum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-22 23:28:54.000000 dsenum-0.4.3/src/dsenum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 23:28:54.000000 dsenum-0.4.3/src/dsenum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.117437 dsenum-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:54.117437 dsenum-0.4.3/tests/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/cluster/test_point_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_coloring_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_derivative_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_enumeration.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_polya.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_smith_normal_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_superlattice.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 23:28:47.000000 dsenum-0.4.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.867218 dsenum-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 08:22:10.000000 dsenum-0.4.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.855218 dsenum-0.4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 08:22:10.000000 dsenum-0.4.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.855218 dsenum-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 08:22:10.000000 dsenum-0.4.4/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-23 08:22:10.000000 dsenum-0.4.4/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-23 08:22:10.000000 dsenum-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-23 08:22:10.000000 dsenum-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-23 08:22:10.000000 dsenum-0.4.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-23 08:22:10.000000 dsenum-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 08:22:10.000000 dsenum-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-23 08:22:19.867218 dsenum-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-23 08:22:10.000000 dsenum-0.4.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      168 2024-04-23 08:22:10.000000 dsenum-0.4.4/clean.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.855218 dsenum-0.4.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.855218 dsenum-0.4.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/developer_note.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.855218 dsenum-0.4.4/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/examples/basic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/examples/constraints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   158042 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/examples/performance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2024-04-23 08:22:10.000000 dsenum-0.4.4/docs/supercell.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-23 08:22:10.000000 dsenum-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-23 08:22:19.867218 dsenum-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-23 08:22:10.000000 dsenum-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.851218 dsenum-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.859218 dsenum-0.4.4/src/dsenum/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.863218 dsenum-0.4.4/src/dsenum/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10556 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/cluster/point_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/coloring_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)   296279 2024-04-23 08:22:18.000000 dsenum-0.4.4/src/dsenum/core.c
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     6629 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/derivative_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19016 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/permutation_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/polya.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/superlattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-23 08:22:10.000000 dsenum-0.4.4/src/dsenum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.863218 dsenum-0.4.4/src/dsenum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2024-04-23 08:22:19.000000 dsenum-0.4.4/src/dsenum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-23 08:22:19.000000 dsenum-0.4.4/src/dsenum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:22:19.000000 dsenum-0.4.4/src/dsenum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:22:19.000000 dsenum-0.4.4/src/dsenum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 08:22:19.000000 dsenum-0.4.4/src/dsenum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 08:22:19.000000 dsenum-0.4.4/src/dsenum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.863218 dsenum-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:19.863218 dsenum-0.4.4/tests/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/cluster/test_point_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_coloring_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_derivative_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7263 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_enumeration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_polya.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_smith_normal_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_superlattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 08:22:10.000000 dsenum-0.4.4/tests/test_utils.py
```

### Comparing `dsenum-0.4.3/.github/workflows/deploy.yml` & `dsenum-0.4.4/.github/workflows/deploy.yml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
   workflow_run:
     workflows: [testing]
     types: [completed]
 
 jobs:
   deploy-docs:
     # https://github.community/t/workflow-run-completed-event-triggered-by-failed-workflow/128001
-    if: ${{ github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags') }}
     runs-on: ubuntu-latest
     permissions:
       contents: write
 
     steps:
       - uses: actions/checkout@v4
         with:
@@ -36,17 +35,18 @@
           python -m pip install --upgrade pip
           pip install setuptools setuptools_scm wheel
           pip install -e .[dev,docs]
       - name: Build
         run: |
           sphinx-build docs docs_build
       - name: Deploy
+        if: ${{ github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags') }}
         uses: peaceiris/actions-gh-pages@v4
         with:
-          deploy_key: ${{ secrets.GITHUB_TOKEN }}
+          deploy_key: ${{ secrets.ACTIONS_DEPLOY_KEY }}
           publish_dir: ./docs_build
 
   build_wheels:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
```

### Comparing `dsenum-0.4.3/.github/workflows/testing.yml` & `dsenum-0.4.4/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/.gitignore` & `dsenum-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/.pre-commit-config.yaml` & `dsenum-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/CITATION.cff` & `dsenum-0.4.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/LICENSE` & `dsenum-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/PKG-INFO` & `dsenum-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsenum
-Version: 0.4.3
+Version: 0.4.4
 Summary: Derivative structure enumerator for multilattice
 Author: Kohei Shinohara
 Author-email: kohei19950508@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 Requires-Dist: wheel
 Requires-Dist: pymatgen>2022.11.7
 Requires-Dist: numpy
 Requires-Dist: sympy
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: hsnf>=0.3.15
-Requires-Dist: pyzdd==0.2.8
+Requires-Dist: pyzdd
 Provides-Extra: dev
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: notebook; extra == "dev"
 Requires-Dist: jupyter_contrib_nbextensions; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: seaborn; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
```

### Comparing `dsenum-0.4.3/README.md` & `dsenum-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/docs/conf.py` & `dsenum-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/docs/developer_note.rst` & `dsenum-0.4.4/docs/developer_note.rst`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/docs/examples/basic.ipynb` & `dsenum-0.4.4/docs/examples/basic.ipynb`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/docs/examples/constraints.ipynb` & `dsenum-0.4.4/docs/examples/constraints.ipynb`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/docs/examples/performance.ipynb` & `dsenum-0.4.4/docs/examples/performance.ipynb`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/docs/supercell.rst` & `dsenum-0.4.4/docs/supercell.rst`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/pyproject.toml` & `dsenum-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/setup.py` & `dsenum-0.4.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "wheel",
         "pymatgen>2022.11.7",
         "numpy",
         "sympy",  # sympy.utilities.iterables.multiset_permutations
         "scipy",  # scipy.special.binom
         "tqdm",
         "hsnf>=0.3.15",
-        "pyzdd==0.2.8",
+        "pyzdd",
     ],
     extras_require={
         "dev": [
             "ipython",
             "notebook",
             "jupyter_contrib_nbextensions",
             "matplotlib",
```

### Comparing `dsenum-0.4.3/src/dsenum/cluster/point_cluster.py` & `dsenum-0.4.4/src/dsenum/cluster/point_cluster.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/coloring.py` & `dsenum-0.4.4/src/dsenum/coloring.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/coloring_generator.py` & `dsenum-0.4.4/src/dsenum/coloring_generator.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/converter.py` & `dsenum-0.4.4/src/dsenum/converter.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/core.c` & `dsenum-0.4.4/src/dsenum/core.c`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/core.pyx` & `dsenum-0.4.4/src/dsenum/core.pyx`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/derivative_structure.py` & `dsenum-0.4.4/src/dsenum/derivative_structure.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/enumerate.py` & `dsenum-0.4.4/src/dsenum/enumerate.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/permutation_group.py` & `dsenum-0.4.4/src/dsenum/permutation_group.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/polya.py` & `dsenum-0.4.4/src/dsenum/polya.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/superlattice.py` & `dsenum-0.4.4/src/dsenum/superlattice.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum/utils.py` & `dsenum-0.4.4/src/dsenum/utils.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/src/dsenum.egg-info/PKG-INFO` & `dsenum-0.4.4/src/dsenum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsenum
-Version: 0.4.3
+Version: 0.4.4
 Summary: Derivative structure enumerator for multilattice
 Author: Kohei Shinohara
 Author-email: kohei19950508@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 Requires-Dist: wheel
 Requires-Dist: pymatgen>2022.11.7
 Requires-Dist: numpy
 Requires-Dist: sympy
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Requires-Dist: hsnf>=0.3.15
-Requires-Dist: pyzdd==0.2.8
+Requires-Dist: pyzdd
 Provides-Extra: dev
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: notebook; extra == "dev"
 Requires-Dist: jupyter_contrib_nbextensions; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: seaborn; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
```

### Comparing `dsenum-0.4.3/src/dsenum.egg-info/SOURCES.txt` & `dsenum-0.4.4/src/dsenum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/README.md` & `dsenum-0.4.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/cluster/test_point_cluster.py` & `dsenum-0.4.4/tests/cluster/test_point_cluster.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_benchmark.py` & `dsenum-0.4.4/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_coloring_generator.py` & `dsenum-0.4.4/tests/test_coloring_generator.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_converter.py` & `dsenum-0.4.4/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_derivative_structure.py` & `dsenum-0.4.4/tests/test_derivative_structure.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_enumeration.py` & `dsenum-0.4.4/tests/test_enumeration.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_permutation.py` & `dsenum-0.4.4/tests/test_permutation.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_polya.py` & `dsenum-0.4.4/tests/test_polya.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_smith_normal_form.py` & `dsenum-0.4.4/tests/test_smith_normal_form.py`

 * *Files identical despite different names*

### Comparing `dsenum-0.4.3/tests/test_superlattice.py` & `dsenum-0.4.4/tests/test_superlattice.py`

 * *Files identical despite different names*

