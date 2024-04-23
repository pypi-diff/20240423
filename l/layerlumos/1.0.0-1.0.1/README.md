# Comparing `tmp/layerlumos-1.0.0.tar.gz` & `tmp/layerlumos-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layerlumos-1.0.0.tar", last modified: Thu Mar 21 17:25:25 2024, max compression
+gzip compressed data, was "layerlumos-1.0.1.tar", last modified: Tue Apr 23 19:25:55 2024, max compression
```

## Comparing `layerlumos-1.0.0.tar` & `layerlumos-1.0.1.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.601141 layerlumos-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.135151 layerlumos-1.0.0/.github/
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.209134 layerlumos-1.0.0/.github/workflows/
--rw-rw-rw-   0        0        0     1300 2024-03-20 05:00:04.000000 layerlumos-1.0.0/.github/workflows/static.yml
--rw-rw-rw-   0        0        0     3281 2024-03-17 22:48:11.000000 layerlumos-1.0.0/.gitignore
--rw-rw-rw-   0        0        0     1084 2024-03-08 16:32:27.000000 layerlumos-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3156 2024-03-21 17:25:25.597139 layerlumos-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2304 2024-03-10 19:48:41.000000 layerlumos-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.301136 layerlumos-1.0.0/docs/
--rw-rw-rw-   0        0        0      516 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/API_Documentation.md
--rw-rw-rw-   0        0        0      654 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/Makefile
--rw-rw-rw-   0        0        0       15 2024-03-10 20:11:51.000000 layerlumos-1.0.0/docs/_config.yml
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.350140 layerlumos-1.0.0/docs/api/
--rw-rw-rw-   0        0        0     6687 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/api/index.html
--rw-rw-rw-   0        0        0    23696 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/api/layerlumos.html
--rw-rw-rw-   0        0        0    19823 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/api/utils.html
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.373144 layerlumos-1.0.0/docs/assets/
--rw-rw-rw-   0        0        0  1724033 2024-03-08 16:32:27.000000 layerlumos-1.0.0/docs/assets/Icon1.jpg
--rw-rw-rw-   0        0        0  1385382 2024-03-08 16:32:27.000000 layerlumos-1.0.0/docs/assets/Icon2.jpg
--rw-rw-rw-   0        0        0  1181740 2024-03-08 16:32:27.000000 layerlumos-1.0.0/docs/assets/icon3.jpg
--rw-rw-rw-   0        0        0     1230 2024-03-20 03:49:18.000000 layerlumos-1.0.0/docs/conf.py
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.392136 layerlumos-1.0.0/docs/examples/
--rw-rw-rw-   0        0        0        0 2024-03-21 02:39:46.000000 layerlumos-1.0.0/docs/examples/Lumerical_RF.py
--rw-rw-rw-   0        0        0     4737 2024-03-21 02:39:56.000000 layerlumos-1.0.0/docs/examples/RF_example.ipynb
--rw-rw-rw-   0        0        0    53617 2024-03-21 02:39:56.000000 layerlumos-1.0.0/docs/examples/angle_example.ipynb
--rw-rw-rw-   0        0        0     1800 2024-03-21 02:39:46.000000 layerlumos-1.0.0/docs/examples/compare_res_lumerical.py
--rw-rw-rw-   0        0        0    71036 2024-03-21 02:39:56.000000 layerlumos-1.0.0/docs/examples/simple_example.ipynb
--rw-rw-rw-   0        0        0     2616 2024-03-21 02:39:46.000000 layerlumos-1.0.0/docs/examples/time_compare_lumerical.py
--rw-rw-rw-   0        0        0        0 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/examples.md
--rw-rw-rw-   0        0        0      373 2024-03-21 02:39:46.000000 layerlumos-1.0.0/docs/examples.rst
--rw-rw-rw-   0        0        0     2381 2024-03-10 21:07:09.000000 layerlumos-1.0.0/docs/getting-started.md
--rw-rw-rw-   0        0        0     2736 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/index.md
--rw-rw-rw-   0        0        0      642 2024-03-20 04:10:07.000000 layerlumos-1.0.0/docs/index.rst
--rwxrwxrwx   0        0        0      800 2024-03-17 22:48:11.000000 layerlumos-1.0.0/docs/make.bat
--rw-rw-rw-   0        0        0      231 2024-03-20 03:51:50.000000 layerlumos-1.0.0/docs/modules.rst
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.408139 layerlumos-1.0.0/layerlumos/
--rw-rw-rw-   0        0        0        0 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/__init__.py
--rw-rw-rw-   0        0        0     7905 2024-03-20 03:57:49.000000 layerlumos-1.0.0/layerlumos/layerlumos.py
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.578137 layerlumos-1.0.0/layerlumos/materials/
--rw-rw-rw-   0        0        0    10150 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Ag_Yang.csv
--rw-rw-rw-   0        0        0    11498 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Al2O3_Querry.csv
--rw-rw-rw-   0        0        0     5357 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Al_Rakic.csv
--rw-rw-rw-   0        0        0    21926 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Cr_Rakic.csv
--rw-rw-rw-   0        0        0     1428 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Ni_Ordal.csv
--rw-rw-rw-   0        0        0     3552 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Pd_Werner.csv
--rw-rw-rw-   0        0        0    35891 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Si3N4_Kischkat.csv
--rw-rw-rw-   0        0        0    40129 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/SiO2_Kischkat.csv
--rw-rw-rw-   0        0        0    29705 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/TiN_Beliaev.csv
--rw-rw-rw-   0        0        0    44951 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/TiO2_Siefke.csv
--rw-rw-rw-   0        0        0     1300 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/Ti_Ordal.csv
--rw-rw-rw-   0        0        0     1294 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials/W_Ordal.csv
--rw-rw-rw-   0        0        0      483 2024-03-12 17:59:28.000000 layerlumos-1.0.0/layerlumos/materials.json
--rw-rw-rw-   0        0        0     5880 2024-03-17 22:48:11.000000 layerlumos-1.0.0/layerlumos/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.594136 layerlumos-1.0.0/layerlumos.egg-info/
--rw-rw-rw-   0        0        0     3156 2024-03-21 17:25:24.000000 layerlumos-1.0.0/layerlumos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1404 2024-03-21 17:25:25.000000 layerlumos-1.0.0/layerlumos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 17:25:24.000000 layerlumos-1.0.0/layerlumos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-21 17:25:24.000000 layerlumos-1.0.0/layerlumos.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-21 17:25:24.000000 layerlumos-1.0.0/layerlumos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1046 2024-03-21 17:24:01.000000 layerlumos-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       69 2024-03-17 22:48:11.000000 layerlumos-1.0.0/pytest.ini
--rw-rw-rw-   0        0        0       42 2024-03-21 17:25:25.601141 layerlumos-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-21 17:25:25.591151 layerlumos-1.0.0/tests/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:32:27.000000 layerlumos-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1365 2024-03-17 22:48:11.000000 layerlumos-1.0.0/tests/test_RF.py
--rw-rw-rw-   0        0        0     2137 2024-03-17 22:48:11.000000 layerlumos-1.0.0/tests/test_angle.py
--rw-rw-rw-   0        0        0     2112 2024-03-17 22:48:11.000000 layerlumos-1.0.0/tests/test_materials.py
--rw-rw-rw-   0        0        0     1956 2024-03-17 22:48:11.000000 layerlumos-1.0.0/tests/test_stackrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.724394 layerlumos-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.704394 layerlumos-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.708394 layerlumos-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-23 19:25:44.000000 layerlumos-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-23 19:25:44.000000 layerlumos-1.0.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-23 19:25:44.000000 layerlumos-1.0.1/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-23 19:25:44.000000 layerlumos-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-23 19:25:44.000000 layerlumos-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 19:25:44.000000 layerlumos-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-23 19:25:55.724394 layerlumos-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-23 19:25:44.000000 layerlumos-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.708394 layerlumos-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.708394 layerlumos-1.0.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/api/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23347 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/api/layerlumos.html
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/api/utils.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.716394 layerlumos-1.0.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)  1724033 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/assets/Icon1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1385382 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/assets/Icon2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)  1181740 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/assets/icon3.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.716394 layerlumos-1.0.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/examples/Lumerical_RF.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/examples/RF_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/examples/angle_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/examples/compare_res_lumerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139190 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/examples/simple_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/examples/time_compare_lumerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/home.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 19:25:44.000000 layerlumos-1.0.1/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.716394 layerlumos-1.0.1/layerlumos/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/layerlumos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.720394 layerlumos-1.0.1/layerlumos/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Ag_Yang.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Al2O3_Querry.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5150 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Al_Rakic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20925 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Cr_Rakic.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Ni_Ordal.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Pd_Werner.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    34439 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Si3N4_Kischkat.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38468 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/SiO2_Kischkat.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28528 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/TiN_Beliaev.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    43086 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/TiO2_Siefke.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/Ti_Ordal.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials/W_Ordal.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/materials.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/utils_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-23 19:25:44.000000 layerlumos-1.0.1/layerlumos/utils_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.724394 layerlumos-1.0.1/layerlumos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-23 19:25:55.000000 layerlumos-1.0.1/layerlumos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-23 19:25:55.000000 layerlumos-1.0.1/layerlumos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:25:55.000000 layerlumos-1.0.1/layerlumos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 19:25:55.000000 layerlumos-1.0.1/layerlumos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 19:25:55.000000 layerlumos-1.0.1/layerlumos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-23 19:25:44.000000 layerlumos-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:25:55.724394 layerlumos-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:25:55.720394 layerlumos-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-23 19:25:44.000000 layerlumos-1.0.1/tests/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 19:25:44.000000 layerlumos-1.0.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-23 19:25:44.000000 layerlumos-1.0.1/tests/test_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-23 19:25:44.000000 layerlumos-1.0.1/tests/test_radio_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-04-23 19:25:44.000000 layerlumos-1.0.1/tests/test_stackrt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-23 19:25:44.000000 layerlumos-1.0.1/tests/test_version.py
```

### Comparing `layerlumos-1.0.0/.github/workflows/static.yml` & `layerlumos-1.0.1/.github/workflows/static.yml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Simple workflow for deploying static content to GitHub Pages
-name: Deploy static content to Pages
-
-on:
-  # Runs on pushes targeting the default branch
-  push:
-    branches: ["main"]
-
-  # Allows you to run this workflow manually from the Actions tab
-  workflow_dispatch:
-
-# Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
-permissions:
-  contents: read
-  pages: write
-  id-token: write
-
-# Allow only one concurrent deployment, skipping runs queued between the run in-progress and latest queued.
-# However, do NOT cancel in-progress runs as we want to allow these production deployments to complete.
-concurrency:
-  group: "pages"
-  cancel-in-progress: false
-
-jobs:
-  # Single deploy job since we're just deploying
-  deploy:
-    environment:
-      name: github-pages
-      url: ${{ steps.deployment.outputs.page_url }}
-    runs-on: ubuntu-latest
-    steps:
-      - name: Checkout
-        uses: actions/checkout@v4
-      - name: Setup Pages
-        uses: actions/configure-pages@v4
-      - name: Upload artifact
-        uses: actions/upload-pages-artifact@v3
-        with:
-          # Upload entire repository
-          path: 'build/html'
-      - name: Deploy to GitHub Pages
-        id: deployment
+# Simple workflow for deploying static content to GitHub Pages
+name: Deploy static content to Pages
+
+on:
+  # Runs on pushes targeting the default branch
+  push:
+    branches: ["main"]
+
+  # Allows you to run this workflow manually from the Actions tab
+  workflow_dispatch:
+
+# Sets permissions of the GITHUB_TOKEN to allow deployment to GitHub Pages
+permissions:
+  contents: read
+  pages: write
+  id-token: write
+
+# Allow only one concurrent deployment, skipping runs queued between the run in-progress and latest queued.
+# However, do NOT cancel in-progress runs as we want to allow these production deployments to complete.
+concurrency:
+  group: "pages"
+  cancel-in-progress: false
+
+jobs:
+  # Single deploy job since we're just deploying
+  deploy:
+    environment:
+      name: github-pages
+      url: ${{ steps.deployment.outputs.page_url }}
+    runs-on: ubuntu-latest
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v4
+      - name: Setup Pages
+        uses: actions/configure-pages@v4
+      - name: Upload artifact
+        uses: actions/upload-pages-artifact@v3
+        with:
+          # Upload entire repository
+          path: 'build/html'
+      - name: Deploy to GitHub Pages
+        id: deployment
         uses: actions/deploy-pages@v4
```

### Comparing `layerlumos-1.0.0/.gitignore` & `layerlumos-1.0.1/.gitignore`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,165 +1,165 @@
-# Byte-compiled / optimized / DLL files
-__pycache__/
-*.py[cod]
-*$py.class
-
-# C extensions
-*.so
-
-# Distribution / packaging
-.Python
-develop-eggs/
-dist/
-downloads/
-eggs/
-.eggs/
-lib/
-lib64/
-parts/
-sdist/
-var/
-wheels/
-share/python-wheels/
-*.egg-info/
-.installed.cfg
-*.egg
-MANIFEST
-
-# PyInstaller
-#  Usually these files are written by a python script from a template
-#  before PyInstaller builds the exe, so as to inject date/other infos into it.
-*.manifest
-*.spec
-
-# Installer logs
-pip-log.txt
-pip-delete-this-directory.txt
-
-# Unit test / coverage reports
-htmlcov/
-.tox/
-.nox/
-.coverage
-.coverage.*
-.cache
-nosetests.xml
-coverage.xml
-*.cover
-*.py,cover
-.hypothesis/
-.pytest_cache/
-cover/
-
-# Translations
-*.mo
-*.pot
-
-# Django stuff:
-*.log
-local_settings.py
-db.sqlite3
-db.sqlite3-journal
-
-# Flask stuff:
-instance/
-.webassets-cache
-
-# Scrapy stuff:
-.scrapy
-
-# Sphinx documentation
-docs/_build/
-
-# PyBuilder
-.pybuilder/
-target/
-
-# Jupyter Notebook
-.ipynb_checkpoints
-
-# IPython
-profile_default/
-ipython_config.py
-
-# pyenv
-#   For a library or package, you might want to ignore these files since the code is
-#   intended to run in multiple environments; otherwise, check them in:
-# .python-version
-
-# pipenv
-#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
-#   However, in case of collaboration, if having platform-specific dependencies or dependencies
-#   having no cross-platform support, pipenv may install dependencies that don't work, or not
-#   install all needed dependencies.
-#Pipfile.lock
-
-# poetry
-#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
-#   This is especially recommended for binary packages to ensure reproducibility, and is more
-#   commonly ignored for libraries.
-#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
-#poetry.lock
-
-# pdm
-#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
-#pdm.lock
-#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
-#   in version control.
-#   https://pdm.fming.dev/#use-with-ide
-.pdm.toml
-
-# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
-__pypackages__/
-
-# Celery stuff
-celerybeat-schedule
-celerybeat.pid
-
-# SageMath parsed files
-*.sage.py
-
-# Environments
-.env
-.venv
-env/
-venv/
-ENV/
-env.bak/
-venv.bak/
-
-# Spyder project settings
-.spyderproject
-.spyproject
-
-# Rope project settings
-.ropeproject
-
-# mkdocs documentation
-/site
-
-# mypy
-.mypy_cache/
-.dmypy.json
-dmypy.json
-
-# Pyre type checker
-.pyre/
-
-# pytype static type analyzer
-.pytype/
-
-# Cython debug symbols
-cython_debug/
-
-# PyCharm
-#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
-#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
-#  and can be added to the global gitignore or merged into this file.  For a more nuclear
-#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-#.idea/
-
-# custom
-.DS_Store
-__MACOSX/
-*.swp
-outputs/
+# Byte-compiled / optimized / DLL files
+__pycache__/
+*.py[cod]
+*$py.class
+
+# C extensions
+*.so
+
+# Distribution / packaging
+.Python
+develop-eggs/
+dist/
+downloads/
+eggs/
+.eggs/
+lib/
+lib64/
+parts/
+sdist/
+var/
+wheels/
+share/python-wheels/
+*.egg-info/
+.installed.cfg
+*.egg
+MANIFEST
+
+# PyInstaller
+#  Usually these files are written by a python script from a template
+#  before PyInstaller builds the exe, so as to inject date/other infos into it.
+*.manifest
+*.spec
+
+# Installer logs
+pip-log.txt
+pip-delete-this-directory.txt
+
+# Unit test / coverage reports
+htmlcov/
+.tox/
+.nox/
+.coverage
+.coverage.*
+.cache
+nosetests.xml
+coverage.xml
+*.cover
+*.py,cover
+.hypothesis/
+.pytest_cache/
+cover/
+
+# Translations
+*.mo
+*.pot
+
+# Django stuff:
+*.log
+local_settings.py
+db.sqlite3
+db.sqlite3-journal
+
+# Flask stuff:
+instance/
+.webassets-cache
+
+# Scrapy stuff:
+.scrapy
+
+# Sphinx documentation
+docs/_build/
+
+# PyBuilder
+.pybuilder/
+target/
+
+# Jupyter Notebook
+.ipynb_checkpoints
+
+# IPython
+profile_default/
+ipython_config.py
+
+# pyenv
+#   For a library or package, you might want to ignore these files since the code is
+#   intended to run in multiple environments; otherwise, check them in:
+# .python-version
+
+# pipenv
+#   According to pypa/pipenv#598, it is recommended to include Pipfile.lock in version control.
+#   However, in case of collaboration, if having platform-specific dependencies or dependencies
+#   having no cross-platform support, pipenv may install dependencies that don't work, or not
+#   install all needed dependencies.
+#Pipfile.lock
+
+# poetry
+#   Similar to Pipfile.lock, it is generally recommended to include poetry.lock in version control.
+#   This is especially recommended for binary packages to ensure reproducibility, and is more
+#   commonly ignored for libraries.
+#   https://python-poetry.org/docs/basic-usage/#commit-your-poetrylock-file-to-version-control
+#poetry.lock
+
+# pdm
+#   Similar to Pipfile.lock, it is generally recommended to include pdm.lock in version control.
+#pdm.lock
+#   pdm stores project-wide configurations in .pdm.toml, but it is recommended to not include it
+#   in version control.
+#   https://pdm.fming.dev/#use-with-ide
+.pdm.toml
+
+# PEP 582; used by e.g. github.com/David-OConnor/pyflow and github.com/pdm-project/pdm
+__pypackages__/
+
+# Celery stuff
+celerybeat-schedule
+celerybeat.pid
+
+# SageMath parsed files
+*.sage.py
+
+# Environments
+.env
+.venv
+env/
+venv/
+ENV/
+env.bak/
+venv.bak/
+
+# Spyder project settings
+.spyderproject
+.spyproject
+
+# Rope project settings
+.ropeproject
+
+# mkdocs documentation
+/site
+
+# mypy
+.mypy_cache/
+.dmypy.json
+dmypy.json
+
+# Pyre type checker
+.pyre/
+
+# pytype static type analyzer
+.pytype/
+
+# Cython debug symbols
+cython_debug/
+
+# PyCharm
+#  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
+#  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
+#  and can be added to the global gitignore or merged into this file.  For a more nuclear
+#  option (not recommended) you can uncomment the following to ignore the entire idea folder.
+#.idea/
+
+# custom
+.DS_Store
+__MACOSX/
+*.swp
+outputs/
```

### Comparing `layerlumos-1.0.0/LICENSE` & `layerlumos-1.0.1/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Mil152
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Mingxuan Li
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `layerlumos-1.0.0/PKG-INFO` & `layerlumos-1.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,74 @@
-Metadata-Version: 2.1
-Name: layerlumos
-Version: 1.0.0
-Summary: An open-source software for TMM optical simulations.
-Author-email: Mingxuan Li <mil152@pitt.edu>
-License: MIT
-Project-URL: Homepage, https://github.com/mil152/layerlumos
-Project-URL: Source, https://github.com/mil152/layerlumos
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: wheel; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# LayerLumos
-![LayerLumos Icon](/docs/assets/icon3.jpg)
-## Overview
-
-**LayerLumos** is an open-source software designed for scientists, engineers, and researchers in optics and photonics. It provides a powerful yet intuitive interface for calculating the reflection and transmission (RT) of light through multi-layer optical structures. By inputting the refractive index, thickness of each layer, and the frequency vector, users can analyze how light interacts with layered materials, including the option to adjust for incidence angles.
-
-Our mission is to offer a lightweight, flexible, and fast alternative to commercial software, enabling users to perform complex optical simulations with ease. LayerLumos is built with performance and usability in mind, facilitating the exploration of optical phenomena in research and development settings.
-
-## Features
-
-- **Lightweight and Efficient**: Optimized for performance, LayerLumos ensures rapid calculations without the overhead of large-scale commercial software.
-- **Flexibility**: Accommodates a wide range of materials and structures by allowing users to specify complex refractive indices, layer thicknesses, and frequency vectors.
-- **Angle of Incidence Support**: Expands simulation capabilities to include angled light incidence, providing more detailed analysis for advanced optical designs.
-- **Open Source and Community-Driven**: Encourages contributions and feedback from the community, ensuring continuous improvement and innovation.
-- **Comprehensive Material Database**: Includes a growing database of materials with their optical properties, streamlining the simulation setup process.
-
-## Getting Started
-
-1. **Installation**: Instructions on how to install LayerLumos on various operating systems.
-2. **Quick Start Guide**: A brief tutorial on how to perform your first RT calculation using LayerLumos.
-3. **Examples**: Explore a collection of examples illustrating various use cases and capabilities of LayerLumos.
-
-## License
-
-LayerLumos is released under the [MIT License](https://github.com/Mil152/LayerLumos/blob/main/LICENSE), promoting open and unrestricted access to software for academic and commercial use.
-
-## Acknowledgments
-
-- Thanks to all contributors and users for your support and feedback.
+Metadata-Version: 2.1
+Name: layerlumos
+Version: 1.0.1
+Summary: An open-source software for TMM optical simulations
+Author-email: Mingxuan Li <mil152@pitt.edu>
+License: MIT
+Project-URL: Homepage, https://github.com/mil152/layerlumos
+Project-URL: Source, https://github.com/mil152/layerlumos
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+
+# LayerLumos
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/mil152/LayerLumos/main/docs/assets/icon3.jpg" width="400" />
+</p>
+
+## Overview
+
+**LayerLumos** is an open-source software designed for scientists, engineers, and researchers in optics and photonics. It provides a powerful yet intuitive interface for calculating the reflection and transmission (RT) of light through multi-layer optical structures. By inputting the refractive index, thickness of each layer, and the frequency vector, users can analyze how light interacts with layered materials, including the option to adjust for incidence angles.
+
+Our mission is to offer a lightweight, flexible, and fast alternative to commercial software, enabling users to perform complex optical simulations with ease. LayerLumos is built with performance and usability in mind, facilitating the exploration of optical phenomena in research and development settings.
+
+For details, check out our [Documentation](https://mil152.github.io/LayerLumos/index.html).
+
+## Features
+
+- **Lightweight and Efficient**: Optimized for performance, LayerLumos ensures rapid calculations without the overhead of large-scale commercial software.
+- **Flexibility**: Accommodates a wide range of materials and structures by allowing users to specify complex refractive indices, layer thicknesses, and frequency vectors.
+- **Angle of Incidence Support**: Expands simulation capabilities to include angled light incidence, providing more detailed analysis for advanced optical designs.
+- **Open Source and Community-Driven**: Encourages contributions and feedback from the community, ensuring continuous improvement and innovation.
+- **Comprehensive Material Database**: Includes a growing database of materials with their optical properties, streamlining the simulation setup process.
+
+## Getting Started
+
+### Installation
+
+LayerLumos can be easily installed via pip:
+
+```bash
+pip install layerlumos
+```
+
+For more detailed installation instructions, please refer to our [Installation Guide](https://github.com/Mil152/LayerLumos/docs/installation.md).
+
+### Quick Start Guide
+
+To get started with your first RT calculation, check out our [Quick Start Guide](https://github.com/Mil152/LayerLumos/docs/quickstart.md).
+
+### Examples
+
+Explore a collection of examples illustrating various use cases and capabilities of LayerLumos in the [Examples Directory](https://mil152.github.io/LayerLumos/examples.html#jupyter-notebook-examples).
+
+## License
+
+LayerLumos is released under the [MIT License](LICENSE), promoting open and unrestricted access to software for academic and commercial use.
+
+## Acknowledgments
+
+- Thanks to all contributors and users for your support and feedback.
```

