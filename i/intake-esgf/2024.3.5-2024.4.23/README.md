# Comparing `tmp/intake-esgf-2024.3.5.tar.gz` & `tmp/intake_esgf-2024.4.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake-esgf-2024.3.5.tar", last modified: Tue Mar  5 17:46:26 2024, max compression
+gzip compressed data, was "intake_esgf-2024.4.23.tar", last modified: Tue Apr 23 13:46:54 2024, max compression
```

## Comparing `intake-esgf-2024.3.5.tar` & `intake_esgf-2024.4.23.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.051094 intake-esgf-2024.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.043094 intake-esgf-2024.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.043094 intake-esgf-2024.3.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.043094 intake-esgf-2024.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-05 17:46:26.051094 intake-esgf-2024.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.043094 intake-esgf-2024.3.5/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/ci/environment-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/ci/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.047093 intake-esgf-2024.3.5/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.047093 intake-esgf-2024.3.5/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    18651 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/beginner.md
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/configure.md
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/dictkeys.md
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/logging.md
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/measures.md
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/modelgroups.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/operators.md
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/reproduce.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.047093 intake-esgf-2024.3.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/examples/adding_cell_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/examples/bayesian_model_averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/examples/carbon_cycle_anomalies.py
--rw-r--r--   0 runner    (1001) docker     (127)   512714 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/examples/cmip6-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/examples/find_ilamb_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.047093 intake-esgf-2024.3.5/intake_esgf/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15995 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25106 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.051094 intake-esgf-2024.3.5/intake_esgf/core/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5695 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/core/globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/core/solr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.051094 intake-esgf-2024.3.5/intake_esgf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/tests/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/tests/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/tests/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/intake_esgf/tests/test_solr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:46:26.051094 intake-esgf-2024.3.5/intake_esgf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-05 17:46:26.000000 intake-esgf-2024.3.5/intake_esgf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-05 17:46:26.000000 intake-esgf-2024.3.5/intake_esgf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 17:46:26.000000 intake-esgf-2024.3.5/intake_esgf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-05 17:46:26.000000 intake-esgf-2024.3.5/intake_esgf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-05 17:46:26.000000 intake-esgf-2024.3.5/intake_esgf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-05 17:46:15.000000 intake-esgf-2024.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-05 17:46:26.051094 intake-esgf-2024.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.631889 intake_esgf-2024.4.23/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.623889 intake_esgf-2024.4.23/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.623889 intake_esgf-2024.4.23/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.623889 intake_esgf-2024.4.23/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-23 13:46:54.631889 intake_esgf-2024.4.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.623889 intake_esgf-2024.4.23/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/ci/environment-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/ci/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.627889 intake_esgf-2024.4.23/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.627889 intake_esgf-2024.4.23/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    18651 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6378 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/beginner.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/configure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/dictkeys.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/globus.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/measures.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/modelgroups.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/operators.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/reproduce.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.627889 intake_esgf-2024.4.23/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/examples/adding_cell_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/examples/bayesian_model_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/examples/carbon_cycle_anomalies.py
+-rw-r--r--   0 runner    (1001) docker     (127)   512714 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/examples/cmip6-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/examples/find_ilamb_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.627889 intake_esgf-2024.4.23/intake_esgf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15483 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31960 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.631889 intake_esgf-2024.4.23/intake_esgf/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/core/globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/core/solr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.631889 intake_esgf-2024.4.23/intake_esgf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/tests/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/intake_esgf/tests/test_solr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:54.631889 intake_esgf-2024.4.23/intake_esgf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-23 13:46:54.000000 intake_esgf-2024.4.23/intake_esgf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-23 13:46:54.000000 intake_esgf-2024.4.23/intake_esgf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:46:54.000000 intake_esgf-2024.4.23/intake_esgf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 13:46:54.000000 intake_esgf-2024.4.23/intake_esgf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 13:46:54.000000 intake_esgf-2024.4.23/intake_esgf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 13:46:37.000000 intake_esgf-2024.4.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-23 13:46:54.631889 intake_esgf-2024.4.23/setup.cfg
```

### Comparing `intake-esgf-2024.3.5/.github/ISSUE_TEMPLATE/bug_report.md` & `intake_esgf-2024.4.23/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/.github/ISSUE_TEMPLATE/feature_request.md` & `intake_esgf-2024.4.23/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/.github/workflows/ci.yml` & `intake_esgf-2024.4.23/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/.github/workflows/pypi.yml` & `intake_esgf-2024.4.23/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/LICENSE` & `intake_esgf-2024.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/PKG-INFO` & `intake_esgf-2024.4.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-esgf
-Version: 2024.3.5
+Version: 2024.4.23
 Summary: An intake-esm inspired catalog for ESGF
 Author: Nathan Collier
 Author-email: nathaniel.collier@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `intake-esgf-2024.3.5/README.md` & `intake_esgf-2024.4.23/README.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/Makefile` & `intake_esgf-2024.4.23/doc/Makefile`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/_static/logo.png` & `intake_esgf-2024.4.23/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/conf.py` & `intake_esgf-2024.4.23/doc/conf.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/dictkeys.md` & `intake_esgf-2024.4.23/doc/dictkeys.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/index.rst` & `intake_esgf-2024.4.23/doc/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -56,14 +56,21 @@
    reproduce
    dictkeys
    logging
 
 .. toctree::
    :maxdepth: 2
    :hidden:
+   :caption: Experimental
+
+   globus
+
+.. toctree::
+   :maxdepth: 2
+   :hidden:
    :caption: Communicate
 
    GitHub repository <https://github.com/esgf2-us/intake-esgf>
    Bugs or Suggestions <https://github.com/esgf2-us/intake-esgf/issues>
 
 .. _intake: https://github.com/intake/intake
 .. _intake-esm: https://github.com/intake/intake-esm
