# Comparing `tmp/mbp-1.5.90.tar.gz` & `tmp/mbp-1.5.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbp-1.5.90.tar", last modified: Sun Mar 10 10:50:37 2024, max compression
+gzip compressed data, was "mbp-1.5.91.tar", last modified: Mon Apr 22 04:40:25 2024, max compression
```

## Comparing `mbp-1.5.90.tar` & `mbp-1.5.91.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 10:50:37.744217 mbp-1.5.90/
--rw-rw-rw-   0        0        0     1088 2024-01-28 00:08:12.000000 mbp-1.5.90/LICENSE
--rw-rw-rw-   0        0        0     1621 2024-03-10 10:50:37.744217 mbp-1.5.90/PKG-INFO
--rw-rw-rw-   0        0        0     1059 2024-03-10 10:50:13.000000 mbp-1.5.90/README.md
--rw-rw-rw-   0        0        0       42 2024-03-10 10:50:37.744217 mbp-1.5.90/setup.cfg
--rw-rw-rw-   0        0        0      808 2024-03-10 10:50:17.000000 mbp-1.5.90/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-10 10:50:37.717493 mbp-1.5.90/src/
-drwxrwxrwx   0        0        0        0 2024-03-10 10:50:37.729115 mbp-1.5.90/src/mbp/
--rw-rw-rw-   0        0        0       19 2024-01-28 00:08:12.000000 mbp-1.5.90/src/mbp/__init__.py
--rw-rw-rw-   0        0        0    37389 2024-03-10 10:49:46.000000 mbp-1.5.90/src/mbp/core.py
--rw-rw-rw-   0        0        0      374 2024-03-10 10:50:02.000000 mbp-1.5.90/src/mbp/info.py
--rw-rw-rw-   0        0        0     1774 2024-01-28 00:08:12.000000 mbp-1.5.90/src/mbp/llm.py
--rw-rw-rw-   0        0        0      149 2024-01-28 00:08:12.000000 mbp-1.5.90/src/mbp/sync.py
-drwxrwxrwx   0        0        0        0 2024-03-10 10:50:37.743210 mbp-1.5.90/src/mbp.egg-info/
--rw-rw-rw-   0        0        0     1621 2024-03-10 10:50:37.000000 mbp-1.5.90/src/mbp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2024-03-10 10:50:37.000000 mbp-1.5.90/src/mbp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 10:50:37.000000 mbp-1.5.90/src/mbp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-03-10 10:50:37.000000 mbp-1.5.90/src/mbp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-03-10 10:50:37.000000 mbp-1.5.90/src/mbp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 04:40:25.142082 mbp-1.5.91/
+-rw-rw-rw-   0        0        0     1088 2024-04-22 04:13:20.000000 mbp-1.5.91/LICENSE
+-rw-rw-rw-   0        0        0     1621 2024-04-22 04:40:25.141070 mbp-1.5.91/PKG-INFO
+-rw-rw-rw-   0        0        0     1059 2024-04-22 04:27:07.000000 mbp-1.5.91/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-22 04:40:25.142082 mbp-1.5.91/setup.cfg
+-rw-rw-rw-   0        0        0      810 2024-04-22 04:27:13.000000 mbp-1.5.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:40:25.122845 mbp-1.5.91/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 04:40:25.130969 mbp-1.5.91/src/mbp/
+-rw-rw-rw-   0        0        0       19 2024-04-22 04:13:20.000000 mbp-1.5.91/src/mbp/__init__.py
+-rw-rw-rw-   0        0        0    37795 2024-04-22 04:25:25.000000 mbp-1.5.91/src/mbp/core.py
+-rw-rw-rw-   0        0        0      374 2024-04-22 04:27:03.000000 mbp-1.5.91/src/mbp/info.py
+-rw-rw-rw-   0        0        0     1774 2024-04-22 04:13:20.000000 mbp-1.5.91/src/mbp/llm.py
+-rw-rw-rw-   0        0        0      149 2024-04-22 04:13:20.000000 mbp-1.5.91/src/mbp/sync.py
+drwxrwxrwx   0        0        0        0 2024-04-22 04:40:25.140070 mbp-1.5.91/src/mbp.egg-info/
+-rw-rw-rw-   0        0        0     1621 2024-04-22 04:40:25.000000 mbp-1.5.91/src/mbp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2024-04-22 04:40:25.000000 mbp-1.5.91/src/mbp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 04:40:25.000000 mbp-1.5.91/src/mbp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-22 04:40:25.000000 mbp-1.5.91/src/mbp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-22 04:40:25.000000 mbp-1.5.91/src/mbp.egg-info/top_level.txt
```

### Comparing `mbp-1.5.90/LICENSE` & `mbp-1.5.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mbp-1.5.90/PKG-INFO` & `mbp-1.5.91/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbp
-Version: 1.5.90
+Version: 1.5.91
 Summary: Make Python even more beautiful :) This package includes implementations that you wish were in the standard library.
 Home-page: https://github.com/sudongqi/MoreBeautifulPython.git
 Author: Dongqi Su
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12.0
@@ -22,15 +22,15 @@
     python -m pip install mbp
     python -m mbp.info
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp\core.py
     cpu_count             16
