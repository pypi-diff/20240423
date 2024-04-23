# Comparing `tmp/fscan-0.3.5.tar.gz` & `tmp/fscan-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fscan-0.3.5.tar", last modified: Sat Feb 17 00:13:25 2024, max compression
+gzip compressed data, was "fscan-0.3.6.tar", last modified: Tue Apr 23 00:59:34 2024, max compression
```

## Comparing `fscan-0.3.5.tar` & `fscan-0.3.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.208689 fscan-0.3.5/
--rw-r--r--   0 egoetz     (501) staff       (20)       87 2023-10-30 21:32:21.000000 fscan-0.3.5/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)      208 2023-10-30 21:32:21.000000 fscan-0.3.5/.gitlab-ci.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     6398 2022-10-18 23:51:06.000000 fscan-0.3.5/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35150 2023-10-30 21:32:21.000000 fscan-0.3.5/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       26 2023-10-30 21:32:21.000000 fscan-0.3.5/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     2515 2024-02-17 00:13:25.208235 fscan-0.3.5/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     1198 2023-11-23 17:48:55.000000 fscan-0.3.5/README.md
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.176270 fscan-0.3.5/condor-production/
--rwxr-xr-x   0 egoetz     (501) staff       (20)      811 2023-12-01 19:10:14.000000 fscan-0.3.5/condor-production/fscan_clean
--rw-r--r--   0 egoetz     (501) staff       (20)      559 2023-10-31 16:39:10.000000 fscan-0.3.5/condor-production/fscan_clean.sub
--rwxr-xr-x   0 egoetz     (501) staff       (20)      775 2023-12-01 19:10:14.000000 fscan-0.3.5/condor-production/fscan_daily
--rw-r--r--   0 egoetz     (501) staff       (20)      557 2023-10-31 16:39:10.000000 fscan-0.3.5/condor-production/fscan_daily.sub
--rwxr-xr-x   0 egoetz     (501) staff       (20)      807 2023-12-01 19:10:14.000000 fscan-0.3.5/condor-production/fscan_monthly
--rw-r--r--   0 egoetz     (501) staff       (20)      563 2023-10-31 16:39:10.000000 fscan-0.3.5/condor-production/fscan_monthly.sub
--rwxr-xr-x   0 egoetz     (501) staff       (20)      809 2023-12-01 19:10:14.000000 fscan-0.3.5/condor-production/fscan_weekly
--rw-r--r--   0 egoetz     (501) staff       (20)      560 2023-10-31 16:39:10.000000 fscan-0.3.5/condor-production/fscan_weekly.sub
--rwxr-xr-x   0 egoetz     (501) staff       (20)     1123 2023-12-19 17:13:59.000000 fscan-0.3.5/condor-production/status_summary_daily
--rw-r--r--   0 egoetz     (501) staff       (20)      598 2023-10-31 16:39:10.000000 fscan-0.3.5/condor-production/status_summary_daily.sub
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.163229 fscan-0.3.5/configuration/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.178007 fscan-0.3.5/configuration/examples/
--rw-r--r--   0 egoetz     (501) staff       (20)      853 2023-12-06 01:45:06.000000 fscan-0.3.5/configuration/examples/example.config
--rw-r--r--   0 egoetz     (501) staff       (20)     1115 2023-11-23 17:48:55.000000 fscan-0.3.5/configuration/examples/example_ch_info.yml
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.180122 fscan-0.3.5/configuration/production/
--rw-r--r--   0 egoetz     (501) staff       (20)    27458 2023-11-23 17:48:55.000000 fscan-0.3.5/configuration/production/O4_H1_Fscan_ch_info.yml
--rw-r--r--   0 egoetz     (501) staff       (20)    19747 2023-09-28 21:20:11.000000 fscan-0.3.5/configuration/production/O4_L1_Fscan_ch_info.yml
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.187523 fscan-0.3.5/fscan/
--rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-11-22 00:29:13.000000 fscan-0.3.5/fscan/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15823 2024-02-15 01:09:24.000000 fscan-0.3.5/fscan/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-02-17 00:13:25.000000 fscan-0.3.5/fscan/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)    19326 2024-02-17 00:13:02.000000 fscan-0.3.5/fscan/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4069 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/clean.py
--rw-r--r--   0 egoetz     (501) staff       (20)    31861 2024-02-15 01:09:24.000000 fscan-0.3.5/fscan/html.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.193003 fscan-0.3.5/fscan/plot/
--rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-11-22 00:29:19.000000 fscan-0.3.5/fscan/plot/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    25030 2024-02-17 00:13:02.000000 fscan-0.3.5/fscan/plot/finetoothplot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10296 2024-02-02 19:33:13.000000 fscan-0.3.5/fscan/plot/static.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13999 2024-02-15 00:23:30.000000 fscan-0.3.5/fscan/post.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.200344 fscan-0.3.5/fscan/process/
--rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/process/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    11838 2023-11-23 17:48:55.000000 fscan-0.3.5/fscan/process/autotag.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9735 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/process/combfinder.py
--rw-r--r--   0 egoetz     (501) staff       (20)    16509 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/process/linecount.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7097 2024-02-03 01:10:22.000000 fscan-0.3.5/fscan/process/linefinder.py
--rw-r--r--   0 egoetz     (501) staff       (20)    18754 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/process/lineobjects.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9195 2024-02-15 00:23:30.000000 fscan-0.3.5/fscan/process/spectlinetools.py
--rw-r--r--   0 egoetz     (501) staff       (20)    27049 2023-12-19 17:13:59.000000 fscan-0.3.5/fscan/status.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.206534 fscan-0.3.5/fscan/utils/
--rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/utils/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2603 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/utils/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    35814 2024-02-15 01:09:24.000000 fscan-0.3.5/fscan/utils/dtutils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3819 2024-01-06 01:38:41.000000 fscan-0.3.5/fscan/utils/io.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5753 2024-02-17 00:13:02.000000 fscan-0.3.5/fscan/utils/reuse.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5732 2023-10-30 21:32:21.000000 fscan-0.3.5/fscan/utils/segments.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5559 2024-02-15 01:09:24.000000 fscan-0.3.5/fscan/utils/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-02-17 00:13:25.207229 fscan-0.3.5/fscan.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     2515 2024-02-17 00:13:25.000000 fscan-0.3.5/fscan.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     1330 2024-02-17 00:13:25.000000 fscan-0.3.5/fscan.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-02-17 00:13:25.000000 fscan-0.3.5/fscan.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      352 2024-02-17 00:13:25.000000 fscan-0.3.5/fscan.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       66 2024-02-17 00:13:25.000000 fscan-0.3.5/fscan.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        6 2024-02-17 00:13:25.000000 fscan-0.3.5/fscan.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     1930 2024-01-26 19:41:27.000000 fscan-0.3.5/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-02-17 00:13:25.208773 fscan-0.3.5/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.949343 fscan-0.3.6/
+-rw-r--r--   0 egoetz     (501) staff       (20)       87 2023-10-30 21:32:21.000000 fscan-0.3.6/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)      208 2023-10-30 21:32:21.000000 fscan-0.3.6/.gitlab-ci.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     6398 2022-10-18 23:51:06.000000 fscan-0.3.6/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35150 2023-10-30 21:32:21.000000 fscan-0.3.6/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       26 2023-10-30 21:32:21.000000 fscan-0.3.6/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     2515 2024-04-23 00:59:34.948565 fscan-0.3.6/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     1198 2023-11-23 17:48:55.000000 fscan-0.3.6/README.md
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.920951 fscan-0.3.6/condor-production/
+-rwxr-xr-x   0 egoetz     (501) staff       (20)      811 2023-12-01 19:10:14.000000 fscan-0.3.6/condor-production/fscan_clean
+-rw-r--r--   0 egoetz     (501) staff       (20)      559 2023-10-31 16:39:10.000000 fscan-0.3.6/condor-production/fscan_clean.sub
+-rwxr-xr-x   0 egoetz     (501) staff       (20)      685 2024-04-18 21:58:55.000000 fscan-0.3.6/condor-production/fscan_daily
+-rw-r--r--   0 egoetz     (501) staff       (20)      557 2023-10-31 16:39:10.000000 fscan-0.3.6/condor-production/fscan_daily.sub
+-rwxr-xr-x   0 egoetz     (501) staff       (20)      718 2024-04-18 21:58:55.000000 fscan-0.3.6/condor-production/fscan_monthly
+-rw-r--r--   0 egoetz     (501) staff       (20)      563 2023-10-31 16:39:10.000000 fscan-0.3.6/condor-production/fscan_monthly.sub
+-rwxr-xr-x   0 egoetz     (501) staff       (20)      719 2024-04-18 21:58:55.000000 fscan-0.3.6/condor-production/fscan_weekly
+-rw-r--r--   0 egoetz     (501) staff       (20)      560 2023-10-31 16:39:10.000000 fscan-0.3.6/condor-production/fscan_weekly.sub
+-rwxr-xr-x   0 egoetz     (501) staff       (20)     1123 2023-12-19 17:13:59.000000 fscan-0.3.6/condor-production/status_summary_daily
+-rw-r--r--   0 egoetz     (501) staff       (20)      598 2023-10-31 16:39:10.000000 fscan-0.3.6/condor-production/status_summary_daily.sub
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.911012 fscan-0.3.6/configuration/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.922241 fscan-0.3.6/configuration/examples/
+-rw-r--r--   0 egoetz     (501) staff       (20)      853 2023-12-06 01:45:06.000000 fscan-0.3.6/configuration/examples/example.config
+-rw-r--r--   0 egoetz     (501) staff       (20)     1115 2023-11-23 17:48:55.000000 fscan-0.3.6/configuration/examples/example_ch_info.yml
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.923724 fscan-0.3.6/configuration/production/
+-rw-r--r--   0 egoetz     (501) staff       (20)    27458 2023-11-23 17:48:55.000000 fscan-0.3.6/configuration/production/O4_H1_Fscan_ch_info.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)    19747 2023-09-28 21:20:11.000000 fscan-0.3.6/configuration/production/O4_L1_Fscan_ch_info.yml
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.928910 fscan-0.3.6/fscan/
+-rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-11-22 00:29:13.000000 fscan-0.3.6/fscan/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15802 2024-04-18 22:02:10.000000 fscan-0.3.6/fscan/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      411 2024-04-23 00:59:34.000000 fscan-0.3.6/fscan/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    18999 2024-04-18 22:02:10.000000 fscan-0.3.6/fscan/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4069 2023-10-30 21:32:21.000000 fscan-0.3.6/fscan/clean.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    31861 2024-04-23 00:58:08.000000 fscan-0.3.6/fscan/html.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.933079 fscan-0.3.6/fscan/plot/
+-rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-11-22 00:29:19.000000 fscan-0.3.6/fscan/plot/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    25030 2024-02-17 00:13:02.000000 fscan-0.3.6/fscan/plot/finetoothplot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10296 2024-02-02 19:33:13.000000 fscan-0.3.6/fscan/plot/static.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14562 2024-04-18 22:02:10.000000 fscan-0.3.6/fscan/post.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.939781 fscan-0.3.6/fscan/process/
+-rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-10-30 21:32:21.000000 fscan-0.3.6/fscan/process/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    11838 2023-11-23 17:48:55.000000 fscan-0.3.6/fscan/process/autotag.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9797 2024-04-17 23:36:59.000000 fscan-0.3.6/fscan/process/combfinder.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    16509 2023-10-30 21:32:21.000000 fscan-0.3.6/fscan/process/linecount.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7097 2024-02-03 01:10:22.000000 fscan-0.3.6/fscan/process/linefinder.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    18754 2023-10-30 21:32:21.000000 fscan-0.3.6/fscan/process/lineobjects.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9195 2024-02-15 00:23:30.000000 fscan-0.3.6/fscan/process/spectlinetools.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    27049 2023-12-19 17:13:59.000000 fscan-0.3.6/fscan/status.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.946025 fscan-0.3.6/fscan/utils/
+-rw-r--r--   0 egoetz     (501) staff       (20)      109 2023-10-30 21:32:21.000000 fscan-0.3.6/fscan/utils/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2603 2023-10-30 21:32:21.000000 fscan-0.3.6/fscan/utils/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    35814 2024-02-15 01:09:24.000000 fscan-0.3.6/fscan/utils/dtutils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3819 2024-01-06 01:38:41.000000 fscan-0.3.6/fscan/utils/io.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5753 2024-02-17 00:13:02.000000 fscan-0.3.6/fscan/utils/reuse.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5732 2023-10-30 21:32:21.000000 fscan-0.3.6/fscan/utils/segments.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5559 2024-02-15 01:09:24.000000 fscan-0.3.6/fscan/utils/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2024-04-23 00:59:34.947010 fscan-0.3.6/fscan.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2515 2024-04-23 00:59:34.000000 fscan-0.3.6/fscan.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     1330 2024-04-23 00:59:34.000000 fscan-0.3.6/fscan.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2024-04-23 00:59:34.000000 fscan-0.3.6/fscan.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      352 2024-04-23 00:59:34.000000 fscan-0.3.6/fscan.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       66 2024-04-23 00:59:34.000000 fscan-0.3.6/fscan.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        6 2024-04-23 00:59:34.000000 fscan-0.3.6/fscan.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     1930 2024-01-26 19:41:27.000000 fscan-0.3.6/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2024-04-23 00:59:34.949496 fscan-0.3.6/setup.cfg
```

### Comparing `fscan-0.3.5/CONTRIBUTING.md` & `fscan-0.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/LICENSE` & `fscan-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/PKG-INFO` & `fscan-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fscan
-Version: 0.3.5
+Version: 0.3.6
 Summary: Fscan tool for monitoring narrow spectral artifacts in LIGO data
 Author-email: Evan Goetz <evan.goetz@ligo.org>, Ansel Neunzert <ansel.neunzert@ligo.org>, Sudhagar Suyamprakasam <sudhagar.suyamprakasam@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Source Code, https://git.ligo.org/CW/instrumental/fscan
 Project-URL: Bug Tracker, https://git.ligo.org/CW/instrumental/fscan/-/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `fscan-0.3.5/README.md` & `fscan-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/condor-production/fscan_clean` & `fscan-0.3.6/condor-production/fscan_clean`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/condor-production/fscan_clean.sub` & `fscan-0.3.6/condor-production/fscan_clean.sub`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/condor-production/fscan_daily` & `fscan-0.3.6/condor-production/fscan_daily`

 * *Files 24% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 fi
 
 # Set paths
 DATAFIND_PATH=/home/pulsar/.conda/envs/fscan-py3.10/bin/
 LALSUITE_INSTALL=/home/pulsar/gitrepos/lalsuite/_inst/bin/
 
 # Run FscanDriver
