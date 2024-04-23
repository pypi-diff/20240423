# Comparing `tmp/nodespecs-0.0.5.tar.gz` & `tmp/nodespecs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodespecs-0.0.5.tar", last modified: Thu Apr 18 21:08:36 2024, max compression
+gzip compressed data, was "nodespecs-0.0.6.tar", last modified: Tue Apr 23 13:38:25 2024, max compression
```

## Comparing `nodespecs-0.0.5.tar` & `nodespecs-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.093700 nodespecs-0.0.5/
--rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5854 2024-04-18 21:08:36.091010 nodespecs-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3973 2024-04-18 20:55:37.000000 nodespecs-0.0.5/README.md
--rw-rw-rw-   0        0        0      899 2024-04-18 21:07:43.000000 nodespecs-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 21:08:36.094153 nodespecs-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.055012 nodespecs-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.089013 nodespecs-0.0.5/src/nodespecs.egg-info/
--rw-rw-rw-   0        0        0     5854 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 21:08:36.000000 nodespecs-0.0.5/src/nodespecs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 21:08:36.087014 nodespecs-0.0.5/src/specs/
--rw-rw-rw-   0        0        0       91 2024-04-18 21:06:53.000000 nodespecs-0.0.5/src/specs/__init__.py
--rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.5/src/specs/__main__.py
--rw-rw-rw-   0        0        0      172 2024-04-18 19:56:34.000000 nodespecs-0.0.5/src/specs/cmd.py
--rw-rw-rw-   0        0        0     1400 2024-04-12 15:15:38.000000 nodespecs-0.0.5/src/specs/cpu-benchmark.py
--rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.5/src/specs/cpuinfo.py
--rw-rw-rw-   0        0        0     7189 2024-04-12 22:25:26.000000 nodespecs-0.0.5/src/specs/hardware.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.835840 nodespecs-0.0.6/
+-rw-rw-rw-   0        0        0     1098 2024-04-13 00:06:04.000000 nodespecs-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     6207 2024-04-23 13:38:25.832850 nodespecs-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4326 2024-04-23 13:35:19.000000 nodespecs-0.0.6/README.md
+-rw-rw-rw-   0        0        0      899 2024-04-23 13:30:54.000000 nodespecs-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:38:25.835840 nodespecs-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.786956 nodespecs-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.830858 nodespecs-0.0.6/src/nodespecs.egg-info/
+-rw-rw-rw-   0        0        0     6207 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-23 13:38:25.000000 nodespecs-0.0.6/src/nodespecs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 13:38:25.824559 nodespecs-0.0.6/src/specs/
+-rw-rw-rw-   0        0        0      125 2024-04-23 13:35:20.000000 nodespecs-0.0.6/src/specs/__init__.py
+-rw-rw-rw-   0        0        0      271 2024-04-18 19:09:52.000000 nodespecs-0.0.6/src/specs/__main__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-23 13:35:21.000000 nodespecs-0.0.6/src/specs/benchmark.py
+-rw-rw-rw-   0        0        0      172 2024-04-18 19:56:34.000000 nodespecs-0.0.6/src/specs/cmd.py
+-rw-rw-rw-   0        0        0    86524 2024-04-12 15:14:05.000000 nodespecs-0.0.6/src/specs/cpuinfo.py
+-rw-rw-rw-   0        0        0     7189 2024-04-19 22:18:04.000000 nodespecs-0.0.6/src/specs/hardware.py
```

### Comparing `nodespecs-0.0.5/LICENSE` & `nodespecs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.5/PKG-INFO` & `nodespecs-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.5
+Version: 0.0.6
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -39,14 +39,21 @@
 ```
 
 ```
 sudo apt install python3-pip
 python3 -m pip install nodespecs && python3 -m specs
 ```
 
+```python
+import specs
+
+specs.info_gpu()
+specs.bench_cpu()
+```
+
 
 
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
@@ -83,17 +90,24 @@
 
 
 
 ### GPU collection
 
 
 
-| id    | name                   | total memory | Synthetic benchmark | CUDA API |
-| ----- | ---------------------- | ------------ | ------------------- | -------- |
-| colab | Tesla T4               | 15360.0MB    | 28.16               | 70627    |
-| dell  | NVIDIA T600 Laptop GPU | 4096.0MB     | 16.69               | 26600    |
+| id    | name                    | total memory | Synthetic benchmark | CUDA API |
+| ----- | ----------------------- | ------------ | ------------------- | -------- |
+| 17    | NVIDIA GeForce RTX 4060 | 8188.0MB     | 50.69               | NA       |
+| colab | Tesla T4                | 15360.0MB    | 28.16               | 70627    |
+| dell  | NVIDIA T600 Laptop GPU  | 4096.0MB     | 16.69               | 26600    |
+| 01    | Quadro M4000            | 8192.0MB     | 17.27               | 16648    |
+
+
 
 
 
 Performance source
 
+* https://browser.geekbench.com/
+  * 
+* https://technical.city/en/video/GeForce-RTX-4060-vs-Tesla-T4
 * https://technical.city/en/video/Tesla-T4-vs-T600
```

