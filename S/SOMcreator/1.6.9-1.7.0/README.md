# Comparing `tmp/SOMcreator-1.6.9.tar.gz` & `tmp/somcreator-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.6.9.tar", last modified: Fri Mar  1 07:43:59 2024, max compression
+gzip compressed data, was "somcreator-1.7.0.tar", last modified: Tue Apr 23 09:34:39 2024, max compression
```

## Comparing `SOMcreator-1.6.9.tar` & `somcreator-1.7.0.tar`

### file list

```diff
@@ -1,81 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.207556 SOMcreator-1.6.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.207556 SOMcreator-1.6.9/src/SOMcreator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/Template/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/Template/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/bookmark_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/fast_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/ifc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/mapping_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/Template/untested_template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39045 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/ifc_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/json_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/log_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/constants/value_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/external_software/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.211556 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/ids_xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/xml_xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/allplan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/card1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/attribute_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bill_of_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bookmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/building_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    19687 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/desite/modelcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)    21973 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/revit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/external_software/vestra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/filehandling/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5269 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/obj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/predefined_pset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/property_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/filehandling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.215556 SOMcreator-1.6.9/src/SOMcreator/ifc_modification/
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/ifc_modification/grouping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/src/SOMcreator/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-01 07:43:53.000000 SOMcreator-1.6.9/src/SOMcreator/tools/merge_projects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:43:59.219555 SOMcreator-1.6.9/src/SOMcreator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-01 07:43:59.000000 SOMcreator-1.6.9/src/SOMcreator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.784447 somcreator-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 09:34:34.000000 somcreator-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-23 09:34:34.000000 somcreator-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 09:34:39.784447 somcreator-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 09:34:34.000000 somcreator-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-23 09:34:34.000000 somcreator-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:34:39.784447 somcreator-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.768447 somcreator-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.772447 somcreator-1.7.0/src/SOMcreator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.772447 somcreator-1.7.0/src/SOMcreator/Template/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.776447 somcreator-1.7.0/src/SOMcreator/Template/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/bookmark_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/fast_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    24389 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/ifc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.776447 somcreator-1.7.0/src/SOMcreator/Template/js_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/mapping_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/Template/untested_template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39044 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.776447 somcreator-1.7.0/src/SOMcreator/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5979 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/constants/ifc_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/constants/json_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/constants/log_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/constants/value_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.776447 somcreator-1.7.0/src/SOMcreator/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/core/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/core/ifctosql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.776447 somcreator-1.7.0/src/SOMcreator/external_software/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.776447 somcreator-1.7.0/src/SOMcreator/external_software/IDS/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/IDS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/IDS/ids_xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/IDS/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/IDS/xml_xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.776447 somcreator-1.7.0/src/SOMcreator/external_software/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/__pyinstaller/hook-SOMcreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/allplan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.780447 somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/card1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.780447 somcreator-1.7.0/src/SOMcreator/external_software/desite/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/desite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/desite/attribute_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/desite/bill_of_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/desite/bookmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/desite/building_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20145 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/desite/modelcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/revit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/external_software/vestra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.780447 somcreator-1.7.0/src/SOMcreator/filehandling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/predefined_pset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/property_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/filehandling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.780447 somcreator-1.7.0/src/SOMcreator/ifc_modification/
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/ifc_modification/grouping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.784447 somcreator-1.7.0/src/SOMcreator/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/module/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/module/ifctosql.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/module/parsesql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.784447 somcreator-1.7.0/src/SOMcreator/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/tool/export_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/tool/ifctosql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/tool/parsesql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.784447 somcreator-1.7.0/src/SOMcreator/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-23 09:34:34.000000 somcreator-1.7.0/src/SOMcreator/tools/merge_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:34:39.784447 somcreator-1.7.0/src/SOMcreator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-23 09:34:39.000000 somcreator-1.7.0/src/SOMcreator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-23 09:34:39.000000 somcreator-1.7.0/src/SOMcreator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:34:39.000000 somcreator-1.7.0/src/SOMcreator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-23 09:34:39.000000 somcreator-1.7.0/src/SOMcreator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 09:34:39.000000 somcreator-1.7.0/src/SOMcreator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 09:34:39.000000 somcreator-1.7.0/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.6.9/LICENSE` & `somcreator-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/PKG-INFO` & `somcreator-1.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.6.9
+Version: 1.7.0
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.6.9/pyproject.toml` & `somcreator-1.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/Template/fast_template.txt` & `somcreator-1.7.0/src/SOMcreator/Template/fast_template.txt`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 }else{
     //-------------------------------------------------------------------------------------------
     //-----------------------------------Attributpruefung----------------------------------------
     //-------------------------------------------------------------------------------------------
     var pset_dict = get_property_set_dict(id);
     var checkfailed = 0;
     var attrib_count =0;
+    var object_not_checked = false;
+
 var ident_value = desiteAPI.getPropertyValue(id,"{{main_pset}}:{{main_attrib}}","xs:string");
 switch(ident_value){
 {% for obj in object_dict %}
 case "{{ obj.ident_value}}":
 {% set pset_dict = object_dict[obj] %}
 
       {%for pset in pset_dict%}
@@ -31,21 +33,15 @@
         {%endif-%}
         {%for attribute in attribute_list%}
 
         attributeName= '{{attribute.name}}';
         returnFormat= '{{xs_dict[attribute.data_type]}}';
         existingData = pset_dict[propertySetName][attributeName]
         {%if attribute.value_type == constants.LIST%}
-        var list = [
-        {%-for value in attribute.value%}
-        {%-if not loop.index==1%} ,'{{value}}'
-        {%-else-%}
-        '{{value}}'
-        {%-endif-%}
-        {%-endfor%}]
+        var list = {{attribute.value}};
         {%if attribute.value ==[]%}
         //Kontrolliert ob Attribut "{{attribute.property_set.name}}:{{attribute.name}}" existiert
         checkfailed +=check_exist(attributeName, propertySetName, returnFormat, existingData)
         {%else%}
         //Kontrolliert ob Attribut "{{attribute.property_set.name}}:{{attribute.name}}" einen dieser Werte entspricht: {{attribute.value}}
         checkfailed +=check_for_value(attributeName, propertySetName, returnFormat, list, existingData);
         {%endif-%}
@@ -69,16 +65,23 @@
     }
     else {checkfailed+= {{ pset.attributes.__len__() }};} //Wenn das PropertySet "{{pset.name}}" nicht existiert werden alle fehlenden Attribut Aufaddiert
 
         {% endfor %}
 
     break;
 {% endfor %}
+default:
+    object_not_checked = true;
 }
 
+    if (object_not_checked == true){
+        desiteResult.setCheckState('ignored');
+
+    }
+    else{
 
     //-------------------------------------------------------------------------------------------
     //--------------------------------------Auswertung-------------------------------------------
     //-------------------------------------------------------------------------------------------
     var check_status = "Undefined"
     if (checkfailed == 0) {
     desiteResult.setCheckState('passed'); check_status = "Passed"
@@ -96,8 +99,9 @@
     check_status = "Warning";
     }
 
     desiteAPI.setPropertyValue( id , "Check_State" , "xs:string", check_status);
     desiteAPI.setPropertyValue(id, "zu_pruefende_eigenschaften","xs:int",attrib_count);
     desiteAPI.setPropertyValue(id, "fehlerhafte_eigenschaften","xs:int",checkfailed);
 
+    }
 }
```

