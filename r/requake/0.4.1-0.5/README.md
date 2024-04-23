# Comparing `tmp/requake-0.4.1.tar.gz` & `tmp/requake-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requake-0.4.1.tar", last modified: Mon Mar 11 14:32:47 2024, max compression
+gzip compressed data, was "requake-0.5.tar", last modified: Tue Apr 23 07:53:32 2024, max compression
```

## Comparing `requake-0.4.1.tar` & `requake-0.5.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.055428 requake-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-03-11 14:32:41.000000 requake-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-11 14:32:41.000000 requake-0.4.1/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-11 14:32:41.000000 requake-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-11 14:32:41.000000 requake-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-11 14:32:47.055428 requake-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-03-11 14:32:41.000000 requake-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.055428 requake-0.4.1/requake/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-11 14:32:41.000000 requake-0.4.1/requake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-11 14:32:47.055428 requake-0.4.1/requake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.047428 requake-0.4.1/requake/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-11 14:32:41.000000 requake-0.4.1/requake/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-03-11 14:32:41.000000 requake-0.4.1/requake/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-11 14:32:41.000000 requake-0.4.1/requake/catalog/read_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-03-11 14:32:41.000000 requake-0.4.1/requake/catalog/read_catalog_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-03-11 14:32:41.000000 requake-0.4.1/requake/catalog/read_catalog_from_fdsnws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-11 14:32:41.000000 requake-0.4.1/requake/catalog/read_catalog_from_quakeml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.047428 requake-0.4.1/requake/config/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.051428 requake-0.4.1/requake/config/configobj/
--rw-r--r--   0 runner    (1001) docker     (127)    88030 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/configspec.conf
--rw-r--r--   0 runner    (1001) docker     (127)    10768 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/parse_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7743 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/rq_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-03-11 14:32:41.000000 requake-0.4.1/requake/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.051428 requake-0.4.1/requake/families/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-11 14:32:41.000000 requake-0.4.1/requake/families/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-03-11 14:32:41.000000 requake-0.4.1/requake/families/build_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-11 14:32:41.000000 requake-0.4.1/requake/families/build_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-03-11 14:32:41.000000 requake-0.4.1/requake/families/families.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-03-11 14:32:41.000000 requake-0.4.1/requake/families/flag_family.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-11 14:32:41.000000 requake-0.4.1/requake/families/print_families.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.051428 requake-0.4.1/requake/formulas/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-11 14:32:41.000000 requake-0.4.1/requake/formulas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-11 14:32:41.000000 requake-0.4.1/requake/formulas/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-03-11 14:32:41.000000 requake-0.4.1/requake/formulas/slip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.051428 requake-0.4.1/requake/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/cached_tiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/map_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/map_tiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/plot_families.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/plot_pair.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/plot_slip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-11 14:32:41.000000 requake-0.4.1/requake/plot/plot_timespans.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-11 14:32:41.000000 requake-0.4.1/requake/requake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.051428 requake-0.4.1/requake/scan/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-11 14:32:41.000000 requake-0.4.1/requake/scan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-03-11 14:32:41.000000 requake-0.4.1/requake/scan/scan_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-03-11 14:32:41.000000 requake-0.4.1/requake/scan/scan_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.055428 requake-0.4.1/requake/waveforms/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-11 14:32:41.000000 requake-0.4.1/requake/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-03-11 14:32:41.000000 requake-0.4.1/requake/waveforms/arrivals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-11 14:32:41.000000 requake-0.4.1/requake/waveforms/station_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-03-11 14:32:41.000000 requake-0.4.1/requake/waveforms/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:32:47.055428 requake-0.4.1/requake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-03-11 14:32:47.000000 requake-0.4.1/requake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-11 14:32:47.000000 requake-0.4.1/requake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 14:32:47.000000 requake-0.4.1/requake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-11 14:32:47.000000 requake-0.4.1/requake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 14:32:47.000000 requake-0.4.1/requake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-11 14:32:47.000000 requake-0.4.1/requake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-11 14:32:47.055428 requake-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-11 14:32:41.000000 requake-0.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-03-11 14:32:41.000000 requake-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-23 07:53:29.000000 requake-0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-23 07:53:29.000000 requake-0.5/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-23 07:53:29.000000 requake-0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 07:53:29.000000 requake-0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-23 07:53:32.114781 requake-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-23 07:53:29.000000 requake-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-23 07:53:29.000000 requake-0.5/requake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-23 07:53:32.114781 requake-0.5/requake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10387 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog_from_fdsnws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-23 07:53:29.000000 requake-0.5/requake/catalog/read_catalog_from_quakeml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-23 07:53:29.000000 requake-0.5/requake/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-23 07:53:29.000000 requake-0.5/requake/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/config/configobj/
+-rw-r--r--   0 runner    (1001) docker     (127)    88030 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-23 07:53:29.000000 requake-0.5/requake/config/configspec.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-23 07:53:29.000000 requake-0.5/requake/config/parse_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-23 07:53:29.000000 requake-0.5/requake/config/rq_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-23 07:53:29.000000 requake-0.5/requake/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.110781 requake-0.5/requake/families/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 07:53:29.000000 requake-0.5/requake/families/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-23 07:53:29.000000 requake-0.5/requake/families/build_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-23 07:53:29.000000 requake-0.5/requake/families/build_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-23 07:53:29.000000 requake-0.5/requake/families/families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-23 07:53:29.000000 requake-0.5/requake/families/flag_family.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-23 07:53:29.000000 requake-0.5/requake/families/print_families.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/formulas/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 07:53:29.000000 requake-0.5/requake/formulas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-23 07:53:29.000000 requake-0.5/requake/formulas/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-23 07:53:29.000000 requake-0.5/requake/formulas/slip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-23 07:53:29.000000 requake-0.5/requake/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/cached_tiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/map_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/map_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_families.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_slip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_timespans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-23 07:53:29.000000 requake-0.5/requake/plot/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/scan/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-23 07:53:29.000000 requake-0.5/requake/scan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-23 07:53:29.000000 requake-0.5/requake/scan/scan_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-23 07:53:29.000000 requake-0.5/requake/scan/scan_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/arrivals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/station_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-04-23 07:53:29.000000 requake-0.5/requake/waveforms/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:53:32.114781 requake-0.5/requake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7740 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 07:53:32.000000 requake-0.5/requake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-23 07:53:32.114781 requake-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-23 07:53:29.000000 requake-0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-04-23 07:53:29.000000 requake-0.5/versioneer.py
```

### Comparing `requake-0.4.1/CHANGELOG.md` & `requake-0.5/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,22 @@
-# Requake - Repeating earthquakes search and analysis
+# Requake Changelog
 
-(c) 2021-2024 Claudio Satriano <satriano@ipgp.fr>
+Copyright (c) 2021-2024 Claudio Satriano <satriano@ipgp.fr>
+
+## v0.5 - 2024-04-23
+
+- New config options: `station_metadata_path` and `waveform_data_path` to
+  read station metadata and waveform data from files. Supports any metadata
+  format supported by ObsPy and SDS (SeisComp Data Structure) waveform
+  archives.
+- Filter catalog files on reading using the criteria in the config file
+- Improved time axes in `plot_timespans` and `plot_slip` for short time
+  intervals
+- `print_families`: autoset duration units based on the average duration
+- `plot_timespans`: default sorting changed to `family_number`
 
 ## v0.4.1 - 2024-03-11
 
 - Bugfix: `requake` executable was not installed
 
 ## v0.4 - 2024-03-11
