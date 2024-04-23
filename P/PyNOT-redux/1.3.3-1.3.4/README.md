# Comparing `tmp/PyNOT-redux-1.3.3.tar.gz` & `tmp/PyNOT-redux-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyNOT-redux-1.3.3.tar", last modified: Wed May 10 07:23:45 2023, max compression
+gzip compressed data, was "PyNOT-redux-1.3.4.tar", last modified: Tue Apr 23 15:25:23 2024, max compression
```

## Comparing `PyNOT-redux-1.3.3.tar` & `PyNOT-redux-1.3.4.tar`

### file list

```diff
@@ -1,99 +1,100 @@
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.767178 PyNOT-redux-1.3.3/
--rw-r--r--   0 krogager   (501) staff       (20)     8196 2023-05-07 20:58:18.000000 PyNOT-redux-1.3.3/.DS_Store
--rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/.gitattributes
--rw-r--r--   0 krogager   (501) staff       (20)     1898 2023-05-09 07:51:28.000000 PyNOT-redux-1.3.3/.gitignore
--rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/LICENSE
--rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/MANIFEST.in
--rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-10 07:23:45.766965 PyNOT-redux-1.3.3/PKG-INFO
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.752210 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/
--rw-r--r--   0 krogager   (501) staff       (20)    13890 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/PKG-INFO
--rw-r--r--   0 krogager   (501) staff       (20)     2169 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/SOURCES.txt
--rw-r--r--   0 krogager   (501) staff       (20)        1 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/dependency_links.txt
--rw-r--r--   0 krogager   (501) staff       (20)       42 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/entry_points.txt
--rw-r--r--   0 krogager   (501) staff       (20)      113 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/requires.txt
--rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-10 07:23:45.000000 PyNOT-redux-1.3.3/PyNOT_redux.egg-info/top_level.txt
--rw-r--r--   0 krogager   (501) staff       (20)    13260 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/README.md
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.760118 PyNOT-redux-1.3.3/pynot/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/.extract_msg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/.identify_msg
--rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.3.3/pynot/.instrument.cfg
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/.response_msg
--rw-r--r--   0 krogager   (501) staff       (20)        6 2023-05-10 07:22:14.000000 PyNOT-redux-1.3.3/pynot/VERSION
--rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.3.3/pynot/alfosc.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.762767 PyNOT-redux-1.3.3/pynot/calib/
--rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/HeAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/HeNe_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ThAr_linelist.dat
--rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr18_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr19_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr4_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/al-gr7_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/alfosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     6013 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/default_options.yml
--rw-r--r--   0 krogager   (501) staff       (20)     3827 2023-05-10 07:21:25.000000 PyNOT-redux-1.3.3/pynot/calib/default_options_img.yml
--rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr13_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr14_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr1_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/ef-gr3_pixeltable.dat
--rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/efosc_filters.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/lapalma.ext
--rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/lasilla.ext
--rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/paranal.ext
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.765610 PyNOT-redux-1.3.3/pynot/calib/std/
--rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd174708.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd262606.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd332642.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/bd75325.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/eg21.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/feige110.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/feige34.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/gd153.dat
--rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/gd50.dat
--rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/gd71.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hd19445.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hd84937.dat
--rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hd93521.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/he3.dat
--rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/hiltner600.dat
--rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/ltt3864.dat
--rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/tcs_namelist.txt
--rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/calib/std/wolf1346.dat
--rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.3.3/pynot/calibs.py
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.766326 PyNOT-redux-1.3.3/pynot/data/
--rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/__init__.py
--rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/alfosc.rules
--rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/efosc.rules
-drwxr-xr-x   0 krogager   (501) staff       (20)        0 2023-05-10 07:23:45.766764 PyNOT-redux-1.3.3/pynot/data/help/
--rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_extract.html
--rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_identify.html
--rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_response.html
--rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/io.py
--rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/obs.py
--rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/data/organizer.py
--rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.3.3/pynot/efosc.py
--rw-r--r--   0 krogager   (501) staff       (20)   114866 2022-06-13 08:59:11.000000 PyNOT-redux-1.3.3/pynot/extract_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.3.3/pynot/extraction.py
--rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.3/pynot/fitsio.py
--rw-r--r--   0 krogager   (501) staff       (20)     8829 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/functions.py
--rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.3.3/pynot/identify_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.3.3/pynot/insconfig.py
--rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/logging.py
--rw-r--r--   0 krogager   (501) staff       (20)    47613 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.3/pynot/main.py
--rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.3.3/pynot/phot.py
--rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/phot_redux.py
--rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.3.3/pynot/redux.py
--rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/reports.py
--rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/response.py
--rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/response_gui.py
--rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.3.3/pynot/scired.py
--rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.3/pynot/scombine.py
--rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/tasks.py
--rw-r--r--   0 krogager   (501) staff       (20)     9913 2023-04-25 14:38:05.000000 PyNOT-redux-1.3.3/pynot/transients.py
--rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.3/pynot/txtio.py
--rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/wavecal.py
--rw-r--r--   0 krogager   (501) staff       (20)    13619 2023-05-10 07:20:54.000000 PyNOT-redux-1.3.3/pynot/wcs.py
--rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pynot/welcome.py
--rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.3/pyproject.toml
--rw-r--r--   0 krogager   (501) staff       (20)       38 2023-05-10 07:23:45.767213 PyNOT-redux-1.3.3/setup.cfg
--rw-r--r--   0 krogager   (501) staff       (20)     5210 2023-02-25 17:18:36.000000 PyNOT-redux-1.3.3/setup.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-23 15:25:23.273803 PyNOT-redux-1.3.4/
+-rw-r--r--   0 krogager   (501) staff       (20)     8196 2024-04-23 14:43:46.000000 PyNOT-redux-1.3.4/.DS_Store
+-rw-r--r--   0 krogager   (501) staff       (20)       66 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/.gitattributes
+-rw-r--r--   0 krogager   (501) staff       (20)     1909 2023-12-29 21:26:57.000000 PyNOT-redux-1.3.4/.gitignore
+-rw-r--r--   0 krogager   (501) staff       (20)     1079 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/LICENSE
+-rw-r--r--   0 krogager   (501) staff       (20)      202 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/MANIFEST.in
+-rw-r--r--   0 krogager   (501) staff       (20)    14696 2024-04-23 15:25:23.273629 PyNOT-redux-1.3.4/PKG-INFO
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-23 15:25:23.254979 PyNOT-redux-1.3.4/PyNOT_redux.egg-info/
+-rw-r--r--   0 krogager   (501) staff       (20)    14696 2024-04-23 15:25:23.000000 PyNOT-redux-1.3.4/PyNOT_redux.egg-info/PKG-INFO
+-rw-r--r--   0 krogager   (501) staff       (20)     2186 2024-04-23 15:25:23.000000 PyNOT-redux-1.3.4/PyNOT_redux.egg-info/SOURCES.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        1 2024-04-23 15:25:23.000000 PyNOT-redux-1.3.4/PyNOT_redux.egg-info/dependency_links.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       43 2024-04-23 15:25:23.000000 PyNOT-redux-1.3.4/PyNOT_redux.egg-info/entry_points.txt
+-rw-r--r--   0 krogager   (501) staff       (20)      113 2024-04-23 15:25:23.000000 PyNOT-redux-1.3.4/PyNOT_redux.egg-info/requires.txt
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2024-04-23 15:25:23.000000 PyNOT-redux-1.3.4/PyNOT_redux.egg-info/top_level.txt
+-rw-r--r--   0 krogager   (501) staff       (20)    14046 2024-04-23 15:16:28.000000 PyNOT-redux-1.3.4/README.md
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-23 15:25:23.265015 PyNOT-redux-1.3.4/pynot/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/.extract_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/.identify_msg
+-rw-r--r--   0 krogager   (501) staff       (20)       86 2023-02-25 17:32:13.000000 PyNOT-redux-1.3.4/pynot/.instrument.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/.response_msg
+-rw-r--r--   0 krogager   (501) staff       (20)        6 2024-04-23 15:15:51.000000 PyNOT-redux-1.3.4/pynot/VERSION
+-rw-r--r--   0 krogager   (501) staff       (20)     1110 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     6867 2022-06-01 17:21:45.000000 PyNOT-redux-1.3.4/pynot/alfosc.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-23 15:25:23.268198 PyNOT-redux-1.3.4/pynot/calib/
+-rw-r--r--   0 krogager   (501) staff       (20)      701 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/HeAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1073 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/HeNe_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      828 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/ThAr_linelist.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      340 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/al-gr18_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/al-gr19_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      318 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/al-gr4_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      186 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/al-gr7_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    19712 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/alfosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     6013 2023-12-29 19:17:16.000000 PyNOT-redux-1.3.4/pynot/calib/default_options.yml
+-rw-r--r--   0 krogager   (501) staff       (20)     3827 2023-12-29 19:17:24.000000 PyNOT-redux-1.3.4/pynot/calib/default_options_img.yml
+-rw-r--r--   0 krogager   (501) staff       (20)      343 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/ef-gr13_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      322 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/ef-gr14_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      300 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/ef-gr1_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      279 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/ef-gr3_pixeltable.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      709 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/efosc_filters.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1638 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/lapalma.ext
+-rw-r--r--   0 krogager   (501) staff       (20)      519 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/lasilla.ext
+-rw-r--r--   0 krogager   (501) staff       (20)     1425 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/paranal.ext
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-23 15:25:23.271561 PyNOT-redux-1.3.4/pynot/calib/std/
+-rw-r--r--   0 krogager   (501) staff       (20)     1454 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/bd174708.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1393 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/bd262606.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1254 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/bd332642.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1083 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/bd75325.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4228 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/eg21.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1251 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/feige110.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2738 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/feige34.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8611 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/gd153.dat
+-rw-r--r--   0 krogager   (501) staff       (20)   129806 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/gd50.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     8631 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/gd71.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1373 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/hd19445.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1376 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/hd84937.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     2609 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/hd93521.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1557 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/he3.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     1255 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/hiltner600.dat
+-rw-r--r--   0 krogager   (501) staff       (20)     4247 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/ltt3864.dat
+-rw-r--r--   0 krogager   (501) staff       (20)      368 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/tcs_namelist.txt
+-rw-r--r--   0 krogager   (501) staff       (20)     1807 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/calib/std/wolf1346.dat
+-rw-r--r--   0 krogager   (501) staff       (20)    26026 2022-04-22 11:31:36.000000 PyNOT-redux-1.3.4/pynot/calibs.py
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-23 15:25:23.272623 PyNOT-redux-1.3.4/pynot/data/
+-rw-r--r--   0 krogager   (501) staff       (20)        0 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/__init__.py
+-rw-r--r--   0 krogager   (501) staff       (20)     1744 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/alfosc.rules
+-rw-r--r--   0 krogager   (501) staff       (20)     1348 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/efosc.rules
+drwxr-xr-x   0 krogager   (501) staff       (20)        0 2024-04-23 15:25:23.273279 PyNOT-redux-1.3.4/pynot/data/help/
+-rw-r--r--   0 krogager   (501) staff       (20)     7423 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/help/welcome_msg_extract.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3876 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/help/welcome_msg_identify.html
+-rw-r--r--   0 krogager   (501) staff       (20)     1594 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/help/welcome_msg_response.html
+-rw-r--r--   0 krogager   (501) staff       (20)     3471 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/io.py
+-rw-r--r--   0 krogager   (501) staff       (20)     4699 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/obs.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26160 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/data/organizer.py
+-rw-r--r--   0 krogager   (501) staff       (20)     7812 2022-06-01 17:24:49.000000 PyNOT-redux-1.3.4/pynot/efosc.py
+-rw-r--r--   0 krogager   (501) staff       (20)   114921 2023-07-02 08:07:17.000000 PyNOT-redux-1.3.4/pynot/extract_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    23413 2022-05-05 20:36:46.000000 PyNOT-redux-1.3.4/pynot/extraction.py
+-rw-r--r--   0 krogager   (501) staff       (20)    19746 2023-04-25 06:53:15.000000 PyNOT-redux-1.3.4/pynot/fitsio.py
+-rw-r--r--   0 krogager   (501) staff       (20)     8905 2023-12-29 21:25:14.000000 PyNOT-redux-1.3.4/pynot/functions.py
+-rw-r--r--   0 krogager   (501) staff       (20)    50862 2022-06-01 17:19:24.000000 PyNOT-redux-1.3.4/pynot/identify_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    12773 2022-11-17 14:10:06.000000 PyNOT-redux-1.3.4/pynot/insconfig.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2614 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/logging.py
+-rw-r--r--   0 krogager   (501) staff       (20)    47395 2023-12-29 21:25:14.000000 PyNOT-redux-1.3.4/pynot/main.py
+-rw-r--r--   0 krogager   (501) staff       (20)    30199 2023-04-24 16:45:04.000000 PyNOT-redux-1.3.4/pynot/phot.py
+-rw-r--r--   0 krogager   (501) staff       (20)    14938 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/phot_redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28868 2022-04-20 11:44:59.000000 PyNOT-redux-1.3.4/pynot/redux.py
+-rw-r--r--   0 krogager   (501) staff       (20)     5048 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/reports.py
+-rw-r--r--   0 krogager   (501) staff       (20)    37586 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/response.py
+-rw-r--r--   0 krogager   (501) staff       (20)    26610 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/response_gui.py
+-rw-r--r--   0 krogager   (501) staff       (20)    20722 2022-05-03 16:23:47.000000 PyNOT-redux-1.3.4/pynot/scired.py
+-rw-r--r--   0 krogager   (501) staff       (20)    18099 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.4/pynot/scombine.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2337 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/tasks.py
+-rw-r--r--   0 krogager   (501) staff       (20)     9913 2023-04-25 14:38:05.000000 PyNOT-redux-1.3.4/pynot/transients.py
+-rw-r--r--   0 krogager   (501) staff       (20)     3391 2022-05-06 15:28:38.000000 PyNOT-redux-1.3.4/pynot/txtio.py
+-rw-r--r--   0 krogager   (501) staff       (20)    28434 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/wavecal.py
+-rw-r--r--   0 krogager   (501) staff       (20)    13619 2023-05-10 07:20:54.000000 PyNOT-redux-1.3.4/pynot/wcs.py
+-rw-r--r--   0 krogager   (501) staff       (20)     2384 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pynot/welcome.py
+-rw-r--r--   0 krogager   (501) staff       (20)      104 2022-03-27 13:12:39.000000 PyNOT-redux-1.3.4/pyproject.toml
+-rw-r--r--   0 krogager   (501) staff       (20)      112 2024-04-23 15:15:51.000000 PyNOT-redux-1.3.4/requirements.txt
+-rw-r--r--   0 krogager   (501) staff       (20)       38 2024-04-23 15:25:23.273849 PyNOT-redux-1.3.4/setup.cfg
+-rw-r--r--   0 krogager   (501) staff       (20)     5172 2024-04-23 15:15:51.000000 PyNOT-redux-1.3.4/setup.py
```

### Comparing `PyNOT-redux-1.3.3/.gitignore` & `PyNOT-redux-1.3.4/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -127,10 +127,11 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 test/implement_identify/identify_gui.py
 pynot/.instrument.cfg
