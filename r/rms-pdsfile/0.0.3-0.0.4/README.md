# Comparing `tmp/rms_pdsfile-0.0.3.tar.gz` & `tmp/rms_pdsfile-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms_pdsfile-0.0.3.tar", last modified: Mon Apr 15 21:40:13 2024, max compression
+gzip compressed data, was "rms_pdsfile-0.0.4.tar", last modified: Tue Apr 23 00:01:53 2024, max compression
```

## Comparing `rms_pdsfile-0.0.3.tar` & `rms_pdsfile-0.0.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.479827 rms_pdsfile-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.483827 rms_pdsfile-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/run-tests-and-opus.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.483827 rms_pdsfile-0.0.3/pdsfile/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/pdsfile/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.483827 rms_pdsfile-0.0.3/pdsfile/pds3file/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.487827 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/ASTROM_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COCIRS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/CORSS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/EBROCC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/GO_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/HSTxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJIR_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJNC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHxxxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RES_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RPX_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGIRIS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_20xx.py
--rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_28xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/rules/pytest_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
--rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_whitebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds4file/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/
--rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23585 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_iss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24720 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_vims.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/pytest_support.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57915 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased.py
--rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    33847 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pds4file/tests/test_pds4file_blackbox.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pdscache.py
--rw-r--r--   0 runner    (1001) docker     (127)   230951 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pdsfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/pdsviewable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pdsfile/preload_and_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 21:40:13.000000 rms_pdsfile-0.0.3/rms_pdsfile.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/run_tests_coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.479827 rms_pdsfile-0.0.3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.491827 rms_pdsfile-0.0.3/scripts/automated_tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/scripts/automated_tests/pdsfile_main_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:40:13.495827 rms_pdsfile-0.0.3/validation/
--rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsarchives.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdschecksums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsdata-sync.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsdependency.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsindexshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdsinfoshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/pdslinkshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/re-validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-15 21:40:08.000000 rms_pdsfile-0.0.3/validation/shelf-consistency-check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.629398 rms_pdsfile-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.633398 rms_pdsfile-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/run-tests-and-opus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.633398 rms_pdsfile-0.0.4/pdsfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/pdsfile/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.633398 rms_pdsfile-0.0.4/pdsfile/pds3file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/ASTROM_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COCIRS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/CORSS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/EBROCC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/GO_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/HSTxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJIR_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJNC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHxxxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RES_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RPX_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGIRIS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_20xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_28xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/pytest_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_whitebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds4file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23705 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_iss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24866 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_vims.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/pytest_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65261 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38424 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/test_pds4file_blackbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pdscache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230951 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pdsfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pdsviewable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/preload_and_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/run_tests_coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.629398 rms_pdsfile-0.0.4/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/scripts/automated_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/scripts/automated_tests/pdsfile_main_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/validation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsarchives.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdschecksums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsdata-sync.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsdependency.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsindexshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsinfoshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdslinkshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/re-validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/shelf-consistency-check.py
```

### Comparing `rms_pdsfile-0.0.3/.github/workflows/publish_to_pypi.yml` & `rms_pdsfile-0.0.4/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/.github/workflows/publish_to_test_pypi.yml` & `rms_pdsfile-0.0.4/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/.github/workflows/run-tests-and-opus.yml` & `rms_pdsfile-0.0.4/.github/workflows/run-tests-and-opus.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/.github/workflows/run-tests.yml` & `rms_pdsfile-0.0.4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/.gitignore` & `rms_pdsfile-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/CODE_OF_CONDUCT.md` & `rms_pdsfile-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/CONTRIBUTING.md` & `rms_pdsfile-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/LICENSE` & `rms_pdsfile-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/PKG-INFO` & `rms_pdsfile-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.3
+Version: 0.0.4
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms_pdsfile-0.0.3/README.md` & `rms_pdsfile-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/conftest.py` & `rms_pdsfile-0.0.4/conftest.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/__init__.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/ASTROM_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/ASTROM_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COCIRS_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COCIRS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COISS_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/CORSS_8xxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/CORSS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COSP_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_0xxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COUVIS_8xxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_0xxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/COVIMS_8xxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/EBROCC_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/EBROCC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/GO_0xxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/GO_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/HSTxx_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/HSTxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJIR_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJIR_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOJNC_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJNC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/JNOSP_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHSP_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/NHxxxx_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHxxxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RES_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RES_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/RPX_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RPX_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGIRIS_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGIRIS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VGISS_xxxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_0xxx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_20xx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_20xx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/VG_28xx.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_28xx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/__init__.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/rules/pytest_support.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/helper.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pds3file_whitebox.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_whitebox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py` & `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/__init__.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/__init__.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_iss.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_iss.py`

 * *Files 3% similar despite different names*

```diff
@@ -330,69 +330,69 @@
 ##########################################################################################
 # Unit tests
 ##########################################################################################
 
 import pytest
 from .pytest_support import *
 
