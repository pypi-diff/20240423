# Comparing `tmp/meafs-4.6.1.tar.gz` & `tmp/meafs-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meafs-4.6.1.tar", last modified: Tue Apr 23 18:51:34 2024, max compression
+gzip compressed data, was "meafs-4.6.2.tar", last modified: Tue Apr 23 18:55:24 2024, max compression
```

## Comparing `meafs-4.6.1.tar` & `meafs-4.6.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:51:34.298080 meafs-4.6.1/
--rwxr-xr-x   0 castro    (1000) users      (984)     1074 2024-04-23 18:50:35.000000 meafs-4.6.1/LICENSE.txt
--rwxr-xr-x   0 castro    (1000) users      (984)       32 2024-04-23 18:50:35.000000 meafs-4.6.1/MANIFEST.in
--rw-r--r--   0 castro    (1000) users      (984)     9619 2024-04-23 18:51:34.298080 meafs-4.6.1/PKG-INFO
--rwxr-xr-x   0 castro    (1000) users      (984)     8960 2024-04-23 18:50:35.000000 meafs-4.6.1/README.md
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:51:34.298080 meafs-4.6.1/meafs.egg-info/
--rw-r--r--   0 castro    (1000) users      (984)     9619 2024-04-23 18:51:34.000000 meafs-4.6.1/meafs.egg-info/PKG-INFO
--rw-r--r--   0 castro    (1000) users      (984)      914 2024-04-23 18:51:34.000000 meafs-4.6.1/meafs.egg-info/SOURCES.txt
--rw-r--r--   0 castro    (1000) users      (984)        1 2024-04-23 18:51:34.000000 meafs-4.6.1/meafs.egg-info/dependency_links.txt
--rw-r--r--   0 castro    (1000) users      (984)      156 2024-04-23 18:51:34.000000 meafs-4.6.1/meafs.egg-info/entry_points.txt
--rw-r--r--   0 castro    (1000) users      (984)       85 2024-04-23 18:51:34.000000 meafs-4.6.1/meafs.egg-info/requires.txt
--rw-r--r--   0 castro    (1000) users      (984)       11 2024-04-23 18:51:34.000000 meafs-4.6.1/meafs.egg-info/top_level.txt
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:51:34.294746 meafs-4.6.1/meafs_code/
--rwxr-xr-x   0 castro    (1000) users      (984)       26 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/__init__.py
--rwxr-xr-x   0 castro    (1000) users      (984)       37 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/__main__.py
--rwxr-xr-x   0 castro    (1000) users      (984)       78 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/convert.sh
--rwxr-xr-x   0 castro    (1000) users      (984)     4259 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/desktop_entry.py
--rw-r--r--   0 castro    (1000) users      (984)    11095 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/fitsettings.ui
--rw-r--r--   0 castro    (1000) users      (984)    14517 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/fitsettings_qt.py
--rwxr-xr-x   0 castro    (1000) users      (984)    46615 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/gui.py
--rwxr-xr-x   0 castro    (1000) users      (984)    42133 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/gui_qt.py
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:51:34.294746 meafs-4.6.1/meafs_code/images/
--rw-r--r--   0 castro    (1000) users      (984)   190114 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/images/Meafs_Gui.png
--rwxr-xr-x   0 castro    (1000) users      (984)    42476 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/images/Meafs_Icon.ico
--rwxr-xr-x   0 castro    (1000) users      (984)   220589 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/images/Meafs_Logo.png
--rwxr-xr-x   0 castro    (1000) users      (984)    36066 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/meafs.ui
-drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:51:34.298080 meafs-4.6.1/meafs_code/scripts/
--rwxr-xr-x   0 castro    (1000) users      (984)      142 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/__init__.py
--rwxr-xr-x   0 castro    (1000) users      (984)    12110 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/abundance_analysis.py
--rwxr-xr-x   0 castro    (1000) users      (984)    28910 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/abundance_fit.py
--rwxr-xr-x   0 castro    (1000) users      (984)     1936 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/bisec_interpol.c
--rwxr-xr-x   0 castro    (1000) users      (984)    15472 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/bisec_interpol.so
--rwxr-xr-x   0 castro    (1000) users      (984)      148 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/comp.sh
--rw-r--r--   0 castro    (1000) users      (984)     5078 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/fit_functions.py
--rw-r--r--   0 castro    (1000) users      (984)     4975 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/turbospec_functions.py
--rwxr-xr-x   0 castro    (1000) users      (984)     3343 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/unify_plots.py
--rw-r--r--   0 castro    (1000) users      (984)     2868 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/scripts/voigt_functions.py
--rw-r--r--   0 castro    (1000) users      (984)       27 2024-04-23 18:50:35.000000 meafs-4.6.1/meafs_code/settings.csv
--rwxr-xr-x   0 castro    (1000) users      (984)      766 2024-04-23 18:50:35.000000 meafs-4.6.1/pyproject.toml
--rw-r--r--   0 castro    (1000) users      (984)       38 2024-04-23 18:51:34.298080 meafs-4.6.1/setup.cfg
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:55:24.877720 meafs-4.6.2/
+-rwxr-xr-x   0 castro    (1000) users      (984)     1074 2024-04-23 18:50:35.000000 meafs-4.6.2/LICENSE.txt
+-rwxr-xr-x   0 castro    (1000) users      (984)       32 2024-04-23 18:50:35.000000 meafs-4.6.2/MANIFEST.in
+-rw-r--r--   0 castro    (1000) users      (984)     9616 2024-04-23 18:55:24.877720 meafs-4.6.2/PKG-INFO
+-rwxr-xr-x   0 castro    (1000) users      (984)     8957 2024-04-23 18:55:09.000000 meafs-4.6.2/README.md
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:55:24.877720 meafs-4.6.2/meafs.egg-info/
+-rw-r--r--   0 castro    (1000) users      (984)     9616 2024-04-23 18:55:24.000000 meafs-4.6.2/meafs.egg-info/PKG-INFO
+-rw-r--r--   0 castro    (1000) users      (984)      914 2024-04-23 18:55:24.000000 meafs-4.6.2/meafs.egg-info/SOURCES.txt
+-rw-r--r--   0 castro    (1000) users      (984)        1 2024-04-23 18:55:24.000000 meafs-4.6.2/meafs.egg-info/dependency_links.txt
+-rw-r--r--   0 castro    (1000) users      (984)      156 2024-04-23 18:55:24.000000 meafs-4.6.2/meafs.egg-info/entry_points.txt
+-rw-r--r--   0 castro    (1000) users      (984)       85 2024-04-23 18:55:24.000000 meafs-4.6.2/meafs.egg-info/requires.txt
+-rw-r--r--   0 castro    (1000) users      (984)       11 2024-04-23 18:55:24.000000 meafs-4.6.2/meafs.egg-info/top_level.txt
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:55:24.874387 meafs-4.6.2/meafs_code/
+-rwxr-xr-x   0 castro    (1000) users      (984)       26 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/__init__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)       37 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/__main__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)       78 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/convert.sh
+-rwxr-xr-x   0 castro    (1000) users      (984)     4259 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/desktop_entry.py
+-rw-r--r--   0 castro    (1000) users      (984)    11095 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/fitsettings.ui
+-rw-r--r--   0 castro    (1000) users      (984)    14517 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/fitsettings_qt.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    46615 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/gui.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    42133 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/gui_qt.py
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:55:24.874387 meafs-4.6.2/meafs_code/images/
+-rw-r--r--   0 castro    (1000) users      (984)   190114 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/images/Meafs_Gui.png
+-rwxr-xr-x   0 castro    (1000) users      (984)    42476 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/images/Meafs_Icon.ico
+-rwxr-xr-x   0 castro    (1000) users      (984)   220589 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/images/Meafs_Logo.png
+-rwxr-xr-x   0 castro    (1000) users      (984)    36066 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/meafs.ui
+drwxr-xr-x   0 castro    (1000) users      (984)        0 2024-04-23 18:55:24.877720 meafs-4.6.2/meafs_code/scripts/
+-rwxr-xr-x   0 castro    (1000) users      (984)      142 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/__init__.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    12110 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/abundance_analysis.py
+-rwxr-xr-x   0 castro    (1000) users      (984)    28910 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/abundance_fit.py
+-rwxr-xr-x   0 castro    (1000) users      (984)     1936 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/bisec_interpol.c
+-rwxr-xr-x   0 castro    (1000) users      (984)    15472 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/bisec_interpol.so
+-rwxr-xr-x   0 castro    (1000) users      (984)      148 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/comp.sh
+-rw-r--r--   0 castro    (1000) users      (984)     5078 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/fit_functions.py
+-rw-r--r--   0 castro    (1000) users      (984)     4975 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/turbospec_functions.py
+-rwxr-xr-x   0 castro    (1000) users      (984)     3343 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/unify_plots.py
+-rw-r--r--   0 castro    (1000) users      (984)     2868 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/scripts/voigt_functions.py
+-rw-r--r--   0 castro    (1000) users      (984)       27 2024-04-23 18:50:35.000000 meafs-4.6.2/meafs_code/settings.csv
+-rwxr-xr-x   0 castro    (1000) users      (984)      766 2024-04-23 18:55:09.000000 meafs-4.6.2/pyproject.toml
+-rw-r--r--   0 castro    (1000) users      (984)       38 2024-04-23 18:55:24.877720 meafs-4.6.2/setup.cfg
```

### Comparing `meafs-4.6.1/LICENSE.txt` & `meafs-4.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/PKG-INFO` & `meafs-4.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meafs
-Version: 4.6.1
+Version: 4.6.2
 Summary: Multiple Element Abundance Fit Software
 Author: Matheus J. Castro
 Project-URL: Homepage, https://github.com/MatheusJCastro/meafs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -85,17 +85,17 @@
 
 - Then, to activate the environment, type `conda activate meafs`;
 
 ### Getting the pip version (recommended)
 
 The pip version can easily be acquired by typing in the terminal:
 