-/home/pulsar/.conda/envs/fscan-py3.10/bin/FscanDriver -C 1 -P 1 -A ligo.prod.o4.detchar.linefind.fscan -U evan.goetz -B 1 --analysisEnd=now --snapToLast=midnight --analysisDuration=1day --averageDuration=1day -y /home/pulsar/gitrepos/fscan/configuration/production/O4_${IFO}_Fscan_ch_info.yml -f /home/pulsar/public_html/fscan/ -s ${LALSUITE_INSTALL} -a ${LALSUITE_INSTALL} -S ${LALSUITE_INSTALL} -d ${DATAFIND_PATH} -I 1 --delete-ascii=1 --run=1
-
+/home/pulsar/.conda/envs/fscan-py3.10/bin/FscanDriver -C 1 -P 1 -A ligo.prod.o4.detchar.linefind.fscan -U evan.goetz -B 1 --analysisEnd=now --snapToLast=midnight --analysisDuration=1day --averageDuration=1day -y /home/pulsar/gitrepos/fscan/configuration/production/O4_${IFO}_Fscan_ch_info.yml -f /home/pulsar/public_html/fscan/ -I 1 --delete-ascii=1 --run=1
```

### Comparing `fscan-0.3.5/condor-production/fscan_daily.sub` & `fscan-0.3.6/condor-production/fscan_daily.sub`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/condor-production/fscan_monthly` & `fscan-0.3.6/condor-production/fscan_weekly`

 * *Files 17% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 fi
 
 # Set paths
 DATAFIND_PATH=/home/pulsar/.conda/envs/fscan-py3.10/bin/
 LALSUITE_INSTALL=/home/pulsar/gitrepos/lalsuite/_inst/bin/
 
 # Run FscanDriver
