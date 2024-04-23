# Comparing `tmp/cfunits-3.3.6.tar.gz` & `tmp/cfunits-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfunits-3.3.6.tar", last modified: Wed May  3 10:52:46 2023, max compression
+gzip compressed data, was "cfunits-3.3.7.tar", last modified: Tue Apr 23 07:54:45 2024, max compression
```

## Comparing `cfunits-3.3.6.tar` & `cfunits-3.3.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/
--rw-rw-r--   0 david     (1000) david     (1000)     1065 2022-08-01 08:33:36.000000 cfunits-3.3.6/LICENSE
--rw-rw-r--   0 david     (1000) david     (1000)      333 2022-08-01 08:33:36.000000 cfunits-3.3.6/MANIFEST.in
--rw-rw-r--   0 david     (1000) david     (1000)     2161 2023-05-03 10:52:46.394537 cfunits-3.3.6/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     2122 2022-10-07 10:16:20.000000 cfunits-3.3.6/README.md
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/
--rw-rw-r--   0 david     (1000) david     (1000)     1360 2023-05-03 10:46:34.000000 cfunits-3.3.6/cfunits/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/etc/
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/etc/udunits/
--rw-rw-r--   0 david     (1000) david     (1000)      301 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/README
--rw-rw-r--   0 david     (1000) david     (1000)     7100 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml
--rw-rw-r--   0 david     (1000) david     (1000)     6994 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml.nonCF
--rw-rw-r--   0 david     (1000) david     (1000)     3170 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-base.xml
--rw-rw-r--   0 david     (1000) david     (1000)    55074 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml
--rw-rw-r--   0 david     (1000) david     (1000)    53091 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml.nonCF
--rw-rw-r--   0 david     (1000) david     (1000)     4034 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml
--rw-rw-r--   0 david     (1000) david     (1000)     3915 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml.nonCF
--rw-rw-r--   0 david     (1000) david     (1000)     2308 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2-prefixes.xml
--rw-rw-r--   0 david     (1000) david     (1000)      517 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/etc/udunits/udunits2.xml
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits/test/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2596 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/run_tests.py
--rwxrwxr-x   0 david     (1000) david     (1000)     2083 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/run_tests_and_coverage
--rw-rw-r--   0 david     (1000) david     (1000)    16697 2023-05-03 10:45:26.000000 cfunits-3.3.6/cfunits/test/test_Units.py
--rw-rw-r--   0 david     (1000) david     (1000)     2117 2022-08-01 08:33:36.000000 cfunits-3.3.6/cfunits/test/test_style.py
--rw-rw-r--   0 david     (1000) david     (1000)    83127 2023-05-03 10:45:26.000000 cfunits-3.3.6/cfunits/units.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-05-03 10:52:46.394537 cfunits-3.3.6/cfunits.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     2161 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      806 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)      243 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        8 2023-05-03 10:52:46.000000 cfunits-3.3.6/cfunits.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      433 2022-08-01 08:33:37.000000 cfunits-3.3.6/pyproject.toml
--rw-rw-r--   0 david     (1000) david     (1000)       42 2022-09-22 15:21:51.000000 cfunits-3.3.6/requirements.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-05-03 10:52:46.394537 cfunits-3.3.6/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)     4234 2023-05-03 10:45:26.000000 cfunits-3.3.6/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-23 07:54:45.536083 cfunits-3.3.7/
+-rw-rw-r--   0 david     (1000) david     (1000)     1065 2022-08-01 08:33:36.000000 cfunits-3.3.7/LICENSE
+-rw-rw-r--   0 david     (1000) david     (1000)      333 2022-08-01 08:33:36.000000 cfunits-3.3.7/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)     2820 2024-04-23 07:54:45.536083 cfunits-3.3.7/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     2122 2022-10-07 10:16:20.000000 cfunits-3.3.7/README.md
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-23 07:54:45.536083 cfunits-3.3.7/cfunits/
+-rw-rw-r--   0 david     (1000) david     (1000)     1360 2024-04-23 07:52:34.000000 cfunits-3.3.7/cfunits/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-23 07:54:45.536083 cfunits-3.3.7/cfunits/etc/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-23 07:54:45.536083 cfunits-3.3.7/cfunits/etc/udunits/
+-rw-rw-r--   0 david     (1000) david     (1000)      301 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/README
+-rw-rw-r--   0 david     (1000) david     (1000)     7100 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-accepted.xml
+-rw-rw-r--   0 david     (1000) david     (1000)     6994 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-accepted.xml.nonCF
+-rw-rw-r--   0 david     (1000) david     (1000)     3170 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-base.xml
+-rw-rw-r--   0 david     (1000) david     (1000)    55074 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-common.xml
+-rw-rw-r--   0 david     (1000) david     (1000)    53091 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-common.xml.nonCF
+-rw-rw-r--   0 david     (1000) david     (1000)     4034 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-derived.xml
+-rw-rw-r--   0 david     (1000) david     (1000)     3915 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-derived.xml.nonCF
+-rw-rw-r--   0 david     (1000) david     (1000)     2308 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2-prefixes.xml
+-rw-rw-r--   0 david     (1000) david     (1000)      517 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/etc/udunits/udunits2.xml
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-23 07:54:45.536083 cfunits-3.3.7/cfunits/test/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2596 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/test/run_tests.py
+-rwxrwxr-x   0 david     (1000) david     (1000)     2083 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/test/run_tests_and_coverage
+-rw-rw-r--   0 david     (1000) david     (1000)    16825 2024-04-23 07:49:55.000000 cfunits-3.3.7/cfunits/test/test_Units.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2117 2022-08-01 08:33:36.000000 cfunits-3.3.7/cfunits/test/test_style.py
+-rw-rw-r--   0 david     (1000) david     (1000)    83383 2024-04-23 07:49:55.000000 cfunits-3.3.7/cfunits/units.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-23 07:54:45.536083 cfunits-3.3.7/cfunits.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)     2820 2024-04-23 07:54:45.000000 cfunits-3.3.7/cfunits.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      806 2024-04-23 07:54:45.000000 cfunits-3.3.7/cfunits.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2024-04-23 07:54:45.000000 cfunits-3.3.7/cfunits.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      243 2024-04-23 07:54:45.000000 cfunits-3.3.7/cfunits.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        8 2024-04-23 07:54:45.000000 cfunits-3.3.7/cfunits.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      433 2022-08-01 08:33:37.000000 cfunits-3.3.7/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)       42 2022-09-22 15:21:51.000000 cfunits-3.3.7/requirements.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2024-04-23 07:54:45.536083 cfunits-3.3.7/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)     4234 2023-05-03 10:45:26.000000 cfunits-3.3.7/setup.py
```

### Comparing `cfunits-3.3.6/LICENSE` & `cfunits-3.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/PKG-INFO` & `cfunits-3.3.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfunits
-Version: 3.3.6
+Version: 3.3.7
 Summary: A python interface to UNIDATA's UDUNITS-2 package with CF extensions 
 Home-page: https://bitbucket.org/cfpython/cfunits-python
 Download-URL: https://bitbucket.org/cfpython/cfunits-python/downloads
 Author: David Hassell
 Author-email: david.hassell@ncas.ac.uk
 Maintainer: David Hassell
 Maintainer-email: david.hassell@ncas.ac.uk
