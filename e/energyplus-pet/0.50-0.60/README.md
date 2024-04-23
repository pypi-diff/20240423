# Comparing `tmp/energyplus_pet-0.50.tar.gz` & `tmp/energyplus_pet-0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyplus_pet-0.50.tar", last modified: Fri Jun  2 22:04:22 2023, max compression
+gzip compressed data, was "energyplus_pet-0.60.tar", last modified: Tue Apr 23 14:08:50 2024, max compression
```

## Comparing `energyplus_pet-0.50.tar` & `energyplus_pet-0.60.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/
--rw-r--r--   0 runner    (1001) docker     (122)     1735 2023-06-02 22:03:51.000000 energyplus_pet-0.50/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-06-02 22:04:22.443636 energyplus_pet-0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-02 22:03:51.000000 energyplus_pet-0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.439636 energyplus_pet-0.50/energyplus_pet/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/configure.py
--rw-r--r--   0 runner    (1001) docker     (122)     7858 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/correction_factor.py
--rw-r--r--   0 runner    (1001) docker     (122)     5776 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/data_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/energyplus_pet/equipment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13066 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/column_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     2291 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/common_curves.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/equip_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    20165 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wahp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15424 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wahp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wwhp_cooling_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)    15053 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/equipment/wwhp_heating_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)      137 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/energyplus_pet/forms/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16776 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/base_data_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/basic_message_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     4170 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/catalog_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/comparison_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/constant_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)    22194 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/correction_detail_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     9698 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/correction_summary_form.py
--rw-r--r--   0 runner    (1001) docker     (122)     6408 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/correction_summary_widget.py
--rw-r--r--   0 runner    (1001) docker     (122)     3421 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/header_preview.py
--rw-r--r--   0 runner    (1001) docker     (122)    31620 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/forms/main.py
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    12745 2023-06-02 22:03:51.000000 energyplus_pet-0.50/energyplus_pet/units.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 22:04:22.443636 energyplus_pet-0.50/energyplus_pet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2720 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1364 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 22:04:22.000000 energyplus_pet-0.50/energyplus_pet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-02 22:04:22.447636 energyplus_pet-0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1944 2023-06-02 22:03:51.000000 energyplus_pet-0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-23 14:08:33.000000 energyplus_pet-0.60/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-23 14:08:50.194627 energyplus_pet-0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-23 14:08:33.000000 energyplus_pet-0.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.190627 energyplus_pet-0.60/energyplus_pet/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/correction_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/data_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/energyplus_pet/equipment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13225 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/column_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/common_curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/equip_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20165 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wahp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15424 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wahp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wwhp_cooling_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15053 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/equipment/wwhp_heating_curve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/energyplus_pet/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/base_data_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/basic_message_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/catalog_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/comparison_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8198 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/constant_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22344 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/correction_detail_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/correction_summary_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/correction_summary_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/header_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/forms/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12745 2024-04-23 14:08:33.000000 energyplus_pet-0.60/energyplus_pet/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:08:50.194627 energyplus_pet-0.60/energyplus_pet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 14:08:50.000000 energyplus_pet-0.60/energyplus_pet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 14:08:50.194627 energyplus_pet-0.60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-23 14:08:33.000000 energyplus_pet-0.60/setup.py
```

### Comparing `energyplus_pet-0.50/LICENSE.txt` & `energyplus_pet-0.60/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/PKG-INFO` & `energyplus_pet-0.60/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus_pet
-Version: 0.50
+Version: 0.60
 Summary: Parameter Estimation Tools for Generating EnergyPlus Inputs from Raw Performance Data
 Home-page: https://github.com/Myoldmopar/EnergyPlusPet
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus "PET"
         
         This project is a cross platform Python (Tk) GUI and tool kit for generating EnergyPlus inputs from component performance data.
```

### Comparing `energyplus_pet-0.50/README.md` & `energyplus_pet-0.60/README.md`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/correction_factor.py` & `energyplus_pet-0.60/energyplus_pet/correction_factor.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/data_manager.py` & `energyplus_pet-0.60/energyplus_pet/data_manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/base.py` & `energyplus_pet-0.60/energyplus_pet/equipment/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import abstractmethod
+from math import sqrt
 from typing import Callable, Dict, List, Tuple
 
-from numpy import sqrt, diag, average
 from scipy.optimize import curve_fit
 
 from energyplus_pet.equipment.equip_types import EquipType
 from energyplus_pet.equipment.column_header import ColumnHeaderArray
 from energyplus_pet.units import UnitType
 
 
@@ -252,15 +252,18 @@
         curve_fit_response = curve_fit(
             eval_function,
             independent_variable_arrays,
             dependent_variable_array
         )
         raw_parameters = curve_fit_response[0]
         calculated_parameters = list(raw_parameters)
-        average_err_one_sigma = average(sqrt(diag(curve_fit_response[1])))
+        diagonal = curve_fit_response[1].diagonal()
+        square_roots = [sqrt(d) for d in diagonal]
+        average_err_one_sigma = sum(square_roots) / len(square_roots)
+        # average_err_one_sigma = average(sqrt(diag(curve_fit_response[1])))
         return calculated_parameters, average_err_one_sigma
 
     @staticmethod
     def eval_curve_at_points(
             eval_function: Callable,
             independent_variable_arrays: Tuple[List[float], ...],
             generated_parameter_array: List[float],
```

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/column_header.py` & `energyplus_pet-0.60/energyplus_pet/equipment/column_header.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/common_curves.py` & `energyplus_pet-0.60/energyplus_pet/equipment/common_curves.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/equip_types.py` & `energyplus_pet-0.60/energyplus_pet/equipment/equip_types.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/manager.py` & `energyplus_pet-0.60/energyplus_pet/equipment/manager.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/wahp_cooling_curve.py` & `energyplus_pet-0.60/energyplus_pet/equipment/wahp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/wahp_heating_curve.py` & `energyplus_pet-0.60/energyplus_pet/equipment/wahp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/wwhp_cooling_curve.py` & `energyplus_pet-0.60/energyplus_pet/equipment/wwhp_cooling_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/equipment/wwhp_heating_curve.py` & `energyplus_pet-0.60/energyplus_pet/equipment/wwhp_heating_curve.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/base_data_form.py` & `energyplus_pet-0.60/energyplus_pet/forms/base_data_form.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from enum import Enum, auto
 from tkinter import Toplevel, Frame, LabelFrame  # containers
 from tkinter import Button, Label  # widgets
 from tkinter import HORIZONTAL, TOP, X, BOTH, ALL  # appearance attributes
 from tkinter import StringVar  # dynamic variables
 from tkinter.ttk import Separator
