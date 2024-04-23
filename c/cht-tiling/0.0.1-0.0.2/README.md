# Comparing `tmp/cht_tiling-0.0.1.tar.gz` & `tmp/cht_tiling-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cht_tiling-0.0.1.tar", last modified: Mon Jan 29 19:15:54 2024, max compression
+gzip compressed data, was "cht_tiling-0.0.2.tar", last modified: Tue Apr 23 13:18:15 2024, max compression
```

## Comparing `cht_tiling-0.0.1.tar` & `cht_tiling-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-29 19:15:54.955582 cht_tiling-0.0.1/
--rw-rw-rw-   0        0        0     1081 2023-12-06 13:52:03.000000 cht_tiling-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      697 2024-01-29 19:15:54.955582 cht_tiling-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-12-06 13:52:03.000000 cht_tiling-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-29 19:15:54.941058 cht_tiling-0.0.1/cht_tiling/
--rw-rw-rw-   0        0        0      115 2023-12-06 13:52:03.000000 cht_tiling-0.0.1/cht_tiling/__init__.py
--rw-rw-rw-   0        0        0     2813 2023-12-06 13:52:03.000000 cht_tiling-0.0.1/cht_tiling/fileops.py
--rw-rw-rw-   0        0        0    44740 2024-01-27 16:45:58.000000 cht_tiling-0.0.1/cht_tiling/tiling.py
-drwxrwxrwx   0        0        0        0 2024-01-29 19:15:54.955582 cht_tiling-0.0.1/cht_tiling.egg-info/
--rw-rw-rw-   0        0        0      697 2024-01-29 19:15:54.000000 cht_tiling-0.0.1/cht_tiling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-01-29 19:15:54.000000 cht_tiling-0.0.1/cht_tiling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-29 19:15:54.000000 cht_tiling-0.0.1/cht_tiling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-01-29 19:15:54.000000 cht_tiling-0.0.1/cht_tiling.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-29 19:15:54.000000 cht_tiling-0.0.1/cht_tiling.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-12-06 13:52:51.000000 cht_tiling-0.0.1/cht_tiling.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1015 2024-01-29 19:15:39.000000 cht_tiling-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-29 19:15:54.955582 cht_tiling-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-29 19:15:54.955582 cht_tiling-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-12-06 13:52:03.000000 cht_tiling-0.0.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:18:15.031573 cht_tiling-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-23 13:17:49.000000 cht_tiling-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-23 13:18:15.031573 cht_tiling-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 13:17:49.000000 cht_tiling-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:18:15.027573 cht_tiling-0.0.2/cht_tiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-23 13:17:49.000000 cht_tiling-0.0.2/cht_tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-23 13:17:49.000000 cht_tiling-0.0.2/cht_tiling/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45838 2024-04-23 13:17:49.000000 cht_tiling-0.0.2/cht_tiling/tiling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:18:15.027573 cht_tiling-0.0.2/cht_tiling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-23 13:18:15.000000 cht_tiling-0.0.2/cht_tiling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-23 13:18:15.000000 cht_tiling-0.0.2/cht_tiling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:18:15.000000 cht_tiling-0.0.2/cht_tiling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 13:18:15.000000 cht_tiling-0.0.2/cht_tiling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 13:18:15.000000 cht_tiling-0.0.2/cht_tiling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:17:59.000000 cht_tiling-0.0.2/cht_tiling.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-23 13:17:49.000000 cht_tiling-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:18:15.031573 cht_tiling-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:18:15.027573 cht_tiling-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:17:49.000000 cht_tiling-0.0.2/tests/test.py
```

### Comparing `cht_tiling-0.0.1/LICENSE` & `cht_tiling-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) Deltares
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) Deltares
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `cht_tiling-0.0.1/PKG-INFO` & `cht_tiling-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
-Name: cht_tiling
-Version: 0.0.1
-Summary: CHT Tiling is a package to create and use slippy tiles (xyz)
-Author-email: Maarten van Ormondt <maarten.vanormondt@deltares.nl>
-License: MIT
-Project-URL: Source, https://github.com/Deltares-research/cht_tiling
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: pyproj
-Requires-Dist: pillow
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-
-# Coastal Hazards Toolkit - Tiling
+Metadata-Version: 2.1
+Name: cht_tiling
+Version: 0.0.2
+Summary: CHT Tiling is a package to create and use slippy tiles (xyz)
+Author-email: Maarten van Ormondt <maarten.vanormondt@deltares.nl>
+License: MIT
+Project-URL: Source, https://github.com/Deltares-research/cht_tiling
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pyproj
+Requires-Dist: pillow
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+
+# Coastal Hazards Toolkit - Tiling
```

