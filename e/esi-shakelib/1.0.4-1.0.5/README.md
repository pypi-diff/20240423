# Comparing `tmp/esi-shakelib-1.0.4.tar.gz` & `tmp/esi_shakelib-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esi-shakelib-1.0.4.tar", last modified: Tue Nov 28 19:36:24 2023, max compression
+gzip compressed data, was "esi_shakelib-1.0.5.tar", last modified: Tue Apr 23 17:52:06 2024, max compression
```

## Comparing `esi-shakelib-1.0.4.tar` & `esi_shakelib-1.0.5.tar`

### file list

```diff
@@ -1,85 +1,87 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.933524 esi-shakelib-1.0.4/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       42 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3467 2023-11-28 19:36:24.933524 esi-shakelib-1.0.4/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       99 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1494 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2023-11-28 19:36:24.933524 esi-shakelib-1.0.4/setup.cfg
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/setup.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.917524 esi-shakelib-1.0.4/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.921524 esi-shakelib-1.0.4/src/esi_shakelib/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.921524 esi-shakelib-1.0.4/src/esi_shakelib/conversions/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       27 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/convert_imc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/convert_imt.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.921524 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15879 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13647 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/boore_kishida_2017.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.925524 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30218 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30451 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31298 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31916 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31695 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31928 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31453 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31019 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30999 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.925524 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7121 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3159 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4240 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/newmark_hall_1982.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.925524 esi-shakelib-1.0.4/src/esi_shakelib/correlation/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/correlation/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/correlation/ccf_base.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2651 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/correlation/dummy.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7064 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/correlation/loth_baker_2013.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.925524 esi-shakelib-1.0.4/src/esi_shakelib/directivity/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/directivity/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17704 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/directivity/bayless2013.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25979 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/directivity/rowshandel2013.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.929524 esi-shakelib-1.0.4/src/esi_shakelib/gmice/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmice/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10279 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmice/ak07.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7612 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmice/fm11.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6246 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmice/gmice.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8815 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmice/wald99.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10744 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmice/wgrw12.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.929524 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10455 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.929524 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_small_mag/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_distances.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      195 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_periods.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pga.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pgv.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2730 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.929524 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_tables/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      326 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_tables/nga-east-seed-weights.dat
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3133 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      181 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_tables/readme
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3049 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nullgmpe.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    46908 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/multigmpe.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1452 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/multiutils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.929524 esi-shakelib-1.0.4/src/esi_shakelib/plotting/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/plotting/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6131 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/plotting/contour.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2219 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/plotting/plotrupture.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15298 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/sites.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    54714 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/station.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.929524 esi-shakelib-1.0.4/src/esi_shakelib/utils/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:35:21.000000 esi-shakelib-1.0.4/src/esi_shakelib/utils/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8155 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/utils/containers.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      217 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/utils/exception.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2109 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/utils/imt_string.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11876 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/utils/utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6325 2023-11-28 18:09:07.000000 esi-shakelib-1.0.4/src/esi_shakelib/virtualipe.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2023-11-28 19:36:24.933524 esi-shakelib-1.0.4/src/esi_shakelib.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3467 2023-11-28 19:36:24.000000 esi-shakelib-1.0.4/src/esi_shakelib.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3415 2023-11-28 19:36:24.000000 esi-shakelib-1.0.4/src/esi_shakelib.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2023-11-28 19:36:24.000000 esi-shakelib-1.0.4/src/esi_shakelib.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      450 2023-11-28 19:36:24.000000 esi-shakelib-1.0.4/src/esi_shakelib.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       13 2023-11-28 19:36:24.000000 esi-shakelib-1.0.4/src/esi_shakelib.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.098262 esi_shakelib-1.0.5/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1627 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       42 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-04-23 17:52:06.098262 esi_shakelib-1.0.5/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      517 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1522 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-23 17:52:06.098262 esi_shakelib-1.0.5/setup.cfg
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/setup.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.078262 esi_shakelib-1.0.5/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.086262 esi_shakelib-1.0.5/src/esi_shakelib/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.086262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       27 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6652 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imt.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.086262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15879 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13647 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/boore_kishida_2017.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30218 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30451 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31298 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31916 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31695 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31928 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31453 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    31019 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    30999 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7121 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3159 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4240 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/newmark_hall_1982.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/correlation/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/ccf_base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2651 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/dummy.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7064 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/correlation/loth_baker_2013.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/directivity/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/directivity/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17704 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/directivity/bayless2013.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25636 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/directivity/rowshandel2013.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    26785 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/ffsimmer.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7274 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/generic_site_amplitication.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.090262 esi_shakelib-1.0.5/src/esi_shakelib/gmice/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10279 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/ak07.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7612 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/fm11.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6246 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/gmice.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8815 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/wald99.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10744 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmice/wgrw12.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10920 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_distances.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      195 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_periods.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pga.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      210 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slope_pgv.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2730 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      326 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/nga-east-seed-weights.dat
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3133 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      181 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/readme
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3225 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nullgmpe.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    43334 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/multigmpe.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1722 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/multiutils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/plotting/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/plotting/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6131 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/plotting/contour.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2219 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/plotting/plotrupture.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    15298 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/sites.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    54714 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/station.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib/utils/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:51:02.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8155 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/containers.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      217 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/exception.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2109 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/imt_string.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11907 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/utils/utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6723 2024-04-23 17:42:10.000000 esi_shakelib-1.0.5/src/esi_shakelib/virtualipe.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-23 17:52:06.094262 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3920 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     3491 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      470 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       13 2024-04-23 17:52:06.000000 esi_shakelib-1.0.5/src/esi_shakelib.egg-info/top_level.txt
```

### Comparing `esi-shakelib-1.0.4/LICENSE.md` & `esi_shakelib-1.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/PKG-INFO` & `esi_shakelib-1.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-shakelib
-Version: 1.0.4
+Version: 1.0.5
 Summary: USGS Earthquake Impact Library for ShakeMap
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -65,14 +65,15 @@
 Requires-Dist: numpy>=1.21
 Requires-Dist: openquake.engine==3.18.0
 Requires-Dist: alpha-shapes>=1.0.0
 Requires-Dist: pandas>=2.1.1
 Requires-Dist: scipy>=1.11.2
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: scikit-image>=0.21.0
+Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: usgs-strec>=2.2.8
 Provides-Extra: dev
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: black>=21; extra == "dev"
 Requires-Dist: flake8>=3.9; extra == "dev"
 Requires-Dist: ipython>=7.26; extra == "dev"
 Provides-Extra: test
