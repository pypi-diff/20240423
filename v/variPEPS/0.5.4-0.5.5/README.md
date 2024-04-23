# Comparing `tmp/varipeps-0.5.4.tar.gz` & `tmp/varipeps-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varipeps-0.5.4.tar", max compression
+gzip compressed data, was "varipeps-0.5.5.tar", max compression
```

## Comparing `varipeps-0.5.4.tar` & `varipeps-0.5.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35103 2024-04-22 09:32:46.130676 varipeps-0.5.4/LICENSE
--rw-r--r--   0        0        0     3116 2024-04-22 09:32:46.130676 varipeps-0.5.4/README.md
--rw-r--r--   0        0        0     1157 2024-04-22 09:32:46.142676 varipeps-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      680 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/__init__.py
--rw-r--r--   0        0        0      741 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/__version__.py
--rw-r--r--   0        0        0    11223 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/config.py
--rw-r--r--   0        0        0      100 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/contractions/__init__.py
--rw-r--r--   0        0        0     5553 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/contractions/apply.py
--rw-r--r--   0        0        0    33811 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/contractions/definitions.py
--rw-r--r--   0        0        0      214 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/__init__.py
--rw-r--r--   0        0        0    24093 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/absorption.py
--rw-r--r--   0        0        0    24758 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/projectors.py
--rw-r--r--   0        0        0    22359 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/ctmrg/routine.py
--rw-r--r--   0        0        0      260 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/__init__.py
--rw-r--r--   0        0        0     1956 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/model.py
--rw-r--r--   0        0        0     5609 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/one_site.py
--rw-r--r--   0        0        0     3352 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/spiral_helpers.py
--rw-r--r--   0        0        0    17657 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/three_sites.py
--rw-r--r--   0        0        0    19770 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/expectation/two_sites.py
--rw-r--r--   0        0        0     1184 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/global_state.py
--rw-r--r--   0        0        0      191 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/__init__.py
--rw-r--r--   0        0        0    44983 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/florett_pentagon.py
--rw-r--r--   0        0        0    22817 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/honeycomb.py
--rw-r--r--   0        0        0    39648 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/kagome.py
--rw-r--r--   0        0        0    46761 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/maple_leaf.py
--rw-r--r--   0        0        0     1288 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/model.py
--rw-r--r--   0        0        0    59271 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/square_kagome.py
--rw-r--r--   0        0        0    19197 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/mapping/triangular.py
--rw-r--r--   0        0        0      152 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/__init__.py
--rw-r--r--   0        0        0     6434 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/basinhopping.py
--rw-r--r--   0        0        0    10290 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/inner_function.py
--rw-r--r--   0        0        0    23104 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/line_search.py
--rw-r--r--   0        0        0    24773 2024-04-22 09:32:46.142676 varipeps-0.5.4/varipeps/optimization/optimizer.py
--rw-r--r--   0        0        0      113 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/peps/__init__.py
--rw-r--r--   0        0        0    35787 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/peps/tensor.py
--rw-r--r--   0        0        0    41065 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/peps/unitcell.py
--rw-r--r--   0        0        0     1086 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/typing.py
--rw-r--r--   0        0        0      119 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/__init__.py
--rw-r--r--   0        0        0     1285 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/debug_print.py
--rw-r--r--   0        0        0      739 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/func_cache.py
--rw-r--r--   0        0        0     2438 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/periodic_indices.py
--rw-r--r--   0        0        0     1657 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/projector_dict.py
--rw-r--r--   0        0        0     5398 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/random.py
--rw-r--r--   0        0        0     3396 2024-04-22 09:32:46.146676 varipeps-0.5.4/varipeps/utils/svd.py
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 varipeps-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35103 2024-04-23 10:51:24.456170 varipeps-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3116 2024-04-23 10:51:24.456170 varipeps-0.5.5/README.md
+-rw-r--r--   0        0        0     1157 2024-04-23 10:51:24.468170 varipeps-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      680 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/__init__.py
+-rw-r--r--   0        0        0      741 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/__version__.py
+-rw-r--r--   0        0        0    11223 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/config.py
+-rw-r--r--   0        0        0      100 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/contractions/__init__.py
+-rw-r--r--   0        0        0     5553 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/contractions/apply.py
+-rw-r--r--   0        0        0    33811 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/contractions/definitions.py
+-rw-r--r--   0        0        0      214 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/__init__.py
+-rw-r--r--   0        0        0    24093 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/absorption.py
+-rw-r--r--   0        0        0    24758 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/projectors.py
+-rw-r--r--   0        0        0    22359 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/ctmrg/routine.py
+-rw-r--r--   0        0        0      260 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/__init__.py
+-rw-r--r--   0        0        0     1956 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/model.py
+-rw-r--r--   0        0        0     5609 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/one_site.py
+-rw-r--r--   0        0        0     3352 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/spiral_helpers.py
+-rw-r--r--   0        0        0    17657 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/three_sites.py
+-rw-r--r--   0        0        0    19770 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/expectation/two_sites.py
+-rw-r--r--   0        0        0     1184 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/global_state.py
+-rw-r--r--   0        0        0      191 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/__init__.py
+-rw-r--r--   0        0        0    44983 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/florett_pentagon.py
+-rw-r--r--   0        0        0    22817 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/honeycomb.py
+-rw-r--r--   0        0        0    39648 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/kagome.py
+-rw-r--r--   0        0        0    46761 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/maple_leaf.py
+-rw-r--r--   0        0        0     1288 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/model.py
+-rw-r--r--   0        0        0    59271 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/square_kagome.py
+-rw-r--r--   0        0        0    19197 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/mapping/triangular.py
+-rw-r--r--   0        0        0      152 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/__init__.py
+-rw-r--r--   0        0        0     6434 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/basinhopping.py
+-rw-r--r--   0        0        0    10290 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/inner_function.py
+-rw-r--r--   0        0        0    23104 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/line_search.py
+-rw-r--r--   0        0        0    24682 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/optimization/optimizer.py
+-rw-r--r--   0        0        0      113 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/peps/__init__.py
+-rw-r--r--   0        0        0    35787 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/peps/tensor.py
+-rw-r--r--   0        0        0    41065 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/peps/unitcell.py
+-rw-r--r--   0        0        0     1086 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/typing.py
+-rw-r--r--   0        0        0      119 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/__init__.py
+-rw-r--r--   0        0        0     1285 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/debug_print.py
+-rw-r--r--   0        0        0      739 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/func_cache.py
+-rw-r--r--   0        0        0     2438 2024-04-23 10:51:24.468170 varipeps-0.5.5/varipeps/utils/periodic_indices.py
+-rw-r--r--   0        0        0     1657 2024-04-23 10:51:24.472170 varipeps-0.5.5/varipeps/utils/projector_dict.py
+-rw-r--r--   0        0        0     5398 2024-04-23 10:51:24.472170 varipeps-0.5.5/varipeps/utils/random.py
+-rw-r--r--   0        0        0     3396 2024-04-23 10:51:24.472170 varipeps-0.5.5/varipeps/utils/svd.py
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 varipeps-0.5.5/PKG-INFO
```

### Comparing `varipeps-0.5.4/LICENSE` & `varipeps-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/README.md` & `varipeps-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/pyproject.toml` & `varipeps-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "variPEPS"
-version = "0.5.4"
+version = "0.5.5"
 description = "Versatile tensor network library for variational ground state simulations in two spatial dimensions"
 authors = ["Jan Naumann <j.naumann@fu-berlin.de>", "Philipp Schmoll <philipp.schmoll@fu-berlin.de>", "Frederik Wilde", "Finn Krein"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/variPEPS/variPEPS_Python"
 documentation = "https://varipeps.readthedocs.io/en/stable/"
 packages = [{include = "varipeps"}]
```

### Comparing `varipeps-0.5.4/varipeps/__init__.py` & `varipeps-0.5.5/varipeps/__init__.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/__version__.py` & `varipeps-0.5.5/varipeps/__version__.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/config.py` & `varipeps-0.5.5/varipeps/config.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/contractions/apply.py` & `varipeps-0.5.5/varipeps/contractions/apply.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/contractions/definitions.py` & `varipeps-0.5.5/varipeps/contractions/definitions.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/ctmrg/absorption.py` & `varipeps-0.5.5/varipeps/ctmrg/absorption.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/ctmrg/projectors.py` & `varipeps-0.5.5/varipeps/ctmrg/projectors.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/ctmrg/routine.py` & `varipeps-0.5.5/varipeps/ctmrg/routine.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/expectation/model.py` & `varipeps-0.5.5/varipeps/expectation/model.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/expectation/one_site.py` & `varipeps-0.5.5/varipeps/expectation/one_site.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/expectation/spiral_helpers.py` & `varipeps-0.5.5/varipeps/expectation/spiral_helpers.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/expectation/three_sites.py` & `varipeps-0.5.5/varipeps/expectation/three_sites.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/expectation/two_sites.py` & `varipeps-0.5.5/varipeps/expectation/two_sites.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/global_state.py` & `varipeps-0.5.5/varipeps/global_state.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/mapping/florett_pentagon.py` & `varipeps-0.5.5/varipeps/mapping/florett_pentagon.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/mapping/honeycomb.py` & `varipeps-0.5.5/varipeps/mapping/honeycomb.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/mapping/kagome.py` & `varipeps-0.5.5/varipeps/mapping/kagome.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/mapping/maple_leaf.py` & `varipeps-0.5.5/varipeps/mapping/maple_leaf.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/mapping/model.py` & `varipeps-0.5.5/varipeps/mapping/model.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/mapping/square_kagome.py` & `varipeps-0.5.5/varipeps/mapping/square_kagome.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/mapping/triangular.py` & `varipeps-0.5.5/varipeps/mapping/triangular.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/optimization/basinhopping.py` & `varipeps-0.5.5/varipeps/optimization/basinhopping.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/optimization/inner_function.py` & `varipeps-0.5.5/varipeps/optimization/inner_function.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/optimization/line_search.py` & `varipeps-0.5.5/varipeps/optimization/line_search.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/optimization/optimizer.py` & `varipeps-0.5.5/varipeps/optimization/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -574,26 +574,25 @@
                     "Max. trunc. err.": f"{max_trunc_error:0.8g}",
                 }
             )
             pbar.refresh()
 
             if count % varipeps_config.optimizer_autosave_step_count == 0:
                 auxiliary_data = {
-                    "max_trunc_error_list": tuple(
-                        max_trunc_error_list[k]
-                        for k in sorted(max_trunc_error_list.keys())
-                    ),
-                    "step_energies": tuple(
-                        step_energies[k] for k in sorted(step_energies.keys())
-                    ),
-                    "step_chi": tuple(step_chi[k] for k in sorted(step_chi.keys())),
-                    "step_conv": tuple(step_conv[k] for k in sorted(step_conv.keys())),
                     "best_run": best_run if best_run is not None else 0,
                 }
 
