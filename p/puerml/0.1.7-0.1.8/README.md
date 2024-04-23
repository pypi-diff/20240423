# Comparing `tmp/puerml-0.1.7.tar.gz` & `tmp/puerml-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puerml-0.1.7.tar", last modified: Mon Apr 22 10:31:18 2024, max compression
+gzip compressed data, was "puerml-0.1.8.tar", last modified: Tue Apr 23 13:09:40 2024, max compression
```

## Comparing `puerml-0.1.7.tar` & `puerml-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 10:31:18.888705 puerml-0.1.7/
--rw-r--r--   0 Alexander   (502) staff       (20)     1070 2024-04-22 09:02:31.000000 puerml-0.1.7/LICENSE
--rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-22 10:31:18.888354 puerml-0.1.7/PKG-INFO
--rw-r--r--   0 Alexander   (502) staff       (20)        4 2024-04-22 09:02:31.000000 puerml-0.1.7/README.md
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 10:31:18.883562 puerml-0.1.7/puerml/
--rw-r--r--   0 Alexander   (502) staff       (20)       51 2024-04-22 09:37:20.000000 puerml-0.1.7/puerml/__init__.py
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 10:31:18.887804 puerml-0.1.7/puerml/library/
--rw-r--r--   0 Alexander   (502) staff       (20)      144 2024-04-22 09:37:20.000000 puerml-0.1.7/puerml/library/__init__.py
--rw-r--r--   0 Alexander   (502) staff       (20)      850 2024-04-22 09:10:49.000000 puerml-0.1.7/puerml/library/benchmark.py
--rw-r--r--   0 Alexander   (502) staff       (20)     8390 2024-04-22 09:10:49.000000 puerml-0.1.7/puerml/library/data_frame.py
--rw-r--r--   0 Alexander   (502) staff       (20)     2419 2024-04-22 10:31:04.000000 puerml-0.1.7/puerml/library/jsonl.py
-drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-22 10:31:18.885416 puerml-0.1.7/puerml.egg-info/
--rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-22 10:31:18.000000 puerml-0.1.7/puerml.egg-info/PKG-INFO
--rw-r--r--   0 Alexander   (502) staff       (20)      273 2024-04-22 10:31:18.000000 puerml-0.1.7/puerml.egg-info/SOURCES.txt
--rw-r--r--   0 Alexander   (502) staff       (20)        1 2024-04-22 10:31:18.000000 puerml-0.1.7/puerml.egg-info/dependency_links.txt
--rw-r--r--   0 Alexander   (502) staff       (20)        7 2024-04-22 10:31:18.000000 puerml-0.1.7/puerml.egg-info/top_level.txt
--rw-r--r--   0 Alexander   (502) staff       (20)       38 2024-04-22 10:31:18.888866 puerml-0.1.7/setup.cfg
--rw-r--r--   0 Alexander   (502) staff       (20)      149 2024-04-22 10:31:18.000000 puerml-0.1.7/setup.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.546100 puerml-0.1.8/
+-rw-r--r--   0 Alexander   (502) staff       (20)     1070 2024-04-22 09:02:31.000000 puerml-0.1.8/LICENSE
+-rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-23 13:09:40.545655 puerml-0.1.8/PKG-INFO
+-rw-r--r--   0 Alexander   (502) staff       (20)        4 2024-04-22 09:02:31.000000 puerml-0.1.8/README.md
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.534250 puerml-0.1.8/puerml/
+-rw-r--r--   0 Alexander   (502) staff       (20)       51 2024-04-22 09:37:20.000000 puerml-0.1.8/puerml/__init__.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.543258 puerml-0.1.8/puerml/library/
+-rw-r--r--   0 Alexander   (502) staff       (20)      179 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/__init__.py
+-rw-r--r--   0 Alexander   (502) staff       (20)      850 2024-04-22 09:10:49.000000 puerml-0.1.8/puerml/library/benchmark.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     8390 2024-04-22 09:10:49.000000 puerml-0.1.8/puerml/library/data_frame.py
+-rw-r--r--   0 Alexander   (502) staff       (20)      655 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/decorators.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     2217 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/git.py
+-rw-r--r--   0 Alexander   (502) staff       (20)     2318 2024-04-23 12:52:56.000000 puerml-0.1.8/puerml/library/jsonl.py
+drwxr-xr-x   0 Alexander   (502) staff       (20)        0 2024-04-23 13:09:40.536937 puerml-0.1.8/puerml.egg-info/
+-rw-r--r--   0 Alexander   (502) staff       (20)      153 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/PKG-INFO
+-rw-r--r--   0 Alexander   (502) staff       (20)      324 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/SOURCES.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)        1 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/dependency_links.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)        7 2024-04-23 13:09:40.000000 puerml-0.1.8/puerml.egg-info/top_level.txt
+-rw-r--r--   0 Alexander   (502) staff       (20)       38 2024-04-23 13:09:40.546254 puerml-0.1.8/setup.cfg
+-rw-r--r--   0 Alexander   (502) staff       (20)      149 2024-04-23 13:09:39.000000 puerml-0.1.8/setup.py
```

### Comparing `puerml-0.1.7/LICENSE` & `puerml-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `puerml-0.1.7/puerml/library/benchmark.py` & `puerml-0.1.8/puerml/library/benchmark.py`

 * *Files identical despite different names*

### Comparing `puerml-0.1.7/puerml/library/data_frame.py` & `puerml-0.1.8/puerml/library/data_frame.py`

 * *Files identical despite different names*

### Comparing `puerml-0.1.7/puerml/library/jsonl.py` & `puerml-0.1.8/puerml/library/jsonl.py`

 * *Files 13% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 			file         = open(file_path, 'w')
 			current_size = 0
 			chunk_num += 1
 
 		open_new_file()
 
 		for item in data:
-			jsonl_line = json.dumps(cls._escape(item)) + '\n'
+			jsonl_line = cls.encode(item) + '\n'
 			line_size  = len(jsonl_line.encode('utf-8'))
 			if max_file_size and current_size + line_size > max_file_size:
 				open_new_file()
 			file.write(jsonl_line)
 			current_size += line_size
 
 		if file:
@@ -59,27 +59,26 @@
 	def load_all(cls, name, file_dir):
 		'Load all records at once'
 		all = []
 		files = sorted([os.path.join(file_dir, f) for f in os.listdir(file_dir) if f.startswith(name) and f.endswith('.jsonl')])
 		for file_path in files:
 			with open(file_path, 'r') as file:
 				for line in file:
-					all.append(cls._unescape(json.loads(line.strip())))
-
+					all.append(cls.decode(line))
 		return all
 
 	@classmethod
-	def load(cls, name, file_dir, batch_size=None):
+	def load(cls, name, file_dir):
 		'Generator to read jsonl files in batches'
-		if batch_size is None:
-			return Jsonl.load_all(name, file_dir)
 		files = sorted([os.path.join(file_dir, f) for f in os.listdir(file_dir) if f.startswith(name) and f.endswith('.jsonl')])
 		for file_path in files:
 			with open(file_path, 'r') as file:
-				batch = []
 				for line in file:
-					batch.append(cls._unescape(json.loads(line.strip())))
-					if len(batch) == batch_size:
-						yield batch
-						batch = []
-				if batch:
-					yield batch
+					yield cls.decode(line)
+
+	@classmethod
+	def encode(cls, item):
+		return json.dumps(cls._escape(item))
+
+	@classmethod
+	def decode(cls, line):
+		return cls._unescape(json.loads(line.strip()))
```