-/home/pulsar/.conda/envs/fscan-py3.10/bin/FscanDriver -C 1 -P 1 -A ligo.prod.o4.detchar.linefind.fscan -U evan.goetz -B 1 --analysisEnd=now --snapToLast=monthMidnight --analysisDuration=1month --averageDuration=1month --seek-existing-sfts 1 -y /home/pulsar/gitrepos/fscan/configuration/production/O4_${IFO}_Fscan_ch_info.yml -f /home/pulsar/public_html/fscan/ -s ${LALSUITE_INSTALL} -a ${LALSUITE_INSTALL} -S ${LALSUITE_INSTALL} -d ${DATAFIND_PATH} -I 1 --delete-ascii=1 --run=1
-
+/home/pulsar/.conda/envs/fscan-py3.10/bin/FscanDriver -C 1 -P 1 -A ligo.prod.o4.detchar.linefind.fscan -U evan.goetz -B 1 --analysisEnd=now --snapToLast=midnightWednesday --analysisDuration=1week --averageDuration=1week --seek-existing-sfts 1 -y /home/pulsar/gitrepos/fscan/configuration/production/O4_${IFO}_Fscan_ch_info.yml -f /home/pulsar/public_html/fscan/ -I 1 --delete-ascii=1 --run=1
```

### Comparing `fscan-0.3.5/condor-production/fscan_monthly.sub` & `fscan-0.3.6/condor-production/fscan_monthly.sub`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/condor-production/fscan_weekly.sub` & `fscan-0.3.6/condor-production/fscan_weekly.sub`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/condor-production/status_summary_daily` & `fscan-0.3.6/condor-production/status_summary_daily`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/condor-production/status_summary_daily.sub` & `fscan-0.3.6/condor-production/status_summary_daily.sub`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/configuration/examples/example.config` & `fscan-0.3.6/configuration/examples/example.config`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/configuration/examples/example_ch_info.yml` & `fscan-0.3.6/configuration/examples/example_ch_info.yml`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/configuration/production/O4_H1_Fscan_ch_info.yml` & `fscan-0.3.6/configuration/production/O4_H1_Fscan_ch_info.yml`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/configuration/production/O4_L1_Fscan_ch_info.yml` & `fscan-0.3.6/configuration/production/O4_L1_Fscan_ch_info.yml`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/__main__.py` & `fscan-0.3.6/fscan/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #               Ansel Neunzert (2023)
 #
 # This file is part of fscan
 
 import os
 import subprocess
 
