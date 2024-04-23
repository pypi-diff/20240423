# Comparing `tmp/loe_simp_app_fw-1.1.0.tar.gz` & `tmp/loe_simp_app_fw-1.1.1.tar.gz`

## Comparing `loe_simp_app_fw-1.1.0.tar` & `loe_simp_app_fw-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/config-example.yaml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/src/loe_simp_app_fw/__init__.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/src/loe_simp_app_fw/config.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/src/loe_simp_app_fw/helper.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/src/loe_simp_app_fw/logger.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/tests/test_import.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/LICENSE
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/config-example.yaml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/config.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/helper.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/logger.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/tests/test_import.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 loe_simp_app_fw-1.1.1/PKG-INFO
```

### Comparing `loe_simp_app_fw-1.1.0/src/loe_simp_app_fw/config.py` & `loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 # Setup flags
 isCLI = False
 
 # Parse CLI or not
 def isNotebook() -> bool:
     try:
-        shell = get_ipython().__class__.__name__
+        shell = get_ipython().__class__.__name__ # het_python() is globally available when using jupyter notebook
         if shell == 'ZMQInteractiveShell':
             return True   # Jupyter notebook or qtconsole
         elif shell == 'TerminalInteractiveShell':
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
     except NameError:
```

### Comparing `loe_simp_app_fw-1.1.0/src/loe_simp_app_fw/helper.py` & `loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/helper.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,26 +7,31 @@
     def create_folder_if_not_exists(folder_path: str) -> bool:
         # Return if the folder exists
         # It only create one folder at a time
 
         if not os.path.isfile(folder_path) and not os.path.isdir(folder_path):
             os.mkdir(folder_path)
             print(f"Folder {folder_path} does not exists. Creating a new one.")
+            return True
+        else:
+            return False
 else:
     # Normal mode
-
+    from .logger import Logger
     def create_folder_if_not_exists(folder_path: str) -> bool:
         # Return if the folder exists
         # It only create one folder at a time
 
         if not os.path.isfile(folder_path) and not os.path.isdir(folder_path):
             os.mkdir(folder_path)
-            logger.Logger.info("Folder does not exists. Creating a new one.")
+            Logger.info("Folder does not exists. Creating a new one.")
+            return True
         else:
-            logger.Logger.debug("Folder exists. No further action.")
+            Logger.debug("Folder exists. No further action.")
+            return False
 
 def remove_duplicate_space(input_str: str) -> str:
     # Remove excessive space
     reg = r'\s+'
     result = re.sub(reg, " ", input_str).strip()
     return result
```

### Comparing `loe_simp_app_fw-1.1.0/src/loe_simp_app_fw/logger.py` & `loe_simp_app_fw-1.1.1/src/loe_simp_app_fw/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             log_folder_path (str): path to log folder relative to project root path
             project_root_path (str, optional): path to project top-level directory. Defaults to os.getcwd().
 
         Raises:
             ProjectRootChanged: Project root directory should not be changed once set
         """
         # Sanity check
-        if Logger._project_root_path and project_root_path and os.path.samefile(project_root_path, Logger._project_root_path):
+        if Logger._project_root_path and project_root_path and not os.path.samefile(project_root_path, Logger._project_root_path):
             Logger.error("One should not change project root path twice")
             raise ProjectRootChanged
 
         # Save input
         Logger._log_folder_path = log_folder_path
         Logger._project_root_path = project_root_path
```

### Comparing `loe_simp_app_fw-1.1.0/tests/test_import.py` & `loe_simp_app_fw-1.1.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.0/.gitignore` & `loe_simp_app_fw-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.0/LICENSE` & `loe_simp_app_fw-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.0/README.md` & `loe_simp_app_fw-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `loe_simp_app_fw-1.1.0/pyproject.toml` & `loe_simp_app_fw-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "loe_simp_app_fw"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="loeeeee", email="95266635+loeeeee@users.noreply.github.com" },
 ]
 description = "A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `loe_simp_app_fw-1.1.0/PKG-INFO` & `loe_simp_app_fw-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: loe_simp_app_fw
-Version: 1.1.0
+Version: 1.1.1
 Summary: A super simple python app framework that includes a logger and a config manager. Also usable in jupyter notebook.
 Project-URL: Homepage, https://github.com/loeeeee/loe-simp-app-fw
 Project-URL: Issues, https://github.com/loeeeee/loe-simp-app-fw/issues
 Author-email: loeeeee <95266635+loeeeee@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

