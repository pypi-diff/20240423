# Comparing `tmp/energyplus_pet-0.60.tar.gz` & `tmp/energyplus_pet-0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_pet-0.60.tar", last modified: Tue Apr 23 14:08:50 2024, max compression
+gzip compressed data, was "energyplus_pet-0.61.tar", last modified: Tue Apr 23 14:29:01 2024, max compression
```

## Comparing `energyplus_pet-0.60.tar` & `energyplus_pet-0.61.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-23 14:08:33.000000 energyplus_pet-0.60/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-23 14:08:50.194627 energyplus_pet-0.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-23 14:08:33.000000 energyplus_pet-0.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.190627 energyplus_pet-0.60/energyplus_pet/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/correction_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/energyplus_pet/equipment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/column_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/common_curves.py
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/equip_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    20165 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wahp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wahp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wwhp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wwhp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/energyplus_pet/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/base_data_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/basic_message_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/catalog_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/comparison_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/constant_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    22344 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/correction_detail_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/correction_summary_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/correction_summary_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/header_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/energyplus_pet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 14:08:50.194627 energyplus_pet-0.60/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-23 14:08:33.000000 energyplus_pet-0.60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:01.123963 energyplus_pet-0.61/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-23 14:28:35.000000 energyplus_pet-0.61/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-23 14:29:01.123963 energyplus_pet-0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-23 14:28:35.000000 energyplus_pet-0.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:01.119963 energyplus_pet-0.61/energyplus_pet/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/correction_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:01.119963 energyplus_pet-0.61/energyplus_pet/equipment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/column_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/common_curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/equip_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20165 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/wahp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/wahp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/wwhp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/equipment/wwhp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:01.123963 energyplus_pet-0.61/energyplus_pet/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/base_data_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/basic_message_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/catalog_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/comparison_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/constant_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22344 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/correction_detail_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/correction_summary_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/correction_summary_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/header_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/forms/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-23 14:28:35.000000 energyplus_pet-0.61/energyplus_pet/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:01.119963 energyplus_pet-0.61/energyplus_pet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-23 14:29:00.000000 energyplus_pet-0.61/energyplus_pet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 14:29:00.000000 energyplus_pet-0.61/energyplus_pet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:29:00.000000 energyplus_pet-0.61/energyplus_pet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 14:29:00.000000 energyplus_pet-0.61/energyplus_pet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 14:29:00.000000 energyplus_pet-0.61/energyplus_pet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 14:29:00.000000 energyplus_pet-0.61/energyplus_pet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 14:29:01.123963 energyplus_pet-0.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-23 14:28:35.000000 energyplus_pet-0.61/setup.py
```

### Comparing `energyplus_pet-0.60/LICENSE.txt` & `energyplus_pet-0.61/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/PKG-INFO` & `energyplus_pet-0.61/energyplus_pet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: energyplus_pet
-Version: 0.60
+Name: energyplus-pet
+Version: 0.61
 Summary: Parameter Estimation Tools for Generating EnergyPlus Inputs from Raw Performance Data
 Home-page: https://github.com/Myoldmopar/EnergyPlusPet
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus "PET"
         
         This project is a cross platform Python (Tk) GUI and tool kit for generating EnergyPlus inputs from component performance data.
```

### Comparing `energyplus_pet-0.60/README.md` & `energyplus_pet-0.61/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/correction_factor.py` & `energyplus_pet-0.61/energyplus_pet/correction_factor.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/data_manager.py` & `energyplus_pet-0.61/energyplus_pet/data_manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/base.py` & `energyplus_pet-0.61/energyplus_pet/equipment/base.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/column_header.py` & `energyplus_pet-0.61/energyplus_pet/equipment/column_header.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/common_curves.py` & `energyplus_pet-0.61/energyplus_pet/equipment/common_curves.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/equip_types.py` & `energyplus_pet-0.61/energyplus_pet/equipment/equip_types.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/manager.py` & `energyplus_pet-0.61/energyplus_pet/equipment/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/wahp_cooling_curve.py` & `energyplus_pet-0.61/energyplus_pet/equipment/wahp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/wahp_heating_curve.py` & `energyplus_pet-0.61/energyplus_pet/equipment/wahp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/wwhp_cooling_curve.py` & `energyplus_pet-0.61/energyplus_pet/equipment/wwhp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/equipment/wwhp_heating_curve.py` & `energyplus_pet-0.61/energyplus_pet/equipment/wwhp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/base_data_form.py` & `energyplus_pet-0.61/energyplus_pet/forms/base_data_form.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
             paste_insert_column_limit=self.num_columns,
             startup_select=(1, 1, 1, 1, "cells"),
             align="c",
             header_align="c",
             headers=eq.headers().name_array(),
             data=[[0.0 for _ in range(self.num_columns)] for _ in range(eq.minimum_data_points_for_generation())]
         )
-
         # Would be nice to create a struct of extra data and tag each column with it rather than separate lists
         self.columnar = [MainDataForm.ColumnUnitData() for _ in range(len(column_units))]
         for col in range(self.num_columns):
             this_column_unit_type = column_units[col]
             this_column_unit_type_class = unit_class_factory(this_column_unit_type)
             self.columnar[col].unit_type_class = this_column_unit_type_class
             this_column_unit_id_to_string_mapping = this_column_unit_type_class.get_unit_string_map()
```

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/basic_message_form.py` & `energyplus_pet-0.61/energyplus_pet/forms/basic_message_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/catalog_plot.py` & `energyplus_pet-0.61/energyplus_pet/forms/catalog_plot.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/comparison_plot.py` & `energyplus_pet-0.61/energyplus_pet/forms/comparison_plot.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/constant_parameters.py` & `energyplus_pet-0.61/energyplus_pet/forms/constant_parameters.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/correction_detail_form.py` & `energyplus_pet-0.61/energyplus_pet/forms/correction_detail_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/correction_summary_form.py` & `energyplus_pet-0.61/energyplus_pet/forms/correction_summary_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/correction_summary_widget.py` & `energyplus_pet-0.61/energyplus_pet/forms/correction_summary_widget.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/header_preview.py` & `energyplus_pet-0.61/energyplus_pet/forms/header_preview.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/forms/main.py` & `energyplus_pet-0.61/energyplus_pet/forms/main.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet/units.py` & `energyplus_pet-0.61/energyplus_pet/units.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/energyplus_pet.egg-info/PKG-INFO` & `energyplus_pet-0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: energyplus-pet
-Version: 0.60
+Name: energyplus_pet
+Version: 0.61
 Summary: Parameter Estimation Tools for Generating EnergyPlus Inputs from Raw Performance Data
 Home-page: https://github.com/Myoldmopar/EnergyPlusPet
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus "PET"
         
         This project is a cross platform Python (Tk) GUI and tool kit for generating EnergyPlus inputs from component performance data.
```

### Comparing `energyplus_pet-0.60/energyplus_pet.egg-info/SOURCES.txt` & `energyplus_pet-0.61/energyplus_pet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.60/setup.py` & `energyplus_pet-0.61/setup.py`

 * *Files identical despite different names*

