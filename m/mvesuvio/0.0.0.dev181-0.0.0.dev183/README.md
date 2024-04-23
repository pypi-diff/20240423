# Comparing `tmp/mvesuvio-0.0.0.dev181.tar.gz` & `tmp/mvesuvio-0.0.0.dev183.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvesuvio-0.0.0.dev181.tar", last modified: Fri Apr 19 08:53:35 2024, max compression
+gzip compressed data, was "mvesuvio-0.0.0.dev183.tar", last modified: Tue Apr 23 02:34:51 2024, max compression
```

## Comparing `mvesuvio-0.0.0.dev181.tar` & `mvesuvio-0.0.0.dev183.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/
--rw-r--r--   0 ljg28444 (1219131)  1219131     6536 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/PKG-INFO
--rw-r--r--   0 ljg28444 (1219131)  1219131     5589 2024-04-19 08:51:56.000000 mvesuvio-0.0.0.dev181/README.md
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/
--rw-r--r--   0 ljg28444 (1219131)  1219131     1268 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131       29 2024-04-19 08:53:34.000000 mvesuvio-0.0.0.dev181/mvesuvio/_version.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     1292 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/analysis_runner.py
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/config/
--rw-r--r--   0 ljg28444 (1219131)  1219131       77 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/Mantid.user.properties
--rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     5026 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/analysis_inputs.py
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/
--rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     7027 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018.par
--rw-r--r--   0 ljg28444 (1219131)  1219131     7218 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_2.par
--rw-r--r--   0 ljg28444 (1219131)  1219131     7079 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_3.par
--rw-r--r--   0 ljg28444 (1219131)  1219131     4291 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2019.par
--rw-r--r--   0 ljg28444 (1219131)  1219131       87 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/config/vesuvio.user.properties
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.029948 mvesuvio-0.0.0.dev181/mvesuvio/scripts/
--rw-r--r--   0 ljg28444 (1219131)  1219131     2758 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/scripts/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     3907 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/scripts/handle_config.py
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.033948 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/
--rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     5900 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_analysis.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     4173 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_bootstrap.py
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.033948 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/
--rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     3836 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/expr_for_tests.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     2225 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_jackknife.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     5664 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_yspace_fit.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     5676 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_yspace_fit_GC.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     4723 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/system_tests/tests_IC.py
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/
--rw-r--r--   0 ljg28444 (1219131)  1219131    10860 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/ICHelpers.py
--rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131    41027 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/analysis_functions.py
--rw-r--r--   0 ljg28444 (1219131)  1219131    22158 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap.py
--rw-r--r--   0 ljg28444 (1219131)  1219131    20979 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap_analysis.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     6506 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py
--rw-r--r--   0 ljg28444 (1219131)  1219131    63650 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/fit_in_yspace.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     7963 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/procedures.py
--rw-r--r--   0 ljg28444 (1219131)  1219131     4573 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/run_script.py
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/
--rw-r--r--   0 ljg28444 (1219131)  1219131        0 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/__init__.py
--rw-r--r--   0 ljg28444 (1219131)  1219131      746 2024-01-02 11:36:30.000000 mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py
-drwxr-xr-x   0 ljg28444 (1219131)  1219131        0 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/
--rw-r--r--   0 ljg28444 (1219131)  1219131     6536 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/PKG-INFO
--rw-r--r--   0 ljg28444 (1219131)  1219131     1544 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/SOURCES.txt
--rw-r--r--   0 ljg28444 (1219131)  1219131        1 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/dependency_links.txt
--rw-r--r--   0 ljg28444 (1219131)  1219131       51 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/entry_points.txt
--rw-r--r--   0 ljg28444 (1219131)  1219131       81 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/requires.txt
--rw-r--r--   0 ljg28444 (1219131)  1219131        9 2024-04-19 08:53:35.000000 mvesuvio-0.0.0.dev181/mvesuvio.egg-info/top_level.txt
--rw-r--r--   0 ljg28444 (1219131)  1219131     1921 2024-04-10 09:51:33.000000 mvesuvio-0.0.0.dev181/pyproject.toml
--rw-r--r--   0 ljg28444 (1219131)  1219131       38 2024-04-19 08:53:35.037948 mvesuvio-0.0.0.dev181/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.907732 mvesuvio-0.0.0.dev183/
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-23 02:34:51.907732 mvesuvio-0.0.0.dev183/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.903732 mvesuvio-0.0.0.dev183/mvesuvio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 02:34:51.000000 mvesuvio-0.0.0.dev183/mvesuvio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/analysis_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.903732 mvesuvio-0.0.0.dev183/mvesuvio/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/Mantid.user.properties
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/analysis_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.903732 mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2018.par
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2018_2.par
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2018_3.par
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2019.par
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/config/vesuvio.user.properties
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.903732 mvesuvio-0.0.0.dev183/mvesuvio/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/scripts/handle_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.903732 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.907732 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_config/expr_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_jackknife.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_yspace_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_yspace_fit_GC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/system_tests/tests_IC.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.907732 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)    10860 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/ICHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41027 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/analysis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22158 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/bootstrap_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63650 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/fit_in_yspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/run_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.907732 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:34:51.907732 mvesuvio-0.0.0.dev183/mvesuvio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-23 02:34:51.000000 mvesuvio-0.0.0.dev183/mvesuvio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-23 02:34:51.000000 mvesuvio-0.0.0.dev183/mvesuvio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:34:51.000000 mvesuvio-0.0.0.dev183/mvesuvio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 02:34:51.000000 mvesuvio-0.0.0.dev183/mvesuvio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 02:34:51.000000 mvesuvio-0.0.0.dev183/mvesuvio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 02:34:51.000000 mvesuvio-0.0.0.dev183/mvesuvio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-23 02:19:57.000000 mvesuvio-0.0.0.dev183/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:34:51.907732 mvesuvio-0.0.0.dev183/setup.cfg
```

### Comparing `mvesuvio-0.0.0.dev181/PKG-INFO` & `mvesuvio-0.0.0.dev183/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvesuvio
-Version: 0.0.0.dev181
+Version: 0.0.0.dev183
 Summary: Analyse Vesuvio instrument data
 Author-email: The Mantid Project <mantid-help@mantidproject.org>, Guilherme Pereira <gui.maciel-pereira@stfc.ac.uk>, More Credit <here@stfc.ac.uk>
 Project-URL: Repository, https://github.com/mantidproject/vesuvio
 Project-URL: Bug Tracker, https://github.com/mantidproject/vesuvio/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -27,33 +27,30 @@
 - Vesuvio calibration script
 
 ## Install mvesuvio package
 
 ### For stand-alone (non-conda) Mantid installation
 Currently this method is tested up until Mantid 6.8. 
 
