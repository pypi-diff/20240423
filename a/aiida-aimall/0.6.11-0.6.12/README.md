# Comparing `tmp/aiida_aimall-0.6.11.tar.gz` & `tmp/aiida_aimall-0.6.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_aimall-0.6.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_aimall-0.6.12.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_aimall-0.6.11.tar` & `aiida_aimall-0.6.12.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/LICENSE
--rw-r--r--   0        0        0     9730 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/README.md
--rw-r--r--   0        0        0       86 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/__init__.py
--rw-r--r--   0        0        0    15415 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/calculations.py
--rw-r--r--   0        0        0    16513 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/controllers.py
--rw-r--r--   0        0        0     3431 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/data/__init__.py
--rw-r--r--   0        0        0    15668 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/parsers.py
--rw-r--r--   0        0        0    21001 2024-04-10 19:24:45.293841 aiida_aimall-0.6.11/aiida_aimall/workchains.py
--rw-r--r--   0        0        0     4707 2024-04-10 19:24:45.297841 aiida_aimall-0.6.11/pyproject.toml
--rw-r--r--   0        0        0    12733 1970-01-01 00:00:00.000000 aiida_aimall-0.6.11/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-23 17:39:16.340071 aiida_aimall-0.6.12/LICENSE
+-rw-r--r--   0        0        0     9730 2024-04-23 17:39:16.340071 aiida_aimall-0.6.12/README.md
+-rw-r--r--   0        0        0       86 2024-04-23 17:39:16.340071 aiida_aimall-0.6.12/aiida_aimall/__init__.py
+-rw-r--r--   0        0        0    15432 2024-04-23 17:39:16.340071 aiida_aimall-0.6.12/aiida_aimall/calculations.py
+-rw-r--r--   0        0        0    16513 2024-04-23 17:39:16.344071 aiida_aimall-0.6.12/aiida_aimall/controllers.py
+-rw-r--r--   0        0        0     3431 2024-04-23 17:39:16.344071 aiida_aimall-0.6.12/aiida_aimall/data/__init__.py
+-rw-r--r--   0        0        0    15668 2024-04-23 17:39:16.344071 aiida_aimall-0.6.12/aiida_aimall/parsers.py
+-rw-r--r--   0        0        0    21039 2024-04-23 17:39:16.344071 aiida_aimall-0.6.12/aiida_aimall/workchains.py
+-rw-r--r--   0        0        0     4707 2024-04-23 17:39:16.344071 aiida_aimall-0.6.12/pyproject.toml
+-rw-r--r--   0        0        0    12733 1970-01-01 00:00:00.000000 aiida_aimall-0.6.12/PKG-INFO
```

### Comparing `aiida_aimall-0.6.11/LICENSE` & `aiida_aimall-0.6.12/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.11/README.md` & `aiida_aimall-0.6.12/README.md`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.11/aiida_aimall/calculations.py` & `aiida_aimall-0.6.12/aiida_aimall/calculations.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,21 +82,21 @@
         # spec.input(
         #     'metadata.options.output_filename', valid_type=str, default='aiida.out'
         # )
         spec.input(
             "attached_atom_int",
             valid_type=Int,
             help="id # of attached atom for graph descriptor",
-            default=Int(1),
+            default=lambda: Int(1),
         )
         spec.input(
             "group_atoms",
             valid_type=List,
             help="Integer ids of atoms in groups to include",
-            default=List([]),
+            default=lambda: List([]),
         )
         spec.input(
             "parameters",
             valid_type=AimqbParameters,
             help="Command line parameters for aimqb",
         )
         spec.input(
@@ -177,15 +177,15 @@
         which check extras
         parent_calc_folder: RemoteData, optional: the folder of a completed gaussian calculation
 
     Example:
     ::
 
         builder = GaussianCalculation.get_builder()
-        builder.structure_str = orm.Str("H 0.0 0.0 0.0 -1.0 0.0 0.0) # needs newline but docs doesn't like
+        builder.structure_str = orm.Str("H 0.0 0.0 0.0 -1.0 0.0 0.0") # needs newline but docs doesn't like
         builder.parameters = orm.Dict(dict={
             'link0_parameters': {
                 '%chk':'aiida.chk',
                 "%mem": "3200MB", # Currently set to use 8000 MB in .sh files
                 "%nprocshared": 4,
             },
             'functional':'wb97xd',
```

### Comparing `aiida_aimall-0.6.11/aiida_aimall/controllers.py` & `aiida_aimall-0.6.12/aiida_aimall/controllers.py`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.11/aiida_aimall/data/__init__.py` & `aiida_aimall-0.6.12/aiida_aimall/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.11/aiida_aimall/parsers.py` & `aiida_aimall-0.6.12/aiida_aimall/parsers.py`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.11/aiida_aimall/workchains.py` & `aiida_aimall-0.6.12/aiida_aimall/workchains.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,19 +249,21 @@
     """Workchain to fragment a cml file and generate gaussian calculations on each fragment"""
 
     @classmethod
     def define(cls, spec):
         super().define(spec)
         spec.input("cml_file_dict", valid_type=Dict)
         spec.input("frag_params", valid_type=Dict)
-        spec.input("prev_smi", valid_type=List, default=List([]), required=False)
+        spec.input(
+            "prev_smi", valid_type=List, default=lambda: List([]), required=False
+        )
         spec.input("frag_group", valid_type=Str, required=False)
         spec.input("frame_group", valid_type=Str, required=False)
         # spec.input("g16_code", valid_type=Code)
-        spec.input("procs", valid_type=Int, default=Int(8))
+        spec.input("procs", valid_type=Int, default=lambda: Int(8))
         # spec.input('aim_code',valid_type=Code)
         # spec.input('aim_params',valid_type=AimqbParameters)
         # spec.input("g16_opt_params", valid_type=Dict)
         # spec.input('g16_sp_params',valid_type=Dict)
         spec.outline(cls.generate_fragments)
 
     def generate_fragments(self):
```

### Comparing `aiida_aimall-0.6.11/pyproject.toml` & `aiida_aimall-0.6.12/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_aimall-0.6.11/PKG-INFO` & `aiida_aimall-0.6.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-aimall
-Version: 0.6.11
+Version: 0.6.12
 Summary: A plugin to interface AIMAll with AiiDA
 Keywords: aiida,plugin
 Author-email: Kevin Lefrancois-Gagnon <kgagnon@lakeheadu.ca>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