```

### Comparing `intake-esgf-2024.3.5/doc/logging.md` & `intake_esgf-2024.4.23/doc/logging.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/make.bat` & `intake_esgf-2024.4.23/doc/make.bat`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/measures.md` & `intake_esgf-2024.4.23/doc/measures.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/modelgroups.md` & `intake_esgf-2024.4.23/doc/modelgroups.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/doc/quickstart.md` & `intake_esgf-2024.4.23/doc/quickstart.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ```{code-cell}
 cat = ESGFCatalog()
 print(cat)  # <-- nothing to see here yet
 ```
 
 To populate the catalog, perform a search using the traditional facets. If you
 are not familiar with these, we recommend you starting with
-our[beginner](beginner) tutorial.
+our [beginner](beginner) tutorial.
 
 ```{code-cell}
 cat.search(
     experiment_id="historical",
     source_id="CanESM5",
     frequency="mon",
     variable_id=["gpp", "tas", "pr"],
@@ -96,15 +96,15 @@
    provide you the fastest transfer speeds. Initially we will randomize the
    download locations, but as you use `intake-esgf`, we keep track of which
    servers provide you fastest transfer speeds and future downloads will prefer
    these locations. Once downloaded, we check file validity, and load into
    `xarray` containers.
 
 ```{code-cell}
-dsd = cat.to_dataset_dict()
+dsd = cat.to_dataset_dict(ignore_facets='table_id')
 ```
 
 You will notice that progress bars inform you that file information is being
 obtained and that downloads are taking place. As files are downloaded, they are
 placed into a local cache in `${HOME}/.esgf` in a directory structure that
 mirrors that of the remote storage. For future analysis which uses these
 datasets, `intake-esgf` will first check this cache to see if a file already
@@ -128,23 +128,23 @@
 
 ## Plots
 
 ```{code-cell}
 fig, axs = plt.subplots(figsize=(6, 12), nrows=3)
 
 # temperature
-ds = dsd["Amon.tas"]["tas"].mean(dim="time") - 273.15  # to [C]
+ds = dsd["tas"]["tas"].mean(dim="time") - 273.15  # to [C]
 ds.plot(ax=axs[0], cmap="bwr", vmin=-40, vmax=40, cbar_kwargs={"label": "tas [C]"})
 
 # precipitation
-ds = dsd["Amon.pr"]["pr"].mean(dim="time") * 86400 / 999.8 * 1000  # to [mm d-1]
+ds = dsd["pr"]["pr"].mean(dim="time") * 86400 / 999.8 * 1000  # to [mm d-1]
 ds.plot(ax=axs[1], cmap="Blues", vmax=10, cbar_kwargs={"label": "pr [mm d-1]"})
 
 # gross primary productivty
-ds = dsd["Lmon.gpp"]["gpp"].mean(dim="time") * 86400 * 1000  # to [g m-2 d-1]
+ds = dsd["gpp"]["gpp"].mean(dim="time") * 86400 * 1000  # to [g m-2 d-1]
 ds.plot(ax=axs[2], cmap="Greens", cbar_kwargs={"label": "gpp [g m-2 d-1]"})
 plt.tight_layout()
 ```
 
 ## Summary
 
 `intake-esgf` becomes the way that you download or locate data as well as load
```

### Comparing `intake-esgf-2024.3.5/doc/reproduce.md` & `intake_esgf-2024.4.23/doc/reproduce.md`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/examples/adding_cell_measures.py` & `intake_esgf-2024.4.23/examples/adding_cell_measures.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/examples/bayesian_model_averaging.py` & `intake_esgf-2024.4.23/examples/bayesian_model_averaging.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/examples/carbon_cycle_anomalies.py` & `intake_esgf-2024.4.23/examples/carbon_cycle_anomalies.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/examples/cmip6-example.ipynb` & `intake_esgf-2024.4.23/examples/cmip6-example.ipynb`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/examples/find_ilamb_models.py` & `intake_esgf-2024.4.23/examples/find_ilamb_models.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/intake_esgf/__init__.py` & `intake_esgf-2024.4.23/intake_esgf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     except NameError:
         return False  # Probably standard Python interpreter
 
 
 IN_NOTEBOOK = in_notebook()
 
 from intake_esgf.catalog import ESGFCatalog  # noqa
+from intake_esgf.config import conf  # noqa
 
-__all__ = ["ESGFCatalog", "IN_NOTEBOOK"]
+__all__ = ["ESGFCatalog", "conf", "IN_NOTEBOOK"]
 
 try:
     __version__ = get_distribution(__name__).version
 except DistributionNotFound:  # pragma: no cover
     __version__ = "0.0.0"  # pragma: no cover
```

### Comparing `intake-esgf-2024.3.5/intake_esgf/base.py` & `intake_esgf-2024.4.23/intake_esgf/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 """General functions used in various parts of intake-esgf."""
 
 import hashlib
-import logging
 import re
 import time
 from functools import partial
 from pathlib import Path
 from typing import Any, Literal, Union
 
 import pandas as pd
 import requests
 import xarray as xr
 
-from intake_esgf import IN_NOTEBOOK
+import intake_esgf
 from intake_esgf.database import (
     get_download_rate_dataframe,
     log_download_information,
     sort_download_links,
 )
 from intake_esgf.exceptions import NoSearchResults
-from intake_esgf.logging import setup_logging
 
-if IN_NOTEBOOK:
+if intake_esgf.IN_NOTEBOOK:
     from tqdm import tqdm_notebook as tqdm
 else:
     from tqdm import tqdm
 
 bar_format = "{desc:>20}: {percentage:3.0f}%|{bar}|{n_fmt}/{total_fmt} [{rate_fmt:>15s}{postfix}]"
 
 
 def combine_results(dfs: list[pd.DataFrame]) -> pd.DataFrame:
     """Return a combined dataframe where ids are now a list."""
     # combine and remove duplicate entries
-    logger = setup_logging()
+    logger = intake_esgf.conf.get_logger()
     df = pd.concat(dfs)
     if len(df) == 0:
         logger.info("\x1b[36;32msearch end \x1b[91;20mno results\033[0m")
         raise NoSearchResults()
     combine_time = time.time()
     variable_facet = get_facet_by_type(df, "variable")
     df = df.drop_duplicates(subset=[variable_facet, "id"]).reset_index(drop=True)
@@ -71,17 +69,17 @@
     url: str,
     local_file: Union[str, Path],
     hash: str,
     hash_algorithm: str,
     content_length: int,
     download_db: Path,
     quiet: bool = False,
-    logger: Union[logging.Logger, None] = None,
 ) -> None:
     """Download the url to a local file and check for validity, removing if not."""
+    logger = intake_esgf.conf.get_logger()
     if not isinstance(local_file, Path):
         local_file = Path(local_file)
     max_file_length = 40
     desc = (
         local_file.name
         if len(local_file.name) < max_file_length
         else f"{local_file.name[:(max_file_length-3)]}..."
@@ -95,92 +93,76 @@
             disable=quiet,
             bar_format="{desc}: {percentage:3.0f}%|{bar}|{n_fmt}/{total_fmt} [{rate_fmt}{postfix}]",
             total=content_length,
             unit="B",
             unit_scale=True,
             desc=desc,
             ascii=False,
+            leave=False,
         ) as pbar:
             for chunk in resp.iter_content(chunk_size=1024):
                 if chunk:
                     fdl.write(chunk)
                     pbar.update(len(chunk))
     transfer_time = time.time() - transfer_time
     rate = content_length * 1e-6 / transfer_time
     if get_file_hash(local_file, hash_algorithm) != hash:
-        if logger is not None:
-            logger.info(f"\x1b[91;20mHash error\033[0m {url}")
+        logger.info(f"\x1b[91;20mHash error\033[0m {url}")
         local_file.unlink()
         raise ValueError("Hash does not match")
-    if logger is not None:
-        logger.info(f"{transfer_time=:.2f} [s] at {rate:.2f} [Mb s-1] {url}")
+    logger.info(f"{transfer_time=:.2f} [s] at {rate:.2f} [Mb s-1] {url}")
     host = url[: url.index("/", 10)].replace("http://", "").replace("https://", "")
     log_download_information(download_db, host, transfer_time, content_length * 1e-6)
 
 
 def parallel_download(
     info: dict[str, Any],
-    local_cache: Path,
+    local_cache: list[Path],
     download_db: Path,
-    esg_dataroot: Union[None, Path] = None,
+    esg_dataroot: Union[None, list[Path]] = None,
 ):
     """."""
-    logger = setup_logging()
+    logger = intake_esgf.conf.get_logger()
     # does this exist on a copy we have access to?
-    if esg_dataroot is not None:
-        local_file = esg_dataroot / info["path"]
-        if local_file.exists():
-            if logger is not None:
+    for path in esg_dataroot:
+        if esg_dataroot is not None:
+            local_file = path / info["path"]
+            if local_file.exists():
                 logger.info(f"accessed {local_file}")
-            return info["key"], local_file
+                return info["key"], local_file
     # have we already downloaded this?
-    local_file = local_cache / info["path"]
-    if local_file.exists():
-        if logger is not None:
+    for path in local_cache:
+        local_file = path / info["path"]
+        if local_file.exists():
             logger.info(f"accessed {local_file}")