-from typing import List
 
 from tksheet import Sheet
 
 from energyplus_pet.equipment.base import BaseEquipment
 from energyplus_pet.exceptions import EnergyPlusPetException
 from energyplus_pet.units import unit_class_factory, unit_instance_factory
 from energyplus_pet.forms.basic_message_form import PetMessageForm
@@ -19,291 +18,234 @@
     This form is where the user will enter/paste the raw (typically pretty large) base data set, which will ultimately
     be processed with any correction factors to determine the final data set.
     """
     class MainDataExitCode(Enum):
         Done = auto()
         Cancel = auto()
 
+    class ColumnUnitData:
+        unit_type = None
+        unit_type_class = None
+        unit_id_to_string_mapping = None
+        ip_unit_string = None
+        preferred_unit_string = None
+        units_are_preferred = True  # defaulted to True since we'll assume proper units
+
+        def __str__(self) -> str:
+            return f"{self.unit_type}: {self.unit_type_class}"
+
     def __init__(self, parent_window, eq: BaseEquipment):
-        super().__init__(parent_window, height=200, width=200)
+        super().__init__(parent_window, height=200, width=300)
         self.title(f"{parent_window.title()}: Main Catalog Data Input")
         p = 4
-        self.equipment_instance = eq
+        self.equip = eq
         self.exit_code = MainDataForm.MainDataExitCode.Done
         self.need_to_conform_units = False
-        self.final_base_data_rows: List[List[float]] = [[]]
+        self.final_base_data_rows: list[list[float]] = [[]]
         # create all the objects
         Label(
             self, text="""Now it's time to copy in the bulk of the catalog data.
 To be brought in properly, the data should be divided into columns, delimited by tab characters.
 This is the way most spreadsheets will store data in the clipboard, so the preferred approach is
 to paste/cleanup the data in a spreadsheet, then copy the data and paste directly in the table here."""
         ).pack(
             side=TOP, fill=X, expand=False, padx=p, pady=p
         )
         #
         Separator(self, orient=HORIZONTAL).pack(side=TOP, fill=X, expand=False, padx=p, pady=p)
         #
         tabular_frame = Frame(self)
-        column_titles = eq.headers().name_array()
         column_units = eq.headers().unit_array()
-        self.table = Sheet(tabular_frame)
-        pretend_data = []
+        self.num_columns = len(column_units)
+        self.table = Sheet(
+            tabular_frame,
+            expand_sheet_if_paste_too_big=True,
+            paste_insert_column_limit=self.num_columns,
+            startup_select=(1, 1, 1, 1, "cells"),
+            align="c",
+            header_align="c",
+            headers=eq.headers().name_array(),
+            data=[[0.0 for _ in range(self.num_columns)] for _ in range(eq.minimum_data_points_for_generation())]
+        )
+
         # Would be nice to create a struct of extra data and tag each column with it rather than separate lists
-        self.columnar_unit_types = []
-        self.columnar_unit_type_classes = []
-        self.columnar_unit_id_to_string_mapping = []  # keep this for convenience
-        self.columnar_ip_unit_string = []
-        self.columnar_preferred_unit_string = []
-        self.columnar_units_are_preferred = []  # boolean check
-        for row in range(eq.minimum_data_points_for_generation() + 1):
-            this_row = []
-            if row == 0:
-                for col in range(len(column_units)):
-                    this_column_unit_type = column_units[col]
-                    this_column_unit_type_class = unit_class_factory(this_column_unit_type)
-                    self.columnar_unit_type_classes.append(this_column_unit_type_class)
-                    this_column_unit_id_to_string_mapping = this_column_unit_type_class.get_unit_string_map()
-                    this_column_unit_strings = list(this_column_unit_id_to_string_mapping.values())
-                    this_column_preferred_unit_id = this_column_unit_type_class.calculation_unit_id()
-                    preferred_unit_string = this_column_unit_id_to_string_mapping[this_column_preferred_unit_id]
-                    self.columnar_unit_types.append(this_column_unit_type)
-                    self.columnar_unit_id_to_string_mapping.append(this_column_unit_id_to_string_mapping)
-                    self.columnar_preferred_unit_string.append(preferred_unit_string)
-                    self.columnar_ip_unit_string.append(
-                        this_column_unit_id_to_string_mapping[this_column_unit_type_class.base_ip_unit_id()]
-                    )
-                    self.columnar_units_are_preferred.append(True)
-                    this_row.append(f"{preferred_unit_string}")
-                    self.table.create_dropdown(
-                        r=row,
-                        c=col,
-                        values=this_column_unit_strings,
-                        set_value=preferred_unit_string,
-                        state="readonly",
-                        redraw=False,
-                        selection_function=self._units_changed,
-                        modified_function=None
-                    )
-            else:
-                for col in range(len(column_units)):
-                    this_row.append(0.0)
-            pretend_data.append(this_row)
+        self.columnar = [MainDataForm.ColumnUnitData() for _ in range(len(column_units))]
+        for col in range(self.num_columns):
+            this_column_unit_type = column_units[col]
+            this_column_unit_type_class = unit_class_factory(this_column_unit_type)
+            self.columnar[col].unit_type_class = this_column_unit_type_class
+            this_column_unit_id_to_string_mapping = this_column_unit_type_class.get_unit_string_map()
+            this_column_unit_strings = list(this_column_unit_id_to_string_mapping.values())
+            this_column_preferred_unit_id = this_column_unit_type_class.calculation_unit_id()
+            preferred_unit_string = this_column_unit_id_to_string_mapping[this_column_preferred_unit_id]
+            self.columnar[col].unit_type = this_column_unit_type
+            self.columnar[col].unit_id_to_string_mapping = this_column_unit_id_to_string_mapping
+            self.columnar[col].preferred_unit_string = preferred_unit_string
+            base_ip_unit_id = this_column_unit_type_class.base_ip_unit_id()
+            self.columnar[col].ip_unit_string = (this_column_unit_id_to_string_mapping[base_ip_unit_id])
+            self.table.dropdown(
+                self.table.span(0, col),
+                values=this_column_unit_strings,
+                set_value=preferred_unit_string,
+                state="readonly",
+            )
         self._num_bad_cells = 0
-        self.table.headers(column_titles)
-        self.table.set_sheet_data(pretend_data)
         self.table.enable_bindings()
-        self.table.set_options(expand_sheet_if_paste_too_big=True, paste_insert_column_limit=0)
-        self.table.hide(canvas="row_index")
-        self.table.hide(canvas="top_left")
         self.table.set_all_cell_sizes_to_text(redraw=True)
-        self.table.extra_bindings("end_edit_cell", func=self._cell_edited)
-        self.table.extra_bindings("end_paste", func=self._cells_pasted)
+        self.table.edit_validation(self._cell_edited)
+        # self.table.extra_bindings("end_edit_cell", func=self._cell_edited)
+        self.table.extra_bindings("end_paste", func=self._analyze_table_data)
         # Undo events in the table could bypass our bindings, need to verify this
         self.table.select_cell(row=1, column=0)
         self.table.pack(side=TOP, expand=True, fill=BOTH, padx=p, pady=p)
-        self.table.focus()
-        self.expected_num_columns = self.table.total_columns()  # save this to verify later
         tabular_frame.pack(side=TOP, fill=BOTH, expand=True, padx=p, pady=p)
-        Label(
-            self,
-            text="""Once the numeric data is in place, set the numeric units for each column, conform the data if
-         necessary, and continue the wizard."""
-        ).pack(
+        Label(self, text="""Enter numeric data, set units for each column, then press Conform/OK to continue.""").pack(
             side=TOP, fill=X, expand=False, padx=p, pady=p
         )
-
         #
         Separator(self, orient=HORIZONTAL).pack(side=TOP, fill=X, expand=False, padx=p, pady=p)
         #
         bottom_button_frame = Frame(self)
-        table_ops_label_frame = LabelFrame(bottom_button_frame, text="Table Operations")
-        Button(
-            table_ops_label_frame, text="Add Table Rows", command=self._add_more_table_rows
-        ).grid(
-            row=0, column=0, padx=p, pady=p
-        )
-        Button(
-            table_ops_label_frame, text="Shrink Table to Data", command=self._shrink_table_to_data
-        ).grid(
-            row=0, column=1, padx=p, pady=p
-        )
-        table_ops_label_frame.grid(row=0, column=0, padx=p, pady=p)
-        # Button(
-        #     bottom_button_frame, text="Repair Data Column Order", state=DISABLED, command=self._repair
-        # ).grid(
-        #     row=0, column=1, padx=p, pady=p
-        # )
         quick_convert_label_frame = LabelFrame(bottom_button_frame, text="Quick Convert Units")
         Button(
             quick_convert_label_frame, text="IP Units", command=self._quick_convert_ip
         ).grid(
             row=0, column=0, padx=p, pady=p
         )
         Button(
             quick_convert_label_frame, text="SI Units", command=self._quick_convert_si
         ).grid(
             row=0, column=1, padx=p, pady=p
         )
-        quick_convert_label_frame.grid(row=0, column=1, padx=p, pady=p)
+        quick_convert_label_frame.grid(row=0, column=0, padx=p, pady=p)
         workflow_control_label_frame = LabelFrame(bottom_button_frame, text="Primary Controls")
-        self.done_conform_text = StringVar(value="Done, Continue")
+        self.done_conform_text = StringVar(value="OK, Continue")
         Button(
             workflow_control_label_frame, textvariable=self.done_conform_text, command=self._done_or_conform
         ).grid(
             row=0, column=3, padx=p, pady=p
         )
         Button(
             workflow_control_label_frame, text="Cancel Wizard", command=self.cancel
         ).grid(row=0, column=4, padx=p, pady=p)
-        workflow_control_label_frame.grid(row=0, column=2, padx=p, pady=p)
+        workflow_control_label_frame.grid(row=0, column=1, padx=p, pady=p)
         bottom_button_frame.grid_columnconfigure(ALL, weight=1)
         bottom_button_frame.pack(side=TOP, fill=X, expand=False, padx=p, pady=p)
 
         # set up keybinding and flags
         self.bind('<Key>', self._handle_button_pressed)
 
+        self.table.focus()
+        self.table.see()
+        self.table.redraw()
+
         # finalize UI operations
         self.grab_set()
         self.transient(parent_window)
 
     def _handle_button_pressed(self, event):
         # relevant_modifiers
         # mod_shift = 0x1
         mod_control = 0x4
         # mod_alt = 0x20000
-        if event.keysym == 'a' and mod_control & event.state:
-            self._add_more_table_rows()
-        elif event.keysym == 'd' and mod_control & event.state:
+        if event.keysym == 'd' and mod_control & event.state:
             for row in range(self.table.total_rows()):
                 if row == 0:
                     continue
                 for col in range(self.table.total_columns()):
                     self.table.set_cell_data(row, col, (row + 1.0) * (col + 1.0))
             self.table.redraw()
-            self._cells_pasted()
+            self._analyze_table_data()
 
     def _cell_edited(self, event):
-        row = event.row
-        if row == 0:
-            return
-        column = event.column
-        # first check the current value to see if it was already bad -- it will be the old value in the cell
-        current_value = self.table.get_cell_data(row, column)
-        try:
-            float(current_value)
-            was_good = True
-        except ValueError:
-            was_good = False
-        try:
-            float(event.text)
-            self.table.highlight_cells(row, column, bg='white')
-            # if it was good already, and good now, we are done
-            # if it was bad, and now good, decrement the counter
-            if not was_good:
-                self._num_bad_cells -= 1
-        except ValueError:
-            self.table.highlight_cells(row, column, bg='pink')
-            # if it was bad already, and bad now, we are done
-            # if it was good, and now bad, increment the counter
-            if was_good:
-                self._num_bad_cells += 1
+        for (row, column), old_value in event.cells.table.items():
+            if row == 0:
+                # we are in a units row, handle that here
+                if event.value != self.columnar[column].preferred_unit_string:
+                    self.need_to_conform_units = True
+                self._analyze_table_data()  # simulate a paste event
+                self.refresh_done_conform_button_text()
+                return event.value
+            # first check the current value to see if it was already bad -- it will be the old value in the cell
+            try:
+                float(old_value)
+                was_good = True
+            except ValueError:
+                was_good = False
+            try:
+                float(event.value)
+                self.table.highlight_cells(row, column, bg='white')
+                # if it was good already, and good now, we are done
+                # if it was bad, and now good, decrement the counter
+                if not was_good:
+                    self._num_bad_cells -= 1
+            except KeyError:
+                attrs = ", ".join(event.keys())
+                print(f"Could not access value attribute on event.  Available attributes include: {attrs}")
+            except ValueError:
+                self.table.highlight_cells(row, column, bg='pink')
+                # if it was bad already, and bad now, we are done
+                # if it was good, and now bad, increment the counter
+                if was_good:
+                    self._num_bad_cells += 1
         self.table.redraw()
+        return event.value
 
-    def _cells_pasted(self, _=None):
+    def _analyze_table_data(self, _=None):
         self._num_bad_cells = 0
         for row in range(self.table.total_rows()):
             if row == 0:
                 continue
             for column in range(self.table.total_columns()):
                 try:
-                    float(self.table.get_cell_data(row, column))
+                    float(self.table.data[row][column])
                     self.table.highlight_cells(row, column, bg='white')
                 except ValueError:
                     self._num_bad_cells += 1
                     self.table.highlight_cells(row, column, bg='pink')
         self.table.redraw()
 
-    def _table_data_all_good(self) -> bool:
-        return self._num_bad_cells == 0
-
-    def _add_more_table_rows(self):
-        self.table.insert_rows(rows=10, redraw=True)
-
-    def _shrink_table_to_data(self):
-        # first find the extents of the data
-        current_visible_rows = self.table.total_rows()
-        max_row_index_found = 0
-        for row in range(current_visible_rows):
-            for col in range(self.table.total_columns()):
-                if self.table.get_cell_data(row, col) != '':
-                    max_row_index_found = max(max_row_index_found, row)
-        # constrain it to the minimums
-        minimum_rows = 2  # with the use of correction factors, we are ok allowing just one row here
-        desired_row_count = max(max_row_index_found, minimum_rows)
-        # if table is larger than desired, start at the end and remove until we get to the desired value
-        if current_visible_rows > desired_row_count:
-            for r in range(current_visible_rows - 1, desired_row_count, -1):
-                self.table.delete_row(r)
-        self.table.redraw()
-
     def any_blank_cells(self):
         for row in range(self.table.total_rows()):
             for col in range(self.table.total_columns()):
-                if self.table.get_cell_data(row, col) == '':
+                if self.table.data[row][col] == '':
                     return True
         return False
 
-    # def _repair(self): pass
-
     def _quick_convert_ip(self):
         for col_num in range(self.table.total_columns()):
-            self.table.set_cell_data(0, col_num, self.columnar_ip_unit_string[col_num], redraw=True)
-        self._units_changed()
+            self.table.set_cell_data(0, col_num, self.columnar[col_num].ip_unit_string, redraw=True)
+        self.need_to_conform_units = True  # since we are converting to IP, we know this
+        self.refresh_done_conform_button_text()
 
     def _quick_convert_si(self):
         for col_num in range(self.table.total_columns()):
-            self.table.set_cell_data(0, col_num, self.columnar_preferred_unit_string[col_num], redraw=True)
-        self._units_changed()
-
-    def _units_changed(self, dropdown_edit_cell_event=None):
-        this_column = dropdown_edit_cell_event.column if dropdown_edit_cell_event else None
-        self.need_to_conform_units = False
-        for c in range(self.table.total_columns()):
-            if c == this_column:
-                units_value_this_column = dropdown_edit_cell_event.text  # currently being modified
-            else:
-                units_value_this_column = self.table.get_cell_data(0, c)  # just get the data from the cell
-            if units_value_this_column != self.columnar_preferred_unit_string[c]:
-                self.need_to_conform_units = True
-        self._cells_pasted()  # simulate a paste event
+            self.table.set_cell_data(0, col_num, self.columnar[col_num].preferred_unit_string, redraw=True)
+        self.need_to_conform_units = False  # since we are converting to SI, we know this
         self.refresh_done_conform_button_text()
 
     def refresh_done_conform_button_text(self):
         if self.need_to_conform_units:
             self.done_conform_text.set("Conform units")
         else:
-            self.done_conform_text.set("Done, Continue")
+            self.done_conform_text.set("OK, Continue")
         self.table.redraw()
 
-    def _update_from_traces(self):
-        pass
-
     def _done_or_conform(self):
         # don't try to conorm or exit if there are any bad values
-        if not self._table_data_all_good():
+        if self._num_bad_cells > 0:
             message_window = PetMessageForm(
                 self, "Value Issue", f"{self._num_bad_cells} cell(s) appear to have bad values; fix them and retry"
             )
             self.wait_window(message_window)
             return
         if self.need_to_conform_units:
             self.conform_units()
         else:
-            if self.expected_num_columns != self.table.total_columns():
+            if self.num_columns != self.table.total_columns():
                 message_window = PetMessageForm(
                     self,
                     "Problem with Table Size",
                     "It appears the table column size does not match the expected size, this is odd, cancel and retry"
                 )
                 self.wait_window(message_window)
                 return
@@ -318,37 +260,37 @@
             self.exit_code = MainDataForm.MainDataExitCode.Done
             self.final_base_data_rows = []
             for row in range(self.table.total_rows()):
                 if row == 0:  # unit row
                     continue
                 this_row = []
                 for column in range(self.table.total_columns()):
-                    this_row.append(float(self.table.get_cell_data(row, column)))
+                    this_row.append(float(self.table.data[row][column]))
                 self.final_base_data_rows.append(this_row)
             self.grab_release()
             self.destroy()
 
     def conform_units(self):
         """This is a pretty convoluted way to do this, think harder"""
         for c in range(self.table.total_columns()):
-            current_units_string = self.table.get_cell_data(0, c)
-            if current_units_string != self.columnar_preferred_unit_string[c]:
+            current_units_string = self.table.data[0][c]
+            if current_units_string != self.columnar[c].preferred_unit_string:
                 try:
-                    current_unit_id = self.columnar_unit_type_classes[c].get_id_from_unit_string(current_units_string)
+                    current_unit_id = self.columnar[c].unit_type_class.get_id_from_unit_string(current_units_string)
                 except EnergyPlusPetException:
                     pmf = PetMessageForm(self, "Unit ID Problem", "Could not match unit ID; this is a developer issue.")
                     self.wait_window(pmf)
                     self.cancel()
                     return
                 for r in range(self.table.total_rows()):
                     if r == 0:
-                        self.table.set_cell_data(r, c, self.columnar_preferred_unit_string[c])
+                        self.table.set_cell_data(r, c, self.columnar[c].preferred_unit_string)
                     else:
-                        cell_value = float(self.table.get_cell_data(r, c))
-                        unit_value = unit_instance_factory(cell_value, self.columnar_unit_types[c])
+                        cell_value = float(self.table.data[r][c])
+                        unit_value = unit_instance_factory(cell_value, self.columnar[c].unit_type)
                         unit_value.units = current_unit_id
                         unit_value.convert_to_calculation_unit()
                         self.table.set_cell_data(r, c, unit_value.value)
         self.need_to_conform_units = False
         self.refresh_done_conform_button_text()
 
     def cancel(self):
```

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/basic_message_form.py` & `energyplus_pet-0.60/energyplus_pet/forms/basic_message_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/catalog_plot.py` & `energyplus_pet-0.60/energyplus_pet/forms/catalog_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from enum import Enum, auto
-import numpy as np
 from tkinter import Toplevel, Frame  # containers
 from tkinter import Button, Label  # widgets
 from tkinter import TOP, X, BOTH, ALL  # appearance stuff
 from tkinter.ttk import Notebook, Style  # ttk specific stuff
 
 from energyplus_pet.data_manager import CatalogDataManager
 from energyplus_pet.equipment.base import BaseEquipment
@@ -48,15 +47,15 @@
             )
         for pd in plot_data:
             plot_frame = Frame(plot_notebook)
             plot_frame.pack(side=TOP, expand=True, fill=BOTH)
             plot_notebook.add(plot_frame, text=pd[0])
             fig = Figure(figsize=(7, 5))
             a = fig.add_subplot(111)
-            a.plot(np.array(pd[1]), np.array(pd[2]))
+            a.plot(pd[1], pd[2])
             a.set_title("Catalog Data Display", fontsize=16)
             a.set_ylabel(f"[{pd[3]}]", fontsize=14)
             a.set_xlabel("Catalog Data Points (no order)", fontsize=14)
             canvas = FigureCanvasTkAgg(fig, master=plot_frame)
             canvas.get_tk_widget().pack()
             canvas.draw()
         plot_notebook.pack(side=TOP, expand=True, fill=BOTH, padx=p, pady=p)
```

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/comparison_plot.py` & `energyplus_pet-0.60/energyplus_pet/forms/comparison_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from enum import auto, Enum
 
-import numpy as np
 from tkinter import Frame, Toplevel, TOP, BOTH, Tk, Label, X, Button
 from tkinter.ttk import Notebook, Separator
 
 from energyplus_pet.data_manager import CatalogDataManager
 from energyplus_pet.equipment.base import BaseEquipment
 from energyplus_pet.exceptions import EnergyPlusPetException
 
@@ -57,15 +56,15 @@
             for pd in data_this_plot_type['plot_data']:
                 if pd[1] == 'line':
                     line_arg = '-'
                 elif pd[1] == 'point':
                     line_arg = '--'
                 else:
                     raise EnergyPlusPetException('bad line type')
-                a.plot(np.array(pd[3]), label=pd[0], linestyle=line_arg, color=pd[2])
+                a.plot(pd[3], label=pd[0], linestyle=line_arg, color=pd[2])
             a.legend()
             a.set_title(plot_title, fontsize=16)
             a.set_xlabel("Catalog Data Points (no order)")
             a.set_ylabel(data_this_plot_type['y_label'])
             canvas = FigureCanvasTkAgg(fig, master=plot_frame)
             canvas.get_tk_widget().pack(side=TOP, expand=True, fill=BOTH)
             canvas.draw()
```

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/constant_parameters.py` & `energyplus_pet-0.60/energyplus_pet/forms/constant_parameters.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/correction_detail_form.py` & `energyplus_pet-0.60/energyplus_pet/forms/correction_detail_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             )
             db_wb_frame.pack(side=TOP, fill=X, expand=False, padx=p, pady=p)
             Separator(self, orient=HORIZONTAL).pack(side=TOP, fill=X, expand=False, padx=p, pady=p)
 
         elif _cf.correction_type == CorrectionFactorType.Replacement:
             Label(self, text=f"""Entering correction data for ~~ {_cf.name} ~~
 