-@pytest.mark.parametrize(
-    'input_path,category,expected',
-    [
-        ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
-         'bundles',
-         [
-            'bundles/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
-            'bundles/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
-            'bundles/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.png',
-            'bundles/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'
-         ]),
-        ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
-         'previews',
-         [
-            'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_full.png',
-            'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_med.png',
-            'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_small.png',
-            'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_thumb.png'
-         ]),
-        ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
-         'calibrated',
-         [
-            'calibrated/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_CALIB.IMG',
-            'calibrated/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_CALIB.LBL'
-         ]),
-        ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
-         'documents',
-         [
-            'documents/cassini_iss/Calibration-Plan.pdf',
-            'documents/cassini_iss/Data-Product-SIS.txt',
-            'documents/cassini_iss/ISS-Users-Guide.docx',
-            'documents/cassini_iss/Data-Product-SIS.pdf',
-            'documents/cassini_iss/Calibration-Theoretical-Basis.pdf',
-            'documents/cassini_iss/VICAR-File-Format.pdf',
-            'documents/cassini_iss/Calibration-Report.link',
-            'documents/cassini_iss/Press-Releases-at-RMS.link',
-            'documents/cassini_iss/VICAR-Home-Page-at-JPL.link',
-            'documents/cassini_iss/Press-Releases-at-JPL-Photojournal.link',
-            'documents/cassini_iss/Porco-etal-2004-SSR.link',
-            'documents/cassini_iss/ISS-Users-Guide.pdf',
-            'documents/cassini_iss/Archive-SIS.pdf',
-            'documents/cassini_iss/PDS-ISS-Home-Page.link',
-            'documents/cassini_iss/CISSCAL-Users-Guide.pdf',
-            'documents/cassini_iss/PDS-ISS-Home-Page-at-RMS.link',
-            'documents/cassini_iss/Archive-SIS.txt',
-            'documents/cassini_iss/Cassini-ISS-Final-Report.pdf',
-            'documents/cassini_iss/Calibration-Report.zip'
-         ]),
-        # TODO: add test case for metadata when correct index files & _indexshelf-metadata
-        # are added
-    ]
-)
-def test_associated_abspaths(input_path, category, expected):
-    target_pdsfile = instantiate_target_pdsfile(input_path)
-    res = target_pdsfile.associated_abspaths(category=category)
-    result_paths = []
-    result_paths += pds4file.Pds4File.logicals_for_abspaths(res)
-    assert len(result_paths) != 0
-    for path in result_paths:
-        assert path in expected
+# @pytest.mark.parametrize(
+#     'input_path,category,expected',
+#     [
+#         ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+#          'bundles',
+#          [
+#             'bundles/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+#             'bundles/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+#             'bundles/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.png',
+#             'bundles/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'
+#          ]),
+#         ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+#          'previews',
+#          [
+#             'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_full.png',
+#             'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_med.png',
+#             'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_small.png',
+#             'previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_thumb.png'
+#          ]),
+#         ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+#          'calibrated',
+#          [
+#             'calibrated/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_CALIB.IMG',
+#             'calibrated/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_CALIB.LBL'
+#          ]),
+#         ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+#          'documents',
+#          [
+#             'documents/cassini_iss/Calibration-Plan.pdf',
+#             'documents/cassini_iss/Data-Product-SIS.txt',
+#             'documents/cassini_iss/ISS-Users-Guide.docx',
+#             'documents/cassini_iss/Data-Product-SIS.pdf',
+#             'documents/cassini_iss/Calibration-Theoretical-Basis.pdf',
+#             'documents/cassini_iss/VICAR-File-Format.pdf',
+#             'documents/cassini_iss/Calibration-Report.link',
+#             'documents/cassini_iss/Press-Releases-at-RMS.link',
+#             'documents/cassini_iss/VICAR-Home-Page-at-JPL.link',
+#             'documents/cassini_iss/Press-Releases-at-JPL-Photojournal.link',
+#             'documents/cassini_iss/Porco-etal-2004-SSR.link',
+#             'documents/cassini_iss/ISS-Users-Guide.pdf',
+#             'documents/cassini_iss/Archive-SIS.pdf',
+#             'documents/cassini_iss/PDS-ISS-Home-Page.link',
+#             'documents/cassini_iss/CISSCAL-Users-Guide.pdf',
+#             'documents/cassini_iss/PDS-ISS-Home-Page-at-RMS.link',
+#             'documents/cassini_iss/Archive-SIS.txt',
+#             'documents/cassini_iss/Cassini-ISS-Final-Report.pdf',
+#             'documents/cassini_iss/Calibration-Report.zip'
+#          ]),
+#         # TODO: add test case for metadata when correct index files & _indexshelf-metadata
+#         # are added
+#     ]
+# )
+# def test_associated_abspaths(input_path, category, expected):
+#     target_pdsfile = instantiate_target_pdsfile(input_path)
+#     res = target_pdsfile.associated_abspaths(category=category)
+#     result_paths = []
+#     result_paths += pds4file.Pds4File.logicals_for_abspaths(res)
+#     assert len(result_paths) != 0
+#     for path in result_paths:
+#         assert path in expected
 
 ##########################################################################################