+*.DS_Store
 .DS_Store
 .DS_Store
 .DS_Store
```

### Comparing `PyNOT-redux-1.3.3/LICENSE` & `PyNOT-redux-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/PKG-INFO` & `PyNOT-redux-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.3.3
+Version: 1.3.4
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
@@ -27,20 +28,37 @@
 ```diff
 - The pipeline is currently in a testing stage!
   Feel free to test it on your own data and let me know if you find any issues.
   I'll respond as fast as possible.
 ```
 
 ## Installation
+Before installing the pipeline, it is recommended to setup a virtual environment to avoid contaminating your local python environment. You can create a `pynot` environment using `python -m venv pynot` (or similar in `conda`). The activate the environment before installing and when running PyNOT: `source /path_to_venv/pynot/bin/activate`. Remember to `deactivate` the environment when you're done.
+
 The pipeline can be installed using [pip](https://www.pypi.org):
 
     ]% pip install PyNOT-redux
 
 and requires the following packages : `astroalign`, `astropy`, `astroquery`, `astroscrappy`, `lmfit`, `matplotlib`, `numpy`, `PyQt5`, `PyYAML`, `scipy`, `sep`, and `spectres`. I want to give a huge shout out to all the developers of these packages. Thanks for sharing your work!
 
+Alternatively, clone the repository and install it using:
+
+```
+git clone git@github.com:jkrogager/PyNOT.git
+cd PyNOT
+python -m venv venv-pynot
+source venv-pynot/bin/activate
+python -m pip -r requirements.txt
+
+```
+
+Then run the installer:
+`python -m pip install .` or `python setup.py install`.
+
+
 
 ## Basic Usage
 The pipeline is implemented as a series of modules or "tasks" that can either be executed individually or as a fully assembled pipeline. The available tasks can be shown by running:
 
     ]% pynot -h
 
 and the input parameters for each task can be inspected by running:
@@ -68,14 +86,15 @@
  - **`phot`** : runs the full spectroscopic pipeline using the parameter file generated by `pynot init phot`. The photometric pipeline performs bias and flat field correction, correction of cosmis ray hits, fringe correction, image registration and combination, source extraction and WCS calibration (using Gaia as reference). The final combined images are in units of counts per second (see more details below).
  If the observed frames are covered by the SDSS imaging foot print, PyNOT will perform an automatic self-calibration using SDSS photometry of sources in the field.
 
 
 
 ## Documentation
 
+You can see the documentation on the [PyNOT Website](https://jkrogager.github.io/pynot/).
 The full documentation is currently being compiled... stay tuned.
 
 
 
 ## Example: Spectroscopy
 A standard example would be the reduction of the data from one night of observations. All the raw data would be located in a single folder - let's call it `raw_data/`. This folder will contain the necessary raw data: bias frames, flux standard star spectra, arc line frames, spectroscopic flat fields, and the object spectra. Any other data in the folder (imaging files, sky flats, acquisition images, slit images etc.) will be ignored in the pipeline.
 
@@ -195,7 +214,9 @@
 where `class` refers to the classes defined above:
 
   0: not consistent with BAT nor XRT  (red)
 
   1: consistent with BAT  (orange)
 
   2: consistent with BAT and XRT  (green)
+
+
```

### Comparing `PyNOT-redux-1.3.3/PyNOT_redux.egg-info/PKG-INFO` & `PyNOT-redux-1.3.4/PyNOT_redux.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: PyNOT-redux
-Version: 1.3.3
+Version: 1.3.4
 Summary: Data Reduction Pipeline for NOT/ALFOSC
 Home-page: https://github.com/jkrogager/PyNOT
 Author: Jens-Kristian Krogager
 Author-email: krogager.jk@gmail.com
 License: MIT
 Keywords: spectroscopy astronomy longslit data processing pipeline
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >3.7
 Description-Content-Type: text/markdown
@@ -27,20 +28,37 @@
 ```diff
 - The pipeline is currently in a testing stage!
   Feel free to test it on your own data and let me know if you find any issues.
   I'll respond as fast as possible.
 ```
 
 ## Installation
+Before installing the pipeline, it is recommended to setup a virtual environment to avoid contaminating your local python environment. You can create a `pynot` environment using `python -m venv pynot` (or similar in `conda`). The activate the environment before installing and when running PyNOT: `source /path_to_venv/pynot/bin/activate`. Remember to `deactivate` the environment when you're done.
+
 The pipeline can be installed using [pip](https://www.pypi.org):
 
     ]% pip install PyNOT-redux
 
 and requires the following packages : `astroalign`, `astropy`, `astroquery`, `astroscrappy`, `lmfit`, `matplotlib`, `numpy`, `PyQt5`, `PyYAML`, `scipy`, `sep`, and `spectres`. I want to give a huge shout out to all the developers of these packages. Thanks for sharing your work!
 
+Alternatively, clone the repository and install it using:
+
+```
+git clone git@github.com:jkrogager/PyNOT.git
+cd PyNOT
+python -m venv venv-pynot
+source venv-pynot/bin/activate
+python -m pip -r requirements.txt
+
+```
+
+Then run the installer:
+`python -m pip install .` or `python setup.py install`.
+
+
 
 ## Basic Usage
 The pipeline is implemented as a series of modules or "tasks" that can either be executed individually or as a fully assembled pipeline. The available tasks can be shown by running:
 
     ]% pynot -h
 
 and the input parameters for each task can be inspected by running:
@@ -68,14 +86,15 @@
  - **`phot`** : runs the full spectroscopic pipeline using the parameter file generated by `pynot init phot`. The photometric pipeline performs bias and flat field correction, correction of cosmis ray hits, fringe correction, image registration and combination, source extraction and WCS calibration (using Gaia as reference). The final combined images are in units of counts per second (see more details below).
  If the observed frames are covered by the SDSS imaging foot print, PyNOT will perform an automatic self-calibration using SDSS photometry of sources in the field.
 
 
 
 ## Documentation
 
+You can see the documentation on the [PyNOT Website](https://jkrogager.github.io/pynot/).
 The full documentation is currently being compiled... stay tuned.
 
 
 
 ## Example: Spectroscopy
 A standard example would be the reduction of the data from one night of observations. All the raw data would be located in a single folder - let's call it `raw_data/`. This folder will contain the necessary raw data: bias frames, flux standard star spectra, arc line frames, spectroscopic flat fields, and the object spectra. Any other data in the folder (imaging files, sky flats, acquisition images, slit images etc.) will be ignored in the pipeline.
 
@@ -195,7 +214,9 @@
 where `class` refers to the classes defined above:
 
   0: not consistent with BAT nor XRT  (red)
 
   1: consistent with BAT  (orange)
 
   2: consistent with BAT and XRT  (green)
+
+
```

### Comparing `PyNOT-redux-1.3.3/PyNOT_redux.egg-info/SOURCES.txt` & `PyNOT-redux-1.3.4/PyNOT_redux.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .DS_Store
 .gitattributes
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 PyNOT_redux.egg-info/PKG-INFO
 PyNOT_redux.egg-info/SOURCES.txt
 PyNOT_redux.egg-info/dependency_links.txt
 PyNOT_redux.egg-info/entry_points.txt
 PyNOT_redux.egg-info/requires.txt
 PyNOT_redux.egg-info/top_level.txt
```

### Comparing `PyNOT-redux-1.3.3/README.md` & `PyNOT-redux-1.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,37 @@
 ```diff
 - The pipeline is currently in a testing stage!
   Feel free to test it on your own data and let me know if you find any issues.
   I'll respond as fast as possible.
 ```
 
 ## Installation
+Before installing the pipeline, it is recommended to setup a virtual environment to avoid contaminating your local python environment. You can create a `pynot` environment using `python -m venv pynot` (or similar in `conda`). The activate the environment before installing and when running PyNOT: `source /path_to_venv/pynot/bin/activate`. Remember to `deactivate` the environment when you're done.
+
 The pipeline can be installed using [pip](https://www.pypi.org):
 
     ]% pip install PyNOT-redux
 
 and requires the following packages : `astroalign`, `astropy`, `astroquery`, `astroscrappy`, `lmfit`, `matplotlib`, `numpy`, `PyQt5`, `PyYAML`, `scipy`, `sep`, and `spectres`. I want to give a huge shout out to all the developers of these packages. Thanks for sharing your work!
 
+Alternatively, clone the repository and install it using:
+
+```
+git clone git@github.com:jkrogager/PyNOT.git
+cd PyNOT
+python -m venv venv-pynot
+source venv-pynot/bin/activate
+python -m pip -r requirements.txt
+
+```
+
+Then run the installer:
+`python -m pip install .` or `python setup.py install`.
+
+
 
 ## Basic Usage
 The pipeline is implemented as a series of modules or "tasks" that can either be executed individually or as a fully assembled pipeline. The available tasks can be shown by running:
 
     ]% pynot -h
 
 and the input parameters for each task can be inspected by running:
@@ -50,14 +67,15 @@
  - **`phot`** : runs the full spectroscopic pipeline using the parameter file generated by `pynot init phot`. The photometric pipeline performs bias and flat field correction, correction of cosmis ray hits, fringe correction, image registration and combination, source extraction and WCS calibration (using Gaia as reference). The final combined images are in units of counts per second (see more details below).
  If the observed frames are covered by the SDSS imaging foot print, PyNOT will perform an automatic self-calibration using SDSS photometry of sources in the field.
 
 
 
 ## Documentation
 
+You can see the documentation on the [PyNOT Website](https://jkrogager.github.io/pynot/).
 The full documentation is currently being compiled... stay tuned.
 
 
 
 ## Example: Spectroscopy
 A standard example would be the reduction of the data from one night of observations. All the raw data would be located in a single folder - let's call it `raw_data/`. This folder will contain the necessary raw data: bias frames, flux standard star spectra, arc line frames, spectroscopic flat fields, and the object spectra. Any other data in the folder (imaging files, sky flats, acquisition images, slit images etc.) will be ignored in the pipeline.
```

### Comparing `PyNOT-redux-1.3.3/pynot/__init__.py` & `PyNOT-redux-1.3.4/pynot/__init__.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/alfosc.py` & `PyNOT-redux-1.3.4/pynot/alfosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/HeAr_linelist.dat` & `PyNOT-redux-1.3.4/pynot/calib/HeAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/HeNe_linelist.dat` & `PyNOT-redux-1.3.4/pynot/calib/HeNe_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/ThAr_linelist.dat` & `PyNOT-redux-1.3.4/pynot/calib/ThAr_linelist.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/alfosc_filters.dat` & `PyNOT-redux-1.3.4/pynot/calib/alfosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/default_options.yml` & `PyNOT-redux-1.3.4/pynot/calib/default_options.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/default_options_img.yml` & `PyNOT-redux-1.3.4/pynot/calib/default_options_img.yml`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/efosc_filters.dat` & `PyNOT-redux-1.3.4/pynot/calib/efosc_filters.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/lapalma.ext` & `PyNOT-redux-1.3.4/pynot/calib/lapalma.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/lasilla.ext` & `PyNOT-redux-1.3.4/pynot/calib/lasilla.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/paranal.ext` & `PyNOT-redux-1.3.4/pynot/calib/paranal.ext`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/bd174708.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/bd174708.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/bd262606.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/bd262606.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/bd332642.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/bd332642.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/bd75325.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/bd75325.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/eg21.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/eg21.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/feige110.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/feige110.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/feige34.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/feige34.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/gd153.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/gd153.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/gd50.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/gd50.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/gd71.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/gd71.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/hd19445.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/hd19445.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/hd84937.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/hd84937.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/hd93521.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/hd93521.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/he3.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/he3.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/hiltner600.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/hiltner600.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/ltt3864.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/ltt3864.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calib/std/wolf1346.dat` & `PyNOT-redux-1.3.4/pynot/calib/std/wolf1346.dat`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/calibs.py` & `PyNOT-redux-1.3.4/pynot/calibs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/alfosc.rules` & `PyNOT-redux-1.3.4/pynot/data/alfosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/efosc.rules` & `PyNOT-redux-1.3.4/pynot/data/efosc.rules`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_extract.html` & `PyNOT-redux-1.3.4/pynot/data/help/welcome_msg_extract.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_identify.html` & `PyNOT-redux-1.3.4/pynot/data/help/welcome_msg_identify.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/help/welcome_msg_response.html` & `PyNOT-redux-1.3.4/pynot/data/help/welcome_msg_response.html`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/io.py` & `PyNOT-redux-1.3.4/pynot/data/io.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/obs.py` & `PyNOT-redux-1.3.4/pynot/data/obs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/data/organizer.py` & `PyNOT-redux-1.3.4/pynot/data/organizer.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/efosc.py` & `PyNOT-redux-1.3.4/pynot/efosc.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/extract_gui.py` & `PyNOT-redux-1.3.4/pynot/extract_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1781,23 +1781,23 @@
             for model in self.trace_models:
                 parameters = model.get_parnames()
                 for ax, parname in zip(self.axes_points, parameters):
                     mask = model.get_mask(parname)
                     for line in model.point_lines[parname]:
                         line.remove()
                     l1, = ax.plot(model.x_binned[mask], model.points[parname][mask],
-                                  color=model.color, marker='o', ls='', mec=color_shade(model.color), picker=True, pickradius=6)
+                                  color=model.color, marker='o', ls='', mec=color_shade(model.color), picker=True, pickradius=10)
                     l2, = ax.plot(model.x_binned[~mask], model.points[parname][~mask],
-                                  color=model.color, marker='o', ls='', alpha=0.3, picker=True, pickradius=6)
+                                  color=model.color, marker='o', ls='', alpha=0.3, picker=True, pickradius=10)
                     l3, = ax.plot(model.x_binned[~mask], model.points[parname][~mask],
                                   color='k', marker='x', ls='')
                     model.point_lines[parname] = [l1, l2, l3]
                     if parname == 'mu':
                         l4, = self.axis_2d.plot(model.x_binned[mask], model.points[parname][mask],
-                                                color=model.color, marker='o', ls='', alpha=0.5, picker=True, pickradius=6)
+                                                color=model.color, marker='o', ls='', alpha=0.5, picker=True, pickradius=10)
                         model.point_lines[parname].append(l4)
 
                     if not model.active:
                         l1.set_visible(False)
                         l1.set_picker(False)
                         l2.set_visible(False)
                         l2.set_picker(False)
@@ -1830,37 +1830,37 @@
                 self.axes_points = self.figure_points.subplots(2, 1)
             else:
                 self.axes_points = [self.figure_points.subplots(1, 1)]
             self.axes_points[0].set_title("Profile Parameters along Dispersion Axis", fontsize=11)
 
             for model in self.trace_models:
                 parameters = model.get_parnames()
-                for ax, parname in zip(self.axes_points, parameters):
+                for axnum, (ax, parname) in enumerate(zip(self.axes_points, parameters), 1):
                     ax.tick_params(axis='both', which='major', labelsize=10)
                     mask = model.get_mask(parname)
                     # -- Plot traced points:
                     l1, = ax.plot(model.x_binned[mask], model.points[parname][mask],
-                                  color=model.color, marker='o', ls='', mec=color_shade(model.color), picker=True, pickradius=6)
+                                  color=model.color, marker='o', ls='', mec=color_shade(model.color), picker=True, pickradius=10)
                     l2, = ax.plot(model.x_binned[~mask], model.points[parname][~mask],
-                                  color=model.color, marker='o', ls='', alpha=0.3, picker=True, pickradius=6)
+                                  color=model.color, marker='o', ls='', alpha=0.3, picker=True, pickradius=10)
                     l3, = ax.plot(model.x_binned[~mask], model.points[parname][~mask],
                                   color='k', marker='x', ls='')
                     model.point_lines[parname] = [l1, l2, l3]
                     if parname == 'mu':
                         l4, = self.axis_2d.plot(model.x_binned[mask], model.points[parname][mask],
-                                                color=model.color, marker='o', ls='', alpha=0.3, picker=True, pickradius=6)
+                                                color=model.color, marker='o', ls='', alpha=0.3, picker=True, pickradius=10)
                         model.point_lines[parname].append(l4)
                     # -- Plot fit to points:
                     if len(model.fit['mu']) > 0:
                         lf, = ax.plot(model.x, model.fit[parname],
                                       color=model.color, ls='--', lw=1.0)
                         model.fit_lines[parname] = lf
                     if not model.fixed:
                         ax.set_ylabel("%s" % model.get_unicode_name(parname))
-                    if not ax.is_last_row():
+                    if not axnum == len(self.axes_points):
                         ax.set_xticklabels("")
         self.canvas_points.figure.tight_layout()
         self.update_xmask_in_points()
         self.canvas_points.draw()
         self.canvas_2d.draw()
 
     def create_model_trace(self, plot=False):
@@ -2040,21 +2040,21 @@
             spec1d = self.data1d[num]
             if model.plot_1d is not None:
                 for child in model.plot_1d.get_children():
                     child.remove()
                     # -- find a way to update the data instead...
             model.plot_1d = self.axis_1d.errorbar(spec1d.wl, spec1d.data, spec1d.error,
                                                   color=model.color, lw=1., elinewidth=0.5)
-            good_pixels = spec1d.data > 5*spec1d.error
+            good_pixels = spec1d.data > 5 * spec1d.error
             if np.sum(good_pixels) < 3:
                 data_min = 0.
-                data_max = 2*np.nanmean(spec1d.data[50:-50])
+                data_max = 2 * np.nanmean(spec1d.data[50:-50])
             else:
-                data_min = -3*np.nanmean(spec1d.error[good_pixels])
-                data_max = 1.2*np.nanmax(spec1d.data[good_pixels])
+                data_min = -3 * np.nanmedian(spec1d.error[good_pixels])
+                data_max = 2. * np.nanmedian(spec1d.data[good_pixels])
             ylims.append([data_min, data_max])
             listItem = self.list_widget.item(num)
             if listItem.checkState() == 2:
                 for child in model.plot_1d.get_children():
                     child.set_visible(True)
             else:
                 for child in model.plot_1d.get_children():
```

### Comparing `PyNOT-redux-1.3.3/pynot/extraction.py` & `PyNOT-redux-1.3.4/pynot/extraction.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/fitsio.py` & `PyNOT-redux-1.3.4/pynot/fitsio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/functions.py` & `PyNOT-redux-1.3.4/pynot/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,29 +33,31 @@
     all_comments = {}
     for num, line in enumerate(opt_lines):
         if line[0] == '#':
             continue
 
         try:
             key, val = line.split(':')[:2]
-        except:
+        except Exception:
             continue
 
         base_indent = get_indent(key)
         if base_indent == 0:
             # Section header:
             section = {}
             indent = get_indent(opt_lines[num+1])
             if indent == 0:
                 continue
             sub_lines = opt_lines[num+1:]
             i = 0
             while get_indent(sub_lines[i]) == indent:
                 sub_line = sub_lines[i]
-                par, value = sub_line.split(':')[:2]
+                items = sub_line.split(':')
+                par = items[0]
+                value = ':'.join(items[1:])
                 par = par.strip()
                 if '#' in value:
                     comment = value.split('#')[1]
                     comment = comment.strip()
                 else:
                     comment = ''
                 section[par] = comment
```

### Comparing `PyNOT-redux-1.3.3/pynot/identify_gui.py` & `PyNOT-redux-1.3.4/pynot/identify_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/insconfig.py` & `PyNOT-redux-1.3.4/pynot/insconfig.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/logging.py` & `PyNOT-redux-1.3.4/pynot/logging.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/main.py` & `PyNOT-redux-1.3.4/pynot/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
         parfile.write("".join(all_lines))
 
     print(" [OUTPUT] - Initiated new parameter file: %s\n" % pars_fname)
     print("\n You can now start the reduction pipeline by running:")
     print("   ]%% pynot %s  %s\n" % (mode, pars_fname))
 
 
-def main():
+def main(inspect=False):
 
     parser = ArgumentParser(prog='pynot')
     tasks = parser.add_subparsers(dest='task')
 
     p_break1 = tasks.add_parser('', help="")
 
     parser_init = tasks.add_parser('init', formatter_class=set_help_width(31),
@@ -319,23 +319,19 @@
     # -- crr :: Cosmic Ray Rejection and Correction
     parser_crr = tasks.add_parser('crr', formatter_class=set_help_width(31),
                                   help="Identification and correction of Cosmic Ray Hits")
     parser_crr.add_argument("input", type=str,
                             help="Input filename")
     parser_crr.add_argument("-o", "--output", type=str, required=True,
                             help="Output filename of cleaned image [REQUIRED]")
-    parser_crr.add_argument('-n', "--niter", type=int, default=4,
+    parser_crr.add_argument('-n', "--niter", type=int, default=2,
                             help="Number of iterations")
-    parser_crr.add_argument("--gain", type=float, default=0.16,
-                            help="Detector gain  (e-/ADU)")
-    parser_crr.add_argument("--readnoise", type=float, default=4.3,
-                            help="Detector read noise (e-)")
     # Define parameters based on default values:
     set_default_pars(parser_crr, section='crr', default_type=int,
-                     ignore_pars=['niter', 'gain', 'readnoise'])
+                     ignore_pars=['niter'])
 
 
     # -- flux1d :: Flux calibration of 1D spectrum
     parser_flux1 = tasks.add_parser('flux1d', formatter_class=set_help_width(31),
                                     help="Flux calibration of 1D spectrum")
     parser_flux1.add_argument("input", type=str,
                               help="Input filename of 1D spectrum")
@@ -547,21 +543,21 @@
                             help='Output filename of the ASCII table')
     parser_f2a.add_argument('--keys', type=str, nargs='+',
                             help='List of keywords from the FITS header to include (ESO keywords must use . not space delimiter)')
 
     parser_fapp = tasks.add_parser('append-ext', formatter_class=set_help_width(30),
                                    help="Append new data to FITS file or create error image")
     parser_fapp.add_argument('input', type=str,
-                            help='Input filename of FITS image to which the new data will be appended')
+                             help='Input filename of FITS image to which the new data will be appended')
     parser_fapp.add_argument('data', type=str,
-                            help='Filename of the image to append to the `input` FITS file')
+                             help='Filename of the image to append to the `input` FITS file')
     parser_fapp.add_argument('-n', '--name', type=str, default='',
-                            help='Name of the new FITS extension.')
+                             help='Name of the new FITS extension.')
     parser_fapp.add_argument('-x', '--ext', type=int, default=0,
-                            help='Extension number of the data file which is appended to the `input` file')
+                             help='Extension number of the data file which is appended to the `input` file')
 
     parser_delext = tasks.add_parser('remove-ext', formatter_class=set_help_width(30),
                                      help="Remove a given extension of a FITS file")
     parser_delext.add_argument('input', type=str,
                                help='Input filename of FITS image to which the new data will be appended')
     parser_delext.add_argument('ext', type=str,
                                help='Extension number or name to remove')
