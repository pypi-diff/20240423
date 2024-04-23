# Comparing `tmp/bruker_utils-0.0.1.tar.gz` & `tmp/bruker_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bruker_utils-0.0.1.tar", last modified: Wed Sep 15 23:41:37 2021, max compression
+gzip compressed data, was "bruker_utils-0.0.2.tar", last modified: Tue Apr 23 17:44:17 2024, max compression
```

## Comparing `bruker_utils-0.0.1.tar` & `bruker_utils-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/
--rw-rw-r--   0 simon     (1000) simon     (1000)       38 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/setup.cfg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1174 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      525 2021-09-15 22:23:38.000000 bruker_utils-0.0.1/README.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)      845 2021-09-15 22:23:39.000000 bruker_utils-0.0.1/setup.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/bruker_utils/
--rw-rw-r--   0 simon     (1000) simon     (1000)       22 2021-09-15 22:23:38.000000 bruker_utils-0.0.1/bruker_utils/_version.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    23778 2021-09-15 22:23:38.000000 bruker_utils-0.0.1/bruker_utils/__init__.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/bruker_utils.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/bruker_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       13 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/bruker_utils.egg-info/top_level.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)      248 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/bruker_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)     1174 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/bruker_utils.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)        6 2021-09-15 23:41:37.000000 bruker_utils-0.0.1/bruker_utils.egg-info/requires.txt
+drwxrwxr-x   0 simonhulse  (1006) simonhulse  (1007)        0 2024-04-23 17:44:17.015277 bruker_utils-0.0.2/
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)     1063 2024-04-23 17:26:52.000000 bruker_utils-0.0.2/LICENSE
+-rw-r--r--   0 simonhulse  (1006) simonhulse  (1007)     1057 2024-04-23 17:44:17.015277 bruker_utils-0.0.2/PKG-INFO
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)      525 2024-04-23 17:26:52.000000 bruker_utils-0.0.2/README.rst
+drwxrwxr-x   0 simonhulse  (1006) simonhulse  (1007)        0 2024-04-23 17:44:17.014277 bruker_utils-0.0.2/bruker_utils/
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)    23895 2024-04-23 17:32:14.000000 bruker_utils-0.0.2/bruker_utils/__init__.py
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)      123 2024-04-23 17:42:37.000000 bruker_utils-0.0.2/bruker_utils/_version.py
+drwxrwxr-x   0 simonhulse  (1006) simonhulse  (1007)        0 2024-04-23 17:44:17.015277 bruker_utils-0.0.2/bruker_utils.egg-info/
+-rw-r--r--   0 simonhulse  (1006) simonhulse  (1007)     1057 2024-04-23 17:44:17.000000 bruker_utils-0.0.2/bruker_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)      270 2024-04-23 17:44:17.000000 bruker_utils-0.0.2/bruker_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)        1 2024-04-23 17:44:17.000000 bruker_utils-0.0.2/bruker_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)        6 2024-04-23 17:44:17.000000 bruker_utils-0.0.2/bruker_utils.egg-info/requires.txt
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)       13 2024-04-23 17:44:17.000000 bruker_utils-0.0.2/bruker_utils.egg-info/top_level.txt
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)       38 2024-04-23 17:44:17.015277 bruker_utils-0.0.2/setup.cfg
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)      845 2024-04-23 17:26:53.000000 bruker_utils-0.0.2/setup.py
+drwxrwxr-x   0 simonhulse  (1006) simonhulse  (1007)        0 2024-04-23 17:44:17.015277 bruker_utils-0.0.2/tests/
+-rw-rw-r--   0 simonhulse  (1006) simonhulse  (1007)     7068 2024-04-23 17:28:21.000000 bruker_utils-0.0.2/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bruker_utils-0.0.1/PKG-INFO` & `bruker_utils-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: bruker_utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: bruker_utils: Helper functions for handling Bruker NMR data.
 Home-page: https://github.com/5hulse/bruker_utils
 Author: Simon Hulse
 Author-email: simon.hulse@chem.ox.ac.uk