-from .batch import MakeSFTJob, NormSFT, CoherenceFromSFT, SummaryJob, write_dag
+from .batch import MakeSFTJob, ProcessSFTs, SummaryJob, write_dag
 from .utils import dtutils as dt
 from .utils.config import CustomConfParser, MultiConfParser
 from .utils.io import read_channel_config
 from .utils.reuse import use_existing_sfts
 from .utils.utils import channels_per_segments, epseg_setup
 from .utils.utils import epoch_info as ep_info
 
@@ -114,23 +114,25 @@
                              'filename (also used if -D option is > 0)')
     parser.add_argument('--run', type='bool', default=False,
                         help='For a trial run do NOT give this option! When '
                              'given this code will run condor_submit_dag! '
                              'Otherwise this script generates the .dag file '
                              'and then stops!')
     parser.add_argument('-s', '--make-sft-dag-path', type=str,
-                        default='/usr/bin',
+                        default='/home/pulsar/gitrepos/lalsuite/_inst/bin',
                         help='Path to the installation of lalpulsar_MakeSFTDAG'
                         )
-    parser.add_argument('-d', '--datafind-path', type=str, default='/usr/bin',
+    parser.add_argument('-d', '--datafind-path', type=str,
+                        default='/cvmfs/software.igwn.org/conda/envs/igwn/bin',
                         help='Path to the installation of gw_data_find')
-    parser.add_argument('-S', '--make-sft-path', type=str, default='/usr/bin',
+    parser.add_argument('-S', '--make-sft-path', type=str,
+                        default='/home/pulsar/gitrepos/lalsuite/_inst/bin',
                         help='Path to the installation of lalpulsar_MakeSFTs')
     parser.add_argument('-a', '--spec-tools-path', type=str,
-                        default='/usr/bin',
+                        default='/home/pulsar/gitrepos/lalsuite/_inst/bin',
                         help='Path to the installation of lalpulsar_spec_avg '
                              'and lalpulsar_spec_avg_long')
     parser.add_argument('-p', '--postproc-path', type=str,
                         default='/home/pulsar/.conda/envs/fscan-py3.10/bin',
                         help='Path to the conda environment for running '
                              'postProcess')
     parser.add_argument('-T', '--Tsft', type=int, default=1800,
@@ -224,29 +226,26 @@
 
                 if epseg_info['havesegs']:
                     # loop over channels
                     for idx, (frametype, chans) in enumerate(channels.items()):
                         for idx2, ch_tup in enumerate(chans):
                             ch = all_ch_info[ch_tup[0]]
 
-                            # normalize SFTs
-                            norm_sft_job = NormSFT(args, epseg_info, ch)
+                            # process SFTs for each channel
+                            processing = ProcessSFTs(args, epseg_info, ch)
+                            processing.write_condor_band_sub()
+                            # full band average (if requested)
                             if args.full_band_avg:
-                                norm_sft_job.write_condor_full_band_sub()
-                            norm_sft_job.write_condor_work_sub()
-
-                            # plot normalized SFTs (if requested)
-                            if args.plot_output:
-                                norm_sft_job.write_condor_plots_sub()
-
+                                processing.write_condor_full_band_sub()
                             # compute and plot coherence (if requested)
                             if 'coherence' in ch:
-                                coh_job = CoherenceFromSFT(
-                                    args, epseg_info, ch)
-                                coh_job.write_condor_work_sub()
+                                processing.write_condor_coherence_sub()
+                            # plot processed SFTs (if requested)
+                            if args.plot_output:
+                                processing.write_condor_plots_sub()
 
                 # prepare summary page job for dag
                 if args.plot_output:
                     summary_job = SummaryJob(args, epseg_info)
                     summary_job.write_condor_work_sub()
 
                 # Write a DAG file that will run everything together:
@@ -269,13 +268,11 @@
                         epseg_info['epoch_path'], 'SUPERDAG.dag')
                     cmd = ['condor_submit_dag',
                            '-maxjobs', f'{args.max_jobs}',
                            '-include_env',
                            ('*DATAFIND*,KRB5*,X509*,BEARER_TOKEN*,SCITOKEN*,'
                             '*SEGMENT*,XDG*'),
                            dagfile]
-                    if (epseg_info['SFTGPSstart'] is not None and
-                            epseg_info['SFTGPSend'] is not None):
-                        print(f"Submitting {dagfile}")
-                        subprocess.run(cmd,
-                                       check=True,
-                                       cwd=os.path.dirname(dagfile))
+                    print(f"Submitting {dagfile}")
+                    subprocess.run(cmd,
+                                   check=True,
+                                   cwd=os.path.dirname(dagfile))
```

### Comparing `fscan-0.3.5/fscan/batch.py` & `fscan-0.3.6/fscan/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -344,24 +344,24 @@
             executable=os.path.join(self.args.make_sft_path,
                                     'lalpulsar_MakeSFTs'),
             acctgroup=self.args.accounting_group,
             acctuser=self.args.accounting_group_user,
             request_disk=self.args.request_disk)
 
 
-class NormSFT(object):
+class ProcessSFTs(object):
 
     def __init__(self, args, epseg_info, ch):
         self.args = args
         self.epseg_info = epseg_info
         self.ch = ch
         self.full_ch_path = os.path.join(self.epseg_info['epoch_path'],
                                          self.ch['channel'].replace(':', '_'))
 
-    def write_condor_work_sub(self):
+    def write_condor_band_sub(self):
 
         """
         Write the submit file for computing the normalized, averaged spectra
         and the spectrograms using lalpulsar_spec_avg
         """
 
         write_sub_file(
@@ -385,51 +385,41 @@
             subname='spectrumAverageLong',
             executable=os.path.join(self.args.spec_tools_path,
                                     'lalpulsar_spec_avg_long'),
             acctgroup=self.args.accounting_group,
             acctuser=self.args.accounting_group_user,
             request_disk=2000)
 
-    def write_condor_plots_sub(self):
+    def write_condor_coherence_sub(self):
         """
-        Write the submit file for computing the normalized, averaged spectra
-        and the spectrograms using postProcess
+        Write the submit file for computing the coherence from SFTs
         """
         write_sub_file(
             full_path=self.full_ch_path,
-            subname='postProcess',
-            executable=os.path.join(self.args.postproc_path,
-                                    'postProcess'),
+            subname='runCoherence',
+            executable=os.path.join(self.args.spec_tools_path,
+                                    'lalpulsar_spec_coherence'),
             acctgroup=self.args.accounting_group,
             acctuser=self.args.accounting_group_user,
-            request_disk=5000,
-            request_memory=5000)
-
-
-class CoherenceFromSFT(object):
-
-    def __init__(self, args, epseg_info, ch):
-        self.args = args
-        self.epseg_info = epseg_info
-        self.ch = ch
-        self.full_ch_path = os.path.join(self.epseg_info['epoch_path'],
-                                         self.ch['channel'].replace(':', '_'))
+            request_disk=500)
 