+                for k in sorted(max_trunc_error_list.keys()):
+                    auxiliary_data[f"max_trunc_error_list_{k:d}"] = (
+                        max_trunc_error_list[k]
+                    )
+                    auxiliary_data[f"step_energies_{k:d}"] = step_energies[k]
+                    auxiliary_data[f"step_chi_{k:d}"] = step_chi[k]
+                    auxiliary_data[f"step_conv_{k:d}"] = step_conv[k]
+
                 if spiral_indices is not None:
                     for spiral_i in spiral_indices:
                         auxiliary_data[f"spiral_vector_{spiral_i:d}"] = working_tensors[
                             spiral_i
                         ]
                 elif additional_input.get("spiral_vectors") is not None:
                     add_input_spiral = additional_input.get("spiral_vectors")
```

### Comparing `varipeps-0.5.4/varipeps/peps/tensor.py` & `varipeps-0.5.5/varipeps/peps/tensor.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/peps/unitcell.py` & `varipeps-0.5.5/varipeps/peps/unitcell.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/typing.py` & `varipeps-0.5.5/varipeps/typing.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/utils/debug_print.py` & `varipeps-0.5.5/varipeps/utils/debug_print.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/utils/func_cache.py` & `varipeps-0.5.5/varipeps/utils/func_cache.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/utils/periodic_indices.py` & `varipeps-0.5.5/varipeps/utils/periodic_indices.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/utils/projector_dict.py` & `varipeps-0.5.5/varipeps/utils/projector_dict.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/utils/random.py` & `varipeps-0.5.5/varipeps/utils/random.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/varipeps/utils/svd.py` & `varipeps-0.5.5/varipeps/utils/svd.py`

 * *Files identical despite different names*

### Comparing `varipeps-0.5.4/PKG-INFO` & `varipeps-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: variPEPS
-Version: 0.5.4
+Version: 0.5.5
 Summary: Versatile tensor network library for variational ground state simulations in two spatial dimensions
 Home-page: https://github.com/variPEPS/variPEPS_Python
 License: GPL-3.0-or-later
 Author: Jan Naumann
 Author-email: j.naumann@fu-berlin.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