@@ -569,14 +565,17 @@
     parser_adderr = tasks.add_parser('add-error', formatter_class=set_help_width(30),
                                      help="Create and append error image for a single HDU FITS file")
     parser_adderr.add_argument('input', type=str,
                                help='Input filename of FITS image to which the new data will be appended')
     parser_adderr.add_argument('-f', '--force', action='store_true',
                                help='Overwrite existing error extension (if name is `ERR`)')
 
+    if inspect:
+        return parser
+
     args = parser.parse_args()
 
 
     # -- Define Workflow
     task = args.task
     log = ""
```

### Comparing `PyNOT-redux-1.3.3/pynot/phot.py` & `PyNOT-redux-1.3.4/pynot/phot.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/phot_redux.py` & `PyNOT-redux-1.3.4/pynot/phot_redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/redux.py` & `PyNOT-redux-1.3.4/pynot/redux.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/reports.py` & `PyNOT-redux-1.3.4/pynot/reports.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/response.py` & `PyNOT-redux-1.3.4/pynot/response.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/response_gui.py` & `PyNOT-redux-1.3.4/pynot/response_gui.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/scired.py` & `PyNOT-redux-1.3.4/pynot/scired.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/scombine.py` & `PyNOT-redux-1.3.4/pynot/scombine.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/tasks.py` & `PyNOT-redux-1.3.4/pynot/tasks.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/transients.py` & `PyNOT-redux-1.3.4/pynot/transients.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/txtio.py` & `PyNOT-redux-1.3.4/pynot/txtio.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/wavecal.py` & `PyNOT-redux-1.3.4/pynot/wavecal.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/wcs.py` & `PyNOT-redux-1.3.4/pynot/wcs.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/pynot/welcome.py` & `PyNOT-redux-1.3.4/pynot/welcome.py`

 * *Files identical despite different names*

### Comparing `PyNOT-redux-1.3.3/setup.py` & `PyNOT-redux-1.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 programming_language = 'Programming Language :: Python :: 3'
 
 std_filelist = glob.glob('pynot/calib/std/*.dat')
 std_filelist += ['tcs_namelist.txt']
 
 calib_files = glob.glob('')
 
+# Load Requirements
+fname = path.join(here, 'requirements.txt')
+with open(fname) as req_file:
+    reqs = req_file.readlines()
+requirements = [r.strip() for r in reqs]
+
 setup(
     name='PyNOT-redux',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
     version=version,
@@ -87,18 +93,15 @@
     # this:
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['matplotlib', 'numpy', 'scipy', 'PyQt5',
-                      'lmfit', 'astropy', 'astroscrappy', 'spectres',
-                      'PyYAML', 'sep', 'astroalign', 'astroquery',
-                      'beautifulsoup4'],
+    install_requires=requirements,
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
     extras_require={},
```

