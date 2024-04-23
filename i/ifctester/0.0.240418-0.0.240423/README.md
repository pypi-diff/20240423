# Comparing `tmp/ifctester-0.0.240418.tar.gz` & `tmp/ifctester-0.0.240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifctester-0.0.240418.tar", last modified: Thu Apr 18 01:14:03 2024, max compression
+gzip compressed data, was "ifctester-0.0.240423.tar", last modified: Tue Apr 23 09:49:55 2024, max compression
```

## Comparing `ifctester-0.0.240418.tar` & `ifctester-0.0.240423.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.941325 ifctester-0.0.240418/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-18 01:14:03.941325 ifctester-0.0.240418/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-18 01:14:00.000000 ifctester-0.0.240418/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.937325 ifctester-0.0.240418/ifctester/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49995 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/facet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/ids.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    21793 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.937325 ifctester-0.0.240418/ifctester/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-18 01:14:00.000000 ifctester-0.0.240418/ifctester/templates/report.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.941325 ifctester-0.0.240418/ifctester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 01:14:03.000000 ifctester-0.0.240418/ifctester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-18 01:14:02.000000 ifctester-0.0.240418/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:14:03.941325 ifctester-0.0.240418/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:14:03.937325 ifctester-0.0.240418/test/
--rw-r--r--   0 runner    (1001) docker     (127)    89195 2024-04-18 01:14:00.000000 ifctester-0.0.240418/test/test_facet.py
--rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-04-18 01:14:00.000000 ifctester-0.0.240418/test/test_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.079672 ifctester-0.0.240423/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 09:49:55.079672 ifctester-0.0.240423/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 09:49:47.000000 ifctester-0.0.240423/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.075672 ifctester-0.0.240423/ifctester/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49995 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13489 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/ids.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    21793 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.075672 ifctester-0.0.240423/ifctester/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-23 09:49:47.000000 ifctester-0.0.240423/ifctester/templates/report.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.079672 ifctester-0.0.240423/ifctester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 09:49:55.000000 ifctester-0.0.240423/ifctester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-23 09:49:52.000000 ifctester-0.0.240423/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 09:49:55.079672 ifctester-0.0.240423/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 09:49:55.075672 ifctester-0.0.240423/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    89195 2024-04-23 09:49:47.000000 ifctester-0.0.240423/test/test_facet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-04-23 09:49:47.000000 ifctester-0.0.240423/test/test_ids.py
```

### Comparing `ifctester-0.0.240418/PKG-INFO` & `ifctester-0.0.240423/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.240418
+Version: 0.0.240423
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
 Requires-Dist: ifcopenshell
-Requires-Dist: dateutil
+Requires-Dist: python-dateutil
 Requires-Dist: xmlschema
 Requires-Dist: numpy
 
 # ifctester
 
 With **IfcTester**, you can author and read **Information Delivery Specification** - **IDS** - files and validate your IFC models against IDS to see if your model is compliant. After the audit, you can generate reports in console, as a web page, JSON or BCF file. It works from the command line, as a web app, or as a library.
```

### Comparing `ifctester-0.0.240418/README.md` & `ifctester-0.0.240423/README.md`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester/__init__.py` & `ifctester-0.0.240423/ifctester/__init__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester/__main__.py` & `ifctester-0.0.240423/ifctester/__main__.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester/facet.py` & `ifctester-0.0.240423/ifctester/facet.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester/ids.py` & `ifctester-0.0.240423/ifctester/ids.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester/ids.xsd` & `ifctester-0.0.240423/ifctester/ids.xsd`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester/reporter.py` & `ifctester-0.0.240423/ifctester/reporter.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester/templates/report.html` & `ifctester-0.0.240423/ifctester/templates/report.html`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/ifctester.egg-info/PKG-INFO` & `ifctester-0.0.240423/ifctester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: ifctester
-Version: 0.0.240418
+Version: 0.0.240423
 Summary: IFC model auditing tool with support for IDS
 Author-email: Dion Moult <dion@thinkmoult.com>
 Project-URL: Homepage, http://ifcopenshell.org
 Project-URL: Documentation, https://docs.ifcopenshell.org
 Project-URL: Issues, https://github.com/IfcOpenShell/IfcOpenShell/issues
 Keywords: IFC,IDS,BIM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
 Requires-Dist: ifcopenshell
-Requires-Dist: dateutil
+Requires-Dist: python-dateutil
 Requires-Dist: xmlschema
 Requires-Dist: numpy
 
 # ifctester
 
 With **IfcTester**, you can author and read **Information Delivery Specification** - **IDS** - files and validate your IFC models against IDS to see if your model is compliant. After the audit, you can generate reports in console, as a web page, JSON or BCF file. It works from the command line, as a web app, or as a library.
```

### Comparing `ifctester-0.0.240418/pyproject.toml` & `ifctester-0.0.240423/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifctester"
-version = "0.0.240418"
+version = "0.0.240423"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC model auditing tool with support for IDS"
 readme = "README.md"
 keywords = ["IFC", "IDS", "BIM"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
 ]
-dependencies = ["ifcopenshell", "dateutil", "xmlschema", "numpy"]
+dependencies = ["ifcopenshell", "python-dateutil", "xmlschema", "numpy"]
 
 [project.urls]
 Homepage = "http://ifcopenshell.org"
 Documentation = "https://docs.ifcopenshell.org"
 Issues = "https://github.com/IfcOpenShell/IfcOpenShell/issues"
 
 [tool.setuptools.packages.find]
```

### Comparing `ifctester-0.0.240418/test/test_facet.py` & `ifctester-0.0.240423/test/test_facet.py`

 * *Files identical despite different names*

### Comparing `ifctester-0.0.240418/test/test_ids.py` & `ifctester-0.0.240423/test/test_ids.py`

 * *Files identical despite different names*