-The easiest way to install the package is to navigate to the installation folder of mantid on your desktop and go to the `bin` folder.
+The easiest way to install the package is to install it through pip.
+To pip install mvesuvio, follow these [instructions](https://docs.mantidproject.org/nightly/concepts/PipInstall.html) and replace `<insert_package_name>` with `mvesuvio`.
 
-You'll see that this folder has a `python` executable. Open up a terminal window from this directory and run the following command:
+Then open mantid workbench and in the editor run the following script:
 
-- `./python -m pip install mvesuvio`
-
-Please make sure that you're writing `./python` and not just `python`, as for the installation to work it needs to use the python executable 
-from this particular mantid installation.
-
-If the installation is successful, you should see that a new executable called `mvesuvio` has appeared in the `bin` folder.
-
-Then type the following command:
-
-- `./mvesuvio config`
+```
+import mvesuvio as mv
+mv.set_config()
+```
 
 You will see that the output shows two directories: one for the inputs file and another for the instrument parameters (IP) file.
 
 Both of these directories sit inside a default location of a `.mvesuvio` folder.
 
+The `.` in front of the directory name means this folder might be hidden by your OS, so you might have to turn on the option of showing hidden folders.
+
 You should place of your IP files inside this IP directory, you will notice that I have placed some example files in there already.
 
 The other directory in the output of the config command tells you which inputs file is being used for running the analysis.
 
 You should go to the directory of the inputs file and copy-and-paste this file into any directory inside your desktop where you want to run the analysis for a given sample.
 
 And that's the end of the installation and setup!
```

### Comparing `mvesuvio-0.0.0.dev181/README.md` & `mvesuvio-0.0.0.dev183/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 - Vesuvio calibration script
 
 ## Install mvesuvio package
 
 ### For stand-alone (non-conda) Mantid installation
 Currently this method is tested up until Mantid 6.8. 
 
-The easiest way to install the package is to navigate to the installation folder of mantid on your desktop and go to the `bin` folder.
+The easiest way to install the package is to install it through pip.
+To pip install mvesuvio, follow these [instructions](https://docs.mantidproject.org/nightly/concepts/PipInstall.html) and replace `<insert_package_name>` with `mvesuvio`.
 
-You'll see that this folder has a `python` executable. Open up a terminal window from this directory and run the following command:
+Then open mantid workbench and in the editor run the following script:
 
-- `./python -m pip install mvesuvio`
-
-Please make sure that you're writing `./python` and not just `python`, as for the installation to work it needs to use the python executable 
-from this particular mantid installation.
-
-If the installation is successful, you should see that a new executable called `mvesuvio` has appeared in the `bin` folder.
-
-Then type the following command:
-
-- `./mvesuvio config`
+```
+import mvesuvio as mv
+mv.set_config()
+```
 
 You will see that the output shows two directories: one for the inputs file and another for the instrument parameters (IP) file.
 
 Both of these directories sit inside a default location of a `.mvesuvio` folder.
 
+The `.` in front of the directory name means this folder might be hidden by your OS, so you might have to turn on the option of showing hidden folders.
+
 You should place of your IP files inside this IP directory, you will notice that I have placed some example files in there already.
 
 The other directory in the output of the config command tells you which inputs file is being used for running the analysis.
 
 You should go to the directory of the inputs file and copy-and-paste this file into any directory inside your desktop where you want to run the analysis for a given sample.
 
 And that's the end of the installation and setup!
```

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/__init__.py` & `mvesuvio-0.0.0.dev183/mvesuvio/__init__.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/analysis_runner.py` & `mvesuvio-0.0.0.dev183/mvesuvio/analysis_runner.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/config/analysis_inputs.py` & `mvesuvio-0.0.0.dev183/mvesuvio/config/analysis_inputs.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018.par` & `mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2018.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_2.par` & `mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2018_2.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2018_3.par` & `mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2018_3.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/config/ip_files/ip2019.par` & `mvesuvio-0.0.0.dev183/mvesuvio/config/ip_files/ip2019.par`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/scripts/__init__.py` & `mvesuvio-0.0.0.dev183/mvesuvio/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/scripts/handle_config.py` & `mvesuvio-0.0.0.dev183/mvesuvio/scripts/handle_config.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_analysis.py` & `mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_bootstrap.py` & `mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_config/expr_for_tests.py` & `mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_config/expr_for_tests.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_jackknife.py` & `mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_jackknife.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_yspace_fit.py` & `mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_yspace_fit.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/test_yspace_fit_GC.py` & `mvesuvio-0.0.0.dev183/mvesuvio/system_tests/test_yspace_fit_GC.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/system_tests/tests_IC.py` & `mvesuvio-0.0.0.dev183/mvesuvio/system_tests/tests_IC.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/ICHelpers.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/ICHelpers.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/analysis_functions.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/bootstrap.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/bootstrap_analysis.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/bootstrap_analysis.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/deprecated_mantid_global_fit.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/fit_in_yspace.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/fit_in_yspace.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/procedures.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/procedures.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/run_script.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/run_script.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py` & `mvesuvio-0.0.0.dev183/mvesuvio/vesuvio_analysis/tests/test_analysis_functions.py`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio.egg-info/PKG-INFO` & `mvesuvio-0.0.0.dev183/mvesuvio.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvesuvio
-Version: 0.0.0.dev181
+Version: 0.0.0.dev183
 Summary: Analyse Vesuvio instrument data
 Author-email: The Mantid Project <mantid-help@mantidproject.org>, Guilherme Pereira <gui.maciel-pereira@stfc.ac.uk>, More Credit <here@stfc.ac.uk>
 Project-URL: Repository, https://github.com/mantidproject/vesuvio
 Project-URL: Bug Tracker, https://github.com/mantidproject/vesuvio/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -27,33 +27,30 @@
 - Vesuvio calibration script
 
 ## Install mvesuvio package
 
 ### For stand-alone (non-conda) Mantid installation
 Currently this method is tested up until Mantid 6.8. 
 
-The easiest way to install the package is to navigate to the installation folder of mantid on your desktop and go to the `bin` folder.
+The easiest way to install the package is to install it through pip.
+To pip install mvesuvio, follow these [instructions](https://docs.mantidproject.org/nightly/concepts/PipInstall.html) and replace `<insert_package_name>` with `mvesuvio`.
 
-You'll see that this folder has a `python` executable. Open up a terminal window from this directory and run the following command:
+Then open mantid workbench and in the editor run the following script:
 
-- `./python -m pip install mvesuvio`
-
-Please make sure that you're writing `./python` and not just `python`, as for the installation to work it needs to use the python executable 
-from this particular mantid installation.
-
-If the installation is successful, you should see that a new executable called `mvesuvio` has appeared in the `bin` folder.
-
-Then type the following command:
-
-- `./mvesuvio config`
+```
+import mvesuvio as mv
+mv.set_config()
+```
 
 You will see that the output shows two directories: one for the inputs file and another for the instrument parameters (IP) file.
 
 Both of these directories sit inside a default location of a `.mvesuvio` folder.
 
+The `.` in front of the directory name means this folder might be hidden by your OS, so you might have to turn on the option of showing hidden folders.
+
 You should place of your IP files inside this IP directory, you will notice that I have placed some example files in there already.
 
 The other directory in the output of the config command tells you which inputs file is being used for running the analysis.
 
 You should go to the directory of the inputs file and copy-and-paste this file into any directory inside your desktop where you want to run the analysis for a given sample.
 
 And that's the end of the installation and setup!
```

### Comparing `mvesuvio-0.0.0.dev181/mvesuvio.egg-info/SOURCES.txt` & `mvesuvio-0.0.0.dev183/mvesuvio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvesuvio-0.0.0.dev181/pyproject.toml` & `mvesuvio-0.0.0.dev183/pyproject.toml`

 * *Files identical despite different names*