-#```bash
-#pip install meafs
-#```
+```bash
+pip install meafs
+```
 
 ### Cloning from GitHub
 
 Or you can directly clone from the GitHub page with:
 
 ```bash
 git clone https://github.com/MatheusJCastro/meafs.git
```

### Comparing `meafs-4.6.1/README.md` & `meafs-4.6.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
 
 - Then, to activate the environment, type `conda activate meafs`;
 
 ### Getting the pip version (recommended)
 
 The pip version can easily be acquired by typing in the terminal:
 
-#```bash
-#pip install meafs
-#```
+```bash
+pip install meafs
+```
 
 ### Cloning from GitHub
 
 Or you can directly clone from the GitHub page with:
 
 ```bash
 git clone https://github.com/MatheusJCastro/meafs.git
```

### Comparing `meafs-4.6.1/meafs.egg-info/PKG-INFO` & `meafs-4.6.2/meafs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meafs
-Version: 4.6.1
+Version: 4.6.2
 Summary: Multiple Element Abundance Fit Software
 Author: Matheus J. Castro
 Project-URL: Homepage, https://github.com/MatheusJCastro/meafs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -85,17 +85,17 @@
 
 - Then, to activate the environment, type `conda activate meafs`;
 
 ### Getting the pip version (recommended)
 
 The pip version can easily be acquired by typing in the terminal:
 
