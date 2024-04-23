# Comparing `tmp/superstore-0.2.1.tar.gz` & `tmp/superstore-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superstore-0.2.1.tar", last modified: Thu Apr  4 21:39:58 2024, max compression
+gzip compressed data, was "superstore-0.2.2.tar", last modified: Tue Apr 23 08:57:21 2024, max compression
```

## Comparing `superstore-0.2.1.tar` & `superstore-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.481467 superstore-0.2.1/
--rw-r--r--   0 timkpaine   (501) staff       (20)      108 2023-04-12 02:10:37.000000 superstore-0.2.1/AUTHORS
--rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-12 02:10:37.000000 superstore-0.2.1/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)      340 2023-04-12 02:10:37.000000 superstore-0.2.1/MANIFEST.in
--rw-r--r--   0 timkpaine   (501) staff       (20)     1083 2024-04-04 21:36:47.000000 superstore-0.2.1/Makefile
--rw-r--r--   0 timkpaine   (501) staff       (20)     1835 2024-04-04 21:39:58.481353 superstore-0.2.1/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      816 2023-04-12 02:10:37.000000 superstore-0.2.1/README.md
--rw-r--r--   0 timkpaine   (501) staff       (20)      141 2024-04-04 21:36:47.000000 superstore-0.2.1/pyproject.toml
--rw-r--r--   0 timkpaine   (501) staff       (20)      575 2024-04-04 21:39:58.481799 superstore-0.2.1/setup.cfg
--rw-r--r--   0 timkpaine   (501) staff       (20)     1334 2024-04-04 21:39:21.000000 superstore-0.2.1/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.478916 superstore-0.2.1/superstore/
--rw-r--r--   0 timkpaine   (501) staff       (20)      123 2024-04-04 21:39:21.000000 superstore-0.2.1/superstore/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2302 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/superstore.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.480058 superstore-0.2.1/superstore/tests/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1293 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/tests/test_superstore.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      253 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/tests/test_vendored.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2726 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/utils.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.480359 superstore-0.2.1/superstore/vendored/
--rw-r--r--   0 timkpaine   (501) staff       (20)       57 2023-11-05 22:17:20.000000 superstore-0.2.1/superstore/vendored/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2601 2024-04-04 21:36:47.000000 superstore-0.2.1/superstore/vendored/timeseries.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-04 21:39:58.480581 superstore-0.2.1/superstore.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1835 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)      486 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2023-04-12 02:18:21.000000 superstore-0.2.1/superstore.egg-info/not-zip-safe
--rw-r--r--   0 timkpaine   (501) staff       (20)      145 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       11 2024-04-04 21:39:58.000000 superstore-0.2.1/superstore.egg-info/top_level.txt
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-23 08:57:21.062911 superstore-0.2.2/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      108 2023-04-12 02:10:37.000000 superstore-0.2.2/AUTHORS
+-rw-r--r--   0 timkpaine   (501) staff       (20)    11352 2023-04-12 02:10:37.000000 superstore-0.2.2/LICENSE
+-rw-r--r--   0 timkpaine   (501) staff       (20)      347 2024-04-23 08:49:42.000000 superstore-0.2.2/MANIFEST.in
+-rw-r--r--   0 timkpaine   (501) staff       (20)    15065 2024-04-23 08:57:21.062552 superstore-0.2.2/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      816 2023-04-12 02:10:37.000000 superstore-0.2.2/README.md
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1593 2024-04-23 08:56:44.000000 superstore-0.2.2/pyproject.toml
+-rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-23 08:57:21.062964 superstore-0.2.2/setup.cfg
+-rw-r--r--   0 timkpaine   (501) staff       (20)       92 2024-04-23 08:49:42.000000 superstore-0.2.2/setup.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-23 08:57:21.059614 superstore-0.2.2/superstore/
+-rw-r--r--   0 timkpaine   (501) staff       (20)      100 2024-04-23 08:56:44.000000 superstore-0.2.2/superstore/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     5585 2024-04-23 08:49:42.000000 superstore-0.2.2/superstore/crossfilter.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2351 2024-04-23 08:49:42.000000 superstore-0.2.2/superstore/superstore.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-23 08:57:21.061085 superstore-0.2.2/superstore/tests/
+-rw-r--r--   0 timkpaine   (501) staff       (20)     4087 2024-04-23 08:49:42.000000 superstore-0.2.2/superstore/tests/test_crossfilter.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     1293 2023-11-05 22:17:20.000000 superstore-0.2.2/superstore/tests/test_superstore.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)      253 2023-11-05 22:17:20.000000 superstore-0.2.2/superstore/tests/test_vendored.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2726 2023-11-05 22:17:20.000000 superstore-0.2.2/superstore/utils.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-23 08:57:21.061567 superstore-0.2.2/superstore/vendored/
+-rw-r--r--   0 timkpaine   (501) staff       (20)       26 2024-04-23 08:49:42.000000 superstore-0.2.2/superstore/vendored/__init__.py
+-rw-r--r--   0 timkpaine   (501) staff       (20)     2661 2024-04-23 08:49:42.000000 superstore-0.2.2/superstore/vendored/timeseries.py
+drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-23 08:57:21.061836 superstore-0.2.2/superstore.egg-info/
+-rw-r--r--   0 timkpaine   (501) staff       (20)    15065 2024-04-23 08:57:20.000000 superstore-0.2.2/superstore.egg-info/PKG-INFO
+-rw-r--r--   0 timkpaine   (501) staff       (20)      497 2024-04-23 08:57:21.000000 superstore-0.2.2/superstore.egg-info/SOURCES.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-23 08:57:20.000000 superstore-0.2.2/superstore.egg-info/dependency_links.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)      134 2024-04-23 08:57:20.000000 superstore-0.2.2/superstore.egg-info/requires.txt
+-rw-r--r--   0 timkpaine   (501) staff       (20)       11 2024-04-23 08:57:20.000000 superstore-0.2.2/superstore.egg-info/top_level.txt
```

### Comparing `superstore-0.2.1/LICENSE` & `superstore-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superstore-0.2.1/README.md` & `superstore-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `superstore-0.2.1/superstore/superstore.py` & `superstore-0.2.2/superstore/superstore.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from random import choice, randint, random
-
 import pandas as pd
 from faker import Faker
+from random import choice, randint, random
 
 from .utils import US_SECTORS, US_SECTORS_MAP
 
 fake = Faker()
 
+__all__ = (
+    "superstore",
+    "employees",
+)
+
 
 def superstore(count=1000):
     data = []
     for id in range(count):
         dat = {}
         dat["Row ID"] = id
         dat["Order ID"] = fake.ein()
```

### Comparing `superstore-0.2.1/superstore/tests/test_superstore.py` & `superstore-0.2.2/superstore/tests/test_superstore.py`

 * *Files identical despite different names*

### Comparing `superstore-0.2.1/superstore/utils.py` & `superstore-0.2.2/superstore/utils.py`

 * *Files identical despite different names*

### Comparing `superstore-0.2.1/superstore/vendored/timeseries.py` & `superstore-0.2.2/superstore/vendored/timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,27 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import numpy as np
 import string
 from datetime import datetime
-
-import numpy as np
 from pandas import DataFrame, DatetimeIndex, Series, bdate_range
 
 _N = 30
 _K = 4
 
+__all__ = (
+    "getTimeSeries",
+    "getTimeSeriesData",
+)
+
 
 def getCols(k) -> str:
     return string.ascii_uppercase[:k]
 
 
 def makeDateIndex(k: int = 10, freq="B", name=None, **kwargs) -> DatetimeIndex:
     dt = datetime(2000, 1, 1)
```

