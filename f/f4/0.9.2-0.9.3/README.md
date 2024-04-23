# Comparing `tmp/f4-0.9.2.tar.gz` & `tmp/f4-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.9.2.tar", last modified: Mon Apr 22 21:38:28 2024, max compression
+gzip compressed data, was "f4-0.9.3.tar", last modified: Mon Apr 22 21:52:53 2024, max compression
```

## Comparing `f4-0.9.2.tar` & `f4-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:38:28.892302 f4-0.9.2/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.2/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-22 21:38:28.892238 f4-0.9.2/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.2/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.2/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-22 21:38:28.892933 f4-0.9.2/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:38:28.886908 f4-0.9.2/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:38:28.890362 f4-0.9.2/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.2/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.2/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    16244 2024-04-22 21:33:42.000000 f4-0.9.2/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-22 21:37:57.000000 f4-0.9.2/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.2/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:38:28.892002 f4-0.9.2/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-22 21:38:28.000000 f4-0.9.2/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-22 21:38:28.000000 f4-0.9.2/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-22 21:38:28.000000 f4-0.9.2/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-22 21:38:28.000000 f4-0.9.2/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-22 21:38:28.000000 f4-0.9.2/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:38:28.891242 f4-0.9.2/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    55951 2024-04-22 21:32:21.000000 f4-0.9.2/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.894047 f4-0.9.3/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.3/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-22 21:52:53.893979 f4-0.9.3/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.3/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.3/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-22 21:52:53.894351 f4-0.9.3/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.889430 f4-0.9.3/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.892359 f4-0.9.3/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.3/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.3/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    16338 2024-04-22 21:48:58.000000 f4-0.9.3/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-22 21:50:34.000000 f4-0.9.3/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.3/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.893780 f4-0.9.3/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-22 21:52:53.000000 f4-0.9.3/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-22 21:52:53.893495 f4-0.9.3/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    55962 2024-04-22 21:51:49.000000 f4-0.9.3/test/test.py
```

### Comparing `f4-0.9.2/LICENSE` & `f4-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.9.2/PKG-INFO` & `f4-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.2/setup.cfg` & `f4-0.9.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.9.2
+version = 0.9.3
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.9.2/src/f4/Builder.py` & `f4-0.9.3/src/f4/Builder.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.2/src/f4/Parser.py` & `f4-0.9.3/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.2/src/f4/Transformer.py` & `f4-0.9.3/src/f4/Transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .Builder import *
 from .Parser import *
 
-def transpose(f4_src_file_path, f4_dest_file_path, src_column_for_names, num_parallel=1, tmp_dir_path=None, verbose=False):
+def transpose(f4_src_file_path, f4_dest_file_path, src_column_for_names, index_columns=[], num_parallel=1, tmp_dir_path=None, verbose=False):
     if src_column_for_names is None or not isinstance(src_column_for_names, str) or len(src_column_for_names) == 0:
         raise Exception(f"The value specified for src_column_for_names was invalid.")
 
     print_message(f"Transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
 
     with initialize(f4_src_file_path) as src_file_data:
         num_cols = src_file_data.cache_dict["num_cols"]
@@ -42,15 +42,15 @@
                 with open(chunk_file_path, "rb") as chunk_file:
                     for line in chunk_file:
                         tmp_fw_file.write(line)
 
                 remove(chunk_file_path)
 
     print_message(f"Converting temp file at {tmp_fw_file_path} when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
-    convert_delimited_file(tmp_fw_file_path, f4_dest_file_path, comment_prefix=None, compression_type=src_file_data.decompression_type, num_parallel=num_parallel, verbose=verbose)
+    convert_delimited_file(tmp_fw_file_path, f4_dest_file_path, comment_prefix=None, compression_type=src_file_data.decompression_type, index_columns=index_columns, num_parallel=num_parallel, verbose=verbose)
 
     remove(tmp_fw_file_path)
     rmtree(tmp_dir_path2)
 
 def generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel):
     if num_cols > max_cols_per_chunk:
         column_ranges = generate_range_chunks(num_cols, max_cols_per_chunk)
@@ -195,15 +195,15 @@
     while cn_current < cn_end and (next_char := src_file_data.file_handle[cn_current:(cn_current + 1)]) != b"\n":
         column_name += next_char
         cn_current += 1
 
     return cn_current + 1, column_name
 
 #TODO: This function is not yet designed for files with 1000000+ columns.
-def inner_join(f4_left_src_file_path, f4_right_src_file_path, join_column, f4_dest_file_path, num_parallel=1, tmp_dir_path=None, verbose=False):
+def inner_join(f4_left_src_file_path, f4_right_src_file_path, join_column, f4_dest_file_path, index_columns=[], num_parallel=1, tmp_dir_path=None, verbose=False):
     #TODO: Add error checking to make sure join_column is present in left and right.
     print_message(f"Inner joining {f4_left_src_file_path} and {f4_right_src_file_path} based on the {join_column} column, saving to {f4_dest_file_path}.", verbose)
 
     join_column = join_column.encode()
 
     if tmp_dir_path:
         makedirs(tmp_dir_path, exist_ok=True)
@@ -290,11 +290,11 @@
 
             # TODO: Expand this logic for all compression types. Make sure to document it for users.
             compression_type = None
             if left_file_data.decompression_type == "zstd" or right_file_data.decompression_type == "zstd":
                 compression_type = "zstd"
 
             print_message(f"Converting temp file at {tmp_tsv_file_path} to {f4_dest_file_path}.", verbose)
-            convert_delimited_file(tmp_tsv_file_path, f4_dest_file_path, compression_type=compression_type, num_parallel=num_parallel, comment_prefix=None, verbose=verbose)
+            convert_delimited_file(tmp_tsv_file_path, f4_dest_file_path, compression_type=compression_type, index_columns=index_columns, num_parallel=num_parallel, comment_prefix=None, verbose=verbose)
 
     remove(tmp_tsv_file_path)
     rmtree(tmp_dir_path)
```

### Comparing `f4-0.9.2/src/f4/Utilities.py` & `f4-0.9.3/src/f4/Utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "0.9.2"
+    return "0.9.3"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
```

### Comparing `f4-0.9.2/src/f4.egg-info/PKG-INFO` & `f4-0.9.3/src/f4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.2/test/test.py` & `f4-0.9.3/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,26 +859,27 @@
     num_lines = 0
     with open(out_file_path, "r", newline="\n") as out_file:
         for line in out_file:
             num_lines += 1
 
     print(f"  {elapsed_time:.2f} seconds, {num_lines} lines in output file")
 
-#run_all_small_tests()
+run_all_small_tests()
+#sys.exit()
 
 #for compression_type in [None]:
 #for compression_type in ["zstd"]:
 for compression_type in [None, "zstd"]:
     # Medium tests
     run_larger_tests(num_parallel=1, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
 #    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
 
     # Large tests
-    num_parallel = 1
-#    num_parallel = 4
+#    num_parallel = 1
+    num_parallel = 4
 #    num_parallel = 16
     build_outputs = True
     #build_outputs = False
     verbose = True
     #verbose = False
     check_outputs = True
     #check_outputs = False
```