### Comparing `nodespecs-0.0.5/README.md` & `nodespecs-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 ```
 
 ```
 sudo apt install python3-pip
 python3 -m pip install nodespecs && python3 -m specs
 ```
 
+```python
+import specs
+
+specs.info_gpu()
+specs.bench_cpu()
+```
+
 
 
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
@@ -55,17 +62,24 @@
 
 
 
 ### GPU collection
 
 
 
-| id    | name                   | total memory | Synthetic benchmark | CUDA API |
-| ----- | ---------------------- | ------------ | ------------------- | -------- |
-| colab | Tesla T4               | 15360.0MB    | 28.16               | 70627    |
-| dell  | NVIDIA T600 Laptop GPU | 4096.0MB     | 16.69               | 26600    |
+| id    | name                    | total memory | Synthetic benchmark | CUDA API |
+| ----- | ----------------------- | ------------ | ------------------- | -------- |
+| 17    | NVIDIA GeForce RTX 4060 | 8188.0MB     | 50.69               | NA       |
+| colab | Tesla T4                | 15360.0MB    | 28.16               | 70627    |
+| dell  | NVIDIA T600 Laptop GPU  | 4096.0MB     | 16.69               | 26600    |
+| 01    | Quadro M4000            | 8192.0MB     | 17.27               | 16648    |
+
+
 
 
 
 Performance source
 
+* https://browser.geekbench.com/
+  * 
+* https://technical.city/en/video/GeForce-RTX-4060-vs-Tesla-T4
 * https://technical.city/en/video/Tesla-T4-vs-T600
