# Comparing `tmp/f4-0.9.3.tar.gz` & `tmp/f4-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.9.3.tar", last modified: Mon Apr 22 21:52:53 2024, max compression
+gzip compressed data, was "f4-0.9.4.tar", last modified: Tue Apr 23 13:14:56 2024, max compression
```

## Comparing `f4-0.9.3.tar` & `f4-0.9.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.894047 f4-0.9.3/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.3/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-22 21:52:53.893979 f4-0.9.3/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.3/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.3/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-22 21:52:53.894351 f4-0.9.3/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.889430 f4-0.9.3/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.892359 f4-0.9.3/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.3/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.3/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    16338 2024-04-22 21:48:58.000000 f4-0.9.3/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-22 21:50:34.000000 f4-0.9.3/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.3/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.893780 f4-0.9.3/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.893495 f4-0.9.3/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    55962 2024-04-22 21:51:49.000000 f4-0.9.3/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.204438 f4-0.9.4/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.4/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 13:14:56.204382 f4-0.9.4/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.4/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.4/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-23 13:14:56.204724 f4-0.9.4/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.199612 f4-0.9.4/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.202629 f4-0.9.4/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.4/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.4/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    16337 2024-04-23 12:38:12.000000 f4-0.9.4/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-23 13:13:25.000000 f4-0.9.4/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.4/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.204172 f4-0.9.4/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.203626 f4-0.9.4/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    55960 2024-04-23 13:11:33.000000 f4-0.9.4/test/test.py
```

### Comparing `f4-0.9.3/LICENSE` & `f4-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.9.3/PKG-INFO` & `f4-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.3
+Version: 0.9.4
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.3/setup.cfg` & `f4-0.9.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.9.3
+version = 0.9.4
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.9.3/src/f4/Builder.py` & `f4-0.9.4/src/f4/Builder.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.3/src/f4/Parser.py` & `f4-0.9.4/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.3/src/f4/Transformer.py` & `f4-0.9.4/src/f4/Transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
                 right_join_column_values.append(value)
 
             common_join_values = set(left_join_column_values) & set(right_join_column_values)
 
             # Get column names from the left file.
             left_cn_current, left_cn_end = advance_to_column_names(left_file_data, -1)
             left_columns = []
-            for column_index in range(right_file_data.cache_dict["num_cols"]):
+            for column_index in range(left_file_data.cache_dict["num_cols"]):
                 left_cn_current, column_name = get_next_column_name(left_file_data, left_cn_current, left_cn_end)
                 left_columns.append(column_name)
 
             # Get column names from the right file (excluding the join column).
             right_cn_current, right_cn_end = advance_to_column_names(right_file_data, -1)
             right_columns = []
             for column_index in range(right_file_data.cache_dict["num_cols"]):
```

### Comparing `f4-0.9.3/src/f4/Utilities.py` & `f4-0.9.4/src/f4/Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "0.9.3"
+    return "0.9.4"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
```

### Comparing `f4-0.9.3/src/f4.egg-info/PKG-INFO` & `f4-0.9.4/src/f4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.3
+Version: 0.9.4
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.3/test/test.py` & `f4-0.9.4/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,21 +866,21 @@
 run_all_small_tests()
 #sys.exit()
 
 #for compression_type in [None]:
 #for compression_type in ["zstd"]:
 for compression_type in [None, "zstd"]:
     # Medium tests
-    run_larger_tests(num_parallel=1, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
-#    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
+#    run_larger_tests(num_parallel=1, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
+    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
 
     # Large tests
 #    num_parallel = 1
-    num_parallel = 4
-#    num_parallel = 16
+#    num_parallel = 4
+    num_parallel = 16
     build_outputs = True
     #build_outputs = False
     verbose = True
     #verbose = False
     check_outputs = True
     #check_outputs = False
 
@@ -899,14 +899,14 @@
 #    run_super_tests(num_parallel=num_parallel, size="super_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/super_tall")
 #    run_super_tests(num_parallel=num_parallel, size="super_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/super_wide")
 #    run_super_tests(num_parallel=num_parallel, size="hyper_tall", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_tall")
 #    run_super_tests(num_parallel=num_parallel, size="hyper_wide", extension=".gz", compression_type=compression_type, verbose=verbose, tmp_dir_path="/tmp/hyper_wide")
 
     #Attempt this? https://community.hpe.com/t5/servers-systems-the-right/cray-graph-engine-takes-on-a-trillion-triples/ba-p/7096770
 
-#    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
+    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
 #    f4.transpose("data/large_tall.f4", "/tmp/large_tall_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
 
     f4.inner_join("data/medium.f4", "data/medium.f4", "ID", "/tmp/medium_joined.f4", num_parallel=num_parallel, verbose=verbose)
-    ##f4.inner_join("data/large_tall.f4", "data/large_wide.f4", "ID", "/tmp/large_joined.f4", num_parallel=num_parallel, verbose=verbose)
+#    f4.inner_join("data/large_tall.f4", "data/large_wide.f4", "ID", "/tmp/large_joined.f4", num_parallel=num_parallel, verbose=verbose)
 
 print("All tests passed!!")
```