```

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/cassini_vims.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_vims.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,82 +325,82 @@
 ##########################################################################################
 # Unit tests
 ##########################################################################################
 
 import pytest
 from .pytest_support import *
 
-@pytest.mark.parametrize(
-    'input_path,category,expected',
-    [
-        ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
-         'bundles',
-         [
-            'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.qub',
-            'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
-            'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947223-full.png',
-            'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947223-full.xml'
-         ]),
-        ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
-         'bundles',
-         [
-            'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
-            'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.xml',
-            'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003-full.png',
-            'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003-full.xml'
-         ]),
-        ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
-         'previews',
-         [
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_full.png',
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_med.png',
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_small.png',
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_thumb.png'
-         ]),
-        ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
-         'previews',
-         [
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_full.png',
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_med.png',
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_small.png',
-            'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_thumb.png'
-         ]),
-        ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
-         'documents',
-         [
-            'documents/cassini_vims/Brown-etal-2004-SSR.link',
-            'documents/cassini_vims/PDS-VIMS-Home-Page.link',
-            'documents/cassini_vims/Data-Product-SIS.txt',
-            'documents/cassini_vims/VIMS-Preview-Interpretation-Guide.pdf',
-            'documents/cassini_vims/PDS-VIMS-Home-Page-at-RMS.link',
-            'documents/cassini_vims/ISIS-Home-Page-at-USGS.link',
-            'documents/cassini_vims/ISIS-2-User-Documentation.link',
-            'documents/cassini_vims/Cassini-VIMS-Final-Report.pdf',
-            'documents/cassini_vims/Archive-SIS.txt'
-         ]),
-        ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
-         'documents',
-         [
-            'documents/cassini_vims/Brown-etal-2004-SSR.link',
-            'documents/cassini_vims/PDS-VIMS-Home-Page.link',
-            'documents/cassini_vims/Data-Product-SIS.txt',
-            'documents/cassini_vims/VIMS-Preview-Interpretation-Guide.pdf',
-            'documents/cassini_vims/PDS-VIMS-Home-Page-at-RMS.link',
-            'documents/cassini_vims/ISIS-Home-Page-at-USGS.link',
-            'documents/cassini_vims/ISIS-2-User-Documentation.link',
-            'documents/cassini_vims/Cassini-VIMS-Final-Report.pdf',
-            'documents/cassini_vims/Archive-SIS.txt'
-         ]),
-        # TODO: add test case for metadata when correct index files & _indexshelf-metadata
-        # are added
-    ]
-)
-def test_associated_abspaths(input_path, category, expected):
-    target_pdsfile = instantiate_target_pdsfile(input_path)
-    res = target_pdsfile.associated_abspaths(category=category)
-    result_paths = []
-    result_paths += pds4file.Pds4File.logicals_for_abspaths(res)
-    assert len(result_paths) != 0
-    for path in result_paths:
-        assert path in expected
+# @pytest.mark.parametrize(
+#     'input_path,category,expected',
+#     [
+#         ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
+#          'bundles',
+#          [
+#             'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.qub',
+#             'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
+#             'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947223-full.png',
+#             'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947223-full.xml'
+#          ]),
+#         ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
+#          'bundles',
+#          [
+#             'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
+#             'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.xml',
+#             'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003-full.png',
+#             'bundles/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003-full.xml'
+#          ]),
+#         ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
+#          'previews',
+#          [
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_full.png',
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_med.png',
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_small.png',
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_thumb.png'
+#          ]),
+#         ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
+#          'previews',
+#          [
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_full.png',
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_med.png',
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_small.png',
+#             'previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_thumb.png'
+#          ]),
+#         ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
+#          'documents',
+#          [
+#             'documents/cassini_vims/Brown-etal-2004-SSR.link',
+#             'documents/cassini_vims/PDS-VIMS-Home-Page.link',
+#             'documents/cassini_vims/Data-Product-SIS.txt',
+#             'documents/cassini_vims/VIMS-Preview-Interpretation-Guide.pdf',
+#             'documents/cassini_vims/PDS-VIMS-Home-Page-at-RMS.link',
+#             'documents/cassini_vims/ISIS-Home-Page-at-USGS.link',
+#             'documents/cassini_vims/ISIS-2-User-Documentation.link',
+#             'documents/cassini_vims/Cassini-VIMS-Final-Report.pdf',
+#             'documents/cassini_vims/Archive-SIS.txt'
+#          ]),
+#         ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
+#          'documents',
+#          [
+#             'documents/cassini_vims/Brown-etal-2004-SSR.link',
+#             'documents/cassini_vims/PDS-VIMS-Home-Page.link',
+#             'documents/cassini_vims/Data-Product-SIS.txt',
+#             'documents/cassini_vims/VIMS-Preview-Interpretation-Guide.pdf',
+#             'documents/cassini_vims/PDS-VIMS-Home-Page-at-RMS.link',
+#             'documents/cassini_vims/ISIS-Home-Page-at-USGS.link',
+#             'documents/cassini_vims/ISIS-2-User-Documentation.link',
+#             'documents/cassini_vims/Cassini-VIMS-Final-Report.pdf',
+#             'documents/cassini_vims/Archive-SIS.txt'
+#          ]),
+#         # TODO: add test case for metadata when correct index files & _indexshelf-metadata
+#         # are added
+#     ]
+# )
+# def test_associated_abspaths(input_path, category, expected):
+#     target_pdsfile = instantiate_target_pdsfile(input_path)
+#     res = target_pdsfile.associated_abspaths(category=category)
+#     result_paths = []
+#     result_paths += pds4file.Pds4File.logicals_for_abspaths(res)
+#     assert len(result_paths) != 0
+#     for path in result_paths:
+#         assert path in expected
 
 ##########################################################################################
```

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/pytest_support.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,20 +38,26 @@
 ])
 
 ##########################################################################################
 # VIEWABLES
 ##########################################################################################
 
 default_viewables = translator.TranslatorByRegex([
-    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data(.*|_[a-z]*])/.*)\.[a-z]{3}', 0,
-        [r'previews/\1_full.png',
-         r'previews/\1_med.png',
-         r'previews/\1_small.png',
-         r'previews/\1_thumb.png',
-        ])
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/atmosphere/.*-v-.*)\.[a-z]{3}', 0,
+        [r'previews/\1_preview_full.png',
+         r'previews/\1_preview_med.png',
+         r'previews/\1_preview_small.png',
+         r'previews/\1_preview_thumb.png',
+    ]),
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/(rings|global))/(.*)_\d+m\.[a-z]{3}', 0,
+        [r'previews/\1/\3_preview_full.png',
+         r'previews/\1/\3_preview_med.png',
+         r'previews/\1/\3_preview_small.png',
+         r'previews/\1/\3_preview_thumb.png',
+    ]),
 ])
 
 ##########################################################################################
 # ASSOCIATIONS
 ##########################################################################################
 
 associations_to_bundles = translator.TranslatorByRegex([
@@ -64,20 +70,42 @@
          r'bundles/\1/browse\3.xml',
         ]),
     (r'documents/uranus_occs_earthbased.*', 0,
         r'bundles/uranus_occs_earthbased'),
 ])
 
 associations_to_previews = translator.TranslatorByRegex([
-    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/(data|browse)(.*|_[a-z]*])/.*)\.[a-z]{3}', 0,
-        [r'previews/\1_full.png',
-         r'previews/\1_med.png',
-         r'previews/\1_small.png',
-         r'previews/\1_thumb.png',
-        ])
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/(data|browse)/atmosphere/.*-v-.*)\.[a-z]{3}', 0,
+        [r'previews/\1_preview_full.png',
+         r'previews/\1_preview_med.png',
+         r'previews/\1_preview_small.png',
+         r'previews/\1_preview_thumb.png',
+    ]),
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/(data|browse)/(rings|global))/(.*)_\d+m\.[a-z]{3}', 0,
+        [r'previews/\1/\4_preview_full.png',
+         r'previews/\1/\4_preview_med.png',
+         r'previews/\1/\4_preview_small.png',
+         r'previews/\1/\4_preview_thumb.png',
+    ]),
+
+])
+
+associations_to_diagrams = translator.TranslatorByRegex([
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/(data|browse)/atmosphere/.*-v-.*)\.[a-z]{3}', 0,
+        [r'diagrams/\1_diagram_full.png',
+         r'diagrams/\1_diagram_med.png',
+         r'diagrams/\1_diagram_small.png',
+         r'diagrams/\1_diagram_thumb.png',
+    ]),
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/(data|browse)/(rings|global))/(.*)_\d+m\.[a-z]{3}', 0,
+        [r'diagrams/\1/\4_diagram_full.png',
+         r'diagrams/\1/\4_diagram_med.png',
+         r'diagrams/\1/\4_diagram_small.png',
+         r'diagrams/\1/\4_diagram_thumb.png',
+    ]),
 ])
 
 associations_to_metadata = translator.TranslatorByRegex([
     (r'.*/(uranus_occs_earthbased)/*', 0,
         r'metadata/\1'),
     (r'.*/(uranus_occs_earthbased/uranus_occ_u[a-z0-9\_]*)/*', 0,
         r'metadata/\1'),
@@ -165,15 +193,14 @@
     (r'.*uranus_occ_support/document/user_guide/.*\.(pro|py)',                                 0, ('Uranus Earth-based Occultations', 160, 'ebur_occ_software', 'Software', False)),
     (r'.*uranus_occ_support/document/user_guide/plot.*\.pdf',                                  0, ('Uranus Earth-based Occultations', 160, 'ebur_occ_software', 'Software', False)),
     (r'.*uranus_occ_support/spice_kernels/fk/.*\.(tf|xml)',                                    0, ('Uranus Earth-based Occultations', 170, 'ebur_occ_kernels', 'SPICE Kernels', False)),
     (r'.*uranus_occ_support/spice_kernels/spk/.*\.(bsp|xml)',                                  0, ('Uranus Earth-based Occultations', 170, 'ebur_occ_kernels', 'SPICE Kernels', False)),
 
     # rms_index
     (r'metadata/uranus_occs.*/.*/.*_index.csv',                                                0, ('metadata', 5, 'rms_index', 'RMS Node Augmented Index',     False)),
-    # TODO: Add preview and diagram images when they are available
 ])
 
 ##########################################################################################
 # OPUS_FORMAT
 ##########################################################################################
 
 opus_format = translator.TranslatorByRegex([
@@ -200,15 +227,16 @@
          r'bundles/\1/data/ring_models/\2*_fitted_*.tab',
          r'bundles/\1/data/ring_models/\2*_fitted_*.xml',
          r'bundles/\1/data/ring_models/\2*_predicted_*.pdf',
          r'bundles/\1/data/ring_models/\2*_predicted_*.tab',
          r'bundles/\1/data/ring_models/\2*_predicted_*.xml',
          r'bundles/\1/data/ring_models/\2*_wavelengths.csv',
          r'bundles/\1/data/ring_models/\2*_wavelengths.xml',
-         r'metadata/\1/uranus_occ_\2_rings_index.csv']
+         r'metadata/\1/uranus_occ_\2_rings_index.csv',
+         ]
     ),
     # Atmosphere-specific products
     (r'.*/(uranus_occs_earthbased/uranus_occ_([a-zA-Z0-9\_]+))/(data/atmosphere)/.*_counts-v-time_atmos_(egress|ingress)\.[a-z]{3}', 0,
         [r'bundles/\1/\3/\2*_counts-v-time_atmos_\4.tab',
          r'bundles/\1/\3/\2*_counts-v-time_atmos_\4.xml',
          r'metadata/\1/uranus_occ_\2_atmos*_index.csv']
     ),
