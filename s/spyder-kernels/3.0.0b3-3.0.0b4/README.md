# Comparing `tmp/spyder-kernels-3.0.0b3.tar.gz` & `tmp/spyder-kernels-3.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder-kernels-3.0.0b3.tar", last modified: Mon Dec 18 00:59:21 2023, max compression
+gzip compressed data, was "spyder-kernels-3.0.0b4.tar", last modified: Thu Feb  8 00:58:30 2024, max compression
```

## Comparing `spyder-kernels-3.0.0b3.tar` & `spyder-kernels-3.0.0b4.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.914148 spyder-kernels-3.0.0b3/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      314 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b3/.codecov.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      269 2019-02-03 15:33:04.000000 spyder-kernels-3.0.0b3/.coveragerc
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4930 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/.gitattributes
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.894140 spyder-kernels-3.0.0b3/.github/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       24 2021-04-02 18:19:53.000000 spyder-kernels-3.0.0b3/.github/FUNDING.yml
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.894140 spyder-kernels-3.0.0b3/.github/workflows/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1856 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/.github/workflows/linux-pip-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2071 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/.github/workflows/linux-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1863 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/.github/workflows/macos-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1862 2023-04-15 18:12:27.000000 spyder-kernels-3.0.0b3/.github/workflows/windows-tests.yml
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b3/.gitignore
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      891 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/AUTHORS.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    70429 2023-12-18 00:56:30.000000 spyder-kernels-3.0.0b3/CHANGELOG.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1103 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/LICENSE.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       79 2019-07-11 12:23:54.000000 spyder-kernels-3.0.0b3/MANIFEST.in
--rw-r--r--   0 carlos    (1000) carlos    (1000)     4919 2023-12-18 00:59:21.910147 spyder-kernels-3.0.0b3/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2830 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/README.md
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      727 2021-06-12 22:37:24.000000 spyder-kernels-3.0.0b3/RELEASE.md
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.894140 spyder-kernels-3.0.0b3/requirements/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      120 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/requirements/posix.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/requirements/tests.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       91 2023-10-10 22:15:49.000000 spyder-kernels-3.0.0b3/requirements/windows.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2023-12-18 00:59:21.914148 spyder-kernels-3.0.0b3/setup.cfg
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2951 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/setup.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.894140 spyder-kernels-3.0.0b3/spyder_kernels/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1476 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/spyder_kernels/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      405 2023-12-18 00:57:41.000000 spyder-kernels-3.0.0b3/spyder_kernels/_version.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.894140 spyder-kernels-3.0.0b3/spyder_kernels/comms/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1540 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b3/spyder_kernels/comms/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    17756 2023-12-18 00:17:34.000000 spyder-kernels-3.0.0b3/spyder_kernels/comms/commbase.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      685 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/comms/decorators.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7563 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/comms/frontendcomm.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2327 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/comms/utils.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.898142 spyder-kernels-3.0.0b3/spyder_kernels/console/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      353 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1023 2021-11-22 19:09:05.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/__main__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    36366 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/kernel.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      731 2021-07-28 17:22:20.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/outstream.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    12350 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/shell.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     7206 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/start.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.898142 spyder-kernels-3.0.0b3/spyder_kernels/console/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2018-08-23 02:20:23.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/tests/load_data.npz
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:49:54.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/tests/load_data.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    45828 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/console/tests/test_console_kernel.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.902143 spyder-kernels-3.0.0b3/spyder_kernels/customize/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      511 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    20487 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/code_runner.py
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4195 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/namespace_manager.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     9773 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/spydercustomize.py
--rwxrwxr-x   0 carlos    (1000) carlos    (1000)    32678 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/spyderpdb.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.902143 spyder-kernels-3.0.0b3/spyder_kernels/customize/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-02-03 15:33:04.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2520 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/tests/test_umr.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      820 2023-02-20 16:51:15.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/tests/test_utils.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     3330 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/umr.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4664 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/customize/utils.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.906145 spyder-kernels-3.0.0b3/spyder_kernels/utils/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      348 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    11593 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/dochelpers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    21324 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/iofuncs.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2094 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/lazymodules.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1564 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/misc.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1106 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/mpl.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    24439 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/nsview.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1425 2019-08-05 17:14:47.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/test_utils.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.910147 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      343 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/__init__.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)   138515 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/data.dcm
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      482 2018-06-18 15:46:26.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/data.mat
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/export_data.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/export_data_renamed.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:50:47.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/export_data_withfunction.spydata
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/import_data.npz
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1301 2018-06-18 15:46:26.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/numpy_data.npz
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     4212 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_dochelpers.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    12159 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_iofuncs.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     1257 2021-07-28 13:28:52.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_lazymodules.py
--rw-rw-r--   0 carlos    (1000) carlos    (1000)    13727 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_nsview.py
-drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2023-12-18 00:59:21.894140 spyder-kernels-3.0.0b3/spyder_kernels.egg-info/
--rw-r--r--   0 carlos    (1000) carlos    (1000)     4919 2023-12-18 00:59:21.000000 spyder-kernels-3.0.0b3/spyder_kernels.egg-info/PKG-INFO
--rw-rw-r--   0 carlos    (1000) carlos    (1000)     2356 2023-12-18 00:59:21.000000 spyder-kernels-3.0.0b3/spyder_kernels.egg-info/SOURCES.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2023-12-18 00:59:21.000000 spyder-kernels-3.0.0b3/spyder_kernels.egg-info/dependency_links.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)      396 2023-12-18 00:59:21.000000 spyder-kernels-3.0.0b3/spyder_kernels.egg-info/requires.txt
--rw-rw-r--   0 carlos    (1000) carlos    (1000)       15 2023-12-18 00:59:21.000000 spyder-kernels-3.0.0b3/spyder_kernels.egg-info/top_level.txt
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.172774 spyder-kernels-3.0.0b4/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      314 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b4/.codecov.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      269 2019-02-03 15:33:04.000000 spyder-kernels-3.0.0b4/.coveragerc
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4930 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/.gitattributes
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.152775 spyder-kernels-3.0.0b4/.github/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       24 2021-04-02 18:19:53.000000 spyder-kernels-3.0.0b4/.github/FUNDING.yml
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.152775 spyder-kernels-3.0.0b4/.github/workflows/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1856 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/.github/workflows/linux-pip-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2071 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/.github/workflows/linux-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1863 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/.github/workflows/macos-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1862 2023-04-15 18:12:27.000000 spyder-kernels-3.0.0b4/.github/workflows/windows-tests.yml
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b4/.gitignore
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      891 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/AUTHORS.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    70722 2024-02-08 00:55:59.000000 spyder-kernels-3.0.0b4/CHANGELOG.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1103 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/LICENSE.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       79 2019-07-11 12:23:54.000000 spyder-kernels-3.0.0b4/MANIFEST.in
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     4919 2024-02-08 00:58:30.172774 spyder-kernels-3.0.0b4/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2830 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/README.md
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      727 2021-06-12 22:37:24.000000 spyder-kernels-3.0.0b4/RELEASE.md
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.156775 spyder-kernels-3.0.0b4/requirements/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      120 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/requirements/posix.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      105 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/requirements/tests.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       91 2023-10-10 22:15:49.000000 spyder-kernels-3.0.0b4/requirements/windows.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       38 2024-02-08 00:58:30.172774 spyder-kernels-3.0.0b4/setup.cfg
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2951 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/setup.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.156775 spyder-kernels-3.0.0b4/spyder_kernels/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1476 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/spyder_kernels/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      405 2024-02-08 00:57:22.000000 spyder-kernels-3.0.0b4/spyder_kernels/_version.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.156775 spyder-kernels-3.0.0b4/spyder_kernels/comms/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1540 2019-12-29 23:57:49.000000 spyder-kernels-3.0.0b4/spyder_kernels/comms/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    17756 2023-12-18 00:17:34.000000 spyder-kernels-3.0.0b4/spyder_kernels/comms/commbase.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      685 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/comms/decorators.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7563 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/comms/frontendcomm.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2327 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/comms/utils.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.156775 spyder-kernels-3.0.0b4/spyder_kernels/console/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      353 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1023 2021-11-22 19:09:05.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/__main__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    36718 2024-02-08 00:51:23.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/kernel.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      731 2021-07-28 17:22:20.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/outstream.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12350 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/shell.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     7206 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/start.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.160775 spyder-kernels-3.0.0b4/spyder_kernels/console/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        0 2018-08-23 02:20:23.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/tests/load_data.npz
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:49:54.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/tests/load_data.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    45828 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/console/tests/test_console_kernel.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.160775 spyder-kernels-3.0.0b4/spyder_kernels/customize/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      511 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    20487 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/code_runner.py
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)     4195 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/namespace_manager.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     9773 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/spydercustomize.py
+-rwxrwxr-x   0 carlos    (1000) carlos    (1000)    32678 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/spyderpdb.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.164775 spyder-kernels-3.0.0b4/spyder_kernels/customize/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      363 2019-02-03 15:33:04.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2520 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/tests/test_umr.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      820 2023-02-20 16:51:15.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/tests/test_utils.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     3330 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/umr.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4664 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/customize/utils.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.164775 spyder-kernels-3.0.0b4/spyder_kernels/utils/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      348 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    11593 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/dochelpers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    21324 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/iofuncs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2094 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/lazymodules.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1564 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/misc.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1106 2023-12-18 00:07:17.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/mpl.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    24439 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/nsview.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1425 2019-08-05 17:14:47.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/test_utils.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.168774 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      343 2018-08-07 19:28:05.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/__init__.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)   138515 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/data.dcm
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      482 2018-06-18 15:46:26.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/data.mat
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/export_data.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    20480 2023-02-20 16:51:47.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/export_data_renamed.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    10240 2019-01-26 09:50:47.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/export_data_withfunction.spydata
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      270 2020-02-28 19:57:03.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/import_data.npz
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1301 2018-06-18 15:46:26.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/numpy_data.npz
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     4212 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_dochelpers.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    12159 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_iofuncs.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     1257 2021-07-28 13:28:52.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_lazymodules.py
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)    13727 2023-11-06 17:29:19.000000 spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_nsview.py
+drwxrwxr-x   0 carlos    (1000) carlos    (1000)        0 2024-02-08 00:58:30.168774 spyder-kernels-3.0.0b4/spyder_kernels.egg-info/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     4919 2024-02-08 00:58:30.000000 spyder-kernels-3.0.0b4/spyder_kernels.egg-info/PKG-INFO
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)     2356 2024-02-08 00:58:30.000000 spyder-kernels-3.0.0b4/spyder_kernels.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)        1 2024-02-08 00:58:30.000000 spyder-kernels-3.0.0b4/spyder_kernels.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)      396 2024-02-08 00:58:30.000000 spyder-kernels-3.0.0b4/spyder_kernels.egg-info/requires.txt
+-rw-rw-r--   0 carlos    (1000) carlos    (1000)       15 2024-02-08 00:58:30.000000 spyder-kernels-3.0.0b4/spyder_kernels.egg-info/top_level.txt
```

### Comparing `spyder-kernels-3.0.0b3/.gitattributes` & `spyder-kernels-3.0.0b4/.gitattributes`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/.github/workflows/linux-pip-tests.yml` & `spyder-kernels-3.0.0b4/.github/workflows/linux-pip-tests.yml`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/.github/workflows/linux-tests.yml` & `spyder-kernels-3.0.0b4/.github/workflows/linux-tests.yml`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/.github/workflows/macos-tests.yml` & `spyder-kernels-3.0.0b4/.github/workflows/macos-tests.yml`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/.github/workflows/windows-tests.yml` & `spyder-kernels-3.0.0b4/.github/workflows/windows-tests.yml`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/AUTHORS.txt` & `spyder-kernels-3.0.0b4/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/CHANGELOG.md` & `spyder-kernels-3.0.0b4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # History of changes
 
+## Version 3.0.0b4 (2024-02-08)
+
+### Pull Requests Merged
+
+* [PR 477](https://github.com/spyder-ide/spyder-kernels/pull/477) - PR: Handle new Inline backend options `fontsize` and `bottom`, by [@jitseniesen](https://github.com/jitseniesen)
+
+In this release 1 pull request was closed.
+
+
+----
+
+
 ## Version 3.0.0b3 (2023-12-18)
 
 ### Pull Requests Merged
 
 * [PR 476](https://github.com/spyder-ide/spyder-kernels/pull/476) - PR: Send back pickling error correctly, by [@impact27](https://github.com/impact27)
 * [PR 467](https://github.com/spyder-ide/spyder-kernels/pull/467) - PR: Fix index when skipping hidden frames (Debugger), by [@impact27](https://github.com/impact27)
 * [PR 466](https://github.com/spyder-ide/spyder-kernels/pull/466) - PR: Simplify kernel configuration, by [@impact27](https://github.com/impact27)
```