-        return info["key"], local_file
+            return info["key"], local_file
     # else we try to download it, first we sort links by the fastest host to you
     df_rate = get_download_rate_dataframe(download_db)
     info["HTTPServer"] = sorted(
         info["HTTPServer"], key=partial(sort_download_links, df_rate=df_rate)
     )
     # keep trying to download until one works out
     for url in info["HTTPServer"]:
         try:
             download_and_verify(
                 url,
-                local_file,
+                local_cache[0] / info["path"],
                 info["checksum"],
                 info["checksum_type"],
                 info["size"],
                 download_db=download_db,
-                logger=logger,
             )
-        except Exception as exc:
-            print(exc)
+        except Exception:
             logger.info(f"\x1b[91;20mdownload failed\033[0m {url}")
             continue
         if local_file.exists():
             return info["key"], local_file
     return None, None
 
 
-def check_for_esgf_dataroot() -> Union[Path, None]:
-    """Return a direct path to the ESGF data is it exists."""
-    to_check = [
-        "/p/css03/esgf_publish",  # Nimbus
-        "/eagle/projects/ESGF2/esg_dataroot",  # ALCF
-        "/global/cfs/projectdirs/m3522/cmip6/",  # NERSC data lake
-    ]
-    for check in to_check:
-        if Path(check).is_dir():
-            return check
-    return None
-
-
 def get_search_criteria(ds: xr.Dataset) -> dict[str, str]:
     """Return a dictionary of facet information from the dataset attributes."""
     keys = [
         "activity_id",
         "experiment_id",
         "frequency",
         "grid_label",
```

### Comparing `intake-esgf-2024.3.5/intake_esgf/catalog.py` & `intake_esgf-2024.4.23/intake_esgf/catalog.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,142 +8,147 @@
 from pathlib import Path
 from typing import Any, Callable, Literal, Union
 
 import pandas as pd
 import requests
 import xarray as xr
 from datatree import DataTree
+from globus_sdk import TransferAPIError, TransferData
 from numpy import argmax
 
+import intake_esgf
 from intake_esgf import IN_NOTEBOOK
 from intake_esgf.base import (
     add_cell_measures,
     bar_format,
-    check_for_esgf_dataroot,
     combine_results,
     get_facet_by_type,
     parallel_download,
 )
 from intake_esgf.core import GlobusESGFIndex, SolrESGFIndex
-from intake_esgf.database import create_download_database, get_download_rate_dataframe
-from intake_esgf.exceptions import NoSearchResults
-from intake_esgf.logging import setup_logging
+from intake_esgf.core.globus import get_authorized_transfer_client, variable_info
+from intake_esgf.database import (
+    create_download_database,
+    get_download_rate_dataframe,
+    log_download_information,
+    sort_globus_endpoints,
+)
+from intake_esgf.exceptions import LocalCacheNotWritable, NoSearchResults
 
 if IN_NOTEBOOK:
     from tqdm import tqdm_notebook as tqdm
 else:
     from tqdm import tqdm
 
 
 class ESGFCatalog:
     """A data catalog for searching ESGF nodes and downloading data.
 
     This catalog is largely experimental. We are using it to test capabilities and
     understand consequences of index design. Please feel free to use it but understand
     that the API will likely change.
 
-    Parameters
-    ----------
-    esgf1_indices
-        Set to True (defaults to False) to use all ESGF1 nodes in the federation or
-        specify a node or list of nodes.
-
     Attributes
     ----------
     indices : list[Union[SolrESGFIndex, GlobusESGFIndex]]
         A list of indices to search, implementations are in `intake_esgf.core`. The test
         Globus index `anl-dev` is default and always included.
     df : pd.DataFrame
         A pandas dataframe into which the results from the search are parsed. Once you
         are satisfied with the datasets listed in this dataframe, calling
         `to_dataset_dict()` will then requery the indices to obtain file information and
         then download files in parallel.
-    local_cache : pathlib.Path
-        The location to which this package will download files if necessary, mirroring
-        the directory structure of the ESGF node.
-    esgf_data_root : Union[pathlib.Path, None]
-        The location where a portion of the ESGF holdings are available locally. This
-        allows for the same search interface to be used in a Jupyter notebook. Once the
-        file information is obtained for the datasets in a search, we check this
-        location for existence before downloading the files to `local_cache`.
+    last_search: dict
+        The keywords and values used in the previous call to `search()`.
     session_time : pd.Timestamp
         The time that the class instance was initialized. Used in `session_log()` to
         parse out only the portion of the log used in this session.
     """
 
-    _esgf1_indices = [
-        "esgf.ceda.ac.uk",
-        "esgf-data.dkrz.de",
-        "esgf-node.ipsl.upmc.fr",
-        "esg-dn1.nsc.liu.se",
-        "esgf-node.llnl.gov",
-        "esgf.nci.org.au",
-        "esgf-node.ornl.gov",
-    ]
-
-    def __init__(
-        self,
-        esgf1_indices: Union[bool, str, list[str]] = False,
-    ):
-        self.indices = [GlobusESGFIndex("anl-dev"), GlobusESGFIndex("ornl-dev")]
-        if isinstance(esgf1_indices, bool) and esgf1_indices:
-            self.indices += [
-                SolrESGFIndex(node, distrib=False)
-                for node in ESGFCatalog._esgf1_indices
-            ]
-        elif isinstance(esgf1_indices, list):
-            self.indices += [
-                SolrESGFIndex(node, distrib=False) for node in esgf1_indices
-            ]
-        elif isinstance(esgf1_indices, str):
-            self.indices.append(SolrESGFIndex(esgf1_indices, distrib=False))
+    def __init__(self):
+        self.indices = []
+        self.indices += [
+            GlobusESGFIndex(ind)
+            for ind in intake_esgf.conf["globus_indices"]
+            if intake_esgf.conf["globus_indices"][ind]
+        ]
+        self.indices += [
+            SolrESGFIndex(ind)
+            for ind in intake_esgf.conf["solr_indices"]
+            if intake_esgf.conf["solr_indices"][ind]
+        ]
+        if not self.indices:
+            raise ValueError("You must have at least 1 search index configured")
         self.df = None
-        self.local_cache = None
-        self.set_local_cache_directory()
-        self.esgf_data_root = check_for_esgf_dataroot()
-        if self.esgf_data_root is not None:
-            self.logger.info(f"ESGF dataroot set {self.esgf_data_root}")
         self.session_time = pd.Timestamp.now()
         self.last_search = {}
+        self.local_cache = []
+        self.esg_dataroot = []
+        self.download_db = None
+        self._initialize()
 
     def __repr__(self):
         """Return the unique facets and values from the search."""
         if self.df is None:
             return "Perform a search() to populate the catalog."
         repr = f"Summary information for {len(self.df)} results:\n"
         return repr + self.unique().__repr__()
 
-    def set_local_cache_directory(self, path: Union[str, Path, None] = None):
-        """Set the local cache directory and create it if it does not exist."""
-        if path is None:
-            path = Path.home() / ".esgf"
-        if not isinstance(path, Path):
-            path = Path(path)
-        path.mkdir(parents=True, exist_ok=True)
-        # a change to the local cache means a change to logging
-        self.local_cache = path
-        self.logger = setup_logging(self.local_cache)
-        for index in self.indices:
-            index.logger = self.logger
+    def _initialize(self):
+        """Ensure that directories and pertinent files are created."""
+
+        def is_writable(dir: Path) -> bool:
+            test = dir / "tmp.txt"
+            try:
+                test.touch()
+                test.unlink()
+                return True
+            except Exception:
+                pass
+            return False
+
+        # ensure the local_cache directories exist, we will use the first one that is
+        # writeable
+        for path in intake_esgf.conf["local_cache"]:
+            path = Path(path).expanduser()
+            try:
+                path.mkdir(parents=True, exist_ok=True)
+            except Exception:
+                continue
+            if not path.is_dir():
+                continue
+            if is_writable(path):
+                self.local_cache.append(path)
+        if not self.local_cache:
+            raise LocalCacheNotWritable(intake_esgf.conf["local_cache"])
+
+        # check which esg_dataroot's exist and store with catalog
+        for path in intake_esgf.conf["esg_dataroot"]:
+            path = Path(path).expanduser()
+            if path.is_dir():
+                self.esg_dataroot.append(path)
+
         # initialize the local database
-        self.download_db = path / "download.db"
-        if not self.download_db.is_file():
-            create_download_database(self.download_db)
+        download_db = Path(intake_esgf.conf["download_db"]).expanduser()
+        download_db.parent.mkdir(parents=True, exist_ok=True)
+        if not download_db.is_file():
+            create_download_database(download_db)
+        self.download_db = download_db
 
     def clone(self):
         """Return a new instance of a catalog with the same indices and settings.
 
         This is used internally for when we want to find cell measures relating to the
         previous search but not overwrite the results.
 
         """
         cat = ESGFCatalog()
         cat.indices = self.indices
-        cat.esgf_data_root = self.esgf_data_root
         cat.local_cache = self.local_cache
+        cat.esg_dataroot = self.esg_dataroot
         return cat
 
     def unique(self) -> pd.Series:
         """Return the the unique values in each facet of the search."""
         out = {}
         for col in self.df.drop(columns=["id", "version"]).columns:
             out[col] = self.df[col].unique()
@@ -205,22 +210,23 @@
         ----------
         quiet
             Enable to silence the progress bar.
         search
             Any number of facet keywords and values.
 
         """
+        logger = intake_esgf.conf.get_logger()
 
         def _search(index):
             try:
                 df = index.search(**search)
             except NoSearchResults:
                 return pd.DataFrame([])
             except requests.exceptions.RequestException:
-                self.logger.info(f"└─{index} \x1b[91;20mno response\033[0m")
+                logger.info(f"└─{index} \x1b[91;20mno response\033[0m")
                 warnings.warn(
                     f"{index} failed to return a response, results may be incomplete"
                 )
                 return pd.DataFrame([])
             return df
 
         # drop empty search fields
@@ -246,15 +252,15 @@
         # log what is being searched for
         search_str = ", ".join(
             [
                 f"{key}={val if isinstance(val,list) else [val]}"
                 for key, val in search.items()
             ]
         )
-        self.logger.info(f"\x1b[36;32msearch begin\033[0m {search_str}")
+        logger.info(f"\x1b[36;32msearch begin\033[0m {search_str}")
 
         # threaded search over indices
         search_time = time.time()
         dfs = ThreadPool(len(self.indices)).imap_unordered(_search, self.indices)
         self.df = combine_results(
             tqdm(
                 dfs,
@@ -271,15 +277,15 @@
         # even though we are using latest=True, because the search is distributed, we
         # may have different versions.
         for r, row in self.df.iterrows():
             latest = max([x.split("|")[0].split(".")[-1] for x in row.id])
             self.df.loc[r, "id"] = [x for x in row.id if latest in x]
 
         search_time = time.time() - search_time
-        self.logger.info(f"\x1b[36;32msearch end\033[0m total_time={search_time:.2f}")
+        logger.info(f"\x1b[36;32msearch end\033[0m total_time={search_time:.2f}")
         self.last_search = search
         return self
 
     def from_tracking_ids(
         self, tracking_ids: Union[str, list[str]], quiet: bool = False
     ):
         """Populate the catalog by speciying tracking ids.
@@ -292,33 +298,34 @@
         ----------
         tracking_ids
             The ids whose datasets will form the items in the catalog.
         quiet
             Enable to silence the progress bar.
 
         """
+        logger = intake_esgf.conf.get_logger()
 
         def _from_tracking_ids(index):
             try:
                 df = index.from_tracking_ids(tracking_ids)
             except NoSearchResults:
                 return pd.DataFrame([])
             except requests.exceptions.RequestException:
-                self.logger.info(f"└─{index} \x1b[91;20mno response\033[0m")
+                logger.info(f"└─{index} \x1b[91;20mno response\033[0m")
                 warnings.warn(
                     f"{index} failed to return a response, results may be incomplete"
                 )
                 return pd.DataFrame([])
             return df
 
         if isinstance(tracking_ids, str):
             tracking_ids = [tracking_ids]
 
         # log what is being searched for
-        self.logger.info("\x1b[36;32mfrom_tracking_ids begin\033[0m")
+        logger.info("\x1b[36;32mfrom_tracking_ids begin\033[0m")
 
         # threaded search over indices
         search_time = time.time()
         dfs = ThreadPool(len(self.indices)).imap_unordered(
             _from_tracking_ids, self.indices
         )
         self.df = combine_results(
@@ -331,44 +338,271 @@
                 desc="Searching indices",
                 ascii=False,
                 total=len(self.indices),
             )
         )
         search_time = time.time() - search_time
         if len(self.df) != len(tracking_ids):
-            self.logger.info(
-                "One or more of the tracking_ids resolve to multiple files."
-            )
-        self.logger.info(
+            logger.info("One or more of the tracking_ids resolve to multiple files.")
+        logger.info(
             f"\x1b[36;32mfrom_tracking_ids end\033[0m total_time={search_time:.2f}"
         )
 
         return self
 
-    def set_esgf_data_root(self, root: Union[str, Path]) -> None:
-        """Set the root directory of the ESGF data local to your system.
+    def _get_file_info(
+        self, dataset_ids, quiet, separator, search_facets
+    ) -> list[dict]:
+        """Query and return file information for the given datasets."""
+
+        def _get_file_info(index, dataset_ids, **search_facets):
+            try:
+                info = index.get_file_info(list(dataset_ids.keys()), **search_facets)
+            except NoSearchResults:
+                return []
+            except requests.exceptions.RequestException:
+                logger.info(f"└─{index} \x1b[91;20mno response\033[0m")
+                warnings.warn(
+                    f"{index} failed to return a response, info may be incomplete"
+                )
+                return []
+            return info
 
-        It may be that you are working on a resource that has direct access to a copy of
-        the ESGF data. If you set this root, then when calling `to_dataset_dict()`, we
-        will check if the requested dataset is available through direct access.
+        logger = intake_esgf.conf.get_logger()
+        logger.info("\x1b[36;32mfile info begin\033[0m")
 
-        """
-        if isinstance(root, str):
-            root = Path(root)
-        assert root.is_dir()
-        self.esgf_data_root = root
+        # threaded file info over indices and flatten output
+        info_time = time.time()
+        get_file_info = ThreadPool(len(self.indices)).imap_unordered(
+            partial(_get_file_info, dataset_ids=dataset_ids, **search_facets),
+            self.indices,
+        )
+        index_infos = list(
+            tqdm(
+                get_file_info,
+                disable=quiet,
+                bar_format=bar_format,
+                unit="index",
+                unit_scale=False,
+                desc="Get file information",
+                ascii=False,
+                total=len(self.indices),
+            )
+        )
+        index_infos = [info for index_info in index_infos for info in index_info]
+
+        # now we merge this info together.
+        def _which_key(path, keys):
+            """Return the key that is likely correct based on counts in the path."""
+            counts = []
+            for key in keys:
+                counts.append(sum([str(path).count(k) for k in key.split(separator)]))
+            return keys[argmax(counts)]
+
+        merged_info = {}
+        for info in index_infos:
+            path = info["path"]
+            if path not in merged_info:
+                # Because CMIP5 is annoying, we may have multiple dataset_ids for each
+                # path (file). So here we choose which key is more likely correct.
+                if isinstance(dataset_ids[info["dataset_id"]], list):
+                    merged_info[path] = {
+                        "key": _which_key(path, dataset_ids[info["dataset_id"]])
+                    }
+                else:
+                    merged_info[path] = {"key": dataset_ids[info["dataset_id"]]}
+
+            for key, val in info.items():
+                if isinstance(val, list):
+                    if key not in merged_info[path]:
+                        merged_info[path][key] = val
+                    else:
+                        merged_info[path][key] += val
+                else:
+                    if key not in merged_info[path]:
+                        merged_info[path][key] = val
+        infos = [info for _, info in merged_info.items()]
+        info_time = time.time() - info_time
+        logger.info(f"\x1b[36;32mfile info end\033[0m total_time={info_time:.2f}")
+        return infos
+
+    def _partition_infos(self, infos: list[dict]) -> tuple[list, dict]:
+        """Separate out infos that have globus endpoints."""
+        logger = intake_esgf.conf.get_logger()
+        # loop thru infos and find all globus endpoints in the infos
+        globus_endpoints = []
+        for info in infos:
+            if "Globus" not in info:
+                continue
+            for entry in info["Globus"]:
+                m = re.search(r"globus:/*([a-z0-9\-]+)/(.*)", entry)
+                if not m:
+                    raise ValueError(f"Could not match {entry}")
+                uuid = m.group(1)
+                if uuid not in globus_endpoints:
+                    globus_endpoints.append(uuid)
+        # check which endpoints are available
+        infos_globus = {}
+        client = get_authorized_transfer_client()
+        for uuid in globus_endpoints:
+            try:
+                ep = client.get_endpoint(uuid)
+                if ep["acl_available"]:
+                    infos_globus[uuid] = []
+                else:
+                    logger.info(
+                        f"└─Endpoint '{uuid}' ({ep['display_name']}) not available."
+                    )
+                    continue
+            except TransferAPIError as exc:
+                logger.info(f"└─{exc.message}")
+        # sort endpoints by fastest transer rates
+        df_rate = get_download_rate_dataframe(self.download_db)
+        globus_endpoints = sorted(
+            infos_globus.keys(),
+            key=partial(sort_globus_endpoints, df_rate=df_rate),
+            reverse=True,
+        )
+
+        # partition the infos
+        def _partition(info):
+            # no globus entries so https it is
+            if "Globus" not in info:
+                info_https.append(info)
+                return
+            # if the file exists we need not transer it, leave it in https infos
+            for path in self.esg_dataroot + self.local_cache:
+                local_file = path / info["path"]
+                if local_file.exists():
+                    info_https.append(info)
+                    return
+            # start with the fastest endpoints
+            for uuid in globus_endpoints:
+                entries = [entry for entry in info["Globus"] if uuid in entry]
+                if entries:
+                    info["Globus"] = entries
+                    infos_globus[uuid].append(info)
+                    return
+            # if you get here, there is no globus endpoint
+            info_https.append(info)
+            return
+
+        info_https = []
+        for info in infos:
+            _partition(info)
+        return info_https, infos_globus
+
+    def _move_data(
+        self,
+        infos,
+        num_threads,
+        globus_endpoint: Union[str, None] = None,
+        globus_path: Union[Path, None] = None,
+    ):
+        """Move data either by https or globus transfers."""
+        logger = intake_esgf.conf.get_logger()
+        logger.info("\x1b[36;32mbegin move_data\033[0m")
+
+        # partition infos if an endpoint is given
+        infos_https = infos
+        infos_globus = {}
+        num_globus = 0
+        if globus_endpoint is not None:
+            logger.info("partition info counts")
+            infos_https, infos_globus = self._partition_infos(infos)
+            globus_path = Path(globus_path).expanduser()
+            logger.info(f"└─ {len(infos_https)}: https")
+            for key, item in infos_globus.items():
+                logger.info(f"└─ {len(item)}: {key}")
+                num_globus += len(item)
+
+        # only grab the client if we need it
+        if num_globus:
+            transfer_client = get_authorized_transfer_client()
+            logger.info("globus transfer task_ids")
+
+        # build up task data and submit to the transfer client
+        tasks = []
+        for source_uuid, infos in infos_globus.items():
+            # create the task data
+            task_data = TransferData(
+                source_endpoint=source_uuid, destination_endpoint=globus_endpoint
+            )
+
+            # the infos at this point should have a single entry
+            for info in infos:
+                m = re.search(r"globus:/*([a-z0-9\-]+)/(.*)", info["Globus"][0])
+                if not m:
+                    raise ValueError(f"Could not match {info['Globus'][0]}")
+                task_data.add_item(m.group(2), str(globus_path / info["path"]))
+
+            # only submit the transfer if there is data
+            if task_data["DATA"]:
+                task_doc = transfer_client.submit_transfer(task_data)
+                logger.info(f"└─ {task_doc['task_id']}")
+                tasks.append(task_doc)
+
+        # download in parallel using threads
+        results = []
+        if infos_https:
+            results += ThreadPool(min(num_threads, len(infos_https))).imap_unordered(
+                partial(
+                    parallel_download,
+                    local_cache=self.local_cache,
+                    download_db=self.download_db,
+                    esg_dataroot=self.esg_dataroot,
+                ),
+                infos_https,
+            )
+
+        # block until globus transfer completes
+        for task_doc in tasks:
+            time_interval = 5.0
+            while True:
+                response = transfer_client.get_task(task_doc["task_id"])
+                logger.info(f"task_id {task_doc['task_id']} {response.data['status']}")
+                if response.data["status"] == "SUCCEEDED":
+                    log_download_information(
+                        self.download_db,
+                        response["source_endpoint_id"],
+                        (
+                            pd.Timestamp(response["completion_time"])
+                            - pd.Timestamp(response["request_time"])
+                        ).total_seconds(),
+                        response["bytes_transferred"] * 1e-6,
+                    )
+                    break
+                time.sleep(time_interval)
+                time_interval = min(time_interval * 1.1, 30.0)
+
+        # find these newly downloaded files and populate into results
+        def _find_local_file(info):
+            for path in self.esg_dataroot + self.local_cache:
+                local_file = path / info["path"]
+                if local_file.exists():
+                    return info["key"], local_file
+            return None, None
+
+        for _, infos in infos_globus.items():
+            for info in infos:
+                results.append(_find_local_file(info))
+
+        logger.info("\x1b[36;32mend move_data\033[0m")
+        return results
 
     def to_dataset_dict(
         self,
         minimal_keys: bool = True,
         ignore_facets: Union[None, str, list[str]] = None,
         separator: str = ".",
         num_threads: int = 6,
         quiet: bool = False,
         add_measures: bool = True,
+        globus_endpoint: Union[str, None] = None,
+        globus_path: Union[Path, None] = None,
         operators: list[Any] = [],
     ) -> dict[str, xr.Dataset]:
         """Return the current search as a dictionary of datasets.
 
         By default, the keys of the returned dictionary are the minimal set of facets
         required to uniquely describe the search. If you prefer to use a full set of
         facets, set `minimal_keys=False`.
@@ -427,91 +661,21 @@
         # to pass the variables to the file info search to make sure we do not get more
         # than we want.
         search_facets = {}
         variable_facet = get_facet_by_type(self.df, "variable")
         if variable_facet in self.last_search:
             search_facets[variable_facet] = self.last_search[variable_facet]
 
-        def _get_file_info(index, dataset_ids, **search_facets):
-            try:
-                info = index.get_file_info(list(dataset_ids.keys()), **search_facets)
-            except NoSearchResults:
-                return []
-            except requests.exceptions.RequestException:
-                self.logger.info(f"└─{index} \x1b[91;20mno response\033[0m")
-                warnings.warn(
-                    f"{index} failed to return a response, info may be incomplete"
-                )
-                return []
-            return info
-
-        self.logger.info("\x1b[36;32mfile info begin\033[0m")
+        # Get the file info
+        infos = self._get_file_info(dataset_ids, quiet, separator, search_facets)
 
-        # threaded file info over indices and flatten output
-        info_time = time.time()
-        get_file_info = ThreadPool(len(self.indices)).imap_unordered(
-            partial(_get_file_info, dataset_ids=dataset_ids, **search_facets),
-            self.indices,
-        )
-        index_infos = list(
-            tqdm(
-                get_file_info,
-                disable=quiet,
-                bar_format=bar_format,
-                unit="index",
-                unit_scale=False,
-                desc="Get file information",
-                ascii=False,
-                total=len(self.indices),
-            )
-        )
-        index_infos = [info for index_info in index_infos for info in index_info]
+        # Move the data if we need to
+        results = self._move_data(infos, num_threads, globus_endpoint, globus_path)
 
-        # now we merge this info together.
-        def _which_key(path, keys):
-            """Return the key that is likely correct based on counts in the path."""
-            counts = []
-            for key in keys:
-                counts.append(sum([str(path).count(k) for k in key.split(separator)]))
-            return keys[argmax(counts)]
-
-        merged_info = {}
-        for info in index_infos:
-            path = info["path"]
-            if path not in merged_info:
-                # Because CMIP5 is annoying, we may have multiple dataset_ids for each
-                # path (file). So here we choose which key is more likely correct.
-                if isinstance(dataset_ids[info["dataset_id"]], list):
-                    merged_info[path] = {
-                        "key": _which_key(path, dataset_ids[info["dataset_id"]])
-                    }
-                else:
-                    merged_info[path] = {"key": dataset_ids[info["dataset_id"]]}
-
-            for key, val in info.items():
-                if isinstance(val, list):
-                    if key not in merged_info[path]:
-                        merged_info[path][key] = val
-                    else:
-                        merged_info[path][key] += val
-                else:
-                    if key not in merged_info[path]:
-                        merged_info[path][key] = val
-        infos = [info for _, info in merged_info.items()]
-        info_time = time.time() - info_time
-        self.logger.info(f"\x1b[36;32mfile info end\033[0m total_time={info_time:.2f}")
-
-        # Download in parallel using threads
-        fetch = partial(
-            parallel_download,
-            local_cache=self.local_cache,
-            download_db=self.download_db,
-            esg_dataroot=self.esgf_data_root,
-        )
-        results = ThreadPool(min(num_threads, len(infos))).imap_unordered(fetch, infos)
+        # Load into xarray objects
         ds = {}
         for key, local_file in results:
             if local_file is None:  # there was a problem getting this file
                 continue
             if key in ds:
                 ds[key].append(local_file)
             else:
@@ -539,15 +703,14 @@
                 total=len(ds),
             ):
                 ds[key] = add_cell_measures(ds[key], self)
 
         # If the user specifies operators, apply them now
         for op in operators:
             ds = op(ds)
