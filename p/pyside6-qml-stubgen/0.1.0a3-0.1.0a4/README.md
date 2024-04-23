# Comparing `tmp/pyside6_qml_stubgen-0.1.0a3.tar.gz` & `tmp/pyside6_qml_stubgen-0.1.0a4.tar.gz`

## Comparing `pyside6_qml_stubgen-0.1.0a3.tar` & `pyside6_qml_stubgen-0.1.0a4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/conftest.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/requirements.txt
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/.github/workflows/test.yml
--rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/__init__.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/__main__.py
--rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/dirty_file_detection.py
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/pyside_patching.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/qmlregistrar_types.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/__init__.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/test_run.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/README
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/qmldir
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/qmltyperegistrations1-0.cpp
--rw-r--r--   0        0        0    15603 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/types1-0.json
--rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/types1-0.qmltypes
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced/qmldir
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced/types1-100.json
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced/types1-100.qmltypes
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced2/qmldir
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced2/types1-100.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced2/types1-100.qmltypes
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/sub/qmldir
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/sub/qmltyperegistrations2-1.cpp
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/sub/types2-1.json
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/reference/target/sub/types2-1.qmltypes
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/target/__init__.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/target/advanced.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/target/advanced2.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/target/clses.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/target/clses2.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/tests/target/submodule.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/.gitignore
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/LICENCE.md
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/README.md
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/conftest.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/requirements.txt
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/.github/workflows/test.yml
+-rw-r--r--   0        0        0    14283 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__init__.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__main__.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/dirty_file_detection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/py.typed
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/pyside_patching.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/qmlregistrar_types.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/__init__.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/test_run.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/README
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/qmldir
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/qmltyperegistrations1-0.cpp
+-rw-r--r--   0        0        0    15603 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.json
+-rw-r--r--   0        0        0     5097 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.qmltypes
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/qmldir
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.json
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.qmltypes
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/qmldir
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.qmltypes
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/qmldir
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/qmltyperegistrations2-1.cpp
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.json
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.qmltypes
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/advanced.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/advanced2.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/clses.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/clses2.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/tests/target/submodule.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/.gitignore
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/LICENCE.md
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/README.md
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 pyside6_qml_stubgen-0.1.0a4/PKG-INFO
```

### Comparing `pyside6_qml_stubgen-0.1.0a3/.github/workflows/test.yml` & `pyside6_qml_stubgen-0.1.0a4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/__init__.py` & `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__init__.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/__main__.py` & `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/__main__.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/dirty_file_detection.py` & `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/dirty_file_detection.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/pyside_patching.py` & `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/pyside_patching.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/pyside6_qml_stubgen/qmlregistrar_types.py` & `pyside6_qml_stubgen-0.1.0a4/pyside6_qml_stubgen/qmlregistrar_types.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/test_run.py` & `pyside6_qml_stubgen-0.1.0a4/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/qmltyperegistrations1-0.cpp` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/qmltyperegistrations1-0.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/types1-0.json` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/types1-0.qmltypes` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/types1-0.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/qmltyperegistrations1-100.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced/types1-100.json` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced/types1-100.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/qmltyperegistrations1-100.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced2/types1-100.json` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/advanced2/types1-100.qmltypes` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/advanced2/types1-100.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/sub/qmltyperegistrations2-1.cpp` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/qmltyperegistrations2-1.cpp`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/sub/types2-1.json` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.json`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/reference/target/sub/types2-1.qmltypes` & `pyside6_qml_stubgen-0.1.0a4/tests/reference/target/sub/types2-1.qmltypes`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/target/advanced.py` & `pyside6_qml_stubgen-0.1.0a4/tests/target/advanced.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/target/advanced2.py` & `pyside6_qml_stubgen-0.1.0a4/tests/target/advanced2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/target/clses.py` & `pyside6_qml_stubgen-0.1.0a4/tests/target/clses.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/tests/target/clses2.py` & `pyside6_qml_stubgen-0.1.0a4/tests/target/clses2.py`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/LICENCE.md` & `pyside6_qml_stubgen-0.1.0a4/LICENCE.md`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/README.md` & `pyside6_qml_stubgen-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/pyproject.toml` & `pyside6_qml_stubgen-0.1.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyside6_qml_stubgen-0.1.0a3/PKG-INFO` & `pyside6_qml_stubgen-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyside6-qml-stubgen
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Generate QML stub files (.qmltypes) from Python modules (which use PySide6)
 Project-URL: Homepage, https://github.com/matsjoyce/pyside6-qml-stubgen
 Project-URL: Repository, https://github.com/matsjoyce/pyside6-qml-stubgen.git
 Project-URL: Issues, https://github.com/matsjoyce/pyside6-qml-stubgen/issues
 Author: Matthew Joyce
 License-File: LICENCE.md
 Keywords: pyside6,qml,qt6,type checking
```