@@ -240,15 +268,39 @@
          r'bundles/\1/uranus_occ_support/document/user_guide/*.py',
          r'bundles/\1/uranus_occ_support/document/user_guide/plot*.pdf',
          r'bundles/\1/uranus_occ_support/spice_kernels/fk/*.tf',
          r'bundles/\1/uranus_occ_support/spice_kernels/fk/*.xml',
          r'bundles/\1/uranus_occ_support/spice_kernels/spk/*.bsp',
          r'bundles/\1/uranus_occ_support/spice_kernels/spk/*.xml']
     ),
-    # TODO: Add preview and diagram images when they are available
+    # Previews and diagrams
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/atmosphere/.*-v-.*)\.[a-z]{3}', 0,
+        [r'previews/\1_preview_full.png',
+         r'previews/\1_preview_med.png',
+         r'previews/\1_preview_small.png',
+         r'previews/\1_preview_thumb.png']
+    ),
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/(rings|global))/(.*)_\d+m\.[a-z]{3}', 0,
+        [r'previews/\1/\3_preview_full.png',
+         r'previews/\1/\3_preview_med.png',
+         r'previews/\1/\3_preview_small.png',
+         r'previews/\1/\3_preview_thumb.png']
+    ),
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/atmosphere/.*-v-.*)\.[a-z]{3}', 0,
+        [r'diagrams/\1_diagram_full.png',
+         r'diagrams/\1_diagram_med.png',
+         r'diagrams/\1_diagram_small.png',
+         r'diagrams/\1_diagram_thumb.png']
+    ),
+    (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/(rings|global))/(.*)_\d+m\.[a-z]{3}', 0,
+        [r'diagrams/\1/\3_diagram_full.png',
+         r'diagrams/\1/\3_diagram_med.png',
+         r'diagrams/\1/\3_diagram_small.png',
+         r'diagrams/\1/\3_diagram_thumb.png']
+    ),
 ])
 
 ##########################################################################################
 # OPUS_ID
 ##########################################################################################
 # OPUS ID Abbrev is based on the telescope name from the collection_context.csv
 # Detector:
@@ -400,14 +452,15 @@
     OPUS_ID_TO_PRIMARY_LOGICAL_PATH = opus_id_to_primary_logical_path
 
     VIEWABLES = {'default': default_viewables}
 
     ASSOCIATIONS = pds4file.Pds4File.ASSOCIATIONS.copy()
     ASSOCIATIONS['bundles']    += associations_to_bundles
     ASSOCIATIONS['previews']   += associations_to_previews
+    ASSOCIATIONS['diagrams'] += associations_to_diagrams
     ASSOCIATIONS['metadata']   += associations_to_metadata
     ASSOCIATIONS['documents']  += associations_to_documents
 
     pds4file.Pds4File.FILESPEC_TO_BUNDLESET = filespec_to_bundleset + \
                                               pds4file.Pds4File.FILESPEC_TO_BUNDLESET
 # Global attribute shared by all subclasses
 opus_id_to_subclass_set = set()
@@ -562,14 +615,42 @@
            False): [
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/spk/urkao_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/spk/urkao_v1.bsp',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_rfrench20201201_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_rfrench20201201_v1.tf',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_french_et_al_1988_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_french_et_al_1988_v1.tf'
+            ],
+          ('diagram',
+           40,
+           'diagram_full',
+           'Browse Diagram (full)',
+           True): [
+                'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_full.png'
+            ],
+          ('diagram',
+           30,
+           'diagram_medium',
+           'Browse Diagram (medium)',
+           False): [
+                'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_med.png'
+            ],
+          ('diagram',
+           20,
+           'diagram_small',
+           'Browse Diagram (small)',
+           False): [
+                'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_small.png'
+            ],
+          ('diagram',
+           10,
+           'diagram_thumb',
+           'Browse Diagram (thumbnail)',
+           False): [
+                'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_thumb.png'
             ]}
         ),
         # atmosphere
         ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress.xml',
          {('Uranus Earth-based Occultations',
            60,
            'ebur_occ_atmos',
@@ -635,14 +716,42 @@
            False): [
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/spk/urkao_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/spk/urkao_v1.bsp',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_rfrench20201201_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_rfrench20201201_v1.tf',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_french_et_al_1988_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_french_et_al_1988_v1.tf'
+            ],
+          ('diagram',
+           40,
+           'diagram_full',
+           'Browse Diagram (full)',
+           True): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress_diagram_full.png'
+            ],
+          ('diagram',
+           30,
+           'diagram_medium',
+           'Browse Diagram (medium)',
+           False): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress_diagram_med.png'
+            ],
+          ('diagram',
+           20,
+           'diagram_small',
+           'Browse Diagram (small)',
+           False): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress_diagram_small.png'
+            ],
+          ('diagram',
+           10,
+           'diagram_thumb',
+           'Browse Diagram (thumbnail)',
+           False): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress_diagram_thumb.png'
             ]}
         ),
         # global
         ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_100m.xml',
          {('Uranus Earth-based Occultations',
            70,
            'ebur_occ_global_0100',
@@ -744,15 +853,43 @@
            'SPICE Kernels',
            False): [
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/spk/urkao_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/spk/urkao_v1.bsp',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_rfrench20201201_v1.xml',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_rfrench20201201_v1.tf',
                 'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_french_et_al_1988_v1.xml',
-                'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_french_et_al_1988_v1.tf']}
+                'bundles/uranus_occs_earthbased/uranus_occ_support/spice_kernels/fk/uranus_ringframes_french_et_al_1988_v1.tf'],
+          ('diagram',
+           40,
+           'diagram_full',
+           'Browse Diagram (full)',
+           True): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_full.png'
+            ],
+          ('diagram',
+           30,
+           'diagram_medium',
+           'Browse Diagram (medium)',
+           False): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_med.png'
+            ],
+          ('diagram',
+           20,
+           'diagram_small',
+           'Browse Diagram (small)',
+           False): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_small.png'
+            ],
+          ('diagram',
+           10,
+           'diagram_thumb',
+           'Browse Diagram (thumbnail)',
+           False): [
+               'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_thumb.png'
+            ]}
         )
     ]
 )
 def test_opus_products(input_path, expected):
     opus_products_test(input_path, expected)
 
 @pytest.mark.parametrize(
@@ -762,29 +899,45 @@
          'bundles',
          [
             'bundles/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.tab',
             'bundles/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
             'bundles/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/browse/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.pdf',
             'bundles/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/browse/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml'
          ]),
