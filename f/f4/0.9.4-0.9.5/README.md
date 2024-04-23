# Comparing `tmp/f4-0.9.4.tar.gz` & `tmp/f4-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f4-0.9.4.tar", last modified: Tue Apr 23 13:14:56 2024, max compression
+gzip compressed data, was "f4-0.9.5.tar", last modified: Tue Apr 23 18:15:10 2024, max compression
```

## Comparing `f4-0.9.4.tar` & `f4-0.9.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.204438 f4-0.9.4/
--rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.4/LICENSE
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 13:14:56.204382 f4-0.9.4/PKG-INFO
--rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.4/README.md
--rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.4/pyproject.toml
--rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-23 13:14:56.204724 f4-0.9.4/setup.cfg
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.199612 f4-0.9.4/src/
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.202629 f4-0.9.4/src/f4/
--rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.4/src/f4/Builder.py
--rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.4/src/f4/Parser.py
--rw-r--r--   0 srp33      (503) staff       (20)    16337 2024-04-23 12:38:12.000000 f4-0.9.4/src/f4/Transformer.py
--rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-23 13:13:25.000000 f4-0.9.4/src/f4/Utilities.py
--rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.4/src/f4/__init__.py
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.204172 f4-0.9.4/src/f4.egg-info/
--rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/PKG-INFO
--rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/SOURCES.txt
--rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/dependency_links.txt
--rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/requires.txt
--rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-23 13:14:56.000000 f4-0.9.4/src/f4.egg-info/top_level.txt
-drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 13:14:56.203626 f4-0.9.4/test/
--rwxr-xr-x   0 srp33      (503) staff       (20)    55960 2024-04-23 13:11:33.000000 f4-0.9.4/test/test.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.774664 f4-0.9.5/
+-rw-r--r--   0 srp33      (503) staff       (20)    11357 2023-12-07 22:20:43.000000 f4-0.9.5/LICENSE
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:15:10.774606 f4-0.9.5/PKG-INFO
+-rwxr-xr-x   0 srp33      (503) staff       (20)       67 2023-12-07 22:20:43.000000 f4-0.9.5/README.md
+-rw-r--r--   0 srp33      (503) staff       (20)      104 2023-12-07 22:20:43.000000 f4-0.9.5/pyproject.toml
+-rw-r--r--   0 srp33      (503) staff       (20)      733 2024-04-23 18:15:10.774971 f4-0.9.5/setup.cfg
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.770460 f4-0.9.5/src/
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.773333 f4-0.9.5/src/f4/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    43623 2024-04-19 19:32:05.000000 f4-0.9.5/src/f4/Builder.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)    57954 2024-04-20 14:29:06.000000 f4-0.9.5/src/f4/Parser.py
+-rw-r--r--   0 srp33      (503) staff       (20)    15334 2024-04-23 18:14:14.000000 f4-0.9.5/src/f4/Transformer.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)     8388 2024-04-23 18:14:41.000000 f4-0.9.5/src/f4/Utilities.py
+-rwxr-xr-x   0 srp33      (503) staff       (20)      390 2024-04-20 14:32:09.000000 f4-0.9.5/src/f4/__init__.py
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.774391 f4-0.9.5/src/f4.egg-info/
+-rw-r--r--   0 srp33      (503) staff       (20)      711 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/PKG-INFO
+-rw-r--r--   0 srp33      (503) staff       (20)      300 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/SOURCES.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        1 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/dependency_links.txt
+-rw-r--r--   0 srp33      (503) staff       (20)       67 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/requires.txt
+-rw-r--r--   0 srp33      (503) staff       (20)        3 2024-04-23 18:15:10.000000 f4-0.9.5/src/f4.egg-info/top_level.txt
+drwxr-xr-x   0 srp33      (503) staff       (20)        0 2024-04-23 18:15:10.774196 f4-0.9.5/test/
+-rwxr-xr-x   0 srp33      (503) staff       (20)    55963 2024-04-23 17:55:35.000000 f4-0.9.5/test/test.py
```

### Comparing `f4-0.9.4/LICENSE` & `f4-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `f4-0.9.4/PKG-INFO` & `f4-0.9.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.4/setup.cfg` & `f4-0.9.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = f4
-version = 0.9.4
+version = 0.9.5
 author = Stephen R. Piccolo
 author_email = stephen.piccolo.byu@gmail.com
 description = A Python package for the Fast Fixed-width File Format (F4)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/srp33/f4py
 project_urls =
```

