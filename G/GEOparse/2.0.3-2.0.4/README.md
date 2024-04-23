# Comparing `tmp/GEOparse-2.0.3.tar.gz` & `tmp/geoparse-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GEOparse-2.0.3.tar", last modified: Wed Feb  3 20:49:31 2021, max compression
+gzip compressed data, was "geoparse-2.0.4.tar", last modified: Tue Apr 23 18:59:15 2024, max compression
```

## Comparing `GEOparse-2.0.3.tar` & `geoparse-2.0.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-03 20:49:31.637439 GEOparse-2.0.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      291 2021-02-03 20:45:51.000000 GEOparse-2.0.3/.editorconfig
--rw-rw-r--   0 travis    (2000) travis    (2000)     1023 2021-02-03 20:45:51.000000 GEOparse-2.0.3/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      320 2021-02-03 20:45:51.000000 GEOparse-2.0.3/AUTHORS.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2925 2021-02-03 20:45:51.000000 GEOparse-2.0.3/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4204 2021-02-03 20:45:51.000000 GEOparse-2.0.3/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2021-02-03 20:45:51.000000 GEOparse-2.0.3/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2021-02-03 20:45:51.000000 GEOparse-2.0.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     8351 2021-02-03 20:49:31.637439 GEOparse-2.0.3/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1281 2021-02-03 20:45:51.000000 GEOparse-2.0.3/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-03 20:49:31.633439 GEOparse-2.0.3/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20987 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/Analyse_hsa-miR-124a-3p_transfection_time-course.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      739 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/GEOparse.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6769 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/authors.rst
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8525 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/introduction.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6462 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/modules.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    39083 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/output_20_0.png
--rw-rw-r--   0 travis    (2000) travis    (2000)    52034 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/output_43_1.png
--rw-rw-r--   0 travis    (2000) travis    (2000)     7586 2021-02-03 20:45:51.000000 GEOparse-2.0.3/docs/usage.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-03 20:49:31.633439 GEOparse-2.0.3/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3345 2021-02-03 20:45:51.000000 GEOparse-2.0.3/scripts/geo2fastq
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-02-03 20:49:31.637439 GEOparse-2.0.3/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2057 2021-02-03 20:45:51.000000 GEOparse-2.0.3/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-03 20:49:31.629439 GEOparse-2.0.3/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-03 20:49:31.633439 GEOparse-2.0.3/src/GEOparse/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    39720 2021-02-03 20:45:51.000000 GEOparse-2.0.3/src/GEOparse/GEOTypes.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    23879 2021-02-03 20:45:51.000000 GEOparse-2.0.3/src/GEOparse/GEOparse.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      361 2021-02-03 20:45:51.000000 GEOparse-2.0.3/src/GEOparse/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8957 2021-02-03 20:45:51.000000 GEOparse-2.0.3/src/GEOparse/downloader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1276 2021-02-03 20:45:51.000000 GEOparse-2.0.3/src/GEOparse/logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10210 2021-02-03 20:45:51.000000 GEOparse-2.0.3/src/GEOparse/sra_downloader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8769 2021-02-03 20:45:51.000000 GEOparse-2.0.3/src/GEOparse/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-03 20:49:31.633439 GEOparse-2.0.3/src/GEOparse.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8351 2021-02-03 20:49:31.000000 GEOparse-2.0.3/src/GEOparse.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1375 2021-02-03 20:49:31.000000 GEOparse-2.0.3/src/GEOparse.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-03 20:49:31.000000 GEOparse-2.0.3/src/GEOparse.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-03 20:49:31.000000 GEOparse-2.0.3/src/GEOparse.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       54 2021-02-03 20:49:31.000000 GEOparse-2.0.3/src/GEOparse.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2021-02-03 20:49:31.000000 GEOparse-2.0.3/src/GEOparse.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-03 20:49:31.637439 GEOparse-2.0.3/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)   162654 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/Analyse_hsa-miR-124a-3p_transfection_time-course.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)     4570 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/GPL20814_family.soft
--rw-rw-r--   0 travis    (2000) travis    (2000)     5742 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/GPL4133.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     5752 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/GPL4134.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1882 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/GSE105845_family.soft
--rw-rw-r--   0 travis    (2000) travis    (2000)      432 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/GSE6207_experiments.tab
--rw-rw-r--   0 travis    (2000) travis    (2000)      423 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/GSM2795971.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      839 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/GSM32878.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)       52 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)   101355 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/seed-mirza-g_all_mirnas_per_gene_scores_miR_124a.tab
--rw-rw-r--   0 travis    (2000) travis    (2000)    22701 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/soft_ex_family.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)    24808 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/test_GEOparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/test_gsm_annotated.tab
--rw-rw-r--   0 travis    (2000) travis    (2000)      924 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/test_merged_by_id_and_averaged_by_gb_acc.tab
--rw-rw-r--   0 travis    (2000) travis    (2000)      828 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/test_sample_pivoted_by_value.tab
--rw-rw-r--   0 travis    (2000) travis    (2000)     1013 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tests/test_sample_pivoted_by_value_and_annotated_by_gbacc.tab
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2021-02-03 20:45:51.000000 GEOparse-2.0.3/tox.ini
+drwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)        0 2024-04-23 18:59:15.579777 geoparse-2.0.4/
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      291 2024-04-23 18:48:06.000000 geoparse-2.0.4/.editorconfig
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1023 2024-04-23 18:48:06.000000 geoparse-2.0.4/.travis.yml
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      320 2024-04-23 18:48:06.000000 geoparse-2.0.4/AUTHORS.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     2925 2024-04-23 18:48:06.000000 geoparse-2.0.4/CONTRIBUTING.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     4204 2024-04-23 18:48:36.000000 geoparse-2.0.4/HISTORY.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1469 2024-04-23 18:48:06.000000 geoparse-2.0.4/LICENSE
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      308 2024-04-23 18:48:06.000000 geoparse-2.0.4/MANIFEST.in
+-rw-r--r--   0 rgumienny  (1000) rgumienny  (1000)     6522 2024-04-23 18:59:15.579777 geoparse-2.0.4/PKG-INFO
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1281 2024-04-23 18:48:06.000000 geoparse-2.0.4/README.rst
+drwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)        0 2024-04-23 18:59:15.571777 geoparse-2.0.4/docs/
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)    20987 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/Analyse_hsa-miR-124a-3p_transfection_time-course.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      739 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/GEOparse.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     6769 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/Makefile
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       27 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/authors.rst
+-rwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)     8525 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/conf.py
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       32 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/contributing.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       27 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/history.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      520 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/index.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      402 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/installation.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       26 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/introduction.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     6462 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/make.bat
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       61 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/modules.rst
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)    39083 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/output_20_0.png
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)    52034 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/output_43_1.png
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     7585 2024-04-23 18:48:06.000000 geoparse-2.0.4/docs/usage.rst
+drwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)        0 2024-04-23 18:59:15.575777 geoparse-2.0.4/scripts/
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     3345 2024-04-23 18:48:06.000000 geoparse-2.0.4/scripts/geo2fastq
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       38 2024-04-23 18:59:15.579777 geoparse-2.0.4/setup.cfg
+-rwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)     2057 2024-04-23 18:48:43.000000 geoparse-2.0.4/setup.py
+drwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)        0 2024-04-23 18:59:15.563778 geoparse-2.0.4/src/
+drwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)        0 2024-04-23 18:59:15.575777 geoparse-2.0.4/src/GEOparse/
+-rwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)    39796 2024-04-23 18:48:06.000000 geoparse-2.0.4/src/GEOparse/GEOTypes.py
+-rwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)    23879 2024-04-23 18:48:06.000000 geoparse-2.0.4/src/GEOparse/GEOparse.py
+-rwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)      361 2024-04-23 18:48:30.000000 geoparse-2.0.4/src/GEOparse/__init__.py
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     8987 2024-04-23 18:48:06.000000 geoparse-2.0.4/src/GEOparse/downloader.py
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1276 2024-04-23 18:48:06.000000 geoparse-2.0.4/src/GEOparse/logger.py
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)    10025 2024-04-23 18:48:06.000000 geoparse-2.0.4/src/GEOparse/sra_downloader.py
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     8769 2024-04-23 18:48:06.000000 geoparse-2.0.4/src/GEOparse/utils.py
+drwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)        0 2024-04-23 18:59:15.579777 geoparse-2.0.4/src/GEOparse.egg-info/
+-rw-r--r--   0 rgumienny  (1000) rgumienny  (1000)     6522 2024-04-23 18:59:15.000000 geoparse-2.0.4/src/GEOparse.egg-info/PKG-INFO
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1375 2024-04-23 18:59:15.000000 geoparse-2.0.4/src/GEOparse.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)        1 2024-04-23 18:59:15.000000 geoparse-2.0.4/src/GEOparse.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)        1 2024-04-23 18:59:15.000000 geoparse-2.0.4/src/GEOparse.egg-info/not-zip-safe
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       54 2024-04-23 18:59:15.000000 geoparse-2.0.4/src/GEOparse.egg-info/requires.txt
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)        9 2024-04-23 18:59:15.000000 geoparse-2.0.4/src/GEOparse.egg-info/top_level.txt
+drwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)        0 2024-04-23 18:59:15.579777 geoparse-2.0.4/tests/
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)   162654 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/Analyse_hsa-miR-124a-3p_transfection_time-course.ipynb
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     4570 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/GPL20814_family.soft
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     5742 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/GPL4133.txt
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     5752 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/GPL4134.txt
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1882 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/GSE105845_family.soft
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      432 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/GSE6207_experiments.tab
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      423 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/GSM2795971.txt
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      839 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/GSM32878.txt
+-rwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)       52 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/__init__.py
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)       55 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/pytest.ini
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)   101355 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/seed-mirza-g_all_mirnas_per_gene_scores_miR_124a.tab
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)    22701 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/soft_ex_family.txt
+-rwxrwxr-x   0 rgumienny  (1000) rgumienny  (1000)    24808 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/test_GEOparse.py
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1321 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/test_gsm_annotated.tab
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      924 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/test_merged_by_id_and_averaged_by_gb_acc.tab
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      828 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/test_sample_pivoted_by_value.tab
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)     1013 2024-04-23 18:48:06.000000 geoparse-2.0.4/tests/test_sample_pivoted_by_value_and_annotated_by_gbacc.tab
+-rw-rw-r--   0 rgumienny  (1000) rgumienny  (1000)      272 2024-04-23 18:48:06.000000 geoparse-2.0.4/tox.ini
```

### Comparing `GEOparse-2.0.3/.travis.yml` & `geoparse-2.0.4/.travis.yml`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/CONTRIBUTING.rst` & `geoparse-2.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/HISTORY.rst` & `geoparse-2.0.4/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/LICENSE` & `geoparse-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/README.rst` & `geoparse-2.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/Analyse_hsa-miR-124a-3p_transfection_time-course.rst` & `geoparse-2.0.4/docs/Analyse_hsa-miR-124a-3p_transfection_time-course.rst`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/GEOparse.rst` & `geoparse-2.0.4/docs/GEOparse.rst`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/Makefile` & `geoparse-2.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/conf.py` & `geoparse-2.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/index.rst` & `geoparse-2.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/make.bat` & `geoparse-2.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/output_20_0.png` & `geoparse-2.0.4/docs/output_20_0.png`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/output_43_1.png` & `geoparse-2.0.4/docs/output_43_1.png`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/docs/usage.rst` & `geoparse-2.0.4/docs/usage.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     print()
     print("GSM example:")
     for gsm_name, gsm in gse.gsms.items():
         print("Name: ", gsm_name)
         print("Metadata:",)
         for key, value in gsm.metadata.items():
             print(" - %s : %s" % (key, ", ".join(value)))
-        print ("Table data:",)
-        print (gsm.table.head())
+        print("Table data:",)
+        print(gsm.table.head())
         break
 
     print()
     print("GPL example:")
     for gpl_name, gpl in gse.gpls.items():
         print("Name: ", gpl_name)
         print("Metadata:",)
@@ -56,15 +56,15 @@
 specifying path to the file::
 
     import GEOparse
     gse = GEOparse.get_GEO(filepath="./GSE1563.soft.gz")
 
 This will read the file into GSE object.
 
-Crating and saving SOFT file
+Creating and saving SOFT file
 ----------------------------
 
 When doing own experiments one might want to submit the data to the GEO. In this case, one shuld
 first create all necessary elements of given GEO object, create this object and use :func:`to_soft`
 method to save it as SOFT files.
 
 .. warning::
```

