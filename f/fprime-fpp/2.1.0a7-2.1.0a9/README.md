# Comparing `tmp/fprime_fpp-2.1.0a7-py3-none-any.whl.zip` & `tmp/fprime_fpp-2.1.0a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1379 bytes, number of entries: 4
--rw-r--r--  2.0 unx     1442 b- defN 24-Apr-12 00:01 fprime_fpp-2.1.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 00:01 fprime_fpp-2.1.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-12 00:01 fprime_fpp-2.1.0a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      317 b- defN 24-Apr-12 00:01 fprime_fpp-2.1.0a7.dist-info/RECORD
-4 files, 1852 bytes uncompressed, 757 bytes compressed:  59.1%
+Zip file size: 1382 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     1442 b- defN 24-Apr-23 02:11 fprime_fpp-2.1.0a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 02:11 fprime_fpp-2.1.0a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-23 02:11 fprime_fpp-2.1.0a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      317 b- defN 24-Apr-23 02:11 fprime_fpp-2.1.0a9.dist-info/RECORD
+4 files, 1852 bytes uncompressed, 760 bytes compressed:  59.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: fprime_fpp-2.1.0a7.dist-info/METADATA
+Filename: fprime_fpp-2.1.0a9.dist-info/METADATA
 Comment: 
 
-Filename: fprime_fpp-2.1.0a7.dist-info/WHEEL
+Filename: fprime_fpp-2.1.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: fprime_fpp-2.1.0a7.dist-info/top_level.txt
+Filename: fprime_fpp-2.1.0a9.dist-info/top_level.txt
 Comment: 
 
-Filename: fprime_fpp-2.1.0a7.dist-info/RECORD
+Filename: fprime_fpp-2.1.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fprime_fpp-2.1.0a7.dist-info/METADATA` & `fprime_fpp-2.1.0a9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-fpp
-Version: 2.1.0a7
+Version: 2.1.0a9
 Summary: fprime-fpp meta-package
 Author-email: Michael Starch <Michael.D.Starch@jpl.nasa.gov>, Thomas Boyer-Chammard <Thomas.Boyer.Chammard@jpl.nasa.gov>
 Project-URL: homepage, https://fprime.jpl.nasa.gov
 Project-URL: documentation, https://nasa.github.io/fprime/
 Keywords: fprime,embedded,nasa,flight,software
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -14,20 +14,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Requires-Dist: fprime-fpp-locate-defs ==2.1.0a7
-Requires-Dist: fprime-fpp-from-xml ==2.1.0a7
-Requires-Dist: fprime-fpp-filenames ==2.1.0a7
-Requires-Dist: fprime-fpp-depend ==2.1.0a7
-Requires-Dist: fprime-fpp-to-dict ==2.1.0a7
-Requires-Dist: fprime-fpp-locate-uses ==2.1.0a7
-Requires-Dist: fprime-fpp-syntax ==2.1.0a7
-Requires-Dist: fprime-fpp-to-cpp ==2.1.0a7
-Requires-Dist: fprime-fpp-to-xml ==2.1.0a7
-Requires-Dist: fprime-fpp-format ==2.1.0a7
-Requires-Dist: fprime-fpp-check ==2.1.0a7
-Requires-Dist: fprime-fpp-to-json ==2.1.0a7
+Requires-Dist: fprime-fpp-depend ==2.1.0a9
+Requires-Dist: fprime-fpp-from-xml ==2.1.0a9
+Requires-Dist: fprime-fpp-to-cpp ==2.1.0a9
+Requires-Dist: fprime-fpp-locate-uses ==2.1.0a9
+Requires-Dist: fprime-fpp-syntax ==2.1.0a9
+Requires-Dist: fprime-fpp-check ==2.1.0a9
+Requires-Dist: fprime-fpp-filenames ==2.1.0a9
+Requires-Dist: fprime-fpp-format ==2.1.0a9
+Requires-Dist: fprime-fpp-locate-defs ==2.1.0a9
+Requires-Dist: fprime-fpp-to-dict ==2.1.0a9
+Requires-Dist: fprime-fpp-to-xml ==2.1.0a9
+Requires-Dist: fprime-fpp-to-json ==2.1.0a9
```

