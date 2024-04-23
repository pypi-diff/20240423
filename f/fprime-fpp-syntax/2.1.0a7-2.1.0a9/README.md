# Comparing `tmp/fprime_fpp_syntax-2.1.0a7-py3-none-manylinux_2_28_aarch64.whl.zip` & `tmp/fprime_fpp_syntax-2.1.0a9-py3-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 9444466 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-12 00:00 fprime_fpp_syntax/__init__.py
--rw-r--r--  2.0 unx      570 b- defN 24-Apr-12 00:00 fprime_fpp_syntax/__main__.py
--rwxr--r--  2.0 unx 36760632 b- defN 24-Apr-12 00:00 fprime_fpp_syntax-2.1.0a7.data/data/bin/fpp-syntax
--rw-r--r--  2.0 unx      940 b- defN 24-Apr-12 00:00 fprime_fpp_syntax-2.1.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx      111 b- defN 24-Apr-12 00:00 fprime_fpp_syntax-2.1.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 24-Apr-12 00:00 fprime_fpp_syntax-2.1.0a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      625 b- defN 24-Apr-12 00:00 fprime_fpp_syntax-2.1.0a7.dist-info/RECORD
-7 files, 36762896 bytes uncompressed, 9443344 bytes compressed:  74.3%
+Zip file size: 9122464 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 02:11 fprime_fpp_syntax/__init__.py
+-rw-r--r--  2.0 unx      570 b- defN 24-Apr-23 02:11 fprime_fpp_syntax/__main__.py
+-rwxr--r--  2.0 unx 34353840 b- defN 24-Apr-23 02:10 fprime_fpp_syntax-2.1.0a9.data/data/bin/fpp-syntax
+-rw-r--r--  2.0 unx      940 b- defN 24-Apr-23 02:11 fprime_fpp_syntax-2.1.0a9.dist-info/METADATA
+-rw-r--r--  2.0 unx      111 b- defN 24-Apr-23 02:11 fprime_fpp_syntax-2.1.0a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-23 02:11 fprime_fpp_syntax-2.1.0a9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      625 b- defN 24-Apr-23 02:11 fprime_fpp_syntax-2.1.0a9.dist-info/RECORD
+7 files, 34356104 bytes uncompressed, 9121342 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: fprime_fpp_syntax/__init__.py
 Comment: 
 
 Filename: fprime_fpp_syntax/__main__.py
 Comment: 
 
-Filename: fprime_fpp_syntax-2.1.0a7.data/data/bin/fpp-syntax
+Filename: fprime_fpp_syntax-2.1.0a9.data/data/bin/fpp-syntax
 Comment: 
 
-Filename: fprime_fpp_syntax-2.1.0a7.dist-info/METADATA
+Filename: fprime_fpp_syntax-2.1.0a9.dist-info/METADATA
 Comment: 
 
-Filename: fprime_fpp_syntax-2.1.0a7.dist-info/WHEEL
+Filename: fprime_fpp_syntax-2.1.0a9.dist-info/WHEEL
 Comment: 
 
-Filename: fprime_fpp_syntax-2.1.0a7.dist-info/top_level.txt
+Filename: fprime_fpp_syntax-2.1.0a9.dist-info/top_level.txt
 Comment: 
 
-Filename: fprime_fpp_syntax-2.1.0a7.dist-info/RECORD
+Filename: fprime_fpp_syntax-2.1.0a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `fprime_fpp_syntax-2.1.0a7.dist-info/METADATA` & `fprime_fpp_syntax-2.1.0a9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-fpp-syntax
-Version: 2.1.0a7
+Version: 2.1.0a9
 Summary: FPP distribution package for fprime-fpp-syntax
 Author-email: Michael Starch <Michael.D.Starch@jpl.nasa.gov>, Thomas Boyer-Chammard <Thomas.Boyer.Chammard@jpl.nasa.gov>
 Project-URL: homepage, https://fprime.jpl.nasa.gov
 Project-URL: documentation, https://nasa.github.io/fprime/
 Keywords: fprime,embedded,nasa,flight,software
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `fprime_fpp_syntax-2.1.0a7.dist-info/RECORD` & `fprime_fpp_syntax-2.1.0a9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 fprime_fpp_syntax/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fprime_fpp_syntax/__main__.py,sha256=y54UV3ovGnAVymoI1WCKq1iG10LUFKMTZmXel_XipHc,570
-fprime_fpp_syntax-2.1.0a7.data/data/bin/fpp-syntax,sha256=w0aLZBMCBVbv5TezCTKrQfM-LkJ5TiPtvV3H_06PAmw,36760632
-fprime_fpp_syntax-2.1.0a7.dist-info/METADATA,sha256=DTivODEP-gZzNOu-t2LAFtip_xPP2U75UrePDiQPMXU,940
-fprime_fpp_syntax-2.1.0a7.dist-info/WHEEL,sha256=xQv73YPWaW3i7Mlfj4mkEpuxImCuaYTNejAkb84apzE,111
-fprime_fpp_syntax-2.1.0a7.dist-info/top_level.txt,sha256=EXLEWYWdvuGI9i_zPZQiuYSM6QlGB8l7TgVUWV2Jd8c,18
-fprime_fpp_syntax-2.1.0a7.dist-info/RECORD,,
+fprime_fpp_syntax-2.1.0a9.data/data/bin/fpp-syntax,sha256=i2Quedu1YwR5TwsLUG_DnQfZfEDpQsRvFx9ZFeh4Ql8,34353840
+fprime_fpp_syntax-2.1.0a9.dist-info/METADATA,sha256=KuTvD-SGTfgLZObk9JvqYLpb2RVHNgEBLvvMgjaoGZo,940
+fprime_fpp_syntax-2.1.0a9.dist-info/WHEEL,sha256=UuqJ77MDEXqQIQU-XaG7_1qSZVtCXjnsvXZSZzIiiPU,111
+fprime_fpp_syntax-2.1.0a9.dist-info/top_level.txt,sha256=EXLEWYWdvuGI9i_zPZQiuYSM6QlGB8l7TgVUWV2Jd8c,18
+fprime_fpp_syntax-2.1.0a9.dist-info/RECORD,,
```

