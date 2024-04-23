# Comparing `tmp/rms_pdsfile-0.0.4.tar.gz` & `tmp/rms_pdsfile-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms_pdsfile-0.0.4.tar", last modified: Tue Apr 23 00:01:53 2024, max compression
+gzip compressed data, was "rms_pdsfile-0.0.5.tar", last modified: Tue Apr 23 17:46:20 2024, max compression
```

## Comparing `rms_pdsfile-0.0.4.tar` & `rms_pdsfile-0.0.5.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.629398 rms_pdsfile-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.633398 rms_pdsfile-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/run-tests-and-opus.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.633398 rms_pdsfile-0.0.4/pdsfile/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/pdsfile/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.633398 rms_pdsfile-0.0.4/pdsfile/pds3file/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/ASTROM_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COCIRS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/CORSS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_8xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/EBROCC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/GO_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/HSTxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJIR_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJNC_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHSP_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHxxxx_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RES_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RPX_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGIRIS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGISS_xxxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_0xxx.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_20xx.py
--rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_28xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/rules/pytest_support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
--rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_whitebox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds4file/
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/
--rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23705 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_iss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24866 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_vims.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/pytest_support.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    65261 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased.py
--rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.641399 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    38424 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pds4file/tests/test_pds4file_blackbox.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pdscache.py
--rw-r--r--   0 runner    (1001) docker     (127)   230951 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pdsfile.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/pdsviewable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pdsfile/preload_and_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 00:01:53.000000 rms_pdsfile-0.0.4/rms_pdsfile.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/run_tests_coverage.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.629398 rms_pdsfile-0.0.4/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/scripts/automated_tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/scripts/automated_tests/pdsfile_main_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 00:01:53.645398 rms_pdsfile-0.0.4/validation/
--rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsarchives.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdschecksums.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsdata-sync.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsdependency.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsindexshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdsinfoshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/pdslinkshelf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/re-validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-23 00:01:49.000000 rms_pdsfile-0.0.4/validation/shelf-consistency-check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.902540 rms_pdsfile-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.886540 rms_pdsfile-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.890540 rms_pdsfile-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/.github/workflows/run-tests-and-opus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 17:46:20.902540 rms_pdsfile-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.890540 rms_pdsfile-0.0.5/pdsfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 17:46:20.000000 rms_pdsfile-0.0.5/pdsfile/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.890540 rms_pdsfile-0.0.5/pdsfile/pds3file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.894540 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1513 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/ASTROM_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61669 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COCIRS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46937 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    51098 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/CORSS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2378 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25774 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COUVIS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22138 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COUVIS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43611 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COVIMS_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22895 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COVIMS_8xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20096 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/EBROCC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    77854 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/GO_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21822 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/HSTxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9721 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/JNOJIR_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7790 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/JNOJNC_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2388 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/JNOSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2380 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/NHSP_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53813 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/NHxxxx_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/RES_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12928 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/RPX_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2523 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VGIRIS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64913 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VGISS_xxxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12074 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VG_0xxx.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2483 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VG_20xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)   129879 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VG_28xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36492 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4823 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/rules/pytest_support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.894540 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    89512 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pds3file_blackbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30950 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35786 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pds3file_whitebox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.894540 rms_pdsfile-0.0.5/pdsfile/pds4file/
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.898540 rms_pdsfile-0.0.5/pdsfile/pds4file/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)    36279 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/rules/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23705 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/rules/cassini_iss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24866 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/rules/cassini_vims.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4872 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/rules/pytest_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    65261 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/rules/uranus_occs_earthbased.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101120 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.898540 rms_pdsfile-0.0.5/pdsfile/pds4file/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38357 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pds4file/tests/test_pds4file_blackbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34894 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pdscache.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230951 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pdsfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19658 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/pdsviewable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pdsfile/preload_and_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.902540 rms_pdsfile-0.0.5/rms_pdsfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 17:46:20.000000 rms_pdsfile-0.0.5/rms_pdsfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-23 17:46:20.000000 rms_pdsfile-0.0.5/rms_pdsfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:46:20.000000 rms_pdsfile-0.0.5/rms_pdsfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-23 17:46:20.000000 rms_pdsfile-0.0.5/rms_pdsfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 17:46:20.000000 rms_pdsfile-0.0.5/rms_pdsfile.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      761 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/run_tests_coverage.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.886540 rms_pdsfile-0.0.5/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.898540 rms_pdsfile-0.0.5/scripts/automated_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/scripts/automated_tests/pdsfile_main_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 17:46:20.902540 rms_pdsfile-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:46:20.902540 rms_pdsfile-0.0.5/validation/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18175 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/pdsarchives.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31377 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/pdschecksums.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/pdsdata-sync.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34502 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/pdsdependency.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17150 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/pdsindexshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31801 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/pdsinfoshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    73841 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/pdslinkshelf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29426 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/re-validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-23 17:46:07.000000 rms_pdsfile-0.0.5/validation/shelf-consistency-check.py
```

### Comparing `rms_pdsfile-0.0.4/.github/workflows/publish_to_pypi.yml` & `rms_pdsfile-0.0.5/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/.github/workflows/publish_to_test_pypi.yml` & `rms_pdsfile-0.0.5/.github/workflows/publish_to_test_pypi.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/.github/workflows/run-tests-and-opus.yml` & `rms_pdsfile-0.0.5/.github/workflows/run-tests-and-opus.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Checkout rms-opus
         uses: actions/checkout@v4
         with:
           repository: SETI/rms-opus
           path: rms-opus