### Comparing `GEOparse-2.0.3/scripts/geo2fastq` & `geoparse-2.0.4/scripts/geo2fastq`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/setup.py` & `geoparse-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 test_requirements = [
     "tox",
 ]
 
 setup(
     name="GEOparse",
-    version="2.0.3",
+    version="2.0.4",
     description="Python library to access Gene Expression Omnibus Database (GEO)",
     long_description=readme + "\n\n" + history,
     author="Rafal Gumienny",
     author_email="guma44@gmail.com",
     url="https://github.com/guma44/GEOparse",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `GEOparse-2.0.3/src/GEOparse/GEOTypes.py` & `geoparse-2.0.4/src/GEOparse/GEOTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,39 +483,40 @@
         utils.mkdir_p(os.path.abspath(directory_path))
         downloaded_paths = dict()
         if sra_kwargs is None:
             sra_kwargs = {}
         # Possible erroneous values that could be identified and skipped right
         # after
         blacklist = ("NONE",)
+
         for metakey, metavalue in iteritems(self.metadata):
             if "supplementary_file" in metakey:
-                assert len(metavalue) == 1 and metavalue != ""
-                if metavalue[0] in blacklist:
-                    logger.warning(
-                        "%s value is blacklisted as '%s' - skipping"
-                        % (metakey, metavalue[0])
-                    )
-                    continue
                 # SRA will be downloaded elsewhere
-                if "sra" not in metavalue[0]:
-                    download_path = os.path.abspath(
-                        os.path.join(
-                            directory,
-                            os.path.join(directory_path, metavalue[0].split("/")[-1]),
+                for one_metavalue in metavalue:
+                    if one_metavalue in blacklist:
+                        logger.warning(
+                            "%s value is blacklisted as '%s' - skipping"
+                            % (metakey, one_metavalue)
                         )
-                    )
-                    try:
-                        utils.download_from_url(metavalue[0], download_path)
-                        downloaded_paths[metavalue[0]] = download_path
-                    except Exception as err:
-                        logger.error(
-                            "Cannot download %s supplementary file (%s)"
-                            % (self.get_accession(), err)
+                        continue
+                    if "sra" not in one_metavalue:
+                        download_path = os.path.abspath(
+                            os.path.join(
+                                directory,
+                                os.path.join(directory_path, one_metavalue.split("/")[-1]),
+                            )
                         )
+                        try:
+                            utils.download_from_url(one_metavalue, download_path)
+                            downloaded_paths[one_metavalue] = download_path
+                        except Exception as err:
+                            logger.error(
+                                "Cannot download %s supplementary file (%s)"
+                                % (self.get_accession(), err)
+                            )
         if download_sra:
             try:
                 downloaded_files = self.download_SRA(
                     email, directory=directory, **sra_kwargs
                 )
                 downloaded_paths.update(downloaded_files)
             except Exception as err:
```

### Comparing `GEOparse-2.0.3/src/GEOparse/GEOparse.py` & `geoparse-2.0.4/src/GEOparse/GEOparse.py`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/src/GEOparse/downloader.py` & `geoparse-2.0.4/src/GEOparse/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,21 +138,22 @@
     def _get_filename(self):
         filename = os.path.basename(urlparse(self.url).path).strip(" \n\t.")
         if len(filename) == 0:
             raise Exception("Cannot parse filename from %s" % self.url)
         return filename
 
     def _download_ftp(self, silent=False):
+        total_size = 0
         parsed_url = urlparse(self.url)
         try:
             ftp = FTP(parsed_url.netloc)
             ftp.login()
-            total_size = ftp.size(parsed_url.path)
-            if total_size is None:
-                total_size = 0
+            ftp_size = ftp.size(parsed_url.path)
+            if ftp_size is not None:
+                total_size = ftp_size
             wrote = list()  # cannot add in the callback, has to be a list
             with open(self._temp_file_name, "wb") as f:
                 if silent:
 
                     def _write(data):
                         f.write(data)
                         wrote.append(len(data))
```

### Comparing `GEOparse-2.0.3/src/GEOparse/logger.py` & `geoparse-2.0.4/src/GEOparse/logger.py`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/src/GEOparse/sra_downloader.py` & `geoparse-2.0.4/src/GEOparse/sra_downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """A module that helps to deal with SRA files."""
 
 import glob
+from io import StringIO
 import json
 import os
 import platform
 import re
 import subprocess as sp
 
-from pandas import DataFrame, concat
+from pandas import DataFrame, concat, read_xml
 from six import iteritems
 
 from . import utils
 from .logger import geoparse_logger as logger
 
 
 class NoSRARelationException(Exception):
@@ -155,23 +156,18 @@
                 # retrieve IDs for given SRX
                 answer = utils.esearch(db="sra", term=query, email=self.email)
                 ids = answer["esearchresult"]["idlist"]
                 if len(ids) != 1:
                     raise ValueError("There should be one and only one ID per SRX")
 
                 results = utils.efetch(
-                    db="sra", id=ids[0], rettype="runinfo", email=self.email
+                    db="sra", id=ids[0], rettype="runinfo", retmode="xml", email=self.email
                 )
                 try:
-                    df_tmp = DataFrame(
-                        [i.split(",") for i in results.split("\n") if i != ""][1:],
-                        columns=[i.split(",") for i in results.split("\n") if i != ""][
-                            0
-                        ],
-                    )
+                    df_tmp = read_xml(StringIO(results))
                 except IndexError:
                     logger.error(
                         (
                             "SRA is empty (ID: %s, query: %s). "
                             "Check if it is publicly available."
                         )
                         % (ids[0], query)
```

### Comparing `GEOparse-2.0.3/src/GEOparse/utils.py` & `geoparse-2.0.4/src/GEOparse/utils.py`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/src/GEOparse.egg-info/SOURCES.txt` & `geoparse-2.0.4/src/GEOparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/Analyse_hsa-miR-124a-3p_transfection_time-course.ipynb` & `geoparse-2.0.4/tests/Analyse_hsa-miR-124a-3p_transfection_time-course.ipynb`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/GPL20814_family.soft` & `geoparse-2.0.4/tests/GPL20814_family.soft`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/GPL4133.txt` & `geoparse-2.0.4/tests/GPL4133.txt`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/GPL4134.txt` & `geoparse-2.0.4/tests/GPL4134.txt`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/GSE105845_family.soft` & `geoparse-2.0.4/tests/GSE105845_family.soft`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/GSM32878.txt` & `geoparse-2.0.4/tests/GSM32878.txt`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/seed-mirza-g_all_mirnas_per_gene_scores_miR_124a.tab` & `geoparse-2.0.4/tests/seed-mirza-g_all_mirnas_per_gene_scores_miR_124a.tab`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/soft_ex_family.txt` & `geoparse-2.0.4/tests/soft_ex_family.txt`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/test_GEOparse.py` & `geoparse-2.0.4/tests/test_GEOparse.py`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/test_gsm_annotated.tab` & `geoparse-2.0.4/tests/test_gsm_annotated.tab`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/test_merged_by_id_and_averaged_by_gb_acc.tab` & `geoparse-2.0.4/tests/test_merged_by_id_and_averaged_by_gb_acc.tab`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/test_sample_pivoted_by_value.tab` & `geoparse-2.0.4/tests/test_sample_pivoted_by_value.tab`

 * *Files identical despite different names*

### Comparing `GEOparse-2.0.3/tests/test_sample_pivoted_by_value_and_annotated_by_gbacc.tab` & `geoparse-2.0.4/tests/test_sample_pivoted_by_value_and_annotated_by_gbacc.tab`

 * *Files identical despite different names*