-    version               1.5.90
+    version               1.5.91
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 -   replacement for logging
```

### Comparing `mbp-1.5.90/README.md` & `mbp-1.5.91/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     python -m pip install mbp
     python -m mbp.info
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp\core.py
     cpu_count             16
-    version               1.5.90
+    version               1.5.91
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 -   replacement for logging
```

### Comparing `mbp-1.5.90/setup.py` & `mbp-1.5.91/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mbp",
-    version="1.5.90",
+    version="1.5.91",
     author="Dongqi Su",
     description="Make Python even more beautiful :) This package includes implementations that you wish were in the standard library.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sudongqi/MoreBeautifulPython.git",
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -17,8 +17,8 @@
     package_dir={"": "src"},
     packages=find_packages(where="src"),
     python_requires=">=3.12.0",
     install_requires=[
         "wcwidth>=0.2.5",
         "pyyaml>=5.1",
     ],
-)
+)
```

### Comparing `mbp-1.5.90/src/mbp/core.py` & `mbp-1.5.91/src/mbp/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     # logging levels
     'NOTSET', 'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL', 'SILENT',
     # replacement for multiprocessing
     'Workers', 'work',
     # syntax sugar for common utilities
     'try_f', 'stop', 'type_of', 'range_of', 'items_of', 'npath', 'jpath', 'run_dir', 'lib_path',
     # handling data files
-    'load_lines', 'load_txt', 'load_jsonl', 'load_json', 'load_yaml', 'save_txt', 'save_json', 'save_jsonl', 'save_yaml', 'iterate', 'open_file',
+    'load_lines', 'load_txt', 'load_jsonl', 'load_json', 'load_yaml', 'save_txt', 'save_json', 'save_jsonl', 'save_yaml', 'iterate', 'open_file', "load_config",
     # handling paths
     'unwrap_file', 'unwrap_dir', 'file_basename', 'dir_basename',
     # tools for file system
     'traverse', 'this_dir', 'dir_of', 'build_dirs', 'build_files', 'build_dirs_for', 'iterate_files', 'open_files',
     # handling string
     'break_str', 'shorten_str', 'fill_str',
     # tools for debug
@@ -434,14 +434,26 @@
         for d in data:
             f.write(json.dumps(d, ensure_ascii=False) + '\n')
 
 
 def save_json(path, data, indent=4, encoding='utf-8'):
     with open(path, 'w', encoding=encoding) as f:
         return json.dump(data, f, indent=indent)
+    
+
+def load_config(path, user_overwrite_key="__user__"):
+    if path.endswith(".yaml") or path.endswith(".yml"):
+        res = load_yaml(path)
+    elif path.endswith(".json"):
+        res = load_json(path)
+    else:
+        assert False, "path must ends with yaml, yml, or json"
+    res.update(res.get(user_overwrite_key))
+    res.pop(user_overwrite_key, None)
+    return res
 
 
 def type_of(data, types):
     assert isinstance(types, list), 'types must be a list'
     for idx, _type in enumerate(types):
         if isinstance(data, _type):
             return idx + 1
```

### Comparing `mbp-1.5.90/src/mbp/llm.py` & `mbp-1.5.91/src/mbp/llm.py`

 * *Files identical despite different names*

### Comparing `mbp-1.5.90/src/mbp.egg-info/PKG-INFO` & `mbp-1.5.91/src/mbp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbp
-Version: 1.5.90
+Version: 1.5.91
 Summary: Make Python even more beautiful :) This package includes implementations that you wish were in the standard library.
 Home-page: https://github.com/sudongqi/MoreBeautifulPython.git
 Author: Dongqi Su
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12.0
@@ -22,15 +22,15 @@
     python -m pip install mbp
     python -m mbp.info
     =================================== More Beautiful Python ===================================
     examples              https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
     execution_directory   C:\Users\sudon\MoreBeautifulPython
     library_path          C:\Users\sudon\MoreBeautifulPython\src\mbp\core.py
     cpu_count             16
-    version               1.5.90
+    version               1.5.91
     =============================================================================================
 
 ### Examples
 
 https://github.com/sudongqi/MoreBeautifulPython/blob/main/examples.py
 
 -   replacement for logging
```