-License: UNKNOWN
-Description: .. class:: center
-        
-           .. image:: https://github.com/5hulse/bruker_utils/workflows/build/badge.svg
-             :target: https://github.com/5hulse/bruker_utils/actions?query=workflow%3Abuild
-        
-           .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
-              :target: https://opensource.org/licenses/MIT
-        
-        **bruker_utils**: Module for handling Bruker NMR data in Python.
-        
-        This package provides a number of features to make handling Bruker NMR data
-        in Python straightforward.
-        
-        Documentation: https://5hulse.github.io/bruker_utils/
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+
+.. class:: center
+
+   .. image:: https://github.com/5hulse/bruker_utils/workflows/build/badge.svg
+     :target: https://github.com/5hulse/bruker_utils/actions?query=workflow%3Abuild
+
+   .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
+      :target: https://opensource.org/licenses/MIT
+
+**bruker_utils**: Module for handling Bruker NMR data in Python.
+
+This package provides a number of features to make handling Bruker NMR data
+in Python straightforward.
+
+Documentation: https://5hulse.github.io/bruker_utils/
```

### Comparing `bruker_utils-0.0.1/README.rst` & `bruker_utils-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `bruker_utils-0.0.1/setup.py` & `bruker_utils-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `bruker_utils-0.0.1/bruker_utils/__init__.py` & `bruker_utils-0.0.2/bruker_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# __init__.py
+# Simon Hulse
+# simonhulse@protonmail.com
+# Last Edited: Tue 23 Apr 2024 13:31:18 EDT
+
 import functools
 from pathlib import Path
 import re
 from typing import Iterable, List, Union
 import numpy as np
 
 from ._version import __version__
@@ -713,17 +718,18 @@
         """
         clevels = self.directory / 'clevels'
         if not clevels.is_file():
             print('WARNING: clevels file could not be found. None will be'
                   'returned')
             return None
 
-        levels = \
+        levels = sorted(
             [float(x) for x in parse_jcampdx(clevels)['LEVELS']
              if x not in ['', '0']]
+        )
         return levels
 
         # I originally had this, but scaling seemed to be an issue...
         # params = parse_jcampdx(clevels)
         # maxlev = params['MAXLEV']
         # negbase = params['NEGBASE']
         # posbase = params['POSBASE']
```

### Comparing `bruker_utils-0.0.1/bruker_utils.egg-info/PKG-INFO` & `bruker_utils-0.0.2/bruker_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
-Name: bruker-utils
-Version: 0.0.1
+Name: bruker_utils
+Version: 0.0.2
 Summary: bruker_utils: Helper functions for handling Bruker NMR data.
 Home-page: https://github.com/5hulse/bruker_utils
 Author: Simon Hulse
 Author-email: simon.hulse@chem.ox.ac.uk
-License: UNKNOWN
-Description: .. class:: center
-        
-           .. image:: https://github.com/5hulse/bruker_utils/workflows/build/badge.svg
-             :target: https://github.com/5hulse/bruker_utils/actions?query=workflow%3Abuild
-        
-           .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
-              :target: https://opensource.org/licenses/MIT
-        
-        **bruker_utils**: Module for handling Bruker NMR data in Python.
-        
-        This package provides a number of features to make handling Bruker NMR data
-        in Python straightforward.
-        
-        Documentation: https://5hulse.github.io/bruker_utils/
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy
+
+.. class:: center
+
+   .. image:: https://github.com/5hulse/bruker_utils/workflows/build/badge.svg
+     :target: https://github.com/5hulse/bruker_utils/actions?query=workflow%3Abuild
+
+   .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
+      :target: https://opensource.org/licenses/MIT
+
+**bruker_utils**: Module for handling Bruker NMR data in Python.
+
+This package provides a number of features to make handling Bruker NMR data
+in Python straightforward.
+
+Documentation: https://5hulse.github.io/bruker_utils/
```