### Comparing `f4-0.9.4/src/f4/Builder.py` & `f4-0.9.5/src/f4/Builder.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.4/src/f4/Parser.py` & `f4-0.9.5/src/f4/Parser.py`

 * *Files identical despite different names*

### Comparing `f4-0.9.4/src/f4/Transformer.py` & `f4-0.9.5/src/f4/Transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .Builder import *
 from .Parser import *
 
 def transpose(f4_src_file_path, f4_dest_file_path, src_column_for_names, index_columns=[], num_parallel=1, tmp_dir_path=None, verbose=False):
     if src_column_for_names is None or not isinstance(src_column_for_names, str) or len(src_column_for_names) == 0:
         raise Exception(f"The value specified for src_column_for_names was invalid.")
 
-    print_message(f"Transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
+    print_message(f"Finding max column width when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
 
     with initialize(f4_src_file_path) as src_file_data:
         num_cols = src_file_data.cache_dict["num_cols"]
         max_column_width = get_max_column_width(src_file_data)
 
     tmp_dir_path2 = prepare_tmp_dir(tmp_dir_path)
     tmp_fw_file_path = f"{tmp_dir_path2}fw"
@@ -30,14 +30,16 @@
             chunk_range,
             max_column_width,
             f"{tmp_dir_path2}chunk_{chunk_number}.fw",
             verbose)
                 for chunk_number, chunk_range in enumerate(generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel))
         )
 