```

### Comparing `nodespecs-0.0.5/pyproject.toml` & `nodespecs-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nodespecs"
-version = "0.0.5"
+version = "0.0.6"
 description = "The specs summarize utilities for computer instance"
 readme = "README.md"
 authors = [{ name = "jinsanity", email = "jinsanityff@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `nodespecs-0.0.5/src/nodespecs.egg-info/PKG-INFO` & `nodespecs-0.0.6/src/nodespecs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodespecs
-Version: 0.0.5
+Version: 0.0.6
 Summary: The specs summarize utilities for computer instance
 Author-email: jinsanity <jinsanityff@gmail.com>
 License: The MIT License (MIT)
         Copyright © 2024 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -39,14 +39,21 @@
 ```
 
 ```
 sudo apt install python3-pip
 python3 -m pip install nodespecs && python3 -m specs
 ```
 
+```python
+import specs
+
+specs.info_gpu()
+specs.bench_cpu()
+```
+
 
 
 #### Deprecated  (install and use with git)
 
 ```
 !git clone https://github.com/jinsanity07git/hardwareSummary && python hardwareSummary/hardware.py && python hardwareSummary/cpu-benchmark.py
 
@@ -83,17 +90,24 @@
 
 
 
 ### GPU collection
 
 
 
-| id    | name                   | total memory | Synthetic benchmark | CUDA API |
-| ----- | ---------------------- | ------------ | ------------------- | -------- |
-| colab | Tesla T4               | 15360.0MB    | 28.16               | 70627    |
-| dell  | NVIDIA T600 Laptop GPU | 4096.0MB     | 16.69               | 26600    |
+| id    | name                    | total memory | Synthetic benchmark | CUDA API |
+| ----- | ----------------------- | ------------ | ------------------- | -------- |
+| 17    | NVIDIA GeForce RTX 4060 | 8188.0MB     | 50.69               | NA       |
+| colab | Tesla T4                | 15360.0MB    | 28.16               | 70627    |
+| dell  | NVIDIA T600 Laptop GPU  | 4096.0MB     | 16.69               | 26600    |
+| 01    | Quadro M4000            | 8192.0MB     | 17.27               | 16648    |
+
+
 
 
 
 Performance source
 
+* https://browser.geekbench.com/
+  * 
+* https://technical.city/en/video/GeForce-RTX-4060-vs-Tesla-T4
 * https://technical.city/en/video/Tesla-T4-vs-T600
```

### Comparing `nodespecs-0.0.5/src/specs/cpu-benchmark.py` & `nodespecs-0.0.6/src/specs/benchmark.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 #!/usr/bin/python3
 #Python CPU Benchmark by Alex Dedyura (Windows, macOS, Linux)
 #https://github.com/alexdedyura/cpu-benchmark
 
 import time
 import platform
-import cpuinfo
+from . import cpuinfo
 
-print('Python CPU Benchmark by Alex Dedyura (Windows, macOS(Darwin), Linux)')
-print('CPU: ' + cpuinfo.get_cpu_info().get('brand_raw', "Unknown"))
-print('Arch: ' + cpuinfo.get_cpu_info().get('arch_string_raw', "Unknown"))
-print('OS: ' + platform.system(), platform.release())
-print('Python: ' + platform.python_version())
+def bench_cpu():
+  print('Python CPU Benchmark by Alex Dedyura (Windows, macOS(Darwin), Linux)')
+  print('CPU: ' + cpuinfo.get_cpu_info().get('brand_raw', "Unknown"))
+  print('Arch: ' + cpuinfo.get_cpu_info().get('arch_string_raw', "Unknown"))
+  print('OS: ' + platform.system(), platform.release())
+  print('Python: ' + platform.python_version())
 
-print('\nBenchmarking: \n')
+  print('\nBenchmarking: \n')
 
-start_benchmark = 10000 # change this if you like (sample: 1000, 5000, etc)
-start_benchmark = int(start_benchmark)
+  start_benchmark = 10000 # change this if you like (sample: 1000, 5000, etc)
+  start_benchmark = int(start_benchmark)
 
-repeat_benchmark = 10 # attemps, change this if you like (sample: 3, 5, etc)
-repeat_benchmark = int(repeat_benchmark)
+  repeat_benchmark = 10 # attemps, change this if you like (sample: 3, 5, etc)
+  repeat_benchmark = int(repeat_benchmark)
 
-average_benchmark = 0
+  average_benchmark = 0
 
-for a in range(0,repeat_benchmark):
+  for a in range(0,repeat_benchmark):
 
-  start = time.perf_counter()
+    start = time.perf_counter()
 
-  for i in range(0,start_benchmark):
-    for x in range(1,1000):
-      3.141592 * 2**x
-    for x in range(1,10000):
-      float(x) / 3.141592
-    for x in range(1,10000):
-      float(3.141592) / x
+    for i in range(0,start_benchmark):
+      for x in range(1,1000):
+        3.141592 * 2**x
+      for x in range(1,10000):
+        float(x) / 3.141592
+      for x in range(1,10000):
+        float(3.141592) / x
 
-  end = time.perf_counter()
-  duration = (end - start)
-  duration = round(duration, 3)
-  average_benchmark += duration
-  print('Time: ' + str(duration) + 's')
+    end = time.perf_counter()
+    duration = (end - start)
+    duration = round(duration, 3)
+    average_benchmark += duration
+    print('Time: ' + str(duration) + 's')
 
-average_benchmark = round(average_benchmark / repeat_benchmark, 3)
-print('Average (from {} repeats): {}s'.format(repeat_benchmark, average_benchmark))
+  average_benchmark = round(average_benchmark / repeat_benchmark, 3)
+  print('Average (from {} repeats): {}s'.format(repeat_benchmark, average_benchmark))
```

### Comparing `nodespecs-0.0.5/src/specs/cpuinfo.py` & `nodespecs-0.0.6/src/specs/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `nodespecs-0.0.5/src/specs/hardware.py` & `nodespecs-0.0.6/src/specs/hardware.py`

 * *Files identical despite different names*