### Comparing `SOMcreator-1.6.9/src/SOMcreator/Template/ifc.json` & `somcreator-1.7.0/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_check_start.js` & `somcreator-1.7.0/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -25,16 +25,14 @@
     var text2 = '" nicht vorhanden! ';
     var text3 = '" liegt außerhalb des vorgegebenen Wertebereichs in MEM! ';
     var text4 = '" ( Wert ist : ';
     var text5 = "[Fehler ";
     var svalue = property_set_name + attribute_name;
 
 
-
-
     //Kontrolle, ob Attribut existiert
     if (check_exist(attribute_name, property_set_name, return_format, existing_data) === 1) {
         return 1
     }
     var value = existing_data["Value"];
     var unit = existing_data["Unit"];
     //Wenn das Format xs:string ist, wird das Attribut in eine Float Zahl umgewandelt
@@ -166,42 +164,46 @@
 
     var value = existing_data["Value"];
 
     //Kontrolliert ob das Element in Liste enthalten ist
     if (list.indexOf(value) !== -1) {
         return 0
     }
+    if (typeof(value) == "string") {
+        //Kontrolle, durch welchen Seperator die Liste getrennt ist -> Liste dementsprechend aufteilen
+        if (value.indexOf(",") !== -1) {
+            var val_list = value.split(",")
+        } else if (value.indexOf("/") != -1) {
+            var val_list = value.split("/")
+        }
+        //Wenn keine Trennzeichen vorhanden sind, besteht die Liste aus einem Element
+        else {
+            val_list = [value]
+        }
 
-    //Kontrolle, durch welchen Seperator die Liste getrennt ist -> Liste dementsprechend aufteilen
-    if (value.indexOf(",") !== -1) {
-        var val_list = value.split(",")
-    } else if (value.indexOf("/") != -1) {
-        var val_list = value.split("/")
-    }
-    //Wenn keine Trennzeichen vorhanden sind, besteht die Liste aus einem Element
-    else {
-        val_list = [value]
-    }
-
-    for (i in val_list) {
+        for (i in val_list) {
 
-        val_list[i] = val_list[i].trim(); //evtl. Leerzeichen am Anfang und Ende beseitigen
+            val_list[i] = val_list[i].trim(); //evtl. Leerzeichen am Anfang und Ende beseitigen
 
 
-        //Kontrolle, ob Das Element aus val_list in list enthalten ist (Case-insensitive)
-        if (list.indexOf(val_list[i]) === -1) {
-            desiteResult.addMessage(text1 + svalue + '" (' + value + ") " + text3 + text5 + "1]");
-            error += 1;
+            //Kontrolle, ob Das Element aus val_list in list enthalten ist (Case-insensitive)
+            if (list.indexOf(val_list[i]) === -1) {
+                desiteResult.addMessage(text1 + svalue + '" (' + value + ") " + text3 + text5 + "1]");
+                error += 1;
+            }
+        }
+        //Wenn alle Werte in liste enthalten sind, ist die Prüfung erfolgreich abgeschlossen
+        if (error === 0) {
+            return 0;
+        } else {
+            return 1;
         }
-    }
-    //Wenn alle Werte in liste enthalten sind, ist die Prüfung erfolgreich abgeschlossen
-    if (error === 0) {
-        return 0;
     } else {
-        return 1
+        desiteResult.addMessage(text1 + svalue + '" (' + value + ") " + text3 + text5 + "1]");
+        return 1;
     }
 }
 
 function get_property_set_dict(id) {
 
     var values = desiteAPI.getPropertyValuesByObject(id)
```

### Comparing `SOMcreator-1.6.9/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `somcreator-1.7.0/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/Template/mapping_template.txt` & `somcreator-1.7.0/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/Template/template.txt` & `somcreator-1.7.0/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/Template/untested_template.txt` & `somcreator-1.7.0/src/SOMcreator/Template/untested_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/classes.py` & `somcreator-1.7.0/src/SOMcreator/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,17 +284,18 @@
         use_case.name = new_name
 
     def remove_project_phase(self, project_phase_name: str) -> None:
         phase = self.get_project_phase_by_name(project_phase_name)
         if phase is None:
             return
         index = self.get_phase_index(phase)
-        self._project_phases.remove(phase)
         for item in self.get_all_hirarchy_items():
             item.remove_project_phase(phase)
+
+        self._project_phases.remove(phase)
         self._filter_matrix.pop(index)
 
     def remove_use_case(self, use_case_name: str) -> None:
         use_case = self.get_use_case_by_name(use_case_name)
         if use_case is None:
             return
         index = self.get_use_case_index(use_case)
@@ -955,42 +956,38 @@
     def name(self, value: str) -> None:
         # ToDo: add request for unlink
         self._name = value
         for child in self.children:
             child.name = value
 
     @property
+    def is_inheriting_values(self) -> bool:
+        if self.parent is None:
+            return False
+        if self.parent.is_inheriting_values or self.parent.child_inherits_values:
+            return True
+        return False
+
+    @property
     def value(self) -> list:
+        if self.is_inheriting_values:
+            values = [v for v in self._value if v not in self.parent.value]
+            return self.parent.value + values
         return self._value
 
     @value.setter
-    def value(self, value: list) -> None:
-        def can_be_changed() -> bool:
-            change_bool = True
-            if self.is_child:
-                parent: Attribute = self.parent
-                if parent.child_inherits_values:
-                    change_bool = False
-            return change_bool
-
-        new_value = []
-
-        for el in value:
-            if isinstance(el, str):
-                if "|" in el:
-                    el = el.split("|")
-                    for item in el:
-                        new_value.append(item)
-                else:
-                    new_value.append(el)
-            else:
-                new_value.append(el)
-
-        if can_be_changed():
-            self._value = new_value
+    def value(self, values: list) -> None:
+        if self.is_inheriting_values:
+            own_values = list()
+            for value in values:
+                if value not in self.parent.value:
+                    own_values.append(value)
+            self._value = own_values
+        else:
+            self._value = values
 
     @property
     def value_type(self) -> str:
         return self._value_type
 
     @value_type.setter
     def value_type(self, value: str):
```

### Comparing `SOMcreator-1.6.9/src/SOMcreator/constants/ifc_datatypes.py` & `somcreator-1.7.0/src/SOMcreator/constants/ifc_datatypes.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/constants/value_constants.py` & `somcreator-1.7.0/src/SOMcreator/constants/value_constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/ids_xsd.py` & `somcreator-1.7.0/src/SOMcreator/external_software/IDS/ids_xsd.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/main.py` & `somcreator-1.7.0/src/SOMcreator/external_software/IDS/main.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/IDS/xml_xsd.py` & `somcreator-1.7.0/src/SOMcreator/external_software/IDS/xml_xsd.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/allplan.py` & `somcreator-1.7.0/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/condition.py` & `somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/condition.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/constants.py` & `somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py` & `somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/bim_collab_zoom/rule.py` & `somcreator-1.7.0/src/SOMcreator/external_software/bim_collab_zoom/rule.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/card1.py` & `somcreator-1.7.0/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/__init__.py` & `somcreator-1.7.0/src/SOMcreator/external_software/desite/__init__.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/attribute_json.py` & `somcreator-1.7.0/src/SOMcreator/external_software/desite/attribute_json.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bill_of_quantities.py` & `somcreator-1.7.0/src/SOMcreator/external_software/desite/bill_of_quantities.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/bookmarks.py` & `somcreator-1.7.0/src/SOMcreator/external_software/desite/bookmarks.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/building_structure.py` & `somcreator-1.7.0/src/SOMcreator/external_software/desite/building_structure.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/desite/modelcheck.py` & `somcreator-1.7.0/src/SOMcreator/external_software/desite/modelcheck.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 import codecs
 import logging
 import os
 import uuid
 from xml.etree.ElementTree import Element
 
 import jinja2
-from anytree import AnyNode
 from lxml import etree
+from typing import TypedDict
 
 from . import handle_header, output_date_time
 from ...constants.value_constants import XS_DATATYPE_DICT
 from ..bim_collab_zoom.rule import merge_list
-from ... import __version__
 from ... import classes, constants, Template
 from ...constants import json_constants, value_constants
 
 JS_EXPORT = "JS"
 TABLE_EXPORT = "TABLE"
 
 
+class ObjectStructureDict(TypedDict):
+    children: set[classes.Object]
+
+
 def _handle_template(path: str | os.PathLike) -> jinja2.Template:
     file_loader = jinja2.FileSystemLoader(Template.HOME_DIR)
     env = jinja2.Environment(loader=file_loader)
     env.trim_blocks = True
     env.lstrip_blocks = True
     template = env.get_template(path)
     return template
@@ -139,74 +142,77 @@
 
 
 def _handle_attribute_rule_tree(xml_rule: Element) -> Element:
     attribute_rule_tree = etree.SubElement(xml_rule, "attributeRuleTree")
     return attribute_rule_tree
 
 
-def _handle_tree_structure(author: str, required_data_dict: dict, parent_xml_container, parent_node: AnyNode, template,
+def _handle_tree_structure(author: str, required_data_dict: dict, parent_xml_container,
+                           object_structure: dict[classes.Object, set[classes.Object]], parent_obj: classes.Object,
+                           template,
                            xml_object_dict, export_type: str) -> None:
-    def check_basics(node):
-        obj: classes.Object = node.obj
+    def check_basics(obj: classes.Object):
         if obj.ident_attrib is None:
             return obj, None, True
 
         pset_dict = required_data_dict.get(obj)
         if pset_dict is None:
             return obj, None, True
         return obj, pset_dict, False
 
-    def create_container(xml_container, node: AnyNode):
-        new_xml_container = _handle_container(xml_container, node.obj.name)
+    def create_container(xml_container):
+        new_xml_container = _handle_container(xml_container, parent_obj.name)
         if export_type == JS_EXPORT:
-            create_js_object(new_xml_container, parent_node)
+            create_js_object(new_xml_container)
         elif export_type == TABLE_EXPORT:
-            create_table_object(new_xml_container, parent_node)
-        for child_node in sorted(node.children, key=lambda x: x.id):
-            _handle_tree_structure(author, required_data_dict, new_xml_container, child_node, template, xml_object_dict,
+            create_table_object(new_xml_container)
+        children = object_structure.get(parent_obj)
+        for child_obj in sorted(children, key=lambda x: x.name):
+            _handle_tree_structure(author, required_data_dict, new_xml_container, object_structure, child_obj, template,
+                                   xml_object_dict,
                                    export_type)
 
-    def create_js_object(xml_container, node: AnyNode):
-        obj, pset_dict, abort = check_basics(node)
+    def create_js_object(xml_container):
+        obj, pset_dict, abort = check_basics(parent_obj)
         if abort:
             return
         xml_checkrun = _handle_checkrun(xml_container, obj.name, author)
         xml_rule = _handle_rule(xml_checkrun, "Attributes")
         xml_attribute_rule_list = _handle_attribute_rule_list(xml_rule)
         xml_rule_script = _handle_rule_script(xml_attribute_rule_list, name=obj.name)
         xml_code = _handle_code(xml_rule_script)
         cdata_code = template.render(pset_dict=pset_dict, constants=value_constants,
                                      ignore_pset=json_constants.IGNORE_PSET, xs_dict=XS_DATATYPE_DICT)
         xml_code.text = cdata_code
         _handle_rule(xml_checkrun, "UniquePattern")
 
         xml_object_dict[xml_checkrun] = obj
 
-    def create_table_object(xml_container, node: AnyNode):
-        obj, pset_dict, abort = check_basics(node)
+    def create_table_object(xml_container):
+        obj, pset_dict, abort = check_basics(parent_obj)
         if abort:
             return
         xml_checkrun = _handle_checkrun(xml_container, obj.name, author)
         xml_rule = _handle_rule(xml_checkrun, "Attributes")
         xml_attribute_rule_tree = _handle_attribute_rule_tree(xml_rule)
         xml_code = _handle_code(xml_container)
 
         _handle_rule_items_by_pset_dict(pset_dict, xml_attribute_rule_tree)
         xml_code.text = "<![CDATA[]]>"
         _handle_rule(xml_checkrun, "UniquePattern")
 
         xml_object_dict[xml_checkrun] = obj
 
-    if parent_node.children:
-        create_container(parent_xml_container, parent_node)
+    if object_structure.get(parent_obj) and required_data_dict.get(parent_obj):
+        create_container(parent_xml_container)
     else:
         if export_type == JS_EXPORT:
-            create_js_object(parent_xml_container, parent_node)
+            create_js_object(parent_xml_container)
         elif export_type == TABLE_EXPORT:
-            create_table_object(parent_xml_container, parent_node)
+            create_table_object(parent_xml_container)
 
 
 def _csv_value_in_list(attribute: classes.Attribute):
     return " ".join(f'"{str(val)}"' for val in attribute.value)
 
 
 def _csv_check_range(attribute: classes.Attribute) -> str:
@@ -268,22 +274,25 @@
 
 def _handle_rule_items_by_pset_dict(pset_dict: dict[classes.PropertySet, list[classes.Attribute]],
                                     attribute_rule_tree: etree.Element):
     for pset, attribute_list in pset_dict.items():
         _handle_rule_item_pset(attribute_rule_tree, pset, attribute_list)
 
 
-def _handle_object_rules(author: str, required_data_dict: dict, project_tree: AnyNode, base_xml_container: Element,
+def _handle_object_rules(author: str, required_data_dict: dict,
+                         object_structure: dict[classes.Object, set[classes.Object]],
+                         base_xml_container: Element,
                          template: jinja2.Template, export_type: str) -> dict[Element, classes.Object]:
     xml_object_dict: dict[Element, classes.Object] = dict()
 
-    root_nodes = project_tree.children
+    root_nodes = {obj for obj, value in object_structure.items() if not value}
 
-    for root_node in sorted(root_nodes, key=lambda x: x.id):
-        _handle_tree_structure(author, required_data_dict, base_xml_container, root_node, template, xml_object_dict,
+    for root_node in sorted(root_nodes, key=lambda x: x.name):
+        _handle_tree_structure(author, required_data_dict, base_xml_container, object_structure, root_node, template,
+                               xml_object_dict,
                                export_type)
     return xml_object_dict
 
 
 def _handle_data_section(xml_qa_export: Element, xml_checkrun_first: Element,
                          xml_checkrun_obj: dict[Element, classes.Object | None],
                          xml_checkrun_last: Element) -> None:
@@ -365,15 +374,14 @@
          " ".join([f'"{str(v)}"' for v in attribute.value]),
          f"Pruefung"])
 
 
 def _fast_object_check(main_pset: str, main_attrib: str, author: str, required_data_dict: dict,
                        base_xml_container: Element,
                        template: jinja2.Template) -> dict[Element, None]:
-    xml_object_dict: dict[Element, classes.Object] = dict()
     xml_checkrun = _handle_checkrun(base_xml_container, "Main Check", author)
     xml_rule = _handle_rule(xml_checkrun, "Attributes")
     xml_attribute_rule_list = _handle_attribute_rule_list(xml_rule)
     xml_rule_script = _handle_rule_script(xml_attribute_rule_list, name="Main Check")
     xml_code = _handle_code(xml_rule_script)
     cdata_code = template.render(object_dict=required_data_dict, main_pset=main_pset, main_attrib=main_attrib,
                                  constants=value_constants,
@@ -393,45 +401,39 @@
             for attribute in pset.attributes:
                 d[obj][pset].append(attribute)
     return d
 
 
 def export(project: classes.Project,
            required_data_dict: dict[classes.Object, dict[classes.PropertySet, list[classes.Attribute]]],
-           path: str, main_pset: str, main_attribute: str, project_tree: AnyNode = None,
+           path: str, main_pset: str, main_attribute: str,
+           object_structure: dict[classes.Object, set[classes.Object]] = None,
            export_type: str = "JS") -> None:
-    """
-
-    :param project:
-    :param required_data_dict:
-    :param path:
-    :param project_tree:
-    :param export_type: either JS or TABLE
-    :return:
-    """
+    if not object_structure:
+        object_structure = {o: o.children for o in project.objects}
 
-    if project_tree is None:
-        project_tree = project.tree()
     template = _handle_template(Template.TEMPLATE)
     xml_container, xml_qa_export = _init_xml(project.author, project.name, project.version)
     xml_checkrun_first, xml_attribute_rule_list = _define_xml_elements(project.author, xml_container, "initial_tests")
     _handle_js_rules(xml_attribute_rule_list, "start")
-    xml_checkrun_obj = _handle_object_rules(project.author, required_data_dict, project_tree, xml_container, template,
+    xml_checkrun_obj = _handle_object_rules(project.author, required_data_dict, object_structure, xml_container,
+                                            template,
                                             export_type)
     xml_checkrun_last, xml_attribute_rule_list = _define_xml_elements(project.author, xml_container, "untested")
     _handle_untested(xml_attribute_rule_list, main_pset, main_attribute)
     _handle_data_section(xml_qa_export, xml_checkrun_first, xml_checkrun_obj, xml_checkrun_last)
     _handle_property_section(xml_qa_export)
 
     tree = etree.ElementTree(xml_qa_export)
     with open(path, "wb") as f:
         tree.write(f, xml_declaration=True, pretty_print=True, encoding="utf-8", method="xml")
 
 
 def csv_export(required_data_dict: dict[classes.Object, dict[classes.PropertySet, list[classes.Attribute]]], path):
+    from ... import __version__
     lines = list()
     lines.append(";".join(["#", f"Created by SOMcreator v{__version__}"]))
     lines.append("H;Property Name;;Data Type;Rule;Comment")
 
     for obj, pset_dict in required_data_dict.items():
         if obj.ident_attrib is None:
             continue
@@ -451,14 +453,16 @@
 
 def fast_check(project: classes.Project, main_pset: str, main_attrib: str,
                required_data_dict: dict[classes.Object, dict[classes.PropertySet, list[classes.Attribute]]],
                path: str) -> None:
     """
     creates a single rule for all elements -> no containers for checkruns
     :param project:
+    :param main_pset: name of main propertyset which is used as matchkey
+    :param main_attrib: name of main Attribute wihich is used as matchkey
     :param required_data_dict: Dictionary of all required Objects, Propertysets and Attributes
     :param path: Export Path
     :return:
     """
     template = _handle_template(Template.FAST_TEMPLATE)
     xml_container, xml_qa_export = _init_xml(project.author, project.name, project.version)
     xml_checkrun_first, xml_attribute_rule_list = _define_xml_elements(project.author, xml_container, "initial_tests")
```

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/revit.py` & `somcreator-1.7.0/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/external_software/vestra.py` & `somcreator-1.7.0/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/__init__.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 plugin_dict = dict()
 
 
 def open_json(cls: Type[Project], path: str):
     SOMcreator.filehandling.parent_dict = dict()
 
     if not os.path.isfile(path):
-        return
+        raise FileNotFoundError(f"File '{path}' does not exist!")
 
     with open(path, "r") as file:
         main_dict: MainDict = json.load(file)
 
     SOMcreator.filehandling.plugin_dict = dict(main_dict)
 
     project_dict = main_dict.get(constants.PROJECT)
```

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/aggregation.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/aggregation.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/attribute.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/attribute.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/constants.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/core.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -78,14 +78,30 @@
                     output_use_cases[output_index] = value
 
         for phase_index, phase in enumerate(output_phases):
             pl = list()
             for use_case_index, use_case in enumerate(output_use_cases):
                 pl.append(bool(output_phases[phase_index] and output_use_cases[use_case_index]))
             matrix.append(pl)
+
+    phase_count = len(SOMcreator.filehandling.phase_list)
+    use_case_count = len(SOMcreator.filehandling.use_case_list)
+
+    if phase_count > len(matrix):
+        for _ in range(phase_count - len(matrix)):
+            matrix.append([True for _ in range(use_case_count)])
+    elif phase_count < len(matrix):
+        matrix = matrix[:phase_count]
+
+    for phase_index, use_case_list in enumerate(matrix):
+        if use_case_count > len(use_case_list):
+            [use_case_list.append(True) for _ in range(use_case_count - len(use_case_list))]
+        elif use_case_count < len(use_case_list):
+            use_case_list = use_case_list[:use_case_count]
+        matrix[phase_index] = use_case_list
     return name, description, optional, parent, matrix
 
 
 def check_dict(d: dict | None, d_name: str) -> bool:
     if d is None:
         logging.error(f"loading Error: {d_name} doesn't exist!")
         return True
```

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/inheritance.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/inheritance.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/obj.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/obj.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/predefined_pset.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/predefined_pset.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/project.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/project.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/property_set.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/property_set.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/filehandling/typing.py` & `somcreator-1.7.0/src/SOMcreator/filehandling/typing.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/ifc_modification/grouping.py` & `somcreator-1.7.0/src/SOMcreator/ifc_modification/grouping.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator/tools/merge_projects.py` & `somcreator-1.7.0/src/SOMcreator/tools/merge_projects.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.6.9/src/SOMcreator.egg-info/PKG-INFO` & `somcreator-1.7.0/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.6.9
+Version: 1.7.0
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.6.9/src/SOMcreator.egg-info/SOURCES.txt` & `somcreator-1.7.0/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -22,24 +22,28 @@
 src/SOMcreator/Template/js_templates/start_check_start.js
 src/SOMcreator/Template/js_templates/start_koordinaten.js
 src/SOMcreator/constants/__init__.py
 src/SOMcreator/constants/ifc_datatypes.py
 src/SOMcreator/constants/json_constants.py
 src/SOMcreator/constants/log_constants.py
 src/SOMcreator/constants/value_constants.py
+src/SOMcreator/core/__init__.py
+src/SOMcreator/core/export_excel.py
+src/SOMcreator/core/ifctosql.py
 src/SOMcreator/external_software/__init__.py
 src/SOMcreator/external_software/allplan.py
 src/SOMcreator/external_software/card1.py
-src/SOMcreator/external_software/excel.py
 src/SOMcreator/external_software/revit.py
 src/SOMcreator/external_software/vestra.py
 src/SOMcreator/external_software/IDS/__init__.py
 src/SOMcreator/external_software/IDS/ids_xsd.py
 src/SOMcreator/external_software/IDS/main.py
 src/SOMcreator/external_software/IDS/xml_xsd.py
+src/SOMcreator/external_software/__pyinstaller/__init__.py
+src/SOMcreator/external_software/__pyinstaller/hook-SOMcreator.py
 src/SOMcreator/external_software/bim_collab_zoom/__init__.py
 src/SOMcreator/external_software/bim_collab_zoom/action.py
 src/SOMcreator/external_software/bim_collab_zoom/condition.py
 src/SOMcreator/external_software/bim_collab_zoom/constants.py
 src/SOMcreator/external_software/bim_collab_zoom/modelcheck.py
 src/SOMcreator/external_software/bim_collab_zoom/rule.py
 src/SOMcreator/external_software/desite/__init__.py
@@ -56,9 +60,17 @@
 src/SOMcreator/filehandling/inheritance.py
 src/SOMcreator/filehandling/obj.py
 src/SOMcreator/filehandling/predefined_pset.py
 src/SOMcreator/filehandling/project.py
 src/SOMcreator/filehandling/property_set.py
 src/SOMcreator/filehandling/typing.py
 src/SOMcreator/ifc_modification/grouping.py
+src/SOMcreator/module/__init__.py
+src/SOMcreator/module/export_excel.py
+src/SOMcreator/module/ifctosql.py
+src/SOMcreator/module/parsesql.py
+src/SOMcreator/tool/__init__.py
+src/SOMcreator/tool/export_excel.py
+src/SOMcreator/tool/ifctosql.py
+src/SOMcreator/tool/parsesql.py
 src/SOMcreator/tools/__init__.py
 src/SOMcreator/tools/merge_projects.py
```

