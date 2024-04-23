# Comparing `tmp/tdprepview-1.4.0.tar.gz` & `tmp/tdprepview-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdprepview-1.4.0.tar", last modified: Tue Apr  9 09:27:19 2024, max compression
+gzip compressed data, was "tdprepview-1.4.1.tar", last modified: Tue Apr 23 12:14:30 2024, max compression
```

## Comparing `tdprepview-1.4.0.tar` & `tdprepview-1.4.1.tar`

### file list

```diff
@@ -1,74 +1,76 @@
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.280473 tdprepview-1.4.0/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      135 2024-02-29 18:16:39.000000 tdprepview-1.4.0/AUTHORS.md
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    35148 2024-02-29 18:16:39.000000 tdprepview-1.4.0/LICENSE
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      271 2024-02-29 18:16:39.000000 tdprepview-1.4.0/MANIFEST.in
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    11993 2024-04-09 09:27:19.280063 tdprepview-1.4.0/PKG-INFO
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5709 2024-03-26 09:24:33.000000 tdprepview-1.4.0/README.md
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.082471 tdprepview-1.4.0/docs/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      611 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/Makefile
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/authors.rst
--rwxr-xr-x   0 martin.hillebrand   (502) staff       (20)     4832 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/conf.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       33 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/contributing.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)   521877 2024-03-20 17:24:59.000000 tdprepview-1.4.0/docs/deployment_infrastructure.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    66135 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/example_sankey.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/history.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      307 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/index.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      549 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/installation.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      808 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/make.bat
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       28 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/readme.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)   405456 2024-03-20 17:14:35.000000 tdprepview-1.4.0/docs/supportedpreprocessors_v130.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)   407482 2024-03-26 09:19:30.000000 tdprepview-1.4.0/docs/supportedpreprocessors_v131.png
--rwxrwxrwx   0 martin.hillebrand   (502) staff       (20)    91544 2023-03-07 08:54:58.000000 tdprepview-1.4.0/docs/tdprepview_logo.png
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       76 2024-02-29 18:16:39.000000 tdprepview-1.4.0/docs/usage.rst
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      427 2024-04-09 09:27:19.282058 tdprepview-1.4.0/setup.cfg
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1731 2024-04-08 14:42:16.000000 tdprepview-1.4.0/setup.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.084915 tdprepview-1.4.0/tdprepview/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      595 2024-04-09 08:17:52.000000 tdprepview-1.4.0/tdprepview/__init__.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.100085 tdprepview-1.4.0/tdprepview/autoprep/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-04-05 14:49:36.000000 tdprepview-1.4.0/tdprepview/autoprep/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5060 2024-04-09 08:51:25.000000 tdprepview-1.4.0/tdprepview/autoprep/_builder.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     4609 2024-04-05 14:53:25.000000 tdprepview-1.4.0/tdprepview/autoprep/_checker.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.125359 tdprepview-1.4.0/tdprepview/pipeline/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    13568 2024-03-06 11:46:59.000000 tdprepview-1.4.0/tdprepview/pipeline/_DAG.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/pipeline/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    22634 2024-04-08 13:05:42.000000 tdprepview-1.4.0/tdprepview/pipeline/_pipeline.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3291 2024-04-02 07:47:11.000000 tdprepview-1.4.0/tdprepview/pipeline/_plotter.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     4652 2024-03-27 16:52:11.000000 tdprepview-1.4.0/tdprepview/pipeline/_serializer.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5679 2024-03-01 15:12:39.000000 tdprepview-1.4.0/tdprepview/pipeline/_utils.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.185377 tdprepview-1.4.0/tdprepview/preprocessing/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2033 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_TODO.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1358 2024-03-27 16:27:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2587 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_dimensionality_reduction.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    19880 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_discretize.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9610 2024-04-09 09:01:36.000000 tdprepview-1.4.0/tdprepview/preprocessing/_features.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2320 2024-03-01 12:37:27.000000 tdprepview-1.4.0/tdprepview/preprocessing/_hashing.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9407 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_impute.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3989 2024-03-06 12:03:25.000000 tdprepview-1.4.0/tdprepview/preprocessing/_miscellaneous.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2670 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_preprocessing.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    24391 2024-03-25 17:15:35.000000 tdprepview-1.4.0/tdprepview/preprocessing/_transform.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1982 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/preprocessing/_utils.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.193712 tdprepview-1.4.0/tdprepview/sql/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      497 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/__init__.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.233649 tdprepview-1.4.0/tdprepview/sql/generator/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/generator/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)      430 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/generator/_utils.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     6556 2024-04-09 09:01:36.000000 tdprepview-1.4.0/tdprepview/sql/generator/multicol.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    15100 2024-03-26 08:23:10.000000 tdprepview-1.4.0/tdprepview/sql/generator/singlecol.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.246933 tdprepview-1.4.0/tdprepview/sql/templates/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       56 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/templates/from.sql
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       97 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/templates/replaceview.sql
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       98 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/sql/templates/withas.sql
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.266541 tdprepview-1.4.0/tdprepview/statistics/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/statistics/__init__.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5336 2024-03-25 17:17:48.000000 tdprepview-1.4.0/tdprepview/statistics/collector.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2904 2024-03-25 16:46:47.000000 tdprepview-1.4.0/tdprepview/statistics/collector_sklearn.py
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     7526 2024-03-19 13:21:24.000000 tdprepview-1.4.0/tdprepview/statistics/collector_vantage.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.279082 tdprepview-1.4.0/tdprepview/tests/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.0/tdprepview/tests/__init__.py
-drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-09 09:27:19.092039 tdprepview-1.4.0/tdprepview.egg-info/
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)    11993 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/PKG-INFO
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1798 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/SOURCES.txt
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/dependency_links.txt
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-03-01 15:56:38.000000 tdprepview-1.4.0/tdprepview.egg-info/not-zip-safe
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       91 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/requires.txt
--rw-r--r--   0 martin.hillebrand   (502) staff       (20)       11 2024-04-09 09:27:18.000000 tdprepview-1.4.0/tdprepview.egg-info/top_level.txt
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.712674 tdprepview-1.4.1/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      135 2024-02-29 18:16:39.000000 tdprepview-1.4.1/AUTHORS.md
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    35148 2024-02-29 18:16:39.000000 tdprepview-1.4.1/LICENSE
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      271 2024-02-29 18:16:39.000000 tdprepview-1.4.1/MANIFEST.in
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    12101 2024-04-23 12:14:30.711682 tdprepview-1.4.1/PKG-INFO
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5838 2024-04-09 17:16:52.000000 tdprepview-1.4.1/README.md
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.327600 tdprepview-1.4.1/docs/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      611 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/Makefile
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/authors.rst
+-rwxr-xr-x   0 martin.hillebrand   (502) staff       (20)     4832 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/conf.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       33 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/contributing.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)   521877 2024-03-20 17:24:59.000000 tdprepview-1.4.1/docs/deployment_infrastructure.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    66135 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/example_sankey.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       29 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/history.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      307 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/index.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      549 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/installation.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      808 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/make.bat
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       28 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/readme.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)   405456 2024-03-20 17:14:35.000000 tdprepview-1.4.1/docs/supportedpreprocessors_v130.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)   407482 2024-03-26 09:19:30.000000 tdprepview-1.4.1/docs/supportedpreprocessors_v131.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)   454972 2024-04-16 13:19:05.000000 tdprepview-1.4.1/docs/tdprepview_intro.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    52004 2024-04-16 13:33:54.000000 tdprepview-1.4.1/docs/tdprepview_intro_last.png
+-rwxrwxrwx   0 martin.hillebrand   (502) staff       (20)    91544 2023-03-07 08:54:58.000000 tdprepview-1.4.1/docs/tdprepview_logo.png
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       76 2024-02-29 18:16:39.000000 tdprepview-1.4.1/docs/usage.rst
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      427 2024-04-23 12:14:30.718382 tdprepview-1.4.1/setup.cfg
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1731 2024-04-23 12:14:07.000000 tdprepview-1.4.1/setup.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.329124 tdprepview-1.4.1/tdprepview/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      595 2024-04-23 12:14:07.000000 tdprepview-1.4.1/tdprepview/__init__.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.376731 tdprepview-1.4.1/tdprepview/autoprep/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-04-05 14:49:36.000000 tdprepview-1.4.1/tdprepview/autoprep/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5060 2024-04-09 08:51:25.000000 tdprepview-1.4.1/tdprepview/autoprep/_builder.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     4609 2024-04-05 14:53:25.000000 tdprepview-1.4.1/tdprepview/autoprep/_checker.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.467408 tdprepview-1.4.1/tdprepview/pipeline/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    13568 2024-03-06 11:46:59.000000 tdprepview-1.4.1/tdprepview/pipeline/_DAG.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/pipeline/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    22634 2024-04-08 13:05:42.000000 tdprepview-1.4.1/tdprepview/pipeline/_pipeline.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3291 2024-04-02 07:47:11.000000 tdprepview-1.4.1/tdprepview/pipeline/_plotter.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     4652 2024-03-27 16:52:11.000000 tdprepview-1.4.1/tdprepview/pipeline/_serializer.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5679 2024-03-01 15:12:39.000000 tdprepview-1.4.1/tdprepview/pipeline/_utils.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.579377 tdprepview-1.4.1/tdprepview/preprocessing/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2033 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/preprocessing/_TODO.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1358 2024-03-27 16:27:39.000000 tdprepview-1.4.1/tdprepview/preprocessing/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2587 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/preprocessing/_dimensionality_reduction.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    19880 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/preprocessing/_discretize.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9610 2024-04-09 09:01:36.000000 tdprepview-1.4.1/tdprepview/preprocessing/_features.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2320 2024-03-01 12:37:27.000000 tdprepview-1.4.1/tdprepview/preprocessing/_hashing.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     9407 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/preprocessing/_impute.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     3989 2024-03-06 12:03:25.000000 tdprepview-1.4.1/tdprepview/preprocessing/_miscellaneous.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2670 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/preprocessing/_preprocessing.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    24391 2024-03-25 17:15:35.000000 tdprepview-1.4.1/tdprepview/preprocessing/_transform.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1982 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/preprocessing/_utils.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.591425 tdprepview-1.4.1/tdprepview/sql/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      497 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/sql/__init__.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.651145 tdprepview-1.4.1/tdprepview/sql/generator/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/sql/generator/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)      430 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/sql/generator/_utils.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     6556 2024-04-09 09:01:36.000000 tdprepview-1.4.1/tdprepview/sql/generator/multicol.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    15100 2024-03-26 08:23:10.000000 tdprepview-1.4.1/tdprepview/sql/generator/singlecol.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.667977 tdprepview-1.4.1/tdprepview/sql/templates/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       56 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/sql/templates/from.sql
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       97 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/sql/templates/replaceview.sql
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       98 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/sql/templates/withas.sql
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.695902 tdprepview-1.4.1/tdprepview/statistics/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/statistics/__init__.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     5336 2024-03-25 17:17:48.000000 tdprepview-1.4.1/tdprepview/statistics/collector.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     2904 2024-03-25 16:46:47.000000 tdprepview-1.4.1/tdprepview/statistics/collector_sklearn.py
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     8160 2024-04-22 15:49:37.000000 tdprepview-1.4.1/tdprepview/statistics/collector_vantage.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.709744 tdprepview-1.4.1/tdprepview/tests/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        0 2024-02-29 18:16:39.000000 tdprepview-1.4.1/tdprepview/tests/__init__.py
+drwxr-xr-x   0 martin.hillebrand   (502) staff       (20)        0 2024-04-23 12:14:30.344792 tdprepview-1.4.1/tdprepview.egg-info/
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)    12101 2024-04-23 12:14:29.000000 tdprepview-1.4.1/tdprepview.egg-info/PKG-INFO
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)     1855 2024-04-23 12:14:29.000000 tdprepview-1.4.1/tdprepview.egg-info/SOURCES.txt
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-04-23 12:14:29.000000 tdprepview-1.4.1/tdprepview.egg-info/dependency_links.txt
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)        1 2024-03-01 15:56:38.000000 tdprepview-1.4.1/tdprepview.egg-info/not-zip-safe
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       91 2024-04-23 12:14:29.000000 tdprepview-1.4.1/tdprepview.egg-info/requires.txt
+-rw-r--r--   0 martin.hillebrand   (502) staff       (20)       11 2024-04-23 12:14:29.000000 tdprepview-1.4.1/tdprepview.egg-info/top_level.txt
```

### Comparing `tdprepview-1.4.0/LICENSE` & `tdprepview-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/PKG-INFO` & `tdprepview-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdprepview
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python Package that creates Data Preparation Pipeline in Teradata-SQL in Views
 Author: Martin Hillebrand
 Author-email: martin.hillebrand@teradata.com
 Keywords: tdprepview,teradata,database,preprocessing,data engineering,data science
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -33,21 +33,23 @@
 # tdprepview
 
 Python Package that creates Data Preparation Pipelines in Views written in Teradata-SQL.
 
 ## Installation
 
 