-This correction factor requires {_cf.num_corrections} replacement values for both dry and wet bulb temps.
+This correction factor requires {_cf.num_corrections} replacement values for the specified independent variable.
 
 The correction factor requires multiplier values for the following {len(_cf.columns_to_modify)} column(s):
 {dep_column_names}""").pack(side=TOP, fill=X, anchor=W, expand=False, padx=p, pady=p)
             replacement_frame = Frame(self)
             replacement_label = Label(replacement_frame, text="Specify the units of the replacement data (column 1):")
             # all we need to do is look up the UnitType for the replacement column
             # from this type, we can get a Base unit class and get everything we need from it.
@@ -121,31 +121,29 @@
             column_titles.append(eq.headers().name_array()[eq.headers().get_db_column()])
             column_titles.append(eq.headers().name_array()[eq.headers().get_wb_column()])
         # then add the dependent variables
         for mod_column in _cf.columns_to_modify:
             column_titles.append(eq.headers().name_array()[mod_column])
         num_columns_in_table = len(column_titles)
         num_rows_in_table = self.completed_factor.num_corrections  # no need to add a header or anything here
-        pretend_data = []
-        for row in range(num_rows_in_table):
-            this_row = []
-            for col in range(num_columns_in_table):
-                this_row.append(0.0)
-            pretend_data.append(this_row)
         self._num_bad_cells = 0
-        self.table = Sheet(self.tabular_frame)
-        self.table.set_sheet_data(pretend_data)
-        self.table.headers(column_titles)
+        self.table = Sheet(
+            self.tabular_frame,
+            expand_sheet_if_paste_too_big=False,
+            startup_select=(1, 1, 1, 1, "cells"),
+            align="c",
+            header_align="c",
+            headers=column_titles,
+            data=[[0.0 for _ in range(num_columns_in_table)] for _ in range(num_rows_in_table)]
+        )
         self.table.enable_bindings()
-        self.table.set_options(expand_sheet_if_paste_too_big=False)
-        self.table.hide(canvas="row_index")
-        self.table.hide(canvas="top_left")
         self.table.set_all_cell_sizes_to_text(redraw=True)
         # https://github.com/ragardner/tksheet/blob/master/DOCUMENTATION.md#25-example-custom-right-click-and-text-editor-functionality
-        self.table.extra_bindings("end_edit_cell", func=self._cell_edited)
+        self.table.edit_validation(self._cell_edited)
+        # self.table.extra_bindings([("end_edit_cell", self._cell_edited)])
         self.table.extra_bindings("end_paste", func=self._cells_pasted)
         self.table.pack(side=TOP, expand=True, fill=BOTH, padx=p, pady=p)
         self.table.select_cell(row=0, column=0)
         self.table.focus()
         self.tabular_frame.pack(side=TOP, fill=BOTH, expand=True, padx=p, pady=p)
         # we block resizing the table when pasting, and we are hiding the row titles to block inserting rows via title,
         # but we can't seem to block tksheet from allowing a column insert, so we will just have to check later
@@ -169,14 +167,18 @@
 
         # draw factors, in case there already are any
         # self.draw_factors()
 
         # set up keybinding and flags
         self.bind('<Key>', self._handle_button_pressed)
 
+        self.table.focus()
+        self.table.see()
+        self.table.redraw()
+
         # finalize UI operations
         self.grab_set()
         self.transient(parent_window)
 
     def _handle_button_pressed(self, event):
         # relevant_modifiers
         # mod_shift = 0x1
@@ -185,55 +187,58 @@
         if event.keysym == 'd' and mod_control & event.state:
             for row in range(self.completed_factor.num_corrections):
                 for col in range(len(self.completed_factor.columns_to_modify) + 1):
                     self.table.set_cell_data(row, col, (row + 1.0) * (col + 1.0))
             self._cells_pasted()
 
     def _cell_edited(self, event):
-        row = event.row
-        column = event.column
-        # first check the current value to see if it was already bad -- it will be the old value in the cell
-        current_value = self.table.get_cell_data(row, column)
-        try:
-            float(current_value)
-            was_good = True
-        except ValueError:
-            was_good = False
-        try:
-            float(event.text)
-            self.table.highlight_cells(row, column, bg='white')
-            # if it was good already, and good now, we are done
-            # if it was bad, and now good, decrement the counter
-            if not was_good:
-                self._num_bad_cells -= 1
-        except ValueError:
-            self.table.highlight_cells(row, column, bg='pink')
-            # if it was bad already, and bad now, we are done
-            # if it was good, and now bad, increment the counter
-            if was_good:
-                self._num_bad_cells += 1
+        for (row, column), old_value in event.cells.table.items():
+            # first check the current value to see if it was already bad -- it will be the old value in the cell
+            try:
+                float(old_value)
+                was_good = True
+            except ValueError:
+                was_good = False
+            try:
+                float(event.value)
+                self.table.highlight_cells(row, column, bg='white')
+                # if it was good already, and good now, we are done
+                # if it was bad, and now good, decrement the counter
+                if not was_good:
+                    self._num_bad_cells -= 1
+            except KeyError:
+                attrs = ", ".join(event.keys())
+                print(f"Could not access value attribute on event.  Available attributes include: {attrs}")
+            except ValueError:
+                self.table.highlight_cells(row, column, bg='pink')
+                # if it was bad already, and bad now, we are done
+                # if it was good, and now bad, increment the counter
+                if was_good:
+                    self._num_bad_cells += 1
+        self.table.redraw()
+        return event.value
 
     def _cells_pasted(self, _=None):
         self._num_bad_cells = 0
         for row in range(self.table.total_rows()):
             for column in range(self.table.total_columns()):
                 try:
-                    float(self.table.get_cell_data(row, column))
+                    float(self.table.data[row][column])
                     self.table.highlight_cells(row, column, bg='white')
                 except ValueError:
                     self._num_bad_cells += 1
                     self.table.highlight_cells(row, column, bg='pink')
 
     def _table_data_all_good(self) -> bool:
         return self._num_bad_cells == 0
 
     def any_blank_cells(self):
         for row in range(self.table.total_rows()):
             for col in range(self.table.total_columns()):
-                if self.table.get_cell_data(row, col) == '':
+                if self.table.data[row][col] == '':
                     return True
         return False
 
     def _units_changed(self, *_):
         """This function is called back by the unit traces, just check all of them"""
         self.need_to_conform_units = False
         if self.completed_factor.correction_type == CorrectionFactorType.Multiplier:
@@ -278,44 +283,44 @@
                     "Problem with Table Entries",
                     "Blank entries detected in the table, fix and retry"
                 )
                 self.wait_window(message_window)
                 return
             for r in range(self.table.total_rows()):
                 for c in range(self.table.total_columns()):
-                    value = self.table.get_cell_data(r, c)
+                    value = self.table.data[r][c]
                     if value == '':
                         message_window = PetMessageForm(
                             self,
                             "Problem with Correction Factor Data",
                             "Encountered at least one blank cell in the data, populate the full table and retry"
                         )
                         self.wait_window(message_window)
                         return
             # OK, so if we are done, units must be ready, so we just need to update the data in the correction factor
             # for regular correction factors, read the first column of data into the base correction of the CF
             if self.completed_factor.correction_type != CorrectionFactorType.CombinedDbWb:
                 self.completed_factor.base_correction = [
-                    float(self.table.get_cell_data(row, 0)) for row in range(self.completed_factor.num_corrections)
+                    float(self.table.data[row][0]) for row in range(self.completed_factor.num_corrections)
                 ]
                 last_column_read = 0
             else:  # for db/wb, read the first column into the db array and the second column into the wb array
                 self.completed_factor.base_correction_db = [
-                    float(self.table.get_cell_data(row, 0)) for row in range(self.completed_factor.num_corrections)
+                    float(self.table.data[row][0]) for row in range(self.completed_factor.num_corrections)
                 ]
                 self.completed_factor.base_correction_wb = [
-                    float(self.table.get_cell_data(row, 1)) for row in range(self.completed_factor.num_corrections)
+                    float(self.table.data[row][1]) for row in range(self.completed_factor.num_corrections)
                 ]
                 last_column_read = 1
             # then iterate over the mod column ids of the CF and read the data into lists and then into the CF map
             for equipment_column_index in self.completed_factor.columns_to_modify:
                 last_column_read += 1
                 this_column = []
                 for row in range(self.table.total_rows()):
-                    this_column.append(float(self.table.get_cell_data(row, last_column_read)))
+                    this_column.append(float(self.table.data[row][last_column_read]))
                 self.completed_factor.mod_correction_data_column_map[equipment_column_index] = this_column
             output_message = ""
             db = self.equipment_instance.headers().get_db_column()
             wb = self.equipment_instance.headers().get_wb_column()
             if not self.completed_factor.check_ok(db, wb):
                 output_message += f"Errors for {self.completed_factor.name}:\n"
                 for e in self.completed_factor.check_ok_messages:
@@ -339,15 +344,15 @@
                 current_db_unit_id = self.unit_type_class.get_id_from_unit_string(db_units_string)
             except EnergyPlusPetException:
                 pmf = PetMessageForm(self, "Unit ID Problem", "Could not match unit ID; this is a developer issue.")
                 self.wait_window(pmf)
                 self.cancel()
                 return
             for r in range(self.table.total_rows()):
-                cell_value = float(self.table.get_cell_data(r, 0))
+                cell_value = float(self.table.data[r][0])
                 unit_value = unit_instance_factory(cell_value, self.replacement_column_unit_type)
                 unit_value.units = current_db_unit_id
                 unit_value.convert_to_calculation_unit()
                 self.table.set_cell_data(r, 0, unit_value.value)
             self._tk_var_replacement_units_string.set(self.preferred_replacement_unit_string)
         elif self.completed_factor.correction_type == CorrectionFactorType.CombinedDbWb:
             db_units_string = self._tk_var_db_units_string.get()
@@ -355,30 +360,30 @@
                 current_db_unit_id = TemperatureValue.get_id_from_unit_string(db_units_string)
             except EnergyPlusPetException:
                 pmf = PetMessageForm(self, "Unit ID Problem", "Could not match DB unit ID; this is a developer issue.")
                 self.wait_window(pmf)
                 self.cancel()
                 return
             for r in range(self.table.total_rows()):
-                cell_value = float(self.table.get_cell_data(r, 0))
+                cell_value = float(self.table.data[r][0])
                 unit_value = unit_instance_factory(cell_value, UnitType.Temperature)
                 unit_value.units = current_db_unit_id
                 unit_value.convert_to_calculation_unit()
                 self.table.set_cell_data(r, 0, unit_value.value)
             self._tk_var_db_units_string.set(self.preferred_db_wb_unit_string)
             wb_units_string = self._tk_var_wb_units_string.get()
             try:
                 current_wb_unit_id = TemperatureValue.get_id_from_unit_string(wb_units_string)
             except EnergyPlusPetException:
                 pmf = PetMessageForm(self, "Unit ID Problem", "Could not match WB unit ID; this is a developer issue.")
                 self.wait_window(pmf)
                 self.cancel()
                 return
             for r in range(self.table.total_rows()):
-                cell_value = float(self.table.get_cell_data(r, 1))
+                cell_value = float(self.table.data[r][1])
                 unit_value = unit_instance_factory(cell_value, UnitType.Temperature)
                 unit_value.units = current_wb_unit_id
                 unit_value.convert_to_calculation_unit()
                 self.table.set_cell_data(r, 1, unit_value.value)
             self._tk_var_wb_units_string.set(self.preferred_db_wb_unit_string)
         self.need_to_conform_units = False
         self._refresh_done_conform_button_text()
```

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/correction_summary_form.py` & `energyplus_pet-0.60/energyplus_pet/forms/correction_summary_form.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/correction_summary_widget.py` & `energyplus_pet-0.60/energyplus_pet/forms/correction_summary_widget.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/header_preview.py` & `energyplus_pet-0.60/energyplus_pet/forms/header_preview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from tkinter import Toplevel, Button, Frame, Label, HORIZONTAL, TOP, X
 from tkinter.ttk import Separator
 
-from pyperclip import copy
-
 from energyplus_pet.equipment.base import BaseEquipment
 
 
 class RequiredDataPreviewForm(Toplevel):
     """Allows users to view the required equipment data and copy it to the clipboard"""
     def __init__(self, parent_window, equipment: BaseEquipment):
         super().__init__(parent_window)
@@ -43,18 +41,20 @@
         button_frame.grid_columnconfigure(2, weight=1)
         button_frame.pack(side=TOP, fill=X, expand=False, padx=3, pady=3)
         # finalize UI operations
         self.grab_set()
         self.transient(parent_window)
 
     def _copy(self):
-        copy(self._summary)
+        self.clipboard_clear()
+        self.clipboard_append(self._summary)
 
     def _copy_csv(self):
-        copy(self._csv)
+        self.clipboard_clear()
+        self.clipboard_append(self._csv)
 
     def _done(self):
         self.grab_release()
         self.destroy()
 
 
 if __name__ == "__main__":
```

### Comparing `energyplus_pet-0.50/energyplus_pet/forms/main.py` & `energyplus_pet-0.60/energyplus_pet/forms/main.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet/units.py` & `energyplus_pet-0.60/energyplus_pet/units.py`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/energyplus_pet.egg-info/PKG-INFO` & `energyplus_pet-0.60/energyplus_pet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyplus-pet
-Version: 0.50
+Version: 0.60
 Summary: Parameter Estimation Tools for Generating EnergyPlus Inputs from Raw Performance Data
 Home-page: https://github.com/Myoldmopar/EnergyPlusPet
 Author: Edwin Lee, for NREL, for United States Department of Energy
 License: ModifiedBSD
 Description: # EnergyPlus "PET"
         
         This project is a cross platform Python (Tk) GUI and tool kit for generating EnergyPlus inputs from component performance data.
```

### Comparing `energyplus_pet-0.50/energyplus_pet.egg-info/SOURCES.txt` & `energyplus_pet-0.60/energyplus_pet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `energyplus_pet-0.50/setup.py` & `energyplus_pet-0.60/setup.py`

 * *Files identical despite different names*

