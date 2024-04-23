# Comparing `tmp/the_utils-0.3.5.tar.gz` & `tmp/the_utils-0.3.6.tar.gz`

## Comparing `the_utils-0.3.5.tar` & `the_utils-0.3.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.3.5/.editorconfig
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 the_utils-0.3.5/.gitmodules
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 the_utils-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 the_utils-0.3.5/.pylintrc
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 the_utils-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 the_utils-0.3.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.3.5/requirements-dev.txt
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 the_utils-0.3.5/requirements.txt
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 the_utils-0.3.5/.ci/cuda.sh
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 the_utils-0.3.5/.ci/docs.sh
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 the_utils-0.3.5/.ci/install-cpu.sh
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 the_utils-0.3.5/.ci/install-dev.sh
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 the_utils-0.3.5/.ci/install.sh
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 the_utils-0.3.5/.ci/nb.sh
--rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 the_utils-0.3.5/.ci/configs/nb.py
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 the_utils-0.3.5/.github/workflows/release.yml
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 the_utils-0.3.5/.vscode/extensions.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 the_utils-0.3.5/demos/demo.ipynb
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/Makefile
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/conf.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/_static/css/table.css
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/rst/the_utils.bot.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/rst/the_utils.common.rst
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/rst/the_utils.evaluation.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/rst/the_utils.file.rst
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/rst/the_utils.plt.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/rst/the_utils.save_load.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/rst/the_utils.setting.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/tpls/module.rst_t
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/tpls/package.rst_t
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 the_utils-0.3.5/docs/tpls/toc.rst_t
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/__init__.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/bot.py
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/common.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/file.py
--rw-r--r--   0        0        0    10058 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/plt.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/save_load.py
--rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/setting.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/evaluation/__init__.py
--rw-r--r--   0        0        0    18771 2020-02-02 00:00:00.000000 the_utils-0.3.5/the_utils/evaluation/unsupervised_graph_learning.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 the_utils-0.3.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 the_utils-0.3.5/LICENSE
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 the_utils-0.3.5/README.md
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 the_utils-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 the_utils-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.3.6/.editorconfig
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 the_utils-0.3.6/.gitmodules
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 the_utils-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 the_utils-0.3.6/.pylintrc
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 the_utils-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 the_utils-0.3.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 the_utils-0.3.6/requirements-dev.txt
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 the_utils-0.3.6/requirements.txt
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 the_utils-0.3.6/.ci/cuda.sh
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 the_utils-0.3.6/.ci/docs.sh
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 the_utils-0.3.6/.ci/install-cpu.sh
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 the_utils-0.3.6/.ci/install-dev.sh
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 the_utils-0.3.6/.ci/install.sh
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 the_utils-0.3.6/.ci/nb.sh
+-rw-r--r--   0        0        0    56106 2020-02-02 00:00:00.000000 the_utils-0.3.6/.ci/configs/nb.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 the_utils-0.3.6/.github/workflows/release.yml
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 the_utils-0.3.6/.vscode/extensions.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 the_utils-0.3.6/demos/demo.ipynb
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/Makefile
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/conf.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/_static/css/table.css
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/rst/the_utils.bot.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/rst/the_utils.common.rst
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/rst/the_utils.evaluation.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/rst/the_utils.file.rst
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/rst/the_utils.plt.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/rst/the_utils.save_load.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/rst/the_utils.setting.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/tpls/module.rst_t
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/tpls/package.rst_t
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 the_utils-0.3.6/docs/tpls/toc.rst_t
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 the_utils-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/__init__.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/bot.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/common.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/file.py
+-rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/plt.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/save_load.py
+-rw-r--r--   0        0        0     3017 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/setting.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/evaluation/__init__.py
+-rw-r--r--   0        0        0    18771 2020-02-02 00:00:00.000000 the_utils-0.3.6/the_utils/evaluation/unsupervised_graph_learning.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 the_utils-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 the_utils-0.3.6/LICENSE
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 the_utils-0.3.6/README.md
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 the_utils-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 the_utils-0.3.6/PKG-INFO
```

### Comparing `the_utils-0.3.5/.pre-commit-config.yaml` & `the_utils-0.3.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/.pylintrc` & `the_utils-0.3.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/CHANGELOG.md` & `the_utils-0.3.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.3.6 (2024-04-23)
+
+### Fix
+
+* fix(plt): types not defined ([`4850e72`](https://github.com/galogm/the_utils/commit/4850e728cb57d617b15fa7069d47f3b5a949737e))
+
+
 ## v0.3.5 (2024-03-07)
 
 ### Fix
 
 * fix: no head for csv2file when is_dict_list=True ([`6c6c26c`](https://github.com/galogm/the_utils/commit/6c6c26cd747b6233e18c3755d128f2c65e89894f))
```

### Comparing `the_utils-0.3.5/.ci/cuda.sh` & `the_utils-0.3.6/.ci/cuda.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/.ci/install-cpu.sh` & `the_utils-0.3.6/.ci/install-cpu.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/.ci/install-dev.sh` & `the_utils-0.3.6/.ci/install-dev.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/.ci/install.sh` & `the_utils-0.3.6/.ci/install.sh`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/.ci/configs/nb.py` & `the_utils-0.3.6/.ci/configs/nb.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/.github/workflows/release.yml` & `the_utils-0.3.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/demos/demo.ipynb` & `the_utils-0.3.6/demos/demo.ipynb`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/docs/Makefile` & `the_utils-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/docs/conf.py` & `the_utils-0.3.6/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'the_utils'
 copyright = '2023, galo.gm'
 author = 'galo.gm'
 
 # The full version, including alpha/beta/rc tags
-release = '0.3.5'
+release = '0.3.6'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `the_utils-0.3.5/docs/index.rst` & `the_utils-0.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/docs/make.bat` & `the_utils-0.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/docs/tpls/package.rst_t` & `the_utils-0.3.6/docs/tpls/package.rst_t`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/the_utils/bot.py` & `the_utils-0.3.6/the_utils/bot.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/the_utils/common.py` & `the_utils-0.3.6/the_utils/common.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/the_utils/file.py` & `the_utils-0.3.6/the_utils/file.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/the_utils/plt.py` & `the_utils-0.3.6/the_utils/plt.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                     "width": bar_width,
                 })
             else:
                 optional_args.append({})
     elif isinstance(types, str):
         for _ in range(len(ys)):
             funcs.append(charts(types, ax))
-            if t == "bar":
+            if types == "bar":
                 optional_args.append({
                     "width": bar_width,
                 })
             else:
                 optional_args.append({})
     else:
         raise ValueError(f"The arg 'types:'{types} has values not supported.")
```

### Comparing `the_utils-0.3.5/the_utils/save_load.py` & `the_utils-0.3.6/the_utils/save_load.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/the_utils/setting.py` & `the_utils-0.3.6/the_utils/setting.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/the_utils/evaluation/unsupervised_graph_learning.py` & `the_utils-0.3.6/the_utils/evaluation/unsupervised_graph_learning.py`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/.gitignore` & `the_utils-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/LICENSE` & `the_utils-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/README.md` & `the_utils-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `the_utils-0.3.5/pyproject.toml` & `the_utils-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "the_utils"
-version = "0.3.5"
+version = "0.3.6"
 authors = [{ name = "galo.gm", email = "galo.gm.work@gmail.com" }]
 keywords = [""]
 description = ""
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `the_utils-0.3.5/PKG-INFO` & `the_utils-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: the_utils
-Version: 0.3.5
+Version: 0.3.6
 Project-URL: Homepage, https://github.com/galogm/the_utils
 Project-URL: Bug Tracker, https://github.com/galogm/the_utils/issues
 Author-email: "galo.gm" <galo.gm.work@gmail.com>
 License: MIT License
         
         Copyright (c) 2023-present Author
```

