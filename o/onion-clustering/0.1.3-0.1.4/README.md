# Comparing `tmp/onion_clustering-0.1.3.tar.gz` & `tmp/onion_clustering-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.1.3.tar", last modified: Fri Mar  8 09:31:11 2024, max compression
+gzip compressed data, was "onion_clustering-0.1.4.tar", last modified: Tue Apr 23 13:36:47 2024, max compression
```

## Comparing `onion_clustering-0.1.3.tar` & `onion_clustering-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.741135 onion_clustering-0.1.3/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-03-08 09:29:51.000000 onion_clustering-0.1.3/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       50 2024-02-16 13:11:19.000000 onion_clustering-0.1.3/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.1.3/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-03-08 09:31:11.740388 onion_clustering-0.1.3/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-02-26 12:16:27.000000 onion_clustering-0.1.3/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.724850 onion_clustering-0.1.3/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3663 2024-02-28 14:02:24.000000 onion_clustering-0.1.3/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3668 2024-02-28 14:02:24.000000 onion_clustering-0.1.3/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      635 2024-02-26 12:16:27.000000 onion_clustering-0.1.3/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      942 2024-03-08 09:29:53.000000 onion_clustering-0.1.3/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.1.3/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-03-08 09:31:11.741414 onion_clustering-0.1.3/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.720292 onion_clustering-0.1.3/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.729897 onion_clustering-0.1.3/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.1.3/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      465 2024-02-26 12:16:27.000000 onion_clustering-0.1.3/src/onion_clustering/__version__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    34308 2024-03-08 09:18:52.000000 onion_clustering-0.1.3/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    19430 2024-03-08 09:20:38.000000 onion_clustering-0.1.3/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23149 2024-03-08 09:26:40.000000 onion_clustering-0.1.3/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    17171 2024-03-08 09:21:04.000000 onion_clustering-0.1.3/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23147 2024-02-28 14:02:24.000000 onion_clustering-0.1.3/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-02-26 12:16:27.000000 onion_clustering-0.1.3/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.739416 onion_clustering-0.1.3/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-03-08 09:31:11.000000 onion_clustering-0.1.3/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      878 2024-03-08 09:31:11.000000 onion_clustering-0.1.3/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-03-08 09:31:11.000000 onion_clustering-0.1.3/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-03-08 09:31:11.000000 onion_clustering-0.1.3/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-03-08 09:31:11.000000 onion_clustering-0.1.3/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.734548 onion_clustering-0.1.3/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.1.3/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.736948 onion_clustering-0.1.3/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-02-16 13:11:19.000000 onion_clustering-0.1.3/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-02-16 13:11:19.000000 onion_clustering-0.1.3/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-02-16 13:11:19.000000 onion_clustering-0.1.3/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-03-08 09:31:11.738771 onion_clustering-0.1.3/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      265 2024-03-07 15:16:22.000000 onion_clustering-0.1.3/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-03-07 15:16:22.000000 onion_clustering-0.1.3/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-03-07 15:06:33.000000 onion_clustering-0.1.3/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3304 2024-02-28 14:02:24.000000 onion_clustering-0.1.3/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3238 2024-03-07 15:07:12.000000 onion_clustering-0.1.3/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.651843 onion_clustering-0.1.4/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/.coverage
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       50 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.1.4/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-23 13:36:47.650762 onion_clustering-0.1.4/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.621250 onion_clustering-0.1.4/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3664 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      635 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      942 2024-04-23 13:36:22.000000 onion_clustering-0.1.4/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.1.4/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-04-23 13:36:47.652041 onion_clustering-0.1.4/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.608999 onion_clustering-0.1.4/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.630698 onion_clustering-0.1.4/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      465 2024-02-26 12:16:27.000000 onion_clustering-0.1.4/src/onion_clustering/__version__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    34309 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    19431 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23224 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    17172 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23148 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.649444 onion_clustering-0.1.4/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      878 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.639323 onion_clustering-0.1.4/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.1.4/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.643144 onion_clustering-0.1.4/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.648433 onion_clustering-0.1.4/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      265 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3361 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3271 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/test_uni.py
```

### Comparing `onion_clustering-0.1.3/.coverage` & `onion_clustering-0.1.4/.coverage`

 * *Files 14% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -46,19 +46,19 @@
     context_id integer,         -- foreign key to `context`.
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
 INSERT INTO line_bits VALUES(1,1,X'02');
-INSERT INTO line_bits VALUES(2,1,X'e2bd0326b8f901943f00000070f4e4c90040b777fbaef23b300060d7ebadf23bb0dc10fefcbefef77b030000000000000000000000e40f0048f7cd27ef71c801c8f9fcc2da9e3e0700bb156c5a4e2301e3fffb7d9600de25');
-INSERT INTO line_bits VALUES(3,1,X'b2bf40d92f224b9edfdb15e814a751317efc269fccf22960110100000000205c00000080dc3d3fef3e56fcfcc8c72d13e4fdfe499e1fe3e7e57f7e9e77bfdf8f6f6952b2fde36605b8ddf5e7c7ffdfdf1f03000058000bf2fefd4ffc0500000000000000000000000098dffbf73ffffefbf71f7fd932cbcffee306');
-INSERT INTO line_bits VALUES(4,1,X'b22f010060fc2e60c62f20e33104e005042c000040e05b2020808dc33673bfc7cffffdbe8c8701189f05082cf07b0200018130db4c7efef7653cf0ffbebfef4600aff8ff2f');
-INSERT INTO line_bits VALUES(5,1,X'd24b18940000080c2000a07db504004e0000dab77200001eff010000609eeb5ffc3c01801c0000248fc51200e06ff8033e0080bffc07c0f16f7e3e0ebbb720c0ff910300108f1cfe27ff5d79fef98d8ff3dd02');
-INSERT INTO line_bits VALUES(6,1,X'e2dd014c7086fc00ca0100b0ffefdbdf3f0000700098e7c3fc3c7e1ecf0dfb5ebd3fcb0f00e4eee693f738e400c0f97c61dd7b0e00769b60362da79904ccfff7fb4c00ef12');
+INSERT INTO line_bits VALUES(2,1,X'c27b074c70f303287f000000e0e8c99301806eeff65de5776000c0aed75be57760b921fcf97dfdeff7060000000000000000000000c81f0090ee9b4fdee3900390f3f985b53d7d0e00762bd8b49c4602c6fff7fb2c01bc4b');
+INSERT INTO line_bits VALUES(3,1,X'627f81b25f44963cbfb72bd0294ea362fcf84d3e99e553c022020000000040b800000000b97b7ede7dacf8f9918f5b26c8fbfd933c3fc6cfcbfffc3cef7ebf1fdfd2a464fbc7cd0a70bbebcf8fffbfbf3f060000b00016e4fdfb9ff80b00000000000000000000000030bff7ef7ffefdf7ef3ffeb265969ffdc70d');
+INSERT INTO line_bits VALUES(4,1,X'625f0200c0f85dc08c5f40c66308c00b0858000080c0b74040001b876de67e8f9ffffb7d190f03303e0b1058e0f70400020261b699fcfcefcb78e0ff7d7fdf8d005ef1ff5f');
+INSERT INTO line_bits VALUES(5,1,X'a297302801001018400040fb6a09009c0000b46fe500003cfe030000c03cd7bff8790200390000481e8b2500c0dff0077c00007ff90f80e37df3f371d8bd0501fe8f1c008078e4f03ff9efcaf3cf6f7c9cef16');
+INSERT INTO line_bits VALUES(6,1,X'c2bb0398e00cf90194030060ffdfb7bf7f0000e00030cf87f979fc3c9e1bf6bd7a7f961f00c8ddcd27ef71c80180f3f9c2baf71c00ec36c16c5a4e330998ffeff79900de25');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `onion_clustering-0.1.3/LICENSE` & `onion_clustering-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.3/PKG-INFO` & `onion_clustering-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.1.3
+Version: 0.1.4
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.1.3/README.md` & `onion_clustering-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.3/examples/example_script.py` & `onion_clustering-0.1.4/examples/example_script.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Example script for running onion_clustering
 """
+
 import os
 import shutil
 from pathlib import Path
 
 from onion_clustering import main
 
 ##############################################################################
```

### Comparing `onion_clustering-0.1.3/examples/example_script_2d.py` & `onion_clustering-0.1.4/examples/example_script_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Example script for running onion_clustering
 """