-
         return ds
 
     def to_datatree(
         self,
         minimal_keys: bool = True,
         ignore_facets: Union[None, str, list[str]] = None,
     ) -> DataTree:
@@ -615,15 +778,15 @@
             q = " & ".join([f"({n} == '{v}')" for n, v in zip(names, lbl)])
             q += f" & ({variant_facet} != '{variant}')"
             self.df = self.df.drop(self.df.query(q).index)
         return self
 
     def session_log(self) -> str:
         """Return the log since the instantiation of `ESGFCatalog()`."""
-        log = open(self.local_cache / "esgf.log").readlines()[::-1]
+        log = open(Path(intake_esgf.conf["logfile"]).expanduser()).readlines()[::-1]
         for n, line in enumerate(log):
             m = re.search(r"\x1b\[36;20m(.*)\s\033\[0m", line)
             if not m:
                 continue
             if pd.to_datetime(m.group(1)) < (
                 self.session_time - pd.Timedelta(1, "s")  # little pad
             ):
@@ -654,7 +817,29 @@
             columns=dict(
                 transfer_time="transfer_time [s]",
                 transfer_size="transfer_size [Mb]",
                 rate="rate [Mb s-1]",
             )
         )
         return df
+
+    def variable_info(self, query: str, project: str = "CMIP6") -> pd.DataFrame:
+        """Return a dataframe with variable information from a query.
+
+        If you are new to searching for data in ESGF, you may not know how to figure out
+        what variables you need for your purpose.
+
+        Parameters
+        ----------
+        query
+            A search string whose contents we will use to search all record fields.
+        project
+            The project whose records we will search, defaults to `CMIP6`.
+
+        Returns
+        -------
+        df
+            A dataframe with the possibly relevant variables, their units, and various
+            name and description fields.
+
+        """
+        return variable_info(query, project)
```

### Comparing `intake-esgf-2024.3.5/intake_esgf/core/globus.py` & `intake_esgf-2024.4.23/intake_esgf/core/solr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,136 @@
-"""A Globus-based ESGF1 style index."""
+"""A ESGF1 Solr index class."""
 
 import time
 from typing import Any, Union
 
 import pandas as pd