-    def write_condor_work_sub(self):
+    def write_condor_plots_sub(self):
         """
-        Write the submit file for computing the coherence from SFTs
+        Write the submit file for computing the plots and follow-on analyses
+        using postProcess
         """
         write_sub_file(
             full_path=self.full_ch_path,
-            subname='runCoherence',
-            executable=os.path.join(self.args.spec_tools_path,
-                                    'lalpulsar_spec_coherence'),
+            subname='postProcess',
+            executable=os.path.join(self.args.postproc_path,
+                                    'postProcess'),
             acctgroup=self.args.accounting_group,
             acctuser=self.args.accounting_group_user,
-            request_disk=500)
+            request_disk=5000,
+            request_memory=5000)
 
 
 class SummaryJob(object):
 
     def __init__(self, args, epseg_info):
         self.args = args
         self.epoch_path = epseg_info['epoch_path']
```

### Comparing `fscan-0.3.5/fscan/clean.py` & `fscan-0.3.6/fscan/clean.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/html.py` & `fscan-0.3.6/fscan/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,23 @@
                             args_to_intervals)
 from .utils.io import read_channel_config
 from .plot.static import expected_pngs
 from .utils.utils import channels_per_segments, epseg_setup, epoch_info
 
 
 JS_FILES = [
-    'https://code.jquery.com/jquery-3.5.1.min.js',
-    'https://code.jquery.com/ui/1.12.1/jquery-ui.min.js',
-    'https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.1/moment.min.js',
+    'https://code.jquery.com/jquery-3.7.1.min.js',
+    'https://code.jquery.com/ui/1.13.2/jquery-ui.min.js',
+    'https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.30.1/moment.min.js',
     'https://cdnjs.cloudflare.com/ajax/libs/jquery.lazy/1.7.11/jquery.lazy.min.js',  # noqa
-    'https://cdn.jsdelivr.net/npm/bootstrap@4.5.3/dist/js/bootstrap.bundle.min.js',  # noqa
-    'https://cdnjs.cloudflare.com/ajax/libs/fancybox/3.5.7/jquery.fancybox.min.js',  # noqa
+    'https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js',  # noqa
+    'https://cdn.jsdelivr.net/npm/@fancyapps/ui@5.0/dist/fancybox/fancybox.umd.js',  # noqa
     'https://cdnjs.cloudflare.com/ajax/libs/bootstrap-datepicker/1.9.0/js/bootstrap-datepicker.min.js',  # noqa
-    'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.2/lib/gwbootstrap.min.js',
-    'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.2/lib/gwbootstrap-extra.min.js']  # noqa
+    'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.6/lib/gwbootstrap.min.js',
+    'https://cdn.jsdelivr.net/npm/gwbootstrap@1.3.6/lib/gwbootstrap-extra.min.js']  # noqa
 
 
 def navbar(ifo, metadata, ch_list=[]):
     """
     Create the navigation bar that contains a title, calendar, and links to
     other pages for this particular Fscan run. A calendar is only created for
     day, week, or month modes. Any other mode does not generate a calendar
```

### Comparing `fscan-0.3.5/fscan/plot/finetoothplot.py` & `fscan-0.3.6/fscan/plot/finetoothplot.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/plot/static.py` & `fscan-0.3.6/fscan/plot/static.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/post.py` & `fscan-0.3.6/fscan/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,29 +14,26 @@
 from .process import autotag, linefinder
 from .process.linecount import runForestOfLines
 from .utils import io
 from .utils import dtutils as dtl
 from .utils.utils import str_to_bool
 
 
-def convert_fscan_txt_to_npz(parentPathInput, spects, metadata,
-                             delete_converted_text):
+def convert_fscan_txt_to_npz(parentPathInput, spects, metadata):
     """
     Convert Fscan txt files to npz files
 
     Parameters
     ----------
     parentPathInput : `str`
         Full path to files
     spects : `str`
         glob-style string for txt files to convert to npz
     metadata: dictionary
         output of dtutils.parse_filepath