+        # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
+        #  'previews',
+        #  [
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_full.png',
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_med.png',
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_small.png',
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_thumb.png',
+        #  ]),
+        # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
+        #  'previews',
+        #  [
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_full.png',
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_med.png',
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_small.png',
+        #     'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_thumb.png',
+        #  ]),
         ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
-         'previews',
+         'diagrams',
          [
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_full.png',
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_med.png',
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_small.png',
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_thumb.png'
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_full.png',
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_med.png',
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_small.png',
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_thumb.png',
          ]),
         ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
-         'previews',
+         'diagrams',
          [
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_full.png',
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_med.png',
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_small.png',
-            'previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_thumb.png'
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_full.png',
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_med.png',
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_small.png',
+            'diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_thumb.png',
          ]),
         ('uranus_occs_earthbased',
          'metadata',
          [
             'metadata/uranus_occs_earthbased',
          ]),
         ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
```

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/tests/helper.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pds4file/tests/test_pds4file_blackbox.py` & `rms_pdsfile-0.0.4/pdsfile/pds4file/tests/test_pds4file_blackbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 ##########################################################################################
 # Blackbox tests for pds4file.py
 ##########################################################################################
 class TestPds4FileBlackBox:
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
-             'co-iss-n1308947228'),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947880n.xml',
-             'co-iss-n1308947880'),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947440w.img',
-             'co-iss-w1308947440'),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947440w.img',
-             'co-iss-w1308947440'),
-            ('cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947440w-full.png',
-             'co-iss-w1308947440'),
-            ('cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947880n-full.xml',
-             'co-iss-n1308947880'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub',
-             'co-vims-v1308946681_002'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
-             'co-vims-v1308947235'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947009_xxx/1308947009_002.qub',
-             'co-vims-v1308947009_002'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947715.xml',
-             'co-vims-v1308947715'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
-             'co-vims-v1308947926_008'),
-            ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947235-full.png',
-             'co-vims-v1308947235'),
-            ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_001-full.xml',
-             'co-vims-v1308947079_001'),
-            ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947009_xxx/1308947009_002-full.png',
-             'co-vims-v1308947009_002'),
-            ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947715-full.png',
-             'co-vims-v1308947715'),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            #  'co-iss-n1308947228'),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947880n.xml',
+            #  'co-iss-n1308947880'),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947440w.img',
+            #  'co-iss-w1308947440'),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947440w.img',
+            #  'co-iss-w1308947440'),
+            # ('cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947440w-full.png',
+            #  'co-iss-w1308947440'),
+            # ('cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947880n-full.xml',
+            #  'co-iss-n1308947880'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub',
+            #  'co-vims-v1308946681_002'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
+            #  'co-vims-v1308947235'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947009_xxx/1308947009_002.qub',
+            #  'co-vims-v1308947009_002'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947715.xml',
+            #  'co-vims-v1308947715'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
+            #  'co-vims-v1308947926_008'),
+            # ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947235-full.png',
+            #  'co-vims-v1308947235'),
+            # ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_001-full.xml',
+            #  'co-vims-v1308947079_001'),
+            # ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947009_xxx/1308947009_002-full.png',
+            #  'co-vims-v1308947009_002'),
+            # ('cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947715-full.png',
+            #  'co-vims-v1308947715'),
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
              'kao0m91-vis-occ-1977-069-u0-uranus-e'),
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress.tab',
              'kao0m91-vis-occ-1977-069-u0-uranus-i'),
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_egress_100m.xml',
              'kao0m91-vis-occ-1977-069-u0-ringpl-e'),
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_1000m.tab',
@@ -123,321 +123,378 @@
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
              f'{PDS4_BUNDLES_DIR}/uranus_occs_earthbased/uranus_occ_u0_kao_91cm'),
-             ('cassini_iss/cassini_iss_cruise',
-             f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
-             ('cassini_vims/cassini_vims_cruise',
-             f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
+            #  ('cassini_iss/cassini_iss_cruise',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
+            #  ('cassini_vims/cassini_vims_cruise',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
         ]
     )
     def test_abspath(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.abspath
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml',
-#            'bundles/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml'),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
-            'bundles/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub',
-            'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
-            'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub'),
+           ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml',
+           'bundles/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml'),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            # 'bundles/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub',
+            # 'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
+            # 'bundles/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub'),
         ]
     )
     def test_logical_path(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.logical_path
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml',
-#             True),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/non-existent-filename.txt',
-#             False),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
-            True),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.xml',
-            True),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947009_xxx/1308947009_002.qub',
-            True),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml',
+             True),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/non-existent-filename.txt',
+             False),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+            # True),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.xml',
+            # True),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947009_xxx/1308947009_002.qub',
+            # True),
     ]
     )
     def test_exists(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.exists
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased/',
-#             ''), # bundlesets currently have empty string instead of False
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
-#             True),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
-#             False),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
-#             False),
-            ('cassini_iss',
+            ('uranus_occs_earthbased/',
              ''), # bundlesets currently have empty string instead of False
-            ('cassini_iss/cassini_iss_cruise',
-             True),
-            ('cassini_iss/cassini_iss_cruise/bundle.xml',
-             False),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
-             False),
-            ('cassini_vims',
-             ''), # bundlesets currently have empty string instead of False
-            ('cassini_vims/cassini_vims_cruise',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
              True),
-            ('cassini_vims/cassini_vims_cruise/bundle.xml',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
              False),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
-             False),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.xml',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
              False),
+            # ('cassini_iss',
+            #  ''), # bundlesets currently have empty string instead of False
+            # ('cassini_iss/cassini_iss_cruise',
+            #  True),
+            # ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            #  False),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            #  False),
+            # ('cassini_vims',
+            #  ''), # bundlesets currently have empty string instead of False
+            # ('cassini_vims/cassini_vims_cruise',
+            #  True),
+            # ('cassini_vims/cassini_vims_cruise/bundle.xml',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.xml',
+            #  False),
         ]
     )
     def test_is_bundle(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.is_bundle
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
-#             True), # This test fails with `ValueError: Illegal bundle set directory "": bundles`, because of match failure with BUNDLE_SET_PLUS_REGEX_I on line 3254 of pds4file.py
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/browse',
-#             False),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/xml_schema/collection_xml_schema.csv',
-#             False),
-#            ('uranus_occs_earthbased',
-#             ''), # Bundlesets return empty string, rather than False at the moment
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
-#             False),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
-#             False),
-#            ('uranus_occs_earthbased/',
-#             ''), # bundlesets currently have empty string instead of False
-            ('cassini_iss',
-             ''), # bundlesets currently have empty string instead of False
-            ('cassini_iss/cassini_iss_cruise',
-             True),
-            ('cassini_iss/cassini_iss_cruise/browse',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
+             True), # This test fails with `ValueError: Illegal bundle set directory "": bundles`, because of match failure with BUNDLE_SET_PLUS_REGEX_I on line 3254 of pds4file.py
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/browse',
              False),
-            ('cassini_iss/cassini_iss_cruise/xml_schema/collection_xml_schema.csv',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/xml_schema/collection_xml_schema.csv',
              False),
-            ('cassini_iss/cassini_iss_cruise',
-             True),
-            ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            ('uranus_occs_earthbased',
+             ''), # Bundlesets return empty string, rather than False at the moment
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
              False),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
              False),
-            ('cassini_iss/cassini_iss_cruise/',
-             True),
-            ('cassini_vims',
+            ('uranus_occs_earthbased/',
              ''), # bundlesets currently have empty string instead of False
-            ('cassini_vims/cassini_vims_cruise',
-             True),
-            ('cassini_vims/cassini_vims_cruise/calibration',
-             False),
-            ('cassini_vims/cassini_vims_cruise/xml_schema/collection_xml_schema.csv',
-             False),
-            ('cassini_vims/cassini_vims_cruise',
-             True),
-            ('cassini_vims/cassini_vims_cruise/bundle.xml',
-             False),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
-             False),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx//1308947715.xml',
-             False),
-            ('cassini_vims/cassini_vims_cruise/',
-             True),
+            # ('cassini_iss',
+            #  ''), # bundlesets currently have empty string instead of False
+            # ('cassini_iss/cassini_iss_cruise',
+            #  True),
+            # ('cassini_iss/cassini_iss_cruise/browse',
+            #  False),
+            # ('cassini_iss/cassini_iss_cruise/xml_schema/collection_xml_schema.csv',
+            #  False),
+            # ('cassini_iss/cassini_iss_cruise',
+            #  True),
+            # ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            #  False),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            #  False),
+            # ('cassini_iss/cassini_iss_cruise/',
+            #  True),
+            # ('cassini_vims',
+            #  ''), # bundlesets currently have empty string instead of False
+            # ('cassini_vims/cassini_vims_cruise',
+            #  True),
+            # ('cassini_vims/cassini_vims_cruise/calibration',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise/xml_schema/collection_xml_schema.csv',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise',
+            #  True),
+            # ('cassini_vims/cassini_vims_cruise/bundle.xml',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx//1308947715.xml',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise/',
+            #  True),
         ]
     )
     def test_is_bundle_dir(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.is_bundle_dir
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml',
-#             False),
-#             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
-#             False),
-             ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_alpha_egress_1000m.xml',
              False),
-             ('cassini_iss/cassini_iss_cruise/bundle.xml',
-             False),
-             ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
-             False),
-             ('cassini_vims/cassini_vims_cruise/bundle.xml',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
              False),
+            #  ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            #  False),
+            #  ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            #  False),
+            #  ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
+            #  False),
+            #  ('cassini_vims/cassini_vims_cruise/bundle.xml',
+            #  False),
         ]
     )
     def test_is_bundle_file(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.is_bundle_file
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased',
-#             True),
-#            ('uranus_occs_earthbased/',
-#             True),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
-#             False),
-            ('cassini_iss',
+            ('uranus_occs_earthbased',
              True),
-            ('cassini_vims/',
+            ('uranus_occs_earthbased/',
              True),
-            ('cassini_iss/cassini_iss_cruise/bundle.xml',
-             False),
-            ('cassini_iss/cassini_iss_cruise/',
-             False),
-            ('cassini_vims/cassini_vims_cruise',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
              False),
+            # ('cassini_iss',
+            #  True),
+            # ('cassini_vims/',
+            #  True),
+            # ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            #  False),
+            # ('cassini_iss/cassini_iss_cruise/',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise',
+            #  False),
       ]
     )
     def test_is_bundleset(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.is_bundleset
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased',
-#             True),
-#            ('uranus_occs_earthbased/',
-#             True),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
-#             False),
-            ('cassini_vims',
+            ('uranus_occs_earthbased',
              True),
-            ('cassini_iss/',
+            ('uranus_occs_earthbased/',
              True),
-            ('cassini_iss/cassini_iss_cruise/bundle.xml',
-             False),
-            ('cassini_iss/cassini_iss_cruise',
-             False),
-            ('cassini_vims/cassini_vims_cruise',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
              False),
+            # ('cassini_vims',
+            #  True),
+            # ('cassini_iss/',
+            #  True),
+            # ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            #  False),
+            # ('cassini_iss/cassini_iss_cruise',
+            #  False),
+            # ('cassini_vims/cassini_vims_cruise',
+            #  False),
         ]
     )
     def test_is_bundleset_dir(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.is_bundleset_dir
         assert res == expected
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased/',
-#             'uranus_occs_earthbased'),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
-#             'uranus_occs_earthbased'),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
-#             'uranus_occs_earthbased'),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress.tab',
-#             'uranus_occs_earthbased'),
-            ('cassini_iss/',
-             'cassini_iss'),
-            ('cassini_iss/cassini_iss_cruise',
-             'cassini_iss'),
-            ('cassini_iss/cassini_iss_cruise/bundle.xml',
-             'cassini_iss'),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
-             'cassini_iss'),
-            ('cassini_vims/',
-             'cassini_vims'),
-            ('cassini_vims/cassini_vims_cruise',
-             'cassini_vims'),
-            ('cassini_vims/cassini_vims_cruise/bundle.xml',
-             'cassini_vims'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
-             'cassini_vims'),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
-             'cassini_vims'),
+            ('uranus_occs_earthbased/',
+             'uranus_occs_earthbased'),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
+             'uranus_occs_earthbased'),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
+             'uranus_occs_earthbased'),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_ingress.tab',
+             'uranus_occs_earthbased'),
+            # ('cassini_iss/',
+            #  'cassini_iss'),
+            # ('cassini_iss/cassini_iss_cruise',
+            #  'cassini_iss'),
+            # ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            #  'cassini_iss'),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.img',
+            #  'cassini_iss'),
+            # ('cassini_vims/',
+            #  'cassini_vims'),
+            # ('cassini_vims/cassini_vims_cruise',
+            #  'cassini_vims'),
+            # ('cassini_vims/cassini_vims_cruise/bundle.xml',
+            #  'cassini_vims'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947926_xxx/1308947926_008.qub',
+            #  'cassini_vims'),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947235.qub',
+            #  'cassini_vims'),
         ]
     )
     def test_bundleset(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.bundleset
         assert res == expected
 
 
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-#            ('uranus_occs_earthbased/',
-#             ['uranus_occ_u0_kao_91cm']),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
-#             ['browse', 'bundle.xml', 'bundle_member_index.csv', 'bundle_member_index230313.csv', 'context', 'data', 'document', 'readme.txt', 'xml_schema']),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
-#             []),
-#            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
-#             []),
-            ('cassini_iss/',
-             ['cassini_iss_cruise']),
-            ('cassini_iss/cassini_iss_cruise',
-             ['browse_raw', 'bundle.xml', 'context', 'data_raw', 'document','xml_schema']),
-            ('cassini_iss/cassini_iss_cruise/bundle.xml',
-             []),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+            # expected bundles for uranus are coming from staging server
+            # /volumes/pdsdata-admin/pds4-holdings/bundles/uranus_occs_earthbased
+            ('uranus_occs_earthbased/',
+             ['checksums_uranus_occs_earthbased',
+              'known-errors.txt',
+              'uranus_occ_u11_ctio_400cm',
+              'uranus_occ_u23_ctio_400cm',
+              'uranus_occ_u149_lowell_180cm',
+              'uranus_occ_u138_palomar_508cm',
+              'uranus_occ_u36_sso_390cm',
+              'uranus_occ_u12_eso_360cm',
+              'uranus_occ_u15_mso_190cm',
+              'uranus_occ_u0_kao_91cm',
+              'uranus_occ_u36_sso_230cm',
+              'uranus_occ_u14_ctio_400cm',
+              'uranus_occ_u12_lco_250cm',
+              'uranus_occ_u138_hst_fos',
+              'uranus_occ_u23_teide_155cm',
+              'uranus_occ_u14_eso_104cm',
+              'uranus_occ_u102a_irtf_320cm',
+              'uranus_occ_u9539_ctio_400cm',
+              'uranus_occ_u14_lco_250cm',
+              'uranus_occ_u14_lco_100cm',
+              'uranus_occ_u103_eso_220cm',
+              'uranus_occ_u14_opmt_200cm',
+              'uranus_occ_u14_opmt_106cm',
+              'uranus_occ_u5_lco_250cm',
+              'uranus_occ_u12_eso_104cm',
+              'uranus_occ_support',
+              'uranus_occ_u13_sso_390cm',
+              'uranus_occ_u2_teide_155cm',
+              'uranus_occ_u9_lco_250cm',
+              'uranus_occ_u103_palomar_508cm',
+              'uranus_occ_u23_mcdonald_270cm',
+              'uranus_occ_u25_ctio_400cm',
+              'uranus_occ_u83_irtf_320cm',
+              'uranus_occ_u36_maunakea_380cm',
+              'uranus_occ_u28_irtf_320cm',
+              'uranus_occ_u14_teide_155cm',
+              'uranus_occ_u25_palomar_508cm',
+              'uranus_occ_u36_irtf_320cm',
+              'uranus_occ_u137_irtf_320cm',
+              'uranus_occ_u25_mcdonald_270cm',
+              'uranus_occ_u12_ctio_400cm',
+              'uranus_occ_u16_palomar_508cm',
+              'uranus_occ_u149_irtf_320cm',
+              'uranus_occ_u34_irtf_320cm',
+              'uranus_occ_u65_irtf_320cm',
+              'uranus_occ_u0201_palomar_508cm',
+              'uranus_occ_u1052_irtf_320cm',
+              'uranus_occ_u36_ctio_400cm',
+              'uranus_occ_u134_saao_188cm',
+              'uranus_occ_u144_caha_123cm',
+              'uranus_occ_u17b_saao_188cm',
+              'uranus_occ_u137_hst_fos',
+              'bundleset_index.csv',
+              'uranus_occ_u14_ctio_150cm',
+              'uranus_occ_u144_saao_188cm',
+              'uranus_occ_u102b_irtf_320cm',
+              'uranus_occ_u84_irtf_320cm']),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/bundle.xml',
              []),
-            ('cassini_vims/',
-             ['bundleset_member_index.csv', 'cassini_vims_cruise']),
-            ('cassini_vims/cassini_vims_cruise',
-             ['browse_raw', 'bundle.xml', 'bundle_member_index.csv', 'calibration', 'context', 'data_raw', 'document', 'xml_schema']),
-            ('cassini_vims/cassini_vims_cruise/bundle.xml',
-             []),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub',
-             []),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/13089xxxxx/1308947235.xml',
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
              []),
+            # ('cassini_iss/',
+            #  ['cassini_iss_cruise']),
+            # ('cassini_iss/cassini_iss_cruise',
+            #  ['browse_raw', 'bundle.xml', 'context', 'data_raw', 'document','xml_schema']),
+            # ('cassini_iss/cassini_iss_cruise/bundle.xml',
+            #  []),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+            #  []),
+            # ('cassini_vims/',
+            #  ['bundleset_member_index.csv', 'cassini_vims_cruise']),
+            # ('cassini_vims/cassini_vims_cruise',
+            #  ['browse_raw', 'bundle.xml', 'bundle_member_index.csv', 'calibration', 'context', 'data_raw', 'document', 'xml_schema']),
+            # ('cassini_vims/cassini_vims_cruise/bundle.xml',
+            #  []),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_002.qub',
+            #  []),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/13089xxxxx/1308947235.xml',
+            #  []),
         ]
     )
     def test_childnames(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.childnames
-        assert set(res) == set(expected)
+        for child in res:
+            assert child in expected
 
     @pytest.mark.parametrize(
     'input_path,expected',
         [
-            ('cassini_iss/cassini_iss_cruise',
-             f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
-            ('cassini_iss_cruise',
-             f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
-            ('cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml',
-             f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'),
-            ('cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml',
-             f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'),
-            ('cassini_vims/cassini_vims_cruise',
-             f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
-            ('cassini_vims_cruise',
-             f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
-            ('cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml',
-             f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml'),
+            # ('cassini_iss/cassini_iss_cruise',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
+            # ('cassini_iss_cruise',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
+            # ('cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'),
+            # ('cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'),
+            # ('cassini_vims/cassini_vims_cruise',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
+            # ('cassini_vims_cruise',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
+            # ('cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml'),
             ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm',
              f'{PDS4_BUNDLES_DIR}/uranus_occs_earthbased/uranus_occ_u0_kao_91cm'),
             ('uranus_occ_u0_kao_91cm',
              f'{PDS4_BUNDLES_DIR}/uranus_occs_earthbased/uranus_occ_u0_kao_91cm'),
             ('uranus_occ_u0_kao_91cm/data/atmosphere',
              f'{PDS4_BUNDLES_DIR}/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere'),
             ('uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
@@ -450,20 +507,20 @@
         res = pds4file.Pds4File.from_path(path=input_path)
         assert isinstance(res, pds4file.PdsFile)
         assert res.abspath == expected
 
     @pytest.mark.parametrize(
         'filespec,expected',
         [
-            ('cassini_iss_cruise', f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
-            ('cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml',
-             f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'),
-            ('cassini_vims_cruise', f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
-            ('cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml',
-             f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml'),
+            # ('cassini_iss_cruise', f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise'),
+            # ('cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_iss/cassini_iss_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308947228n-full.xml'),
+            # ('cassini_vims_cruise', f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise'),
+            # ('cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml',
+            #  f'{PDS4_BUNDLES_DIR}/cassini_vims/cassini_vims_cruise/browse_raw/130xxxxxxx/13089xxxxx/1308946681_xxx/1308946681_001-full.xml'),
             ('uranus_occ_u0_kao_91cm',
              f'{PDS4_BUNDLES_DIR}/uranus_occs_earthbased/uranus_occ_u0_kao_91cm'),
             ('uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
              f'{PDS4_BUNDLES_DIR}/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml'),
         ]
     )
     def test_from_filespec(self, filespec, expected):
@@ -473,54 +530,71 @@
         assert res.abspath == expected
 
 
     # For now we fake all the images files under previews dir
     @pytest.mark.parametrize(
         'input_path,expected',
         [
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
-             [
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_full.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_med.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_small.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_thumb.png',
-             ]
-            ),
-            ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n.img',
-             [
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_full.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_med.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_small.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_thumb.png',
-             ]
-            ),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
-             [
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_full.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_med.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_small.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_thumb.png',
-             ]
-            ),
-            ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
-             [
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_full.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_med.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_small.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_thumb.png',
-             ]
-            ),
-            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
-             [
-                 f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_full.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_med.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_small.png',
-                 f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_thumb.png',
-             ]
-            ),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n.xml',
+            #  [
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_full.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_med.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_small.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947228n_thumb.png',
+            #  ]
+            # ),
+            # ('cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n.img',
+            #  [
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_full.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_med.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_small.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_iss/cassini_iss_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947273n_thumb.png',
+            #  ]
+            # ),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223.xml',
+            #  [
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_full.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_med.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_small.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947223_thumb.png',
+            #  ]
+            # ),
+            # ('cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003.qub',
+            #  [
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_full.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_med.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_small.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_thumb.png',
+            #  ]
+            # ),
+            # TODO: uncomment these test cases when previews for uranus occ are available
+            # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_100m.xml',
+            #  [
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_full.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_med.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_small.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_thumb.png'
+            #  ]
+            # ),
+            # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
+            #  [
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_full.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_med.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_small.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_thumb.png'
+            #  ]
+            # ),
+            # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_100m.xml',
+            #  [
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_full.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_med.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_small.png',
+            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_thumb.png'
+            #  ]
+            # ),
         ]
     )
     def test_viewset(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.viewset
         if res != False:
             assert isinstance(res, pdsviewable.PdsViewSet)
```