+
 import os
 import shutil
 from pathlib import Path
 
 from onion_clustering import main_2d
 
 ##############################################################################
```

### Comparing `onion_clustering-0.1.3/justfile` & `onion_clustering-0.1.4/justfile`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.3/pyproject.toml` & `onion_clustering-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.1.3"
+version = "0.1.4"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
```

### Comparing `onion_clustering-0.1.3/src/onion_clustering/classes.py` & `onion_clustering-0.1.4/src/onion_clustering/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains the classes used for storing the clustering data.
 """
+
 import os
 from typing import List, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import plotly.graph_objects as go
 from matplotlib.colors import rgb2hex
```

### Comparing `onion_clustering-0.1.3/src/onion_clustering/first_classes.py` & `onion_clustering-0.1.4/src/onion_clustering/first_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains the classes used for storing parameters and system states.
 """
+
 import copy
 from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.signal
 from matplotlib.colors import rgb2hex
```

### Comparing `onion_clustering-0.1.3/src/onion_clustering/functions.py` & `onion_clustering-0.1.4/src/onion_clustering/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Should contains all the functions in common between the 2 codes.
 """
+
 from typing import List, Tuple
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.optimize
 import scipy.signal
 
@@ -440,27 +441,29 @@
             if elem[1] == pair[0]:
                 best_merge[j][1] = pair[1]
 
     # Relabel the labels in all_the_labels
     relabel_dic = {}
     for pair in best_merge:
         relabel_dic[pair[0]] = pair[1]
+    if_env0 = np.any(np.unique(all_the_labels) == 0)
+
     relabel_map = np.zeros(max(np.unique(all_the_labels) + 1), dtype=int)
     for i, _ in enumerate(relabel_map):
         relabel_map[i] = i
     for key, value in relabel_dic.items():
         relabel_map[key + 1] = value + 1
 
     all_the_labels = relabel_map[all_the_labels.flatten()].reshape(
         all_the_labels.shape
     )
 
     final_map = np.zeros(max(np.unique(all_the_labels)) + 1, dtype=int)
     for i, el in enumerate(np.unique(all_the_labels)):
-        final_map[el] = i
+        final_map[el] = i + 1 * (1 - if_env0)
     for i, particle in enumerate(all_the_labels):
         for j, el in enumerate(particle):
             all_the_labels[i][j] = final_map[el]
 
     # Remove merged states from the state list
     states_to_remove = set(s0 for s0, s1 in best_merge)
     updated_states = [
```

### Comparing `onion_clustering-0.1.3/src/onion_clustering/main.py` & `onion_clustering-0.1.4/src/onion_clustering/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Code for clustering of univariate time-series data.
 See the documentation for all the details.
 """