+        print_message(f"Assembling chunks when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
+
         # Put the chunks together.
         with open(tmp_fw_file_path, "wb") as tmp_fw_file:
             for chunk_number, _ignore in enumerate(generate_column_ranges(max_cols_per_chunk, num_cols, num_parallel)):
                 chunk_file_path = f"{tmp_dir_path2}chunk_{chunk_number}.fw"
 
                 with open(chunk_file_path, "rb") as chunk_file:
                     for line in chunk_file:
@@ -73,23 +75,25 @@
         column_size = column_coords[1] - column_coords[0]
         max_column_width = max(max_column_width, column_size)
 
     return max_column_width
 
 def transpose_column_chunk(f4_src_file_path, src_column_for_names, chunk_number, column_range, max_column_width, tmp_fw_file_path, verbose):
     with initialize(f4_src_file_path) as src_file_data:
+        print_message(f"Parsing column coordinates for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
         # Get basic meta information.
         num_rows = src_file_data.cache_dict["num_rows"]
         src_column_for_names_index = get_column_index_from_name(src_file_data, src_column_for_names.encode())
         src_column_for_names_coords = parse_data_coord(src_file_data, "", src_column_for_names_index)
         parse_row_value_function = get_parse_row_value_function(src_file_data)
         parse_row_values_function = get_parse_row_values_function(src_file_data)
 
         all_column_coords = parse_data_coords(src_file_data, "", column_range)
 
+        print_message(f"Filling temp file {tmp_fw_file_path} with empty space for chunk {chunk_number} when transposing {f4_src_file_path}.", verbose)
         # We can't compress this file because we have to navigate around it later.
         with open(tmp_fw_file_path, "wb") as fw_file:
             if chunk_number == 0:
                 # Write the value to the top-left cell.
                 fw_file.write(format_string_as_fixed_width(src_column_for_names.encode(), max_column_width) + b"\t")
 
                 # Write the transposed column names (except the last one).
@@ -115,71 +119,48 @@
 
         cn_current, cn_end = advance_to_column_names(src_file_data, column_range[0] - 1)
         # Skip the first column name because we already wrote it in the top-left corner.
         cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
 
         # We can't compress this file because we have to navigate within it.
         with open(tmp_fw_file_path, "rb+") as fw_file:
-            with mmap(fw_file.fileno(), 0, prot=PROT_WRITE) as fw_handle:
-                # Save new row names.
-                for chunk_column_index, overall_column_index in enumerate(column_range):
-                    if overall_column_index == src_column_for_names_index:
-                        continue
-
-                    cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
-                    row_start = chunk_column_index * new_row_width
-                    fw_handle[row_start:(row_start + len(column_name))] = column_name
-
-                # Save values in transposed orientation.
-                for row_index in range(num_rows):
-                    if row_index < 10 or (row_index < 100 and row_index % 10 == 0) or row_index % 100 == 0:
-                        print_message(f"Transposing {f4_src_file_path} to temporary file {tmp_fw_file_path} for row {row_index}.", verbose)
-
-                    #FYI: Retrieving all values in a row is much faster than one at a time.
-                    values = parse_row_values_function(src_file_data, "", row_index, all_column_coords)
-
-                    for chunk_column_index, overall_column_index in enumerate(column_range):
-                        if overall_column_index == src_column_for_names_index:
-                            continue
-
-                        value = values[chunk_column_index]
+            # FYI: Using memory mapping is an option, but it can consume a lot of memory
+            #      in this context.
+            # with mmap(fw_file.fileno(), 0, prot=PROT_WRITE) as fw_handle:
+            # Save new row names.
+            for chunk_column_index, overall_column_index in enumerate(column_range):
+                if overall_column_index == src_column_for_names_index:
+                    continue
 
-                        row_start = chunk_column_index * new_row_width
-                        value_start = row_start + (row_index + 1) * (max_column_width + 1)
+                cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
+                row_start = chunk_column_index * new_row_width
+                # fw_handle[row_start:(row_start + len(column_name))] = column_name
+                fw_file.seek(row_start)
+                fw_file.write(column_name)
+
+            # Save values in transposed orientation.
+            for row_index in range(num_rows):
+                if row_index < 10 or (row_index < 100 and row_index % 10 == 0) or row_index % 100 == 0:
+                    print_message(f"Transposing {f4_src_file_path} to temporary file {tmp_fw_file_path} for row {row_index}.", verbose)
 
-                        fw_handle[value_start:(value_start + len(value))] = value
+                #FYI: Retrieving all values in a row is much faster than one at a time.
+                values = parse_row_values_function(src_file_data, "", row_index, all_column_coords)
 
-def transpose_chunk(f4_src_file_path, f4_dest_file_path, src_column_for_names_index, row_chunk_range, col_chunk_range, tsv_chunk_file_path, write_mode, verbose):
-    with initialize(f4_src_file_path) as src_file_data:
-        # with open_temp_file_to_compress(tsv_chunk_file_path, write_mode) as tsv_file:
-        with open(tsv_chunk_file_path, write_mode) as tsv_file:
-            if row_chunk_range[0] == 0:
-                cn_current, cn_end = advance_to_column_names(src_file_data, col_chunk_range[0])
-
-            for column_index in col_chunk_range:
-                #if len(col_chunk_range) < 100 or column_index % 100 == 0:
-                #print_message(f"Transposing {f4_src_file_path} to temporary file {tsv_chunk_file_path} for column {column_index} when transposing {f4_src_file_path} to {f4_dest_file_path}.", verbose)
-
-                if row_chunk_range[0] == 0:
-                    cn_current, column_name = get_next_column_name(src_file_data, cn_current, cn_end)
-                    values = [column_name]
-                else:
-                    values = []
-
-                if column_index == src_column_for_names_index:
-                    continue
+                for chunk_column_index, overall_column_index in enumerate(column_range):
+                    if overall_column_index == src_column_for_names_index:
+                        continue
 
-                column_coords = parse_data_coord(src_file_data, "", column_index)
-                parse_row_value_function = get_parse_row_value_function(src_file_data)
+                    value = values[chunk_column_index]
 
-                # TODO: Don't allow the values list to get too large (save in chunks).
-                for row_index in row_chunk_range:
-                    values.append(parse_row_value_function(src_file_data, "", row_index, column_coords))
+                    row_start = chunk_column_index * new_row_width
+                    value_start = row_start + (row_index + 1) * (max_column_width + 1)
 
-                tsv_file.write(b"\t".join(values) + b"\n")
+                    # fw_handle[value_start:(value_start + len(value))] = value
+                    fw_file.seek(value_start)
+                    fw_file.write(value)
 
 def advance_to_column_names(src_file_data, first_col_index):
     cn_current = src_file_data.file_map_dict["cn"][0]
     cn_end = src_file_data.file_map_dict["cn"][1]
 
     # Advance to the first column name for this chunk range.
     for column_index in range(first_col_index):
```

### Comparing `f4-0.9.4/src/f4/Utilities.py` & `f4-0.9.5/src/f4/Utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import sqlite3
 import sys
 from tempfile import mkdtemp
 from uuid import uuid4
 from zstandard import ZstdCompressor, ZstdDecompressor
 
 def get_current_version():
-    return "0.9.4"
+    return "0.9.5"
 
 #####################################################
 # Constants
 #####################################################
 
 def get_current_version_major():
     return get_current_version().split(".")[0]
```

### Comparing `f4-0.9.4/src/f4.egg-info/PKG-INFO` & `f4-0.9.5/src/f4.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f4
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Python package for the Fast Fixed-width File Format (F4)
 Home-page: https://github.com/srp33/f4py
 Author: Stephen R. Piccolo
 Author-email: stephen.piccolo.byu@gmail.com
 Project-URL: Docs, https://f4py.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `f4-0.9.4/test/test.py` & `f4-0.9.5/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -862,25 +862,25 @@
             num_lines += 1
 
     print(f"  {elapsed_time:.2f} seconds, {num_lines} lines in output file")
 
 run_all_small_tests()
 #sys.exit()
 
-#for compression_type in [None]:
+for compression_type in [None]:
 #for compression_type in ["zstd"]:
-for compression_type in [None, "zstd"]:
+#for compression_type in [None, "zstd"]:
     # Medium tests
 #    run_larger_tests(num_parallel=1, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
-    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
+#    run_larger_tests(num_parallel=2, size="medium", extension="", discrete1_index=11, numeric1_index=21, build_outputs=True, verbose=True, compression_type=compression_type, tmp_dir_path="/tmp/medium")
 
     # Large tests
-#    num_parallel = 1
+    num_parallel = 1
 #    num_parallel = 4
-    num_parallel = 16
+#    num_parallel = 16
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
 
-    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
+#    f4.transpose("data/medium.f4", "/tmp/medium_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
 #    f4.transpose("data/large_tall.f4", "/tmp/large_tall_transposed.f4", src_column_for_names="ID", num_parallel=num_parallel, verbose=verbose)
 
-    f4.inner_join("data/medium.f4", "data/medium.f4", "ID", "/tmp/medium_joined.f4", num_parallel=num_parallel, verbose=verbose)
+#    f4.inner_join("data/medium.f4", "data/medium.f4", "ID", "/tmp/medium_joined.f4", num_parallel=num_parallel, verbose=verbose)
 #    f4.inner_join("data/large_tall.f4", "data/large_wide.f4", "ID", "/tmp/large_joined.f4", num_parallel=num_parallel, verbose=verbose)
 
 print("All tests passed!!")
```