### Comparing `rms_pdsfile-0.0.3/pdsfile/pdscache.py` & `rms_pdsfile-0.0.4/pdsfile/pdscache.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pdsfile.py` & `rms_pdsfile-0.0.4/pdsfile/pdsfile.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/pdsviewable.py` & `rms_pdsfile-0.0.4/pdsfile/pdsviewable.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pdsfile/preload_and_cache.py` & `rms_pdsfile-0.0.4/pdsfile/preload_and_cache.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/pyproject.toml` & `rms_pdsfile-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/rms_pdsfile.egg-info/PKG-INFO` & `rms_pdsfile-0.0.4/rms_pdsfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.3
+Version: 0.0.4
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms_pdsfile-0.0.3/rms_pdsfile.egg-info/SOURCES.txt` & `rms_pdsfile-0.0.4/rms_pdsfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/run_tests_coverage.sh` & `rms_pdsfile-0.0.4/run_tests_coverage.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/scripts/automated_tests/pdsfile_main_test.sh` & `rms_pdsfile-0.0.4/scripts/automated_tests/pdsfile_main_test.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/pdsarchives.py` & `rms_pdsfile-0.0.4/validation/pdsarchives.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/pdschecksums.py` & `rms_pdsfile-0.0.4/validation/pdschecksums.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/pdsdata-sync.sh` & `rms_pdsfile-0.0.4/validation/pdsdata-sync.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/pdsdependency.py` & `rms_pdsfile-0.0.4/validation/pdsdependency.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/pdsindexshelf.py` & `rms_pdsfile-0.0.4/validation/pdsindexshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/pdsinfoshelf.py` & `rms_pdsfile-0.0.4/validation/pdsinfoshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/pdslinkshelf.py` & `rms_pdsfile-0.0.4/validation/pdslinkshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/re-validate.py` & `rms_pdsfile-0.0.4/validation/re-validate.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.3/validation/shelf-consistency-check.py` & `rms_pdsfile-0.0.4/validation/shelf-consistency-check.py`

 * *Files identical despite different names*

