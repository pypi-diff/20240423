# Comparing `tmp/pybunch-1.0.6.tar.gz` & `tmp/pybunch-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybunch-1.0.6.tar", last modified: Tue Apr 23 08:42:41 2024, max compression
+gzip compressed data, was "pybunch-1.0.7.tar", last modified: Tue Apr 23 08:47:32 2024, max compression
```

## Comparing `pybunch-1.0.6.tar` & `pybunch-1.0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.052087 pybunch-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 08:42:36.000000 pybunch-1.0.6/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 08:42:36.000000 pybunch-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 08:42:36.000000 pybunch-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:42:41.056087 pybunch-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 08:42:36.000000 pybunch-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/example/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/fibonnaci.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/example/submodule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/submodule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/submodule/motd.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:36.000000 pybunch-1.0.6/example/unused.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 08:42:36.000000 pybunch-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:42:41.056087 pybunch-1.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.052087 pybunch-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/src/pybunch/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/packed_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-23 08:42:36.000000 pybunch-1.0.6/src/pybunch/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:42:41.056087 pybunch-1.0.6/src/pybunch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:42:41.000000 pybunch-1.0.6/src/pybunch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-23 08:47:27.000000 pybunch-1.0.7/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-23 08:47:27.000000 pybunch-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-23 08:47:27.000000 pybunch-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:47:32.004324 pybunch-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-23 08:47:27.000000 pybunch-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/fibonnaci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/example/submodule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/submodule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/submodule/motd.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:27.000000 pybunch-1.0.7/example/unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 08:47:27.000000 pybunch-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 08:47:32.004324 pybunch-1.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.000324 pybunch-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/src/pybunch/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/packed_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-23 08:47:27.000000 pybunch-1.0.7/src/pybunch/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 08:47:32.004324 pybunch-1.0.7/src/pybunch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 08:47:31.000000 pybunch-1.0.7/src/pybunch.egg-info/top_level.txt
```

### Comparing `pybunch-1.0.6/.github/workflows/publish-to-pypi.yaml` & `pybunch-1.0.7/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.6/LICENSE` & `pybunch-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.6/PKG-INFO` & `pybunch-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pybunch-1.0.6/pyproject.toml` & `pybunch-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.6/src/pybunch/__main__.py` & `pybunch-1.0.7/src/pybunch/__main__.py`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.6/src/pybunch/packed_base.py` & `pybunch-1.0.7/src/pybunch/packed_base.py`

 * *Files identical despite different names*

### Comparing `pybunch-1.0.6/src/pybunch/project.py` & `pybunch-1.0.7/src/pybunch/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,17 @@
 
         code_entries = []
         package_entries = []
         for pth in included_packages:
             name = '.'.join(pth.parts)
             escaped_name = 'PYBUNCH_%s' % '_'.join(pth.parts).upper()
             code = self._package_mapping[pth].read_text()
+            escaped_code = code.replace('"', '\\"')
 
-            code_entries.append(f'# Code for module <{name}>\n{escaped_name} = """\\n{code}\\n"""[1:]')
+            code_entries.append(f'# Code for module <{name}>\n{escaped_name} = """\n{escaped_code}\n"""[1:]')
             package_entries.append(f"'{name}': ModuleDescription('{name}', code={escaped_name})")
 
         header = ''.join(entry + "\n\n\n" for entry in code_entries)
         footer = f"""\n\n
 dli = DynamicLocalImporter({{
 {',\n'.join("    %s" % entry for entry in package_entries)}
 }})
```

### Comparing `pybunch-1.0.6/src/pybunch.egg-info/PKG-INFO` & `pybunch-1.0.7/src/pybunch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybunch
-Version: 1.0.6
+Version: 1.0.7
 Summary: A python utility to pack python projects into a single python file
 Author-email: Yonatan Karidi <ykaridi@gmail.com>
 Project-URL: Homepage, https://github.com/ykaridi/pybunch
 Project-URL: Issues, https://github.com/ykaridi/pybunch/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