### Comparing `layerlumos-1.0.0/README.md` & `layerlumos-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,49 @@
-# LayerLumos
-![LayerLumos Icon](/docs/assets/icon3.jpg)
-## Overview
-
-**LayerLumos** is an open-source software designed for scientists, engineers, and researchers in optics and photonics. It provides a powerful yet intuitive interface for calculating the reflection and transmission (RT) of light through multi-layer optical structures. By inputting the refractive index, thickness of each layer, and the frequency vector, users can analyze how light interacts with layered materials, including the option to adjust for incidence angles.
-
-Our mission is to offer a lightweight, flexible, and fast alternative to commercial software, enabling users to perform complex optical simulations with ease. LayerLumos is built with performance and usability in mind, facilitating the exploration of optical phenomena in research and development settings.
-
-## Features
-
-- **Lightweight and Efficient**: Optimized for performance, LayerLumos ensures rapid calculations without the overhead of large-scale commercial software.
-- **Flexibility**: Accommodates a wide range of materials and structures by allowing users to specify complex refractive indices, layer thicknesses, and frequency vectors.
-- **Angle of Incidence Support**: Expands simulation capabilities to include angled light incidence, providing more detailed analysis for advanced optical designs.
-- **Open Source and Community-Driven**: Encourages contributions and feedback from the community, ensuring continuous improvement and innovation.
-- **Comprehensive Material Database**: Includes a growing database of materials with their optical properties, streamlining the simulation setup process.
-
-## Getting Started
-
-1. **Installation**: Instructions on how to install LayerLumos on various operating systems.
-2. **Quick Start Guide**: A brief tutorial on how to perform your first RT calculation using LayerLumos.
-3. **Examples**: Explore a collection of examples illustrating various use cases and capabilities of LayerLumos.
-
-## License
-
-LayerLumos is released under the [MIT License](https://github.com/Mil152/LayerLumos/blob/main/LICENSE), promoting open and unrestricted access to software for academic and commercial use.
-
-## Acknowledgments
-
-- Thanks to all contributors and users for your support and feedback.
+# LayerLumos
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/mil152/LayerLumos/main/docs/assets/icon3.jpg" width="400" />
+</p>
+
+## Overview
+
+**LayerLumos** is an open-source software designed for scientists, engineers, and researchers in optics and photonics. It provides a powerful yet intuitive interface for calculating the reflection and transmission (RT) of light through multi-layer optical structures. By inputting the refractive index, thickness of each layer, and the frequency vector, users can analyze how light interacts with layered materials, including the option to adjust for incidence angles.
+
+Our mission is to offer a lightweight, flexible, and fast alternative to commercial software, enabling users to perform complex optical simulations with ease. LayerLumos is built with performance and usability in mind, facilitating the exploration of optical phenomena in research and development settings.
+
+For details, check out our [Documentation](https://mil152.github.io/LayerLumos/index.html).
+
+## Features
+
+- **Lightweight and Efficient**: Optimized for performance, LayerLumos ensures rapid calculations without the overhead of large-scale commercial software.
+- **Flexibility**: Accommodates a wide range of materials and structures by allowing users to specify complex refractive indices, layer thicknesses, and frequency vectors.
+- **Angle of Incidence Support**: Expands simulation capabilities to include angled light incidence, providing more detailed analysis for advanced optical designs.
+- **Open Source and Community-Driven**: Encourages contributions and feedback from the community, ensuring continuous improvement and innovation.
+- **Comprehensive Material Database**: Includes a growing database of materials with their optical properties, streamlining the simulation setup process.
+
+## Getting Started
+
+### Installation
+
+LayerLumos can be easily installed via pip:
+
+```bash
+pip install layerlumos
+```
+
+For more detailed installation instructions, please refer to our [Installation Guide](https://github.com/Mil152/LayerLumos/docs/installation.md).
+
+### Quick Start Guide
+
+To get started with your first RT calculation, check out our [Quick Start Guide](https://github.com/Mil152/LayerLumos/docs/quickstart.md).
+
+### Examples
+
+Explore a collection of examples illustrating various use cases and capabilities of LayerLumos in the [Examples Directory](https://mil152.github.io/LayerLumos/examples.html#jupyter-notebook-examples).
+
+## License
+
+LayerLumos is released under the [MIT License](LICENSE), promoting open and unrestricted access to software for academic and commercial use.
+
+## Acknowledgments
+
+- Thanks to all contributors and users for your support and feedback.
```

### Comparing `layerlumos-1.0.0/docs/Makefile` & `layerlumos-1.0.1/docs/Makefile`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Minimal makefile for Sphinx documentation
-#
-
-# You can set these variables from the command line, and also
-# from the environment for the first two.
-SPHINXOPTS    ?=
-SPHINXBUILD   ?= sphinx-build
-SOURCEDIR     = .
-BUILDDIR      = _build
-
-# Put it first so that "make" without argument is like "make help".
-help:
-	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
-
-.PHONY: help Makefile
-
-# Catch-all target: route all unknown targets to Sphinx using the new
-# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
-%: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+# Minimal makefile for Sphinx documentation
+#
+
+# You can set these variables from the command line, and also
+# from the environment for the first two.
+SPHINXOPTS    ?=
+SPHINXBUILD   ?= sphinx-build
+SOURCEDIR     = .
+BUILDDIR      = _build
+
+# Put it first so that "make" without argument is like "make help".
+help:
+	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+
+.PHONY: help Makefile
+
+# Catch-all target: route all unknown targets to Sphinx using the new
+# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
+%: Makefile
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `layerlumos-1.0.0/docs/api/index.html` & `layerlumos-1.0.1/docs/api/index.html`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-<!doctype html>
-<html lang="en">
-<head>
-<meta charset="utf-8">
-<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
-<meta name="generator" content="pdoc 0.10.0" />
-<title>layerlumos API documentation</title>
-<meta name="description" content="" />
-<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
-<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
-<link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
-<style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
-<style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
-<style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
-<script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
-<script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
-</head>
-<body>
-<main>
-<article id="content">
-<header>
-<h1 class="title">Package <code>layerlumos</code></h1>
-</header>
-<section id="section-intro">
-</section>
-<section>
-<h2 class="section-title" id="header-submodules">Sub-modules</h2>
-<dl>
-<dt><code class="name"><a title="layerlumos.layerlumos" href="layerlumos.html">layerlumos.layerlumos</a></code></dt>
-<dd>
-<div class="desc"></div>
-</dd>
-<dt><code class="name"><a title="layerlumos.utils" href="utils.html">layerlumos.utils</a></code></dt>
-<dd>
-<div class="desc"></div>
-</dd>
-</dl>
-</section>
-<section>
-</section>
-<section>
-</section>
-<section>
-</section>
-</article>
-<nav id="sidebar">
-<h1>Index</h1>
-<div class="toc">
-<ul></ul>
-</div>
-<ul id="index">
-<li><h3><a href="#header-submodules">Sub-modules</a></h3>
-<ul>
-<li><code><a title="layerlumos.layerlumos" href="layerlumos.html">layerlumos.layerlumos</a></code></li>
-<li><code><a title="layerlumos.utils" href="utils.html">layerlumos.utils</a></code></li>
-</ul>
-</li>
-</ul>
-</nav>
-</main>
-<footer id="footer">
-<p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
-</footer>
-</body>
+<!doctype html>
+<html lang="en">
+<head>
+<meta charset="utf-8">
+<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
+<meta name="generator" content="pdoc 0.10.0" />
+<title>layerlumos API documentation</title>
+<meta name="description" content="" />
+<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
+<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
+<link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
+<style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
+<style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
+<style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
+<script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
+<script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
+</head>
+<body>
+<main>
+<article id="content">
+<header>
+<h1 class="title">Package <code>layerlumos</code></h1>
+</header>
+<section id="section-intro">
+</section>
+<section>
+<h2 class="section-title" id="header-submodules">Sub-modules</h2>
+<dl>
+<dt><code class="name"><a title="layerlumos.layerlumos" href="layerlumos.html">layerlumos.layerlumos</a></code></dt>
+<dd>
+<div class="desc"></div>
+</dd>
+<dt><code class="name"><a title="layerlumos.utils" href="utils.html">layerlumos.utils</a></code></dt>
+<dd>
+<div class="desc"></div>
+</dd>
+</dl>
+</section>
+<section>
+</section>
+<section>
+</section>
+<section>
+</section>
+</article>
+<nav id="sidebar">
+<h1>Index</h1>
+<div class="toc">
+<ul></ul>
+</div>
+<ul id="index">
+<li><h3><a href="#header-submodules">Sub-modules</a></h3>
+<ul>
+<li><code><a title="layerlumos.layerlumos" href="layerlumos.html">layerlumos.layerlumos</a></code></li>
+<li><code><a title="layerlumos.utils" href="utils.html">layerlumos.utils</a></code></li>
+</ul>
+</li>
+</ul>
+</nav>
+</main>
+<footer id="footer">
+<p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
+</footer>
+</body>
 </html>
```

### Comparing `layerlumos-1.0.0/docs/api/layerlumos.html` & `layerlumos-1.0.1/docs/api/layerlumos.html`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,350 +1,350 @@
-<!doctype html>
-<html lang="en">
-<head>
-<meta charset="utf-8">
-<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
-<meta name="generator" content="pdoc 0.10.0" />
-<title>layerlumos.layerlumos API documentation</title>
-<meta name="description" content="" />
-<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
-<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
-<link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
-<style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
-<style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
-<style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
-<script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
-<script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
-</head>
-<body>
-<main>
-<article id="content">
-<header>
-<h1 class="title">Module <code>layerlumos.layerlumos</code></h1>
-</header>
-<section id="section-intro">
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">import numpy as np
-from scipy.constants import c
-from .utils import load_material, interpolate_material
-import numpy as np
-
-def stackrt(n, d, f, theta=np.array([0])):
-    &#34;&#34;&#34;
-    Calculates the reflection and transmission coefficients for a multilayer stack
-    at different frequencies and incidence angles.
-
-    Parameters:
-    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
-                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
-                         frequencies and Nlayers is the number of layers.
-    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
-    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
-                         Shape should be (Nfreq,).
-    - theta (float or numpy.ndarray): The incidence angle(s) in degrees. Can be a single value or an array of angles.
-
-    Returns:
-    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
-    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
-    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
-    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
-    &#34;&#34;&#34;
-    c = 3e8  # Speed of light in vacuum
-    wvl = c / f  # Convert frequency to wavelength
-    theta_radians = np.radians(theta)  # Convert incidence angle to radians
-
-    # Initialize arrays for both amplitude and intensity coefficients
-    r_TE, r_TM, t_TE, t_TM = np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128)
-    R_TE, T_TE, R_TM, T_TM = np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians)))
-
-    for i, lambda_i in enumerate(wvl):
-        for angle_idx, theta_i in enumerate(theta_radians):
-            M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
-            # Snell&#39;s law to calculate angle in each layer
-            sin_theta_i = np.sin(theta_i)
-            n_0 = n[i, 0]
-            sin_theta_layers = n_0 * sin_theta_i / n[i, :]
-            cos_theta_layers = np.sqrt(1 - sin_theta_layers**2)
-            
-            for j in range(len(d) - 1):
-                n_j, n_next = n[i, j], n[i, j+1]
-                d_j = d[j+1]
-                cos_theta_j, cos_theta_next = cos_theta_layers[j], cos_theta_layers[j+1]
-
-                # Interface calculations for TE and TM polarization with angle consideration
-                r_jk_TE = (n_j * cos_theta_j - n_next * cos_theta_next) / (n_j * cos_theta_j + n_next * cos_theta_next)
-                t_jk_TE = 2 * n_j * cos_theta_j / (n_j * cos_theta_j + n_next * cos_theta_next)
-                r_jk_TM = (n_next * cos_theta_j - n_j * cos_theta_next) / (n_next * cos_theta_j + n_j * cos_theta_next)
-                t_jk_TM = 2 * n_j * cos_theta_j / (n_next * cos_theta_j + n_j * cos_theta_next)
-                
-                M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
-                M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
-                
-                # Adjusting phase change calculation for angle
-                delta = 2 * np.pi * n_next * d_j * cos_theta_j / lambda_i
-                P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
-                
-                M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
-                M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
-
-            r_TE[i, angle_idx], t_TE[i, angle_idx] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
-            r_TM[i, angle_idx], t_TM[i, angle_idx] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
-            R_TE[i, angle_idx], T_TE[i, angle_idx] = np.abs(r_TE[i, angle_idx])**2, np.abs(t_TE[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
-            R_TM[i, angle_idx], T_TM[i, angle_idx] = np.abs(r_TM[i, angle_idx])**2, np.abs(t_TM[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
-    return R_TE, T_TE, R_TM, T_TM
-
-def stackrt0(n, d, f):
-    &#34;&#34;&#34;
-    Calculates the reflection and transmission coefficients for a multilayer stack
-    at different frequencies under normal incidence.
-
-    Parameters:
-    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
-                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
-                         frequencies and Nlayers is the number of layers.
-    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
-    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
-                         Shape should be (Nfreq,).
-
-    Returns:
-    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
-    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
-    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
-    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
-    &#34;&#34;&#34;
-    wvl = c / f  # Convert frequency to wavelength
-    # Initialize arrays for both amplitude and intensity coefficients
-    r_TE, r_TM, t_TE, t_TM = np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128)
-    R_TE, T_TE, R_TM, T_TM = np.zeros_like(f), np.zeros_like(f), np.zeros_like(f), np.zeros_like(f)
-
-    for i, freq in enumerate(f):  # Iterate over each frequency
-        lambda_i = wvl[i]
-        M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
-        for j in range(0, len(n[i, :]) - 1):
-            n_j = n[i, j]
-            n_next = n[i, j+1]
-            d_next = d[j+1]
-
-            # Interface calculations for TE and TM polarization
-            r_jk_TE = (n_j - n_next) / (n_j + n_next)
-            t_jk_TE = 2 * n_j / (n_j + n_next)
-            M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
-            r_jk_TM = (n_next - n_j) / (n_next + n_j)
-            t_jk_TM = 2 * n_j / (n_next + n_j)
-            M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
-            
-            delta = 2 * np.pi * n_next * d_next / lambda_i
-            P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
-            M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
-            M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
-
-        r_TE[i], t_TE[i] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
-        r_TM[i], t_TM[i] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
-        R_TE[i], T_TE[i] = np.abs(r_TE[i])**2, np.abs(t_TE[i])**2 * np.real(n[i, -1] / n[i, 0])
-        R_TM[i], T_TM[i] = np.abs(r_TM[i])**2, np.abs(t_TM[i])**2 * np.real(n[i, -1] / n[i, 0])
-
-    return R_TE, T_TE, R_TM, T_TM</code></pre>
-</details>
-</section>
-<section>
-</section>
-<section>
-</section>
-<section>
-<h2 class="section-title" id="header-functions">Functions</h2>
-<dl>
-<dt id="layerlumos.layerlumos.stackrt"><code class="name flex">
-<span>def <span class="ident">stackrt</span></span>(<span>n, d, f, theta=array([0]))</span>
-</code></dt>
-<dd>
-<div class="desc"><p>Calculates the reflection and transmission coefficients for a multilayer stack
-at different frequencies and incidence angles.</p>
-<p>Parameters:
-- n (numpy.ndarray): The refractive indices of the layers for each frequency.
-Shape should be (Nfreq, Nlayers), where Nfreq is the number of
-frequencies and Nlayers is the number of layers.
-- d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
-- f (numpy.ndarray): The frequencies at which to calculate the coefficients.
-Shape should be (Nfreq,).
-- theta (float or numpy.ndarray): The incidence angle(s) in degrees. Can be a single value or an array of angles.</p>
-<p>Returns:
-- R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
-- T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
-- R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
-- T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def stackrt(n, d, f, theta=np.array([0])):
-    &#34;&#34;&#34;
-    Calculates the reflection and transmission coefficients for a multilayer stack
-    at different frequencies and incidence angles.
-
-    Parameters:
-    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
-                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
-                         frequencies and Nlayers is the number of layers.
-    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
-    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
-                         Shape should be (Nfreq,).
-    - theta (float or numpy.ndarray): The incidence angle(s) in degrees. Can be a single value or an array of angles.
-
-    Returns:
-    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
-    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
-    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
-    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
-    &#34;&#34;&#34;
-    c = 3e8  # Speed of light in vacuum
-    wvl = c / f  # Convert frequency to wavelength
-    theta_radians = np.radians(theta)  # Convert incidence angle to radians
-
-    # Initialize arrays for both amplitude and intensity coefficients
-    r_TE, r_TM, t_TE, t_TM = np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128)
-    R_TE, T_TE, R_TM, T_TM = np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians)))
-
-    for i, lambda_i in enumerate(wvl):
-        for angle_idx, theta_i in enumerate(theta_radians):
-            M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
-            # Snell&#39;s law to calculate angle in each layer
-            sin_theta_i = np.sin(theta_i)
-            n_0 = n[i, 0]
-            sin_theta_layers = n_0 * sin_theta_i / n[i, :]
-            cos_theta_layers = np.sqrt(1 - sin_theta_layers**2)
-            
-            for j in range(len(d) - 1):
-                n_j, n_next = n[i, j], n[i, j+1]
-                d_j = d[j+1]
-                cos_theta_j, cos_theta_next = cos_theta_layers[j], cos_theta_layers[j+1]
-
-                # Interface calculations for TE and TM polarization with angle consideration
-                r_jk_TE = (n_j * cos_theta_j - n_next * cos_theta_next) / (n_j * cos_theta_j + n_next * cos_theta_next)
-                t_jk_TE = 2 * n_j * cos_theta_j / (n_j * cos_theta_j + n_next * cos_theta_next)
-                r_jk_TM = (n_next * cos_theta_j - n_j * cos_theta_next) / (n_next * cos_theta_j + n_j * cos_theta_next)
-                t_jk_TM = 2 * n_j * cos_theta_j / (n_next * cos_theta_j + n_j * cos_theta_next)
-                
-                M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
-                M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
-                
-                # Adjusting phase change calculation for angle
-                delta = 2 * np.pi * n_next * d_j * cos_theta_j / lambda_i
-                P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
-                
-                M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
-                M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
-
-            r_TE[i, angle_idx], t_TE[i, angle_idx] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
-            r_TM[i, angle_idx], t_TM[i, angle_idx] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
-            R_TE[i, angle_idx], T_TE[i, angle_idx] = np.abs(r_TE[i, angle_idx])**2, np.abs(t_TE[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
-            R_TM[i, angle_idx], T_TM[i, angle_idx] = np.abs(r_TM[i, angle_idx])**2, np.abs(t_TM[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
-    return R_TE, T_TE, R_TM, T_TM</code></pre>
-</details>
-</dd>
-<dt id="layerlumos.layerlumos.stackrt0"><code class="name flex">
-<span>def <span class="ident">stackrt0</span></span>(<span>n, d, f)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>Calculates the reflection and transmission coefficients for a multilayer stack
-at different frequencies under normal incidence.</p>
-<p>Parameters:
-- n (numpy.ndarray): The refractive indices of the layers for each frequency.
-Shape should be (Nfreq, Nlayers), where Nfreq is the number of
-frequencies and Nlayers is the number of layers.
-- d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
-- f (numpy.ndarray): The frequencies at which to calculate the coefficients.
-Shape should be (Nfreq,).</p>
-<p>Returns:
-- R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
-- T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
-- R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
-- T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def stackrt0(n, d, f):
-    &#34;&#34;&#34;
-    Calculates the reflection and transmission coefficients for a multilayer stack
-    at different frequencies under normal incidence.
-
-    Parameters:
-    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
-                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
-                         frequencies and Nlayers is the number of layers.
-    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
-    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
-                         Shape should be (Nfreq,).
-
-    Returns:
-    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
-    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
-    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
-    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
-    &#34;&#34;&#34;
-    wvl = c / f  # Convert frequency to wavelength
-    # Initialize arrays for both amplitude and intensity coefficients
-    r_TE, r_TM, t_TE, t_TM = np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128)
-    R_TE, T_TE, R_TM, T_TM = np.zeros_like(f), np.zeros_like(f), np.zeros_like(f), np.zeros_like(f)
-
-    for i, freq in enumerate(f):  # Iterate over each frequency
-        lambda_i = wvl[i]
-        M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
-        for j in range(0, len(n[i, :]) - 1):
-            n_j = n[i, j]
-            n_next = n[i, j+1]
-            d_next = d[j+1]
-
-            # Interface calculations for TE and TM polarization
-            r_jk_TE = (n_j - n_next) / (n_j + n_next)
-            t_jk_TE = 2 * n_j / (n_j + n_next)
-            M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
-            r_jk_TM = (n_next - n_j) / (n_next + n_j)
-            t_jk_TM = 2 * n_j / (n_next + n_j)
-            M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
-            
-            delta = 2 * np.pi * n_next * d_next / lambda_i
-            P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
-            M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
-            M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
-
-        r_TE[i], t_TE[i] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
-        r_TM[i], t_TM[i] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
-        R_TE[i], T_TE[i] = np.abs(r_TE[i])**2, np.abs(t_TE[i])**2 * np.real(n[i, -1] / n[i, 0])
-        R_TM[i], T_TM[i] = np.abs(r_TM[i])**2, np.abs(t_TM[i])**2 * np.real(n[i, -1] / n[i, 0])
-
-    return R_TE, T_TE, R_TM, T_TM</code></pre>
-</details>
-</dd>
-</dl>
-</section>
-<section>
-</section>
-</article>
-<nav id="sidebar">
-<h1>Index</h1>
-<div class="toc">
-<ul></ul>
-</div>
-<ul id="index">
-<li><h3>Super-module</h3>
-<ul>
-<li><code><a title="layerlumos" href="index.html">layerlumos</a></code></li>
-</ul>
-</li>
-<li><h3><a href="#header-functions">Functions</a></h3>
-<ul class="">
-<li><code><a title="layerlumos.layerlumos.stackrt" href="#layerlumos.layerlumos.stackrt">stackrt</a></code></li>
-<li><code><a title="layerlumos.layerlumos.stackrt0" href="#layerlumos.layerlumos.stackrt0">stackrt0</a></code></li>
-</ul>
-</li>
-</ul>
-</nav>
-</main>
-<footer id="footer">
-<p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
-</footer>
-</body>
+<!doctype html>
+<html lang="en">
+<head>
+<meta charset="utf-8">
+<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
+<meta name="generator" content="pdoc 0.10.0" />
+<title>layerlumos.layerlumos API documentation</title>
+<meta name="description" content="" />
+<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
+<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
+<link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
+<style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
+<style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
+<style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
+<script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
+<script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
+</head>
+<body>
+<main>
+<article id="content">
+<header>
+<h1 class="title">Module <code>layerlumos.layerlumos</code></h1>
+</header>
+<section id="section-intro">
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">import numpy as np
+from scipy.constants import c
+from .utils import load_material, interpolate_material
+import numpy as np
+
+def stackrt(n, d, f, theta=np.array([0])):
+    &#34;&#34;&#34;
+    Calculates the reflection and transmission coefficients for a multilayer stack
+    at different frequencies and incidence angles.
+
+    Parameters:
+    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
+                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
+                         frequencies and Nlayers is the number of layers.
+    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
+    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
+                         Shape should be (Nfreq,).
+    - theta (float or numpy.ndarray): The incidence angle(s) in degrees. Can be a single value or an array of angles.
+
+    Returns:
+    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
+    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
+    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
+    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
+    &#34;&#34;&#34;
+    c = 3e8  # Speed of light in vacuum
+    wvl = c / f  # Convert frequency to wavelength
+    theta_radians = np.radians(theta)  # Convert incidence angle to radians
+
+    # Initialize arrays for both amplitude and intensity coefficients
+    r_TE, r_TM, t_TE, t_TM = np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128)
+    R_TE, T_TE, R_TM, T_TM = np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians)))
+
+    for i, lambda_i in enumerate(wvl):
+        for angle_idx, theta_i in enumerate(theta_radians):
+            M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
+            # Snell&#39;s law to calculate angle in each layer
+            sin_theta_i = np.sin(theta_i)
+            n_0 = n[i, 0]
+            sin_theta_layers = n_0 * sin_theta_i / n[i, :]
+            cos_theta_layers = np.sqrt(1 - sin_theta_layers**2)
+            
+            for j in range(len(d) - 1):
+                n_j, n_next = n[i, j], n[i, j+1]
+                d_j = d[j+1]
+                cos_theta_j, cos_theta_next = cos_theta_layers[j], cos_theta_layers[j+1]
+
+                # Interface calculations for TE and TM polarization with angle consideration
+                r_jk_TE = (n_j * cos_theta_j - n_next * cos_theta_next) / (n_j * cos_theta_j + n_next * cos_theta_next)
+                t_jk_TE = 2 * n_j * cos_theta_j / (n_j * cos_theta_j + n_next * cos_theta_next)
+                r_jk_TM = (n_next * cos_theta_j - n_j * cos_theta_next) / (n_next * cos_theta_j + n_j * cos_theta_next)
+                t_jk_TM = 2 * n_j * cos_theta_j / (n_next * cos_theta_j + n_j * cos_theta_next)
+                
+                M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
+                M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
+                
+                # Adjusting phase change calculation for angle
+                delta = 2 * np.pi * n_next * d_j * cos_theta_j / lambda_i
+                P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
+                
+                M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
+                M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
+
+            r_TE[i, angle_idx], t_TE[i, angle_idx] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
+            r_TM[i, angle_idx], t_TM[i, angle_idx] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
+            R_TE[i, angle_idx], T_TE[i, angle_idx] = np.abs(r_TE[i, angle_idx])**2, np.abs(t_TE[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
+            R_TM[i, angle_idx], T_TM[i, angle_idx] = np.abs(r_TM[i, angle_idx])**2, np.abs(t_TM[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
+    return R_TE, T_TE, R_TM, T_TM
+
+def stackrt0(n, d, f):
+    &#34;&#34;&#34;
+    Calculates the reflection and transmission coefficients for a multilayer stack
+    at different frequencies under normal incidence.
+
+    Parameters:
+    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
+                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
+                         frequencies and Nlayers is the number of layers.
+    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
+    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
+                         Shape should be (Nfreq,).
+
+    Returns:
+    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
+    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
+    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
+    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
+    &#34;&#34;&#34;
+    wvl = c / f  # Convert frequency to wavelength
+    # Initialize arrays for both amplitude and intensity coefficients
+    r_TE, r_TM, t_TE, t_TM = np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128)
+    R_TE, T_TE, R_TM, T_TM = np.zeros_like(f), np.zeros_like(f), np.zeros_like(f), np.zeros_like(f)
+
+    for i, freq in enumerate(f):  # Iterate over each frequency
+        lambda_i = wvl[i]
+        M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
+        for j in range(0, len(n[i, :]) - 1):
+            n_j = n[i, j]
+            n_next = n[i, j+1]
+            d_next = d[j+1]
+
+            # Interface calculations for TE and TM polarization
+            r_jk_TE = (n_j - n_next) / (n_j + n_next)
+            t_jk_TE = 2 * n_j / (n_j + n_next)
+            M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
+            r_jk_TM = (n_next - n_j) / (n_next + n_j)
+            t_jk_TM = 2 * n_j / (n_next + n_j)
+            M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
+            
+            delta = 2 * np.pi * n_next * d_next / lambda_i
+            P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
+            M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
+            M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
+
+        r_TE[i], t_TE[i] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
+        r_TM[i], t_TM[i] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
+        R_TE[i], T_TE[i] = np.abs(r_TE[i])**2, np.abs(t_TE[i])**2 * np.real(n[i, -1] / n[i, 0])
+        R_TM[i], T_TM[i] = np.abs(r_TM[i])**2, np.abs(t_TM[i])**2 * np.real(n[i, -1] / n[i, 0])
+
+    return R_TE, T_TE, R_TM, T_TM</code></pre>
+</details>
+</section>
+<section>
+</section>
+<section>
+</section>
+<section>
+<h2 class="section-title" id="header-functions">Functions</h2>
+<dl>
+<dt id="layerlumos.layerlumos.stackrt"><code class="name flex">
+<span>def <span class="ident">stackrt</span></span>(<span>n, d, f, theta=array([0]))</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Calculates the reflection and transmission coefficients for a multilayer stack
+at different frequencies and incidence angles.</p>
+<p>Parameters:
+- n (numpy.ndarray): The refractive indices of the layers for each frequency.
+Shape should be (Nfreq, Nlayers), where Nfreq is the number of
+frequencies and Nlayers is the number of layers.
+- d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
+- f (numpy.ndarray): The frequencies at which to calculate the coefficients.
+Shape should be (Nfreq,).
+- theta (float or numpy.ndarray): The incidence angle(s) in degrees. Can be a single value or an array of angles.</p>
+<p>Returns:
+- R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
+- T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
+- R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
+- T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def stackrt(n, d, f, theta=np.array([0])):
+    &#34;&#34;&#34;
+    Calculates the reflection and transmission coefficients for a multilayer stack
+    at different frequencies and incidence angles.
+
+    Parameters:
+    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
+                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
+                         frequencies and Nlayers is the number of layers.
+    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
+    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
+                         Shape should be (Nfreq,).
+    - theta (float or numpy.ndarray): The incidence angle(s) in degrees. Can be a single value or an array of angles.
+
+    Returns:
+    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
+    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
+    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
+    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
+    &#34;&#34;&#34;
+    c = 3e8  # Speed of light in vacuum
+    wvl = c / f  # Convert frequency to wavelength
+    theta_radians = np.radians(theta)  # Convert incidence angle to radians
+
+    # Initialize arrays for both amplitude and intensity coefficients
+    r_TE, r_TM, t_TE, t_TM = np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128), np.zeros((len(f), len(theta_radians)), dtype=np.complex128)
+    R_TE, T_TE, R_TM, T_TM = np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians))), np.zeros((len(f), len(theta_radians)))
+
+    for i, lambda_i in enumerate(wvl):
+        for angle_idx, theta_i in enumerate(theta_radians):
+            M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
+            # Snell&#39;s law to calculate angle in each layer
+            sin_theta_i = np.sin(theta_i)
+            n_0 = n[i, 0]
+            sin_theta_layers = n_0 * sin_theta_i / n[i, :]
+            cos_theta_layers = np.sqrt(1 - sin_theta_layers**2)
+            
+            for j in range(len(d) - 1):
+                n_j, n_next = n[i, j], n[i, j+1]
+                d_j = d[j+1]
+                cos_theta_j, cos_theta_next = cos_theta_layers[j], cos_theta_layers[j+1]
+
+                # Interface calculations for TE and TM polarization with angle consideration
+                r_jk_TE = (n_j * cos_theta_j - n_next * cos_theta_next) / (n_j * cos_theta_j + n_next * cos_theta_next)
+                t_jk_TE = 2 * n_j * cos_theta_j / (n_j * cos_theta_j + n_next * cos_theta_next)
+                r_jk_TM = (n_next * cos_theta_j - n_j * cos_theta_next) / (n_next * cos_theta_j + n_j * cos_theta_next)
+                t_jk_TM = 2 * n_j * cos_theta_j / (n_next * cos_theta_j + n_j * cos_theta_next)
+                
+                M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
+                M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
+                
+                # Adjusting phase change calculation for angle
+                delta = 2 * np.pi * n_next * d_j * cos_theta_j / lambda_i
+                P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
+                
+                M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
+                M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
+
+            r_TE[i, angle_idx], t_TE[i, angle_idx] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
+            r_TM[i, angle_idx], t_TM[i, angle_idx] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
+            R_TE[i, angle_idx], T_TE[i, angle_idx] = np.abs(r_TE[i, angle_idx])**2, np.abs(t_TE[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
+            R_TM[i, angle_idx], T_TM[i, angle_idx] = np.abs(r_TM[i, angle_idx])**2, np.abs(t_TM[i, angle_idx])**2 * np.real(n[i, -1] / n_0)
+    return R_TE, T_TE, R_TM, T_TM</code></pre>
+</details>
+</dd>
+<dt id="layerlumos.layerlumos.stackrt0"><code class="name flex">
+<span>def <span class="ident">stackrt0</span></span>(<span>n, d, f)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Calculates the reflection and transmission coefficients for a multilayer stack
+at different frequencies under normal incidence.</p>
+<p>Parameters:
+- n (numpy.ndarray): The refractive indices of the layers for each frequency.
+Shape should be (Nfreq, Nlayers), where Nfreq is the number of
+frequencies and Nlayers is the number of layers.
+- d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
+- f (numpy.ndarray): The frequencies at which to calculate the coefficients.
+Shape should be (Nfreq,).</p>
+<p>Returns:
+- R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
+- T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
+- R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
+- T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def stackrt0(n, d, f):
+    &#34;&#34;&#34;
+    Calculates the reflection and transmission coefficients for a multilayer stack
+    at different frequencies under normal incidence.
+
+    Parameters:
+    - n (numpy.ndarray): The refractive indices of the layers for each frequency.
+                         Shape should be (Nfreq, Nlayers), where Nfreq is the number of
+                         frequencies and Nlayers is the number of layers.
+    - d (numpy.ndarray): The thicknesses of the layers. Shape should be (Nlayers,).
+    - f (numpy.ndarray): The frequencies at which to calculate the coefficients.
+                         Shape should be (Nfreq,).
+
+    Returns:
+    - R_TE (numpy.ndarray): Reflectance for TE polarization. Shape is (Nfreq,).
+    - T_TE (numpy.ndarray): Transmittance for TE polarization. Shape is (Nfreq,).
+    - R_TM (numpy.ndarray): Reflectance for TM polarization. Shape is (Nfreq,).
+    - T_TM (numpy.ndarray): Transmittance for TM polarization. Shape is (Nfreq,).
+    &#34;&#34;&#34;
+    wvl = c / f  # Convert frequency to wavelength
+    # Initialize arrays for both amplitude and intensity coefficients
+    r_TE, r_TM, t_TE, t_TM = np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128), np.zeros_like(f, dtype=np.complex128)
+    R_TE, T_TE, R_TM, T_TM = np.zeros_like(f), np.zeros_like(f), np.zeros_like(f), np.zeros_like(f)
+
+    for i, freq in enumerate(f):  # Iterate over each frequency
+        lambda_i = wvl[i]
+        M_TE, M_TM = np.eye(2, dtype=np.complex128), np.eye(2, dtype=np.complex128)
+        for j in range(0, len(n[i, :]) - 1):
+            n_j = n[i, j]
+            n_next = n[i, j+1]
+            d_next = d[j+1]
+
+            # Interface calculations for TE and TM polarization
+            r_jk_TE = (n_j - n_next) / (n_j + n_next)
+            t_jk_TE = 2 * n_j / (n_j + n_next)
+            M_jk_TE = np.array([[1/t_jk_TE, r_jk_TE/t_jk_TE], [r_jk_TE/t_jk_TE, 1/t_jk_TE]], dtype=np.complex128)
+            r_jk_TM = (n_next - n_j) / (n_next + n_j)
+            t_jk_TM = 2 * n_j / (n_next + n_j)
+            M_jk_TM = np.array([[1/t_jk_TM, r_jk_TM/t_jk_TM], [r_jk_TM/t_jk_TM, 1/t_jk_TM]], dtype=np.complex128)
+            
+            delta = 2 * np.pi * n_next * d_next / lambda_i
+            P = np.array([[np.exp(-1j * delta.item()), 0], [0, np.exp(1j * delta.item())]], dtype=np.complex128)
+            M_TE = np.dot(M_TE, np.dot(M_jk_TE, P))
+            M_TM = np.dot(M_TM, np.dot(M_jk_TM, P))
+
+        r_TE[i], t_TE[i] = M_TE[1, 0] / M_TE[0, 0], 1 / M_TE[0, 0]
+        r_TM[i], t_TM[i] = M_TM[1, 0] / M_TM[0, 0], 1 / M_TM[0, 0]
+        R_TE[i], T_TE[i] = np.abs(r_TE[i])**2, np.abs(t_TE[i])**2 * np.real(n[i, -1] / n[i, 0])
+        R_TM[i], T_TM[i] = np.abs(r_TM[i])**2, np.abs(t_TM[i])**2 * np.real(n[i, -1] / n[i, 0])
+
+    return R_TE, T_TE, R_TM, T_TM</code></pre>
+</details>
+</dd>
+</dl>
+</section>
+<section>
+</section>
+</article>
+<nav id="sidebar">
+<h1>Index</h1>
+<div class="toc">
+<ul></ul>
+</div>
+<ul id="index">
+<li><h3>Super-module</h3>
+<ul>
+<li><code><a title="layerlumos" href="index.html">layerlumos</a></code></li>
+</ul>
+</li>
+<li><h3><a href="#header-functions">Functions</a></h3>
+<ul class="">
+<li><code><a title="layerlumos.layerlumos.stackrt" href="#layerlumos.layerlumos.stackrt">stackrt</a></code></li>
+<li><code><a title="layerlumos.layerlumos.stackrt0" href="#layerlumos.layerlumos.stackrt0">stackrt0</a></code></li>
+</ul>
+</li>
+</ul>
+</nav>
+</main>
+<footer id="footer">
+<p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
+</footer>
+</body>
 </html>
```

### Comparing `layerlumos-1.0.0/docs/api/utils.html` & `layerlumos-1.0.1/docs/api/utils.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,393 +1,393 @@
-<!doctype html>
-<html lang="en">
-<head>
-<meta charset="utf-8">
-<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
-<meta name="generator" content="pdoc 0.10.0" />
-<title>layerlumos.utils API documentation</title>
-<meta name="description" content="" />
-<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
-<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
-<link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
-<style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
-<style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
-<style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
-<script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
-<script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
-</head>
-<body>
-<main>
-<article id="content">
-<header>
-<h1 class="title">Module <code>layerlumos.utils</code></h1>
-</header>
-<section id="section-intro">
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">import csv
-import json
-import os
-from pathlib import Path
-import numpy as np
-from scipy.interpolate import interp1d
-from scipy.constants import c
-
-Metals_sigma = {
-    &#39;Cu&#39;: 5.96e7,
-    &#39;Cr&#39;: 7.74e6,
-    &#39;Ag&#39;: 6.3e7,
-    &#39;Al&#39;: 3.77e7,
-    &#39;Ni&#39; : 1.43e7,
-    &#39;W&#39; : 1.79e7,
-    &#39;Ti&#39; : 2.38e6,
-    &#39;Pd&#39; : 9.52e6
-}
-Metals_nk_updated_specific_sigma = {}
-mu0 = 4 * np.pi * 1e-7  # H/m
-Z_0 = 377  # Ohms, impedance of free space
-# Frequency range
-nu = np.linspace(8e9, 18e9, 11)  # From 8 GHz to 18 GHz
-omega = 2 * np.pi * nu  # Angular frequency
-for metal, sigma in Metals_sigma.items():
-    Z = np.sqrt(1j * omega * mu0 / sigma)  # Impedance of the material using specific sigma
-    n_complex = Z_0 / Z  # Complex refractive index
-
-    # Extract real and imaginary parts of the refractive index
-    n_real = np.real(n_complex)
-    k_imag = np.imag(n_complex)
-    
-    # Update the dictionary with the new values
-    Metals_nk_updated_specific_sigma[metal] = {
-        &#39;freq_data&#39;: nu.tolist(),
-        &#39;n_data&#39;: n_real.tolist(),
-        &#39;k_data&#39;: k_imag.tolist()
-    }
-def load_material_RF(material_name, frequencies):
-    &#34;&#34;&#34;
-    Load material RF data for a given material and frequencies.
-    
-    Parameters:
-    - material_name: The name of the material to load.
-    - frequencies: Array of frequencies for which data is requested.
-    
-    Returns:
-    - A NumPy array with columns for frequency, n, and k.
-    &#34;&#34;&#34;
-    # Check if the material is defined
-    if material_name not in Metals_nk_updated_specific_sigma:
-        # Material not found, return default values (n=1, k=0) for given frequencies
-        n_default = np.ones_like(frequencies)
-        k_default = np.zeros_like(frequencies)
-        data = np.column_stack((frequencies, n_default, k_default))
-    else:
-        # Material found, extract the data
-        material_data = Metals_nk_updated_specific_sigma[material_name]
-        freq_data = np.array(material_data[&#39;freq_data&#39;])
-        n_data = np.array(material_data[&#39;n_data&#39;])
-        k_data = np.array(material_data[&#39;k_data&#39;])
-        
-        # Interpolate n and k data for the input frequencies, if necessary
-        n_interpolated = np.interp(frequencies, freq_data, n_data)
-        k_interpolated = np.interp(frequencies, freq_data, k_data)
-        
-        # Combine the data
-        data = np.column_stack((frequencies, n_interpolated, k_interpolated))
-    
-    return data
-
-
-
-def load_material(material_name):
-    &#34;&#34;&#34;
-    Load material data from its CSV file, converting wavelength to frequency.
-
-    Parameters:
-    - material_name: The name of the material to load.
-    
-    Returns:
-    - A NumPy array with columns for frequency (converted from wavelength), n, and k.
-    &#34;&#34;&#34;
-    # Determine the directory of the current script
-    current_dir = Path(__file__).parent
-
-    # Build the absolute path to materials.json
-    materials_file = current_dir / &#34;materials.json&#34;
-
-    # Load the material index JSON to find the CSV file path
-    with open(materials_file, &#39;r&#39;) as file:
-        material_index = json.load(file)
-    
-    # Get the file path for the requested material
-    relative_file_path = material_index.get(material_name)
-    if not relative_file_path:
-        raise ValueError(f&#34;Material {material_name} not found in the index.&#34;)
-    
-    # Construct the absolute path to the material CSV file
-    csv_file_path = current_dir / relative_file_path
-
-    # Initialize a list to hold the converted data
-    data = []
-    
-    # Open and read the CSV file
-    with open(csv_file_path, &#39;r&#39;) as csvfile:
-        csvreader = csv.reader(csvfile)
-        next(csvreader)  # Skip the header row
-        for row in csvreader:
-            try:
-                # Attempt to convert wavelength, n, and k to floats
-                wavelength_um, n, k = map(float, row)
-                # Convert wavelength in um to frequency in Hz
-                frequency = c / (wavelength_um * 1e-6)
-                data.append((frequency, n, k))
-            except ValueError:
-                # If conversion fails, skip this row
-                continue
-    
-    # Convert to a NumPy array for easier handling in calculations
-    data = np.array(data)
-    # Ensure the data is sorted by frequency in ascending order
-    data = data[data[:, 0].argsort()]
-    
-    return data
-
-def interpolate_material(material_data, frequencies):
-    &#34;&#34;&#34;
-    Interpolate n and k values for the specified frequencies.
-
-    Parameters:
-    - material_data: The data for the material, as returned by load_material.
-    - frequencies: A list or NumPy array of frequencies to interpolate n and k for.
-    
-    Returns:
-    - Interpolated values of n and k as a NumPy array.
-    &#34;&#34;&#34;
-    # Extract frequency, n, and k columns
-    freqs, n_values, k_values = material_data.T
-    
-    # Remove duplicates (if any) while preserving order
-    unique_freqs, indices = np.unique(freqs, return_index=True)
-    unique_n_values = n_values[indices]
-    unique_k_values = k_values[indices]
-    
-    # Ensure frequencies are sorted (usually they should be, but just in case)
-    sorted_indices = np.argsort(unique_freqs)
-    sorted_freqs = unique_freqs[sorted_indices]
-    sorted_n_values = unique_n_values[sorted_indices]
-    sorted_k_values = unique_k_values[sorted_indices]
-    
-    # Create interpolation functions for the sorted, unique data
-    n_interp = interp1d(sorted_freqs, sorted_n_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
-    k_interp = interp1d(sorted_freqs, sorted_k_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
-    
-    # Interpolate n and k for the given frequencies
-    n_interp_values = n_interp(frequencies)
-    k_interp_values = k_interp(frequencies)
-    
-    return np.vstack((n_interp_values, k_interp_values)).T</code></pre>
-</details>
-</section>
-<section>
-</section>
-<section>
-</section>
-<section>
-<h2 class="section-title" id="header-functions">Functions</h2>
-<dl>
-<dt id="layerlumos.utils.interpolate_material"><code class="name flex">
-<span>def <span class="ident">interpolate_material</span></span>(<span>material_data, frequencies)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>Interpolate n and k values for the specified frequencies.</p>
-<p>Parameters:
-- material_data: The data for the material, as returned by load_material.
-- frequencies: A list or NumPy array of frequencies to interpolate n and k for.</p>
-<p>Returns:
-- Interpolated values of n and k as a NumPy array.</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def interpolate_material(material_data, frequencies):
-    &#34;&#34;&#34;
-    Interpolate n and k values for the specified frequencies.
-
-    Parameters:
-    - material_data: The data for the material, as returned by load_material.
-    - frequencies: A list or NumPy array of frequencies to interpolate n and k for.
-    
-    Returns:
-    - Interpolated values of n and k as a NumPy array.
-    &#34;&#34;&#34;
-    # Extract frequency, n, and k columns
-    freqs, n_values, k_values = material_data.T
-    
-    # Remove duplicates (if any) while preserving order
-    unique_freqs, indices = np.unique(freqs, return_index=True)
-    unique_n_values = n_values[indices]
-    unique_k_values = k_values[indices]
-    
-    # Ensure frequencies are sorted (usually they should be, but just in case)
-    sorted_indices = np.argsort(unique_freqs)
-    sorted_freqs = unique_freqs[sorted_indices]
-    sorted_n_values = unique_n_values[sorted_indices]
-    sorted_k_values = unique_k_values[sorted_indices]
-    
-    # Create interpolation functions for the sorted, unique data
-    n_interp = interp1d(sorted_freqs, sorted_n_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
-    k_interp = interp1d(sorted_freqs, sorted_k_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
-    
-    # Interpolate n and k for the given frequencies
-    n_interp_values = n_interp(frequencies)
-    k_interp_values = k_interp(frequencies)
-    
-    return np.vstack((n_interp_values, k_interp_values)).T</code></pre>
-</details>
-</dd>
-<dt id="layerlumos.utils.load_material"><code class="name flex">
-<span>def <span class="ident">load_material</span></span>(<span>material_name)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>Load material data from its CSV file, converting wavelength to frequency.</p>
-<p>Parameters:
-- material_name: The name of the material to load.</p>
-<p>Returns:
-- A NumPy array with columns for frequency (converted from wavelength), n, and k.</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def load_material(material_name):
-    &#34;&#34;&#34;
-    Load material data from its CSV file, converting wavelength to frequency.
-
-    Parameters:
-    - material_name: The name of the material to load.
-    
-    Returns:
-    - A NumPy array with columns for frequency (converted from wavelength), n, and k.
-    &#34;&#34;&#34;
-    # Determine the directory of the current script
-    current_dir = Path(__file__).parent
-
-    # Build the absolute path to materials.json
-    materials_file = current_dir / &#34;materials.json&#34;
-
-    # Load the material index JSON to find the CSV file path
-    with open(materials_file, &#39;r&#39;) as file:
-        material_index = json.load(file)
-    
-    # Get the file path for the requested material
-    relative_file_path = material_index.get(material_name)
-    if not relative_file_path:
-        raise ValueError(f&#34;Material {material_name} not found in the index.&#34;)
-    
-    # Construct the absolute path to the material CSV file
-    csv_file_path = current_dir / relative_file_path
-
-    # Initialize a list to hold the converted data
-    data = []
-    
-    # Open and read the CSV file
-    with open(csv_file_path, &#39;r&#39;) as csvfile:
-        csvreader = csv.reader(csvfile)
-        next(csvreader)  # Skip the header row
-        for row in csvreader:
-            try:
-                # Attempt to convert wavelength, n, and k to floats
-                wavelength_um, n, k = map(float, row)
-                # Convert wavelength in um to frequency in Hz
-                frequency = c / (wavelength_um * 1e-6)
-                data.append((frequency, n, k))
-            except ValueError:
-                # If conversion fails, skip this row
-                continue
-    
-    # Convert to a NumPy array for easier handling in calculations
-    data = np.array(data)
-    # Ensure the data is sorted by frequency in ascending order
-    data = data[data[:, 0].argsort()]
-    
-    return data</code></pre>
-</details>
-</dd>
-<dt id="layerlumos.utils.load_material_RF"><code class="name flex">
-<span>def <span class="ident">load_material_RF</span></span>(<span>material_name, frequencies)</span>
-</code></dt>
-<dd>
-<div class="desc"><p>Load material RF data for a given material and frequencies.</p>
-<p>Parameters:
-- material_name: The name of the material to load.
-- frequencies: Array of frequencies for which data is requested.</p>
-<p>Returns:
-- A NumPy array with columns for frequency, n, and k.</p></div>
-<details class="source">
-<summary>
-<span>Expand source code</span>
-</summary>
-<pre><code class="python">def load_material_RF(material_name, frequencies):
-    &#34;&#34;&#34;
-    Load material RF data for a given material and frequencies.
-    
-    Parameters:
-    - material_name: The name of the material to load.
-    - frequencies: Array of frequencies for which data is requested.
-    
-    Returns:
-    - A NumPy array with columns for frequency, n, and k.
-    &#34;&#34;&#34;
-    # Check if the material is defined
-    if material_name not in Metals_nk_updated_specific_sigma:
-        # Material not found, return default values (n=1, k=0) for given frequencies
-        n_default = np.ones_like(frequencies)
-        k_default = np.zeros_like(frequencies)
-        data = np.column_stack((frequencies, n_default, k_default))
-    else:
-        # Material found, extract the data
-        material_data = Metals_nk_updated_specific_sigma[material_name]
-        freq_data = np.array(material_data[&#39;freq_data&#39;])
-        n_data = np.array(material_data[&#39;n_data&#39;])
-        k_data = np.array(material_data[&#39;k_data&#39;])
-        
-        # Interpolate n and k data for the input frequencies, if necessary
-        n_interpolated = np.interp(frequencies, freq_data, n_data)
-        k_interpolated = np.interp(frequencies, freq_data, k_data)
-        
-        # Combine the data
-        data = np.column_stack((frequencies, n_interpolated, k_interpolated))
-    
-    return data</code></pre>
-</details>
-</dd>
-</dl>
-</section>
-<section>
-</section>
-</article>
-<nav id="sidebar">
-<h1>Index</h1>
-<div class="toc">
-<ul></ul>
-</div>
-<ul id="index">
-<li><h3>Super-module</h3>
-<ul>
-<li><code><a title="layerlumos" href="index.html">layerlumos</a></code></li>
-</ul>
-</li>
-<li><h3><a href="#header-functions">Functions</a></h3>
-<ul class="">
-<li><code><a title="layerlumos.utils.interpolate_material" href="#layerlumos.utils.interpolate_material">interpolate_material</a></code></li>
-<li><code><a title="layerlumos.utils.load_material" href="#layerlumos.utils.load_material">load_material</a></code></li>
-<li><code><a title="layerlumos.utils.load_material_RF" href="#layerlumos.utils.load_material_RF">load_material_RF</a></code></li>
-</ul>
-</li>
-</ul>
-</nav>
-</main>
-<footer id="footer">
-<p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
-</footer>
-</body>
+<!doctype html>
+<html lang="en">
+<head>
+<meta charset="utf-8">
+<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1" />
+<meta name="generator" content="pdoc 0.10.0" />
+<title>layerlumos.utils API documentation</title>
+<meta name="description" content="" />
+<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/sanitize.min.css" integrity="sha256-PK9q560IAAa6WVRRh76LtCaI8pjTJ2z11v0miyNNjrs=" crossorigin>
+<link rel="preload stylesheet" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/10up-sanitize.css/11.0.1/typography.min.css" integrity="sha256-7l/o7C8jubJiy74VsKTidCy1yBkRtiUGbVkYBylBqUg=" crossorigin>
+<link rel="stylesheet preload" as="style" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/styles/github.min.css" crossorigin>
+<style>:root{--highlight-color:#fe9}.flex{display:flex !important}body{line-height:1.5em}#content{padding:20px}#sidebar{padding:30px;overflow:hidden}#sidebar > *:last-child{margin-bottom:2cm}.http-server-breadcrumbs{font-size:130%;margin:0 0 15px 0}#footer{font-size:.75em;padding:5px 30px;border-top:1px solid #ddd;text-align:right}#footer p{margin:0 0 0 1em;display:inline-block}#footer p:last-child{margin-right:30px}h1,h2,h3,h4,h5{font-weight:300}h1{font-size:2.5em;line-height:1.1em}h2{font-size:1.75em;margin:1em 0 .50em 0}h3{font-size:1.4em;margin:25px 0 10px 0}h4{margin:0;font-size:105%}h1:target,h2:target,h3:target,h4:target,h5:target,h6:target{background:var(--highlight-color);padding:.2em 0}a{color:#058;text-decoration:none;transition:color .3s ease-in-out}a:hover{color:#e82}.title code{font-weight:bold}h2[id^="header-"]{margin-top:2em}.ident{color:#900}pre code{background:#f8f8f8;font-size:.8em;line-height:1.4em}code{background:#f2f2f1;padding:1px 4px;overflow-wrap:break-word}h1 code{background:transparent}pre{background:#f8f8f8;border:0;border-top:1px solid #ccc;border-bottom:1px solid #ccc;margin:1em 0;padding:1ex}#http-server-module-list{display:flex;flex-flow:column}#http-server-module-list div{display:flex}#http-server-module-list dt{min-width:10%}#http-server-module-list p{margin-top:0}.toc ul,#index{list-style-type:none;margin:0;padding:0}#index code{background:transparent}#index h3{border-bottom:1px solid #ddd}#index ul{padding:0}#index h4{margin-top:.6em;font-weight:bold}@media (min-width:200ex){#index .two-column{column-count:2}}@media (min-width:300ex){#index .two-column{column-count:3}}dl{margin-bottom:2em}dl dl:last-child{margin-bottom:4em}dd{margin:0 0 1em 3em}#header-classes + dl > dd{margin-bottom:3em}dd dd{margin-left:2em}dd p{margin:10px 0}.name{background:#eee;font-weight:bold;font-size:.85em;padding:5px 10px;display:inline-block;min-width:40%}.name:hover{background:#e0e0e0}dt:target .name{background:var(--highlight-color)}.name > span:first-child{white-space:nowrap}.name.class > span:nth-child(2){margin-left:.4em}.inherited{color:#999;border-left:5px solid #eee;padding-left:1em}.inheritance em{font-style:normal;font-weight:bold}.desc h2{font-weight:400;font-size:1.25em}.desc h3{font-size:1em}.desc dt code{background:inherit}.source summary,.git-link-div{color:#666;text-align:right;font-weight:400;font-size:.8em;text-transform:uppercase}.source summary > *{white-space:nowrap;cursor:pointer}.git-link{color:inherit;margin-left:1em}.source pre{max-height:500px;overflow:auto;margin:0}.source pre code{font-size:12px;overflow:visible}.hlist{list-style:none}.hlist li{display:inline}.hlist li:after{content:',\2002'}.hlist li:last-child:after{content:none}.hlist .hlist{display:inline;padding-left:1em}img{max-width:100%}td{padding:0 .5em}.admonition{padding:.1em .5em;margin-bottom:1em}.admonition-title{font-weight:bold}.admonition.note,.admonition.info,.admonition.important{background:#aef}.admonition.todo,.admonition.versionadded,.admonition.tip,.admonition.hint{background:#dfd}.admonition.warning,.admonition.versionchanged,.admonition.deprecated{background:#fd4}.admonition.error,.admonition.danger,.admonition.caution{background:lightpink}</style>
+<style media="screen and (min-width: 700px)">@media screen and (min-width:700px){#sidebar{width:30%;height:100vh;overflow:auto;position:sticky;top:0}#content{width:70%;max-width:100ch;padding:3em 4em;border-left:1px solid #ddd}pre code{font-size:1em}.item .name{font-size:1em}main{display:flex;flex-direction:row-reverse;justify-content:flex-end}.toc ul ul,#index ul{padding-left:1.5em}.toc > ul > li{margin-top:.5em}}</style>
+<style media="print">@media print{#sidebar h1{page-break-before:always}.source{display:none}}@media print{*{background:transparent !important;color:#000 !important;box-shadow:none !important;text-shadow:none !important}a[href]:after{content:" (" attr(href) ")";font-size:90%}a[href][title]:after{content:none}abbr[title]:after{content:" (" attr(title) ")"}.ir a:after,a[href^="javascript:"]:after,a[href^="#"]:after{content:""}pre,blockquote{border:1px solid #999;page-break-inside:avoid}thead{display:table-header-group}tr,img{page-break-inside:avoid}img{max-width:100% !important}@page{margin:0.5cm}p,h2,h3{orphans:3;widows:3}h1,h2,h3,h4,h5,h6{page-break-after:avoid}}</style>
+<script defer src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/10.1.1/highlight.min.js" integrity="sha256-Uv3H6lx7dJmRfRvH8TH6kJD1TSK1aFcwgx+mdg3epi8=" crossorigin></script>
+<script>window.addEventListener('DOMContentLoaded', () => hljs.initHighlighting())</script>
+</head>
+<body>
+<main>
+<article id="content">
+<header>
+<h1 class="title">Module <code>layerlumos.utils</code></h1>
+</header>
+<section id="section-intro">
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">import csv
+import json
+import os
+from pathlib import Path
+import numpy as np
+from scipy.interpolate import interp1d
+from scipy.constants import c
+
+Metals_sigma = {
+    &#39;Cu&#39;: 5.96e7,
+    &#39;Cr&#39;: 7.74e6,
+    &#39;Ag&#39;: 6.3e7,
+    &#39;Al&#39;: 3.77e7,
+    &#39;Ni&#39; : 1.43e7,
+    &#39;W&#39; : 1.79e7,
+    &#39;Ti&#39; : 2.38e6,
+    &#39;Pd&#39; : 9.52e6
+}
+Metals_nk_updated_specific_sigma = {}
+mu0 = 4 * np.pi * 1e-7  # H/m
+Z_0 = 377  # Ohms, impedance of free space
+# Frequency range
+nu = np.linspace(8e9, 18e9, 11)  # From 8 GHz to 18 GHz
+omega = 2 * np.pi * nu  # Angular frequency
+for metal, sigma in Metals_sigma.items():
+    Z = np.sqrt(1j * omega * mu0 / sigma)  # Impedance of the material using specific sigma
+    n_complex = Z_0 / Z  # Complex refractive index
+
+    # Extract real and imaginary parts of the refractive index
+    n_real = np.real(n_complex)
+    k_imag = np.imag(n_complex)
+    
+    # Update the dictionary with the new values
+    Metals_nk_updated_specific_sigma[metal] = {
+        &#39;freq_data&#39;: nu.tolist(),
+        &#39;n_data&#39;: n_real.tolist(),
+        &#39;k_data&#39;: k_imag.tolist()
+    }
+def load_material_RF(material_name, frequencies):
+    &#34;&#34;&#34;
+    Load material RF data for a given material and frequencies.
+    
+    Parameters:
+    - material_name: The name of the material to load.
+    - frequencies: Array of frequencies for which data is requested.
+    
+    Returns:
+    - A NumPy array with columns for frequency, n, and k.
+    &#34;&#34;&#34;
+    # Check if the material is defined
+    if material_name not in Metals_nk_updated_specific_sigma:
+        # Material not found, return default values (n=1, k=0) for given frequencies
+        n_default = np.ones_like(frequencies)
+        k_default = np.zeros_like(frequencies)
+        data = np.column_stack((frequencies, n_default, k_default))
+    else:
+        # Material found, extract the data
+        material_data = Metals_nk_updated_specific_sigma[material_name]
+        freq_data = np.array(material_data[&#39;freq_data&#39;])
+        n_data = np.array(material_data[&#39;n_data&#39;])
+        k_data = np.array(material_data[&#39;k_data&#39;])
+        
+        # Interpolate n and k data for the input frequencies, if necessary
+        n_interpolated = np.interp(frequencies, freq_data, n_data)
+        k_interpolated = np.interp(frequencies, freq_data, k_data)
+        
+        # Combine the data
+        data = np.column_stack((frequencies, n_interpolated, k_interpolated))
+    
+    return data
+
+
+
+def load_material(material_name):
+    &#34;&#34;&#34;
+    Load material data from its CSV file, converting wavelength to frequency.
+
+    Parameters:
+    - material_name: The name of the material to load.
+    
+    Returns:
+    - A NumPy array with columns for frequency (converted from wavelength), n, and k.
+    &#34;&#34;&#34;
+    # Determine the directory of the current script
+    current_dir = Path(__file__).parent
+
+    # Build the absolute path to materials.json
+    materials_file = current_dir / &#34;materials.json&#34;
+
+    # Load the material index JSON to find the CSV file path
+    with open(materials_file, &#39;r&#39;) as file:
+        material_index = json.load(file)
+    
+    # Get the file path for the requested material
+    relative_file_path = material_index.get(material_name)
+    if not relative_file_path:
+        raise ValueError(f&#34;Material {material_name} not found in the index.&#34;)
+    
+    # Construct the absolute path to the material CSV file
+    csv_file_path = current_dir / relative_file_path
+
+    # Initialize a list to hold the converted data
+    data = []
+    
+    # Open and read the CSV file
+    with open(csv_file_path, &#39;r&#39;) as csvfile:
+        csvreader = csv.reader(csvfile)
+        next(csvreader)  # Skip the header row
+        for row in csvreader:
+            try:
+                # Attempt to convert wavelength, n, and k to floats
+                wavelength_um, n, k = map(float, row)
+                # Convert wavelength in um to frequency in Hz
+                frequency = c / (wavelength_um * 1e-6)
+                data.append((frequency, n, k))
+            except ValueError:
+                # If conversion fails, skip this row
+                continue
+    
+    # Convert to a NumPy array for easier handling in calculations
+    data = np.array(data)
+    # Ensure the data is sorted by frequency in ascending order
+    data = data[data[:, 0].argsort()]
+    
+    return data
+
+def interpolate_material(material_data, frequencies):
+    &#34;&#34;&#34;
+    Interpolate n and k values for the specified frequencies.
+
+    Parameters:
+    - material_data: The data for the material, as returned by load_material.
+    - frequencies: A list or NumPy array of frequencies to interpolate n and k for.
+    
+    Returns:
+    - Interpolated values of n and k as a NumPy array.
+    &#34;&#34;&#34;
+    # Extract frequency, n, and k columns
+    freqs, n_values, k_values = material_data.T
+    
+    # Remove duplicates (if any) while preserving order
+    unique_freqs, indices = np.unique(freqs, return_index=True)
+    unique_n_values = n_values[indices]
+    unique_k_values = k_values[indices]
+    
+    # Ensure frequencies are sorted (usually they should be, but just in case)
+    sorted_indices = np.argsort(unique_freqs)
+    sorted_freqs = unique_freqs[sorted_indices]
+    sorted_n_values = unique_n_values[sorted_indices]
+    sorted_k_values = unique_k_values[sorted_indices]
+    
+    # Create interpolation functions for the sorted, unique data
+    n_interp = interp1d(sorted_freqs, sorted_n_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
+    k_interp = interp1d(sorted_freqs, sorted_k_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
+    
+    # Interpolate n and k for the given frequencies
+    n_interp_values = n_interp(frequencies)
+    k_interp_values = k_interp(frequencies)
+    
+    return np.vstack((n_interp_values, k_interp_values)).T</code></pre>
+</details>
+</section>
+<section>
+</section>
+<section>
+</section>
+<section>
+<h2 class="section-title" id="header-functions">Functions</h2>
+<dl>
+<dt id="layerlumos.utils.interpolate_material"><code class="name flex">
+<span>def <span class="ident">interpolate_material</span></span>(<span>material_data, frequencies)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Interpolate n and k values for the specified frequencies.</p>
+<p>Parameters:
+- material_data: The data for the material, as returned by load_material.
+- frequencies: A list or NumPy array of frequencies to interpolate n and k for.</p>
+<p>Returns:
+- Interpolated values of n and k as a NumPy array.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def interpolate_material(material_data, frequencies):
+    &#34;&#34;&#34;
+    Interpolate n and k values for the specified frequencies.
+
+    Parameters:
+    - material_data: The data for the material, as returned by load_material.
+    - frequencies: A list or NumPy array of frequencies to interpolate n and k for.
+    
+    Returns:
+    - Interpolated values of n and k as a NumPy array.
+    &#34;&#34;&#34;
+    # Extract frequency, n, and k columns
+    freqs, n_values, k_values = material_data.T
+    
+    # Remove duplicates (if any) while preserving order
+    unique_freqs, indices = np.unique(freqs, return_index=True)
+    unique_n_values = n_values[indices]
+    unique_k_values = k_values[indices]
+    
+    # Ensure frequencies are sorted (usually they should be, but just in case)
+    sorted_indices = np.argsort(unique_freqs)
+    sorted_freqs = unique_freqs[sorted_indices]
+    sorted_n_values = unique_n_values[sorted_indices]
+    sorted_k_values = unique_k_values[sorted_indices]
+    
+    # Create interpolation functions for the sorted, unique data
+    n_interp = interp1d(sorted_freqs, sorted_n_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
+    k_interp = interp1d(sorted_freqs, sorted_k_values, kind=&#39;cubic&#39;, fill_value=&#34;extrapolate&#34;)
+    
+    # Interpolate n and k for the given frequencies
+    n_interp_values = n_interp(frequencies)
+    k_interp_values = k_interp(frequencies)
+    
+    return np.vstack((n_interp_values, k_interp_values)).T</code></pre>
+</details>
+</dd>
+<dt id="layerlumos.utils.load_material"><code class="name flex">
+<span>def <span class="ident">load_material</span></span>(<span>material_name)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Load material data from its CSV file, converting wavelength to frequency.</p>
+<p>Parameters:
+- material_name: The name of the material to load.</p>
+<p>Returns:
+- A NumPy array with columns for frequency (converted from wavelength), n, and k.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def load_material(material_name):
+    &#34;&#34;&#34;
+    Load material data from its CSV file, converting wavelength to frequency.
+
+    Parameters:
+    - material_name: The name of the material to load.
+    
+    Returns:
+    - A NumPy array with columns for frequency (converted from wavelength), n, and k.
+    &#34;&#34;&#34;
+    # Determine the directory of the current script
+    current_dir = Path(__file__).parent
+
+    # Build the absolute path to materials.json
+    materials_file = current_dir / &#34;materials.json&#34;
+
+    # Load the material index JSON to find the CSV file path
+    with open(materials_file, &#39;r&#39;) as file:
+        material_index = json.load(file)
+    
+    # Get the file path for the requested material
+    relative_file_path = material_index.get(material_name)
+    if not relative_file_path:
+        raise ValueError(f&#34;Material {material_name} not found in the index.&#34;)
+    
+    # Construct the absolute path to the material CSV file
+    csv_file_path = current_dir / relative_file_path
+
+    # Initialize a list to hold the converted data
+    data = []
+    
+    # Open and read the CSV file
+    with open(csv_file_path, &#39;r&#39;) as csvfile:
+        csvreader = csv.reader(csvfile)
+        next(csvreader)  # Skip the header row
+        for row in csvreader:
+            try:
+                # Attempt to convert wavelength, n, and k to floats
+                wavelength_um, n, k = map(float, row)
+                # Convert wavelength in um to frequency in Hz
+                frequency = c / (wavelength_um * 1e-6)
+                data.append((frequency, n, k))
+            except ValueError:
+                # If conversion fails, skip this row
+                continue
+    
+    # Convert to a NumPy array for easier handling in calculations
+    data = np.array(data)
+    # Ensure the data is sorted by frequency in ascending order
+    data = data[data[:, 0].argsort()]
+    
+    return data</code></pre>
+</details>
+</dd>
+<dt id="layerlumos.utils.load_material_RF"><code class="name flex">
+<span>def <span class="ident">load_material_RF</span></span>(<span>material_name, frequencies)</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Load material RF data for a given material and frequencies.</p>
+<p>Parameters:
+- material_name: The name of the material to load.
+- frequencies: Array of frequencies for which data is requested.</p>
+<p>Returns:
+- A NumPy array with columns for frequency, n, and k.</p></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def load_material_RF(material_name, frequencies):
+    &#34;&#34;&#34;
+    Load material RF data for a given material and frequencies.
+    
+    Parameters:
+    - material_name: The name of the material to load.
+    - frequencies: Array of frequencies for which data is requested.
+    
+    Returns:
+    - A NumPy array with columns for frequency, n, and k.
+    &#34;&#34;&#34;
+    # Check if the material is defined
+    if material_name not in Metals_nk_updated_specific_sigma:
+        # Material not found, return default values (n=1, k=0) for given frequencies
+        n_default = np.ones_like(frequencies)
+        k_default = np.zeros_like(frequencies)
+        data = np.column_stack((frequencies, n_default, k_default))
+    else:
+        # Material found, extract the data
+        material_data = Metals_nk_updated_specific_sigma[material_name]
+        freq_data = np.array(material_data[&#39;freq_data&#39;])
+        n_data = np.array(material_data[&#39;n_data&#39;])
+        k_data = np.array(material_data[&#39;k_data&#39;])
+        
+        # Interpolate n and k data for the input frequencies, if necessary
+        n_interpolated = np.interp(frequencies, freq_data, n_data)
+        k_interpolated = np.interp(frequencies, freq_data, k_data)
+        
+        # Combine the data
+        data = np.column_stack((frequencies, n_interpolated, k_interpolated))
+    
+    return data</code></pre>
+</details>
+</dd>
+</dl>
+</section>
+<section>
+</section>
+</article>
+<nav id="sidebar">
+<h1>Index</h1>
+<div class="toc">
+<ul></ul>
+</div>
+<ul id="index">
+<li><h3>Super-module</h3>
+<ul>
+<li><code><a title="layerlumos" href="index.html">layerlumos</a></code></li>
+</ul>
+</li>
+<li><h3><a href="#header-functions">Functions</a></h3>
+<ul class="">
+<li><code><a title="layerlumos.utils.interpolate_material" href="#layerlumos.utils.interpolate_material">interpolate_material</a></code></li>
+<li><code><a title="layerlumos.utils.load_material" href="#layerlumos.utils.load_material">load_material</a></code></li>
+<li><code><a title="layerlumos.utils.load_material_RF" href="#layerlumos.utils.load_material_RF">load_material_RF</a></code></li>
+</ul>
+</li>
+</ul>
+</nav>
+</main>
+<footer id="footer">
+<p>Generated by <a href="https://pdoc3.github.io/pdoc" title="pdoc: Python API documentation generator"><cite>pdoc</cite> 0.10.0</a>.</p>
+</footer>
+</body>
 </html>
```

### Comparing `layerlumos-1.0.0/docs/assets/Icon1.jpg` & `layerlumos-1.0.1/docs/assets/Icon1.jpg`

 * *Files identical despite different names*

### Comparing `layerlumos-1.0.0/docs/assets/Icon2.jpg` & `layerlumos-1.0.1/docs/assets/Icon2.jpg`

 * *Files identical despite different names*

### Comparing `layerlumos-1.0.0/docs/assets/icon3.jpg` & `layerlumos-1.0.1/docs/assets/icon3.jpg`

 * *Files identical despite different names*

### Comparing `layerlumos-1.0.0/docs/conf.py` & `layerlumos-1.0.1/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-import os
-import sys
-sys.path.insert(0, os.path.abspath('../'))
-sys.path.insert(0, os.path.abspath('../examples'))
-
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
-
-project = 'LayerLumos'
-copyright = '2024, Mingxuan Li'
-author = 'Mingxuan Li'
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = [
-    'nbsphinx',
-    'sphinx.ext.mathjax',  # If you have mathematical content
-    'sphinx.ext.autodoc',
-    # Other extensions here
-]
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-html_theme = 'alabaster'
-html_static_path = ['_static']
+import os
+import sys
+sys.path.insert(0, os.path.abspath('../'))
+sys.path.insert(0, os.path.abspath('../examples'))
+
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
+
+project = 'LayerLumos'
+copyright = '2024, Mingxuan Li'
+author = 'Mingxuan Li'
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = [
+    'nbsphinx',
+    'myst_parser',
+    'sphinx.ext.mathjax',  # If you have mathematical content
+    # 'sphinx_sitemap',
+    'sphinx.ext.autodoc',
+    # Other extensions here
+]
+# site_url = 'https://mil152.github.io/LayerLumos/'
+templates_path = ['_templates']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+html_theme = 'alabaster'
+html_static_path = ['_static']
```

### Comparing `layerlumos-1.0.0/docs/examples/compare_res_lumerical.py` & `layerlumos-1.0.1/docs/examples/compare_res_lumerical.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import sys, os
-sys.path.append("C:\\Program Files\\Lumerical\\v241\\api\\python\\")
-sys.path.append("C:\\Program Files\\Lumerical\\v232\\api\\python\\")
-import lumapi
-import numpy as np
-from scipy.constants import c
-import matplotlib.pyplot as plt
-
-fdtd = lumapi.FDTD(hide=True)
-wavelengths = np.linspace(300e-9, 900e-9, 50)  # 100 points from 300nm to 700nm
-frequencies = c / wavelengths  # Convert wavelengths to frequencies
-
-layer_materials = ['Air', 'TiO2 (Titanium Dioxide) - Siefke', 'Air']
-layer_thicknesses = np.array([0, 20e-9, 0])
-num_layers = len(layer_materials)
-num_freqs = len(frequencies)
-n_matrix = np.zeros((num_layers, num_freqs), dtype=np.complex128)
-for i, material_name in enumerate(layer_materials):
-    if material_name == 'Air':
-        n_matrix[i, :] = 1
-    else:
-        n_complex = fdtd.getindex(str(material_name), frequencies)
-        n_matrix[i, :] = n_complex[:, 0]
-theta = np.linspace(0, 89, 90)
-RT_lumerical = fdtd.stackrt(n_matrix, layer_thicknesses, frequencies, theta)
-
-R_Lumercal = (RT_lumerical['Rp'] + RT_lumerical['Rs']) / 2
-T_Lumercal = (RT_lumerical['Tp'] + RT_lumerical['Ts']) / 2
-
-wavelengths_nm = wavelengths * 1e9
-
-# Assuming 'theta' represents incidence angles in degrees
-
-# Create the plots
-fig, ax = plt.subplots(figsize=(10, 6))
-
-# Reflectance heatmap
-# The 'extent' argument defines the data bounds for the axes: [x_min, x_max, y_min, y_max]
-refl = ax.imshow(T_Lumercal.T, extent=(wavelengths_nm.min(), wavelengths_nm.max(), theta.min(), theta.max()), 
-                 origin='lower', aspect='auto', cmap='viridis')
-ax.set_title('Transmittance')
-ax.set_ylabel('Incidence Angle (degrees)')
-ax.set_xlabel('Wavelength (nm)')
-fig.colorbar(refl, ax=ax, label='Transmittance')
-
-plt.tight_layout()
+import sys, os
+sys.path.append("C:\\Program Files\\Lumerical\\v241\\api\\python\\")
+sys.path.append("C:\\Program Files\\Lumerical\\v232\\api\\python\\")
+import lumapi
+import numpy as np
+from scipy.constants import c
+import matplotlib.pyplot as plt
+
+fdtd = lumapi.FDTD(hide=True)
+wavelengths = np.linspace(300e-9, 900e-9, 50)  # 100 points from 300nm to 700nm
+frequencies = c / wavelengths  # Convert wavelengths to frequencies
+
+layer_materials = ['Air', 'TiO2 (Titanium Dioxide) - Siefke', 'Air']
+layer_thicknesses = np.array([0, 20e-9, 0])
+num_layers = len(layer_materials)
+num_freqs = len(frequencies)
+n_matrix = np.zeros((num_layers, num_freqs), dtype=np.complex128)
+for i, material_name in enumerate(layer_materials):
+    if material_name == 'Air':
+        n_matrix[i, :] = 1
+    else:
+        n_complex = fdtd.getindex(str(material_name), frequencies)
+        n_matrix[i, :] = n_complex[:, 0]
+theta = np.linspace(0, 89, 90)
+RT_lumerical = fdtd.stackrt(n_matrix, layer_thicknesses, frequencies, theta)
+
+R_Lumercal = (RT_lumerical['Rp'] + RT_lumerical['Rs']) / 2
+T_Lumercal = (RT_lumerical['Tp'] + RT_lumerical['Ts']) / 2
+
+wavelengths_nm = wavelengths * 1e9
+
+# Assuming 'theta' represents incidence angles in degrees
+
+# Create the plots
+fig, ax = plt.subplots(figsize=(10, 6))
+
+# Reflectance heatmap
+# The 'extent' argument defines the data bounds for the axes: [x_min, x_max, y_min, y_max]
+refl = ax.imshow(T_Lumercal.T, extent=(wavelengths_nm.min(), wavelengths_nm.max(), theta.min(), theta.max()), 
+                 origin='lower', aspect='auto', cmap='viridis')
+ax.set_title('Transmittance')
+ax.set_ylabel('Incidence Angle (degrees)')
+ax.set_xlabel('Wavelength (nm)')
+fig.colorbar(refl, ax=ax, label='Transmittance')
+
+plt.tight_layout()
 plt.show()
```

### Comparing `layerlumos-1.0.0/docs/examples/time_compare_lumerical.py` & `layerlumos-1.0.1/docs/examples/time_compare_lumerical.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-import timeit
-
-# Define the setup code (import statements, variable definitions, etc.)
-setup_code1 = '''
-import numpy as np
-from scipy.constants import c
-from layerlumos.utils import load_material, interpolate_material
-from layerlumos.layerlumos import stackrt, stackrt0
-import numpy as np
-'''
-
-setup_code2 = '''
-import sys, os
-import lumapi
-import numpy as np
-from scipy.constants import c
-'''
-
-# Define the code snippets to be tested
-code_snippet1 = '''
-si02_data = load_material('SiO2')
-
-# Define wavelength range (in meters)
-wavelengths = np.linspace(300e-9, 900e-9, 50)  # 100 points from 300nm to 700nm
-frequencies = c / wavelengths  # Convert wavelengths to frequencies
-
-# Interpolate n and k values for SiO2 over the specified frequency range
-n_k_si02 = interpolate_material(si02_data, frequencies)
-n_si02 = n_k_si02[:, 0] + 1j*n_k_si02[:, 1]  # Combine n and k into a complex refractive index
-
-# Define stack configuration
-n_air = np.ones_like(wavelengths)  # Refractive index of air is approximately 1
-d_air = np.array([0])
-d_si02 = np.array([2e-6])  # Thickness of SiO2 layer in meters (e.g., 2 microns)
-
-# Stack refractive indices and thicknesses for air-SiO2-air
-n_stack = np.vstack([n_air, n_si02, n_air]).T  # Transpose to match expected shape (Nlayers x Nfreq)
-d_stack = np.vstack([d_air, d_si02, d_air])  # No frequency dependence on thickness
-thetas = np.linspace(0, 89, 90)
-# Calculate R and T over the frequency (wavelength) range
-R_TE, T_TE, R_TM, T_TM = stackrt(n_stack, d_stack, frequencies, thetas)
-
-'''
-
-code_snippet2 = '''
-
-fdtd = lumapi.FDTD(hide=True)
-wavelengths = np.linspace(300e-9, 900e-9, 50)  # 100 points from 300nm to 700nm
-frequencies = c / wavelengths  # Convert wavelengths to frequencies
-
-layer_materials = ['Air', 'SiO2 (Glass) - Palik', 'Air']
-layer_thicknesses = np.array([0, 2e-6, 0])
-num_layers = len(layer_materials)
-num_freqs = len(frequencies)
-n_matrix = np.zeros((num_layers, num_freqs), dtype=np.complex128)
-for i, material_name in enumerate(layer_materials):
-    if material_name == 'Air':
-        n_matrix[i, :] = 1
-    else:
-        n_complex = fdtd.getindex(str(material_name), frequencies)
-        n_matrix[i, :] = n_complex[:, 0]
-theta = np.linspace(0, 89, 90)
-RT = fdtd.stackrt(n_matrix, layer_thicknesses, frequencies, theta)
-'''
-
-# Run timeit
-time1 = timeit.timeit(stmt=code_snippet1, setup=setup_code1, number=10)
-time2 = timeit.timeit(stmt=code_snippet2, setup=setup_code2, number=10)
-
-print(f"Code snippet 1 execution time: {time1}")
-print(f"Code snippet 2 execution time: {time2}")
+import timeit
+
+# Define the setup code (import statements, variable definitions, etc.)
+setup_code1 = '''
+import numpy as np
+from scipy.constants import c
+from layerlumos.utils import load_material, interpolate_material
+from layerlumos.layerlumos import stackrt, stackrt0
+import numpy as np
+'''
+
+setup_code2 = '''
+import sys, os
+import lumapi
+import numpy as np
+from scipy.constants import c
+'''
+
+# Define the code snippets to be tested
+code_snippet1 = '''
+si02_data = load_material('SiO2')
+
+# Define wavelength range (in meters)
+wavelengths = np.linspace(300e-9, 900e-9, 50)  # 100 points from 300nm to 700nm
+frequencies = c / wavelengths  # Convert wavelengths to frequencies
+
+# Interpolate n and k values for SiO2 over the specified frequency range
+n_k_si02 = interpolate_material(si02_data, frequencies)
+n_si02 = n_k_si02[:, 0] + 1j*n_k_si02[:, 1]  # Combine n and k into a complex refractive index
+
+# Define stack configuration
+n_air = np.ones_like(wavelengths)  # Refractive index of air is approximately 1
+d_air = np.array([0])
+d_si02 = np.array([2e-6])  # Thickness of SiO2 layer in meters (e.g., 2 microns)
+
+# Stack refractive indices and thicknesses for air-SiO2-air
+n_stack = np.vstack([n_air, n_si02, n_air]).T  # Transpose to match expected shape (Nlayers x Nfreq)
+d_stack = np.vstack([d_air, d_si02, d_air])  # No frequency dependence on thickness
+thetas = np.linspace(0, 89, 90)
+# Calculate R and T over the frequency (wavelength) range
+R_TE, T_TE, R_TM, T_TM = stackrt(n_stack, d_stack, frequencies, thetas)
+
+'''
+
+code_snippet2 = '''
+
+fdtd = lumapi.FDTD(hide=True)
+wavelengths = np.linspace(300e-9, 900e-9, 50)  # 100 points from 300nm to 700nm
+frequencies = c / wavelengths  # Convert wavelengths to frequencies
+
+layer_materials = ['Air', 'SiO2 (Glass) - Palik', 'Air']
+layer_thicknesses = np.array([0, 2e-6, 0])
+num_layers = len(layer_materials)
+num_freqs = len(frequencies)
+n_matrix = np.zeros((num_layers, num_freqs), dtype=np.complex128)
+for i, material_name in enumerate(layer_materials):
+    if material_name == 'Air':
+        n_matrix[i, :] = 1
+    else:
+        n_complex = fdtd.getindex(str(material_name), frequencies)
+        n_matrix[i, :] = n_complex[:, 0]
+theta = np.linspace(0, 89, 90)
+RT = fdtd.stackrt(n_matrix, layer_thicknesses, frequencies, theta)
+'''
+
+# Run timeit
+time1 = timeit.timeit(stmt=code_snippet1, setup=setup_code1, number=10)
+time2 = timeit.timeit(stmt=code_snippet2, setup=setup_code2, number=10)
+
+print(f"Code snippet 1 execution time: {time1}")
+print(f"Code snippet 2 execution time: {time2}")
```

### Comparing `layerlumos-1.0.0/docs/getting-started.md` & `layerlumos-1.0.1/docs/getting-started.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# Frequently Asked Questions (FAQ)
-
-## Installation and Setup
-
-### How do I install LayerLumos?
-
-LayerLumos can be installed by cloning our GitHub repository and following the setup instructions in the README. Ensure you have the necessary dependencies installed before running the software.
-
-### What are the system requirements for LayerLumos?
-
-LayerLumos requires Python 3.6 or higher and works on Windows, macOS, and Linux. Specific library dependencies are listed in the `requirements.txt` file.
-
-## Usage
-
-### How do I perform a basic RT calculation?
-
-After installing LayerLumos, you can perform a basic RT calculation by running the provided example scripts or by using the LayerLumos API in your Python scripts. Check the Quick Start Guide in the README for more details.
-
-### Can LayerLumos simulate RT for any angle of incidence?
-
-Yes, LayerLumos supports simulations for any angle of incidence. Users can specify the angle in the simulation parameters.
-
-### How do I add new materials to the material database?
-
-To add a new material, you can edit the `materials.json` file and include the optical properties of your material. Please refer to the documentation for the required data format.
-
-## Troubleshooting
-
-### I'm getting an error when trying to run a simulation. What should I do?
-
-Ensure that all dependencies are correctly installed and that your Python environment is set up properly. Check the error message for hints on what might be wrong. If the problem persists, please file an issue on our GitHub page with details of the error.
-
-### The simulation results seem off. How can I verify them?
-
-Double-check the input parameters for your simulation, including material indices, layer thicknesses, and frequency vector. Compare your results with known values or simpler cases to verify accuracy.
-
-## Contribution and Support
-
-### How can I contribute to LayerLumos?
-
-We welcome contributions in the form of bug reports, feature requests, and pull requests. Please refer to our CONTRIBUTING.md file for guidelines on how to contribute.
-
-### Where can I ask questions or seek support?
-
-If you have questions or need support, you can open an issue on our GitHub repository or contact us via the details provided in the README. We also have a community forum (if applicable) where you can seek help from other users.
+# Frequently Asked Questions (FAQ)
+
+## Installation and Setup
+
+### How do I install LayerLumos?
+
+LayerLumos can be installed by cloning our GitHub repository and following the setup instructions in the README. Ensure you have the necessary dependencies installed before running the software.
+
+### What are the system requirements for LayerLumos?
+
+LayerLumos requires Python 3.6 or higher and works on Windows, macOS, and Linux. Specific library dependencies are listed in the `requirements.txt` file.
+
+## Usage
+
+### How do I perform a basic RT calculation?
+
+After installing LayerLumos, you can perform a basic RT calculation by running the provided example scripts or by using the LayerLumos API in your Python scripts. Check the Quick Start Guide in the README for more details.
+
+### Can LayerLumos simulate RT for any angle of incidence?
+
+Yes, LayerLumos supports simulations for any angle of incidence. Users can specify the angle in the simulation parameters.
+
+### How do I add new materials to the material database?
+
+To add a new material, you can edit the `materials.json` file and include the optical properties of your material. Please refer to the documentation for the required data format.
+
+## Troubleshooting
+
+### I'm getting an error when trying to run a simulation. What should I do?
+
+Ensure that all dependencies are correctly installed and that your Python environment is set up properly. Check the error message for hints on what might be wrong. If the problem persists, please file an issue on our GitHub page with details of the error.
+
+### The simulation results seem off. How can I verify them?
+
+Double-check the input parameters for your simulation, including material indices, layer thicknesses, and frequency vector. Compare your results with known values or simpler cases to verify accuracy.
+
+## Contribution and Support
+
+### How can I contribute to LayerLumos?
+
+We welcome contributions in the form of bug reports, feature requests, and pull requests. Please refer to our CONTRIBUTING.md file for guidelines on how to contribute.
+
+### Where can I ask questions or seek support?
+
+If you have questions or need support, you can open an issue on our GitHub repository or contact us via the details provided in the README. We also have a community forum (if applicable) where you can seek help from other users.
```

### Comparing `layerlumos-1.0.0/docs/index.md` & `layerlumos-1.0.1/docs/home.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,39 @@
----
-layout: page
-title: "Home"
-permalink: /
----
-
-# Welcome to LayerLumos Documentation
-
-## Introduction
-
-**LayerLumos** is an innovative open-source tool designed to revolutionize optical simulations. It enables precise calculations of light reflection and transmission through multi-layer structures for both academic and commercial users. Tailored for the optics and photonics community, LayerLumos combines efficiency, flexibility, and ease of use in a powerful simulation package.
-
-## Key Features
-
-- **High Performance**: Built for speed, LayerLumos delivers rapid simulations, enabling you to focus on innovation and design.
-- **Versatility in Simulations**: Offers extensive customization options through detailed material databases, varied layer thicknesses, and comprehensive frequency vectors.
-- **Angle of Incidence Calculations**: Enhances analysis with the ability to simulate light interaction at different incidence angles.
-- **Open-Source Excellence**: As a community-driven project, we welcome contributions and aim to foster a collaborative environment for development.
-- **Rich Material Library**: Access an expansive collection of materials and their optical properties to streamline your simulation setups.
-
-## Getting Started
-
-To get started with LayerLumos, follow these simple steps:
-
-1. **Installation Guide**: Check out our step-by-step instructions for setting up LayerLumos on your system.
-2. **Quick Start Tutorial**: Dive into your first light interaction simulation with our beginner-friendly guide.
-3. **Explore Examples**: Learn from a curated selection of examples that demonstrate the versatility and capabilities of LayerLumos.
-For more detailed information on our API, see our [API documentation](API_Documentation.md).
-
-## Contribute
-
-Join our growing community of developers and researchers by contributing to LayerLumos. Your feedback, suggestions, and contributions are valuable to us. Together, we can make LayerLumos even better.
-
-## License
-
-LayerLumos is proudly released under the [MIT License](https://github.com/Mil152/LayerLumos/blob/main/LICENSE). We support open innovation and encourage the use and modification of our software for a wide range of applications.
-
-## Support and Feedback
-
-Encountered an issue or have a question? Our community is here to help. Please feel free to [submit an issue](https://github.com/Mil152/LayerLumos/issues) or reach out for support. We're committed to providing assistance and improving LayerLumos for everyone.
-
-## Acknowledgments
-
-A special thank you to all contributors, users, and supporters of LayerLumos. Your engagement and feedback drive the continuous improvement and success of this project.
-
+# Welcome to LayerLumos Documentation
+
+## Introduction
+
+**LayerLumos** is an innovative open-source tool designed to revolutionize optical simulations. It enables precise calculations of light reflection and transmission through multi-layer structures for both academic and commercial users. Tailored for the optics and photonics community, LayerLumos combines efficiency, flexibility, and ease of use in a powerful simulation package.
+
+## Key Features
+
+- **High Performance**: Built for speed, LayerLumos delivers rapid simulations, enabling you to focus on innovation and design.
+- **Versatility in Simulations**: Offers extensive customization options through detailed material databases, varied layer thicknesses, and comprehensive frequency vectors.
+- **Angle of Incidence Calculations**: Enhances analysis with the ability to simulate light interaction at different incidence angles.
+- **Open-Source Excellence**: As a community-driven project, we welcome contributions and aim to foster a collaborative environment for development.
+- **Rich Material Library**: Access an expansive collection of materials and their optical properties to streamline your simulation setups.
+
+## Getting Started
+
+To get started with LayerLumos, follow these simple steps:
+
+1. **Installation Guide**: Check out our step-by-step instructions for setting up LayerLumos on your system.
+2. **Quick Start Tutorial**: Dive into your first light interaction simulation with our beginner-friendly guide.
+3. **Explore Examples**: Learn from a curated selection of examples that demonstrate the versatility and capabilities of LayerLumos.
+For more detailed information on our API, see our [API documentation](https://mil152.github.io/LayerLumos/modules.html).
+
+## Contribute
+
+Join our growing community of developers and researchers by contributing to LayerLumos. Your feedback, suggestions, and contributions are valuable to us. Together, we can make LayerLumos even better.
+
+## License
+
+LayerLumos is proudly released under the [MIT License](https://github.com/Mil152/LayerLumos/blob/main/LICENSE). We support open innovation and encourage the use and modification of our software for a wide range of applications.
+
+## Support and Feedback
+
+Encountered an issue or have a question? Our community is here to help. Please feel free to [submit an issue](https://github.com/Mil152/LayerLumos/issues) or reach out for support. We're committed to providing assistance and improving LayerLumos for everyone.
+
+## Acknowledgments
+
+A special thank you to all contributors, users, and supporters of LayerLumos. Your engagement and feedback drive the continuous improvement and success of this project.
+
```

### Comparing `layerlumos-1.0.0/docs/index.rst` & `layerlumos-1.0.1/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-.. LayerLumos documentation master file, created by
-   sphinx-quickstart on Fri Mar 15 18:08:05 2024.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-Welcome to LayerLumos's documentation!
-======================================
-LayerLumos is a lightweight, efficient TMM library designed to accelerate your optical simulations, offering a wide range of tools and functionalities.
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-
-   modules
-   examples
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+.. LayerLumos documentation master file, created by
+   sphinx-quickstart on Fri Mar 15 18:08:05 2024.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+Welcome to LayerLumos's documentation!
+======================================
+LayerLumos is a lightweight, efficient TMM library designed to accelerate your optical simulations, offering a wide range of tools and functionalities.
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Contents:
+
+   home
+   getting-started
+   modules
+   examples
+
+Indices and tables
+==================
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
```

### Comparing `layerlumos-1.0.0/docs/make.bat` & `layerlumos-1.0.1/docs/make.bat`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `layerlumos-1.0.0/layerlumos/materials/Al_Rakic.csv` & `layerlumos-1.0.1/layerlumos/materials/Al_Rakic.csv`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,207 +1,207 @@
-wl,n,k
-0.00012399,0.9999946,8.241E-08
-0.00013051,0.999994,1.272E-07
-0.00013776,0.999993,1.2488E-07
-0.00015498,0.999991,1.9173E-07
-0.00017712,0.999989,3.1463E-07
-0.00020664,0.999984,5.5102E-07
-0.00024797,0.99998,1.0726E-06
-0.00030996,0.99997,2.4843E-06
-0.00035424,0.99995,4.0484E-06
-0.00041328,0.99994,7.1408E-06
-0.00049594,0.99991,0.000013642
-0.00061993,0.99987,0.000032079
-0.00065255,0.99986,0.000038497
-0.00068881,0.99985,0.000047138
-0.00072932,0.99984,0.000057974
-0.00074021,0.99984,0.000061633
-0.00077734,0.99986,0.000074862
-0.00078472,0.99987,0.00007848
-0.00079274,0.9999,0.000085418
-0.00079376,0.99992,0.000071847
-0.00079478,0.99993,0.000049998
-0.00079529,0.99992,0.000041131
-0.0007958,0.99992,0.000032911
-0.00079785,0.99991,0.000023687
-0.00079887,0.99991,0.000011026
-0.0007999,0.99989,6.0484E-06
-0.0008051,0.99987,6.1901E-06
-0.00081569,0.99985,6.4818E-06
-0.00082657,0.99983,6.8049E-06
-0.00085507,0.99981,7.8422E-06
-0.00088561,0.99979,0.00000894
-0.00095373,0.99974,0.000011636
-0.0010332,0.99968,0.000015628
-0.0011271,0.99961,0.000021586
-0.0012399,0.99953,0.000031115
-0.0013776,0.9994,0.000046771
-0.0015498,0.99924,0.000072992
-0.0017712,0.99898,0.00011811
-0.0020664,0.9986,0.00022001
-0.0024797,0.99797,0.00043503
-0.0030996,0.99694,0.00096887
-0.0041328,0.9948,0.0023492
-0.0049594,0.99313,0.0041863
-0.0061993,0.99111,0.0075099
-0.0065255,0.99054,0.0084716
-0.0068881,0.99007,0.0096517
-0.0072932,0.98909,0.010987
-0.0077491,0.98912,0.013728
-0.0082657,0.98966,0.014773
-0.0085507,0.98934,0.015437
-0.0088561,0.98883,0.016304
-0.0091841,0.98793,0.017765
-0.0095373,0.98761,0.020606
-0.0099188,0.98941,0.023421
-0.010332,0.99139,0.024063
-0.010781,0.99233,0.024928
-0.011271,0.99415,0.025452
-0.011808,0.99285,0.024415
-0.012399,0.99123,0.02992
-0.012652,0.99265,0.033061
-0.012915,0.99652,0.035883
-0.01319,1.0012,0.035311
-0.013477,1.0041,0.033392
-0.013776,1.0058,0.030918
-0.014089,1.006,0.028956
-0.014417,1.0065,0.028232
-0.01476,1.0074,0.026826
-0.01512,1.0077,0.02546
-0.015498,1.0075,0.024476
-0.015694,1.0075,0.024501
-0.015896,1.0078,0.024757
-0.016102,1.0095,0.02518
-0.016314,1.0106,0.023853
-0.016422,1.011,0.023955
-0.016531,1.0118,0.02402
-0.016642,1.0132,0.024343
-0.016755,1.0151,0.024184
-0.016777,1.0156,0.024228
-0.0168,1.0161,0.024282
-0.016823,1.0167,0.024375
-0.016846,1.0173,0.024499
-0.016869,1.0181,0.024831
-0.016892,1.0194,0.025432
-0.016915,1.0219,0.026018
-0.016938,1.0259,0.024227
-0.016961,1.0262,0.019564
-0.016984,1.0246,0.019145
-0.017008,1.0255,0.020012
-0.017031,1.0305,0.020072
-0.017054,1.0349,0.012476
-0.017078,1.0305,0.0041164
-0.017101,1.0249,0.0036218
-0.017125,1.0226,0.0034141
-0.017149,1.0206,0.00344
-0.017172,1.0192,0.0034767
-0.017196,1.0179,0.0034877
-0.017208,1.0174,0.0035108
-0.01722,1.0169,0.0035249
-0.017463,1.0108,0.0034957
-0.017712,1.007,0.0035425
-0.018233,1.0019,0.003673
-0.018786,0.99791,0.0038926
-0.019373,0.99457,0.0041092
-0.019998,0.99143,0.0042397
-0.020664,0.98827,0.0043696
-0.022543,0.97998,0.0050004
-0.024797,0.97048,0.0057469
-0.027552,0.95834,0.0066191
-0.030996,0.94189,0.0078466
-0.035424,0.91802,0.0093121
-0.041328,0.88013,0.011651
-0.049594,0.81512,0.015894
-0.061993,0.67912,0.02234
-0.065255,0.63242,0.02477
-0.068881,0.57251,0.027681
-0.072932,0.49131,0.032409
-0.077491,0.37197,0.044202
-0.078472,0.34031,0.04832
-0.079478,0.30373,0.053349
-0.07999,0.28271,0.056697
-0.08051,0.25936,0.061407
-0.081036,0.23344,0.068348
-0.081569,0.20569,0.079959
-0.082109,0.17943,0.094223
-0.082657,0.15065,0.11041
-0.083774,0.094517,0.16589
-0.084921,0.067041,0.2342
-0.086101,0.054863,0.29293
-0.088561,0.044168,0.39115
-0.095373,0.036437,0.59086
-0.10332,0.035753,0.77163
-0.11271,0.038468,0.95677
-0.12399,0.046304,1.1555
-0.13776,0.057167,1.3775
-0.15498,0.072505,1.6366
-0.17712,0.094236,1.9519
-0.20664,0.12677,2.3563
-0.24797,0.18137,2.9029
-0.30996,0.28003,3.7081
-0.32628,0.31474,3.9165
-0.36466,0.39877,4.3957
-0.41328,0.52135,5.0008
-0.4428,0.6079,5.3676
-0.47687,0.7278,5.7781
-0.5166,0.8734,6.2418
-0.56357,1.0728,6.7839
-0.61993,1.366,7.4052
-0.65225,1.5724,7.7354
-0.68881,1.8301,8.0601
-0.72932,2.1606,8.3565
-0.77491,2.6154,8.4914
-0.79478,2.7675,8.3866
-0.81569,2.7668,8.2573
-0.83774,2.6945,8.1878
-0.88561,2.2802,8.1134
-0.91166,1.9739,8.3058
-0.93928,1.6784,8.597
-0.96863,1.4867,9.0655
-0.99988,1.4359,9.4939
-1.0332,1.3998,9.8914
-1.1271,1.3281,10.969
-1.2399,1.3157,12.245
-1.3776,1.3899,13.784
-1.5498,1.5782,15.656
-1.7712,1.9205,17.991
-2.0664,2.4738,20.982
-2.4797,3.3372,25.004
-2.7552,3.938,27.58
-3.0996,4.7097,30.737
-3.2628,5.0735,32.183
-3.444,5.4903,33.814
-3.6466,5.9564,35.608
-3.8745,6.4808,37.595
-4.1328,7.0796,39.826
-4.428,7.7757,42.367
-4.7687,8.5881,45.257
-5.166,9.558,48.593
-5.6357,10.742,52.518
-6.1993,12.195,57.156
-6.8881,14.088,62.841
-7.7491,16.755,69.857
-8.8561,20.837,78.274
-10.332,26.216,88.197
-12.399,33.519,101.28
-13.776,38.461,108.96
-15.498,43.775,118.39
-17.712,50.951,129.49
-19.075,54.413,136.09
-20.664,58.58,144.23
-22.543,63.554,153.45
-24.797,68.535,164.81
-27.552,75.748,181.78
-30.996,91.955,199.99
-33.333,102.1,208.1
-40,125.14,230.19
-44.444,140.05,243.43
-50,157.3,258.26
-57.144,177.93,275.34
-66.666,202.63,295.42
-80.001,233.56,321.08
-99.996,274.38,354.35
-125,318.81,391.71
-137.76,339.62,408.92
-153.85,364.04,429.62
-177.12,397.93,458.5
-200,423.96,483.7
+wl,n,k
+0.00012399,0.9999946,8.241E-08
+0.00013051,0.999994,1.272E-07
+0.00013776,0.999993,1.2488E-07
+0.00015498,0.999991,1.9173E-07
+0.00017712,0.999989,3.1463E-07
+0.00020664,0.999984,5.5102E-07
+0.00024797,0.99998,1.0726E-06
+0.00030996,0.99997,2.4843E-06
+0.00035424,0.99995,4.0484E-06
+0.00041328,0.99994,7.1408E-06
+0.00049594,0.99991,0.000013642
+0.00061993,0.99987,0.000032079
+0.00065255,0.99986,0.000038497
+0.00068881,0.99985,0.000047138
+0.00072932,0.99984,0.000057974
+0.00074021,0.99984,0.000061633
+0.00077734,0.99986,0.000074862
+0.00078472,0.99987,0.00007848
+0.00079274,0.9999,0.000085418
+0.00079376,0.99992,0.000071847
+0.00079478,0.99993,0.000049998
+0.00079529,0.99992,0.000041131
+0.0007958,0.99992,0.000032911
+0.00079785,0.99991,0.000023687
+0.00079887,0.99991,0.000011026
+0.0007999,0.99989,6.0484E-06
+0.0008051,0.99987,6.1901E-06
+0.00081569,0.99985,6.4818E-06
+0.00082657,0.99983,6.8049E-06
+0.00085507,0.99981,7.8422E-06
+0.00088561,0.99979,0.00000894
+0.00095373,0.99974,0.000011636
+0.0010332,0.99968,0.000015628
+0.0011271,0.99961,0.000021586
+0.0012399,0.99953,0.000031115
+0.0013776,0.9994,0.000046771
+0.0015498,0.99924,0.000072992
+0.0017712,0.99898,0.00011811
+0.0020664,0.9986,0.00022001
+0.0024797,0.99797,0.00043503
+0.0030996,0.99694,0.00096887
+0.0041328,0.9948,0.0023492
+0.0049594,0.99313,0.0041863
+0.0061993,0.99111,0.0075099
+0.0065255,0.99054,0.0084716
+0.0068881,0.99007,0.0096517
+0.0072932,0.98909,0.010987
+0.0077491,0.98912,0.013728
+0.0082657,0.98966,0.014773
+0.0085507,0.98934,0.015437
+0.0088561,0.98883,0.016304
+0.0091841,0.98793,0.017765
+0.0095373,0.98761,0.020606
+0.0099188,0.98941,0.023421
+0.010332,0.99139,0.024063
+0.010781,0.99233,0.024928
+0.011271,0.99415,0.025452
+0.011808,0.99285,0.024415
+0.012399,0.99123,0.02992
+0.012652,0.99265,0.033061
+0.012915,0.99652,0.035883
+0.01319,1.0012,0.035311
+0.013477,1.0041,0.033392
+0.013776,1.0058,0.030918
+0.014089,1.006,0.028956
+0.014417,1.0065,0.028232
+0.01476,1.0074,0.026826
+0.01512,1.0077,0.02546
+0.015498,1.0075,0.024476
+0.015694,1.0075,0.024501
+0.015896,1.0078,0.024757
+0.016102,1.0095,0.02518
+0.016314,1.0106,0.023853
+0.016422,1.011,0.023955
+0.016531,1.0118,0.02402
+0.016642,1.0132,0.024343
+0.016755,1.0151,0.024184
+0.016777,1.0156,0.024228
+0.0168,1.0161,0.024282
+0.016823,1.0167,0.024375
+0.016846,1.0173,0.024499
+0.016869,1.0181,0.024831
+0.016892,1.0194,0.025432
+0.016915,1.0219,0.026018
+0.016938,1.0259,0.024227
+0.016961,1.0262,0.019564
+0.016984,1.0246,0.019145
+0.017008,1.0255,0.020012
+0.017031,1.0305,0.020072
+0.017054,1.0349,0.012476
+0.017078,1.0305,0.0041164
+0.017101,1.0249,0.0036218
+0.017125,1.0226,0.0034141
+0.017149,1.0206,0.00344
+0.017172,1.0192,0.0034767
+0.017196,1.0179,0.0034877
+0.017208,1.0174,0.0035108
+0.01722,1.0169,0.0035249
+0.017463,1.0108,0.0034957
+0.017712,1.007,0.0035425
+0.018233,1.0019,0.003673
+0.018786,0.99791,0.0038926
+0.019373,0.99457,0.0041092
+0.019998,0.99143,0.0042397
+0.020664,0.98827,0.0043696
+0.022543,0.97998,0.0050004
+0.024797,0.97048,0.0057469
+0.027552,0.95834,0.0066191
+0.030996,0.94189,0.0078466
+0.035424,0.91802,0.0093121
+0.041328,0.88013,0.011651
+0.049594,0.81512,0.015894
+0.061993,0.67912,0.02234
+0.065255,0.63242,0.02477
+0.068881,0.57251,0.027681
+0.072932,0.49131,0.032409
+0.077491,0.37197,0.044202
+0.078472,0.34031,0.04832
+0.079478,0.30373,0.053349
+0.07999,0.28271,0.056697
+0.08051,0.25936,0.061407
+0.081036,0.23344,0.068348
+0.081569,0.20569,0.079959
+0.082109,0.17943,0.094223
+0.082657,0.15065,0.11041
+0.083774,0.094517,0.16589
+0.084921,0.067041,0.2342
+0.086101,0.054863,0.29293
+0.088561,0.044168,0.39115
+0.095373,0.036437,0.59086
+0.10332,0.035753,0.77163
+0.11271,0.038468,0.95677
+0.12399,0.046304,1.1555
+0.13776,0.057167,1.3775
+0.15498,0.072505,1.6366
+0.17712,0.094236,1.9519
+0.20664,0.12677,2.3563
+0.24797,0.18137,2.9029
+0.30996,0.28003,3.7081
+0.32628,0.31474,3.9165
+0.36466,0.39877,4.3957
+0.41328,0.52135,5.0008
+0.4428,0.6079,5.3676
+0.47687,0.7278,5.7781
+0.5166,0.8734,6.2418
+0.56357,1.0728,6.7839
+0.61993,1.366,7.4052
+0.65225,1.5724,7.7354
+0.68881,1.8301,8.0601
+0.72932,2.1606,8.3565
+0.77491,2.6154,8.4914
+0.79478,2.7675,8.3866
+0.81569,2.7668,8.2573
+0.83774,2.6945,8.1878
+0.88561,2.2802,8.1134
+0.91166,1.9739,8.3058
+0.93928,1.6784,8.597
+0.96863,1.4867,9.0655
+0.99988,1.4359,9.4939
+1.0332,1.3998,9.8914
+1.1271,1.3281,10.969
+1.2399,1.3157,12.245
+1.3776,1.3899,13.784
+1.5498,1.5782,15.656
+1.7712,1.9205,17.991
+2.0664,2.4738,20.982
+2.4797,3.3372,25.004
+2.7552,3.938,27.58
+3.0996,4.7097,30.737
+3.2628,5.0735,32.183
+3.444,5.4903,33.814
+3.6466,5.9564,35.608
+3.8745,6.4808,37.595
+4.1328,7.0796,39.826
+4.428,7.7757,42.367
+4.7687,8.5881,45.257
+5.166,9.558,48.593
+5.6357,10.742,52.518
+6.1993,12.195,57.156
+6.8881,14.088,62.841
+7.7491,16.755,69.857
+8.8561,20.837,78.274
+10.332,26.216,88.197
+12.399,33.519,101.28
+13.776,38.461,108.96
+15.498,43.775,118.39
+17.712,50.951,129.49
+19.075,54.413,136.09
+20.664,58.58,144.23
+22.543,63.554,153.45
+24.797,68.535,164.81
+27.552,75.748,181.78
+30.996,91.955,199.99
+33.333,102.1,208.1
+40,125.14,230.19
+44.444,140.05,243.43
+50,157.3,258.26
+57.144,177.93,275.34
+66.666,202.63,295.42
+80.001,233.56,321.08
+99.996,274.38,354.35
+125,318.81,391.71
+137.76,339.62,408.92
+153.85,364.04,429.62
+177.12,397.93,458.5
+200,423.96,483.7
```

### Comparing `layerlumos-1.0.0/layerlumos/materials/TiN_Beliaev.csv` & `layerlumos-1.0.1/layerlumos/materials/TiN_Beliaev.csv`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,1177 +1,1177 @@
-wl,n,k
-0.2114,2.47401,1.97842
-0.21298,2.49873,1.94326
-0.21456,2.52109,1.91041
-0.21614,2.54137,1.87953
-0.21772,2.55979,1.85035
-0.2193,2.57656,1.82264
-0.22089,2.59185,1.79624
-0.22247,2.60579,1.77099
-0.22405,2.61852,1.74678
-0.22563,2.63013,1.7235
-0.22721,2.64071,1.70106
-0.2288,2.65035,1.67941
-0.23038,2.65913,1.65846
-0.23196,2.66709,1.63817
-0.23354,2.67429,1.61849
-0.23513,2.6808,1.59939
-0.23671,2.68664,1.58081
-0.23829,2.69186,1.56275
-0.23987,2.69651,1.54515
-0.24146,2.7006,1.52801
-0.24304,2.70417,1.5113
-0.24462,2.70726,1.495
-0.24621,2.70987,1.47908
-0.24779,2.71205,1.46354
-0.24937,2.7138,1.44837
-0.25096,2.71516,1.43353
-0.25254,2.71613,1.41903
-0.25412,2.71673,1.40485
-0.25571,2.71699,1.39099
-0.25729,2.71691,1.37742
-0.25887,2.71652,1.36414
-0.26046,2.71581,1.35115
-0.26204,2.71481,1.33844
-0.26363,2.71353,1.32599
-0.26521,2.71197,1.3138
-0.2668,2.71015,1.30187
-0.26838,2.70808,1.29018
-0.26996,2.70576,1.27874
-0.27155,2.70321,1.26753
-0.27313,2.70042,1.25656
-0.27472,2.69742,1.24581
-0.2763,2.6942,1.23528
-0.27789,2.69078,1.22496
-0.27947,2.68716,1.21486
-0.28106,2.68334,1.20497
-0.28264,2.67933,1.19528
-0.28423,2.67514,1.18579
-0.28581,2.67077,1.1765
-0.2874,2.66623,1.1674
-0.28898,2.66152,1.15849
-0.29057,2.65664,1.14977
-0.29215,2.6516,1.14123
-0.29374,2.64641,1.13286
-0.29533,2.64106,1.12468
-0.29691,2.63557,1.11667
-0.2985,2.62993,1.10883
-0.30008,2.62415,1.10117
-0.30167,2.61823,1.09367
-0.30325,2.61217,1.08633
-0.30484,2.60598,1.07915
-0.30643,2.59965,1.07214
-0.30801,2.5932,1.06528
-0.3096,2.58663,1.05858
-0.31119,2.57993,1.05203
-0.31277,2.5731,1.04564
-0.31436,2.56616,1.0394
-0.31595,2.55911,1.0333
-0.31753,2.55193,1.02735
-0.31912,2.54464,1.02155
-0.3207,2.53724,1.01589
-0.32229,2.52973,1.01037
-0.32388,2.52211,1.00499
-0.32547,2.51439,0.99976
-0.32705,2.50655,0.99466
-0.32864,2.49862,0.9897
-0.33023,2.49058,0.98487
-0.33181,2.48243,0.98018
-0.3334,2.47419,0.97563
-0.33499,2.46585,0.97121
-0.33658,2.4574,0.96692
-0.33816,2.44886,0.96276
-0.33975,2.44022,0.95873
-0.34134,2.43149,0.95484
-0.34292,2.42266,0.95107
-0.34451,2.41373,0.94743
-0.3461,2.40471,0.94392
-0.34769,2.3956,0.94053
-0.34928,2.3864,0.93728
-0.35086,2.3771,0.93415
-0.35245,2.36771,0.93114
-0.35404,2.35823,0.92827
-0.35563,2.34866,0.92552
-0.35721,2.339,0.92289
-0.3588,2.32925,0.92039
-0.36039,2.31942,0.91802
-0.36198,2.30949,0.91577
-0.36357,2.29948,0.91365
-0.36515,2.28937,0.91165
-0.36674,2.27919,0.90978
-0.36833,2.26891,0.90803
-0.36992,2.25855,0.90641
-0.37151,2.2481,0.90492
-0.3731,2.23756,0.90355
-0.37468,2.22694,0.90231
-0.37627,2.21624,0.9012
-0.37786,2.20545,0.90022
-0.37945,2.19457,0.89937
-0.38104,2.18361,0.89864
-0.38263,2.17257,0.89805
-0.38422,2.16144,0.89759
-0.38581,2.15023,0.89726
-0.38739,2.13893,0.89706
-0.38898,2.12756,0.89699
-0.39057,2.11609,0.89706
-0.39216,2.10455,0.89727
-0.39375,2.09293,0.89761
-0.39534,2.08122,0.89809
-0.39693,2.06943,0.89871
-0.39852,2.05756,0.89947
-0.40011,2.04562,0.90038
-0.40169,2.03359,0.90142
-0.40328,2.02148,0.90261
-0.40487,2.00929,0.90395
-0.40646,1.99703,0.90544
-0.40805,1.98469,0.90708
-0.40964,1.97227,0.90886
-0.41123,1.95977,0.91081
-0.41282,1.9472,0.9129
-0.41441,1.93456,0.91516
-0.416,1.92184,0.91757
-0.41759,1.90905,0.92015
-0.41918,1.89619,0.92289
-0.42077,1.88326,0.9258
-0.42235,1.87026,0.92887
-0.42394,1.8572,0.93212
-0.42553,1.84406,0.93553
-0.42712,1.83087,0.93913
-0.42871,1.81761,0.9429
-0.4303,1.80429,0.94685
-0.43189,1.79091,0.95099
-0.43348,1.77748,0.95531
-0.43507,1.76399,0.95982
-0.43666,1.75045,0.96453
-0.43825,1.73686,0.96942
-0.43984,1.72322,0.97452
-0.44143,1.70954,0.97981
-0.44302,1.69582,0.9853
-0.44461,1.68206,0.991
-0.4462,1.66827,0.99691
-0.44779,1.65445,1.00303
-0.44938,1.6406,1.00936
-0.45097,1.62673,1.01591
-0.45256,1.61284,1.02267
-0.45415,1.59893,1.02965
-0.45574,1.58502,1.03686
-0.45733,1.5711,1.04429
-0.45892,1.55718,1.05195
-0.46051,1.54327,1.05983
-0.4621,1.52937,1.06795
-0.46369,1.51549,1.07629
-0.46528,1.50162,1.08487
-0.46687,1.48779,1.09368
-0.46846,1.47399,1.10273
-0.47005,1.46024,1.11201
-0.47164,1.44653,1.12153
-0.47323,1.43287,1.13129
-0.47482,1.41927,1.14128
-0.47641,1.40575,1.1515
-0.478,1.39229,1.16195
-0.47959,1.37892,1.17264
-0.48118,1.36563,1.18356
-0.48277,1.35244,1.19471
-0.48436,1.33936,1.20608
-0.48595,1.32638,1.21768
-0.48754,1.31351,1.2295
-0.48913,1.30077,1.24153
-0.49072,1.28815,1.25378
-0.49231,1.27567,1.26623
-0.4939,1.26333,1.27889
-0.49549,1.25113,1.29175
-0.49708,1.23909,1.3048
-0.49867,1.2272,1.31804
-0.50026,1.21548,1.33146
-0.50185,1.20392,1.34506
-0.50344,1.19254,1.35883
-0.50503,1.18132,1.37277
-0.50662,1.17029,1.38686
-0.50821,1.15944,1.40111
-0.5098,1.14877,1.4155
-0.51139,1.1383,1.43003
-0.51298,1.12801,1.44469
-0.51457,1.11791,1.45947
-0.51616,1.10801,1.47437
-0.51775,1.0983,1.48938
-0.51934,1.08878,1.5045
-0.52093,1.07947,1.51971
-0.52252,1.07034,1.53502
-0.52411,1.06142,1.5504
-0.52569,1.05269,1.56587
-0.52728,1.04415,1.58141
-0.52887,1.03581,1.59701
-0.53046,1.02766,1.61267
-0.53205,1.0197,1.62838
-0.53364,1.01193,1.64415
-0.53523,1.00434,1.65995
-0.53682,0.99695,1.6758
-0.53841,0.98974,1.69167
-0.54,0.9827,1.70757
-0.54159,0.97585,1.7235
-0.54318,0.96917,1.73945
-0.54477,0.96267,1.75541
-0.54636,0.95634,1.77138
-0.54795,0.95018,1.78736
-0.54954,0.94418,1.80334
-0.55113,0.93835,1.81932
-0.55272,0.93267,1.8353
-0.55431,0.92715,1.85128
-0.5559,0.92179,1.86724
-0.55749,0.91658,1.88319
-0.55908,0.91151,1.89913
-0.56067,0.90659,1.91505
-0.56226,0.90182,1.93095
-0.56385,0.89718,1.94684
-0.56544,0.89268,1.96269
-0.56703,0.88831,1.97853
-0.56861,0.88408,1.99434
-0.5702,0.87997,2.01012
-0.57179,0.87599,2.02587
-0.57338,0.87213,2.04159
-0.57497,0.86839,2.05728
-0.57656,0.86477,2.07293
-0.57815,0.86126,2.08855
-0.57974,0.85787,2.10414
-0.58133,0.85458,2.11969
-0.58292,0.85141,2.1352
-0.58451,0.84833,2.15068
-0.5861,0.84537,2.16611
-0.58768,0.8425,2.18151
-0.58927,0.83973,2.19687
-0.59086,0.83706,2.21219
-0.59245,0.83448,2.22746
-0.59404,0.83199,2.2427
-0.59563,0.82959,2.2579
-0.59722,0.82728,2.27305
-0.59881,0.82506,2.28817
-0.60039,0.82292,2.30324
-0.60198,0.82087,2.31827
-0.60357,0.81889,2.33326
-0.60516,0.817,2.3482
-0.60675,0.81518,2.3631
-0.60834,0.81343,2.37796
-0.60993,0.81176,2.39278
-0.61151,0.81016,2.40756
-0.6131,0.80864,2.42229
-0.61469,0.80718,2.43698
-0.61628,0.80579,2.45163
-0.61787,0.80447,2.46623
-0.61946,0.80321,2.4808
-0.62104,0.80202,2.49532
-0.62263,0.80088,2.5098
-0.62422,0.79981,2.52424
-0.62581,0.7988,2.53863
-0.6274,0.79785,2.55299
-0.62898,0.79695,2.5673
-0.63057,0.79611,2.58157
-0.63216,0.79533,2.5958
-0.63375,0.7946,2.60999
-0.63533,0.79392,2.62414
-0.63692,0.7933,2.63825
-0.63851,0.79273,2.65232
-0.6401,0.7922,2.66635
-0.64168,0.79173,2.68034
-0.64327,0.7913,2.69429
-0.64486,0.79092,2.70821
-0.64645,0.79059,2.72208
-0.64803,0.7903,2.73591
-0.64962,0.79005,2.74971
-0.65121,0.78985,2.76347
-0.6528,0.7897,2.77719
-0.65438,0.78958,2.79087
-0.65597,0.78951,2.80451
-0.65756,0.78947,2.81812
-0.65914,0.78948,2.83169
-0.66073,0.78953,2.84522
-0.66232,0.78961,2.85872
-0.6639,0.78973,2.87218
-0.66549,0.78989,2.88561
-0.66708,0.79008,2.899
-0.66866,0.79031,2.91235
-0.67025,0.79058,2.92567
-0.67184,0.79088,2.93895
-0.67342,0.79121,2.9522
-0.67501,0.79158,2.96542
-0.67659,0.79198,2.9786
-0.67818,0.79241,2.99175
-0.67977,0.79287,3.00486
-0.68135,0.79337,3.01794
-0.68294,0.79389,3.03099
-0.68452,0.79445,3.044
-0.68611,0.79504,3.05698
-0.6877,0.79565,3.06993
-0.68928,0.79629,3.08285
-0.69087,0.79696,3.09573
-0.69245,0.79766,3.10859
-0.69404,0.79839,3.12141
-0.69562,0.79914,3.1342
-0.69721,0.79992,3.14696
-0.69879,0.80073,3.15969
-0.70038,0.80156,3.17239
-0.70196,0.80241,3.18506
-0.70355,0.8033,3.19769
-0.70513,0.8042,3.2103
-0.70672,0.80513,3.22288
-0.7083,0.80608,3.23543
-0.70989,0.80706,3.24795
-0.71147,0.80806,3.26044
-0.71306,0.80908,3.2729
-0.71464,0.81013,3.28534
-0.71623,0.8112,3.29774
-0.71781,0.81228,3.31012
-0.7194,0.81339,3.32247
-0.72098,0.81452,3.33479
-0.72256,0.81568,3.34708
-0.72415,0.81685,3.35935
-0.72573,0.81804,3.37159
-0.72732,0.81925,3.3838
-0.7289,0.82049,3.39599
-0.73048,0.82174,3.40815
-0.73207,0.82301,3.42028
-0.73365,0.8243,3.43239
-0.73523,0.8256,3.44447
-0.73682,0.82693,3.45652
-0.7384,0.82828,3.46855
-0.73998,0.82964,3.48055
-0.74157,0.83102,3.49253
-0.74315,0.83241,3.50448
-0.74473,0.83383,3.51641
-0.74631,0.83526,3.52832
-0.7479,0.83671,3.54019
-0.74948,0.83817,3.55205
-0.75106,0.83965,3.56388
-0.75264,0.84115,3.57568
-0.75423,0.84266,3.58746
-0.75581,0.84419,3.59922
-0.75739,0.84573,3.61096
-0.75897,0.84729,3.62267
-0.76056,0.84886,3.63435
-0.76214,0.85045,3.64602
-0.76372,0.85205,3.65766
-0.7653,0.85367,3.66928
-0.76688,0.8553,3.68087
-0.76846,0.85694,3.69244
-0.77004,0.8586,3.70399
-0.77163,0.86028,3.71552
-0.77321,0.86196,3.72703
-0.77479,0.86366,3.73851
-0.77637,0.86538,3.74997
-0.77795,0.8671,3.76141
-0.77953,0.86884,3.77283
-0.78111,0.8706,3.78422
-0.78269,0.87236,3.7956
-0.78427,0.87414,3.80695
-0.78585,0.87593,3.81828
-0.78743,0.87773,3.82959
-0.78901,0.87954,3.84088
-0.79059,0.88137,3.85215
-0.79217,0.88321,3.8634
-0.79375,0.88506,3.87463
-0.79533,0.88692,3.88584
-0.79691,0.88879,3.89703
-0.79849,0.89067,3.90819
-0.80007,0.89257,3.91934
-0.80165,0.89447,3.93047
-0.80323,0.89639,3.94157
-0.80481,0.89832,3.95266
-0.80639,0.90026,3.96373
-0.80797,0.9022,3.97478
-0.80955,0.90416,3.98581
-0.81113,0.90613,3.99682
-0.8127,0.90811,4.00781
-0.81428,0.9101,4.01878
-0.81586,0.9121,4.02973
-0.81744,0.91411,4.04066
-0.81902,0.91613,4.05158
-0.82059,0.91816,4.06247
-0.82217,0.92019,4.07335
-0.82375,0.92224,4.08421
-0.82533,0.9243,4.09505
-0.82691,0.92636,4.10587
-0.82848,0.92844,4.11668
-0.83006,0.93052,4.12746
-0.83164,0.93262,4.13823
-0.83321,0.93472,4.14898
-0.83479,0.93683,4.15971
-0.83637,0.93895,4.17042
-0.83794,0.94108,4.18112
-0.83952,0.94321,4.1918
-0.8411,0.94536,4.20246
-0.84267,0.94751,4.2131
-0.84425,0.94967,4.22373
-0.84583,0.95184,4.23434
-0.8474,0.95402,4.24493
-0.84898,0.95621,4.2555
-0.85055,0.9584,4.26606
-0.85213,0.9606,4.2766
-0.8537,0.96281,4.28712
-0.85528,0.96503,4.29763
-0.85686,0.96726,4.30812
-0.85843,0.96949,4.31859
-0.86001,0.97173,4.32905
-0.86158,0.97397,4.33949
-0.86315,0.97623,4.34991
-0.86473,0.97849,4.36032
-0.8663,0.98076,4.37071
-0.86788,0.98304,4.38108
-0.86945,0.98532,4.39144
-0.87103,0.98761,4.40178
-0.8726,0.98991,4.4121
-0.87417,0.99221,4.42241
-0.87575,0.99452,4.43271
-0.87732,0.99684,4.44298
-0.87889,0.99916,4.45324
-0.88047,1.0015,4.46349
-0.88204,1.00383,4.47372
-0.88361,1.00618,4.48393
-0.88519,1.00853,4.49413
-0.88676,1.01088,4.50431
-0.88833,1.01325,4.51448
-0.8899,1.01562,4.52463
-0.89148,1.01799,4.53476
-0.89305,1.02038,4.54488
-0.89462,1.02276,4.55499
-0.89619,1.02516,4.56508
-0.89776,1.02756,4.57515
-0.89934,1.02997,4.58521
-0.90091,1.03238,4.59525
-0.90248,1.0348,4.60527
-0.90405,1.03722,4.61528
-0.90562,1.03965,4.62528
-0.90719,1.04209,4.63526
-0.90876,1.04453,4.64522
-0.91033,1.04698,4.65517
-0.9119,1.04943,4.6651
-0.91347,1.05189,4.67501
-0.91504,1.05435,4.68491
-0.91661,1.05682,4.69479
-0.91818,1.05928,4.70466
-0.91975,1.06176,4.71451
-0.92132,1.06423,4.72434
-0.92289,1.06671,4.73416
-0.92446,1.06919,4.74397
-0.92603,1.07168,4.75376
-0.9276,1.07417,4.76353
-0.92917,1.07666,4.77329
-0.93074,1.07915,4.78304
-0.9323,1.08165,4.79277
-0.93387,1.08415,4.80249
-0.93544,1.08666,4.8122
-0.93701,1.08916,4.82189
-0.93858,1.09167,4.83157
-0.94014,1.09419,4.84123
-0.94171,1.0967,4.85088
-0.94328,1.09922,4.86052
-0.94485,1.10174,4.87014
-0.94641,1.10426,4.87975
-0.94798,1.10679,4.88935
-0.94955,1.10932,4.89893
-0.95111,1.11185,4.90851
-0.95268,1.11438,4.91806
-0.95425,1.11692,4.92761
-0.95581,1.11946,4.93714
-0.95738,1.122,4.94666
-0.95894,1.12455,4.95617
-0.96051,1.12709,4.96567
-0.96207,1.12964,4.97515
-0.96364,1.1322,4.98462
-0.9652,1.13475,4.99408
-0.96677,1.13731,5.00353
-0.96833,1.13987,5.01296
-0.9699,1.14243,5.02238
-0.97146,1.14499,5.03179
-0.97303,1.14756,5.04119
-0.97459,1.15013,5.05058
-0.97616,1.1527,5.05995
-0.97772,1.15527,5.06931
-0.97928,1.15785,5.07866
-0.98085,1.16042,5.088
-0.98241,1.163,5.09733
-0.98397,1.16559,5.10665
-0.98554,1.16817,5.11595
-0.9871,1.17076,5.12524
-0.98866,1.17335,5.13452
-0.99022,1.17594,5.14379
-0.99179,1.17853,5.15305
-0.99335,1.18112,5.1623
-0.99491,1.18372,5.17154
-0.99647,1.18632,5.18076
-0.99803,1.18892,5.18998
-0.99959,1.19152,5.19918
-1.01061,1.20994,5.26381
-1.014,1.21565,5.28364
-1.0174,1.22136,5.30343
-1.0208,1.22708,5.32318
-1.02419,1.23282,5.34288
-1.02759,1.23856,5.36254
-1.03099,1.24431,5.38216
-1.03439,1.25008,5.40174
-1.03778,1.25585,5.42128
-1.04118,1.26163,5.44078
-1.04458,1.26743,5.46025
-1.04798,1.27323,5.47967
-1.05138,1.27904,5.49905
-1.05479,1.28486,5.51839
-1.05819,1.29069,5.5377
-1.06159,1.29653,5.55697
-1.06499,1.30238,5.5762
-1.06839,1.30824,5.59539
-1.0718,1.3141,5.61454
-1.0752,1.31997,5.63366
-1.0786,1.32586,5.65274
-1.08201,1.33175,5.67179
-1.08541,1.33764,5.6908
-1.08882,1.34355,5.70977
-1.09223,1.34946,5.72871
-1.09563,1.35538,5.74761
-1.09904,1.36131,5.76648
-1.10245,1.36725,5.78532
-1.10585,1.37319,5.80411
-1.10926,1.37914,5.82288
-1.11267,1.3851,5.84161
-1.11608,1.39107,5.86031
-1.11949,1.39704,5.87897
-1.1229,1.40302,5.8976
-1.12631,1.409,5.9162
-1.12972,1.41499,5.93476
-1.13313,1.42099,5.95329
-1.13654,1.427,5.97179
-1.13996,1.43301,5.99026
-1.14337,1.43903,6.00869
-1.14678,1.44505,6.0271
-1.1502,1.45108,6.04547
-1.15361,1.45712,6.06381
-1.15702,1.46316,6.08212
-1.16044,1.4692,6.10039
-1.16385,1.47526,6.11864
-1.16727,1.48131,6.13686
-1.17069,1.48738,6.15504
-1.1741,1.49345,6.1732
-1.17752,1.49952,6.19132
-1.18094,1.5056,6.20942
-1.18436,1.51168,6.22748
-1.18777,1.51777,6.24552
-1.19119,1.52387,6.26352
-1.19461,1.52997,6.2815
-1.19803,1.53607,6.29945
-1.20145,1.54218,6.31737
-1.20487,1.54829,6.33526
-1.20829,1.55441,6.35312
-1.21172,1.56053,6.37095
-1.21514,1.56666,6.38876
-1.21856,1.57279,6.40653
-1.22198,1.57892,6.42428
-1.22541,1.58506,6.442
-1.22883,1.5912,6.45969
-1.23225,1.59735,6.47736
-1.23568,1.6035,6.49499
-1.2391,1.60965,6.5126
-1.24253,1.61581,6.53019
-1.24596,1.62197,6.54774
-1.24938,1.62813,6.56527
-1.25281,1.6343,6.58277
-1.25624,1.64047,6.60025
-1.25966,1.64665,6.6177
-1.26309,1.65282,6.63512
-1.26652,1.659,6.65252
-1.26995,1.66519,6.66989
-1.27338,1.67137,6.68723
-1.27681,1.67756,6.70455
-1.28024,1.68376,6.72184
-1.28367,1.68995,6.73911
-1.2871,1.69615,6.75635
-1.29054,1.70235,6.77357
-1.29397,1.70855,6.79076
-1.2974,1.71476,6.80793
-1.30083,1.72096,6.82507
-1.30427,1.72717,6.84218
-1.3077,1.73339,6.85928
-1.31114,1.7396,6.87634
-1.31457,1.74582,6.89338
-1.31801,1.75203,6.9104
-1.32144,1.75825,6.9274
-1.32488,1.76448,6.94437
-1.32832,1.7707,6.96131
-1.33175,1.77693,6.97823
-1.33519,1.78315,6.99513
-1.33863,1.78938,7.012
-1.34207,1.79562,7.02885
-1.34551,1.80185,7.04568
-1.34895,1.80808,7.06248
-1.35239,1.81432,7.07926
-1.35583,1.82055,7.09602
-1.35927,1.82679,7.11275
-1.36271,1.83303,7.12946
-1.36615,1.83927,7.14615
-1.36959,1.84551,7.16281
-1.37303,1.85175,7.17946
-1.37648,1.858,7.19607
-1.37992,1.86424,7.21267
-1.38336,1.87049,7.22925
-1.38681,1.87673,7.2458
-1.39025,1.88298,7.26233
-1.3937,1.88923,7.27883
-1.39714,1.89547,7.29532
-1.40059,1.90172,7.31178
-1.40404,1.90797,7.32822
-1.40748,1.91422,7.34464
-1.41093,1.92047,7.36104
-1.41438,1.92672,7.37742
-1.41783,1.93297,7.39377
-1.42128,1.93922,7.41011
-1.42472,1.94547,7.42642
-1.42817,1.95172,7.44271
-1.43162,1.95797,7.45898
-1.43508,1.96422,7.47523
-1.43853,1.97048,7.49146
-1.44198,1.97673,7.50766
-1.44543,1.98298,7.52385
-1.44888,1.98923,7.54002
-1.45233,1.99548,7.55616
-1.45579,2.00173,7.57229
-1.45924,2.00798,7.58839
-1.4627,2.01423,7.60447
-1.46615,2.02048,7.62054
-1.4696,2.02672,7.63658
-1.47306,2.03297,7.6526
-1.47652,2.03922,7.66861
-1.47997,2.04547,7.68459
-1.48343,2.05171,7.70055
-1.48689,2.05796,7.71649
-1.49034,2.0642,7.73242
-1.4938,2.07044,7.74832
-1.49726,2.07669,7.76421
-1.50072,2.08293,7.78007
-1.50418,2.08917,7.79592
-1.50764,2.09541,7.81174
-1.5111,2.10165,7.82755
-1.51456,2.10788,7.84334
-1.51802,2.11412,7.85911
-1.52148,2.12036,7.87486
-1.52494,2.12659,7.89059
-1.52841,2.13282,7.9063
-1.53187,2.13905,7.92199
-1.53533,2.14528,7.93767
-1.5388,2.15151,7.95332
-1.54226,2.15774,7.96896
-1.54573,2.16396,7.98458
-1.54919,2.17019,8.00018
-1.55266,2.17641,8.01576
-1.55612,2.18263,8.03132
-1.55959,2.18885,8.04687
-1.56306,2.19507,8.0624
-1.56652,2.20128,8.07791
-1.56999,2.2075,8.0934
-1.57346,2.21371,8.10887
-1.57693,2.21992,8.12433
-1.5804,2.22613,8.13976
-1.58387,2.23233,8.15518
-1.58734,2.23854,8.17059
-1.59081,2.24474,8.18597
-1.59428,2.25094,8.20134
-1.59775,2.25714,8.21669
-1.60122,2.26333,8.23202
-1.60469,2.26953,8.24734
-1.60817,2.27572,8.26263
-1.61164,2.28191,8.27792
-1.61511,2.2881,8.29318
-1.61859,2.29428,8.30843
-1.62206,2.30046,8.32366
-1.62554,2.30664,8.33887
-1.62901,2.31282,8.35407
-1.63249,2.319,8.36924
-1.63596,2.32517,8.38441
-1.63944,2.33134,8.39955
-1.64292,2.33751,8.41468
-1.6464,2.34367,8.4298
-1.64987,2.34983,8.44489
-1.65335,2.35599,8.45997
-1.65683,2.36215,8.47504
-1.66031,2.3683,8.49008
-1.66379,2.37445,8.50512
-1.66727,2.3806,8.52013
-1.67075,2.38675,8.53513
-1.67423,2.39289,8.55011
-1.67771,2.39903,8.56508
-1.6812,2.40517,8.58003
-1.68468,2.4113,8.59497
-1.68816,2.41743,8.60989
-2,3.05703,9.90258
-2.00377,3.06613,9.91862
-2.00756,3.07528,9.9347
-2.01136,3.08446,9.95082
-2.01518,3.09368,9.96699
-2.01901,3.10294,9.9832
-2.02285,3.11225,9.99945
-2.02671,3.12159,10.01574
-2.03058,3.13098,10.03208
-2.03448,3.14041,10.04846
-2.03838,3.14988,10.06488
-2.0423,3.15939,10.08134
-2.04623,3.16895,10.09785
-2.05018,3.17854,10.1144
-2.05415,3.18818,10.13099
-2.05813,3.19787,10.14763
-2.06212,3.20759,10.16431
-2.06613,3.21737,10.18103
-2.07016,3.22718,10.1978
-2.0742,3.23703,10.21461
-2.07826,3.24694,10.23147
-2.08234,3.25688,10.24837
-2.08642,3.26687,10.26532
-2.09053,3.27691,10.28231
-2.09465,3.28699,10.29935
-2.09879,3.29713,10.31643
-2.10295,3.30729,10.33355
-2.10712,3.31752,10.35073
-2.11131,3.32778,10.36794
-2.11551,3.33809,10.38521
-2.11974,3.34845,10.40252
-2.12397,3.35886,10.41988
-2.12823,3.36931,10.43728
-2.1325,3.37982,10.45473
-2.13679,3.39036,10.47222
-2.1411,3.40096,10.48977
-2.14542,3.41161,10.50736
-2.14977,3.4223,10.525
-2.15412,3.43304,10.54268
-2.1585,3.44384,10.56042
-2.1629,3.45468,10.5782
-2.16731,3.46557,10.59605
-2.17174,3.47652,10.61391
-2.17619,3.48751,10.63183
-2.18066,3.49855,10.64983
-2.18514,3.50965,10.66783
-2.18965,3.52079,10.68592
-2.19417,3.532,10.70402
-2.19871,3.54324,10.7222
-2.20327,3.55455,10.74043
-2.20785,3.5659,10.7587
-2.21245,3.57731,10.77702
-2.21707,3.58877,10.79538
-2.2217,3.60029,10.81379
-2.22636,3.61185,10.83229
-2.23104,3.62348,10.85079
-2.23574,3.63515,10.86937
-2.24045,3.64688,10.88801
-2.24519,3.65866,10.90669
-2.24994,3.67051,10.92541
-2.25472,3.68241,10.94418
-2.25951,3.69437,10.963
-2.26433,3.70637,10.9819
-2.26917,3.71844,11.00081
-2.27402,3.73056,11.01981
-2.2789,3.74275,11.03885
-2.2838,3.75497,11.05798
-2.28872,3.76728,11.07711
-2.29367,3.77964,11.09629
-2.29863,3.79205,11.11556
-2.30362,3.80452,11.13487
-2.30862,3.81705,11.15423
-2.31365,3.82965,11.17364
-2.3187,3.84229,11.19313
-2.32377,3.85501,11.21263
-2.32887,3.86778,11.23222
-2.33398,3.88062,11.25185
-2.33913,3.89351,11.27157
-2.34429,3.90647,11.2913
-2.34947,3.91949,11.31112
-2.35468,3.93257,11.33098
-2.35991,3.94572,11.35089
-2.36517,3.95893,11.37085
-2.37044,3.9722,11.39089
-2.37574,3.98554,11.41098
-2.38107,3.99894,11.43112
-2.38642,4.01241,11.45131
-2.3918,4.02594,11.47158
-2.39719,4.03954,11.4919
-2.40262,4.0532,11.51227
-2.40806,4.06694,11.53269
-2.41353,4.08073,11.5532
-2.41903,4.09459,11.57375
-2.42455,4.10853,11.59435
-2.4301,4.12254,11.615
-2.43567,4.1366,11.63574
-2.44127,4.15074,11.65653
-2.44689,4.16494,11.6774
-2.45254,4.17923,11.69829
-2.45822,4.19358,11.71926
-2.46392,4.208,11.74028
-2.46965,4.22248,11.76139
-2.4754,4.23704,11.78255
-2.48119,4.25169,11.80377
-2.48699,4.26638,11.82502
-2.49283,4.28118,11.84637
-2.49869,4.29601,11.86776
-2.50458,4.31095,11.88925
-2.51051,4.32597,11.91075
-2.51645,4.34102,11.93233
-2.52242,4.35616,11.954
-2.52843,4.37138,11.97573
-2.53446,4.3867,11.99751
-2.54053,4.40208,12.01933
-2.54662,4.41753,12.04124
-2.55274,4.43307,12.06321
-2.55889,4.44868,12.08527
-2.56506,4.46438,12.10738
-2.57128,4.48014,12.12954
-2.57751,4.496,12.15179
-2.58379,4.51192,12.17409
-2.59008,4.52792,12.19644
-2.59642,4.54403,12.21889
-2.60278,4.56019,12.24138
-2.60917,4.57645,12.26397
-2.6156,4.59277,12.2866
-2.62205,4.6092,12.30929
-2.62854,4.6257,12.33208
-2.63506,4.64228,12.35491
-2.64162,4.65897,12.37784
-2.6482,4.6757,12.40081
-2.65482,4.69255,12.42385
-2.66147,4.7095,12.44698
-2.66815,4.72652,12.47016
-2.67488,4.74361,12.49343
-2.68163,4.76082,12.51676
-2.68841,4.7781,12.54014
-2.69524,4.79547,12.56362
-2.70209,4.81291,12.58718
-2.70898,4.83046,12.6108
-2.71591,4.84808,12.63447
-2.72287,4.86584,12.65825
-2.72987,4.88366,12.68208
-2.7369,4.90159,12.70597
-2.74397,4.91957,12.72997
-2.75108,4.9377,12.75401
-2.75823,4.95589,12.77814
-2.7654,4.97416,12.80236
-2.77263,4.99254,12.82663
-2.77988,5.01106,12.85098
-2.78717,5.02963,12.87541
-2.79451,5.0483,12.8999
-2.80187,5.06709,12.92449
-2.80929,5.08598,12.94914
-2.81673,5.10495,12.97388
-2.82423,5.12401,12.99871
-2.83175,5.14318,13.02357
-2.83932,5.16245,13.04856
-2.84693,5.18185,13.07362
-2.85458,5.20131,13.09873
-2.86228,5.22091,13.12395
-2.87001,5.24058,13.14921
-2.87778,5.26039,13.17459
-2.8856,5.2803,13.20002
-2.89346,5.30027,13.22554
-2.90137,5.32041,13.25114
-2.90931,5.34062,13.27683
-2.91731,5.36095,13.30259
-2.92534,5.38139,13.32844
-2.93341,5.40193,13.35439
-2.94154,5.42259,13.38041
-2.9497,5.44337,13.4065
-2.95792,5.46425,13.43268
-2.96618,5.48523,13.45896
-2.97449,5.50632,13.48531
-2.98284,5.52757,13.51173
-2.99124,5.54891,13.53826
-2.99969,5.57034,13.56487
-3.00818,5.59192,13.59156
-3.01673,5.6136,13.61835
-3.02532,5.63542,13.64522
-3.03395,5.65733,13.67218
-3.04265,5.67937,13.69924
-3.05139,5.70152,13.72634
-3.06018,5.72382,13.75358
-3.06902,5.74622,13.78089
-3.07792,5.76874,13.80831
-3.08686,5.79139,13.83579
-3.09585,5.81418,13.86336
-3.10491,5.83708,13.89102
-3.114,5.8601,13.91879
-3.12317,5.88327,13.94668
-3.13237,5.90657,13.9746
-3.14164,5.92998,14.00267
-3.15096,5.95351,14.0308
-3.16033,5.9772,14.05901
-3.16976,6.00099,14.08733
-3.17925,6.02493,14.11576
-3.1888,6.04902,14.14428
-3.19839,6.07321,14.17289
-3.20806,6.09756,14.20159
-3.21777,6.12203,14.2304
-3.22755,6.14665,14.25932
-3.23739,6.1714,14.28832
-3.24728,6.1963,14.31741
-3.25724,6.22133,14.3466
-3.26726,6.24652,14.37592
-3.27733,6.27182,14.4053
-3.28748,6.29728,14.43481
-3.29769,6.3229,14.46441
-3.30796,6.34865,14.49411
-3.31829,6.37454,14.52394
-3.3287,6.40058,14.55384
-3.33915,6.42677,14.58384
-3.34968,6.45314,14.61397
-3.36028,6.47963,14.6442
-3.37094,6.50628,14.67452
-3.38168,6.53307,14.70496
-3.39248,6.56001,14.73549
-3.40335,6.58713,14.76615
-3.41429,6.61439,14.7969
-3.42529,6.6418,14.82776
-3.43638,6.66938,14.85872
-3.44753,6.69713,14.88981
-3.45876,6.72502,14.92099
-3.47005,6.75311,14.95231
-3.48143,6.78132,14.98373
-3.49288,6.8097,15.01526
-3.50439,6.83825,15.04691
-3.516,6.86698,15.07868
-3.52767,6.89586,15.11052
-3.53943,6.92494,15.14252
-3.55126,6.95414,15.17462
-3.56317,6.98356,15.20685
-3.57517,7.01315,15.23917
-3.58724,7.04286,15.27164
-3.5994,7.0728,15.3042
-3.61163,7.10291,15.33689
-3.62396,7.13318,15.36972
-3.63636,7.16364,15.40265
-3.64885,7.19427,15.43569
-3.66143,7.22509,15.46887
-3.67409,7.2561,15.50219
-3.68685,7.2873,15.53559
-3.69969,7.31867,15.56916
-3.71263,7.35023,15.60285
-3.72564,7.38199,15.63665
-3.73875,7.41393,15.67056
-3.75197,7.44607,15.70465
-3.76526,7.47842,15.73883
-3.77866,7.51093,15.77314
-3.79214,7.54366,15.80759
-3.80573,7.57658,15.84218
-3.81942,7.60971,15.87689
-3.83319,7.64303,15.91175
-3.84709,7.67655,15.94674
-3.86106,7.7103,15.98186
-3.87516,7.74422,16.01711
-3.88934,7.77838,16.05251
-3.90363,7.81272,16.08806
-3.91803,7.84729,16.12371
-3.93253,7.88207,16.15952
-3.94716,7.91708,16.1955
-3.96187,7.95227,16.23159
-3.97671,7.9877,16.26783
-3.99165,8.02336,16.30421
-4.0067,8.05924,16.34076
-4.02188,8.09532,16.37743
-4.03716,8.13164,16.41428
-4.05257,8.1682,16.45124
-4.06808,8.20496,16.48837
-4.08373,8.24197,16.52565
-4.09949,8.2792,16.56307
-4.11536,8.31668,16.60067
-4.13138,8.35438,16.63841
-4.1475,8.39233,16.6763
-4.16377,8.43053,16.71436
-4.18015,8.46896,16.75259
-4.19666,8.50762,16.79094
-4.21331,8.54655,16.82948
-4.23008,8.58572,16.86818
-4.24701,8.62516,16.90705
-4.26405,8.66483,16.9461
-4.28124,8.70475,16.98528
-4.29856,8.74495,17.02463
-4.31602,8.78539,17.06418
-4.33364,8.82609,17.10389
-4.35138,8.86708,17.14375
-4.36929,8.9083,17.1838
-4.38733,8.94982,17.22403
-4.40554,8.9916,17.26444
-4.42388,9.03365,17.30502
-4.44237,9.07598,17.34579
-4.46104,9.11857,17.38673
-4.47985,9.16145,17.42786
-4.49883,9.20465,17.46916
-4.51796,9.24811,17.51067
-4.53727,9.29183,17.55235
-4.55672,9.33587,17.59424
-4.57634,9.3802,17.6363
-4.59616,9.42483,17.67856
-4.61612,9.46974,17.72103
-4.63628,9.51497,17.76369
-4.6566,9.5605,17.80655
-4.67709,9.60634,17.84962
-4.69779,9.65248,17.89286
-4.71865,9.69894,17.93634
-4.73972,9.74571,17.98001
-4.76095,9.7928,18.0239
-4.7824,9.84025,18.06799
-4.80402,9.88798,18.11229
-4.82584,9.93605,18.15682
-4.84787,9.98444,18.20157
-4.87009,10.03319,18.24653
-4.89254,10.08227,18.29172
-4.91516,10.13165,18.33713
-4.93803,10.18143,18.38278
-4.96108,10.23152,18.42864
-4.98435,10.28198,18.47474
-5.00786,10.33279,18.52108
-5.03157,10.38397,18.56766
-5.05554,10.43549,18.61447
-5.0797,10.48738,18.66152
-5.1041,10.53965,18.70883
-5.12876,10.59229,18.75638
-5.15363,10.6453,18.80416
-5.17877,10.69871,18.85223
-5.20413,10.75248,18.90052
-5.22977,10.80664,18.9491
-5.25563,10.8612,18.99794
-5.28176,10.91616,19.04704
-5.30817,10.97152,19.09639
-5.33481,11.02727,19.14604
-5.36176,11.08343,19.19595
-5.38895,11.14002,19.24615
-5.41644,11.19702,19.29661
-5.44419,11.25445,19.34737
-5.47223,11.31229,19.39842
-5.50058,11.37056,19.44975
-5.5292,11.42928,19.5014
-5.55815,11.48844,19.55332
-5.58737,11.54805,19.60557
-5.61694,11.60811,19.65811
-5.64678,11.6686,19.71097
-5.67695,11.72958,19.76414
-5.70747,11.79102,19.81762
-5.73829,11.85294,19.87144
-5.76947,11.91533,19.92559
-5.80097,11.97819,19.98007
-5.83281,12.04154,20.03489
-5.86503,12.1054,20.09004
-5.89758,12.16976,20.14555
-5.93053,12.23462,20.20141
-5.96381,12.29999,20.25761
-5.99751,12.36589,20.31419
-6.03154,12.43231,20.37111
-6.06597,12.49924,20.42844
-6.10083,12.56673,20.48611
-6.13606,12.63475,20.54417
-6.17173,12.70333,20.60263
-6.20779,12.77246,20.66148
-6.2443,12.84219,20.72073
-6.28121,12.91244,20.78038
-6.31856,12.98331,20.84045
-6.35639,13.05475,20.90094
-6.39464,13.12677,20.96185
-6.43339,13.1994,21.02318
-6.47258,13.27266,21.08496
-6.51228,13.34653,21.14717
-6.55244,13.42103,21.20985
-6.59309,13.49615,21.27296
-6.63429,13.57191,21.33656
-6.67597,13.64834,21.40063
-6.71822,13.72543,21.46519
-6.76096,13.80319,21.53021
-6.80425,13.88162,21.59575
-6.84814,13.96075,21.6618
-6.89256,14.04058,21.72834
-6.9376,14.12112,21.79541
-6.98319,14.20237,21.86301
-7.02943,14.28436,21.93116
-7.07624,14.36709,21.99987
-7.12367,14.45056,22.06911
-7.1718,14.5348,22.13893
-7.22053,14.61983,22.20933
-7.26998,14.70563,22.28032
-7.32005,14.79223,22.35191
-7.37088,14.87965,22.42412
-7.42236,14.96789,22.49693
-7.47457,15.05697,22.57038
-7.52757,15.14688,22.64449
-7.58127,15.23768,22.71924
-7.6358,15.32934,22.79466
-7.69107,15.42188,22.87078
-7.74719,15.51536,22.94758
-7.80409,15.60973,23.02509
-7.86182,15.70505,23.10333
-7.92048,15.80132,23.1823
-7.97995,15.89856,23.26201
-8.04039,15.99678,23.34251
-8.10169,16.09601,23.42378
-8.16393,16.19625,23.50584
-8.2272,16.29754,23.58872
-8.29139,16.39987,23.67245
-8.35666,16.50328,23.757
-8.4229,16.60777,23.84242
-8.49026,16.71341,23.92873
-8.55864,16.82016,24.01595
-8.62813,16.92806,24.10407
-8.69883,17.03714,24.19314
-8.77062,17.14742,24.28318
-8.84369,17.25894,24.37421
-8.9179,17.37169,24.46624
-8.99345,17.48571,24.55928
-9.07021,17.60103,24.65338
-9.14829,17.71767,24.74857
-9.22782,17.83566,24.84486
-9.30865,17.95503,24.94226
-9.39099,18.0758,25.04082
-9.47472,18.198,25.14057
-9.55996,18.32167,25.2415
-9.64683,18.44684,25.34369
-9.7352,18.57351,25.44715
-9.82531,18.70177,25.55189
-9.91699,18.83161,25.65797
-10.01047,18.96308,25.76541
-10.10571,19.09623,25.87425
-10.20277,19.23106,25.98453
-10.30173,19.36769,26.09629
-10.40261,19.50606,26.20955
-10.50549,19.64626,26.32435
-10.61043,19.78825,26.44069
-10.71749,19.93225,26.55872
-10.82673,20.07821,26.67843
-10.93821,20.22621,26.79988
-11.05202,20.37621,26.92306
-11.16823,20.52831,27.04802
-11.2869,20.68266,27.17494
-11.40812,20.83924,27.30377
-11.53196,20.99801,27.43451
-11.65853,21.15925,27.56737
-11.78792,21.32281,27.70226
-11.9202,21.48886,27.83931
-12.05548,21.65746,27.97858
-12.19387,21.82879,28.12021
-12.33549,22.00278,28.26415
-12.48042,22.1795,28.41047
-12.6288,22.3591,28.55929
-12.78075,22.54174,28.71073
-12.93639,22.72748,28.86484
-13.0959,22.91623,29.02157
-13.25936,23.10838,29.18119
-13.42696,23.30385,29.34365
-13.59886,23.5028,29.50904
-13.77522,23.70536,29.67747
-13.95621,23.91166,29.84903
-14.14201,24.12175,30.02374
-14.33283,24.33574,30.20167
-14.52887,24.55374,30.38294
-14.73036,24.77587,30.56764
-14.9375,25.00219,30.7559
-15.15055,25.23278,30.94783
-15.36977,25.46769,31.14358
-15.59544,25.70713,31.34344
-15.82782,25.95104,31.54748
-16.06723,26.19972,31.75606
-16.31399,26.45327,31.96939
-16.56847,26.71202,32.18776
-16.83099,26.97613,32.41143
-17.10197,27.24584,32.64057
-17.38181,27.52154,32.87552
-17.67097,27.8034,33.11646
-17.96994,28.09178,33.36367
-18.27916,28.38706,33.61743
-18.59922,28.68943,33.87798
-18.93068,28.99924,34.14555
-19.27421,29.31693,34.42055
-19.6304,29.64276,34.70325
-20,29.97724,34.99405
+wl,n,k
+0.2114,2.47401,1.97842
+0.21298,2.49873,1.94326
+0.21456,2.52109,1.91041
+0.21614,2.54137,1.87953
+0.21772,2.55979,1.85035
+0.2193,2.57656,1.82264
+0.22089,2.59185,1.79624
+0.22247,2.60579,1.77099
+0.22405,2.61852,1.74678
+0.22563,2.63013,1.7235
+0.22721,2.64071,1.70106
+0.2288,2.65035,1.67941
+0.23038,2.65913,1.65846
+0.23196,2.66709,1.63817
+0.23354,2.67429,1.61849
+0.23513,2.6808,1.59939
+0.23671,2.68664,1.58081
+0.23829,2.69186,1.56275
+0.23987,2.69651,1.54515
+0.24146,2.7006,1.52801
+0.24304,2.70417,1.5113
+0.24462,2.70726,1.495
+0.24621,2.70987,1.47908
+0.24779,2.71205,1.46354
+0.24937,2.7138,1.44837
+0.25096,2.71516,1.43353
+0.25254,2.71613,1.41903
+0.25412,2.71673,1.40485
+0.25571,2.71699,1.39099
+0.25729,2.71691,1.37742
+0.25887,2.71652,1.36414
+0.26046,2.71581,1.35115
+0.26204,2.71481,1.33844
+0.26363,2.71353,1.32599
+0.26521,2.71197,1.3138
+0.2668,2.71015,1.30187
+0.26838,2.70808,1.29018
+0.26996,2.70576,1.27874
+0.27155,2.70321,1.26753
+0.27313,2.70042,1.25656
+0.27472,2.69742,1.24581
+0.2763,2.6942,1.23528
+0.27789,2.69078,1.22496
+0.27947,2.68716,1.21486
+0.28106,2.68334,1.20497
+0.28264,2.67933,1.19528
+0.28423,2.67514,1.18579
+0.28581,2.67077,1.1765
+0.2874,2.66623,1.1674
+0.28898,2.66152,1.15849
+0.29057,2.65664,1.14977
+0.29215,2.6516,1.14123
+0.29374,2.64641,1.13286
+0.29533,2.64106,1.12468
+0.29691,2.63557,1.11667
+0.2985,2.62993,1.10883
+0.30008,2.62415,1.10117
+0.30167,2.61823,1.09367
+0.30325,2.61217,1.08633
+0.30484,2.60598,1.07915
+0.30643,2.59965,1.07214
+0.30801,2.5932,1.06528
+0.3096,2.58663,1.05858
+0.31119,2.57993,1.05203
+0.31277,2.5731,1.04564
+0.31436,2.56616,1.0394
+0.31595,2.55911,1.0333
+0.31753,2.55193,1.02735
+0.31912,2.54464,1.02155
+0.3207,2.53724,1.01589
+0.32229,2.52973,1.01037
+0.32388,2.52211,1.00499
+0.32547,2.51439,0.99976
+0.32705,2.50655,0.99466
+0.32864,2.49862,0.9897
+0.33023,2.49058,0.98487
+0.33181,2.48243,0.98018
+0.3334,2.47419,0.97563
+0.33499,2.46585,0.97121
+0.33658,2.4574,0.96692
+0.33816,2.44886,0.96276
+0.33975,2.44022,0.95873
+0.34134,2.43149,0.95484
+0.34292,2.42266,0.95107
+0.34451,2.41373,0.94743
+0.3461,2.40471,0.94392
+0.34769,2.3956,0.94053
+0.34928,2.3864,0.93728
+0.35086,2.3771,0.93415
+0.35245,2.36771,0.93114
+0.35404,2.35823,0.92827
+0.35563,2.34866,0.92552
+0.35721,2.339,0.92289
+0.3588,2.32925,0.92039
+0.36039,2.31942,0.91802
+0.36198,2.30949,0.91577
+0.36357,2.29948,0.91365
+0.36515,2.28937,0.91165
+0.36674,2.27919,0.90978
+0.36833,2.26891,0.90803
+0.36992,2.25855,0.90641
+0.37151,2.2481,0.90492
+0.3731,2.23756,0.90355
+0.37468,2.22694,0.90231
+0.37627,2.21624,0.9012
+0.37786,2.20545,0.90022
+0.37945,2.19457,0.89937
+0.38104,2.18361,0.89864
+0.38263,2.17257,0.89805
+0.38422,2.16144,0.89759
+0.38581,2.15023,0.89726
+0.38739,2.13893,0.89706
+0.38898,2.12756,0.89699
+0.39057,2.11609,0.89706
+0.39216,2.10455,0.89727
+0.39375,2.09293,0.89761
+0.39534,2.08122,0.89809
+0.39693,2.06943,0.89871
+0.39852,2.05756,0.89947
+0.40011,2.04562,0.90038
+0.40169,2.03359,0.90142
+0.40328,2.02148,0.90261
+0.40487,2.00929,0.90395
+0.40646,1.99703,0.90544
+0.40805,1.98469,0.90708
+0.40964,1.97227,0.90886
+0.41123,1.95977,0.91081
+0.41282,1.9472,0.9129
+0.41441,1.93456,0.91516
+0.416,1.92184,0.91757
+0.41759,1.90905,0.92015
+0.41918,1.89619,0.92289
+0.42077,1.88326,0.9258
+0.42235,1.87026,0.92887
+0.42394,1.8572,0.93212
+0.42553,1.84406,0.93553
+0.42712,1.83087,0.93913
+0.42871,1.81761,0.9429
+0.4303,1.80429,0.94685
+0.43189,1.79091,0.95099
+0.43348,1.77748,0.95531
+0.43507,1.76399,0.95982
+0.43666,1.75045,0.96453
+0.43825,1.73686,0.96942
+0.43984,1.72322,0.97452
+0.44143,1.70954,0.97981
+0.44302,1.69582,0.9853
+0.44461,1.68206,0.991
+0.4462,1.66827,0.99691
+0.44779,1.65445,1.00303
+0.44938,1.6406,1.00936
+0.45097,1.62673,1.01591
+0.45256,1.61284,1.02267
+0.45415,1.59893,1.02965
+0.45574,1.58502,1.03686
+0.45733,1.5711,1.04429
+0.45892,1.55718,1.05195
+0.46051,1.54327,1.05983
+0.4621,1.52937,1.06795
+0.46369,1.51549,1.07629
+0.46528,1.50162,1.08487
+0.46687,1.48779,1.09368
+0.46846,1.47399,1.10273
+0.47005,1.46024,1.11201
+0.47164,1.44653,1.12153
+0.47323,1.43287,1.13129
+0.47482,1.41927,1.14128
+0.47641,1.40575,1.1515
+0.478,1.39229,1.16195
+0.47959,1.37892,1.17264
+0.48118,1.36563,1.18356
+0.48277,1.35244,1.19471
+0.48436,1.33936,1.20608
+0.48595,1.32638,1.21768
+0.48754,1.31351,1.2295
+0.48913,1.30077,1.24153
+0.49072,1.28815,1.25378
+0.49231,1.27567,1.26623
+0.4939,1.26333,1.27889
+0.49549,1.25113,1.29175
+0.49708,1.23909,1.3048
+0.49867,1.2272,1.31804
+0.50026,1.21548,1.33146
+0.50185,1.20392,1.34506
+0.50344,1.19254,1.35883
+0.50503,1.18132,1.37277
+0.50662,1.17029,1.38686
+0.50821,1.15944,1.40111
+0.5098,1.14877,1.4155
+0.51139,1.1383,1.43003
+0.51298,1.12801,1.44469
+0.51457,1.11791,1.45947
+0.51616,1.10801,1.47437
+0.51775,1.0983,1.48938
+0.51934,1.08878,1.5045
+0.52093,1.07947,1.51971
+0.52252,1.07034,1.53502
+0.52411,1.06142,1.5504
+0.52569,1.05269,1.56587
+0.52728,1.04415,1.58141
+0.52887,1.03581,1.59701
+0.53046,1.02766,1.61267
+0.53205,1.0197,1.62838
+0.53364,1.01193,1.64415
+0.53523,1.00434,1.65995
+0.53682,0.99695,1.6758
+0.53841,0.98974,1.69167
+0.54,0.9827,1.70757
+0.54159,0.97585,1.7235
+0.54318,0.96917,1.73945
+0.54477,0.96267,1.75541
+0.54636,0.95634,1.77138
+0.54795,0.95018,1.78736
+0.54954,0.94418,1.80334
+0.55113,0.93835,1.81932
+0.55272,0.93267,1.8353
+0.55431,0.92715,1.85128
+0.5559,0.92179,1.86724
+0.55749,0.91658,1.88319
+0.55908,0.91151,1.89913
+0.56067,0.90659,1.91505
+0.56226,0.90182,1.93095
+0.56385,0.89718,1.94684
+0.56544,0.89268,1.96269
+0.56703,0.88831,1.97853
+0.56861,0.88408,1.99434
+0.5702,0.87997,2.01012
+0.57179,0.87599,2.02587
+0.57338,0.87213,2.04159
+0.57497,0.86839,2.05728
+0.57656,0.86477,2.07293
+0.57815,0.86126,2.08855
+0.57974,0.85787,2.10414
+0.58133,0.85458,2.11969
+0.58292,0.85141,2.1352
+0.58451,0.84833,2.15068
+0.5861,0.84537,2.16611
+0.58768,0.8425,2.18151
+0.58927,0.83973,2.19687
+0.59086,0.83706,2.21219
+0.59245,0.83448,2.22746
+0.59404,0.83199,2.2427
+0.59563,0.82959,2.2579
+0.59722,0.82728,2.27305
+0.59881,0.82506,2.28817
+0.60039,0.82292,2.30324
+0.60198,0.82087,2.31827
+0.60357,0.81889,2.33326
+0.60516,0.817,2.3482
+0.60675,0.81518,2.3631
+0.60834,0.81343,2.37796
+0.60993,0.81176,2.39278
+0.61151,0.81016,2.40756
+0.6131,0.80864,2.42229
+0.61469,0.80718,2.43698
+0.61628,0.80579,2.45163
+0.61787,0.80447,2.46623
+0.61946,0.80321,2.4808
+0.62104,0.80202,2.49532
+0.62263,0.80088,2.5098
+0.62422,0.79981,2.52424
+0.62581,0.7988,2.53863
+0.6274,0.79785,2.55299
+0.62898,0.79695,2.5673
+0.63057,0.79611,2.58157
+0.63216,0.79533,2.5958
+0.63375,0.7946,2.60999
+0.63533,0.79392,2.62414
+0.63692,0.7933,2.63825
+0.63851,0.79273,2.65232
+0.6401,0.7922,2.66635
+0.64168,0.79173,2.68034
+0.64327,0.7913,2.69429
+0.64486,0.79092,2.70821
+0.64645,0.79059,2.72208
+0.64803,0.7903,2.73591
+0.64962,0.79005,2.74971
+0.65121,0.78985,2.76347
+0.6528,0.7897,2.77719
+0.65438,0.78958,2.79087
+0.65597,0.78951,2.80451
+0.65756,0.78947,2.81812
+0.65914,0.78948,2.83169
+0.66073,0.78953,2.84522
+0.66232,0.78961,2.85872
+0.6639,0.78973,2.87218
+0.66549,0.78989,2.88561
+0.66708,0.79008,2.899
+0.66866,0.79031,2.91235
+0.67025,0.79058,2.92567
+0.67184,0.79088,2.93895
+0.67342,0.79121,2.9522
+0.67501,0.79158,2.96542
+0.67659,0.79198,2.9786
+0.67818,0.79241,2.99175
+0.67977,0.79287,3.00486
+0.68135,0.79337,3.01794
+0.68294,0.79389,3.03099
+0.68452,0.79445,3.044
+0.68611,0.79504,3.05698
+0.6877,0.79565,3.06993
+0.68928,0.79629,3.08285
+0.69087,0.79696,3.09573
+0.69245,0.79766,3.10859
+0.69404,0.79839,3.12141
+0.69562,0.79914,3.1342
+0.69721,0.79992,3.14696
+0.69879,0.80073,3.15969
+0.70038,0.80156,3.17239
+0.70196,0.80241,3.18506
+0.70355,0.8033,3.19769
+0.70513,0.8042,3.2103
+0.70672,0.80513,3.22288
+0.7083,0.80608,3.23543
+0.70989,0.80706,3.24795
+0.71147,0.80806,3.26044
+0.71306,0.80908,3.2729
+0.71464,0.81013,3.28534
+0.71623,0.8112,3.29774
+0.71781,0.81228,3.31012
+0.7194,0.81339,3.32247
+0.72098,0.81452,3.33479
+0.72256,0.81568,3.34708
+0.72415,0.81685,3.35935
+0.72573,0.81804,3.37159
+0.72732,0.81925,3.3838
+0.7289,0.82049,3.39599
+0.73048,0.82174,3.40815
+0.73207,0.82301,3.42028
+0.73365,0.8243,3.43239
+0.73523,0.8256,3.44447
+0.73682,0.82693,3.45652
+0.7384,0.82828,3.46855
+0.73998,0.82964,3.48055
+0.74157,0.83102,3.49253
+0.74315,0.83241,3.50448
+0.74473,0.83383,3.51641
+0.74631,0.83526,3.52832
+0.7479,0.83671,3.54019
+0.74948,0.83817,3.55205
+0.75106,0.83965,3.56388
+0.75264,0.84115,3.57568
+0.75423,0.84266,3.58746
+0.75581,0.84419,3.59922
+0.75739,0.84573,3.61096
+0.75897,0.84729,3.62267
+0.76056,0.84886,3.63435
+0.76214,0.85045,3.64602
+0.76372,0.85205,3.65766
+0.7653,0.85367,3.66928
+0.76688,0.8553,3.68087
+0.76846,0.85694,3.69244
+0.77004,0.8586,3.70399
+0.77163,0.86028,3.71552
+0.77321,0.86196,3.72703
+0.77479,0.86366,3.73851
+0.77637,0.86538,3.74997
+0.77795,0.8671,3.76141
+0.77953,0.86884,3.77283
+0.78111,0.8706,3.78422
+0.78269,0.87236,3.7956
+0.78427,0.87414,3.80695
+0.78585,0.87593,3.81828
+0.78743,0.87773,3.82959
+0.78901,0.87954,3.84088
+0.79059,0.88137,3.85215
+0.79217,0.88321,3.8634
+0.79375,0.88506,3.87463
+0.79533,0.88692,3.88584
+0.79691,0.88879,3.89703
+0.79849,0.89067,3.90819
+0.80007,0.89257,3.91934
+0.80165,0.89447,3.93047
+0.80323,0.89639,3.94157
+0.80481,0.89832,3.95266
+0.80639,0.90026,3.96373
+0.80797,0.9022,3.97478
+0.80955,0.90416,3.98581
+0.81113,0.90613,3.99682
+0.8127,0.90811,4.00781
+0.81428,0.9101,4.01878
+0.81586,0.9121,4.02973
+0.81744,0.91411,4.04066
+0.81902,0.91613,4.05158
+0.82059,0.91816,4.06247
+0.82217,0.92019,4.07335
+0.82375,0.92224,4.08421
+0.82533,0.9243,4.09505
+0.82691,0.92636,4.10587
+0.82848,0.92844,4.11668
+0.83006,0.93052,4.12746
+0.83164,0.93262,4.13823
+0.83321,0.93472,4.14898
+0.83479,0.93683,4.15971
+0.83637,0.93895,4.17042
+0.83794,0.94108,4.18112
+0.83952,0.94321,4.1918
+0.8411,0.94536,4.20246
+0.84267,0.94751,4.2131
+0.84425,0.94967,4.22373
+0.84583,0.95184,4.23434
+0.8474,0.95402,4.24493
+0.84898,0.95621,4.2555
+0.85055,0.9584,4.26606
+0.85213,0.9606,4.2766
+0.8537,0.96281,4.28712
+0.85528,0.96503,4.29763
+0.85686,0.96726,4.30812
+0.85843,0.96949,4.31859
+0.86001,0.97173,4.32905
+0.86158,0.97397,4.33949
+0.86315,0.97623,4.34991
+0.86473,0.97849,4.36032
+0.8663,0.98076,4.37071
+0.86788,0.98304,4.38108
+0.86945,0.98532,4.39144
+0.87103,0.98761,4.40178
+0.8726,0.98991,4.4121
+0.87417,0.99221,4.42241
+0.87575,0.99452,4.43271
+0.87732,0.99684,4.44298
+0.87889,0.99916,4.45324
+0.88047,1.0015,4.46349
+0.88204,1.00383,4.47372
+0.88361,1.00618,4.48393
+0.88519,1.00853,4.49413
+0.88676,1.01088,4.50431
+0.88833,1.01325,4.51448
+0.8899,1.01562,4.52463
+0.89148,1.01799,4.53476
+0.89305,1.02038,4.54488
+0.89462,1.02276,4.55499
+0.89619,1.02516,4.56508
+0.89776,1.02756,4.57515
+0.89934,1.02997,4.58521
+0.90091,1.03238,4.59525
+0.90248,1.0348,4.60527
+0.90405,1.03722,4.61528
+0.90562,1.03965,4.62528
+0.90719,1.04209,4.63526
+0.90876,1.04453,4.64522
+0.91033,1.04698,4.65517
+0.9119,1.04943,4.6651
+0.91347,1.05189,4.67501
+0.91504,1.05435,4.68491
+0.91661,1.05682,4.69479
+0.91818,1.05928,4.70466
+0.91975,1.06176,4.71451
+0.92132,1.06423,4.72434
+0.92289,1.06671,4.73416
+0.92446,1.06919,4.74397
+0.92603,1.07168,4.75376
+0.9276,1.07417,4.76353
+0.92917,1.07666,4.77329
+0.93074,1.07915,4.78304
+0.9323,1.08165,4.79277
+0.93387,1.08415,4.80249
+0.93544,1.08666,4.8122
+0.93701,1.08916,4.82189
+0.93858,1.09167,4.83157
+0.94014,1.09419,4.84123
+0.94171,1.0967,4.85088
+0.94328,1.09922,4.86052
+0.94485,1.10174,4.87014
+0.94641,1.10426,4.87975
+0.94798,1.10679,4.88935
+0.94955,1.10932,4.89893
+0.95111,1.11185,4.90851
+0.95268,1.11438,4.91806
+0.95425,1.11692,4.92761
+0.95581,1.11946,4.93714
+0.95738,1.122,4.94666
+0.95894,1.12455,4.95617
+0.96051,1.12709,4.96567
+0.96207,1.12964,4.97515
+0.96364,1.1322,4.98462
+0.9652,1.13475,4.99408
+0.96677,1.13731,5.00353
+0.96833,1.13987,5.01296
+0.9699,1.14243,5.02238
+0.97146,1.14499,5.03179
+0.97303,1.14756,5.04119
+0.97459,1.15013,5.05058
+0.97616,1.1527,5.05995
+0.97772,1.15527,5.06931
+0.97928,1.15785,5.07866
+0.98085,1.16042,5.088
+0.98241,1.163,5.09733
+0.98397,1.16559,5.10665
+0.98554,1.16817,5.11595
+0.9871,1.17076,5.12524
+0.98866,1.17335,5.13452
+0.99022,1.17594,5.14379
+0.99179,1.17853,5.15305
+0.99335,1.18112,5.1623
+0.99491,1.18372,5.17154
+0.99647,1.18632,5.18076
+0.99803,1.18892,5.18998
+0.99959,1.19152,5.19918
+1.01061,1.20994,5.26381
+1.014,1.21565,5.28364
+1.0174,1.22136,5.30343
+1.0208,1.22708,5.32318
+1.02419,1.23282,5.34288
+1.02759,1.23856,5.36254
+1.03099,1.24431,5.38216
+1.03439,1.25008,5.40174
+1.03778,1.25585,5.42128
+1.04118,1.26163,5.44078
+1.04458,1.26743,5.46025
+1.04798,1.27323,5.47967
+1.05138,1.27904,5.49905
+1.05479,1.28486,5.51839
+1.05819,1.29069,5.5377
+1.06159,1.29653,5.55697
+1.06499,1.30238,5.5762
+1.06839,1.30824,5.59539
+1.0718,1.3141,5.61454
+1.0752,1.31997,5.63366
+1.0786,1.32586,5.65274
+1.08201,1.33175,5.67179
+1.08541,1.33764,5.6908
+1.08882,1.34355,5.70977
+1.09223,1.34946,5.72871
+1.09563,1.35538,5.74761
+1.09904,1.36131,5.76648
+1.10245,1.36725,5.78532
+1.10585,1.37319,5.80411
+1.10926,1.37914,5.82288
+1.11267,1.3851,5.84161
+1.11608,1.39107,5.86031
+1.11949,1.39704,5.87897
+1.1229,1.40302,5.8976
+1.12631,1.409,5.9162
+1.12972,1.41499,5.93476
+1.13313,1.42099,5.95329
+1.13654,1.427,5.97179
+1.13996,1.43301,5.99026
+1.14337,1.43903,6.00869
+1.14678,1.44505,6.0271
+1.1502,1.45108,6.04547
+1.15361,1.45712,6.06381
+1.15702,1.46316,6.08212
+1.16044,1.4692,6.10039
+1.16385,1.47526,6.11864
+1.16727,1.48131,6.13686
+1.17069,1.48738,6.15504
+1.1741,1.49345,6.1732
+1.17752,1.49952,6.19132
+1.18094,1.5056,6.20942
+1.18436,1.51168,6.22748
+1.18777,1.51777,6.24552
+1.19119,1.52387,6.26352
+1.19461,1.52997,6.2815
+1.19803,1.53607,6.29945
+1.20145,1.54218,6.31737
+1.20487,1.54829,6.33526
+1.20829,1.55441,6.35312
+1.21172,1.56053,6.37095
+1.21514,1.56666,6.38876
+1.21856,1.57279,6.40653
+1.22198,1.57892,6.42428
+1.22541,1.58506,6.442
+1.22883,1.5912,6.45969
+1.23225,1.59735,6.47736
+1.23568,1.6035,6.49499
+1.2391,1.60965,6.5126
+1.24253,1.61581,6.53019
+1.24596,1.62197,6.54774
+1.24938,1.62813,6.56527
+1.25281,1.6343,6.58277
+1.25624,1.64047,6.60025
+1.25966,1.64665,6.6177
+1.26309,1.65282,6.63512
+1.26652,1.659,6.65252
+1.26995,1.66519,6.66989
+1.27338,1.67137,6.68723
+1.27681,1.67756,6.70455
+1.28024,1.68376,6.72184
+1.28367,1.68995,6.73911
+1.2871,1.69615,6.75635
+1.29054,1.70235,6.77357
+1.29397,1.70855,6.79076
+1.2974,1.71476,6.80793
+1.30083,1.72096,6.82507
+1.30427,1.72717,6.84218
+1.3077,1.73339,6.85928
+1.31114,1.7396,6.87634
+1.31457,1.74582,6.89338
+1.31801,1.75203,6.9104
+1.32144,1.75825,6.9274
+1.32488,1.76448,6.94437
+1.32832,1.7707,6.96131
+1.33175,1.77693,6.97823
+1.33519,1.78315,6.99513
+1.33863,1.78938,7.012
+1.34207,1.79562,7.02885
+1.34551,1.80185,7.04568
+1.34895,1.80808,7.06248
+1.35239,1.81432,7.07926
+1.35583,1.82055,7.09602
+1.35927,1.82679,7.11275
+1.36271,1.83303,7.12946
+1.36615,1.83927,7.14615
+1.36959,1.84551,7.16281
+1.37303,1.85175,7.17946
+1.37648,1.858,7.19607
+1.37992,1.86424,7.21267
+1.38336,1.87049,7.22925
+1.38681,1.87673,7.2458
+1.39025,1.88298,7.26233
+1.3937,1.88923,7.27883
+1.39714,1.89547,7.29532
+1.40059,1.90172,7.31178
+1.40404,1.90797,7.32822
+1.40748,1.91422,7.34464
+1.41093,1.92047,7.36104
+1.41438,1.92672,7.37742
+1.41783,1.93297,7.39377
+1.42128,1.93922,7.41011
+1.42472,1.94547,7.42642
+1.42817,1.95172,7.44271
+1.43162,1.95797,7.45898
+1.43508,1.96422,7.47523
+1.43853,1.97048,7.49146
+1.44198,1.97673,7.50766
+1.44543,1.98298,7.52385
+1.44888,1.98923,7.54002
+1.45233,1.99548,7.55616
+1.45579,2.00173,7.57229
+1.45924,2.00798,7.58839
+1.4627,2.01423,7.60447
+1.46615,2.02048,7.62054
+1.4696,2.02672,7.63658
+1.47306,2.03297,7.6526
+1.47652,2.03922,7.66861
+1.47997,2.04547,7.68459
+1.48343,2.05171,7.70055
+1.48689,2.05796,7.71649
+1.49034,2.0642,7.73242
+1.4938,2.07044,7.74832
+1.49726,2.07669,7.76421
+1.50072,2.08293,7.78007
+1.50418,2.08917,7.79592
+1.50764,2.09541,7.81174
+1.5111,2.10165,7.82755
+1.51456,2.10788,7.84334
+1.51802,2.11412,7.85911
+1.52148,2.12036,7.87486
+1.52494,2.12659,7.89059
+1.52841,2.13282,7.9063
+1.53187,2.13905,7.92199
+1.53533,2.14528,7.93767
+1.5388,2.15151,7.95332
+1.54226,2.15774,7.96896
+1.54573,2.16396,7.98458
+1.54919,2.17019,8.00018
+1.55266,2.17641,8.01576
+1.55612,2.18263,8.03132
+1.55959,2.18885,8.04687
+1.56306,2.19507,8.0624
+1.56652,2.20128,8.07791
+1.56999,2.2075,8.0934
+1.57346,2.21371,8.10887
+1.57693,2.21992,8.12433
+1.5804,2.22613,8.13976
+1.58387,2.23233,8.15518
+1.58734,2.23854,8.17059
+1.59081,2.24474,8.18597
+1.59428,2.25094,8.20134
+1.59775,2.25714,8.21669
+1.60122,2.26333,8.23202
+1.60469,2.26953,8.24734
+1.60817,2.27572,8.26263
+1.61164,2.28191,8.27792
+1.61511,2.2881,8.29318
+1.61859,2.29428,8.30843
+1.62206,2.30046,8.32366
+1.62554,2.30664,8.33887
+1.62901,2.31282,8.35407
+1.63249,2.319,8.36924
+1.63596,2.32517,8.38441
+1.63944,2.33134,8.39955
+1.64292,2.33751,8.41468
+1.6464,2.34367,8.4298
+1.64987,2.34983,8.44489
+1.65335,2.35599,8.45997
+1.65683,2.36215,8.47504
+1.66031,2.3683,8.49008
+1.66379,2.37445,8.50512
+1.66727,2.3806,8.52013
+1.67075,2.38675,8.53513
+1.67423,2.39289,8.55011
+1.67771,2.39903,8.56508
+1.6812,2.40517,8.58003
+1.68468,2.4113,8.59497
+1.68816,2.41743,8.60989
+2,3.05703,9.90258
+2.00377,3.06613,9.91862
+2.00756,3.07528,9.9347
+2.01136,3.08446,9.95082
+2.01518,3.09368,9.96699
+2.01901,3.10294,9.9832
+2.02285,3.11225,9.99945
+2.02671,3.12159,10.01574
+2.03058,3.13098,10.03208
+2.03448,3.14041,10.04846
+2.03838,3.14988,10.06488
+2.0423,3.15939,10.08134
+2.04623,3.16895,10.09785
+2.05018,3.17854,10.1144
+2.05415,3.18818,10.13099
+2.05813,3.19787,10.14763
+2.06212,3.20759,10.16431
+2.06613,3.21737,10.18103
+2.07016,3.22718,10.1978
+2.0742,3.23703,10.21461
+2.07826,3.24694,10.23147
+2.08234,3.25688,10.24837
+2.08642,3.26687,10.26532
+2.09053,3.27691,10.28231
+2.09465,3.28699,10.29935
+2.09879,3.29713,10.31643
+2.10295,3.30729,10.33355
+2.10712,3.31752,10.35073
+2.11131,3.32778,10.36794
+2.11551,3.33809,10.38521
+2.11974,3.34845,10.40252
+2.12397,3.35886,10.41988
+2.12823,3.36931,10.43728
+2.1325,3.37982,10.45473
+2.13679,3.39036,10.47222
+2.1411,3.40096,10.48977
+2.14542,3.41161,10.50736
+2.14977,3.4223,10.525
+2.15412,3.43304,10.54268
+2.1585,3.44384,10.56042
+2.1629,3.45468,10.5782
+2.16731,3.46557,10.59605
+2.17174,3.47652,10.61391
+2.17619,3.48751,10.63183
+2.18066,3.49855,10.64983
+2.18514,3.50965,10.66783
+2.18965,3.52079,10.68592
+2.19417,3.532,10.70402
+2.19871,3.54324,10.7222
+2.20327,3.55455,10.74043
+2.20785,3.5659,10.7587
+2.21245,3.57731,10.77702
+2.21707,3.58877,10.79538
+2.2217,3.60029,10.81379
+2.22636,3.61185,10.83229
+2.23104,3.62348,10.85079
+2.23574,3.63515,10.86937
+2.24045,3.64688,10.88801
+2.24519,3.65866,10.90669
+2.24994,3.67051,10.92541
+2.25472,3.68241,10.94418
+2.25951,3.69437,10.963
+2.26433,3.70637,10.9819
+2.26917,3.71844,11.00081
+2.27402,3.73056,11.01981
+2.2789,3.74275,11.03885
+2.2838,3.75497,11.05798
+2.28872,3.76728,11.07711
+2.29367,3.77964,11.09629
+2.29863,3.79205,11.11556
+2.30362,3.80452,11.13487
+2.30862,3.81705,11.15423
+2.31365,3.82965,11.17364
+2.3187,3.84229,11.19313
+2.32377,3.85501,11.21263
+2.32887,3.86778,11.23222
+2.33398,3.88062,11.25185
+2.33913,3.89351,11.27157
+2.34429,3.90647,11.2913
+2.34947,3.91949,11.31112
+2.35468,3.93257,11.33098
+2.35991,3.94572,11.35089
+2.36517,3.95893,11.37085
+2.37044,3.9722,11.39089
+2.37574,3.98554,11.41098
+2.38107,3.99894,11.43112
+2.38642,4.01241,11.45131
+2.3918,4.02594,11.47158
+2.39719,4.03954,11.4919
+2.40262,4.0532,11.51227
+2.40806,4.06694,11.53269
+2.41353,4.08073,11.5532
+2.41903,4.09459,11.57375
+2.42455,4.10853,11.59435
+2.4301,4.12254,11.615
+2.43567,4.1366,11.63574
+2.44127,4.15074,11.65653
+2.44689,4.16494,11.6774
+2.45254,4.17923,11.69829
+2.45822,4.19358,11.71926
+2.46392,4.208,11.74028
+2.46965,4.22248,11.76139
+2.4754,4.23704,11.78255
+2.48119,4.25169,11.80377
+2.48699,4.26638,11.82502
+2.49283,4.28118,11.84637
+2.49869,4.29601,11.86776
+2.50458,4.31095,11.88925
+2.51051,4.32597,11.91075
+2.51645,4.34102,11.93233
+2.52242,4.35616,11.954
+2.52843,4.37138,11.97573
+2.53446,4.3867,11.99751
+2.54053,4.40208,12.01933
+2.54662,4.41753,12.04124
+2.55274,4.43307,12.06321
+2.55889,4.44868,12.08527
+2.56506,4.46438,12.10738
+2.57128,4.48014,12.12954
+2.57751,4.496,12.15179
+2.58379,4.51192,12.17409
+2.59008,4.52792,12.19644
+2.59642,4.54403,12.21889
+2.60278,4.56019,12.24138
+2.60917,4.57645,12.26397
+2.6156,4.59277,12.2866
+2.62205,4.6092,12.30929
+2.62854,4.6257,12.33208
+2.63506,4.64228,12.35491
+2.64162,4.65897,12.37784
+2.6482,4.6757,12.40081
+2.65482,4.69255,12.42385
+2.66147,4.7095,12.44698
+2.66815,4.72652,12.47016
+2.67488,4.74361,12.49343
+2.68163,4.76082,12.51676
+2.68841,4.7781,12.54014
+2.69524,4.79547,12.56362
+2.70209,4.81291,12.58718
+2.70898,4.83046,12.6108
+2.71591,4.84808,12.63447
+2.72287,4.86584,12.65825
+2.72987,4.88366,12.68208
+2.7369,4.90159,12.70597
+2.74397,4.91957,12.72997
+2.75108,4.9377,12.75401
+2.75823,4.95589,12.77814
+2.7654,4.97416,12.80236
+2.77263,4.99254,12.82663
+2.77988,5.01106,12.85098
+2.78717,5.02963,12.87541
+2.79451,5.0483,12.8999
+2.80187,5.06709,12.92449
+2.80929,5.08598,12.94914
+2.81673,5.10495,12.97388
+2.82423,5.12401,12.99871
+2.83175,5.14318,13.02357
+2.83932,5.16245,13.04856
+2.84693,5.18185,13.07362
+2.85458,5.20131,13.09873
+2.86228,5.22091,13.12395
+2.87001,5.24058,13.14921
+2.87778,5.26039,13.17459
+2.8856,5.2803,13.20002
+2.89346,5.30027,13.22554
+2.90137,5.32041,13.25114
+2.90931,5.34062,13.27683
+2.91731,5.36095,13.30259
+2.92534,5.38139,13.32844
+2.93341,5.40193,13.35439
+2.94154,5.42259,13.38041
+2.9497,5.44337,13.4065
+2.95792,5.46425,13.43268
+2.96618,5.48523,13.45896
+2.97449,5.50632,13.48531
+2.98284,5.52757,13.51173
+2.99124,5.54891,13.53826
+2.99969,5.57034,13.56487
+3.00818,5.59192,13.59156
+3.01673,5.6136,13.61835
+3.02532,5.63542,13.64522
+3.03395,5.65733,13.67218
+3.04265,5.67937,13.69924
+3.05139,5.70152,13.72634
+3.06018,5.72382,13.75358
+3.06902,5.74622,13.78089
+3.07792,5.76874,13.80831
+3.08686,5.79139,13.83579
+3.09585,5.81418,13.86336
+3.10491,5.83708,13.89102
+3.114,5.8601,13.91879
+3.12317,5.88327,13.94668
+3.13237,5.90657,13.9746
+3.14164,5.92998,14.00267
+3.15096,5.95351,14.0308
+3.16033,5.9772,14.05901
+3.16976,6.00099,14.08733
+3.17925,6.02493,14.11576
+3.1888,6.04902,14.14428
+3.19839,6.07321,14.17289
+3.20806,6.09756,14.20159
+3.21777,6.12203,14.2304
+3.22755,6.14665,14.25932
+3.23739,6.1714,14.28832
+3.24728,6.1963,14.31741
+3.25724,6.22133,14.3466
+3.26726,6.24652,14.37592
+3.27733,6.27182,14.4053
+3.28748,6.29728,14.43481
+3.29769,6.3229,14.46441
+3.30796,6.34865,14.49411
+3.31829,6.37454,14.52394
+3.3287,6.40058,14.55384
+3.33915,6.42677,14.58384
+3.34968,6.45314,14.61397
+3.36028,6.47963,14.6442
+3.37094,6.50628,14.67452
+3.38168,6.53307,14.70496
+3.39248,6.56001,14.73549
+3.40335,6.58713,14.76615
+3.41429,6.61439,14.7969
+3.42529,6.6418,14.82776
+3.43638,6.66938,14.85872
+3.44753,6.69713,14.88981
+3.45876,6.72502,14.92099
+3.47005,6.75311,14.95231
+3.48143,6.78132,14.98373
+3.49288,6.8097,15.01526
+3.50439,6.83825,15.04691
+3.516,6.86698,15.07868
+3.52767,6.89586,15.11052
+3.53943,6.92494,15.14252
+3.55126,6.95414,15.17462
+3.56317,6.98356,15.20685
+3.57517,7.01315,15.23917
+3.58724,7.04286,15.27164
+3.5994,7.0728,15.3042
+3.61163,7.10291,15.33689
+3.62396,7.13318,15.36972
+3.63636,7.16364,15.40265
+3.64885,7.19427,15.43569
+3.66143,7.22509,15.46887
+3.67409,7.2561,15.50219
+3.68685,7.2873,15.53559
+3.69969,7.31867,15.56916
+3.71263,7.35023,15.60285
+3.72564,7.38199,15.63665
+3.73875,7.41393,15.67056
+3.75197,7.44607,15.70465
+3.76526,7.47842,15.73883
+3.77866,7.51093,15.77314
+3.79214,7.54366,15.80759
+3.80573,7.57658,15.84218
+3.81942,7.60971,15.87689
+3.83319,7.64303,15.91175
+3.84709,7.67655,15.94674
+3.86106,7.7103,15.98186
+3.87516,7.74422,16.01711
+3.88934,7.77838,16.05251
+3.90363,7.81272,16.08806
+3.91803,7.84729,16.12371
+3.93253,7.88207,16.15952
+3.94716,7.91708,16.1955
+3.96187,7.95227,16.23159
+3.97671,7.9877,16.26783
+3.99165,8.02336,16.30421
+4.0067,8.05924,16.34076
+4.02188,8.09532,16.37743
+4.03716,8.13164,16.41428
+4.05257,8.1682,16.45124
+4.06808,8.20496,16.48837
+4.08373,8.24197,16.52565
+4.09949,8.2792,16.56307
+4.11536,8.31668,16.60067
+4.13138,8.35438,16.63841
+4.1475,8.39233,16.6763
+4.16377,8.43053,16.71436
+4.18015,8.46896,16.75259
+4.19666,8.50762,16.79094
+4.21331,8.54655,16.82948
+4.23008,8.58572,16.86818
+4.24701,8.62516,16.90705
+4.26405,8.66483,16.9461
+4.28124,8.70475,16.98528
+4.29856,8.74495,17.02463
+4.31602,8.78539,17.06418
+4.33364,8.82609,17.10389
+4.35138,8.86708,17.14375
+4.36929,8.9083,17.1838
+4.38733,8.94982,17.22403
+4.40554,8.9916,17.26444
+4.42388,9.03365,17.30502
+4.44237,9.07598,17.34579
+4.46104,9.11857,17.38673
+4.47985,9.16145,17.42786
+4.49883,9.20465,17.46916
+4.51796,9.24811,17.51067
+4.53727,9.29183,17.55235
+4.55672,9.33587,17.59424
+4.57634,9.3802,17.6363
+4.59616,9.42483,17.67856
+4.61612,9.46974,17.72103
+4.63628,9.51497,17.76369
+4.6566,9.5605,17.80655
+4.67709,9.60634,17.84962
+4.69779,9.65248,17.89286
+4.71865,9.69894,17.93634
+4.73972,9.74571,17.98001
+4.76095,9.7928,18.0239
+4.7824,9.84025,18.06799
+4.80402,9.88798,18.11229
+4.82584,9.93605,18.15682
+4.84787,9.98444,18.20157
+4.87009,10.03319,18.24653
+4.89254,10.08227,18.29172
+4.91516,10.13165,18.33713
+4.93803,10.18143,18.38278
+4.96108,10.23152,18.42864
+4.98435,10.28198,18.47474
+5.00786,10.33279,18.52108
+5.03157,10.38397,18.56766
+5.05554,10.43549,18.61447
+5.0797,10.48738,18.66152
+5.1041,10.53965,18.70883
+5.12876,10.59229,18.75638
+5.15363,10.6453,18.80416
+5.17877,10.69871,18.85223
+5.20413,10.75248,18.90052
+5.22977,10.80664,18.9491
+5.25563,10.8612,18.99794
+5.28176,10.91616,19.04704
+5.30817,10.97152,19.09639
+5.33481,11.02727,19.14604
+5.36176,11.08343,19.19595
+5.38895,11.14002,19.24615
+5.41644,11.19702,19.29661
+5.44419,11.25445,19.34737
+5.47223,11.31229,19.39842
+5.50058,11.37056,19.44975
+5.5292,11.42928,19.5014
+5.55815,11.48844,19.55332
+5.58737,11.54805,19.60557
+5.61694,11.60811,19.65811
+5.64678,11.6686,19.71097
+5.67695,11.72958,19.76414
+5.70747,11.79102,19.81762
+5.73829,11.85294,19.87144
+5.76947,11.91533,19.92559
+5.80097,11.97819,19.98007
+5.83281,12.04154,20.03489
+5.86503,12.1054,20.09004
+5.89758,12.16976,20.14555
+5.93053,12.23462,20.20141
+5.96381,12.29999,20.25761
+5.99751,12.36589,20.31419
+6.03154,12.43231,20.37111
+6.06597,12.49924,20.42844
+6.10083,12.56673,20.48611
+6.13606,12.63475,20.54417
+6.17173,12.70333,20.60263
+6.20779,12.77246,20.66148
+6.2443,12.84219,20.72073
+6.28121,12.91244,20.78038
+6.31856,12.98331,20.84045
+6.35639,13.05475,20.90094
+6.39464,13.12677,20.96185
+6.43339,13.1994,21.02318
+6.47258,13.27266,21.08496
+6.51228,13.34653,21.14717
+6.55244,13.42103,21.20985
+6.59309,13.49615,21.27296
+6.63429,13.57191,21.33656
+6.67597,13.64834,21.40063
+6.71822,13.72543,21.46519
+6.76096,13.80319,21.53021
+6.80425,13.88162,21.59575
+6.84814,13.96075,21.6618
+6.89256,14.04058,21.72834
+6.9376,14.12112,21.79541
+6.98319,14.20237,21.86301
+7.02943,14.28436,21.93116
+7.07624,14.36709,21.99987
+7.12367,14.45056,22.06911
+7.1718,14.5348,22.13893
+7.22053,14.61983,22.20933
+7.26998,14.70563,22.28032
+7.32005,14.79223,22.35191
+7.37088,14.87965,22.42412
+7.42236,14.96789,22.49693
+7.47457,15.05697,22.57038
+7.52757,15.14688,22.64449
+7.58127,15.23768,22.71924
+7.6358,15.32934,22.79466
+7.69107,15.42188,22.87078
+7.74719,15.51536,22.94758
+7.80409,15.60973,23.02509
+7.86182,15.70505,23.10333
+7.92048,15.80132,23.1823
+7.97995,15.89856,23.26201
+8.04039,15.99678,23.34251
+8.10169,16.09601,23.42378
+8.16393,16.19625,23.50584
+8.2272,16.29754,23.58872
+8.29139,16.39987,23.67245
+8.35666,16.50328,23.757
+8.4229,16.60777,23.84242
+8.49026,16.71341,23.92873
+8.55864,16.82016,24.01595
+8.62813,16.92806,24.10407
+8.69883,17.03714,24.19314
+8.77062,17.14742,24.28318
+8.84369,17.25894,24.37421
+8.9179,17.37169,24.46624
+8.99345,17.48571,24.55928
+9.07021,17.60103,24.65338
+9.14829,17.71767,24.74857
+9.22782,17.83566,24.84486
+9.30865,17.95503,24.94226
+9.39099,18.0758,25.04082
+9.47472,18.198,25.14057
+9.55996,18.32167,25.2415
+9.64683,18.44684,25.34369
+9.7352,18.57351,25.44715
+9.82531,18.70177,25.55189
+9.91699,18.83161,25.65797
+10.01047,18.96308,25.76541
+10.10571,19.09623,25.87425
+10.20277,19.23106,25.98453
+10.30173,19.36769,26.09629
+10.40261,19.50606,26.20955
+10.50549,19.64626,26.32435
+10.61043,19.78825,26.44069
+10.71749,19.93225,26.55872
+10.82673,20.07821,26.67843
+10.93821,20.22621,26.79988
+11.05202,20.37621,26.92306
+11.16823,20.52831,27.04802
+11.2869,20.68266,27.17494
+11.40812,20.83924,27.30377
+11.53196,20.99801,27.43451
+11.65853,21.15925,27.56737
+11.78792,21.32281,27.70226
+11.9202,21.48886,27.83931
+12.05548,21.65746,27.97858
+12.19387,21.82879,28.12021
+12.33549,22.00278,28.26415
+12.48042,22.1795,28.41047
+12.6288,22.3591,28.55929
+12.78075,22.54174,28.71073
+12.93639,22.72748,28.86484
+13.0959,22.91623,29.02157
+13.25936,23.10838,29.18119
+13.42696,23.30385,29.34365
+13.59886,23.5028,29.50904
+13.77522,23.70536,29.67747
+13.95621,23.91166,29.84903
+14.14201,24.12175,30.02374
+14.33283,24.33574,30.20167
+14.52887,24.55374,30.38294
+14.73036,24.77587,30.56764
+14.9375,25.00219,30.7559
+15.15055,25.23278,30.94783
+15.36977,25.46769,31.14358
+15.59544,25.70713,31.34344
+15.82782,25.95104,31.54748
+16.06723,26.19972,31.75606
+16.31399,26.45327,31.96939
+16.56847,26.71202,32.18776
+16.83099,26.97613,32.41143
+17.10197,27.24584,32.64057
+17.38181,27.52154,32.87552
+17.67097,27.8034,33.11646
+17.96994,28.09178,33.36367
+18.27916,28.38706,33.61743
+18.59922,28.68943,33.87798
+18.93068,28.99924,34.14555
+19.27421,29.31693,34.42055
+19.6304,29.64276,34.70325
+20,29.97724,34.99405
```

### Comparing `layerlumos-1.0.0/layerlumos/materials/Ti_Ordal.csv` & `layerlumos-1.0.1/layerlumos/materials/Ti_Ordal.csv`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-wl,n,k
-0.667,2.370432,3.0317254
-0.714,2.5658703,3.1836237
-0.769,2.8061078,3.2717366
-0.833,3.1079186,3.3007447
-0.909,3.3065327,3.2405736
-1,3.3957928,3.2418121
-1.05,3.4440424,3.2989913
-1.11,3.5179021,3.3609902
-1.18,3.6009322,3.4342207
-1.25,3.698148,3.5123265
-1.33,3.8097162,3.5906589
-1.43,3.9419174,3.7122171
-1.54,4.0126191,3.8077018
-1.67,4.2746437,3.8609249
-1.82,4.4682212,3.8823682
-2,4.6752372,3.8164244
-2.11,4.7311251,3.7288987
-2.22,4.7418094,3.6030774
-2.35,4.6520327,3.3990496
-2.5,4.364761,3.1898829
-2.67,3.8144105,3.0741948
-2.86,3.0649496,3.5829978
-3.08,2.4004043,4.4865443
-3.33,2.3943002,5.4204022
-3.64,2.5809283,6.2578349
-4,2.7313635,7.0189943
-4.44,2.8327334,7.7291731
-5,2.3660792,8.7896083
-5.71,2.1867059,10.53627
-6.67,2.4841185,12.895769
-8,3.2048691,15.799043
-10,4.0715739,19.664351
-11.1,4.5921948,21.789718
-12.5,5.29318,24.380236
-14.3,6.2397504,27.621553
-16.7,7.5817542,31.846917
-20,9.6744916,37.605191
-22.2,11.217047,41.326081
-25,13.29969,45.839465
-28.6,16.284041,51.475157
-33.3,20.880752,58.046709
-40,27.169229,65.925258
-44.4,31.260311,70.562709
-50,36.217641,75.809491
-57.1,42.303853,81.834224
-66.7,49.906684,88.904473
-80,59.644857,97.484039
-100,72.530316,108.42373
-125,86.399911,120.07897
-154,100.49717,131.88977
-200,119.99544,148.43379
+wl,n,k
+0.667,2.370432,3.0317254
+0.714,2.5658703,3.1836237
+0.769,2.8061078,3.2717366
+0.833,3.1079186,3.3007447
+0.909,3.3065327,3.2405736
+1,3.3957928,3.2418121
+1.05,3.4440424,3.2989913
+1.11,3.5179021,3.3609902
+1.18,3.6009322,3.4342207
+1.25,3.698148,3.5123265
+1.33,3.8097162,3.5906589
+1.43,3.9419174,3.7122171
+1.54,4.0126191,3.8077018
+1.67,4.2746437,3.8609249
+1.82,4.4682212,3.8823682
+2,4.6752372,3.8164244
+2.11,4.7311251,3.7288987
+2.22,4.7418094,3.6030774
+2.35,4.6520327,3.3990496
+2.5,4.364761,3.1898829
+2.67,3.8144105,3.0741948
+2.86,3.0649496,3.5829978
+3.08,2.4004043,4.4865443
+3.33,2.3943002,5.4204022
+3.64,2.5809283,6.2578349
+4,2.7313635,7.0189943
+4.44,2.8327334,7.7291731
+5,2.3660792,8.7896083
+5.71,2.1867059,10.53627
+6.67,2.4841185,12.895769
+8,3.2048691,15.799043
+10,4.0715739,19.664351
+11.1,4.5921948,21.789718
+12.5,5.29318,24.380236
+14.3,6.2397504,27.621553
+16.7,7.5817542,31.846917
+20,9.6744916,37.605191
+22.2,11.217047,41.326081
+25,13.29969,45.839465
+28.6,16.284041,51.475157
+33.3,20.880752,58.046709
+40,27.169229,65.925258
+44.4,31.260311,70.562709
+50,36.217641,75.809491
+57.1,42.303853,81.834224
+66.7,49.906684,88.904473
+80,59.644857,97.484039
+100,72.530316,108.42373
+125,86.399911,120.07897
+154,100.49717,131.88977
+200,119.99544,148.43379
```

### Comparing `layerlumos-1.0.0/layerlumos/materials/W_Ordal.csv` & `layerlumos-1.0.1/layerlumos/materials/W_Ordal.csv`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-wl,n,k
-0.667,3.8312601,2.9042727
-0.714,3.9313491,2.7924078
-0.769,3.778336,2.6322954
-0.833,3.5190631,2.76706
-0.909,3.2814572,3.0100921
-1,3.0826871,3.4208368
-1.05,3.0570934,3.722401
-1.11,3.0821649,3.9693342
-1.18,3.1599449,4.1791582
-1.25,3.1960757,4.3367596
-1.33,3.1990778,4.4460869
-1.43,3.0278249,4.3901355
-1.54,2.2587782,4.7741297
-1.67,1.8828191,5.4881071
-1.82,1.5455798,6.4453363
-2,1.2992808,7.5659499
-2.11,1.1946455,8.2613235
-2.22,1.221203,9.0476312
-2.35,1.2886548,9.8569158
-2.5,1.4507921,10.710594
-2.67,1.6746349,11.554665
-2.86,1.8748013,12.375593
-3.08,1.91692,13.261664
-3.33,1.8505739,14.40046
-3.64,1.8774806,15.887186
-4,1.9949739,17.69477
-4.44,2.2388765,19.89851
-5,2.6672954,22.612178
-5.71,3.3712766,26.005432
-6.67,4.4961625,30.343034
-8,6.2868052,36.072044
-10,9.1935519,44.019189
-11.1,10.843912,48.146015
-12.5,12.935818,53.112521
-14.3,15.634532,59.208636
-16.7,19.231714,66.923752
-20,24.256111,77.087223
-22.2,27.599188,83.517367
-25,31.77255,91.217414
-28.6,37.127733,100.62038
-33.3,44.209069,112.34062
-40,54.191208,128.08146
-44.4,61.731428,136.67195
-50,68.665703,146.58093
-57.1,76.505227,159.83902
-66.7,87.148396,177.92054
-80,103.53408,202.21197
-100,130.219,234.03939
-125,163.02849,265.86909
-154,196.84283,294.94073
-200,242.14161,332.81796
+wl,n,k
+0.667,3.8312601,2.9042727
+0.714,3.9313491,2.7924078
+0.769,3.778336,2.6322954
+0.833,3.5190631,2.76706
+0.909,3.2814572,3.0100921
+1,3.0826871,3.4208368
+1.05,3.0570934,3.722401
+1.11,3.0821649,3.9693342
+1.18,3.1599449,4.1791582
+1.25,3.1960757,4.3367596
+1.33,3.1990778,4.4460869
+1.43,3.0278249,4.3901355
+1.54,2.2587782,4.7741297
+1.67,1.8828191,5.4881071
+1.82,1.5455798,6.4453363
+2,1.2992808,7.5659499
+2.11,1.1946455,8.2613235
+2.22,1.221203,9.0476312
+2.35,1.2886548,9.8569158
+2.5,1.4507921,10.710594
+2.67,1.6746349,11.554665
+2.86,1.8748013,12.375593
+3.08,1.91692,13.261664
+3.33,1.8505739,14.40046
+3.64,1.8774806,15.887186
+4,1.9949739,17.69477
+4.44,2.2388765,19.89851
+5,2.6672954,22.612178
+5.71,3.3712766,26.005432
+6.67,4.4961625,30.343034
+8,6.2868052,36.072044
+10,9.1935519,44.019189
+11.1,10.843912,48.146015
+12.5,12.935818,53.112521
+14.3,15.634532,59.208636
+16.7,19.231714,66.923752
+20,24.256111,77.087223
+22.2,27.599188,83.517367
+25,31.77255,91.217414
+28.6,37.127733,100.62038
+33.3,44.209069,112.34062
+40,54.191208,128.08146
+44.4,61.731428,136.67195
+50,68.665703,146.58093
+57.1,76.505227,159.83902
+66.7,87.148396,177.92054
+80,103.53408,202.21197
+100,130.219,234.03939
+125,163.02849,265.86909
+154,196.84283,294.94073
+200,242.14161,332.81796
```

### Comparing `layerlumos-1.0.0/layerlumos/utils.py` & `layerlumos-1.0.1/layerlumos/utils_materials.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,160 +1,170 @@
-import csv
-import json
-import os
-from pathlib import Path
-import numpy as np
-from scipy.interpolate import interp1d
-from scipy.constants import c
-
-Metals_sigma = {
-    'Cu': 5.96e7,
-    'Cr': 7.74e6,
-    'Ag': 6.3e7,
-    'Al': 3.77e7,
-    'Ni' : 1.43e7,
-    'W' : 1.79e7,
-    'Ti' : 2.38e6,
-    'Pd' : 9.52e6
-}
-Metals_nk_updated_specific_sigma = {}
-mu0 = 4 * np.pi * 1e-7  # H/m
-Z_0 = 377  # Ohms, impedance of free space
-# Frequency range
-nu = np.linspace(8e9, 18e9, 11)  # From 8 GHz to 18 GHz
-omega = 2 * np.pi * nu  # Angular frequency
-for metal, sigma in Metals_sigma.items():
-    Z = np.sqrt(1j * omega * mu0 / sigma)  # Impedance of the material using specific sigma
-    n_complex = Z_0 / Z  # Complex refractive index
-
-    # Extract real and imaginary parts of the refractive index
-    n_real = np.real(n_complex)
-    k_imag = np.imag(n_complex)
-    
-    # Update the dictionary with the new values
-    Metals_nk_updated_specific_sigma[metal] = {
-        'freq_data': nu.tolist(),
-        'n_data': n_real.tolist(),
-        'k_data': k_imag.tolist()
-    }
-def load_material_RF(material_name, frequencies):
-    """
-    Load material RF data for a given material and frequencies.
-    
-    Parameters:
-    - material_name: The name of the material to load.
-    - frequencies: Array of frequencies for which data is requested.
-    
-    Returns:
-    - A NumPy array with columns for frequency, n, and k.
-    """
-    # Check if the material is defined
-    if material_name not in Metals_nk_updated_specific_sigma:
-        # Material not found, return default values (n=1, k=0) for given frequencies
-        n_default = np.ones_like(frequencies)
-        k_default = np.zeros_like(frequencies)
-        data = np.column_stack((frequencies, n_default, k_default))
-    else:
-        # Material found, extract the data
-        material_data = Metals_nk_updated_specific_sigma[material_name]
-        freq_data = np.array(material_data['freq_data'])
-        n_data = np.array(material_data['n_data'])
-        k_data = np.array(material_data['k_data'])
-        
-        # Interpolate n and k data for the input frequencies, if necessary
-        n_interpolated = np.interp(frequencies, freq_data, n_data)
-        k_interpolated = np.interp(frequencies, freq_data, k_data)
-        
-        # Combine the data
-        data = np.column_stack((frequencies, n_interpolated, k_interpolated))
-    
-    return data
-
-
-
-def load_material(material_name):
-    """
-    Load material data from its CSV file, converting wavelength to frequency.
-
-    Parameters:
-    - material_name: The name of the material to load.
-    
-    Returns:
-    - A NumPy array with columns for frequency (converted from wavelength), n, and k.
-    """
-    # Determine the directory of the current script
-    current_dir = Path(__file__).parent
-
-    # Build the absolute path to materials.json
-    materials_file = current_dir / "materials.json"
-
-    # Load the material index JSON to find the CSV file path
-    with open(materials_file, 'r') as file:
-        material_index = json.load(file)
-    
-    # Get the file path for the requested material
-    relative_file_path = material_index.get(material_name)
-    if not relative_file_path:
-        raise ValueError(f"Material {material_name} not found in the index.")
-    
-    # Construct the absolute path to the material CSV file
-    csv_file_path = current_dir / relative_file_path
-
-    # Initialize a list to hold the converted data
-    data = []
-    
-    # Open and read the CSV file
-    with open(csv_file_path, 'r') as csvfile:
-        csvreader = csv.reader(csvfile)
-        next(csvreader)  # Skip the header row
-        for row in csvreader:
-            try:
-                # Attempt to convert wavelength, n, and k to floats
-                wavelength_um, n, k = map(float, row)
-                # Convert wavelength in um to frequency in Hz
-                frequency = c / (wavelength_um * 1e-6)
-                data.append((frequency, n, k))
-            except ValueError:
-                # If conversion fails, skip this row
-                continue
-    
-    # Convert to a NumPy array for easier handling in calculations
-    data = np.array(data)
-    # Ensure the data is sorted by frequency in ascending order
-    data = data[data[:, 0].argsort()]
-    
-    return data
-
-def interpolate_material(material_data, frequencies):
-    """
-    Interpolate n and k values for the specified frequencies.
-
-    Parameters:
-    - material_data: The data for the material, as returned by load_material.
-    - frequencies: A list or NumPy array of frequencies to interpolate n and k for.
-    
-    Returns:
-    - Interpolated values of n and k as a NumPy array.
-    """
-    # Extract frequency, n, and k columns
-    freqs, n_values, k_values = material_data.T
-    
-    # Remove duplicates (if any) while preserving order
-    unique_freqs, indices = np.unique(freqs, return_index=True)
-    unique_n_values = n_values[indices]
-    unique_k_values = k_values[indices]
-    
-    # Ensure frequencies are sorted (usually they should be, but just in case)
-    sorted_indices = np.argsort(unique_freqs)
-    sorted_freqs = unique_freqs[sorted_indices]
-    sorted_n_values = unique_n_values[sorted_indices]
-    sorted_k_values = unique_k_values[sorted_indices]
-    
-    # Create interpolation functions for the sorted, unique data
-    n_interp = interp1d(sorted_freqs, sorted_n_values, kind='cubic', fill_value="extrapolate")
-    k_interp = interp1d(sorted_freqs, sorted_k_values, kind='cubic', fill_value="extrapolate")
-    
-    # Interpolate n and k for the given frequencies
-    n_interp_values = n_interp(frequencies)
-    k_interp_values = k_interp(frequencies)
-    
-    return np.vstack((n_interp_values, k_interp_values)).T
+import numpy as np
+import csv
+import json
+from pathlib import Path
+import scipy.interpolate as scii
+import scipy.constants as scic
+
+from .utils_spectra import convert_frequencies_to_wavelengths
+
+
+Metals_sigma = {
+    'Cu': 5.96e7,
+    'Cr': 7.74e6,
+    'Ag': 6.3e7,
+    'Al': 3.77e7,
+    'Ni' : 1.43e7,
+    'W' : 1.79e7,
+    'Ti' : 2.38e6,
+    'Pd' : 9.52e6
+}
+
+Metals_nk_updated_specific_sigma = {}
+mu0 = 4 * np.pi * 1e-7  # H/m
+Z_0 = scic.physical_constants['characteristic impedance of vacuum'][0]  # Ohms, impedance of free space
+# Frequency range
+nu = np.linspace(8e9, 18e9, 11)  # From 8 GHz to 18 GHz
+omega = 2 * np.pi * nu  # Angular frequency
+
+for metal, sigma in Metals_sigma.items():
+    Z = np.sqrt(1j * omega * mu0 / sigma)  # Impedance of the material using specific sigma
+    n_complex = Z_0 / Z  # Complex refractive index
+
+    # Extract real and imaginary parts of the refractive index
+    n_real = np.real(n_complex)
+    k_imag = np.imag(n_complex)
+
+    # Update the dictionary with the new values
+    Metals_nk_updated_specific_sigma[metal] = {
+        'freq_data': nu.tolist(),
+        'n_data': n_real.tolist(),
+        'k_data': k_imag.tolist()
+    }
+
+
+def load_material_RF(material_name, frequencies):
+    """
+    Load material RF data for a given material and frequencies.
+
+    Parameters:
+    - material_name: The name of the material to load.
+    - frequencies: Array of frequencies for which data is requested.
+
+    Returns:
+    - A NumPy array with columns for frequency, n, and k.
+
+    """
+
+    # Check if the material is defined
+    if material_name not in Metals_nk_updated_specific_sigma:
+        # Material not found, return default values (n=1, k=0) for given frequencies
+        n_default = np.ones_like(frequencies)
+        k_default = np.zeros_like(frequencies)
+        data = np.column_stack((frequencies, n_default, k_default))
+    else:
+        # Material found, extract the data
+        material_data = Metals_nk_updated_specific_sigma[material_name]
+        freq_data = np.array(material_data['freq_data'])
+        n_data = np.array(material_data['n_data'])
+        k_data = np.array(material_data['k_data'])
+
+        # Interpolate n and k data for the input frequencies, if necessary
+        n_interpolated = np.interp(frequencies, freq_data, n_data)
+        k_interpolated = np.interp(frequencies, freq_data, k_data)
+
+        # Combine the data
+        data = np.column_stack((frequencies, n_interpolated, k_interpolated))
+
+    return data
+
+def load_material(material_name):
+    """
+    Load material data from its CSV file, converting wavelength to frequency.
+
+    Parameters:
+    - material_name: The name of the material to load.
+
+    Returns:
+    - A NumPy array with columns for frequency (converted from wavelength), n, and k.
+
+    """
+
+    # Determine the directory of the current script
+    current_dir = Path(__file__).parent
+
+    # Build the absolute path to materials.json
+    materials_file = current_dir / "materials.json"
+
+    # Load the material index JSON to find the CSV file path
+    with open(materials_file, 'r') as file:
+        material_index = json.load(file)
+
+    # Get the file path for the requested material
+    relative_file_path = material_index.get(material_name)
+    if not relative_file_path:
+        raise ValueError(f"Material {material_name} not found in the index.")
+
+    # Construct the absolute path to the material CSV file
+    csv_file_path = current_dir / relative_file_path
+
+    # Initialize a list to hold the converted data
+    data = []
+
+    # Open and read the CSV file
+    with open(csv_file_path, 'r') as csvfile:
+        csvreader = csv.reader(csvfile)
+        next(csvreader)  # Skip the header row
+        for row in csvreader:
+            try:
+                # Attempt to convert wavelength, n, and k to floats
+                wavelength_um, n, k = map(float, row)
+                # Convert wavelength in um to frequency in Hz
+                frequency = convert_frequencies_to_wavelengths(wavelength_um * 1e-6)
+                data.append((frequency, n, k))
+            except ValueError:
+                # If conversion fails, skip this row
+                continue
+
+    # Convert to a NumPy array for easier handling in calculations
+    data = np.array(data)
+    # Ensure the data is sorted by frequency in ascending order
+    data = data[data[:, 0].argsort()]
+
+    return data
+
+def interpolate_material(material_data, frequencies):
+    """
+    Interpolate n and k values for the specified frequencies.
+
+    Parameters:
+    - material_data: The data for the material, as returned by load_material.
+    - frequencies: A list or NumPy array of frequencies to interpolate n and k for.
+
+    Returns:
+    - Interpolated values of n and k as a NumPy array.
+
+    """
+
+    # Extract frequency, n, and k columns
+    freqs, n_values, k_values = material_data.T
+
+    # Remove duplicates (if any) while preserving order
+    unique_freqs, indices = np.unique(freqs, return_index=True)
+    unique_n_values = n_values[indices]
+    unique_k_values = k_values[indices]
+
+    # Ensure frequencies are sorted (usually they should be, but just in case)
+    sorted_indices = np.argsort(unique_freqs)
+    sorted_freqs = unique_freqs[sorted_indices]
+    sorted_n_values = unique_n_values[sorted_indices]
+    sorted_k_values = unique_k_values[sorted_indices]
+
+    # Create interpolation functions for the sorted, unique data
+    n_interp = scii.interp1d(sorted_freqs, sorted_n_values, kind='cubic', fill_value="extrapolate")
+    k_interp = scii.interp1d(sorted_freqs, sorted_k_values, kind='cubic', fill_value="extrapolate")
+
+    # Interpolate n and k for the given frequencies
+    n_interp_values = n_interp(frequencies)
+    k_interp_values = k_interp(frequencies)
+
+    return np.vstack((n_interp_values, k_interp_values)).T
```

### Comparing `layerlumos-1.0.0/layerlumos.egg-info/PKG-INFO` & `layerlumos-1.0.1/layerlumos.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,74 @@
-Metadata-Version: 2.1
-Name: layerlumos
-Version: 1.0.0
-Summary: An open-source software for TMM optical simulations.
-Author-email: Mingxuan Li <mil152@pitt.edu>
-License: MIT
-Project-URL: Homepage, https://github.com/mil152/layerlumos
-Project-URL: Source, https://github.com/mil152/layerlumos
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: wheel; extra == "dev"
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# LayerLumos
-![LayerLumos Icon](/docs/assets/icon3.jpg)
-## Overview
-
-**LayerLumos** is an open-source software designed for scientists, engineers, and researchers in optics and photonics. It provides a powerful yet intuitive interface for calculating the reflection and transmission (RT) of light through multi-layer optical structures. By inputting the refractive index, thickness of each layer, and the frequency vector, users can analyze how light interacts with layered materials, including the option to adjust for incidence angles.
-
-Our mission is to offer a lightweight, flexible, and fast alternative to commercial software, enabling users to perform complex optical simulations with ease. LayerLumos is built with performance and usability in mind, facilitating the exploration of optical phenomena in research and development settings.
-
-## Features
-
-- **Lightweight and Efficient**: Optimized for performance, LayerLumos ensures rapid calculations without the overhead of large-scale commercial software.
-- **Flexibility**: Accommodates a wide range of materials and structures by allowing users to specify complex refractive indices, layer thicknesses, and frequency vectors.
-- **Angle of Incidence Support**: Expands simulation capabilities to include angled light incidence, providing more detailed analysis for advanced optical designs.
-- **Open Source and Community-Driven**: Encourages contributions and feedback from the community, ensuring continuous improvement and innovation.
-- **Comprehensive Material Database**: Includes a growing database of materials with their optical properties, streamlining the simulation setup process.
-
-## Getting Started
-
-1. **Installation**: Instructions on how to install LayerLumos on various operating systems.
-2. **Quick Start Guide**: A brief tutorial on how to perform your first RT calculation using LayerLumos.
-3. **Examples**: Explore a collection of examples illustrating various use cases and capabilities of LayerLumos.
-
-## License
-
-LayerLumos is released under the [MIT License](https://github.com/Mil152/LayerLumos/blob/main/LICENSE), promoting open and unrestricted access to software for academic and commercial use.
-
-## Acknowledgments
-
-- Thanks to all contributors and users for your support and feedback.
+Metadata-Version: 2.1
+Name: layerlumos
+Version: 1.0.1
+Summary: An open-source software for TMM optical simulations
+Author-email: Mingxuan Li <mil152@pitt.edu>
+License: MIT
+Project-URL: Homepage, https://github.com/mil152/layerlumos
+Project-URL: Source, https://github.com/mil152/layerlumos
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+
+# LayerLumos
+
+<p align="center">
+<img src="https://raw.githubusercontent.com/mil152/LayerLumos/main/docs/assets/icon3.jpg" width="400" />
+</p>
+
+## Overview
+
+**LayerLumos** is an open-source software designed for scientists, engineers, and researchers in optics and photonics. It provides a powerful yet intuitive interface for calculating the reflection and transmission (RT) of light through multi-layer optical structures. By inputting the refractive index, thickness of each layer, and the frequency vector, users can analyze how light interacts with layered materials, including the option to adjust for incidence angles.
+
+Our mission is to offer a lightweight, flexible, and fast alternative to commercial software, enabling users to perform complex optical simulations with ease. LayerLumos is built with performance and usability in mind, facilitating the exploration of optical phenomena in research and development settings.
+
+For details, check out our [Documentation](https://mil152.github.io/LayerLumos/index.html).
+
+## Features
+
+- **Lightweight and Efficient**: Optimized for performance, LayerLumos ensures rapid calculations without the overhead of large-scale commercial software.
+- **Flexibility**: Accommodates a wide range of materials and structures by allowing users to specify complex refractive indices, layer thicknesses, and frequency vectors.
+- **Angle of Incidence Support**: Expands simulation capabilities to include angled light incidence, providing more detailed analysis for advanced optical designs.
+- **Open Source and Community-Driven**: Encourages contributions and feedback from the community, ensuring continuous improvement and innovation.
+- **Comprehensive Material Database**: Includes a growing database of materials with their optical properties, streamlining the simulation setup process.
+
+## Getting Started
+
+### Installation
+
+LayerLumos can be easily installed via pip:
+
+```bash
+pip install layerlumos
+```
+
+For more detailed installation instructions, please refer to our [Installation Guide](https://github.com/Mil152/LayerLumos/docs/installation.md).
+
+### Quick Start Guide
+
+To get started with your first RT calculation, check out our [Quick Start Guide](https://github.com/Mil152/LayerLumos/docs/quickstart.md).
+
+### Examples
+
+Explore a collection of examples illustrating various use cases and capabilities of LayerLumos in the [Examples Directory](https://mil152.github.io/LayerLumos/examples.html#jupyter-notebook-examples).
+
+## License
+
+LayerLumos is released under the [MIT License](LICENSE), promoting open and unrestricted access to software for academic and commercial use.
+
+## Acknowledgments
+
+- Thanks to all contributors and users for your support and feedback.
```

### Comparing `layerlumos-1.0.0/layerlumos.egg-info/SOURCES.txt` & `layerlumos-1.0.1/layerlumos.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .gitignore
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
-pytest.ini
+.github/workflows/publish.yml
+.github/workflows/pytest.yml
 .github/workflows/static.yml
-docs/API_Documentation.md
 docs/Makefile
 docs/_config.yml
 docs/conf.py
-docs/examples.md
 docs/examples.rst
 docs/getting-started.md
-docs/index.md
+docs/home.md
 docs/index.rst
 docs/make.bat
 docs/modules.rst
 docs/api/index.html
 docs/api/layerlumos.html
 docs/api/utils.html
 docs/assets/Icon1.jpg
@@ -26,15 +26,16 @@
 docs/examples/angle_example.ipynb
 docs/examples/compare_res_lumerical.py
 docs/examples/simple_example.ipynb
 docs/examples/time_compare_lumerical.py
 layerlumos/__init__.py
 layerlumos/layerlumos.py
 layerlumos/materials.json
-layerlumos/utils.py
+layerlumos/utils_materials.py
+layerlumos/utils_spectra.py
 layerlumos.egg-info/PKG-INFO
 layerlumos.egg-info/SOURCES.txt
 layerlumos.egg-info/dependency_links.txt
 layerlumos.egg-info/requires.txt
 layerlumos.egg-info/top_level.txt
 layerlumos/materials/Ag_Yang.csv
 layerlumos/materials/Al2O3_Querry.csv
@@ -44,12 +45,13 @@
 layerlumos/materials/Pd_Werner.csv
 layerlumos/materials/Si3N4_Kischkat.csv
 layerlumos/materials/SiO2_Kischkat.csv
 layerlumos/materials/TiN_Beliaev.csv
 layerlumos/materials/TiO2_Siefke.csv
 layerlumos/materials/Ti_Ordal.csv
 layerlumos/materials/W_Ordal.csv
-tests/__init__.py
-tests/test_RF.py
 tests/test_angle.py
+tests/test_import.py
 tests/test_materials.py
-tests/test_stackrt.py
+tests/test_radio_frequency.py
+tests/test_stackrt.py
+tests/test_version.py
```

### Comparing `layerlumos-1.0.0/tests/test_RF.py` & `layerlumos-1.0.1/tests/test_radio_frequency.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-import numpy as np
-from layerlumos.utils import load_material_RF
-from layerlumos.layerlumos import stackrt0
-
-def test_stackrt0_RF():
-    # Define frequency range
-    frequencies = np.linspace(8e9, 18e9, 100)  # Frequency range from 8GHz to 18GHz
-
-    # Load material data for 'Ag' over the specified frequency range
-    n_k_si02 = load_material_RF('Ag', frequencies)
-    n_si02 = n_k_si02[:, 1] + 1j*n_k_si02[:, 2]  # Combine n and k into a complex refractive index
-
-    # Define stack configuration
-    n_air = np.ones_like(frequencies)  # Refractive index of air
-    d_air = np.array([0])  # Air layer thickness
-    d_si02 = np.array([5e-8])  # SiO2 layer thickness
-
-    # Stack refractive indices and thicknesses for air-SiO2-air
-    n_stack = np.vstack([n_air, n_si02, n_air]).T  # Transpose to match expected shape
-    d_stack = np.vstack([d_air, d_si02, d_air])  # Stack thickness
-
-    # Calculate R and T over the frequency range
-    R_TE, T_TE, R_TM, T_TM = stackrt0(n_stack, d_stack, frequencies)
-
-    # Calculate average shielding effectiveness
-    SE_TE = -10 * np.log10(T_TE)
-    SE_TM = -10 * np.log10(T_TM)
-    SE = (SE_TE + SE_TM) / 2
-
-    expected_mean_SE = 55.47150237872992
-    # Assert that the actual mean SE is close to the expected value
-    np.testing.assert_allclose(np.mean(SE), expected_mean_SE, rtol=1e-5)
+import numpy as np
+
+from layerlumos.utils_materials import load_material_RF
+from layerlumos.layerlumos import stackrt0
+
+
+def test_stackrt0_RF():
+    # Define frequency range
+    frequencies = np.linspace(8e9, 18e9, 100)  # Frequency range from 8GHz to 18GHz
+
+    # Load material data for 'Ag' over the specified frequency range
+    n_k_si02 = load_material_RF('Ag', frequencies)
+    n_si02 = n_k_si02[:, 1] + 1j*n_k_si02[:, 2]  # Combine n and k into a complex refractive index
+
+    # Define stack configuration
+    n_air = np.ones_like(frequencies)  # Refractive index of air
+    d_air = np.array([0])  # Air layer thickness
+    d_si02 = np.array([5e-8])  # SiO2 layer thickness
+
+    # Stack refractive indices and thicknesses for air-SiO2-air
+    n_stack = np.vstack([n_air, n_si02, n_air]).T  # Transpose to match expected shape
+    d_stack = np.vstack([d_air, d_si02, d_air])  # Stack thickness
+
+    # Calculate R and T over the frequency range
+    R_TE, T_TE, R_TM, T_TM = stackrt0(n_stack, d_stack, frequencies)
+
+    # Calculate average shielding effectiveness
+    SE_TE = -10 * np.log10(T_TE)
+    SE_TM = -10 * np.log10(T_TM)
+    SE = (SE_TE + SE_TM) / 2
+
+    expected_mean_SE = 55.45905006672689
+    # Assert that the actual mean SE is close to the expected value
+    np.testing.assert_allclose(np.mean(SE), expected_mean_SE, rtol=1e-5)
```

### Comparing `layerlumos-1.0.0/tests/test_materials.py` & `layerlumos-1.0.1/tests/test_materials.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-import pytest
-import numpy as np
-from layerlumos.utils import load_material
-from scipy.constants import c
-
-def test_load_material_success():
-    """Test loading a material data successfully."""
-    # Assuming "SiO2" is a material in your database with a known data structure
-    material_name = "SiO2"
-    data = load_material(material_name)
-    
-    # Check that the data is not empty
-    assert data.size > 0
-
-    # Check for the correct structure: frequency, n, k
-    # Assuming at least one data row exists
-    assert len(data[0]) == 3
-
-def test_load_material_failure():
-    """Test loading a non-existent material data to ensure it fails gracefully."""
-    with pytest.raises(ValueError) as e:
-        load_material("FakeMaterial")
-    
-    assert str(e.value) == "Material FakeMaterial not found in the index."
-
-def test_material_data_conversion_and_interpolation():
-    """Test that the material data is correctly converted from wavelength to frequency
-    and that n and k values are correctly retrieved."""
-    material_name = "SiO2"
-    data = load_material(material_name)
-
-    # Values for a known row of SiO2 data
-    expected_wavelength_um = 22.321
-    expected_n = 1.804
-    expected_k = 1.536
-
-    # Convert the expected wavelength to frequency for comparison
-    expected_frequency_hz = c / (expected_wavelength_um * 1e-6)
-
-    # Find the row in the data where the frequency matches the expected frequency
-    # We use np.isclose to handle floating-point comparison
-    row = next((row for row in data if np.isclose(row[0], expected_frequency_hz, atol=1e-6)), None)
-
-    assert row is not None, f"Data row with frequency {expected_frequency_hz} not found."
-
-    # Extract the actual n and k values from the data
-    _, actual_n, actual_k = row
-
-    # Check that the actual n and k values match the expected values within a tolerance
-    assert np.isclose(actual_n, expected_n, atol=1e-6), f"Expected n: {expected_n}, but got: {actual_n}"
-    assert np.isclose(actual_k, expected_k, atol=1e-6), f"Expected k: {expected_k}, but got: {actual_k}"
-
+import pytest
+import numpy as np
+import scipy.constants as scic
+
+from layerlumos.utils_materials import load_material
+
+
+def test_load_material_success():
+    """Test loading a material data successfully."""
+    # Assuming "SiO2" is a material in your database with a known data structure
+    material_name = "SiO2"
+    data = load_material(material_name)
+    
+    # Check that the data is not empty
+    assert data.size > 0
+
+    # Check for the correct structure: frequency, n, k
+    # Assuming at least one data row exists
+    assert len(data[0]) == 3
+
+def test_load_material_failure():
+    """Test loading a non-existent material data to ensure it fails gracefully."""
+    with pytest.raises(ValueError) as e:
+        load_material("FakeMaterial")
+    
+    assert str(e.value) == "Material FakeMaterial not found in the index."
+
+def test_material_data_conversion_and_interpolation():
+    """Test that the material data is correctly converted from wavelength to frequency
+    and that n and k values are correctly retrieved."""
+    material_name = "SiO2"
+    data = load_material(material_name)
+
+    # Values for a known row of SiO2 data
+    expected_wavelength_um = 22.321
+    expected_n = 1.804
+    expected_k = 1.536
+
+    # Convert the expected wavelength to frequency for comparison
+    expected_frequency_hz = scic.c / (expected_wavelength_um * 1e-6)
+
+    # Find the row in the data where the frequency matches the expected frequency
+    # We use np.isclose to handle floating-point comparison
+    row = next((row for row in data if np.isclose(row[0], expected_frequency_hz, atol=1e-6)), None)
+
+    assert row is not None, f"Data row with frequency {expected_frequency_hz} not found."
+
+    # Extract the actual n and k values from the data
+    _, actual_n, actual_k = row
+
+    # Check that the actual n and k values match the expected values within a tolerance
+    assert np.isclose(actual_n, expected_n, atol=1e-6), f"Expected n: {expected_n}, but got: {actual_n}"
+    assert np.isclose(actual_k, expected_k, atol=1e-6), f"Expected k: {expected_k}, but got: {actual_k}"
```

### Comparing `layerlumos-1.0.0/tests/test_stackrt.py` & `layerlumos-1.0.1/tests/test_stackrt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-import unittest
-import numpy as np
-from scipy.constants import c
-# Assume utils and layerlumos are modules you've created or installed that contain the necessary functions
-from layerlumos.utils import load_material, interpolate_material
-from layerlumos.layerlumos import stackrt0
-
-class TestLayerLumos(unittest.TestCase):
-    def test_stackrt0(self):
-        # Load material data for SiO2 (example uses 'Ag', replace with 'SiO2' or appropriate material)
-        si02_data = load_material('Ag')
-
-        # Define a small wavelength range for testing
-        wavelengths = np.linspace(300e-9, 900e-9, 3)  # from 300nm to 700nm
-        frequencies = c / wavelengths  # Convert wavelengths to frequencies
-
-        # Interpolate n and k values for SiO2 over the specified frequency range
-        n_k_si02 = interpolate_material(si02_data, frequencies)
-        n_si02 = n_k_si02[:, 0] + 1j * n_k_si02[:, 1]
-
-        # Stack configuration
-        n_air = np.ones_like(wavelengths)
-        d_air = np.array([0])
-        d_si02 = np.array([2e-6])
-
-        n_stack = np.vstack([n_air, n_si02, n_air]).T
-        d_stack = np.vstack([d_air, d_si02, d_air])
-
-        # Calculate R and T over the frequency range
-        R_TE, T_TE, R_TM, T_TM = stackrt0(n_stack, d_stack, frequencies)
-
-        # Calculate average R and T
-        R_avg = (R_TE + R_TM) / 2
-        T_avg = (T_TE + T_TM) / 2
-
-        # Expected output (based on your script; might need adjustment based on actual results)
-        expected_R_avg = np.array([0.15756072, 0.98613162, 0.99031732])
-        expected_T_avg = np.array([5.87146690e-34, 1.58748575e-71, 5.13012036e-76])
-
-        # Validate the results with a tolerance for floating-point arithmetic
-        np.testing.assert_allclose(R_avg, expected_R_avg, rtol=1e-2, atol=0)
-        np.testing.assert_allclose(T_avg, expected_T_avg, rtol=1e-2, atol=0)
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+import numpy as np
+import scipy.constants as scic
+
+from layerlumos.utils_materials import load_material, interpolate_material
+from layerlumos.layerlumos import stackrt0
+
+
+class TestLayerLumos(unittest.TestCase):
+    def test_stackrt0(self):
+        # Load material data for SiO2 (example uses 'Ag', replace with 'SiO2' or appropriate material)
+        si02_data = load_material('Ag')
+
+        # Define a small wavelength range for testing
+        wavelengths = np.linspace(300e-9, 900e-9, 3)  # from 300nm to 700nm
+        frequencies = scic.c / wavelengths  # Convert wavelengths to frequencies
+
+        # Interpolate n and k values for SiO2 over the specified frequency range
+        n_k_si02 = interpolate_material(si02_data, frequencies)
+        n_si02 = n_k_si02[:, 0] + 1j * n_k_si02[:, 1]
+
+        # Stack configuration
+        n_air = np.ones_like(wavelengths)
+        d_air = np.array([0])
+        d_si02 = np.array([2e-6])
+
+        n_stack = np.vstack([n_air, n_si02, n_air]).T
+        d_stack = np.vstack([d_air, d_si02, d_air])
+
+        # Calculate R and T over the frequency range
+        R_TE, T_TE, R_TM, T_TM = stackrt0(n_stack, d_stack, frequencies)
+
+        # Calculate average R and T
+        R_avg = (R_TE + R_TM) / 2
+        T_avg = (T_TE + T_TM) / 2
+
+        # Expected output (based on your script; might need adjustment based on actual results)
+        expected_R_avg = np.array([0.15756072, 0.98613162, 0.99031732])
+        expected_T_avg = np.array([5.87146690e-34, 1.58748575e-71, 5.13012036e-76])
+
+        # Validate the results with a tolerance for floating-point arithmetic
+        np.testing.assert_allclose(R_avg, expected_R_avg, rtol=1e-2, atol=0)
+        np.testing.assert_allclose(T_avg, expected_T_avg, rtol=1e-2, atol=0)
+
+
+if __name__ == '__main__':
+    unittest.main()
```