-          # ref: uranus_occs_earthbased
+          # ref: rf240417_ring_names
           # Currently we just checkout the current master branch for OPUS.
           # We really need some way to specify a branch so that we can do
           # parallel inter-dependent development on PdsFile and OPUS.
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `rms_pdsfile-0.0.4/.github/workflows/run-tests.yml` & `rms_pdsfile-0.0.5/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/.gitignore` & `rms_pdsfile-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/CODE_OF_CONDUCT.md` & `rms_pdsfile-0.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/CONTRIBUTING.md` & `rms_pdsfile-0.0.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/LICENSE` & `rms_pdsfile-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/PKG-INFO` & `rms_pdsfile-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.4
+Version: 0.0.5
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms_pdsfile-0.0.4/README.md` & `rms_pdsfile-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/conftest.py` & `rms_pdsfile-0.0.5/conftest.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/__init__.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/ASTROM_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/ASTROM_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COCIRS_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COCIRS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COISS_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/CORSS_8xxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/CORSS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COSP_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_0xxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COUVIS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COUVIS_8xxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COUVIS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_0xxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COVIMS_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/COVIMS_8xxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/COVIMS_8xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/EBROCC_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/EBROCC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/GO_0xxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/GO_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/HSTxx_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/HSTxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJIR_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/JNOJIR_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOJNC_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/JNOJNC_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/JNOSP_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/JNOSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHSP_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/NHSP_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/NHxxxx_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/NHxxxx_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RES_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/RES_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/RPX_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/RPX_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGIRIS_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VGIRIS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VGISS_xxxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VGISS_xxxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_0xxx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VG_0xxx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_20xx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VG_20xx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/VG_28xx.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/VG_28xx.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/__init__.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/rules/pytest_support.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/helper.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pds3file_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pds3file_blackbox_cached.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pds3file_whitebox.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pds3file_whitebox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py` & `rms_pdsfile-0.0.5/pdsfile/pds3file/tests/test_pdsviewable_blackbox.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/__init__.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/__init__.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_iss.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/rules/cassini_iss.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/cassini_vims.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/rules/cassini_vims.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/pytest_support.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/rules/pytest_support.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/rules/uranus_occs_earthbased.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,24 @@
 
 ##########################################################################################
 # VIEWABLES
 ##########################################################################################
 
 default_viewables = translator.TranslatorByRegex([
     (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/atmosphere/.*-v-.*)\.[a-z]{3}', 0,
-        [r'previews/\1_preview_full.png',
-         r'previews/\1_preview_med.png',
-         r'previews/\1_preview_small.png',
-         r'previews/\1_preview_thumb.png',
+        [r'diagrams/\1_diagram_full.png',
+         r'diagrams/\1_diagram_med.png',
+         r'diagrams/\1_diagram_small.png',
+         r'diagrams/\1_diagram_thumb.png',
     ]),
     (r'.*/(uranus_occs_earthbased/uranus_occ_u.*/data/(rings|global))/(.*)_\d+m\.[a-z]{3}', 0,
-        [r'previews/\1/\3_preview_full.png',
-         r'previews/\1/\3_preview_med.png',
-         r'previews/\1/\3_preview_small.png',
-         r'previews/\1/\3_preview_thumb.png',
+        [r'diagrams/\1/\3_diagram_full.png',
+         r'diagrams/\1/\3_diagram_med.png',
+         r'diagrams/\1/\3_diagram_small.png',
+         r'diagra,s/\1/\3_diagram_thumb.png',
     ]),
 ])
 
 ##########################################################################################
 # ASSOCIATIONS
 ##########################################################################################
```

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/rules/uranus_occs_earthbased_primary_filespec.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/tests/helper.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/tests/helper.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pds4file/tests/test_pds4file_blackbox.py` & `rms_pdsfile-0.0.5/pdsfile/pds4file/tests/test_pds4file_blackbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,39 +562,39 @@
             #  [
             #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_full.png',
             #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_med.png',
             #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_small.png',
             #      f'/{PDS4_HOLDINGS_NAME}/previews/cassini_vims/cassini_vims_cruise/data_raw/130xxxxxxx/13089xxxxx/1308947079_xxx/1308947079_003_thumb.png',
             #  ]
             # ),