-    delete_converted_text : bool
-        if True, delete the txt file(s)
 
     Returns
     -------
     error_num : int
         Return 0 if successful, 1 if data is all zeros or nans
 
     Raises
@@ -73,51 +70,55 @@
                 error_num = 1
             else:
                 np.savez(out,
                          f=freq,
                          pwa_tavgwt=pwa_tavgwt,
                          pwa_sumwt=pwa_sumwt,
                          metadata=metadata)
+            del freq, pwa_tavgwt, pwa_sumwt
         elif 'spectrogram' in temp_s:
             out = os.path.join(
                 parentPathInput, ".".join(["_".join(n), "npz"]))
             gpstimes = data[0, 1:]
             vals = data[1:, 1:]
             freq = data[1:, 0]
             if np.all(vals == 0):
                 error_num = 1
             else:
                 np.savez(out,
                          f=freq,
                          vals=vals,
                          gpstimes=gpstimes,
                          metadata=metadata)
+            del gpstimes, vals, freq
         elif 'timeaverage' in temp_s:
             out = os.path.join(
                 parentPathInput, ".".join(["_".join(n), "npz"]))
             freq, normpow = data
             if np.all(normpow == 0):
                 error_num = 1
             else:
                 np.savez(out,
                          f=freq,
                          normpow=normpow,
                          metadata=metadata)