+
 import copy
 import os
 import shutil
 from typing import List, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
```

### Comparing `onion_clustering-0.1.3/src/onion_clustering/main_2d.py` & `onion_clustering-0.1.4/src/onion_clustering/main_2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Code for clustering of multivariate (2- or 3-dimensional) time-series data.
 See the documentation for all the details.
 """
+
 import copy
 import os
 import shutil
 from typing import List, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
```

### Comparing `onion_clustering-0.1.3/src/onion_clustering/utilities.py` & `onion_clustering-0.1.4/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.3/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.1.4/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.1.3
+Version: 0.1.4
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.1.3/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.1.4/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.3/test/test_multi.py` & `onion_clustering-0.1.4/test/test_uni.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 import pytest
-from onion_clustering import main_2d
+from onion_clustering import main
 
 
 # Define a fixture to set up the test environment
 @pytest.fixture
 def setup_test_environment(tmpdir):
     # tmpdir is a built-in pytest fixture providing a temporary directory
     original_dir = os.getcwd()  # Save the current working directory
@@ -15,39 +15,40 @@
         original_dir
     )  # Restore the original working directory after the test
 
 
 # Define the actual test
 def test_output_files(setup_test_environment):
     ### Set all the analysis parameters ###
-    PATH_TO_INPUT_DATA = "/Users/mattebecchi/00_signal_analysis/synthetic_2D/3D_synthetic_data.npy"
+    FILE = "water_coex_100ps_1nm_LENS.npy"
+    PATH_TO_INPUT_DATA = "/Users/mattebecchi/00_signal_analysis/data/" + FILE
     TAU_WINDOW = 10  # time resolution of the analysis
-    T_CONV = 200  # convert frames in time units (default 1)
-    T_UNITS = "dt"  # the time units (default 'frames')
-    NUM_TAU_W = 2  # number of tau_window tested (default 20)
-    MAX_TAU_W = 10  # max value of tau_window tested (default auto)
+    T_DELAY = 1  # remove the first t_delay frames (default 0)
+    T_CONV = 0.1  # convert frames in time units (default 1)
+    T_UNITS = "ns"  # the time units (default 'frames')
+    NUM_TAU_W = 2
+    MAX_TAU_W = 10
     MAX_T_SMOOTH = 2  # max value of t_smooth tested (default 5)
-    BINS = 50  # number of histogram bins (default auto)
 
     ### Create the 'data_directory.txt' file ###
     with open("data_directory.txt", "w+", encoding="utf-8") as file:
         print(PATH_TO_INPUT_DATA, file=file)
 
     ### Create the 'input_parameter.txt' file ###
     with open("input_parameters.txt", "w+", encoding="utf-8") as file:
         print("tau_window\t" + str(TAU_WINDOW), file=file)
+        print("t_delay\t" + str(T_DELAY), file=file)
         print("t_conv\t" + str(T_CONV), file=file)
         print("t_units\t" + T_UNITS, file=file)
         print("num_tau_w\t" + str(NUM_TAU_W), file=file)
         print("max_tau_w\t" + str(MAX_TAU_W), file=file)
         print("max_t_smooth\t" + str(MAX_T_SMOOTH), file=file)
-        print("bins\t" + str(BINS), file=file)
 
     # Call your code to generate the output files
-    tmp = main_2d.main()
+    tmp = main.main()
 
     # Test the output
     tmp.plot_tra_figure()
     tmp.plot_input_data("Fig0")
     tmp.plot_cumulative_figure()
     tmp.plot_one_trajectory()
     tmp.data.plot_medoids()
@@ -55,27 +56,31 @@
     tmp.sankey([0, 10, 20, 30, 40])
     tmp.print_labels()
 
     # Define the paths to the expected and actual output files
     original_dir = (
         "/Users/mattebecchi/00_signal_analysis/timeseries_analysis/test/"
     )
-    expected_output_path_1 = original_dir + "output_multi/final_states.txt"
-    expected_output_path_2 = original_dir + "output_multi/number_of_states.txt"
-    expected_output_path_3 = original_dir + "output_multi/fraction_0.txt"
+    expected_output_path_1 = original_dir + "output_uni/final_states.txt"
+    expected_output_path_2 = original_dir + "output_uni/number_of_states.txt"
+    expected_output_path_3 = original_dir + "output_uni/fraction_0.txt"
     actual_output_path_1 = "final_states.txt"
     actual_output_path_2 = "number_of_states.txt"
     actual_output_path_3 = "fraction_0.txt"
 
-    # Use filecmp to compare the contents of the expected and actual output directories
-    with open(expected_output_path_1, "r") as expected_file, open(
-        actual_output_path_1, "r"
-    ) as actual_file:
+    # Use filecmp to compare the contents of the expected
+    # and actual output directories
+    with (
+        open(expected_output_path_1, "r") as expected_file,
+        open(actual_output_path_1, "r") as actual_file,
+    ):
         assert expected_file.read() == actual_file.read()
-    with open(expected_output_path_2, "r") as expected_file, open(
-        actual_output_path_2, "r"
-    ) as actual_file:
+    with (
+        open(expected_output_path_2, "r") as expected_file,
+        open(actual_output_path_2, "r") as actual_file,
+    ):
         assert expected_file.read() == actual_file.read()
-    with open(expected_output_path_3, "r") as expected_file, open(
-        actual_output_path_3, "r"
-    ) as actual_file:
+    with (
+        open(expected_output_path_3, "r") as expected_file,
+        open(actual_output_path_3, "r") as actual_file,
+    ):
         assert expected_file.read() == actual_file.read()
```

### Comparing `onion_clustering-0.1.3/test/test_uni.py` & `onion_clustering-0.1.4/test/test_multi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 import pytest
-from onion_clustering import main
+from onion_clustering import main_2d
 
 
 # Define a fixture to set up the test environment
 @pytest.fixture
 def setup_test_environment(tmpdir):
     # tmpdir is a built-in pytest fixture providing a temporary directory
     original_dir = os.getcwd()  # Save the current working directory
@@ -15,40 +15,40 @@
         original_dir
     )  # Restore the original working directory after the test
 
 
 # Define the actual test
 def test_output_files(setup_test_environment):
     ### Set all the analysis parameters ###
-    FILE = "water_coex_100ps_1nm_LENS.npy"
-    PATH_TO_INPUT_DATA = "/Users/mattebecchi/00_signal_analysis/data/" + FILE
+    PATH_TO_INPUT_DATA = ("/Users/mattebecchi/00_signal_analysis/data/"
+        "synthetic_2D/3D_synthetic_data.npy")
     TAU_WINDOW = 10  # time resolution of the analysis
-    T_DELAY = 1  # remove the first t_delay frames (default 0)
-    T_CONV = 0.1  # convert frames in time units (default 1)
-    T_UNITS = "ns"  # the time units (default 'frames')
-    NUM_TAU_W = 2
-    MAX_TAU_W = 10
+    T_CONV = 200  # convert frames in time units (default 1)
+    T_UNITS = "dt"  # the time units (default 'frames')
+    NUM_TAU_W = 2  # number of tau_window tested (default 20)
+    MAX_TAU_W = 10  # max value of tau_window tested (default auto)
     MAX_T_SMOOTH = 2  # max value of t_smooth tested (default 5)
+    BINS = 50  # number of histogram bins (default auto)
 
     ### Create the 'data_directory.txt' file ###
     with open("data_directory.txt", "w+", encoding="utf-8") as file:
         print(PATH_TO_INPUT_DATA, file=file)
 
     ### Create the 'input_parameter.txt' file ###
     with open("input_parameters.txt", "w+", encoding="utf-8") as file:
         print("tau_window\t" + str(TAU_WINDOW), file=file)
-        print("t_delay\t" + str(T_DELAY), file=file)
         print("t_conv\t" + str(T_CONV), file=file)
         print("t_units\t" + T_UNITS, file=file)
         print("num_tau_w\t" + str(NUM_TAU_W), file=file)
         print("max_tau_w\t" + str(MAX_TAU_W), file=file)
         print("max_t_smooth\t" + str(MAX_T_SMOOTH), file=file)
+        print("bins\t" + str(BINS), file=file)
 
     # Call your code to generate the output files
-    tmp = main.main()
+    tmp = main_2d.main()
 
     # Test the output
     tmp.plot_tra_figure()
     tmp.plot_input_data("Fig0")
     tmp.plot_cumulative_figure()
     tmp.plot_one_trajectory()
     tmp.data.plot_medoids()
@@ -56,28 +56,31 @@
     tmp.sankey([0, 10, 20, 30, 40])
     tmp.print_labels()
 
     # Define the paths to the expected and actual output files
     original_dir = (
         "/Users/mattebecchi/00_signal_analysis/timeseries_analysis/test/"
     )
-    expected_output_path_1 = original_dir + "output_uni/final_states.txt"
-    expected_output_path_2 = original_dir + "output_uni/number_of_states.txt"
-    expected_output_path_3 = original_dir + "output_uni/fraction_0.txt"
+    expected_output_path_1 = original_dir + "output_multi/final_states.txt"
+    expected_output_path_2 = original_dir + "output_multi/number_of_states.txt"
+    expected_output_path_3 = original_dir + "output_multi/fraction_0.txt"
     actual_output_path_1 = "final_states.txt"
     actual_output_path_2 = "number_of_states.txt"
     actual_output_path_3 = "fraction_0.txt"
 
-    # Use filecmp to compare the contents of the expected
-    # and actual output directories
-    with open(expected_output_path_1, "r") as expected_file, open(
-        actual_output_path_1, "r"
-    ) as actual_file:
+    # Use filecmp to compare the contents of the expected and actual
+    # output directories
+    with (
+        open(expected_output_path_1, "r") as expected_file,
+        open(actual_output_path_1, "r") as actual_file,
+    ):
         assert expected_file.read() == actual_file.read()
-    with open(expected_output_path_2, "r") as expected_file, open(
-        actual_output_path_2, "r"
-    ) as actual_file:
+    with (
+        open(expected_output_path_2, "r") as expected_file,
+        open(actual_output_path_2, "r") as actual_file,
+    ):
         assert expected_file.read() == actual_file.read()
-    with open(expected_output_path_3, "r") as expected_file, open(
-        actual_output_path_3, "r"
-    ) as actual_file:
+    with (
+        open(expected_output_path_3, "r") as expected_file,
+        open(actual_output_path_3, "r") as actual_file,
+    ):
         assert expected_file.read() == actual_file.read()
```