-            # TODO: uncomment these test cases when previews for uranus occ are available
-            # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_100m.xml',
-            #  [
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_full.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_med.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_small.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_preview_thumb.png'
-            #  ]
-            # ),
-            # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
-            #  [
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_full.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_med.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_small.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_preview_thumb.png'
-            #  ]
-            # ),
-            # ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_100m.xml',
-            #  [
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_full.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_med.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_small.png',
-            #      f'/{PDS4_HOLDINGS_NAME}/previews/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_preview_thumb.png'
-            #  ]
-            # ),
+            # TODO: change these test cases to previews when available
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_100m.xml',
+             [
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_full.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_med.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_small.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/rings/u0_kao_91cm_734nm_radius_delta_egress_diagram_thumb.png'
+             ]
+            ),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress.xml',
+             [
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_full.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_med.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_small.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/atmosphere/u0_kao_91cm_734nm_counts-v-time_atmos_egress_diagram_thumb.png'
+             ]
+            ),
+            ('uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_100m.xml',
+             [
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_full.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_med.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_small.png',
+                 f'/{PDS4_HOLDINGS_NAME}/diagrams/uranus_occs_earthbased/uranus_occ_u0_kao_91cm/data/global/u0_kao_91cm_734nm_radius_equator_ingress_diagram_thumb.png'
+             ]
+            ),
         ]
     )
     def test_viewset(self, input_path, expected):
         target_pdsfile = instantiate_target_pdsfile(input_path)
         res = target_pdsfile.viewset
         if res != False:
             assert isinstance(res, pdsviewable.PdsViewSet)
```

### Comparing `rms_pdsfile-0.0.4/pdsfile/pdscache.py` & `rms_pdsfile-0.0.5/pdsfile/pdscache.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pdsfile.py` & `rms_pdsfile-0.0.5/pdsfile/pdsfile.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/pdsviewable.py` & `rms_pdsfile-0.0.5/pdsfile/pdsviewable.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pdsfile/preload_and_cache.py` & `rms_pdsfile-0.0.5/pdsfile/preload_and_cache.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/pyproject.toml` & `rms_pdsfile-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/rms_pdsfile.egg-info/PKG-INFO` & `rms_pdsfile-0.0.5/rms_pdsfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rms-pdsfile
-Version: 0.0.4
+Version: 0.0.5
 Summary: pdsfile
 Maintainer-email: "Robert S. French" <rfrench@seti.org>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/SETI/rms-pdsfile
 Project-URL: Repository, https://github.com/SETI/rms-pdsfile
 Project-URL: Source, https://github.com/SETI/rms-pdsfile
 Project-URL: Issues, https://github.com/SETI/rms-pdsfile/issues
```

### Comparing `rms_pdsfile-0.0.4/rms_pdsfile.egg-info/SOURCES.txt` & `rms_pdsfile-0.0.5/rms_pdsfile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/run_tests_coverage.sh` & `rms_pdsfile-0.0.5/run_tests_coverage.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/scripts/automated_tests/pdsfile_main_test.sh` & `rms_pdsfile-0.0.5/scripts/automated_tests/pdsfile_main_test.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/pdsarchives.py` & `rms_pdsfile-0.0.5/validation/pdsarchives.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/pdschecksums.py` & `rms_pdsfile-0.0.5/validation/pdschecksums.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/pdsdata-sync.sh` & `rms_pdsfile-0.0.5/validation/pdsdata-sync.sh`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/pdsdependency.py` & `rms_pdsfile-0.0.5/validation/pdsdependency.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/pdsindexshelf.py` & `rms_pdsfile-0.0.5/validation/pdsindexshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/pdsinfoshelf.py` & `rms_pdsfile-0.0.5/validation/pdsinfoshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/pdslinkshelf.py` & `rms_pdsfile-0.0.5/validation/pdslinkshelf.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/re-validate.py` & `rms_pdsfile-0.0.5/validation/re-validate.py`

 * *Files identical despite different names*

### Comparing `rms_pdsfile-0.0.4/validation/shelf-consistency-check.py` & `rms_pdsfile-0.0.5/validation/shelf-consistency-check.py`

 * *Files identical despite different names*