@@ -21,18 +21,31 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
-Provides-Extra: required C libraries
-Provides-Extra: documentation
-Provides-Extra: pre-commit hooks
 License-File: LICENSE
+Requires-Dist: cftime>=1.5.0
+Requires-Dist: numpy>=1.15
+Requires-Dist: packaging>=20.0
+Provides-Extra: required-c-libraries
+Requires-Dist: udunits2==2.2.20; extra == "required-c-libraries"
+Provides-Extra: documentation
+Requires-Dist: sphinx<=4,>=2; extra == "documentation"
+Requires-Dist: sphinx-copybutton; extra == "documentation"
+Requires-Dist: sphinx-toggleprompt; extra == "documentation"
+Requires-Dist: sphinxcontrib-spelling; extra == "documentation"
+Provides-Extra: pre-commit-hooks
+Requires-Dist: pre-commit; extra == "pre-commit-hooks"
+Requires-Dist: black; extra == "pre-commit-hooks"
+Requires-Dist: docformatter; extra == "pre-commit-hooks"
+Requires-Dist: flake8; extra == "pre-commit-hooks"
+Requires-Dist: pydocstyle; extra == "pre-commit-hooks"
 
 *A Python interface to UNIDATA's UDUNITS-2 library with CF
 extensions*
 
 **Note: Versions 3.0.0 and later are only compatible with version Python 3. Use version 1.9 for Python 2 compatibility.**
 
 Store, combine and compare physical units and convert numeric values