-from globus_sdk import SearchClient, SearchQuery
+import requests
 
 from intake_esgf.base import (
     expand_cmip5_record,
     get_content_path,
     get_dataframe_columns,
 )
+from intake_esgf.exceptions import NoSearchResults
 
 
-class GlobusESGFIndex:
-    GLOBUS_INDEX_IDS = {
-        "anl-dev": "d927e2d9-ccdb-48e4-b05d-adbc3d97bbc5",
-        "ornl-dev": "ea4595f4-7b71-4da7-a1f0-e3f5d8f7f062",
-    }
-
-    def __init__(self, index_id="anl-dev"):
-        self.repr = f"GlobusESGFIndex('{index_id}')"
-        if index_id in GlobusESGFIndex.GLOBUS_INDEX_IDS:
-            index_id = GlobusESGFIndex.GLOBUS_INDEX_IDS[index_id]
-        self.index_id = index_id
-        self.client = SearchClient()
+def esg_search(base_url, **search):
+    """Yields paginated responses using the ESGF REST API."""
+    if "format" not in search:
+        search["format"] = "application/solr+json"
+    offset = search.get("offset", 0)
+    limit = search.get("limit", 10)
+    total = offset + limit + 1
+    while (offset + limit) < total:
+        response = requests.get(f"{base_url}/esg-search/search", params=search)
+        response.raise_for_status()
+        response = response.json()
+        yield response
+        limit = len(response["response"]["docs"])
+        total = response["response"]["numFound"]
+        offset = response["response"]["start"]
+        search["offset"] = offset + limit
+
+
+class SolrESGFIndex:
+    def __init__(self, index_node: str = "esgf-node.llnl.gov", distrib: bool = False):
+        self.repr = f"SolrESGFIndex('{index_node}'{',distrib=True' if distrib else ''})"
+        self.url = f"https://{index_node}"
+        self.distrib = distrib
         self.logger = None
 
     def __repr__(self):
         return self.repr
 
     def search(self, **search: Union[str, list[str]]) -> pd.DataFrame:
-        """Search the index and return as a pandas dataframe.
+        search["distrib"] = search["distrib"] if "distrib" in search else self.distrib
+        total_time = time.time()
 
-        This function uses the Globus `post_search()` function where our query consists
-        of a `match_any` filter for each of the keywords given in the input `search`. We
-        manually add constraints to only look for Dataset entries that are flagged as
-        the latest version. Note that this version of the index only contains CMIP6
-        entries.
-
-        """
-        # the ALCF index encodes booleans as strings
-        if "anl-dev" in self.repr:
-            for key, val in search.items():
-                if isinstance(val, bool):
-                    search[key] = str(val)
-
-        # build up the query and search
-        query_data = SearchQuery("")
-        for key, val in search.items():
-            query_data.add_filter(
-                key, val if isinstance(val, list) else [val], type="match_any"
-            )
-        response_time = time.time()
-        sc = SearchClient()
-        paginator = sc.paginated.post_search(self.index_id, query_data)
-        paginator.limit = 1000
         df = []
-        for response in paginator:
-            for g in response["gmeta"]:
-                content = g["entries"][0]["content"]
+        for response in esg_search(self.url, **search):
+            response = response["response"]
+            if not response["numFound"]:
+                if self.logger is not None:
+                    self.logger.info(f"└─{self} no results")
+                raise NoSearchResults
+            for doc in response["docs"]:
                 record = {
-                    facet: (
-                        content[facet][0]
-                        if isinstance(content[facet], list)
-                        else content[facet]
-                    )
-                    for facet in get_dataframe_columns(content)
-                    if facet in content
+                    facet: doc[facet][0] if isinstance(doc[facet], list) else doc[facet]
+                    for facet in get_dataframe_columns(doc)
+                    if facet in doc
                 }
