# Comparing `tmp/sinaraml-2024.4.19.tar.gz` & `tmp/sinaraml-2024.4.23.tar.gz`

## Comparing `sinaraml-2024.4.19.tar` & `sinaraml-2024.4.23.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/__init__.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/_version.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/org_manager.py
--rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/sinaraml/sinaraml.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/LICENSE
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/pyproject.toml
--rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 sinaraml-2024.4.19/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/sinaraml/__init__.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/sinaraml/_version.py
+-rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/sinaraml/org_manager.py
+-rw-r--r--   0        0        0     5044 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/sinaraml/sinaraml.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/pyproject.toml
+-rw-r--r--   0        0        0     6693 2020-02-02 00:00:00.000000 sinaraml-2024.4.23/PKG-INFO
```

### Comparing `sinaraml-2024.4.19/sinaraml/org_manager.py` & `sinaraml-2024.4.23/sinaraml/org_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,26 +107,25 @@
         
         install_dir = SinaraOrgManager.get_orgs_dir()
         install_dir.mkdir(parents=True, exist_ok=True)
         install_dir = Path(install_dir, 'mlops_organization')
         if install_dir.exists() and install_dir.is_dir():
             shutil.rmtree(install_dir)
         
-        print(install_dir)
-        command = ['git', 'clone', gitref, str(install_dir)]
+        command = f'git clone {gitref} {str(install_dir)}'
         print(command)
         try:
-            subprocess.run(command, timeout=60)
+            subprocess.run(command, timeout=60, shell=True)
         except subprocess.TimeoutExpired:
             print('git clone process ran too long')
             return
         
         with open(f'{install_dir}/mlops_organization.json') as f:
             org = json.load(f)
-        print(org)
+        #print(org)
         new_org_dir = Path(install_dir.parent.absolute(), org["name"])
         #remove destination directory
         if new_org_dir.exists() and new_org_dir.is_dir():
             shutil.rmtree(new_org_dir)
         shutil.move(install_dir, new_org_dir)
 
         SinaraOrgManager._install_org_requirements(new_org_dir)
```

### Comparing `sinaraml-2024.4.19/sinaraml/sinaraml.py` & `sinaraml-2024.4.23/sinaraml/sinaraml.py`

 * *Files identical despite different names*

### Comparing `sinaraml-2024.4.19/.gitignore` & `sinaraml-2024.4.23/.gitignore`

 * *Files identical despite different names*

### Comparing `sinaraml-2024.4.19/LICENSE` & `sinaraml-2024.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `sinaraml-2024.4.19/README.md` & `sinaraml-2024.4.23/README.md`

 * *Files identical despite different names*

### Comparing `sinaraml-2024.4.19/pyproject.toml` & `sinaraml-2024.4.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sinaraml-2024.4.19/PKG-INFO` & `sinaraml-2024.4.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sinaraml
-Version: 2024.4.19
+Version: 2024.4.23
 Summary: SinaraML
 Project-URL: Homepage, https://github.com/4-DS/sinaraml
 Author-email: sinaraml <sinaraml.official@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 SinaraML
```