```

### Comparing `cfunits-3.3.6/README.md` & `cfunits-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/__init__.py` & `cfunits-3.3.7/cfunits/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 In addition, some units are either new to, modified from, or removed
 from the standard UDUNITS-2 database in order to be more consistent
 with the CF conventions.
 
 """
 
-__Conventions__ = "CF-1.10"
-__date__ = "2023-05-03"
-__version__ = "3.3.6"
-__cf_version__ = "1.10"
+__Conventions__ = "CF-1.11"
+__date__ = "2024-04-23"
+__version__ = "3.3.7"
+__cf_version__ = "1.11"
 
 import platform
 
 from packaging.version import Version
 
 try:
     import cftime
```

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-accepted.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-accepted.xml.nonCF` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-accepted.xml.nonCF`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-base.xml` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-base.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-common.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-common.xml.nonCF` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-common.xml.nonCF`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-derived.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-derived.xml.nonCF` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-derived.xml.nonCF`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2-prefixes.xml` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2-prefixes.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/etc/udunits/udunits2.xml` & `cfunits-3.3.7/cfunits/etc/udunits/udunits2.xml`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/test/run_tests.py` & `cfunits-3.3.7/cfunits/test/run_tests.py`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/test/run_tests_and_coverage` & `cfunits-3.3.7/cfunits/test/run_tests_and_coverage`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/test/test_Units.py` & `cfunits-3.3.7/cfunits/test/test_Units.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,13 +417,17 @@
         u = Units("days since 2000-01-01", calendar="standard")
         self.assertEqual(tokenize(u), tokenize(Units("days since 2000-01-01")))
 
         u = Units("bad units")
         self.assertEqual(tokenize(u), tokenize(Units("bad units")))
         self.assertNotEqual(tokenize(u), tokenize(Units("worse units")))
 
+    def test_Units_bytes(self):
+        """Tests initializing with bytes."""
+        self.assertEqual(Units("m"), Units(b"m"))
+
 
 if __name__ == "__main__":
     print("cfunits version:", cfunits.__version__)
     print("cfunits path:", os.path.abspath(cfunits.__file__))
     print("")
     unittest.main(verbosity=2)
```

### Comparing `cfunits-3.3.6/cfunits/test/test_style.py` & `cfunits-3.3.7/cfunits/test/test_style.py`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/cfunits/units.py` & `cfunits-3.3.7/cfunits/units.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,15 +578,15 @@
     comparison, it defaults to the mixed Gregorian/Julian calendar as
     defined by Udunits:
 
     >>> u = Units('days since 2000-1-1')
     >>> u.calendar
     Traceback (most recent call last):
         ...
-    AttributeError: Units has no attribute 'calendar'
+    AttributeError: Units has no attribute 'calendar'...
     >>> v = Units('days since 2000-1-1', 'standard')
     >>> v.calendar
     'standard'
     >>> v.equals(u)
     True
 
 
@@ -797,17 +797,25 @@
 
             else:
                 # ----------------------------------------------------
                 # Set a unit other than a reference time unit
                 # ----------------------------------------------------
                 ut_unit = _cached_ut_unit.get(units, None)
                 if ut_unit is None:
+                    try:
+                        # Try for units being bytes
+                        units = units.decode("utf-8")
+                    except AttributeError:
+                        # units is not bytes
+                        pass
+
                     ut_unit = _ut_parse(
                         _ut_system, _c_char_p(units.encode("utf-8")), _UT_ASCII
                     )
+
                     if not ut_unit:
                         ut_unit = None
                         self._isvalid = False
                         self._new_reason_notvalid(
                             f"Invalid units: {units!r}; Not recognised by "
                             "UDUNITS"
                         )
@@ -1761,15 +1769,15 @@
         >>> Units(calendar='365_day').calendar
         '365_day'
         >>> Units('days since 2001-1-1', calendar='noleap').calendar
         'noleap'
         >>> Units('days since 2001-1-1').calendar
         Traceback (most recent call last):
             ...
-        AttributeError: Units has no attribute 'calendar'
+        AttributeError: Units has no attribute 'calendar'...
 
         """
         value = self._calendar
         if value is not None:
             return value
 
         raise AttributeError(
```

### Comparing `cfunits-3.3.6/cfunits.egg-info/PKG-INFO` & `cfunits-3.3.7/cfunits.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfunits
-Version: 3.3.6
+Version: 3.3.7
 Summary: A python interface to UNIDATA's UDUNITS-2 package with CF extensions 
 Home-page: https://bitbucket.org/cfpython/cfunits-python
 Download-URL: https://bitbucket.org/cfpython/cfunits-python/downloads
 Author: David Hassell
 Author-email: david.hassell@ncas.ac.uk
 Maintainer: David Hassell
 Maintainer-email: david.hassell@ncas.ac.uk
@@ -21,18 +21,31 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
-Provides-Extra: required C libraries
-Provides-Extra: documentation
-Provides-Extra: pre-commit hooks
 License-File: LICENSE
+Requires-Dist: cftime>=1.5.0
+Requires-Dist: numpy>=1.15
+Requires-Dist: packaging>=20.0
+Provides-Extra: required-c-libraries
+Requires-Dist: udunits2==2.2.20; extra == "required-c-libraries"
+Provides-Extra: documentation
+Requires-Dist: sphinx<=4,>=2; extra == "documentation"
+Requires-Dist: sphinx-copybutton; extra == "documentation"
+Requires-Dist: sphinx-toggleprompt; extra == "documentation"
+Requires-Dist: sphinxcontrib-spelling; extra == "documentation"
+Provides-Extra: pre-commit-hooks
+Requires-Dist: pre-commit; extra == "pre-commit-hooks"
+Requires-Dist: black; extra == "pre-commit-hooks"
+Requires-Dist: docformatter; extra == "pre-commit-hooks"
+Requires-Dist: flake8; extra == "pre-commit-hooks"
+Requires-Dist: pydocstyle; extra == "pre-commit-hooks"
 
 *A Python interface to UNIDATA's UDUNITS-2 library with CF
 extensions*
 
 **Note: Versions 3.0.0 and later are only compatible with version Python 3. Use version 1.9 for Python 2 compatibility.**
 
 Store, combine and compare physical units and convert numeric values
```

### Comparing `cfunits-3.3.6/cfunits.egg-info/SOURCES.txt` & `cfunits-3.3.7/cfunits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfunits-3.3.6/setup.py` & `cfunits-3.3.7/setup.py`

 * *Files identical despite different names*