-                record["project"] = content["project"][0]
-                record["id"] = g["subject"]
+                record["project"] = doc["project"][0]
+                record["id"] = doc["id"]
                 if record["project"] == "CMIP5":
                     variables = search["variable"] if "variable" in search else []
                     if not isinstance(variables, list):
                         variables = [variables]
                     record = expand_cmip5_record(
                         variables,
-                        content["variable"],
+                        doc["variable"],
                         record,
                     )
                 df += record if isinstance(record, list) else [record]
         df = pd.DataFrame(df)
-        response_time = time.time() - response_time
+        total_time = time.time() - total_time
+        if self.logger is not None:
+            self.logger.info(f"└─{self} results={len(df)} {total_time=:.2f}")
+        return df
 
-        # logging
+    def from_tracking_ids(self, tracking_ids: list[str]) -> pd.DataFrame:
+        total_time = time.time()
+        df = []
+        for response in esg_search(self.url, type="File", tracking_id=tracking_ids):
+            response = response["response"]
+            if not response["numFound"]:
+                if self.logger is not None:
+                    self.logger.info(f"└─{self} no results")
+                raise NoSearchResults
+            for doc in response["docs"]:
+                record = {
+                    facet: doc[facet][0] if isinstance(doc[facet], list) else doc[facet]
+                    for facet in get_dataframe_columns(doc)
+                    if facet in doc
+                }
+                record["project"] = doc["project"][0]
+                record["id"] = doc["id"]
+                df.append(record)
+        df = pd.DataFrame(df)
+        total_time = time.time() - total_time
         if self.logger is not None:
-            self.logger.info(f"└─{self} results={len(df)} {response_time=:.2f}")
+            self.logger.info(f"└─{self} results={len(df)} {total_time=:.2f}")
         return df
 
     def get_file_info(self, dataset_ids: list[str], **facets) -> dict[str, Any]:
-        """Get file information for the given datasets."""
-        response_time = time.time()
-        sc = SearchClient()
-        query = (
-            SearchQuery("")
-            .add_filter("type", ["File"])
-            .add_filter("dataset_id", dataset_ids, type="match_any")
+        total_time = time.time()
+        search = dict(
+            type="File",
+            latest=True,
+            retracted=False,
+            distrib=self.distrib,
+            dataset_id=dataset_ids,
         )
-        for facet, val in facets.items():
-            query.add_filter(
-                facet, val if isinstance(val, list) else [val], type="match_any"
-            )
-        paginator = sc.paginated.post_search(self.index_id, query)
-        paginator.limit = 1000
+        search.update(facets)
         infos = []
-        for response in paginator:
-            for g in response.get("gmeta"):
-                assert len(g["entries"]) == 1
-                content = g["entries"][0]["content"]
-                info = {
-                    "dataset_id": content["dataset_id"],
-                    "checksum_type": content["checksum_type"][0],
-                    "checksum": content["checksum"][0],
-                    "size": content["size"],
-                    "HTTPServer": [
-                        url.split("|")[0]
-                        for url in content["url"]
-                        if "HTTPServer" in url
-                    ],
-                }
-                info["path"] = get_content_path(content)
+        for response in esg_search(self.url, **search):
+            response = response["response"]
+            if not response["numFound"]:
+                if self.logger is not None:
+                    self.logger.info(f"└─{self} no results")
+                raise NoSearchResults
+            for doc in response["docs"]:
+                info = {}
+                info["dataset_id"] = doc["dataset_id"]
+                info["checksum_type"] = doc["checksum_type"][0]
+                info["checksum"] = doc["checksum"][0]
+                info["size"] = doc["size"]
+                info["path"] = get_content_path(doc)
+                for entry in doc["url"]:
+                    link, _, link_type = entry.split("|")
+                    if link_type not in info:
+                        info[link_type] = []
+                    info[link_type].append(link)
                 infos.append(info)
-        response_time = time.time() - response_time
         if self.logger is not None:
-            self.logger.info(f"└─{self} results={len(infos)} {response_time=:.2f}")
+            self.logger.info(f"└─{self} results={len(infos)} {total_time=:.2f}")
         return infos
-
-    def from_tracking_ids(self, tracking_ids: list[str]) -> pd.DataFrame:
-        response = SearchClient().post_search(
-            self.index_id,
-            SearchQuery("").add_filter("tracking_id", tracking_ids, type="match_any"),
-        )
-        df = []
-        for g in response["gmeta"]:
-            content = g["entries"][0]["content"]
-            record = {
-                facet: (
-                    content[facet][0]
-                    if isinstance(content[facet], list)
-                    else content[facet]
-                )
-                for facet in get_dataframe_columns(content)
-                if facet in content
-            }
-            record["project"] = content["project"][0]
-            record["id"] = content["dataset_id"]
-            df.append(record)
-        df = pd.DataFrame(df)
-        return df
```

### Comparing `intake-esgf-2024.3.5/intake_esgf/database.py` & `intake_esgf-2024.4.23/intake_esgf/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Database functions which interact with SQLite."""
+
 import sqlite3
 from pathlib import Path
 from typing import Literal
 
 import numpy as np
 import pandas as pd
 
@@ -98,7 +99,30 @@
     """
     if not len(df_rate):
         return np.random.rand(1)[0]
     host = link[: link.index("/", 10)].replace("http://", "").replace("https://", "")
     if host not in df_rate.index:
         return df_rate["rate"].max() + np.random.rand(1)[0]
     return df_rate.loc[host, "rate"]
+
+
+def sort_globus_endpoints(uuid: str, df_rate: pd.DataFrame) -> float:
+    """Return the average download rate for the given endpoint uuid.
+
+    This function is to be used to sort the list of endpoints in terms of what is fastest
+    for the user. If a endpoint is not part of the dataframe, we return a random number
+    larger than the fastest server. This is so that future downloads from this host will
+    have entries in the database.
+
+    Parameters
+    ----------
+    uuid
+        The endpoint where the file(s) may be accessed download.
+    df_rate
+        The dataframe whose indices are hosts and contains a `rate` column.
+
+    """
+    if not len(df_rate):
+        return np.random.rand(1)[0]
+    if uuid not in df_rate.index:
+        return df_rate["rate"].max() + np.random.rand(1)[0]
+    return df_rate.loc[uuid, "rate"]
```

### Comparing `intake-esgf-2024.3.5/intake_esgf/operators.py` & `intake_esgf-2024.4.23/intake_esgf/operators.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/intake_esgf/tests/test_basic.py` & `intake_esgf-2024.4.23/intake_esgf/tests/test_basic.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,57 @@
+import intake_esgf
 from intake_esgf import ESGFCatalog
 from intake_esgf.exceptions import NoSearchResults
 
-SOLR_TEST = "esgf-node.ornl.gov"
+SOLR_TEST = "esgf-node.llnl.gov"
 
 
 def test_search():
-    cat = ESGFCatalog(esgf1_indices=SOLR_TEST)
-    print(cat)
-    cat = ESGFCatalog(esgf1_indices=[SOLR_TEST]).search(
-        experiment_id="historical",
-        source_id="CanESM5",
-        variable_id=["gpp"],
-        variant_label=["r1i1p1f1"],
-    )
-    print(cat)
-    ds = cat.to_dataset_dict()
-    assert "gpp" in ds
-    assert "sftlf" in ds["gpp"]
+    with intake_esgf.conf.set(indices={SOLR_TEST: True}):
+        cat = ESGFCatalog().search(
+            experiment_id="historical",
+            source_id="CanESM5",
+            variable_id=["gpp"],
+            variant_label=["r1i1p1f1"],
+        )
+        print(cat)
+        ds = cat.to_dataset_dict()
+        assert "gpp" in ds
+        assert "sftlf" in ds["gpp"]
 
 
 def test_esgroot():
-    cat = ESGFCatalog()
-    cat.set_esgf_data_root(cat.local_cache)
-    cat.search(
-        experiment_id="historical",
-        source_id="CanESM5",
-        variable_id=["gpp"],
-        variant_label=["r1i1p1f1"],
-    )
-    ds = cat.to_dataset_dict(add_measures=False)
-    assert "gpp" in ds
-    log = cat.session_log()
-    assert "download" not in log
-    assert f"accessed {cat.esgf_data_root}" in cat.session_log()
+    with intake_esgf.conf.set(esg_dataroot=intake_esgf.conf["local_cache"]):
+        cat = ESGFCatalog().search(
+            experiment_id="historical",
+            source_id="CanESM5",
+            variable_id=["gpp"],
+            variant_label=["r1i1p1f1"],
+        )
+        ds = cat.to_dataset_dict(add_measures=False)
+        assert "gpp" in ds
+        log = cat.session_log()
+        assert "download" not in log
+        assert f"accessed {cat.esg_dataroot[0]}" in cat.session_log()
 
 
 def test_noresults():
     cat = ESGFCatalog()
     try:
         cat.search(variable_id="does_not_exist")
     except NoSearchResults:
         pass
 
 
 def test_tracking_ids():
-    cat = ESGFCatalog(esgf1_indices=SOLR_TEST).from_tracking_ids(
-        "hdl:21.14100/0577d84f-9954-494f-8cc8-465aa4fd910e"
-    )
-    assert len(cat.df) == 1
+    with intake_esgf.conf.set(indices={SOLR_TEST: True}):
+        cat = ESGFCatalog().from_tracking_ids(
+            "hdl:21.14100/0577d84f-9954-494f-8cc8-465aa4fd910e"
+        )
+        assert len(cat.df) == 1
     cat = ESGFCatalog().from_tracking_ids(
         [
             "hdl:21.14100/0577d84f-9954-494f-8cc8-465aa4fd910e",
             "hdl:21.14100/0972f78b-158e-4c6b-bcdf-7d0d75d7a8cd",
         ]
     )
     assert len(cat.df) == 2
@@ -94,7 +94,26 @@
     assert len(cat.df) == 1
     assert cat.df.iloc[0]["member_id"] == "r1i1p1f2"
 
 
 def test_download_dbase():
     cat = ESGFCatalog()
     assert len(cat.download_summary().columns)
+
+
+def test_variable_info():
+    cat = ESGFCatalog()
+    df = cat.variable_info("temperature")
+    assert df.index.isin(
+        [
+            "sitemptop",
+            "ta",
+            "ta850",
+            "tas",
+            "tasmax",
+            "tasmin",
+            "thetao",
+            "tos",
+            "ts",
+            "tsl",
+        ]
+    ).all()
```

### Comparing `intake-esgf-2024.3.5/intake_esgf/tests/test_globus.py` & `intake_esgf-2024.4.23/intake_esgf/tests/test_globus.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/intake_esgf/tests/test_operators.py` & `intake_esgf-2024.4.23/intake_esgf/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/intake_esgf/tests/test_solr.py` & `intake_esgf-2024.4.23/intake_esgf/tests/test_solr.py`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/intake_esgf.egg-info/PKG-INFO` & `intake_esgf-2024.4.23/intake_esgf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intake-esgf
-Version: 2024.3.5
+Version: 2024.4.23
 Summary: An intake-esm inspired catalog for ESGF
 Author: Nathan Collier
 Author-email: nathaniel.collier@gmail.com
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `intake-esgf-2024.3.5/intake_esgf.egg-info/SOURCES.txt` & `intake_esgf-2024.4.23/intake_esgf.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 ci/environment-docs.yml
 ci/environment.yml
 doc/Makefile
 doc/beginner.md
 doc/conf.py
 doc/configure.md
 doc/dictkeys.md
+doc/globus.md
 doc/index.rst
 doc/logging.md
 doc/make.bat
 doc/measures.md
 doc/modelgroups.md
 doc/operators.md
 doc/quickstart.md
@@ -31,17 +32,17 @@
 examples/bayesian_model_averaging.py
 examples/carbon_cycle_anomalies.py
 examples/cmip6-example.ipynb
 examples/find_ilamb_models.py
 intake_esgf/__init__.py
 intake_esgf/base.py
 intake_esgf/catalog.py
+intake_esgf/config.py
 intake_esgf/database.py
 intake_esgf/exceptions.py
-intake_esgf/logging.py
 intake_esgf/operators.py
 intake_esgf.egg-info/PKG-INFO
 intake_esgf.egg-info/SOURCES.txt
 intake_esgf.egg-info/dependency_links.txt
 intake_esgf.egg-info/requires.txt
 intake_esgf.egg-info/top_level.txt
 intake_esgf/core/__init__.py
```

### Comparing `intake-esgf-2024.3.5/pyproject.toml` & `intake_esgf-2024.4.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intake-esgf-2024.3.5/setup.cfg` & `intake_esgf-2024.4.23/setup.cfg`

 * *Files identical despite different names*