### Comparing `cht_tiling-0.0.1/cht_tiling.egg-info/PKG-INFO` & `cht_tiling-0.0.2/cht_tiling.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1
-Name: cht_tiling
-Version: 0.0.1
-Summary: CHT Tiling is a package to create and use slippy tiles (xyz)
-Author-email: Maarten van Ormondt <maarten.vanormondt@deltares.nl>
-License: MIT
-Project-URL: Source, https://github.com/Deltares-research/cht_tiling
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Hydrology
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: pyproj
-Requires-Dist: pillow
-Provides-Extra: tests
-Requires-Dist: pytest; extra == "tests"
-
-# Coastal Hazards Toolkit - Tiling
+Metadata-Version: 2.1
+Name: cht_tiling
+Version: 0.0.2
+Summary: CHT Tiling is a package to create and use slippy tiles (xyz)
+Author-email: Maarten van Ormondt <maarten.vanormondt@deltares.nl>
+License: MIT
+Project-URL: Source, https://github.com/Deltares-research/cht_tiling
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Hydrology
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: pyproj
+Requires-Dist: pillow
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+
+# Coastal Hazards Toolkit - Tiling
```

### Comparing `cht_tiling-0.0.1/pyproject.toml` & `cht_tiling-0.0.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-[build-system]
-requires = ["setuptools>=61"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "cht_tiling"
-description = "CHT Tiling is a package to create and use slippy tiles (xyz)"
-readme = "README.md"
-authors = [
-    { name = "Maarten van Ormondt", email = "maarten.vanormondt@deltares.nl"}
-]
-license = { text = "MIT" }
-classifiers = [
-    "Intended Audience :: Science/Research",
-    "Topic :: Scientific/Engineering :: Hydrology",
-]
-requires-python = ">=3.10"
-dependencies = ["numpy", "scipy","matplotlib","pyproj","pillow"]
-dynamic = ["version"]
-
-[project.optional-dependencies]
-tests = ["pytest"]
-
-[tool.setuptools]
-zip-safe = true
-
-[tool.setuptools.dynamic]
-version = { attr = "cht_tiling.__version__" }
-
-[tool.setuptools.packages.find]
-include = ["cht_tiling"]
-
-[tool.setuptools.package-data]
-"cht_tiling" = ["py.typed"]
-
-# TODO
-[project.urls]
-Source = "https://github.com/Deltares-research/cht_tiling"
-#Documentation = "https://deltares.github.io/Ribasim"
+[build-system]
+requires = ["setuptools>=61"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "cht_tiling"
+description = "CHT Tiling is a package to create and use slippy tiles (xyz)"
+readme = "README.md"
+authors = [
+    { name = "Maarten van Ormondt", email = "maarten.vanormondt@deltares.nl"}
+]
+license = { text = "MIT" }
+classifiers = [
+    "Intended Audience :: Science/Research",
+    "Topic :: Scientific/Engineering :: Hydrology",
+]
+requires-python = ">=3.10"
+dependencies = ["numpy", "scipy","matplotlib","pyproj","pillow"]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+tests = ["pytest"]
+
+[tool.setuptools]
+zip-safe = true
+
+[tool.setuptools.dynamic]
+version = { attr = "cht_tiling.__version__" }
+
+[tool.setuptools.packages.find]
+include = ["cht_tiling"]
+
+[tool.setuptools.package-data]
+"cht_tiling" = ["py.typed"]
+
+# TODO
+[project.urls]
+Source = "https://github.com/Deltares-research/cht_tiling"
+#Documentation = "https://deltares.github.io/Ribasim"
```