+            del freq, normpow
         elif 'coh' in temp_s:
             out = os.path.join(
                 parentPathInput,
                 "_".join(n).replace("_coh", "_coherence.npz"))
             freq, coh = data
             if np.all(np.isnan(coh)):
                 error_num = 1
             else:
                 np.savez(out,
                          f=freq,
                          coh=coh,
                          metadata=metadata)
+            del freq, coh
         elif 'speclong' in temp_s:
             out = os.path.join(
                 parentPathInput,
                 "".join(["_".join(n), "_speclong.npz"]))
             freq, psd, amppsd, psdwt, amppsdwt, persist = data
             if np.all(psd == 0):
                 error_num = 1
@@ -126,21 +127,47 @@
                          f=freq,
                          psd=psd,
                          amppsd=amppsd,
                          psdwt=psdwt,
                          amppsdwt=amppsdwt,
                          persist=persist,
                          metadata=metadata)
-
-        if delete_converted_text:
-            os.remove(f)
+            del freq, psd, amppsd, psdwt, amppsdwt, persist
 
     return error_num
 
 
+def delete_ascii(parentPathInput, spects):
+    """
+    Delete Fscan txt files
+
+    Parameters
+    ----------
+    parentPathInput : `str`
+        Full path to files
+    spects : `str`
+        glob-style string for txt files to delete
+
+    Raises
+    ------
+    NameError
+        If no files are found with the specified pattern
+    """
+    patt = os.path.join(parentPathInput, spects)
+    files = glob(patt)
+
+    if len(files) == 0:
+        raise NameError(f"No files found with pattern {patt}")
+
+    for f in files:
+        assert f.endswith('txt')
+
+        os.remove(f)
+
+
 def main():
     parser = argparse.ArgumentParser()
     parser.register('type', 'bool', str_to_bool)
     parser.add_argument("--delete-converted-text", type='bool', default=False)
     parser.add_argument("--parentPathInput", type=str)
     parser.add_argument("--plot-sub-band", type=int, default=100,
                         help="Plot frequency bands are rounded to nearest"
@@ -161,28 +188,24 @@
         os.path.expanduser(args.parentPathInput))
 
     # ==============================
     # Save NPZ data for the spectra
     # ==============================
     try:
         errnum1 = convert_fscan_txt_to_npz(
-            args.parentPathInput, "spec_*_timeaverage.txt", metadata,
-            args.delete_converted_text)
+            args.parentPathInput, "spec_*_timeaverage.txt", metadata)
         errnum2 = convert_fscan_txt_to_npz(
-            args.parentPathInput, "spec_*_spectrogram.txt", metadata,
-            args.delete_converted_text)
+            args.parentPathInput, "spec_*_spectrogram.txt", metadata)
         errnum3 = 0
         if len(glob(os.path.join(args.parentPathInput, "spec_*_coh.txt"))) > 0:
             errnum3 = convert_fscan_txt_to_npz(
-                args.parentPathInput, "spec_*_coh.txt", metadata,
-                args.delete_converted_text)
+                args.parentPathInput, "spec_*_coh.txt", metadata)
         # this covers both speclong file outputs
         errnum4 = convert_fscan_txt_to_npz(
-            args.parentPathInput, "speclong_*.txt", metadata,
-            args.delete_converted_text)
+            args.parentPathInput, "speclong_*.txt", metadata)
     except NameError as e:
         # check for nosfts file in the SFTs folder
         if os.path.exists(
                 os.path.join(args.parentPathInput, 'sfts', 'nosfts')):
             print(f'WARNING: {e}. Found a nosfts file. Exiting.')
             return
         else:
@@ -388,9 +411,13 @@
             colorcode='autocolor',
             colorcode_group_min=3
         )
         print(plotArgs.outfile)
 
         finetoothplot.main(plotArgs)
 
+    # Finally, delete the txt files if requested
+    if args.delete_converted_text:
+        delete_ascii(args.parentPathInput, "spec_*.txt")
+
     Path(os.path.join(args.parentPathInput, 'postProcess_success')).touch()
     print("Completed postProcess successfully")
```

### Comparing `fscan-0.3.5/fscan/process/autotag.py` & `fscan-0.3.6/fscan/process/autotag.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/process/combfinder.py` & `fscan-0.3.6/fscan/process/combfinder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is part of fscan
 
 from . import spectlinetools as slt
 import numpy as np
 from .lineobjects import Line, LineList, Spectrum
 
 
-def find_combs(sfreq, sval, lloc, neighbors=50, requirelen=3):
+def find_combs(sfreq, sval, lloc, neighbors=50, requirelen=3, maxlines=5000):
     '''
     Parameters
     ----------
     sfreq: np.ndarray of floats
         Spectral frequencies
 
     sval: np.ndarray of floats
@@ -37,14 +37,16 @@
     Returns
     -------
     combCandidates
         list of LineList objects, each of which should
         have isComb=True and a defined spacing and offset.
     '''
 
+    if len(lloc) > maxlines:
+        return []
     # Sort the lines on their heights
     # (This will help compare lines with their nearest
     # neighbors in height.)
     lheight = sval[lloc]
     inds_that_sort_height = np.argsort(lheight)
     lloc_sorted = lloc[inds_that_sort_height]
```

### Comparing `fscan-0.3.5/fscan/process/linecount.py` & `fscan-0.3.6/fscan/process/linecount.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/process/linefinder.py` & `fscan-0.3.6/fscan/process/linefinder.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/process/lineobjects.py` & `fscan-0.3.6/fscan/process/lineobjects.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/process/spectlinetools.py` & `fscan-0.3.6/fscan/process/spectlinetools.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/status.py` & `fscan-0.3.6/fscan/status.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/utils/config.py` & `fscan-0.3.6/fscan/utils/config.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/utils/dtutils.py` & `fscan-0.3.6/fscan/utils/dtutils.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/utils/io.py` & `fscan-0.3.6/fscan/utils/io.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/utils/reuse.py` & `fscan-0.3.6/fscan/utils/reuse.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/utils/segments.py` & `fscan-0.3.6/fscan/utils/segments.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan/utils/utils.py` & `fscan-0.3.6/fscan/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/fscan.egg-info/PKG-INFO` & `fscan-0.3.6/fscan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fscan
-Version: 0.3.5
+Version: 0.3.6
 Summary: Fscan tool for monitoring narrow spectral artifacts in LIGO data
 Author-email: Evan Goetz <evan.goetz@ligo.org>, Ansel Neunzert <ansel.neunzert@ligo.org>, Sudhagar Suyamprakasam <sudhagar.suyamprakasam@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Source Code, https://git.ligo.org/CW/instrumental/fscan
 Project-URL: Bug Tracker, https://git.ligo.org/CW/instrumental/fscan/-/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `fscan-0.3.5/fscan.egg-info/SOURCES.txt` & `fscan-0.3.6/fscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fscan-0.3.5/pyproject.toml` & `fscan-0.3.6/pyproject.toml`

 * *Files identical despite different names*