```

### Comparing `requake-0.4.1/LICENSE.txt` & `requake-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/PKG-INFO` & `requake-0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requake
-Version: 0.4.1
+Version: 0.5
 Summary: Repeating earthquakes search and analysis
 Home-page: https://requake.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://requake.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/requake
@@ -29,33 +29,37 @@
 License-File: LICENSE.txt
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: obspy>=1.2.0
 Requires-Dist: argcomplete
 Requires-Dist: tqdm
 Requires-Dist: tabulate
 
+<img src="imgs/Requake_logo.svg" width="400">
+
 # Requake
 
 Repeating earthquakes search and analysis.
 
 [![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
+[![docs-badge]][docs-link]
+[![DOI-badge]][DOI-link]
 
 Copyright (c) 2021-2024 Claudio Satriano <satriano@ipgp.fr>
 
 ## Description
 
 Requake is a command line tool to search and analyse repeating earthquakes.
 
 It can either scan an existing earthquake catalog to search for similar events,
 or perform template matching on a continuous waveform stream.
 
-Catalogs and waveforms are downloaded using standard
-[FDSN web services](https://www.fdsn.org/webservices/).
+Catalogs and waveforms can be read from local files or downloaded using
+standard [FDSN web services](https://www.fdsn.org/webservices/).
 
 Requake is written in Python and uses [ObsPy](https://obspy.org) as backend.
 
 ## Installation
 
 ### Installing the latest release
 
@@ -180,14 +184,39 @@
 process 14,100,705 earthquake pairs.
 Dowloaded traces are cached in memory to speed up execution. Processing is not
 yet parallel: some improvements might come in future versions, when
 parallelization will be implemented.
 
 - `requake build_families` is fast™.
 
+## How to Cite
+
+If you used Requake for a scientific paper, please cite it as:
+
+> Satriano, C. (2024). Requake: Repeating earthquakes search and analysis (X.Y).
+> [doi: 10.5281/ZENODO.10832204]
+
+Please replace `X.Y` with the Requake version number you used.
+
+You can also cite the following abstract presented at the
+2016 AGU Fall Meeting:
+
+> Satriano, C., Doucet, A. & Bouin, M.-P. (2021).
+> Probing the creep rate along the Lesser Antilles Subduction Zone through repeating earthquakes.
+> In AGU Fall Meeting Abstracts
+> (Vol. 2021, pp. T25A-0167), [bibcode: 2021AGUFM.T25A0167S]
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/requake.svg
 [PyPI-link]: https://pypi.python.org/pypi/requake
 [license-badge]: https://img.shields.io/badge/license-GPLv3-green
 [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
+[docs-badge]: https://readthedocs.org/projects/requake/badge/?version=latest
+[docs-link]: https://requake.readthedocs.io/en/latest/?badge=latest
 [changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
 [changelog-link]: https://github.com/SeismicSource/requake/blob/main/CHANGELOG.md
+[DOI-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.10832204.svg
+[DOI-link]: https://doi.org/10.5281/zenodo.10832204
+
+<!-- References -->
+[doi: 10.5281/ZENODO.10832204]: https://doi.org/10.5281/ZENODO.10832204
+[bibcode: 2021AGUFM.T25A0167S]: https://ui.adsabs.harvard.edu/abs/2021AGUFM.T25A0167S
```

### Comparing `requake-0.4.1/README.md` & `requake-0.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+<img src="imgs/Requake_logo.svg" width="400">
+
 # Requake
 
 Repeating earthquakes search and analysis.
 
 [![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
+[![docs-badge]][docs-link]
+[![DOI-badge]][DOI-link]
 
 Copyright (c) 2021-2024 Claudio Satriano <satriano@ipgp.fr>
 
 ## Description
 
 Requake is a command line tool to search and analyse repeating earthquakes.
 
 It can either scan an existing earthquake catalog to search for similar events,
 or perform template matching on a continuous waveform stream.
 
-Catalogs and waveforms are downloaded using standard
-[FDSN web services](https://www.fdsn.org/webservices/).
+Catalogs and waveforms can be read from local files or downloaded using
+standard [FDSN web services](https://www.fdsn.org/webservices/).
 
 Requake is written in Python and uses [ObsPy](https://obspy.org) as backend.
 
 ## Installation
 
 ### Installing the latest release
 
@@ -145,14 +149,39 @@
 process 14,100,705 earthquake pairs.
 Dowloaded traces are cached in memory to speed up execution. Processing is not
 yet parallel: some improvements might come in future versions, when
 parallelization will be implemented.
 
 - `requake build_families` is fast™.
 
+## How to Cite
+
+If you used Requake for a scientific paper, please cite it as:
+
+> Satriano, C. (2024). Requake: Repeating earthquakes search and analysis (X.Y).
+> [doi: 10.5281/ZENODO.10832204]
+
+Please replace `X.Y` with the Requake version number you used.
+
+You can also cite the following abstract presented at the
+2016 AGU Fall Meeting:
+
+> Satriano, C., Doucet, A. & Bouin, M.-P. (2021).
+> Probing the creep rate along the Lesser Antilles Subduction Zone through repeating earthquakes.
+> In AGU Fall Meeting Abstracts
+> (Vol. 2021, pp. T25A-0167), [bibcode: 2021AGUFM.T25A0167S]
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/requake.svg
 [PyPI-link]: https://pypi.python.org/pypi/requake
 [license-badge]: https://img.shields.io/badge/license-GPLv3-green
 [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
+[docs-badge]: https://readthedocs.org/projects/requake/badge/?version=latest
+[docs-link]: https://requake.readthedocs.io/en/latest/?badge=latest
 [changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
-[changelog-link]: https://github.com/SeismicSource/requake/blob/main/CHANGELOG.md
+[changelog-link]: https://github.com/SeismicSource/requake/blob/main/CHANGELOG.md
+[DOI-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.10832204.svg
+[DOI-link]: https://doi.org/10.5281/zenodo.10832204
+
+<!-- References -->
+[doi: 10.5281/ZENODO.10832204]: https://doi.org/10.5281/ZENODO.10832204
+[bibcode: 2021AGUFM.T25A0167S]: https://ui.adsabs.harvard.edu/abs/2021AGUFM.T25A0167S
```

### Comparing `requake-0.4.1/requake/catalog/catalog.py` & `requake-0.5/requake/catalog/catalog.py`

 * *Files 22% similar despite different names*

```diff
@@ -178,14 +178,80 @@
         :type filename: str
         """
         with open(filename, 'w', encoding='utf8') as fp:
             for ev in self:
                 fp.write(ev.fdsn_text() + '\n')
 
 
+    def filter(
+            self, starttime=None, endtime=None,
+            minlatitude=None, maxlatitude=None,
+            minlongitude=None, maxlongitude=None,
+            mindepth=None, maxdepth=None,
+            minmagnitude=None, maxmagnitude=None):
+        """
+        Filter the catalog, based on the specified criteria.
+
+        Returns a new catalog.
+
+        :param starttime: start time
+        :type starttime: obspy.UTCDateTime
+        :param endtime: end time
+        :type endtime: obspy.UTCDateTime
+        :param minlatitude: minimum latitude
+        :type minlatitude: float
+        :param maxlatitude: maximum latitude
+        :type maxlatitude: float
+        :param minlongitude: minimum longitude
+        :type minlongitude: float
+        :param maxlongitude: maximum longitude
+        :type maxlongitude: float
+        :param mindepth: minimum depth (in km)
+        :type mindepth: float
+        :param maxdepth: maximum depth (in km)
+        :type maxdepth: float
+        :param minmagnitude: minimum magnitude
+        :type minmagnitude: float
+        :param maxmagnitude: maximum magnitude
+        :type maxmagnitude: float
+
+        :return: a new catalog
+        :rtype: RequakeCatalog
+        """
+        outcat = RequakeCatalog()
+        for ev in self:
+            if ev.orig_time is not None:
+                if starttime is not None and ev.orig_time < starttime:
+                    continue
+                if endtime is not None and ev.orig_time > endtime:
+                    continue
+            if ev.lat is not None:
+                if minlatitude is not None and ev.lat < minlatitude:
+                    continue
+                if maxlatitude is not None and ev.lat > maxlatitude:
+                    continue
+            if ev.lon is not None:
+                if minlongitude is not None and ev.lon < minlongitude:
+                    continue
+                if maxlongitude is not None and ev.lon > maxlongitude:
+                    continue
+            if ev.depth is not None:
+                if mindepth is not None and ev.depth < mindepth:
+                    continue
+                if maxdepth is not None and ev.depth > maxdepth:
+                    continue
+            if ev.mag is not None:
+                if minmagnitude is not None and ev.mag < minmagnitude:
+                    continue
+                if maxmagnitude is not None and ev.mag > maxmagnitude:
+                    continue
+            outcat.append(ev)
+        return outcat
+
+
 def read_stored_catalog(config):
     """
     Read the catalog stored in the output directory.
 
     :param config: Configuration object.
     :type config: config.Config
```

### Comparing `requake-0.4.1/requake/catalog/read_catalog_from_csv.py` & `requake-0.5/requake/catalog/read_catalog_from_csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,15 +179,25 @@
                 hour = int_or_none(row[fields['hour']])
                 minute = int_or_none(row[fields['minute']])
                 seconds = float_or_none(row[fields['seconds']])
                 orig_time = UTCDateTime(
                     year=year, month=month, day=day,
                     hour=hour, minute=minute, second=0) + seconds
             else:
-                orig_time = UTCDateTime(row[fields['orig_time']])
+                try:
+                    orig_time = UTCDateTime(row[fields['orig_time']])
+                except ValueError:
+                    # one last try: check if the time is in the format
+                    # YYYYMMDD.hhmmss.
+                    # Replace the dot with a space, pad with zeros
+                    # and try again
+                    orig_time = UTCDateTime(
+                        row[fields['orig_time']]
+                        .replace('.', ' ').ljust(15, '0')
+                    )
             row[None] = None
             ev = RequakeEvent()
             ev.orig_time = orig_time
             ev.evid = row[fields['evid']]
             if ev.evid is None:
                 ev.evid = generate_evid(ev.orig_time)
             ev.lon = float_or_none(row[fields['lon']])
```

### Comparing `requake-0.4.1/requake/catalog/read_catalog_from_fdsnws.py` & `requake-0.5/requake/catalog/read_catalog_from_fdsnws.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/catalog/read_catalog_from_quakeml.py` & `requake-0.5/requake/catalog/read_catalog_from_quakeml.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/config/config.py` & `requake-0.5/requake/config/config.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/config/configobj/__init__.py` & `requake-0.5/requake/config/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/config/configobj/validate.py` & `requake-0.5/requake/config/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/config/configspec.conf` & `requake-0.5/requake/config/configspec.conf`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 #### Configuration file for Requake
 
 #### Station metadata and waveform data
 ## FDSN station webservice URL to retrieve station metadata.
 ## Use a full URL or a ObsPy shortcut (e.g., IRIS, RESIF, GEOFON, ...)
 fdsn_station_url = string(default=http://example.com)
+## Alternatively, you can provide the path to a local file with station
+## metadata in any format supported by ObsPy (note that some formats may not
+## contain station coordinates, which are required for the scan,
+## see https://docs.obspy.org/packages/obspy.core.inventory.html).
+## If both fdsn_station_url and stationxml_file are provided, the
+## local file will be used.
+station_metadata_path = string(default=None)
 ## FDSN dataselect webservice URL to retrieve waveforms.
 ## Use a full URL or a ObsPy shortcut (e.g., IRIS, RESIF, GEOFON, ...)
 fdsn_dataselect_url = string(default=http://example.com)
+## Alternatively, you can provide the path to a local SDS waveform archive
+## (see https://docs.obspy.org/packages/autogen/obspy.clients.filesystem.sds.html)
+waveform_data_path = string(default=None)
 
 #### Catalog-based scan
 ### The following parameters are for a catalog-based scan:
 ### each catalog event is compared with the other catalog events within
 ### a certain distance range. Similarity is checked by waveform
 ### cross-correlation at one or more stations.
 ### To perform a catalog-based scan use:
```

### Comparing `requake-0.4.1/requake/config/parse_arguments.py` & `requake-0.5/requake/config/parse_arguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,90 +128,87 @@
     #     a parent parser for the "longerthan" option,
     #     used by several subparsers
     longerthan = argparse.ArgumentParser(add_help=False)
     longerthan.add_argument(
         '-l', '--longerthan', type=str, default=0, metavar='DURATION',
         help='only use families lasting longer than this value. '
              'You can specify DURATION in days (e.g., 100d) '
-             'or in years (e.g., 2.5y).'
+             'or in years (e.g., 2.5y)'
     )
     # ---
     # --- minevents
     #     a parent parser for the "minevents" option,
     #     used by several subparsers
     minevents = argparse.ArgumentParser(add_help=False)
     minevents.add_argument(
         '-m', '--minevents', type=int, default=0, metavar='NEVENTS',
-        help='only use families with at least NEVENTS events.'
+        help='only use families with at least NEVENTS events'
     )
     # ---
     # --- familynumbers
     #     a parent parser for the "family_numbers" option,
     #     used by several subparsers
     familynumbers = argparse.ArgumentParser(add_help=False)
     familynumbers.add_argument(
         'family_numbers', default='all', nargs='?',
         help='family numbers to use. It can be a single number, '
              'a comma-separated list (ex.: 1,4,8), '
              'a hyphen-separated number range (ex.: 2-12), or "all" '
-             '(default: "all"). '
+             '(default: %(default)s)'
     )
     # ---
     # --- traceid
     #     a parent parser for the "traceid" option,
     #     used by several subparsers
     traceid = argparse.ArgumentParser(add_help=False)
     traceid.add_argument(
         '-t', '--traceid', type=str, default=None,
-        help='use this traceid instead of the default one for the family.'
+        help='use this traceid instead of the default one for the family'
     )
     # ---
     # --- print_families
     printfamilies = subparser.add_parser(
         'print_families',
         parents=[longerthan, minevents, familynumbers],
         help='print families to screen'
     )
     printfamilies.add_argument(
         '-f', '--format', type=str, default='simple',
-        help='format for the output table.'
-             'Choose between "simple", "markdown" and "csv"'
+        choices=['simple', 'markdown', 'csv'],
+        help='format for the output table (default: %(default)s)'
     )
     # ---
     # --- plot_families
     plotfamilies = subparser.add_parser(
         'plot_families',
         parents=[longerthan, minevents, familynumbers, traceid],
         help='plot traces for one ore more event families'
     )
     plotfamilies.add_argument(
         '-s', '--starttime', type=float, default=None,
-        help='start time, in seconds relative to trace start, for the plot.'
+        help='start time, in seconds relative to trace start, for the plot'
     )
     plotfamilies.add_argument(
         '-e', '--endtime', type=float, default=None,
-        help='end time, in seconds relative to trace start, for the plot.'
+        help='end time, in seconds relative to trace start, for the plot'
     )
     # ---
     # --- plot_timespans
     timespans = subparser.add_parser(
         'plot_timespans',
         parents=[longerthan, minevents, familynumbers],
         help='plot family timespans'
     )
     timespans.add_argument(
-        '-s', '--sortby', type=str, default=None,
+        '-s', '--sortby', type=str, default='family_number',
         choices=[
             'time', 'latitude', 'longitude', 'depth', 'distance_from',
             'family_number'
         ],
-        help='quantity to sort families by on y-axis. '
-             'Possible values are: time, latitude, longitude, depth, '
-             'distance_from, family_number. If not specified, the config '
-             'value "sort_families_by" will be used.'
+        help='quantity to sort families by on y-axis (default: %(default)s)'
     )
     # ---
     # --- plot_slip
     subparser.add_parser(
         'plot_slip',
         parents=[longerthan, minevents, familynumbers],
         help='plot cumulative slip for one or more families'
@@ -225,40 +222,38 @@
     )
     mapfamilies.add_argument(
         '-M', '--mapstyle', type=str, default='satellite',
         choices=[
             'stamen_terrain', 'satellite', 'street', 'hillshade',
             'hillshade_dark', 'ocean'
         ],
-        help='style of map to plot. Possible values are: '
-             'stamen_terrain, satellite, street, hillshade, hillshade_dark, '
-             'ocean'
+        help='style of map to plot (default: %(default)s)'
     )
     mapfamilies.add_argument(
         '-k', '--apikey', type=str, default=None,
-        help='API key for Stamen Terrain map tiles (default: None). '
+        help='API key for Stamen Terrain map tiles (default: %(default)s). '
              'You can get a free API key at https://stadiamaps.com/'
     )
     mapfamilies.add_argument(
         '-z', '--zoom', type=int, default=None,
         help='zoom level for the map tiles (default: None). Note that '
-             'certain map tiles might not be available at all zoom levels.'
+             'certain map tiles might not be available at all zoom levels'
     )
     # ---
     # --- flag_family
     flagfamily = subparser.add_parser(
         'flag_family',
         help='flag a family of repeating earthquakes as valid or not valid. '
              'Note that all families are valid by default when first created'
     )
     flagfamily.add_argument('family_number')
     flagfamily.add_argument(
         'is_valid',
         help='"true" (or "t") to flag family as valid, '
-             '"false" (or "f") to flag family as not valid.'
+             '"false" (or "f") to flag family as not valid'
     )
     # ---
     # --- build_templates
     subparser.add_parser(
         'build_templates',
         parents=[longerthan, minevents, familynumbers, traceid],
         help='build waveform templates for one or more event families'
```

### Comparing `requake-0.4.1/requake/config/rq_setup.py` & `requake-0.5/requake/config/rq_setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 import sys
 import os
 import shutil
 import logging
 import signal
 import tqdm
 from obspy import UTCDateTime
-from obspy.clients.fdsn import Client
+from obspy import read_inventory
+from obspy.clients.filesystem.sds import Client as SDSClient
+from obspy.clients.fdsn import Client as FDSNClient
+from obspy.clients.fdsn.header import FDSNNoServiceException
 from .._version import get_versions
 from .config import Config
 from .utils import (
     parse_configspec, read_config, validate_config, write_sample_config,
     write_ok
 )
 # pylint: disable=global-statement,import-outside-toplevel
@@ -100,22 +103,59 @@
     logger.debug(f'NumPy version: {NUMPY_VERSION_STR}')
     logger.debug(f'SciPy version: {SCIPY_VERSION_STR}')
     logger.debug(f'ObsPy version: {OBSPY_VERSION_STR}')
     logger.debug('Running arguments:')
     logger.debug(' '.join(sys.argv))
 
 
-def _connect_fdsn_station_dataselect(config):
-    """Connect to FDSN station and dataselect services."""
-    config.fdsn_station_client = Client(config.fdsn_station_url)
-    logger.info(f'Connected to FDSN station server: {config.fdsn_station_url}')
-    config.fdsn_dataselect_client = Client(config.fdsn_dataselect_url)
+def _connect_station_dataselect(config):
+    """
+    Connect to station and dataselect services.
+
+    Those can be either FDSN web services or local files.
+    """
+    if config.station_metadata_path is not None:
+        config.inventory = read_inventory(config.station_metadata_path)
+        config.station_client = None
+        logger.info(
+            'Reading station metadata from local file: '
+            f'{config.station_metadata_path}'
+        )
+    else:
+        config.station_client = FDSNClient(config.fdsn_station_url)
+        logger.info(
+            f'Connected to FDSN station server: {config.fdsn_station_url}'
+        )
+    if config.waveform_data_path is not None:
+        _connect_sds(config)
+    else:
+        config.dataselect_client = FDSNClient(config.fdsn_dataselect_url)
+        logger.info(
+            'Connected to FDSN dataselect server: '
+            f'{config.fdsn_dataselect_url}'
+        )
+
+
+def _connect_sds(config):
+    """
+    Connect to a local SeisComP Data Structure (SDS) archive.
+    """
+    _client = SDSClient(config.waveform_data_path)
+    all_nslc = _client.get_all_nslc()
+    if not all_nslc:
+        raise FileNotFoundError(
+            f'No SDS archive found in {config.waveform_data_path}'
+        )
+    config.dataselect_client = _client
     logger.info(
-        f'Connected to FDSN dataselect server: {config.fdsn_dataselect_url}'
+        'Reading waveform data from local SDS archive: '
+        f'{config.waveform_data_path}'
     )
+    all_nslc_str = '\n'.join('.'.join(nslc) for nslc in all_nslc)
+    logger.info(f'Found the following NSLC codes:\n{all_nslc_str}')
 
 
 def _parse_catalog_options(config):
     """Parse catalog options into lists."""
     config.catalog_start_times = []
     config.catalog_end_times = []
     config.catalog_fdsn_event_urls = [config.catalog_fdsn_event_url]
@@ -136,15 +176,15 @@
         config.catalog_end_times.append(UTCDateTime(end_time))
 
 
 def _connect_fdsn_catalog(config):
     """Connect to FDSN catalog services."""
     config.catalog_fdsn_event_clients = []
     for url in config.catalog_fdsn_event_urls:
-        config.catalog_fdsn_event_clients.append(Client(url))
+        config.catalog_fdsn_event_clients.append(FDSNClient(url))
         logger.info(f'Connected to FDSN event server: {url}')
 
 
 def configure(args):
     """Read command line arguments. Read config file. Set up logging."""
     configspec = parse_configspec()
     if args.action == 'sample_config':
@@ -201,18 +241,18 @@
     _parse_catalog_options(config)
     actions_needing_fdsn_station_dataselect = (
         'scan_catalog', 'plot_pair', 'plot_families', 'build_templates',
         'scan_templates'
     )
     try:
         if args.action in actions_needing_fdsn_station_dataselect:
-            _connect_fdsn_station_dataselect(config)
+            _connect_station_dataselect(config)
         if args.action == 'read_catalog' and not args.catalog_file:
             _connect_fdsn_catalog(config)
-    except Exception as m:
+    except (FileNotFoundError, ValueError, FDSNNoServiceException) as m:
         logger.error(m)
         rq_exit(1)
     # Template times must be UTCDateTime objects
     config.template_start_time = UTCDateTime(config.template_start_time)
     config.template_end_time = UTCDateTime(config.template_end_time)
     return config
```

### Comparing `requake-0.4.1/requake/config/utils.py` & `requake-0.5/requake/config/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 import os
 import sys
 import locale
+import traceback
+from .. import __version__
 from .configobj import ConfigObj
 from .configobj.validate import Validator
 locale.setlocale(locale.LC_ALL, '')
 
 
 def err_exit(msg):
     """
@@ -125,7 +127,45 @@
         for entry in test:
             if not test[entry]:
                 sys.stderr.write(
                     f'Invalid value for "{entry}": "{config_obj[entry]}"\n')
         sys.exit(1)
     if not test:
         err_exit('No configuration value present!')
+
+
+def manage_uncaught_exception(exception):
+    """
+    Manage an uncaught exception.
+
+    :param exception: Exception object.
+    :type exception: Exception
+    """
+    sys.stderr.write("""
+# BEGIN TRACEBACK #############################################################
+""")
+    sys.stderr.write('\n')
+    traceback.print_exc()
+    sys.stderr.write("""
+# END TRACEBACK ###############################################################
+""")
+    sys.stderr.write("""
+
+Congratulations, you've found a bug in Requake! 🐞
+
+Please report it on https://github.com/SeismicSource/requake/issues
+or by email to satriano@ipgp.fr.
+
+Include the following information in your report:
+
+""")
+    sys.stderr.write(f'  Requake version: {__version__}\n')
+    sys.stderr.write(f'  Python version: {sys.version}\n')
+    sys.stderr.write(f'  Platform: {sys.platform}\n')
+    sys.stderr.write(f'  Command line: {" ".join(sys.argv)}\n')
+    sys.stderr.write(f'  Error message: {str(exception)}\n')
+    sys.stderr.write('\n')
+    sys.stderr.write(
+        'Also, please copy and paste the traceback above in your '
+        'report.\n\n')
+    sys.stderr.write('Thank you for your help!\n\n')
+    sys.exit(1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `requake-0.4.1/requake/families/__init__.py` & `requake-0.5/requake/families/__init__.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/families/build_families.py` & `requake-0.5/requake/families/build_families.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/families/build_templates.py` & `requake-0.5/requake/families/build_templates.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/families/families.py` & `requake-0.5/requake/families/families.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         self.lat = None
         self.depth = None  # km
         self.starttime = None
         self.endtime = None
         self.duration = None  # years
         self.number = number
         self.valid = True
+        self.trace_id = None
 
     def __str__(self):
         return (
             f'{self.number:2d} {len(self):2d} '
             f'{self.lon:8.4f} {self.lat:8.4f} {self.depth:7.3f} '
             f'{self.starttime} {self.endtime} {self.duration:4.1f} '
             f'{self.valid}'
@@ -52,16 +53,22 @@
         Append an event to the family and update family attributes.
 
         If the event is already in the family, it is not appended.
 
         :param ev: Event to append.
         :type ev: RequakeEvent
         """
+        if not isinstance(ev, RequakeEvent):
+            raise TypeError('Event must be a RequakeEvent')
         if ev in self:
             return
+        if self.trace_id is None:
+            self.trace_id = ev.trace_id
+        elif ev.trace_id != self.trace_id:
+            raise ValueError('Event trace_id does not match family trace_id')
         super().append(ev)
         self.sort()
         self.lon = np.mean([e.lon for e in self])
         self.lat = np.mean([e.lat for e in self])
         self.depth = np.mean([e.depth for e in self])
         self.starttime = np.min([e.orig_time for e in self])
         self.endtime = np.max([e.orig_time for e in self])
```

### Comparing `requake-0.4.1/requake/families/flag_family.py` & `requake-0.5/requake/families/flag_family.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/families/print_families.py` & `requake-0.5/requake/families/print_families.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,23 +29,36 @@
     """
     try:
         families = read_selected_families(config)
     except (FileNotFoundError, FamilyNotFoundError) as msg:
         logger.error(msg)
         rq_exit(1)
 
+    # determine duration units
+    average_duration = np.mean([f.duration for f in families])
+    avg_duration_in_days = average_duration * 365
+    if 30 < avg_duration_in_days < 365:
+        duration_multiplier = 12
+        duration_units = 'm'
+    elif 1 < avg_duration_in_days < 30:
+        duration_multiplier = 365
+        duration_units = 'd'
+    elif avg_duration_in_days < 1:
+        duration_multiplier = 365 * 24
+        duration_units = 'h'
+
     headers = [
         'family',
         'nevents',
         'longitude',
         'latitude',
         'depth (km)',
         'start time',
         'end time',
-        'duration (y)',
+        f'duration ({duration_units})',
         'slip rate (cm/y)'
     ]
     table = []
     tablefmt = config.args.format
     if tablefmt == 'csv':
         writer = csv.writer(sys.stdout)
         writer.writerow(headers)
@@ -54,15 +67,15 @@
             family.number,
             len(family),
             family.lon,
             family.lat,
             family.depth,
             family.starttime,
             family.endtime,
-            family.duration
+            family.duration*duration_multiplier
         ]
         slip = [mag_to_slip_in_cm(config, ev.mag) for ev in family]
         cum_slip = np.cumsum(slip)
         d_slip = cum_slip[-1] - cum_slip[0]
         slip_rate = d_slip/family.duration
         row.append(slip_rate)
         table.append(row)
```

### Comparing `requake-0.4.1/requake/formulas/conversion.py` & `requake-0.5/requake/formulas/conversion.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/formulas/slip.py` & `requake-0.5/requake/formulas/slip.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/plot/__init__.py` & `requake-0.5/requake/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/plot/cached_tiler.py` & `requake-0.5/requake/plot/cached_tiler.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/plot/map_families.py` & `requake-0.5/requake/plot/map_families.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from matplotlib import colors
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
 from obspy.geodetics import gps2dist_azimuth
+from .plot_utils import plot_title, hover_annotation, duration_string
 from .cached_tiler import CachedTiler
 from .map_tiles import (
     EsriHillshade,
     EsriHillshadeDark,
     EsriOcean,
     EsriImagery,
     StamenTerrain,
@@ -91,14 +92,15 @@
     if map_style in {'hillshade', 'hillshade_dark', 'ocean', 'satellite'}:
         ax.attribution_text = 'Map powered by Esri and Natural Earth'
     elif map_style == 'stamen_terrain':
         ax.attribution_text = 'Map powered by Stamen Design and Natural Earth'
     else:
         ax.attribution_text = 'Map powered by Natural Earth'
     ax.gridlines(draw_labels=True, color='#777777', linestyle='--')
+    ax.hover_annotation_element = 'markers'
     return fig, ax
 
 
 def map_families(config):
     """
     Plot families on a map.
     """
@@ -107,58 +109,41 @@
     except (FileNotFoundError, FamilyNotFoundError) as m:
         logger.error(m)
         rq_exit(1)
     fig, ax = _make_basemap(config)
     trans = ccrs.PlateCarree()
     cmap = mpl.colormaps['tab10']
     norm = colors.Normalize(vmin=-0.5, vmax=9.5)
-    markers = []
+    trace_ids = []
     for family in families:
+        if family.trace_id not in trace_ids and family.trace_id is not None:
+            trace_ids.append(family.trace_id)
         fn = family.number
         nevents = len(family)
-        duration = (family.endtime - family.starttime)/(365*24*60*60)
+        duration_str = duration_string(family)
         label = (
-            f'Family {fn}\n{nevents} evts\n{duration:.1f} yrs\n'
+            f'Family {fn}\n{nevents} evts\n{duration_str}\n'
             f'Z {family.depth:.1f} km'
         )
         marker = ax.scatter(
             family.lon, family.lat,
             marker='o', s=100,
             color=cmap(norm(fn % 10)), edgecolor='k',
             transform=trans, label=label, zorder=10)
-        markers.append(marker)
+        marker.to_annotate = True
     sm = cm.ScalarMappable(cmap=cmap, norm=norm)
     cbar = fig.colorbar(sm, ticks=range(10), pad=0.1, ax=ax)
-    cbar.ax.set_ylabel('mod(family number, 10)')
+    cbar.ax.set_ylabel('family number (last digit)')
+    plot_title(
+        ax, len(families), trace_ids, vertical_position=1.05, fontsize=10)
 
     # Empty annotation that will be updated interactively
     annot = ax.annotate(
         '', xy=(0, 0), xytext=(5, 5),
         textcoords='offset points',
         bbox={'boxstyle': 'round', 'fc': 'w'},
         zorder=20
     )
     annot.set_visible(False)
-
-    def hover(event):
-        vis = annot.get_visible()
-        if event.inaxes == ax:
-            for marker in markers:
-                cont, _ind = marker.contains(event)
-                if cont:
-                    color = marker.get_facecolor()[0]
-                    marker.set_linewidth(3)
-                    annot.xy = (event.xdata, event.ydata)
-                    annot.set_text(marker.get_label())
-                    annot.get_bbox_patch().set_facecolor(color)
-                    annot.get_bbox_patch().set_alpha(0.8)
-                    annot.set_visible(True)
-                    fig.canvas.draw_idle()
-                    break
-                marker.set_linewidth(1)
-                if vis:
-                    annot.set_visible(False)
-                    fig.canvas.draw_idle()
-
-    fig.canvas.mpl_connect('motion_notify_event', hover)
-
+    annot.hover_annotation = True
+    fig.canvas.mpl_connect('motion_notify_event', hover_annotation)
     plt.show()
```

### Comparing `requake-0.4.1/requake/plot/map_tiles.py` & `requake-0.5/requake/plot/map_tiles.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/plot/plot_families.py` & `requake-0.5/requake/plot/plot_families.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/plot/plot_pair.py` & `requake-0.5/requake/plot/plot_pair.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/plot/plot_timespans.py` & `requake-0.5/requake/plot/plot_timespans.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,51 +8,82 @@
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 import logging
 import matplotlib as mpl
 import matplotlib.pyplot as plt
-import matplotlib.dates as mdates
 from matplotlib import cm
 from matplotlib import colors
 import numpy as np
+from .plot_utils import (
+    format_time_axis, plot_title, hover_annotation, duration_string)
 from ..families.families import FamilyNotFoundError, read_selected_families
 from ..config.rq_setup import rq_exit
 logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 # Reduce logging level for Matplotlib to avoid DEBUG messages
 mpl_logger = logging.getLogger('matplotlib')
 mpl_logger.setLevel(logging.WARNING)
 # Make text editable in Illustrator
 mpl.rcParams['pdf.fonttype'] = 42
 
 
+ylabels = {
+    'depth': 'Depth (km)',
+    'distance_from': 'Distance from',
+    'family_number': 'Family Number',
+    'latitude': 'Latitude (°N)',
+    'longitude': 'Longitude (°E)',
+    'time': 'Family Start Time',
+}
+
+
+def _plot_family_timespans(family, ax, sort_by, lon0, lat0, color):
+    """
+    Plot the timespan of a single family.
+    """
+    fn = family.number
+    nevents = len(family)
+    duration_str = duration_string(family)
+    label = (
+        f'Family {fn}\n{family.lon:.1f}°E {family.lat:.1f}°N '
+        f'{family.depth:.1f} km'
+        f'\n{nevents} evts {duration_str}'
+    )
+    times = [ev.orig_time.matplotlib_date for ev in family]
+    if sort_by == 'depth':
+        yvals = np.ones(len(times)) * family.depth
+    elif sort_by == 'distance_from':
+        yvals = np.ones(len(times)) * family.distance_from(lon0, lat0)
+    elif sort_by == 'family_number':
+        yvals = np.ones(len(times)) * fn
+    elif sort_by == 'latitude':
+        yvals = np.ones(len(times)) * family.lat
+    elif sort_by == 'longitude':
+        yvals = np.ones(len(times)) * family.lon
+    elif sort_by == 'time':
+        yvals = np.ones(len(times)) * family.starttime.matplotlib_date
+    ax.plot(times, yvals, lw=1, marker='o', color=color, label=label)
+
+
 def plot_timespans(config):
     """
     Plot family timespans.
     """
     try:
         families = read_selected_families(config)
     except (FileNotFoundError, FamilyNotFoundError) as m:
         logger.error(m)
         rq_exit(1)
     fig, ax = plt.subplots(figsize=(8, 8))
-    years = mdates.YearLocator()   # every year
-    months = mdates.MonthLocator()  # every month
-    yearsFmt = mdates.DateFormatter('%Y')
-    ax.xaxis.set_major_locator(years)
-    ax.xaxis.set_major_formatter(yearsFmt)
-    ax.xaxis.set_minor_locator(months)
-    ax.xaxis.grid(True)
     ax.tick_params(which='both', top=True, labeltop=True)
     ax.tick_params(axis='x', which='both', direction='in')
-
     cmap = mpl.colormaps['tab10']
     norm = colors.Normalize(vmin=-0.5, vmax=9.5)
-    lines = []
+
     if config.args.sortby is not None:
         sort_by = config.args.sortby
         valid_sort_by = (
             'time', 'latitude', 'longitude', 'depth', 'distance_from',
             'family_number'
         )
         if sort_by not in valid_sort_by:
@@ -65,81 +96,37 @@
     lon0, lat0 = config.distance_from_lon, config.distance_from_lat
     if sort_by == 'distance_from' and (lon0 is None or lat0 is None):
         logger.error(
             '"sort_families_by" set to "distance_from", '
             'but "distance_from_lon" and/or "distance_from_lat" '
             'are not specified')
         rq_exit(1)
-    if sort_by == 'time':
-        years = mdates.YearLocator()   # every year
-        months = mdates.MonthLocator()  # every month
-        yearsFmt = mdates.DateFormatter('%Y')
-        ax.yaxis.set_major_locator(years)
-        ax.yaxis.set_major_formatter(yearsFmt)
-        ax.yaxis.set_minor_locator(months)
+    trace_ids = []
     for family in families:
-        fn = family.number
-        label = (
-            f'Family {fn}\n{family.lon:.1f}°E {family.lat:.1f}°N '
-            f'{family.depth:.1f} km'
-        )
-        times = [ev.orig_time.matplotlib_date for ev in family]
-        if sort_by == 'time':
-            yvals = np.ones(len(times)) * family.starttime.matplotlib_date
-            ylabel = 'Family Start Time'
-        if sort_by == 'latitude':
-            yvals = np.ones(len(times)) * family.lat
-            ylabel = 'Latitude (°N)'
-        elif sort_by == 'longitude':
-            yvals = np.ones(len(times)) * family.lon
-            ylabel = 'Longitude (°E)'
-        elif sort_by == 'depth':
-            yvals = np.ones(len(times)) * family.depth
-            ylabel = 'Depth (km)'
-        elif sort_by == 'distance_from':
-            yvals = np.ones(len(times)) * family.distance_from(lon0, lat0)
-            ylabel = f'Distance from {lon0:.1f}°E, {lat0:.1f}°N (km)'
-        elif sort_by == 'family_number':
-            yvals = np.ones(len(times)) * fn
-            ylabel = 'Family Number'
-        line, = ax.plot(
-            times, yvals, lw=1, marker='o', color=cmap(norm(fn % 10)),
-            label=label)
-        lines.append(line)
+        if family.trace_id not in trace_ids and family.trace_id is not None:
+            trace_ids.append(family.trace_id)
+        color = cmap(norm(family.number % 10))
+        _plot_family_timespans(family, ax, sort_by, lon0, lat0, color)
+    format_time_axis(ax, which='xaxis')
+    if sort_by == 'time':
+        format_time_axis(ax, which='yaxis')
     ax.set_xlabel('Time')
-    ax.set_ylabel(ylabel)
+    ax.set_ylabel(ylabels[sort_by])
+    plot_title(
+        ax, len(families), trace_ids, vertical_position=1.05, fontsize=10)
+    ax.hover_annotation_element = 'lines'
     sm = cm.ScalarMappable(cmap=cmap, norm=norm)
     cbar = fig.colorbar(sm, ticks=range(10), ax=ax)
-    cbar.ax.set_ylabel('mod(family number, 10)')
+    cbar.ax.set_zorder(-1)
+    cbar.ax.set_ylabel('family number (last digit)')
 
     # Empty annotation that will be updated interactively
     annot = ax.annotate(
         '', xy=(0, 0), xytext=(5, 5),
         textcoords='offset points',
         bbox={'boxstyle': 'round', 'fc': 'w'},
         zorder=20
     )
     annot.set_visible(False)
-
-    def hover(event):
-        vis = annot.get_visible()
-        if event.inaxes == ax:
-            for line in lines:
-                cont, _ind = line.contains(event)
-                if cont:
-                    color = line.get_color()
-                    line.set_linewidth(3)
-                    annot.xy = (event.xdata, event.ydata)
-                    annot.set_text(line.get_label())
-                    annot.get_bbox_patch().set_facecolor(color)
-                    annot.get_bbox_patch().set_alpha(0.8)
-                    annot.set_visible(True)
-                    fig.canvas.draw_idle()
-                    break
-                line.set_linewidth(1)
-                if vis:
-                    annot.set_visible(False)
-                    fig.canvas.draw_idle()
-
-    fig.canvas.mpl_connect('motion_notify_event', hover)
-
+    annot.hover_annotation = True
+    fig.canvas.mpl_connect('motion_notify_event', hover_annotation)
     plt.show()
```

### Comparing `requake-0.4.1/requake/requake.py` & `requake-0.5/requake/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
 # Note: modules are lazily imported to speed up the startup time.
 # pylint: disable=relative-beyond-top-level,import-outside-toplevel
 
 
-def main():
-    """Main function for Requake."""
+def run():
+    """Run Requake."""
     from .config.parse_arguments import parse_arguments
     args = parse_arguments()
     from .config.rq_setup import configure, rq_exit
     config = configure(args)
     if config.args.action == 'read_catalog':
         from .catalog import read_catalog
         read_catalog(config)
@@ -53,7 +53,17 @@
     if config.args.action == 'flag_family':
         from .families import flag_family
         flag_family(config)
     if config.args.action == 'build_templates':
         from .families import build_templates
         build_templates(config)
     rq_exit(0)
+
+
+def main():
+    """Main entry point for Requake."""
+    try:
+        run()
+    # pylint: disable=broad-except
+    except Exception as e:
+        from .config.utils import manage_uncaught_exception
+        manage_uncaught_exception(e)
```

### Comparing `requake-0.4.1/requake/scan/scan_catalog.py` & `requake-0.5/requake/scan/scan_catalog.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import logging
 import csv
 from math import factorial
 from itertools import combinations
 from tqdm import tqdm
 from obspy.geodetics import gps2dist_azimuth
 from ..catalog.catalog import fix_non_locatable_events, read_stored_catalog
-from ..waveforms.station_metadata import NoMetadataError
+from ..waveforms.station_metadata import NoMetadataError, MetadataMismatchError
 from ..waveforms.waveforms import (
     get_waveform_pair, cc_waveform_pair, NoWaveformError,
 )
 from ..config.rq_setup import rq_exit
 logger = logging.getLogger(__name__.rsplit('.', maxsplit=1)[-1])
 
 
@@ -59,15 +59,15 @@
                     stats1.evid, stats2.evid, tr1.id,
                     stats1.orig_time, stats1.ev_lon, stats1.ev_lat,
                     stats1.ev_depth, stats1.mag_type, stats1.mag,
                     stats2.orig_time, stats2.ev_lon, stats2.ev_lat,
                     stats2.ev_depth, stats2.mag_type, stats2.mag,
                     lag, lag_sec, cc_max
                 ])
-            except NoMetadataError as m:
+            except (NoMetadataError, MetadataMismatchError) as m:
                 logger.error(m)
                 rq_exit(1)
             except NoWaveformError as m:
                 # Do not print empty messages
                 if str(m):
                     logger.warning(str(m))
     return npairs
@@ -81,15 +81,19 @@
     :type config: config.Config
     """
     try:
         catalog = read_stored_catalog(config)
     except (ValueError, FileNotFoundError) as m:
         logger.error(m)
         rq_exit(1)
-    fix_non_locatable_events(catalog, config)
+    try:
+        fix_non_locatable_events(catalog, config)
+    except MetadataMismatchError as m:
+        logger.error(m)
+        rq_exit(1)
     nevents = len(catalog)
     logger.info(f'{nevents} events read from catalog file')
     logger.info('Building event pairs...')
     logger.info('Computing waveform cross-correlation...')
     with open(config.scan_catalog_pairs_file, 'w', encoding='utf-8') as fp_out:
         npairs = _process_pairs(fp_out, nevents, catalog, config)
     logger.info(f'Processed {npairs:n} event pairs')
```

### Comparing `requake-0.4.1/requake/scan/scan_templates.py` & `requake-0.5/requake/scan/scan_templates.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/waveforms/arrivals.py` & `requake-0.5/requake/waveforms/arrivals.py`

 * *Files identical despite different names*

### Comparing `requake-0.4.1/requake/waveforms/station_metadata.py` & `requake-0.5/requake/waveforms/station_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     """Exception raised for missing metadata."""
 
 
 class MetadataMismatchError(Exception):
     """Exception raised for mismatched metadata."""
 
 
-def get_metadata(config):
+def download_metadata(config):
     """
     Download metadata for the trace_ids specified in config file.
 
     The metadata is stored in the config object.
 
     :param config: a Config object
     :type config: config.Config
     """
     logger.info('Downloading station metadata...')
     inv = Inventory()
-    cl = config.fdsn_station_client
+    cl = config.station_client
     start_time = min(config.catalog_start_times)
     end_time = max(config.catalog_end_times)
     if config.args.traceid is not None:
         trace_ids = [config.args.traceid, ]
     else:
         trace_ids = config.catalog_trace_id
     for trace_id in trace_ids:
@@ -78,15 +78,15 @@
     :type orig_time: obspy.UTCDateTime
     :return: a dictionary with trace_id as key and coordinates as value
     :rtype: dict
 
     :raises MetadataMismatchError: if coordinates are not found
     """
     if config.inventory is None:
-        get_metadata(config)
+        download_metadata(config)
     traceid_coords = {}
     for trace_id in config.catalog_trace_id:
         try:
             coords = config.inventory.get_coordinates(trace_id, orig_time)
         except Exception as m:
             # note: get_coordinaets raises a generic Exception
             raise MetadataMismatchError(
```

### Comparing `requake-0.4.1/requake/waveforms/waveforms.py` & `requake-0.5/requake/waveforms/waveforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,30 +60,35 @@
         distances[trace_id] = distance
     # return the trace_id for the closest trace
     return min(distances, key=distances.get)
 
 
 def get_waveform(config, traceid, starttime, endtime):
     """Download waveform for a given traceid, start and end time."""
-    cl = config.fdsn_dataselect_client
+    client = config.dataselect_client
     net, sta, loc, chan = traceid.split('.')
     try:
-        st = cl.get_waveforms(
+        st = client.get_waveforms(
             network=net, station=sta, location=loc, channel=chan,
             starttime=starttime, endtime=endtime
         )
     except FDSNNoDataException as m:
         msg = str(m).replace('\n', ' ')
         raise NoWaveformError(
             f'Unable to download waveform data for trace id: {traceid}.\n'
             f'Error message: {msg}'
         ) from m
     # webservices sometimes return longer traces: trim to be sure
     st.trim(starttime=starttime, endtime=endtime)
     st.merge(fill_value='interpolate')
+    if not st:
+        raise NoWaveformError(
+            f'No waveform data for trace id: {traceid} '
+            f'between {starttime} and {endtime}'
+        )
     tr = st[0]
     tr.detrend(type='demean')
     return tr
 
 
 def get_event_waveform(config, ev):
     """Download waveform for a given event at a given trace_id."""
```

### Comparing `requake-0.4.1/requake.egg-info/PKG-INFO` & `requake-0.5/requake.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requake
-Version: 0.4.1
+Version: 0.5
 Summary: Repeating earthquakes search and analysis
 Home-page: https://requake.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://requake.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/requake
@@ -29,33 +29,37 @@
 License-File: LICENSE.txt
 Requires-Dist: scipy>=1.5.0
 Requires-Dist: obspy>=1.2.0
 Requires-Dist: argcomplete
 Requires-Dist: tqdm
 Requires-Dist: tabulate
 
+<img src="imgs/Requake_logo.svg" width="400">
+
 # Requake
 
 Repeating earthquakes search and analysis.
 
 [![changelog-badge]][changelog-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
+[![docs-badge]][docs-link]
+[![DOI-badge]][DOI-link]
 
 Copyright (c) 2021-2024 Claudio Satriano <satriano@ipgp.fr>
 
 ## Description
 
 Requake is a command line tool to search and analyse repeating earthquakes.
 
 It can either scan an existing earthquake catalog to search for similar events,
 or perform template matching on a continuous waveform stream.
 
-Catalogs and waveforms are downloaded using standard
-[FDSN web services](https://www.fdsn.org/webservices/).
+Catalogs and waveforms can be read from local files or downloaded using
+standard [FDSN web services](https://www.fdsn.org/webservices/).
 
 Requake is written in Python and uses [ObsPy](https://obspy.org) as backend.
 
 ## Installation
 
 ### Installing the latest release
 
@@ -180,14 +184,39 @@
 process 14,100,705 earthquake pairs.
 Dowloaded traces are cached in memory to speed up execution. Processing is not
 yet parallel: some improvements might come in future versions, when
 parallelization will be implemented.
 
 - `requake build_families` is fast™.
 
+## How to Cite
+
+If you used Requake for a scientific paper, please cite it as:
+
+> Satriano, C. (2024). Requake: Repeating earthquakes search and analysis (X.Y).
+> [doi: 10.5281/ZENODO.10832204]
+
+Please replace `X.Y` with the Requake version number you used.
+
+You can also cite the following abstract presented at the
+2016 AGU Fall Meeting:
+
+> Satriano, C., Doucet, A. & Bouin, M.-P. (2021).
+> Probing the creep rate along the Lesser Antilles Subduction Zone through repeating earthquakes.
+> In AGU Fall Meeting Abstracts
+> (Vol. 2021, pp. T25A-0167), [bibcode: 2021AGUFM.T25A0167S]
+
 <!-- Badges and project links -->
 [PyPI-badge]: http://img.shields.io/pypi/v/requake.svg
 [PyPI-link]: https://pypi.python.org/pypi/requake
 [license-badge]: https://img.shields.io/badge/license-GPLv3-green
 [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
+[docs-badge]: https://readthedocs.org/projects/requake/badge/?version=latest
+[docs-link]: https://requake.readthedocs.io/en/latest/?badge=latest
 [changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
 [changelog-link]: https://github.com/SeismicSource/requake/blob/main/CHANGELOG.md
+[DOI-badge]: https://zenodo.org/badge/DOI/10.5281/zenodo.10832204.svg
+[DOI-link]: https://doi.org/10.5281/zenodo.10832204
+
+<!-- References -->
+[doi: 10.5281/ZENODO.10832204]: https://doi.org/10.5281/ZENODO.10832204
+[bibcode: 2021AGUFM.T25A0167S]: https://ui.adsabs.harvard.edu/abs/2021AGUFM.T25A0167S
```

### Comparing `requake-0.4.1/requake.egg-info/SOURCES.txt` & `requake-0.5/requake.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 versioneer.py
 requake/__init__.py
 requake/_version.py
-requake/requake.py
+requake/main.py
 requake.egg-info/PKG-INFO
 requake.egg-info/SOURCES.txt
 requake.egg-info/dependency_links.txt
 requake.egg-info/entry_points.txt
 requake.egg-info/requires.txt
 requake.egg-info/top_level.txt
 requake/catalog/__init__.py
@@ -43,14 +43,15 @@
 requake/plot/cached_tiler.py
 requake/plot/map_families.py
 requake/plot/map_tiles.py
 requake/plot/plot_families.py
 requake/plot/plot_pair.py
 requake/plot/plot_slip.py
 requake/plot/plot_timespans.py
+requake/plot/plot_utils.py
 requake/scan/__init__.py
 requake/scan/scan_catalog.py
 requake/scan/scan_templates.py
 requake/waveforms/__init__.py
 requake/waveforms/arrivals.py
 requake/waveforms/station_metadata.py
 requake/waveforms/waveforms.py
```

### Comparing `requake-0.4.1/setup.py` & `requake-0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 }
 
 setup(
     name='requake',
     packages=find_packages(),
     include_package_data=True,
     entry_points={
-        'console_scripts': ['requake = requake.requake:main']
+        'console_scripts': ['requake = requake.main:main']
         },
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     description='Repeating earthquakes search and analysis',
     long_description=long_descr,
     long_description_content_type='text/markdown',
     author='Claudio Satriano',
```

### Comparing `requake-0.4.1/versioneer.py` & `requake-0.5/versioneer.py`

 * *Files identical despite different names*