@@ -83,11 +84,25 @@
 Requires-Dist: twine; extra == "build"
 Requires-Dist: check-wheel-contents; extra == "build"
 
 # esi-shakelib
 
 ## Introduction
 
-Utility package for general ShakeMap functions.
+This repository contains a utility package for general ShakeMap functions that may be of use to other programs.
+Included are:
+
+- IMC and IMT conversions
+- Cross correlation functions
+- Directivity functions
+- GMICE functions
+- Specialized NGA-East GMPEs for small magnitude earthquakes
+- Contour and rupture plotting functions
+- Misc. other functions
+
+See the code for documentation.
 
 ## Installation
 
+The package is available on PyPI. Install with pip:
+
+    pip install esi-shakelib
```

### Comparing `esi-shakelib-1.0.4/pyproject.toml` & `esi_shakelib-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "numpy>=1.21",
     "openquake.engine==3.18.0",
     "alpha-shapes>=1.0.0",
     "pandas>=2.1.1",
     "scipy>=1.11.2",
     "shapely>=2.0.1",
     "scikit-image>=0.21.0",
+    "statsmodels>= 0.14.1",
     "usgs-strec>=2.2.8",
 ]
 
 [project.optional-dependencies]
 dev = [
     "build>=0.7.0",
     "black>=21",
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/convert_imc.py` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imc.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/convert_imt.py` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/convert_imt.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/beyer_bommer_2006.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/boore_kishida_2017.py` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/boore_kishida_2017.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D00D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D00.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D100D50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_D50GMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD100.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerD50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGM50.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imc/data/nga-w2.lmR1M2_LargerGMAR.4paper.RrupMin_0000.RrupMax_0400.Mmin_2.00.Mmax_9.00.csv`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/abrahamson_bhasin_2020.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/bommer_alarcon_2006.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/conversions/imt/newmark_hall_1982.py` & `esi_shakelib-1.0.5/src/esi_shakelib/conversions/imt/newmark_hall_1982.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/correlation/ccf_base.py` & `esi_shakelib-1.0.5/src/esi_shakelib/correlation/ccf_base.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/correlation/dummy.py` & `esi_shakelib-1.0.5/src/esi_shakelib/correlation/dummy.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/correlation/loth_baker_2013.py` & `esi_shakelib-1.0.5/src/esi_shakelib/correlation/loth_baker_2013.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/directivity/bayless2013.py` & `esi_shakelib-1.0.5/src/esi_shakelib/directivity/bayless2013.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/directivity/rowshandel2013.py` & `esi_shakelib-1.0.5/src/esi_shakelib/directivity/rowshandel2013.py`

 * *Files 4% similar despite different names*

```diff
@@ -238,16 +238,15 @@
 
         xcipc = self._xi_prime - self._xi_c
 
         # fd is a list with same length as T
         self._fd = [None] * len(self._T)
         self._DTlist = [None] * len(self._T)
         self._WPlist = [None] * len(self._T)
-        for i in range(len(self._T)):
-            period = self._T[i]
+        for i, period in enumerate(self._T):
             c1sel = self.__c1[self.__periods == period]
             c2sel = self.__c2[self.__periods == period]
 
             # Period dependent parameters
             self.__computeWP(period)
             self.__computeDT(period)
 
@@ -281,15 +280,17 @@
         # First find which quad the hypocenter is on
         # ---------------------------------------------------------------------
 
         x, y, z = latlon2ecef(self._hyp.latitude, self._hyp.longitude, self._hyp.depth)
         hyp_ecef = np.array([[x, y, z]])
         qdist = np.zeros(nquad)
         for i in range(0, nquad):
-            qdist[i] = utils._quad_distance(self._rup.getQuadrilaterals()[i], hyp_ecef)
+            qdist[i] = utils._quad_distance(self._rup.getQuadrilaterals()[i], hyp_ecef)[
+                0, 0
+            ]
         ind = int(np.where(qdist == np.min(qdist))[0][0])
         # *** check that this doesn't break with more than one quad
         q = self._rup.getQuadrilaterals()[ind]
 
         # ---------------------------------------------------------------------
         # Compute Wrup on that quad
         # ---------------------------------------------------------------------
@@ -640,43 +641,22 @@
     qlons = [a.longitude for a in q]
     proj = OrthographicProjection(
         np.min(qlons), np.max(qlons), np.min(qlats), np.max(qlats)
     )
 
     # Convert p and cp to geographic coords
     p0lat, p0lon, p0z = ecef2latlon(
-        cp[
-            0,
-        ],
-        cp[
-            1,
-        ],
-        cp[
-            2,
-        ],
+        cp[0,],
+        cp[1,],
+        cp[2,],
     )
     p1lat, p1lon, p1z = ecef2latlon(
-        cp[
-            0,
-        ]
-        + p[
-            0,
-        ],
-        cp[
-            1,
-        ]
-        + p[
-            1,
-        ],
-        cp[
-            2,
-        ]
-        + p[
-            2,
-        ],
+        cp[0,] + p[0,],
+        cp[1,] + p[1,],
+        cp[2,] + p[2,],
     )
 
     # Convert p to 'local' coords
     p0x, p0y = proj(p0lon, p0lat)
     p1x, p1y = proj(p1lon, p1lat)
     px = p1x - p0x
     py = p1y - p0y
@@ -702,47 +682,35 @@
     )
 
     # Need to track 'origin'
     s0 = np.array([[0], [0], [0]])
 
     # Convert from 'local' to geographic coords
     s1_ll = proj(
-        s1mat[
-            0,
-        ],
-        s1mat[
-            1,
-        ],
+        s1mat[0,],
+        s1mat[1,],
         reverse=True,
     )
     d1_ll = proj(
-        d1mat[
-            0,
-        ],
-        d1mat[
-            1,
-        ],
+        d1mat[0,],
+        d1mat[1,],
         reverse=True,
     )
     s0_ll = proj(s0[0], s0[1], reverse=True)
 
     # And then back to ECEF:
     s1_ecef = latlon2ecef(
         s1_ll[1],
         s1_ll[0],
-        s1mat[
-            2,
-        ],
+        s1mat[2,],
     )
     d1_ecef = latlon2ecef(
         d1_ll[1],
         d1_ll[0],
-        d1mat[
-            2,
-        ],
+        d1mat[2,],
     )
     s0_ecef = latlon2ecef(s0_ll[1], s0_ll[0], s0[2])
     s00 = s0_ecef[0].reshape(-1)
     s01 = s0_ecef[1].reshape(-1)
     s02 = s0_ecef[2].reshape(-1)
     d_mat = np.array(
         [
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmice/ak07.py` & `esi_shakelib-1.0.5/src/esi_shakelib/gmice/ak07.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmice/fm11.py` & `esi_shakelib-1.0.5/src/esi_shakelib/gmice/fm11.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmice/gmice.py` & `esi_shakelib-1.0.5/src/esi_shakelib/gmice/gmice.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmice/wald99.py` & `esi_shakelib-1.0.5/src/esi_shakelib/gmice/wald99.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmice/wgrw12.py` & `esi_shakelib-1.0.5/src/esi_shakelib/gmice/wgrw12.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east.py` & `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,14 +115,27 @@
             self.per_idx_start : self.per_idx_end
         ]
         self.per_array = np.array(
             [float(p.replace("SA", "").replace("P", ".")) for p in per_list_str]
         )
 
     def get_mean_and_stddevs(self, sites, rx, dists, imt, stddev_types):
+        if not isinstance(imt, list):
+            imt = [imt]
+        nstd = len(stddev_types)
+        mean = []
+        std = []
+        for iimt in imt:
+            mm, ss = self.__get_mean_and_stddevs__(sites, rx, dists, iimt, stddev_types)
+            mean.append(mm)
+            for i, sdt in enumerate(stddev_types):
+                std.append(ss[i])
+        return mean, std
+
+    def __get_mean_and_stddevs__(self, sites, rx, dists, imt, stddev_types):
         # List of GMPE weights, which is the product of the the branch weights
         # for the seed models vs the NGA East resampled models as well as the
         # weights for the indivudual GMPES as defined by Petersen et al. (2019)
         #
         # Note that the NGA East resampled models are a function of spectral
         # period.
         #
@@ -217,24 +230,24 @@
                     # No table for PGV, compute vimt, then convert to PGV
                     #
                     vmean, vstddevs = gmpe_gmas(gm, rup, vimt, stddev_types)
                     tmean, tstddevs = ab2020.getPGVandSTDDEVS(
                         vmean, vstddevs, stddev_types, rup.rrup, rup.vs30
                     )
                 except Exception:
-                    logging.error("Unexpected error:", sys.exc_info()[0])
+                    logging.error(f"Unexpected error: {sys.exc_info()[0]}")
                 else:
                     #
                     # Table exists for PGV, proceed normally
                     #
                     tmean, tstddevs = gmpe_gmas(gm, rup, imt, stddev_types)
             else:
                 tmean, tstddevs = gmpe_gmas(gm, rup, imt, stddev_types)
 
-            mean += tmean * total_gmpe_weights[i]
+            mean += tmean[0] * total_gmpe_weights[i]
             for j, sd in enumerate(tstddevs):
                 stddevs[j] += sd * total_gmpe_weights[i]
 
         # Zero out values at distances beyond the range for which NGA East
         # was defined. -->> was dists.rrup, now rup.rrup
         mean[rup.rrup > MAX_RRUP] = -999.0
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt` & `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_small_mag/nga-east-smallM_slopes.txt`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat` & `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nga_east_tables/nga-east-usgs-weights.dat`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/gmpe/nullgmpe.py` & `esi_shakelib-1.0.5/src/esi_shakelib/gmpe/nullgmpe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 A GMPE that returns a constant everywhere. Useful for testing, but
 nothing else.
 """
+
 import numpy as np
 
 from openquake.hazardlib.gsim.base import GMPE, CoeffsTable
 from openquake.hazardlib import const
 from openquake.hazardlib.imt import PGA, PGV, SA
 
 
@@ -40,38 +41,44 @@
                  GMPE (default=0.6)
 
         The total standard deviation returned will be ``sqrt(phi^2 + tau^2)``.
         """
         self.mean = mean
         self.phi = phi
         self.tau = tau
-        self.sigma = np.sqrt(phi ** 2 + tau ** 2)
+        self.sigma = np.sqrt(phi**2 + tau**2)
 
     def get_mean_and_stddevs(self, sites, rup, dists, imt, stddev_types):
         """
         Implements the OpenQuake GroundShakingIntensityModel
         get_mean_and_stddevs interface. See superclass
         `method <http://docs.openquake.org/oq-hazardlib/master/gsim/index.html#openquake.hazardlib.gsim.base.GroundShakingIntensityModel.get_mean_and_stddevs>`__.
 
         Returns a constant values for all locations specified in
         the dists.rbj array, regardless of the contents of that array or
         any of the other contexts. The imt is also ignored.
         """  # noqa
 
-        mean = np.full_like(dists.rjb, self.mean)
+        if isinstance(imt, list):
+            nlist = len(imt)
+        else:
+            nlist = 1
+        N = np.size(dists.rjb)
+        mean = np.zeros((nlist, N))
         stddevs = []
-        for stddev_type in stddev_types:
-            if stddev_type == const.StdDev.TOTAL:
-                stddevs.append(
-                    np.full_like(dists.rjb, np.sqrt(self.phi ** 2 + self.tau ** 2))
-                )
-            elif stddev_type == const.StdDev.INTRA_EVENT:
-                stddevs.append(np.full_like(dists.rjb, self.phi))
-            elif stddev_type == const.StdDev.INTER_EVENT:
-                stddevs.append(np.full_like(dists.rjb, self.tau))
+        for i in range(nlist):
+            for stddev_type in stddev_types:
+                if stddev_type == const.StdDev.TOTAL:
+                    stddevs.append(
+                        np.full_like(dists.rjb, np.sqrt(self.phi**2 + self.tau**2))
+                    )
+                elif stddev_type == const.StdDev.INTRA_EVENT:
+                    stddevs.append(np.full_like(dists.rjb, self.phi))
+                elif stddev_type == const.StdDev.INTER_EVENT:
+                    stddevs.append(np.full_like(dists.rjb, self.tau))
 
         return mean, stddevs
 
     #
     # Dummy COEFFS table so MultiGMPE won't complain
     #
     COEFFS = CoeffsTable(
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/multigmpe.py` & `esi_shakelib-1.0.5/src/esi_shakelib/multigmpe.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,116 +132,108 @@
     REQUIRES_RUPTURE_PARAMETERS = None
     REQUIRES_DISTANCES = None
 
     def get_mean_and_stddevs(self, sites, rup, dists, imt, stddev_types):
         """
         See superclass `method <http://docs.openquake.org/oq-hazardlib/master/gsim/index.html#openquake.hazardlib.gsim.base.GroundShakingIntensityModel.get_mean_and_stddevs>`__.
 
-        Unlike the superclass method, the stddev list returned by this
-        function will have twice as many arrays as are requested in
-        stddev_types: The first set will include the standard deviation
-        inflation due to the point-source to finite fault conversion (if
-        any), and the second set will not include this inflation. In the
-        case where a finite rupture is provided (and, thus, no point-source
-        to finite rupture adjustments are made) the two sets of stddev
-        arrays will be identical. Thus, if::
-
-            stddev_types = [const.StdDev.TOTAL, const.StdDev.INTRA_EVENT,
-                            const.StdDev.INTER_EVENT]
-
-        the returned stddev list will contain six arrays: the first three
-        will include the point-source inflation, and the second three will
-        not.
         """  # noqa
 
         # ---------------------------------------------------------------------
         # Sort out shapes of the sites and dists elements
         # Need to turn all 2D arrays into 1D arrays because of
         # inconsistencies in how arrays are handled in OpenQuake.
         # ---------------------------------------------------------------------
-        shapes = []
-        for k, v in sites.__dict__.items():
-            if k == "_slots_":
-                continue
-            if (k != "lons") and (k != "lats"):
-                shapes.append(v.shape)
-                sites.__dict__[k] = np.reshape(sites.__dict__[k], (-1,))
-        for k, v in dists.__dict__.items():
-            if k == "_slots_":
-                continue
-            if (k != "lons") and (k != "lats") and v is not None:
-                shapes.append(v.shape)
-                dists.__dict__[k] = np.reshape(dists.__dict__[k], (-1,))
-        shapeset = set(shapes)
-        if len(shapeset) != 1:
-            raise Exception("All dists and sites elements must have same shape.")
-        else:
-            orig_shape = list(shapeset)[0]
+        # shapes = []
+        # for k, v in sites.__dict__.items():
+        #     if k == "_slots_":
+        #         continue
+        #     if (k != "lons") and (k != "lats"):
+        #         shapes.append(v.shape)
+        #         sites.__dict__[k] = np.reshape(sites.__dict__[k], (-1,))
+        # for k, v in dists.__dict__.items():
+        #     if k == "_slots_":
+        #         continue
+        #     if (k != "lons") and (k != "lats") and v is not None:
+        #         shapes.append(v.shape)
+        #         dists.__dict__[k] = np.reshape(dists.__dict__[k], (-1,))
+        # shapeset = set(shapes)
+        # if len(shapeset) != 1:
+        #     raise Exception("All dists and sites elements must have same shape.")
+        # else:
+        #     orig_shape = list(shapeset)[0]
 
         sd_avail = self.DEFINED_FOR_STANDARD_DEVIATION_TYPES
         if not sd_avail.issuperset(set(stddev_types)):
             raise Exception("Requested an unavailable stddev_type.")
 
+        if not isinstance(imt, list):
+            imt = [imt]
         # Evaluate MultiGMPE:
         lnmu, lnsd = self.__get_mean_and_stddevs__(sites, rup, dists, imt, stddev_types)
 
         # Check for large-distance cutoff/weights
         if hasattr(self, "CUTOFF_DISTANCE"):
             lnmu_large, lnsd_large = self.__get_mean_and_stddevs__(
                 sites, rup, dists, imt, stddev_types, large_dist=True
             )
             # Stomp on lnmu and lnsd at large distances
             dist_cutoff = self.CUTOFF_DISTANCE
-            lnmu[dists.rjb > dist_cutoff] = lnmu_large[dists.rjb > dist_cutoff]
-            for i in range(len(lnsd)):
-                lnsd[i][dists.rjb > dist_cutoff] = lnsd_large[i][
+            for ix, iimt in enumerate(imt):
+                lnmu[ix][dists.rjb > dist_cutoff] = lnmu_large[ix][
+                    dists.rjb > dist_cutoff
+                ]
+            for i, this_lnsd in enumerate(lnsd):
+                this_lnsd[dists.rjb > dist_cutoff] = lnsd_large[i][
                     dists.rjb > dist_cutoff
                 ]
 
         # Undo reshapes of inputs
-        for k, v in dists.__dict__.items():
-            if k == "_slots_":
-                continue
-            if (k != "lons") and (k != "lats") and v is not None:
-                dists.__dict__[k] = np.reshape(dists.__dict__[k], orig_shape)
-        for k, v in sites.__dict__.items():
-            if k == "_slots_":
-                continue
-            if (k != "lons") and (k != "lats"):
-                sites.__dict__[k] = np.reshape(sites.__dict__[k], orig_shape)
+        # for k, v in dists.__dict__.items():
+        #     if k == "_slots_":
+        #         continue
+        #     if (k != "lons") and (k != "lats") and v is not None:
+        #         dists.__dict__[k] = np.reshape(dists.__dict__[k], orig_shape)
+        # for k, v in sites.__dict__.items():
+        #     if k == "_slots_":
+        #         continue
+        #     if (k != "lons") and (k != "lats"):
+        #         sites.__dict__[k] = np.reshape(sites.__dict__[k], orig_shape)
 
         # Reshape output
-        lnmu = np.reshape(lnmu, orig_shape)
-        for i in range(len(lnsd)):
-            lnsd[i] = np.reshape(lnsd[i], orig_shape)
+        # lnmu = np.reshape(lnmu, orig_shape)
+        # for i, this_lnsd in enumerate(lnsd):
+        #     this_lnsd = np.reshape(this_lnsd, orig_shape)
 
         return lnmu, lnsd
 
     def __get_mean_and_stddevs__(
         self, sites, rup, dists, imt, stddev_types, large_dist=False
     ):
 
+        nsd = len(stddev_types)
         # ---------------------------------------------------------------------
         # Sort out which set of weights to use
         # ---------------------------------------------------------------------
         if large_dist is False:
             wts = self.WEIGHTS
         else:
             wts = self.WEIGHTS_LARGE_DISTANCE
 
+        nimt = len(imt)
         # ---------------------------------------------------------------------
         # This is the array to hold the weighted combination of the GMPEs
         # ---------------------------------------------------------------------
-        lnmu = np.zeros_like(sites.vs30)
+        lnmu = np.zeros((nimt, np.size(sites.vs30)))
         # ---------------------------------------------------------------------
         # Hold on to the individual means and stddevs so we can compute the
         # combined stddev
         # ---------------------------------------------------------------------
-        lnmu_list = []
-        lnsd_list = []
+        lnmu_list = [[] for _ in range(nimt)]
+        lnsd_list = [[] for _ in range(nimt)]
 
         for i, gmpe in enumerate(self.GMPES):
             # -----------------------------------------------------------------
             # Loop over GMPE list
             # -----------------------------------------------------------------
 
             set_sites_depth_parameters(sites, gmpe)
@@ -252,21 +244,23 @@
 
             gmpe_imts = [
                 imt.__name__ for imt in list(gmpe.DEFINED_FOR_INTENSITY_MEASURE_TYPES)
             ]
 
             if (
                 not isinstance(gmpe, MultiGMPE)
-                and (imt.string == "PGV")
+                and PGV() in imt
                 and ("PGV" not in gmpe_imts)
             ):
                 ab2020 = AbrahamsonBhasin2020(rup.mag)
-                timt = SA(ab2020.getTref())
+                timt = copy.copy(imt)
+                pgv_ix = timt.index(PGV())
+                timt[pgv_ix] = SA(ab2020.getTref())
             else:
-                timt = imt
+                timt = copy.copy(imt)
 
             # -----------------------------------------------------------------
             # Grab GMPE_LIMITS in gmpe instance for later as the multigmpe
             # nests downward.
             # -----------------------------------------------------------------
             if hasattr(self, "GMPE_LIMITS"):
                 # Remember that GMPE_LIMITS is only present if it is getting
@@ -297,118 +291,120 @@
             else:
                 lmean, lsd = gmpe.get_mean_and_stddevs(
                     sites, rup, dists, timt, stddev_types
                 )
 
             if not isinstance(gmpe, MultiGMPE):
                 # -------------------------------------------------------------
-                # We may need to inflate the standard deviations to account for
-                # the point-source to finite rupture conversion.
-                # -------------------------------------------------------------
-                lsd_new = self.__inflatePSSigma__(
-                    gmpe, lmean, lsd, sites, rup, dists, timt, stddev_types
-                )
-                for sd in lsd:
-                    lsd_new.append(sd)
-                lsd = lsd_new
-
-                # -------------------------------------------------------------
                 # If IMT is PGV and PGV is not given by the GMPE, then
                 # convert from the appropriate PSA
                 # -------------------------------------------------------------
-                if (imt.string == "PGV") and ("PGV" not in gmpe_imts):
-                    lmean, lsd = ab2020.getPGVandSTDDEVS(
-                        lmean, lsd, stddev_types, ctx.rrup, ctx.vs30
+                if (PGV() in imt) and ("PGV" not in gmpe_imts):
+                    tmean, tsd = ab2020.getPGVandSTDDEVS(
+                        lmean[pgv_ix],
+                        lsd[pgv_ix * nsd : (pgv_ix + 1) * nsd],
+                        stddev_types,
+                        ctx.rrup,
+                        ctx.vs30,
                     )
+                    lmean[pgv_ix] = tmean
+                    for ix, _ in enumerate(stddev_types):
+                        lsd[pgv_ix * nsd + ix] = tsd[ix]
 
                 # -------------------------------------------------------------
                 # -------------------------------------------------------------
                 if self.HAS_SITE[i] is False:
-                    lamps = self.__get_site_factors__(
-                        sites, rup, dists, timt, default=True
-                    )
-                    lmean = lmean + lamps
+                    for kk, kimt in enumerate(timt):
+                        lamps = self.__get_site_factors__(
+                            sites, rup, dists, kimt, default=True
+                        )
+                        lmean[kk] = lmean[kk] + lamps
 
                 # -------------------------------------------------------------
                 # Convertions due to component definition
                 # -------------------------------------------------------------
                 imc_in = gmpe.DEFINED_FOR_INTENSITY_MEASURE_COMPONENT
                 imc_out = self.DEFINED_FOR_INTENSITY_MEASURE_COMPONENT
-                if imc_in != imc_out and imt.string != "MMI":
+                if imc_in != imc_out:
                     bk17 = BooreKishida2017(imc_in, imc_out)
-                    lmean = bk17.convertAmps(imt, lmean, dists.rrup, rup.mag)
-                    #
-                    # The extra sigma from the component conversion appears to
-                    # apply to the total sigma, so the question arises as to
-                    # how to apportion it between the intra- and inter-event
-                    # sigma. Here we assume it all enters as intra-event sigma.
-                    #
-                    for j, stddev_type in enumerate(stddev_types):
-                        if stddev_type == const.StdDev.INTER_EVENT:
+                    for kk, kimt in enumerate(timt):
+                        if kimt.string == "MMI":
                             continue
-                        lsd[j] = bk17.convertSigmas(imt, lsd[j])
+                        lmean[kk] = bk17.convertAmps(
+                            kimt, lmean[kk], dists.rrup, rup.mag
+                        )
+                        #
+                        # The extra sigma from the component conversion appears to
+                        # apply to the total sigma, so the question arises as to
+                        # how to apportion it between the intra- and inter-event
+                        # sigma. Here we assume it all enters as intra-event sigma.
+                        #
+                        for j, stddev_type in enumerate(stddev_types):
+                            if stddev_type == const.StdDev.INTER_EVENT:
+                                continue
+                            lsd[kk * nsd + j] = bk17.convertSigmas(
+                                kimt, lsd[kk * nsd + j]
+                            )
 
             # End: if GMPE is not MultiGMPE
 
             #
-            # At this point lsd will have 2 * len(stddev_types) entries, the
-            # first group will have the point-source to finite rupture
-            # inflation (if any), and the second set will not; in cases where
-            # a finite rupture is used, the two sets will be identical
+            # At this point lsd will have nimt * len(stddev_types) entries, the
             #
 
             # -----------------------------------------------------------------
             # Compute weighted mean and collect the elements to compute sd
             # -----------------------------------------------------------------
 
-            lnmu = lnmu + wts[i] * lmean
-            lnmu_list.append(lmean)
-            lnsd_list = lnsd_list + lsd
+            for kk, kimt in enumerate(timt):
+                lnmu[kk] = lnmu[kk] + wts[i] * lmean[kk]
+                lnmu_list[kk].append(lmean[kk])
+                lnsd_list[kk] = lnsd_list[kk] + lsd[kk * nsd : (kk + 1) * nsd]
 
         # -----------------------------------------------------------------
         # The mean is a weighted sum of random variables, so the stddev
         # is the weighted sum of of their covariances (effectively). See:
         # https://en.wikipedia.org/wiki/Variance#Weighted_sum_of_variables
         # for an explanation. Also see:
         # http://usgs.github.io/shakemap/manual4_0/tg_processing.html#ground-motion-prediction
         # for a discussion on the way this is implemented here.
         # -------------------------------------------------------------- # noqa
 
         nwts = len(wts)
         npwts = np.array(wts).reshape((1, -1))
-        nsites = len(lnmu)
-        # Find the correlation coefficients among the gmpes; if there are
-        # fewer than 10 points, just use an approximation (noting that the
-        # correlation among GMPEs tends to be quite high).
-        if nsites < 10:
-            cc = np.full((nwts, nwts), 0.95)
-            np.fill_diagonal(cc, 1.0)
-        else:
-            np.seterr(divide="ignore", invalid="ignore")
-            cc = np.reshape(np.corrcoef(lnmu_list), (nwts, nwts))
-            np.seterr(divide="warn", invalid="warn")
-            cc[np.isnan(cc)] = 1.0
-
-        # Multiply the correlation coefficients by the weights matrix
-        # (this is cheaper than multiplying all of elements of each
-        # stddev array by their weights since we have to multiply
-        # everything by the correlation coefficient matrix anyway))
-        cc = ((npwts * npwts.T) * cc).reshape((nwts, nwts, 1))
-        nstds = len(stddev_types)
         lnsd_new = []
-        for i in range(nstds * 2):
-            sdlist = []
-            for j in range(nwts):
-                sdlist.append(lnsd_list[j * nstds * 2 + i].reshape((1, 1, -1)))
-            sdstack = np.hstack(sdlist)
-            wcov = (sdstack * np.transpose(sdstack, axes=(1, 0, 2))) * cc
-            # This sums the weighted covariance as each point in the output
-            lnsd_new.append(np.sqrt(wcov.sum((0, 1))))
+        for kk, kimt in enumerate(timt):
+            nsites = len(lnmu[kk])
+            # Find the correlation coefficients among the gmpes; if there are
+            # fewer than 10 points, just use an approximation (noting that the
+            # correlation among GMPEs tends to be quite high).
+            if nsites < 10:
+                cc = np.full((nwts, nwts), 0.95)
+                np.fill_diagonal(cc, 1.0)
+            else:
+                np.seterr(divide="ignore", invalid="ignore")
+                cc = np.reshape(np.corrcoef(lnmu_list[kk]), (nwts, nwts))
+                np.seterr(divide="warn", invalid="warn")
+                cc[np.isnan(cc)] = 1.0
+
+            # Multiply the correlation coefficients by the weights matrix
+            # (this is cheaper than multiplying all of elements of each
+            # stddev array by their weights since we have to multiply
+            # everything by the correlation coefficient matrix anyway))
+            cc = ((npwts * npwts.T) * cc).reshape((nwts, nwts, 1))
+            for i in range(nsd):
+                sdlist = []
+                for j in range(nwts):
+                    sdlist.append(lnsd_list[kk][j * nsd + i].reshape((1, 1, -1)))
+                sdstack = np.hstack(sdlist)
+                wcov = (sdstack * np.transpose(sdstack, axes=(1, 0, 2))) * cc
+                # This sums the weighted covariance as each point in the output
+                lnsd_new.append(np.sqrt(wcov.sum((0, 1))))
 
-        return lnmu, lnsd_new
+        return (lnmu, lnsd_new)
 
     @classmethod
     def __from_config__(cls, conf, filter_imt=None):
         """
         Construct a MultiGMPE from a config file.
 
         Args:
@@ -912,97 +908,23 @@
         distance. For this level of detail, please see the config files.
 
         Returns:
             A dictionary representation of the MultiGMPE.
         """
         gmpe_dict = {"gmpes": [], "weights": [], "name": self.DESCRIPTION}
 
-        for i in range(len(self.GMPES)):
+        for i, this_gmpe in enumerate(self.GMPES):
             gmpe_dict["weights"].append(self.WEIGHTS[i])
-            if isinstance(self.GMPES[i], MultiGMPE):
-                gmpe_dict["gmpes"].append(self.GMPES[i].__describe__())
+            if isinstance(this_gmpe, MultiGMPE):
+                gmpe_dict["gmpes"].append(this_gmpe.__describe__())
             else:
-                gmpe_dict["gmpes"].append(str(self.GMPES[i]))
+                gmpe_dict["gmpes"].append(str(this_gmpe))
 
         return gmpe_dict
 
-    def __inflatePSSigma__(
-        self, gmpe, lmean, lsd, sites, rup, dists, imt, stddev_types
-    ):
-        """
-        If the point-source to finite-fault factors are used, we need to
-        inflate the intra-event and total standard deviations. We do this
-        by standard propagation of error techniques: taking the (numerical)
-        derivative of the GMPE (as a function of distance) squared times the
-        additional variance from the conversion, added
-        to the variance of the GMPE (then taking the square root). We do
-        this separately for each of Rrup and Rjb and sum the results.
-        If Rrup and Rjb are calculated from a finite rupture model, their
-        variance arrays will be "None" and lsd will remain unchanged.
-        Otherwise the error inflation will be applied. Normally one or the
-        other of Rrup/Rjb will not be used and so that term will be zero; in
-        some cases both may be used and both may result in non-zero
-        derivatives.
-
-        Args:
-            gmpe:
-                The GMPE to use for the calculations. Must be a base GMPE and
-                not a GMPE set, otherwise no action is taken.
-            lmean:
-                The mean values returned by the "normal" evaluation of the
-                GMPE.
-            lsd:
-                The standard deviations returned by the "normal" evaluation
-                of the GMPE.
-            sites:
-                The sites context required by the GMPE.
-            rup:
-                The rupture context required by the GMPE.
-            dists:
-                The distance context required by the GMPE.
-            imt:
-                The intensity measure type being evaluated.
-            stddev_types:
-                The list of stddev types found in lsd.
-
-        Returns:
-            list: A list of arrays of inflated standard deviations
-            corresponding to the elements of lsd.
-        """
-        new_sd = []
-        delta_distance = 0.01
-        delta_var = [0, 0]
-        for i, dtype in enumerate(("rrup", "rjb")):
-            # Skip dtype if the gmpe does not require it
-            if dtype not in gmpe.REQUIRES_DISTANCES:
-                continue
-            # Skip dtype if it has not been subject to a point-source to
-            # finite rupture conversion
-            dvar = getattr(dists, dtype + "_var", None)
-            if dvar is None:
-                continue
-            # Add a small amound to the rupture distance (rrup or rjb)
-            # and re-evaluate the GMPE
-            rup_dist = getattr(dists, dtype)
-            rup_dist += delta_distance
-            ctx = stuff_context(sites, rup, dists)
-            tmean, tsd = gmpe_gmas(gmpe, ctx, imt, stddev_types)
-            # Find the derivative w.r.t. the rupture distance
-            dm_dr = (lmean - tmean) / delta_distance
-            # The additional variance is (dm/dr)^2 * dvar
-            delta_var[i] = dm_dr ** 2 * dvar
-            # Put the rupture distance back to what it was
-            rup_dist -= delta_distance
-        for i, stdtype in enumerate(stddev_types):
-            if stdtype == const.StdDev.INTER_EVENT:
-                new_sd.append(lsd[i].copy())
-                continue
-            new_sd.append(np.sqrt(lsd[i] ** 2 + delta_var[0] + delta_var[1]))
-        return new_sd
-
 
 def filter_gmpe_list(gmpes, wts, imt):
     """
     Method to remove GMPEs from the GMPE list that are not applicable
     to a specific IMT. Rescales the weights to sum to one.
 
     Args:
@@ -1026,27 +948,27 @@
             w
             for g, w in zip(gmpes, wts)
             if PGA in g.DEFINED_FOR_INTENSITY_MEASURE_TYPES
         ]
     elif imt == PGV():
         sgmpe = []
         swts = []
-        for i in range(len(gmpes)):
-            if (PGV in gmpes[i].DEFINED_FOR_INTENSITY_MEASURE_TYPES) or (
+        for i, this_gmpe in enumerate(gmpes):
+            if (PGV in this_gmpe.DEFINED_FOR_INTENSITY_MEASURE_TYPES) or (
                 per_max[i] >= 1.0 and per_min[i] <= 1.0
             ):
-                sgmpe.append(gmpes[i])
+                sgmpe.append(this_gmpe)
                 swts.append(wts[i])
     else:
         per = imt.period
         sgmpe = []
         swts = []
-        for i in range(len(gmpes)):
+        for i, this_gmpe in enumerate(gmpes):
             if per_max[i] >= per and per_min[i] <= per:
-                sgmpe.append(gmpes[i])
+                sgmpe.append(this_gmpe)
                 swts.append(wts[i])
 
     if len(sgmpe) == 0:
         raise KeyError(f"No applicable GMPEs from GMPE list for {str(imt)}")
 
     # Scale weights to sum to one
     swts = np.array(swts)
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/plotting/contour.py` & `esi_shakelib-1.0.5/src/esi_shakelib/plotting/contour.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/plotting/plotrupture.py` & `esi_shakelib-1.0.5/src/esi_shakelib/plotting/plotrupture.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/sites.py` & `esi_shakelib-1.0.5/src/esi_shakelib/sites.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/station.py` & `esi_shakelib-1.0.5/src/esi_shakelib/station.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/utils/containers.py` & `esi_shakelib-1.0.5/src/esi_shakelib/utils/containers.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/utils/imt_string.py` & `esi_shakelib-1.0.5/src/esi_shakelib/utils/imt_string.py`

 * *Files identical despite different names*

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/utils/utils.py` & `esi_shakelib-1.0.5/src/esi_shakelib/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,32 +203,33 @@
     origin = rupture.getOrigin()
 
     min_mmi = config["extent"]["mmi"]["threshold"]
     sd_types = [const.StdDev.TOTAL]
 
     # Distance context
     dx = DistancesContext()
-    size = 2000
+    size = 200
     # This imposes minimum/ maximum distances of:
     #   80 and 800 km; could make this configurable
     d_min = config["extent"]["mmi"]["mindist"]
     d_max = config["extent"]["mmi"]["maxdist"]
     dx.rjb = np.logspace(np.log10(d_min), np.log10(d_max), size)
-    dx.rrup = np.sqrt(dx.rjb ** 2 + origin.depth ** 2)
+    dx.rrup = np.sqrt(dx.rjb**2 + origin.depth**2)
     dx.rhypo = dx.rrup
     dx.repi = dx.rjb
     dx.rx = np.zeros_like(dx.rjb)
     dx.ry0 = np.zeros_like(dx.rjb)
     dx.rvolc = np.zeros_like(dx.rjb)
 
     # Sites context
     sx = SitesContext()
     # Set to soft soil conditions
     sx.sids = np.array(range(size))
     sx.vs30 = np.full(size, 180.0)
+    sx.lons = np.full(size, 0.0)
     set_sites_depth_parameters(sx, ipe)
     sx.vs30measured = np.full(size, False, dtype=bool)
     sx.backarc = np.full(size, False, dtype=bool)
 
     # Rupture context
     rx = RuptureContext()
     rx.mag = origin.mag
@@ -243,15 +244,15 @@
     rx.ztor = rupture.getDepthToTop()
     rx.hypo_depth = origin.depth
 
     mmi = imt.from_string("MMI")
     imt_mean, _ = ipe.get_mean_and_stddevs(sx, rx, dx, mmi, sd_types)
 
     # Minimum distance that exceeds threshold MMI?
-    dists_exceed_mmi = dx.rjb[imt_mean > min_mmi]
+    dists_exceed_mmi = dx.rjb[imt_mean[0] > min_mmi]
     if len(dists_exceed_mmi):
         mindist_km = np.max(dists_exceed_mmi)
     else:
         mindist_km = d_min
 
     # Get a projection
     proj = OrthographicProjection(clon - 4, clon + 4, clat + 4, clat - 4)
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib/virtualipe.py` & `esi_shakelib-1.0.5/src/esi_shakelib/virtualipe.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import numpy as np
 
 from openquake.hazardlib.gsim.base import GMPE
 from openquake.hazardlib.imt import PGA, PGV, SA, MMI
 from openquake.hazardlib import const
 
 from esi_shakelib.utils.exception import ShakeLibException
+from esi_shakelib.ffsimmer import FFSimmer
+from esi_shakelib.generic_site_amplitication import GenericSiteAmplification
+from esi_utils_rupture.point_rupture import PointRupture
 
 
 class VirtualIPE(GMPE):
     """
     Implements a virtual IPE that is the combination of a MultiGMPE
     and a GMICE. Will first attempt to use PGV for the intensities,
     and then will try PGA, and then SA(1.0), and then will bail out.
@@ -45,30 +48,34 @@
     DEFINED_FOR_TECTONIC_REGION_TYPE = None
     #: Determined by the GMPE selected.
     REQUIRES_RUPTURE_PARAMETERS = None
     #: Determined by the GMPE selected.
     REQUIRES_SITES_PARAMETERS = None
 
     @classmethod
-    def __fromFuncs__(cls, gmpe, gmice):
+    def __fromFuncs__(cls, gmpe, gmice, rupture_obj=None, rff=None):
         """
         Creates a new VirtualIPE object with the specified MultiGMPE and
         GMICE. There is no default constructor, you must use this method.
 
         Args:
             gmpe: An instance of the MultiGMPE object.
             gmice: An instance of a GMICE object.
+            rupture_obj: A rupture object, if not None and a PointRupture, FFSimmer
+                will be used.
 
         Returns:
             :class:`VirtualIPE`: A new instance of a VirtualIPE object.
 
         """
         self = cls()
         self.gmpe = gmpe
         self.gmice = gmice
+        self.rupture_obj = rupture_obj
+        self.rff = rff
 
         if (
             gmpe.ALL_GMPES_HAVE_PGV is True
             and PGV in gmice.DEFINED_FOR_INTENSITY_MEASURE_TYPES
         ):
             self.imt = PGV()
         elif (
@@ -124,14 +131,16 @@
             prediction/conversion process. The prediction uncertainty will
             typically be either OpenQuake's TOTAL or INTRA_EVENT.  But can
             be any set that the MultiGMPE supports. See the ShakeMap manual
             for a detailed discussion of the way the uncertainty is computed.
 
         """  # noqa
 
+        if isinstance(imt, list):
+            imt = imt[0]
         if imt != MMI():
             raise ValueError("imt must be MMI")
         #
         # Get the mean ground motions and stddev for the preferred IMT
         #
         mgm, sdev = self.gmpe.get_mean_and_stddevs(sx, rx, dx, self.imt, stddev_types)
 
@@ -149,20 +158,18 @@
         mmi, dmda = self.gmice.getMIfromGM(mgm, self.imt, dist4gmice, rx.mag)
 
         #
         # Compute the uncertainty of the combined prediction/conversion
         # Total and intra-event uncertanty are inflated by the uncertainty
         # of the conversion; inter-event uncertainty is not.
         #
-        ntypes = len(stddev_types)
         nsd = len(sdev)
         mmi_sd = [None] * nsd
         gm2mi_var = (self.gmice.getGM2MIsd()[self.imt]) ** 2
         dmda *= dmda
         for i in range(nsd):
-            gm_var_in_mmi = dmda * sdev[i] ** 2
-            if stddev_types[i % ntypes] == const.StdDev.INTER_EVENT:
+            gm_var_in_mmi = dmda[0] * sdev[i] ** 2
+            if stddev_types[i] == const.StdDev.INTER_EVENT:
                 mmi_sd[i] = np.sqrt(gm_var_in_mmi)
             else:
                 mmi_sd[i] = np.sqrt(gm2mi_var + gm_var_in_mmi)
-
         return mmi, mmi_sd
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib.egg-info/PKG-INFO` & `esi_shakelib-1.0.5/src/esi_shakelib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esi-shakelib
-Version: 1.0.4
+Version: 1.0.5
 Summary: USGS Earthquake Impact Library for ShakeMap
 Author-email: Bruce Worden <cbworden@contractor.usgs.gov>, Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United
         States because it contains materials that originally came from the United
@@ -65,14 +65,15 @@
 Requires-Dist: numpy>=1.21
 Requires-Dist: openquake.engine==3.18.0
 Requires-Dist: alpha-shapes>=1.0.0
 Requires-Dist: pandas>=2.1.1
 Requires-Dist: scipy>=1.11.2
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: scikit-image>=0.21.0
+Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: usgs-strec>=2.2.8
 Provides-Extra: dev
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: black>=21; extra == "dev"
 Requires-Dist: flake8>=3.9; extra == "dev"
 Requires-Dist: ipython>=7.26; extra == "dev"
 Provides-Extra: test
@@ -83,11 +84,25 @@
 Requires-Dist: twine; extra == "build"
 Requires-Dist: check-wheel-contents; extra == "build"
 
 # esi-shakelib
 
 ## Introduction
 
-Utility package for general ShakeMap functions.
+This repository contains a utility package for general ShakeMap functions that may be of use to other programs.
+Included are:
+
+- IMC and IMT conversions
+- Cross correlation functions
+- Directivity functions
+- GMICE functions
+- Specialized NGA-East GMPEs for small magnitude earthquakes
+- Contour and rupture plotting functions
+- Misc. other functions
+
+See the code for documentation.
 
 ## Installation
 
+The package is available on PyPI. Install with pip:
+
+    pip install esi-shakelib
```

### Comparing `esi-shakelib-1.0.4/src/esi_shakelib.egg-info/SOURCES.txt` & `esi_shakelib-1.0.5/src/esi_shakelib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/esi_shakelib/__init__.py
+src/esi_shakelib/ffsimmer.py
+src/esi_shakelib/generic_site_amplitication.py
 src/esi_shakelib/multigmpe.py
 src/esi_shakelib/multiutils.py
 src/esi_shakelib/sites.py
 src/esi_shakelib/station.py
 src/esi_shakelib/virtualipe.py
 src/esi_shakelib.egg-info/PKG-INFO
 src/esi_shakelib.egg-info/SOURCES.txt
```

