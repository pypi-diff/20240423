# Comparing `tmp/paraview_trame_components-0.5.0.tar.gz` & `tmp/paraview_trame_components-0.6.0.tar.gz`

## Comparing `paraview_trame_components-0.5.0.tar` & `paraview_trame_components-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/all.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/cone-with-slider.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/cone.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/multi-views.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/pipeline.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/state-loader-slider.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/state-loader.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/test-cols.py
--rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/examples/wavelet-contour-state.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/__init__.py
--rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/colors.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/core.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/palette.py
--rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/pipeline.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/utils.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/vcr.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/assets/__init__.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/layouts/__init__.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/layouts/col.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/layouts/factory.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/ptc/layouts/side.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/.gitignore
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/LICENSE
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/README.md
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 paraview_trame_components-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/all.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/cone-with-slider.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/cone.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/multi-views.py
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/pipeline.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/state-loader-slider.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/state-loader.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/test-cols.py
+-rw-r--r--   0        0        0     8663 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/examples/wavelet-contour-state.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/cli.py
+-rw-r--r--   0        0        0     4722 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/colors.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/core.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/palette.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/pipeline.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/utils.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/vcr.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/vuetify.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/assets/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/__init__.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/col.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/factory.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/ptc/layouts/side.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/.gitignore
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/README.md
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 paraview_trame_components-0.6.0/PKG-INFO
```

### Comparing `paraview_trame_components-0.5.0/examples/cone-with-slider.py` & `paraview_trame_components-0.6.0/examples/cone-with-slider.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/examples/multi-views.py` & `paraview_trame_components-0.6.0/examples/multi-views.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/examples/pipeline.py` & `paraview_trame_components-0.6.0/examples/pipeline.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/examples/state-loader-slider.py` & `paraview_trame_components-0.6.0/examples/state-loader-slider.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/examples/test-cols.py` & `paraview_trame_components-0.6.0/examples/test-cols.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/examples/wavelet-contour-state.py` & `paraview_trame_components-0.6.0/examples/wavelet-contour-state.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/colors.py` & `paraview_trame_components-0.6.0/ptc/colors.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/core.py` & `paraview_trame_components-0.6.0/ptc/core.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/palette.py` & `paraview_trame_components-0.6.0/ptc/palette.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/pipeline.py` & `paraview_trame_components-0.6.0/ptc/pipeline.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/utils.py` & `paraview_trame_components-0.6.0/ptc/utils.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/vcr.py` & `paraview_trame_components-0.6.0/ptc/vcr.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/layouts/col.py` & `paraview_trame_components-0.6.0/ptc/layouts/col.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/ptc/layouts/side.py` & `paraview_trame_components-0.6.0/ptc/layouts/side.py`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/LICENSE` & `paraview_trame_components-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/README.md` & `paraview_trame_components-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `paraview_trame_components-0.5.0/pyproject.toml` & `paraview_trame_components-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "paraview-trame-components"
-version = "0.5.0"
+version = "0.6.0"
 requires-python = ">= 3.10"
 dependencies = [
   "trame",
   "trame-vtk",
   "trame-vuetify",
   "trame-components",
 ]
```

### Comparing `paraview_trame_components-0.5.0/PKG-INFO` & `paraview_trame_components-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: paraview-trame-components
-Version: 0.5.0
+Version: 0.6.0
 Summary: Macro components for ParaView
 Author-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 Maintainer-email: Sebastien Jourdain <sebastien.jourdain@kitware.com>
 License: Copyright 2024 Kitware Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
         you may not use this file except in compliance with the License.
```