-#```bash
-#pip install meafs
-#```
+```bash
+pip install meafs
+```
 
 ### Cloning from GitHub
 
 Or you can directly clone from the GitHub page with:
 
 ```bash
 git clone https://github.com/MatheusJCastro/meafs.git
```

### Comparing `meafs-4.6.1/meafs.egg-info/SOURCES.txt` & `meafs-4.6.2/meafs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/desktop_entry.py` & `meafs-4.6.2/meafs_code/desktop_entry.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/fitsettings.ui` & `meafs-4.6.2/meafs_code/fitsettings.ui`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/fitsettings_qt.py` & `meafs-4.6.2/meafs_code/fitsettings_qt.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/gui.py` & `meafs-4.6.2/meafs_code/gui.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/gui_qt.py` & `meafs-4.6.2/meafs_code/gui_qt.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/images/Meafs_Gui.png` & `meafs-4.6.2/meafs_code/images/Meafs_Gui.png`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/images/Meafs_Icon.ico` & `meafs-4.6.2/meafs_code/images/Meafs_Icon.ico`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/images/Meafs_Logo.png` & `meafs-4.6.2/meafs_code/images/Meafs_Logo.png`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/meafs.ui` & `meafs-4.6.2/meafs_code/meafs.ui`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/abundance_analysis.py` & `meafs-4.6.2/meafs_code/scripts/abundance_analysis.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/abundance_fit.py` & `meafs-4.6.2/meafs_code/scripts/abundance_fit.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/bisec_interpol.c` & `meafs-4.6.2/meafs_code/scripts/bisec_interpol.c`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/bisec_interpol.so` & `meafs-4.6.2/meafs_code/scripts/bisec_interpol.so`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/fit_functions.py` & `meafs-4.6.2/meafs_code/scripts/fit_functions.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/turbospec_functions.py` & `meafs-4.6.2/meafs_code/scripts/turbospec_functions.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/unify_plots.py` & `meafs-4.6.2/meafs_code/scripts/unify_plots.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/meafs_code/scripts/voigt_functions.py` & `meafs-4.6.2/meafs_code/scripts/voigt_functions.py`

 * *Files identical despite different names*

### Comparing `meafs-4.6.1/pyproject.toml` & `meafs-4.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "meafs"
-version = "4.6.1"
+version = "4.6.2"
 authors = [
     { name="Matheus J. Castro" }
 ]
 description="Multiple Element Abundance Fit Software"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers=[
```