### Comparing `spyder-kernels-3.0.0b3/LICENSE.txt` & `spyder-kernels-3.0.0b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/PKG-INFO` & `spyder-kernels-3.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyder-kernels
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Jupyter kernels for Spyder's console
 Home-page: https://github.com/spyder-ide/spyder-kernels
 Download-URL: https://www.spyder-ide.org/#fh5co-download
 Author: Spyder Development Team
 Author-email: spyderlib@googlegroups.com
 License: MIT
 Keywords: spyder jupyter kernel ipython console
```

### Comparing `spyder-kernels-3.0.0b3/README.md` & `spyder-kernels-3.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/RELEASE.md` & `spyder-kernels-3.0.0b4/RELEASE.md`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/setup.py` & `spyder-kernels-3.0.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/__init__.py` & `spyder-kernels-3.0.0b4/spyder_kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/comms/__init__.py` & `spyder-kernels-3.0.0b4/spyder_kernels/comms/__init__.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/comms/commbase.py` & `spyder-kernels-3.0.0b4/spyder_kernels/comms/commbase.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/comms/decorators.py` & `spyder-kernels-3.0.0b4/spyder_kernels/comms/decorators.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/comms/frontendcomm.py` & `spyder-kernels-3.0.0b4/spyder_kernels/comms/frontendcomm.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/comms/utils.py` & `spyder-kernels-3.0.0b4/spyder_kernels/comms/utils.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/console/__main__.py` & `spyder-kernels-3.0.0b4/spyder_kernels/console/__main__.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/console/kernel.py` & `spyder-kernels-3.0.0b4/spyder_kernels/console/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -553,14 +553,16 @@
         """Set matplotlib configuration"""
         pylab_autoload_n = 'pylab/autoload'
         pylab_backend_n = 'pylab/backend'
         figure_format_n = 'pylab/inline/figure_format'
         resolution_n = 'pylab/inline/resolution'
         width_n = 'pylab/inline/width'
         height_n = 'pylab/inline/height'
+        fontsize_n = 'pylab/inline/fontsize'
+        bottom_n = 'pylab/inline/bottom'
         bbox_inches_n = 'pylab/inline/bbox_inches'
         inline_backend = 'inline'
 
         if pylab_autoload_n in conf or pylab_backend_n in conf:
             self._set_mpl_backend(
                 conf.get(pylab_backend_n, inline_backend),
                 pylab=conf.get(pylab_autoload_n, False)
@@ -577,14 +579,23 @@
 
         if width_n in conf and height_n in conf:
             self._set_mpl_inline_rc_config(
                 'figure.figsize',
                 (conf[width_n], conf[height_n])
             )
 
+        if fontsize_n in conf:
+            self._set_mpl_inline_rc_config('font.size', conf[fontsize_n])
+
+        if bottom_n in conf:
+            self._set_mpl_inline_rc_config(
+                'figure.subplot.bottom',
+                conf[bottom_n]
+            )
+
         if bbox_inches_n in conf:
             self.set_mpl_inline_bbox_inches(conf[bbox_inches_n])
 
 
     def set_mpl_inline_bbox_inches(self, bbox_inches):
         """
         Set inline print figure bbox inches.
```

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/console/outstream.py` & `spyder-kernels-3.0.0b4/spyder_kernels/console/outstream.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/console/shell.py` & `spyder-kernels-3.0.0b4/spyder_kernels/console/shell.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/console/start.py` & `spyder-kernels-3.0.0b4/spyder_kernels/console/start.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/console/tests/load_data.spydata` & `spyder-kernels-3.0.0b4/spyder_kernels/console/tests/load_data.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/console/tests/test_console_kernel.py` & `spyder-kernels-3.0.0b4/spyder_kernels/console/tests/test_console_kernel.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/code_runner.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/code_runner.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/namespace_manager.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/namespace_manager.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/spydercustomize.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/spydercustomize.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/spyderpdb.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/spyderpdb.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/tests/test_umr.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/tests/test_umr.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/tests/test_utils.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/umr.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/umr.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/customize/utils.py` & `spyder-kernels-3.0.0b4/spyder_kernels/customize/utils.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/dochelpers.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/dochelpers.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/iofuncs.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/iofuncs.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/lazymodules.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/lazymodules.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/misc.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/mpl.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/mpl.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/nsview.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/nsview.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/test_utils.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/data.dcm` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/data.dcm`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/export_data.spydata` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/export_data.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/export_data_renamed.spydata` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/export_data_renamed.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/export_data_withfunction.spydata` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/export_data_withfunction.spydata`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/numpy_data.npz` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/numpy_data.npz`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_dochelpers.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_dochelpers.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_iofuncs.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_iofuncs.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_lazymodules.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_lazymodules.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels/utils/tests/test_nsview.py` & `spyder-kernels-3.0.0b4/spyder_kernels/utils/tests/test_nsview.py`

 * *Files identical despite different names*

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels.egg-info/PKG-INFO` & `spyder-kernels-3.0.0b4/spyder_kernels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyder-kernels
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: Jupyter kernels for Spyder's console
 Home-page: https://github.com/spyder-ide/spyder-kernels
 Download-URL: https://www.spyder-ide.org/#fh5co-download
 Author: Spyder Development Team
 Author-email: spyderlib@googlegroups.com
 License: MIT
 Keywords: spyder jupyter kernel ipython console
```

### Comparing `spyder-kernels-3.0.0b3/spyder_kernels.egg-info/SOURCES.txt` & `spyder-kernels-3.0.0b4/spyder_kernels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

