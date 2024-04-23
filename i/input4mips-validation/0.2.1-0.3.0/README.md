# Comparing `tmp/input4mips_validation-0.2.1.tar.gz` & `tmp/input4mips_validation-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "input4mips_validation-0.2.1.tar", max compression
+gzip compressed data, was "input4mips_validation-0.3.0.tar", max compression
```

## Comparing `input4mips_validation-0.2.1.tar` & `input4mips_validation-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,26 @@
--rw-r--r--   0        0        0     1685 2024-02-15 16:37:41.551193 input4mips_validation-0.2.1/LICENCE
--rw-r--r--   0        0        0     3810 2024-02-15 16:37:41.551193 input4mips_validation-0.2.1/README.md
--rw-r--r--   0        0        0     5611 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      171 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/__init__.py
--rw-r--r--   0        0        0     3795 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/attrs_helpers.py
--rw-r--r--   0        0        0      282 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/cli/__init__.py
--rw-r--r--   0        0        0     1133 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/cli/root.py
--rw-r--r--   0        0        0      908 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/cli/validate_file.py
--rw-r--r--   0        0        0       39 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/__init__.py
--rw-r--r--   0        0        0     1565 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/constants.py
--rw-r--r--   0        0        0      613 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/file_id.py
--rw-r--r--   0        0        0     2830 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/inference/__init__.py
--rw-r--r--   0        0        0     4384 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/__init__.py
--rw-r--r--   0        0        0     6790 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py
--rw-r--r--   0        0        0      740 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py
--rw-r--r--   0        0        0     2257 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py
--rw-r--r--   0        0        0      779 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/email.py
--rw-r--r--   0        0        0      634 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/uuid.py
--rw-r--r--   0        0        0    10284 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/dataset.py
--rw-r--r--   0        0        0      674 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/exceptions.py
--rw-r--r--   0        0        0      158 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/main.py
--rw-r--r--   0        0        0     3403 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/metadata.py
--rw-r--r--   0        0        0        0 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/py.typed
--rw-r--r--   0        0        0     1429 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/testing.py
--rw-r--r--   0        0        0     5886 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/time.py
--rw-r--r--   0        0        0     1691 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/validation/__init__.py
--rw-r--r--   0        0        0     3094 2024-02-15 16:37:41.555193 input4mips_validation-0.2.1/src/input4mips_validation/xarray_helpers.py
--rw-r--r--   0        0        0     4932 1970-01-01 00:00:00.000000 input4mips_validation-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1685 2024-04-23 10:58:49.919403 input4mips_validation-0.3.0/LICENCE
+-rw-r--r--   0        0        0     3810 2024-04-23 10:58:49.919403 input4mips_validation-0.3.0/README.md
+-rw-r--r--   0        0        0     5606 2024-04-23 10:58:49.919403 input4mips_validation-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      171 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/__init__.py
+-rw-r--r--   0        0        0     3795 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/attrs_helpers.py
+-rw-r--r--   0        0        0     1164 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/cli/__init__.py
+-rw-r--r--   0        0        0     1031 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/cli/cli_logging.py
+-rw-r--r--   0        0        0       39 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/__init__.py
+-rw-r--r--   0        0        0     1793 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/constants.py
+-rw-r--r--   0        0        0      613 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/file_id.py
+-rw-r--r--   0        0        0     3688 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/inference/__init__.py
+-rw-r--r--   0        0        0     4384 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/__init__.py
+-rw-r--r--   0        0        0     6986 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py
+-rw-r--r--   0        0        0      740 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py
+-rw-r--r--   0        0        0     2257 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py
+-rw-r--r--   0        0        0      779 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/email.py
+-rw-r--r--   0        0        0      634 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/uuid.py
+-rw-r--r--   0        0        0    10284 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/dataset.py
+-rw-r--r--   0        0        0      674 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/exceptions.py
+-rw-r--r--   0        0        0     3413 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/metadata.py
+-rw-r--r--   0        0        0        0 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/py.typed
+-rw-r--r--   0        0        0     1429 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/testing.py
+-rw-r--r--   0        0        0     5886 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/time.py
+-rw-r--r--   0        0        0     1691 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/validation/__init__.py
+-rw-r--r--   0        0        0     4207 2024-04-23 10:58:49.923403 input4mips_validation-0.3.0/src/input4mips_validation/xarray_helpers.py
+-rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 input4mips_validation-0.3.0/PKG-INFO
```

### Comparing `input4mips_validation-0.2.1/LICENCE` & `input4mips_validation-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/README.md` & `input4mips_validation-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/pyproject.toml` & `input4mips_validation-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "input4mips-validation"
-version = "0.2.1"
+version = "0.3.0"
 description = "Validation of input4MIPs data (checking file formats, metadata etc.)."
 authors = ["Zebedee Nicholls <zebedee.nicholls@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "input4mips_validation", from = "src"}]
 license = "BSD-3-Clause"
 include = ["LICENCE"]  # poetry uses US English so assumes it will be spelt LICENSE
 
 [tool.poetry.dependencies]
 python = "^3.9"
 matplotlib = { version = ">=3.0", optional = true }
 notebook = { version = ">=6.0", optional = true }
-click = ">=8.0"
 loguru = ">=0.7"
 cf-xarray = ">=0.8"
 xarray = ">=2022.0"
 pint-xarray = ">=0.3"
 numpy = ">=1.23"
 cftime = ">=1.6"
 typing-extensions = ">=4.0"
 pooch = ">=1.0"
 # Pooch is a dependency of cf-xarray but not included in cf-xarray's dependencies.
 # TODO: PR into cf-xarray
 netcdf4 = ">=1.0"
 attrs = ">=22.0"
+typer = "^0.9.0"
 
 [tool.poetry.extras]
 plots = ["matplotlib"]
 notebooks = ["notebook"]
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
@@ -49,15 +49,15 @@
 ruff = "^0.1.8"
 pre-commit = "^3.3.1"
 towncrier = "^23.6.0"
 liccheck = "^0.9.1"
 types-requests = "^2.31.0.20240125"
 
 [tool.poetry.scripts]
-input4mips-validation = "input4mips_validation.main:root_cli"
+input4mips-validation = "input4mips_validation.cli:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/attrs_helpers.py` & `input4mips_validation-0.3.0/src/input4mips_validation/attrs_helpers.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/cli/root.py` & `input4mips_validation-0.3.0/src/input4mips_validation/cli/cli_logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 Root for the command-line interface
 """
 from __future__ import annotations
 
 import sys
 from typing import Any
 
-import click
+import typer
 from loguru import logger
 
+app = typer.Typer()
+
 DEFAULT_LOGGING_CONFIG = dict(
     handlers=[
         dict(
             sink=sys.stderr,
             colorize=True,
             format=" - ".join(
                 [
@@ -39,15 +41,7 @@
         :const:`DEFAULT_LOGGING_CONFIG` is used.
     """
     if config is None:
         config = DEFAULT_LOGGING_CONFIG
 
     logger.configure(**config)
     logger.enable("fgen")
-
-
-@click.group()
-def root_cli() -> None:
-    """
-    Entrypoint for the command-line interface
-    """
-    setup_logging()
```

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/constants.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 # e.g. CVs website, that defines this map
 VARIABLE_DATASET_MAP = {
     "tos": "SSTsAndSeaIce",
     "siconc": "SSTsAndSeaIce",
     "sftof": "SSTsAndSeaIce",
     "areacello": "SSTsAndSeaIce",
     "mole_fraction_of_carbon_dioxide_in_air": "GHGConcentrations",
+    "mole_fraction_of_methane_in_air": "GHGConcentrations",
+    "mole_fraction_of_nitrous_oxide_in_air": "GHGConcentrations",
 }
 
 # TODO: remove this hard-coding based on some logic/map held elsewhere,
 # e.g. CVs website, that defines this map
 VARIABLE_REALM_MAP = {
     "tos": "ocean",
     "siconc": "seaIce",
     "sftof": "ocean",
     "areacello": "ocean",
     "mole_fraction_of_carbon_dioxide_in_air": "atmos",
+    "mole_fraction_of_methane_in_air": "atmos",
+    "mole_fraction_of_nitrous_oxide_in_air": "atmos",
 }
 
 CREATION_DATE_REGEX: re.Pattern[str] = re.compile(
     r"^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}Z$"
 )
 """
 Regular expression that checks the creation date is formatted correctly
```

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/file_id.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/file_id.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/__init__.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,26 @@
 
     Returns
     -------
         Raw JSON
     """
     # TODO: remove this huge hack once we work out where this is meant to come from
     if key == "institution_id":
-        return ("PCMDI",)
+        return ("PCMDI", "CR")
 
     # TODO: remove this huge hack once we work out where this is meant to come from
     if key == "grid_label":
-        return ("placeholder",)
+        return ("placeholder", "gr", "gr1")
+
+    if key == "source_id":
+        return {
+            "source_id": {
+                "CR-CMIP-0-2-0": "To discuss further with Paul how this should be"
+            }
+        }
 
     url_template = "https://raw.githubusercontent.com/PCMDI/input4MIPs_CVs/main/input4MIPs_{key}.json"
     url_to_hit = url_template.format(key=key)
     res = requests.get(url_to_hit, timeout=timeout)
     res.raise_for_status()
 
     return res.json()
```

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/email.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/email.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/controlled_vocabularies/validators/uuid.py` & `input4mips_validation-0.3.0/src/input4mips_validation/controlled_vocabularies/validators/uuid.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/dataset.py` & `input4mips_validation-0.3.0/src/input4mips_validation/dataset.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/exceptions.py` & `input4mips_validation-0.3.0/src/input4mips_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/metadata.py` & `input4mips_validation-0.3.0/src/input4mips_validation/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,19 +52,19 @@
         validator=make_attrs_validator_compatible_attribute_value_input(
             assert_attribute_being_set_matches_controlled_vocabulary
         )
     )
     """Institution ID for the dataset"""
 
     source_id: str = field(
-        validator=make_attrs_validator_compatible_attribute_value_input(
-            assert_attribute_being_set_matches_controlled_vocabulary
-            # TODO: check if there are actually more restrictions on this e.g.
-            # consistency with institution_id
-        )
+        # validator=make_attrs_validator_compatible_attribute_value_input(
+        #     assert_attribute_being_set_matches_controlled_vocabulary
+        #     # TODO: check if there are actually more restrictions on this e.g.
+        #     # consistency with institution_id
+        # )
     )
     """Source ID for the dataset"""
 
     grid_label: str = field(
         validator=make_attrs_validator_compatible_attribute_value_input(
             assert_attribute_being_set_matches_controlled_vocabulary
             # TODO: check if there are actually more restrictions on this e.g.
```

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/testing.py` & `input4mips_validation-0.3.0/src/input4mips_validation/testing.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/time.py` & `input4mips_validation-0.3.0/src/input4mips_validation/time.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/validation/__init__.py` & `input4mips_validation-0.3.0/src/input4mips_validation/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.2.1/src/input4mips_validation/xarray_helpers.py` & `input4mips_validation-0.3.0/src/input4mips_validation/xarray_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     return variables[0]
 
 
 def add_time_bounds(
     ds: xr.Dataset,
     monthly_time_bounds: bool = False,
+    yearly_time_bounds: bool = False,
     output_dim: str = "bounds",
 ) -> xr.Dataset:
     """
     Add time bounds to a dataset
 
     This should be pushed upstream to cf-xarray at some point probably
 
@@ -58,18 +59,28 @@
         Dataset to which to add time bounds
 
     monthly_time_bounds
         Are we looking at monthly data i.e. should the time bounds run from
         the start of one month to the next (which isn't regular spacing but is
         most often what is desired/required)
 
+    yearly_time_bounds
+        Are we looking at yearly data i.e. should the time bounds run from
+        the start of one year to the next (which isn't regular spacing but is
+        sometimes what is desired/required)
+
     Returns
     -------
         Dataset with time bounds
 
+    Raises
+    ------
+    ValueError
+        Both ``monthly_time_bounds`` and ``yearly_time_bounds`` are ``True``.
+
     Notes
     -----
     There is no copy here, ``ds`` is modified in place (call
     :meth:`xarray.Dataset.copy` before passing if you don't
     want this).
     """
     # based on cf-xarray's implementation, to be pushed back upstream at some
@@ -81,27 +92,48 @@
 
     if bname in ds.variables:
         raise ValueError(  # noqa: TRY003
             f"Bounds variable name {bname!r} will conflict!"
         )
 
     if monthly_time_bounds:
+        if yearly_time_bounds:
+            msg = (
+                "Only one of monthly_time_bounds and yearly_time_bounds should be true"
+            )
+            raise ValueError(msg)
+
         ds_ym = split_time_to_year_month(ds, time_axis=variable)
 
         # This may need to be refactored to allow the cftime_converter to be
         # injected, same idea as `convert_to_time`
         bounds = xr.DataArray(
             [
                 [cftime.datetime(y, m, 1), get_start_of_next_month(y, m)]
                 for y, m in zip(ds_ym.year, ds_ym.month)
             ],
             dims=(variable, "bounds"),
             coords={variable: ds[variable], "bounds": [0, 1]},
         ).transpose(..., "bounds")
+
+    elif yearly_time_bounds:
+        # Hacks hacks hacks :)
+        # This may need to be refactored to allow the cftime_converter to be
+        # injected, same idea as `convert_to_time`
+        bounds = xr.DataArray(
+            [
+                [cftime.datetime(y, 1, 1), cftime.datetime(y + 1, 1, 1)]
+                for y in ds["time"].dt.year
+            ],
+            dims=(variable, "bounds"),
+            coords={variable: ds[variable], "bounds": [0, 1]},
+        ).transpose(..., "bounds")
+
     else:
+        # TODO: fix this, quite annoying now.
         # This will require some thinking because `ds.cf.add_bounds(dim)`
         # doesn't work with cftime.datetime objects. Probably needs an issue upstream
         # and then a monkey patch or custom function here as a workaround.
         raise NotImplementedError(monthly_time_bounds)
 
     ds.coords[bname] = bounds
     ds[variable].attrs["bounds"] = bname
```

### Comparing `input4mips_validation-0.2.1/PKG-INFO` & `input4mips_validation-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: input4mips-validation
-Version: 0.2.1
+Version: 0.3.0
 Summary: Validation of input4MIPs data (checking file formats, metadata etc.).
 License: BSD-3-Clause
 Author: Zebedee Nicholls
 Author-email: zebedee.nicholls@climate-resource.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: notebooks
 Provides-Extra: plots
 Requires-Dist: attrs (>=22.0)
 Requires-Dist: cf-xarray (>=0.8)
 Requires-Dist: cftime (>=1.6)
-Requires-Dist: click (>=8.0)
 Requires-Dist: loguru (>=0.7)
 Requires-Dist: matplotlib (>=3.0) ; extra == "plots"
 Requires-Dist: netcdf4 (>=1.0)
 Requires-Dist: notebook (>=6.0) ; extra == "notebooks"
 Requires-Dist: numpy (>=1.23)
 Requires-Dist: pint-xarray (>=0.3)
 Requires-Dist: pooch (>=1.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.0)
 Requires-Dist: xarray (>=2022.0)
 Description-Content-Type: text/markdown
 
 # Input4MIPs-validation
 
 <!---
```