-* pip install tdprepview
+* `pip install tdprepview`
 
 ## Features
 
 * Pipeline class that allows creating in-DB preprocessing pipelines
 * Several Preprocessor functions
 * API similar to sklearn.Pipeline
+* Pipeline can be saved and loaded as dict/json
+* Pipeline can be automatically created based on data types and distributions.
 
 ![Preprocessors](https://raw.githubusercontent.com/martinhillebrand/tdprepview/main/media/supportedpreprocessors_v131.png)
 
 
 ## Quickstart
 
 ### 1. setting up the pipeline
@@ -333,14 +335,14 @@
 ## v1.4.0 (2024-04-08)
 
 Introducing automatic Pipeline creation based on heuristics. Either via `Pipeline.from_DataFrame(...)` or via `auto_code(...)`
 
 ### added
 
 * Pipeline can now automatically created based on a tdml.DataFrame 
-  * `mypipeline = Pipeline.from_DataFrame(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * `mypipeline = Pipeline.from_DataFrame(DF, non_feature_cols=["rowid","target"], fit_pipeline=True)`
   * It'll use heuristics based on datatypes and distributions to decide which preprocessing function would make sense.
 * If you only want to see the code for the `steps` parameter, you can use
-  * `steps_str = auto_code(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * `steps_str = auto_code(DF, non_feature_cols=["rowid","target"])`
   * `print(steps_str) # see steps and adjust if needed...` 
   * `steps = eval(steps_str)`
   * `mypipeline = Pipeline(steps)`
```

### Comparing `tdprepview-1.4.0/README.md` & `tdprepview-1.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 # tdprepview
 
 Python Package that creates Data Preparation Pipelines in Views written in Teradata-SQL.
 
 ## Installation
 
 
-* pip install tdprepview
+* `pip install tdprepview`
 
 ## Features
 
 * Pipeline class that allows creating in-DB preprocessing pipelines
 * Several Preprocessor functions
 * API similar to sklearn.Pipeline
+* Pipeline can be saved and loaded as dict/json
+* Pipeline can be automatically created based on data types and distributions.
 
 ![Preprocessors](https://raw.githubusercontent.com/martinhillebrand/tdprepview/main/media/supportedpreprocessors_v131.png)
 
 
 ## Quickstart
 
 ### 1. setting up the pipeline
```

### Comparing `tdprepview-1.4.0/docs/Makefile` & `tdprepview-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/conf.py` & `tdprepview-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/deployment_infrastructure.png` & `tdprepview-1.4.1/docs/deployment_infrastructure.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/example_sankey.png` & `tdprepview-1.4.1/docs/example_sankey.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/installation.rst` & `tdprepview-1.4.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/make.bat` & `tdprepview-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/supportedpreprocessors_v130.png` & `tdprepview-1.4.1/docs/supportedpreprocessors_v130.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/supportedpreprocessors_v131.png` & `tdprepview-1.4.1/docs/supportedpreprocessors_v131.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/docs/tdprepview_logo.png` & `tdprepview-1.4.1/docs/tdprepview_logo.png`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/setup.py` & `tdprepview-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'plot': ["plotly>=5.0", "seaborn>=0.11"]
 }
 
 # test_requirements = ['pytest>=3', ]
 
 setup(
     name='tdprepview',
-    version='1.4.0',
+    version='1.4.1',
     description="Python Package that creates Data Preparation Pipeline in Teradata-SQL in Views",
 
     author="Martin Hillebrand",
     author_email='martin.hillebrand@teradata.com',
 
     packages=find_packages(include=['tdprepview', 'tdprepview.*']),
```

### Comparing `tdprepview-1.4.0/tdprepview/__init__.py` & `tdprepview-1.4.1/tdprepview/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 and transforming re-usable data preparation pipelines that are
 saved in view definitions. Hence, no other permanent database objects
 are required.
 """
 
 __author__ = """Martin Hillebrand"""
 __email__ = 'martin.hillebrand@teradata.com'
-__version__ = '1.4.0'
+__version__ = '1.4.1'
 
 from .pipeline._pipeline import Pipeline
 from .preprocessing import *
 from . import preprocessing
 from .autoprep._builder import auto_code
 
 __all__ = [
```

### Comparing `tdprepview-1.4.0/tdprepview/autoprep/_builder.py` & `tdprepview-1.4.1/tdprepview/autoprep/_builder.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/autoprep/_checker.py` & `tdprepview-1.4.1/tdprepview/autoprep/_checker.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/pipeline/_DAG.py` & `tdprepview-1.4.1/tdprepview/pipeline/_DAG.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/pipeline/_pipeline.py` & `tdprepview-1.4.1/tdprepview/pipeline/_pipeline.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/pipeline/_plotter.py` & `tdprepview-1.4.1/tdprepview/pipeline/_plotter.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/pipeline/_serializer.py` & `tdprepview-1.4.1/tdprepview/pipeline/_serializer.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/pipeline/_utils.py` & `tdprepview-1.4.1/tdprepview/pipeline/_utils.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_TODO.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_TODO.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/__init__.py` & `tdprepview-1.4.1/tdprepview/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_dimensionality_reduction.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_discretize.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_discretize.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_features.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_features.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_hashing.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_hashing.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_impute.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_impute.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_miscellaneous.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_miscellaneous.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_preprocessing.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_transform.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_transform.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/preprocessing/_utils.py` & `tdprepview-1.4.1/tdprepview/preprocessing/_utils.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/sql/generator/multicol.py` & `tdprepview-1.4.1/tdprepview/sql/generator/multicol.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/sql/generator/singlecol.py` & `tdprepview-1.4.1/tdprepview/sql/generator/singlecol.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/statistics/collector.py` & `tdprepview-1.4.1/tdprepview/statistics/collector.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/statistics/collector_sklearn.py` & `tdprepview-1.4.1/tdprepview/statistics/collector_sklearn.py`

 * *Files identical despite different names*

### Comparing `tdprepview-1.4.0/tdprepview/statistics/collector_vantage.py` & `tdprepview-1.4.1/tdprepview/statistics/collector_vantage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 import pandas as pd
 import teradataml as tdml
 from numpy import dtype
+from urllib.parse import urlparse, parse_qs
+
+def _get_user_name():
+    eng = tdml.get_context()
+    username = ""
+    try:
+        username = eng.url.username
+    except:
+        pass
+    if username == "":
+        url_str = str(eng.url)
+        parsed_url = urlparse(url_str)
+        query_params = parse_qs(parsed_url.query)
+        username = query_params.get('user')[0] if 'user' in query_params else ""
+
+    assert username != "", "username cannot be inferred from engine-url"
+
+    return username
+
 
 def get_numeric_statistics(DF:tdml.DataFrame, cols_standard, cols_median_percentile, centiles)  -> pd.DataFrame:
     # tdml.UnivariateStatistics requires Database Version >= 17.10.x.x
 
     res_df = pd.DataFrame({'ATTRIBUTE': pd.Series(dtype=dtype('O')),
                        'StatName': pd.Series(dtype=dtype('O')),
                        'StatValue': pd.Series(dtype=dtype('float64'))})
@@ -15,15 +34,16 @@
                 newdata = DF,
                 target_columns=cols_standard,
                 stats=["MEAN","MAX","MIN","MODE","STD"]
                 ).result.to_pandas()
         except:
             DF_limited = DF.select(cols_standard)
             DF_limited.to_sql("inbetweenres", temporary=True, if_exists="replace")
-            DF_limited = tdml.DataFrame("inbetweenres")
+            username = _get_user_name()
+            DF_limited = tdml.DataFrame(tdml.in_schema(username,"inbetweenres"))
             df_stats1 = tdml.UnivariateStatistics(
                 newdata=DF_limited,
                 target_columns=cols_standard,
                 stats=["MEAN", "MAX", "MIN", "MODE", "STD"]
             ).result.to_pandas()
 
         res_df = pd.concat([res_df, df_stats1])
@@ -38,15 +58,16 @@
                 target_columns=cols_median_percentile,
                 stats=["MEAN","MAX","MIN","MODE","STD", "MEDIAN", "PERCENTILES"],
                 centiles=centiles,
                 ).result.to_pandas()
         except:
             DF_limited = DF.select(cols_median_percentile)
             DF_limited.to_sql("inbetweenres", temporary=True, if_exists="replace")
-            DF_limited = tdml.DataFrame("inbetweenres")
+            username = _get_user_name()
+            DF_limited = tdml.DataFrame(tdml.in_schema(username,"inbetweenres"))
             df_stats2 = tdml.UnivariateStatistics(
                 newdata=DF_limited,
                 target_columns=cols_median_percentile,
                 stats=["MEAN","MAX","MIN","MODE","STD", "MEDIAN", "PERCENTILES"],
                 centiles=centiles,
                 ).result.to_pandas()
```

### Comparing `tdprepview-1.4.0/tdprepview.egg-info/PKG-INFO` & `tdprepview-1.4.1/tdprepview.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdprepview
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python Package that creates Data Preparation Pipeline in Teradata-SQL in Views
 Author: Martin Hillebrand
 Author-email: martin.hillebrand@teradata.com
 Keywords: tdprepview,teradata,database,preprocessing,data engineering,data science
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -33,21 +33,23 @@
 # tdprepview
 
 Python Package that creates Data Preparation Pipelines in Views written in Teradata-SQL.
 
 ## Installation
 
 
-* pip install tdprepview
+* `pip install tdprepview`
 
 ## Features
 
 * Pipeline class that allows creating in-DB preprocessing pipelines
 * Several Preprocessor functions
 * API similar to sklearn.Pipeline
+* Pipeline can be saved and loaded as dict/json
+* Pipeline can be automatically created based on data types and distributions.
 
 ![Preprocessors](https://raw.githubusercontent.com/martinhillebrand/tdprepview/main/media/supportedpreprocessors_v131.png)
 
 
 ## Quickstart
 
 ### 1. setting up the pipeline
@@ -333,14 +335,14 @@
 ## v1.4.0 (2024-04-08)
 
 Introducing automatic Pipeline creation based on heuristics. Either via `Pipeline.from_DataFrame(...)` or via `auto_code(...)`
 
 ### added
 
 * Pipeline can now automatically created based on a tdml.DataFrame 
-  * `mypipeline = Pipeline.from_DataFrame(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * `mypipeline = Pipeline.from_DataFrame(DF, non_feature_cols=["rowid","target"], fit_pipeline=True)`
   * It'll use heuristics based on datatypes and distributions to decide which preprocessing function would make sense.
 * If you only want to see the code for the `steps` parameter, you can use
-  * `steps_str = auto_code(DF, non_feature_cols=["rowid","target"], fit_pipeline=True))`
+  * `steps_str = auto_code(DF, non_feature_cols=["rowid","target"])`
   * `print(steps_str) # see steps and adjust if needed...` 
   * `steps = eval(steps_str)`
   * `mypipeline = Pipeline(steps)`
```

### Comparing `tdprepview-1.4.0/tdprepview.egg-info/SOURCES.txt` & `tdprepview-1.4.1/tdprepview.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/supportedpreprocessors_v130.png
 docs/supportedpreprocessors_v131.png
+docs/tdprepview_intro.png
+docs/tdprepview_intro_last.png
 docs/tdprepview_logo.png
 docs/usage.rst
 tdprepview/__init__.py
 tdprepview.egg-info/PKG-INFO
 tdprepview.egg-info/SOURCES.txt
 tdprepview.egg-info/dependency_links.txt
 tdprepview.egg-info/not-zip-safe
```

