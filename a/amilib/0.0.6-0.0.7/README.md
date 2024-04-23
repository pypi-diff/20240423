# Comparing `tmp/amilib-0.0.6.tar.gz` & `tmp/amilib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amilib-0.0.6.tar", last modified: Thu Apr 18 23:39:37 2024, max compression
+gzip compressed data, was "dist/amilib-0.0.7.tar", last modified: Tue Apr 23 07:59:02 2024, max compression
```

## Comparing `amilib-0.0.6.tar` & `amilib-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-18 23:39:37.858864 amilib-0.0.6/
--rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-04-16 00:05:01.000000 amilib-0.0.6/LICENSE
--rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-18 23:39:37.858725 amilib-0.0.6/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)       76 2024-04-16 00:05:01.000000 amilib-0.0.6/README.md
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-18 23:39:37.856248 amilib-0.0.6/amilib/
--rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/__init__.py
--rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/ami_bib.py
--rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.000000 amilib-0.0.6/amilib/ami_csv.py
--rw-r--r--   0 pm286      (503) staff       (20)   168064 2024-04-18 06:54:59.000000 amilib-0.0.6/amilib/ami_html.py
--rw-r--r--   0 pm286      (503) staff       (20)    16455 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/ami_integrate.py
--rw-r--r--   0 pm286      (503) staff       (20)     8504 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/ami_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    81920 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/ami_pdf_libs.py
--rw-r--r--   0 pm286      (503) staff       (20)     4976 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/ami_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/ami_util.py
--rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/amidriver.py
--rw-r--r--   0 pm286      (503) staff       (20)    49230 2024-04-18 23:39:25.000000 amilib-0.0.6/amilib/amix.py
--rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/bbox.py
--rw-r--r--   0 pm286      (503) staff       (20)    14085 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/file_lib.py
--rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/html_generator.py
--rw-r--r--   0 pm286      (503) staff       (20)    48143 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/html_marker.py
--rw-r--r--   0 pm286      (503) staff       (20)    27194 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/pdf_args.py
--rw-r--r--   0 pm286      (503) staff       (20)    36799 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/util.py
--rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/wikimedia.py
--rw-r--r--   0 pm286      (503) staff       (20)    54474 2024-04-16 00:05:01.000000 amilib-0.0.6/amilib/xml_lib.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-18 23:39:37.857156 amilib-0.0.6/amilib.egg-info/
--rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-18 23:39:37.000000 amilib-0.0.6/amilib.egg-info/PKG-INFO
--rw-r--r--   0 pm286      (503) staff       (20)      802 2024-04-18 23:39:37.000000 amilib-0.0.6/amilib.egg-info/SOURCES.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-18 23:39:37.000000 amilib-0.0.6/amilib.egg-info/dependency_links.txt
--rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-18 23:39:37.000000 amilib-0.0.6/amilib.egg-info/entry_points.txt
--rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-18 23:35:57.000000 amilib-0.0.6/amilib.egg-info/not-zip-safe
--rw-r--r--   0 pm286      (503) staff       (20)      125 2024-04-18 23:39:37.000000 amilib-0.0.6/amilib.egg-info/requires.txt
--rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-18 23:39:37.000000 amilib-0.0.6/amilib.egg-info/top_level.txt
--rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-18 23:39:37.858912 amilib-0.0.6/setup.cfg
--rw-r--r--   0 pm286      (503) staff       (20)     1651 2024-04-18 23:39:25.000000 amilib-0.0.6/setup.py
-drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-18 23:39:37.858546 amilib-0.0.6/test/
--rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.000000 amilib-0.0.6/test/test_all.py
--rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.000000 amilib-0.0.6/test/test_file.py
--rw-r--r--   0 pm286      (503) staff       (20)    38266 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_headless.py
--rw-r--r--   0 pm286      (503) staff       (20)   121225 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_html.py
--rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_nlp.py
--rw-r--r--   0 pm286      (503) staff       (20)    80007 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_pdf.py
--rw-r--r--   0 pm286      (503) staff       (20)      957 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_stat.py
--rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_svg.py
--rw-r--r--   0 pm286      (503) staff       (20)    10541 2024-04-18 07:00:37.000000 amilib-0.0.6/test/test_util.py
--rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_wikidata.py
--rw-r--r--   0 pm286      (503) staff       (20)     4787 2024-04-16 00:05:02.000000 amilib-0.0.6/test/test_xml.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.018311 amilib-0.0.7/
+-rw-r--r--   0 pm286      (503) staff       (20)    11357 2024-04-16 00:05:01.000000 amilib-0.0.7/LICENSE
+-rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-23 07:59:02.018166 amilib-0.0.7/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)       76 2024-04-16 00:05:01.000000 amilib-0.0.7/README.md
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.012909 amilib-0.0.7/amilib/
+-rw-r--r--   0 pm286      (503) staff       (20)        0 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/__init__.py
+-rw-r--r--   0 pm286      (503) staff       (20)     5132 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_bib.py
+-rw-r--r--   0 pm286      (503) staff       (20)      287 2024-04-17 21:43:55.000000 amilib-0.0.7/amilib/ami_csv.py
+-rw-r--r--   0 pm286      (503) staff       (20)   168064 2024-04-18 06:54:59.000000 amilib-0.0.7/amilib/ami_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16455 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_integrate.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8504 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    81920 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_pdf_libs.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4976 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10651 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/ami_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)     8422 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/amidriver.py
+-rw-r--r--   0 pm286      (503) staff       (20)    49270 2024-04-23 07:57:44.000000 amilib-0.0.7/amilib/amix.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19721 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/bbox.py
+-rw-r--r--   0 pm286      (503) staff       (20)    14085 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/file_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)    19595 2024-04-23 05:05:15.000000 amilib-0.0.7/amilib/headless_lib.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1334 2024-04-23 06:25:16.000000 amilib-0.0.7/amilib/html_extra.py
+-rw-r--r--   0 pm286      (503) staff       (20)    16556 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/html_generator.py
+-rw-r--r--   0 pm286      (503) staff       (20)    48143 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/html_marker.py
+-rw-r--r--   0 pm286      (503) staff       (20)    27194 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/pdf_args.py
+-rw-r--r--   0 pm286      (503) staff       (20)    36799 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    33690 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/wikimedia.py
+-rw-r--r--   0 pm286      (503) staff       (20)    54474 2024-04-16 00:05:01.000000 amilib-0.0.7/amilib/xml_lib.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.013953 amilib-0.0.7/amilib.egg-info/
+-rw-r--r--   0 pm286      (503) staff       (20)      816 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/PKG-INFO
+-rw-r--r--   0 pm286      (503) staff       (20)      846 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/SOURCES.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/dependency_links.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       44 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/entry_points.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        1 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/not-zip-safe
+-rw-r--r--   0 pm286      (503) staff       (20)      125 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/requires.txt
+-rw-r--r--   0 pm286      (503) staff       (20)        7 2024-04-23 07:59:01.000000 amilib-0.0.7/amilib.egg-info/top_level.txt
+-rw-r--r--   0 pm286      (503) staff       (20)       38 2024-04-23 07:59:02.018353 amilib-0.0.7/setup.cfg
+-rw-r--r--   0 pm286      (503) staff       (20)     1651 2024-04-23 07:57:44.000000 amilib-0.0.7/setup.py
+drwxr-xr-x   0 pm286      (503) staff       (20)        0 2024-04-23 07:59:02.017972 amilib-0.0.7/test/
+-rw-r--r--   0 pm286      (503) staff       (20)     2679 2024-04-17 00:12:33.000000 amilib-0.0.7/test/test_all.py
+-rw-r--r--   0 pm286      (503) staff       (20)     3941 2024-04-18 07:09:52.000000 amilib-0.0.7/test/test_file.py
+-rw-r--r--   0 pm286      (503) staff       (20)    21400 2024-04-23 04:51:55.000000 amilib-0.0.7/test/test_headless.py
+-rw-r--r--   0 pm286      (503) staff       (20)   120176 2024-04-23 06:41:05.000000 amilib-0.0.7/test/test_html.py
+-rw-r--r--   0 pm286      (503) staff       (20)      733 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_nlp.py
+-rw-r--r--   0 pm286      (503) staff       (20)    80007 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_pdf.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1087 2024-04-23 06:34:10.000000 amilib-0.0.7/test/test_stat.py
+-rw-r--r--   0 pm286      (503) staff       (20)     1065 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_svg.py
+-rw-r--r--   0 pm286      (503) staff       (20)    10541 2024-04-18 07:00:37.000000 amilib-0.0.7/test/test_util.py
+-rw-r--r--   0 pm286      (503) staff       (20)    35765 2024-04-16 00:05:02.000000 amilib-0.0.7/test/test_wikidata.py
+-rw-r--r--   0 pm286      (503) staff       (20)     4824 2024-04-23 06:34:10.000000 amilib-0.0.7/test/test_xml.py
```

### Comparing `amilib-0.0.6/LICENSE` & `amilib-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/PKG-INFO` & `amilib-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.6
+Version: 0.0.7
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.6/amilib/ami_bib.py` & `amilib-0.0.7/amilib/ami_bib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/ami_html.py` & `amilib-0.0.7/amilib/ami_html.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/ami_integrate.py` & `amilib-0.0.7/amilib/ami_integrate.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/ami_nlp.py` & `amilib-0.0.7/amilib/ami_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/ami_pdf_libs.py` & `amilib-0.0.7/amilib/ami_pdf_libs.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/ami_svg.py` & `amilib-0.0.7/amilib/ami_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/ami_util.py` & `amilib-0.0.7/amilib/ami_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/amidriver.py` & `amilib-0.0.7/amilib/amidriver.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/amix.py` & `amilib-0.0.7/amilib/amix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1151,14 +1151,15 @@
         version = '0.0.1a1'  # 2024-03-27
         version = '0.0.1a3'  # 2024-03-27
         version = '0.0.1'  # 2024-04-03
         version = '0.0.2'  # 2024-04-04
         version = '0.0.3'  # 2024-04-19
         # had to revert here I think
         version = '0.0.6'  # 2024-04-19
+        version = '0.0.7'  # 2024-04-23
 
         # logging.warn(f"VERSION {version}")
         return version
 
 
 class AmiLibArgs(AbstractArgs):
     """Parse args to analyze, edit and annotate HTML"""
```

### Comparing `amilib-0.0.6/amilib/bbox.py` & `amilib-0.0.7/amilib/bbox.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/file_lib.py` & `amilib-0.0.7/amilib/file_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/html_generator.py` & `amilib-0.0.7/amilib/html_generator.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/html_marker.py` & `amilib-0.0.7/amilib/html_marker.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/pdf_args.py` & `amilib-0.0.7/amilib/pdf_args.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/util.py` & `amilib-0.0.7/amilib/util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/wikimedia.py` & `amilib-0.0.7/amilib/wikimedia.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib/xml_lib.py` & `amilib-0.0.7/amilib/xml_lib.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/amilib.egg-info/PKG-INFO` & `amilib-0.0.7/amilib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amilib
-Version: 0.0.6
+Version: 0.0.7
 Summary: document download, cleaning, managemenr
 Home-page: https://github.com/petermr/amilib
 Author: Peter Murray-Rust
 Author-email: petermurrayrust@googlemail.com
 License: Apache2
 Keywords: text and data mining
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `amilib-0.0.6/amilib.egg-info/SOURCES.txt` & `amilib-0.0.7/amilib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 amilib/ami_pdf_libs.py
 amilib/ami_svg.py
 amilib/ami_util.py
 amilib/amidriver.py
 amilib/amix.py
 amilib/bbox.py
 amilib/file_lib.py
+amilib/headless_lib.py
+amilib/html_extra.py
 amilib/html_generator.py
 amilib/html_marker.py
 amilib/pdf_args.py
 amilib/util.py
 amilib/wikimedia.py
 amilib/xml_lib.py
 amilib.egg-info/PKG-INFO
```

### Comparing `amilib-0.0.6/setup.py` & `amilib-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
  'scikit-learn',
 
 ]
 
 setup(
     name='amilib',
     url='https://github.com/petermr/amilib',
-    version='0.0.6',
+    version='0.0.7',
     description='document download, cleaning, managemenr',
     long_description_content_type='text/markdown',
     long_description=readme,
     author="Peter Murray-Rust",
     author_email='petermurrayrust@googlemail.com',
     license='Apache2',
     install_requires=requirements,
```

### Comparing `amilib-0.0.6/test/test_all.py` & `amilib-0.0.7/test/test_all.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/test/test_file.py` & `amilib-0.0.7/test/test_file.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/test/test_html.py` & `amilib-0.0.7/test/test_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from lxml.etree import HTMLParser
 
 from amilib.ami_bib import Reference, Biblioref
 from amilib.file_lib import FileLib
 from amilib.ami_html import HTMLSearcher, HtmlTree, HtmlAnnotator, AnnotatorCommand, URLCache
 from amilib.ami_html import HtmlUtil, H_SPAN, CSSStyle, HtmlTidy, HtmlStyle, HtmlClass, SectionHierarchy, AmiFont, \
     FloatBoundary, Footnote, HtmlGroup
+from amilib.html_extra import HtmlExtra
 from amilib.pdf_args import PDFArgs
 from amilib.ami_pdf_libs import AmiPDFPlumber
 # from pyamihtmlx.ar6 import TargetExtractor, IPCCTarget, LinkFactory, IPCCTargetLink
 from amilib.amix import AmiLib
 from amilib.util import Util
 from amilib.xml_lib import HtmlLib, XmlLib
 from amilib.ami_integrate import HtmlGenerator
@@ -59,18 +60,18 @@
 
 NOTE. the use of classname, classref and similar is inconsistent. We want to have:
 s1  to mean class name (classname)
 .s1 to mean a reference to a classname (only used in <style> elements but involved in conversions
 """
 
 
-def add_children(jats, htmlx):
-    tag = jats.tag()
-    if tag == 'p':
-        html
+# def add_children(jats, htmlx):
+#     tag = jats.tag()
+#     if tag == 'p':
+#         html
 
 
 class TestHtml(AmiAnyTest):
     """
     parsing , structuring linking in/to.form HTML
     This will evolve into an ami_html.py module
     """
@@ -632,108 +633,78 @@
             "\\s*"
              
              f"(?P<{SECTION}>"
              "(?:(?:(?:TS\\.)?[A-Z]|SPM|TS|[Ff]ootnote )\\.?)?"
              "\\d+(?:\\.\\d+)*"
              ")"
         )
-        matched_dict = self.create_matched_dict_and_unmatched_keys(paragraph_dict, node_re)
+        matched_dict = HtmlExtra.create_matched_dict_and_unmatched_keys(paragraph_dict, node_re)
 
-        return self.create_counters(PACKAGE, SECTION, SUBPACKAGE, matched_dict, debug=True)
+        return HtmlExtra.create_counters(PACKAGE, SECTION, SUBPACKAGE, matched_dict, debug=True)
         # print(f"unmatched {len(unmatched_keys)} {unmatched_keys}")
 
         (matched_dict.keys(), Counter(pck_counter), Counter(subp_counter), Counter(sect_counter))
 
         # print(f"counter {counter.most_common_values()}")
 
-    def create_counters(self, PACKAGE, SECTION, SUBPACKAGE, matched_dict, debug=False):
-        pck_counter = defaultdict(int)
-        subp_counter = defaultdict(int)
-        sect_counter = defaultdict(int)
-        for key in matched_dict:
-            value = matched_dict.get(key)
-            pck_counter[value[PACKAGE]] += 1
-            subp_counter[value[SUBPACKAGE]] += 1
-            sect_counter[value[SECTION]] += 1
-        if debug:
-            print(f"package: {Counter(pck_counter)}")
-            print(f"subpack: {Counter(subp_counter)}")
-            print(f"section: {Counter(sect_counter)}")
-
-        return (matched_dict.keys(), Counter(pck_counter), Counter(subp_counter), Counter(sect_counter))
-
-    def create_matched_dict_and_unmatched_keys(self, def_dict, node_re):
-        print(f"def_dict {def_dict}")
-        counter = Counter(def_dict)
-        print(f"counter {len(counter)}: {counter.most_common()}")
-
-        matched_dict = dict()
-        unmatched_keys = set()
-        for key in counter:
-            match = re.match(node_re, key)
-            if match is None:
-                unmatched_keys.add(key)
-            else:
-                matched_dict[key] = match.groupdict()
-        return matched_dict
-
-    @unittest.skip("climate specific")
-    def test_create_target_node_dir_tree_from_ipcc_chapter_html_DEVELOP(self):
-        """reads a chapter in HTML, finds targets in {...'...} , uses div id as anchor
-        and builds directory tree of targets
-        """
-        file = Path(Resources.TEST_IPCC_DIR, "LongerReport", "fulltext.html")
-        assert file.exists(), f"{file} should exist"
-        table = TargetExtractor.extract_ipcc_fulltext_into_source_target_table(file)
-        # TODO make pandas object to manage columns
-        target_extractor = TargetExtractor.create_target_extractor(
-            ['id', 'source', 'target', 'package', 'section', 'object', 'subsection', 'source_text'])
-        df = pd.DataFrame(table, columns=target_extractor.column_dict.keys())
-        print(f"df {df}")
-        lr_path = Path(AmiAnyTest.TEMP_HTML_DIR, "ar6", "kg", "LongReport")
-        lr_path.mkdir(exist_ok=True, parents=True)
-        path = Path(lr_path, "edges.csv")
-        print(f"writing CSV: {path}")
-        df.to_csv(path_or_buf=path)
-        # print(f"data frame {df}")
-        common_source_tuples = target_extractor.find_commonest_in_node_lists (table, node_name="source")
-        common_target_tuples = target_extractor.find_commonest_in_node_lists (table, node_name="target")
-        print(f"target {common_target_tuples}\nsource {common_source_tuples}")
-        temp_dir = Path(AmiAnyTest.TEMP_HTML_DIR, "ar6", "LR_network")
-        temp_dir.mkdir(exist_ok=True)
-
-        IPCCTarget.make_dirs_from_targets(common_target_tuples, temp_dir)
-
-    @unittest.skip("clime specific")
-    def test_create_target_node_dir_trees_from_ipcc_chapters_DEVELOP_HACKATHON(self):
-        """reads a chapter in HTML, finds targets in {...'...} , uses div id as anchor
-        and builds directory tree of targets
-        """
-        packages = [
-            "LongerReport",
-            "wg2_spm",
-            "wg3_spm",
-        ]
-        target_extractor = TargetExtractor.create_target_extractor(
-            ['id', 'source', 'target', 'package', 'section', 'object', 'subsection', 'source_text'])
-
-        for package in packages:
-            file = Path(Resources.TEST_IPCC_DIR, package, "fulltext.html")
-            table = TargetExtractor.extract_ipcc_fulltext_into_source_target_table(file)
-            df = pd.DataFrame(table)
-            print(f"df {df}")
-            print(f"row0 /1 {table[:2]}")
-            common_source_tuples = target_extractor.find_commonest_in_node_lists(table, node_name="source")
-            common_target_tuples = target_extractor.find_commonest_in_node_lists(table, node_name="target")
-            ipcc_dir = Path(AmiAnyTest.TEMP_HTML_DIR, "ar6")
-            temp_dir = Path(ipcc_dir, f"{package}_network")
-            print(f"writing to {temp_dir}")
-            temp_dir.mkdir(exist_ok=True)
 
-            IPCCTarget.make_dirs_from_targets(common_target_tuples, temp_dir)
+    # @unittest.skip("climate specific")
+    # def test_create_target_node_dir_tree_from_ipcc_chapter_html_DEVELOP(self):
+    #     """reads a chapter in HTML, finds targets in {...'...} , uses div id as anchor
+    #     and builds directory tree of targets
+    #     """
+    #     file = Path(Resources.TEST_IPCC_DIR, "LongerReport", "fulltext.html")
+    #     assert file.exists(), f"{file} should exist"
+    #     table = TargetExtractor.extract_ipcc_fulltext_into_source_target_table(file)
+    #     # TODO make pandas object to manage columns
+    #     target_extractor = TargetExtractor.create_target_extractor(
+    #         ['id', 'source', 'target', 'package', 'section', 'object', 'subsection', 'source_text'])
+    #     df = pd.DataFrame(table, columns=target_extractor.column_dict.keys())
+    #     print(f"df {df}")
+    #     lr_path = Path(AmiAnyTest.TEMP_HTML_DIR, "ar6", "kg", "LongReport")
+    #     lr_path.mkdir(exist_ok=True, parents=True)
+    #     path = Path(lr_path, "edges.csv")
+    #     print(f"writing CSV: {path}")
+    #     df.to_csv(path_or_buf=path)
+    #     # print(f"data frame {df}")
+    #     common_source_tuples = target_extractor.find_commonest_in_node_lists (table, node_name="source")
+    #     common_target_tuples = target_extractor.find_commonest_in_node_lists (table, node_name="target")
+    #     print(f"target {common_target_tuples}\nsource {common_source_tuples}")
+    #     temp_dir = Path(AmiAnyTest.TEMP_HTML_DIR, "ar6", "LR_network")
+    #     temp_dir.mkdir(exist_ok=True)
+    #
+    #     IPCCTarget.make_dirs_from_targets(common_target_tuples, temp_dir)
+    #
+    # @unittest.skip("clime specific")
+    # def test_create_target_node_dir_trees_from_ipcc_chapters_DEVELOP_HACKATHON(self):
+    #     """reads a chapter in HTML, finds targets in {...'...} , uses div id as anchor
+    #     and builds directory tree of targets
+    #     """
+    #     packages = [
+    #         "LongerReport",
+    #         "wg2_spm",
+    #         "wg3_spm",
+    #     ]
+    #     target_extractor = TargetExtractor.create_target_extractor(
+    #         ['id', 'source', 'target', 'package', 'section', 'object', 'subsection', 'source_text'])
+    #
+    #     for package in packages:
+    #         file = Path(Resources.TEST_IPCC_DIR, package, "fulltext.html")
+    #         table = TargetExtractor.extract_ipcc_fulltext_into_source_target_table(file)
+    #         df = pd.DataFrame(table)
+    #         print(f"df {df}")
+    #         print(f"row0 /1 {table[:2]}")
+    #         common_source_tuples = target_extractor.find_commonest_in_node_lists(table, node_name="source")
+    #         common_target_tuples = target_extractor.find_commonest_in_node_lists(table, node_name="target")
+    #         ipcc_dir = Path(AmiAnyTest.TEMP_HTML_DIR, "ar6")
+    #         temp_dir = Path(ipcc_dir, f"{package}_network")
+    #         print(f"writing to {temp_dir}")
+    #         temp_dir.mkdir(exist_ok=True)
+    #
+    #         IPCCTarget.make_dirs_from_targets(common_target_tuples, temp_dir)
 
     def test_remove_floats_from_fulltext_html_DEVELOP(self):
         package = "LongerReport"
         file = Path(Resources.TEST_IPCC_DIR, package, "fulltext.html")
         html_elem = lxml.etree.parse(str(file)).getroot()
         FloatBoundary.extract_floats_and_boundaries(html_elem, package, outdir=str(Path(AmiAnyTest.TEMP_HTML_IPCC, package)))
         XmlLib.write_xml(html_elem, Path(AmiAnyTest.TEMP_HTML_IPCC, package, "defloated.html"))
```

### Comparing `amilib-0.0.6/test/test_nlp.py` & `amilib-0.0.7/test/test_nlp.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/test/test_pdf.py` & `amilib-0.0.7/test/test_pdf.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/test/test_stat.py` & `amilib-0.0.7/test/test_stat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import csv
 from pathlib import Path
 
 from amilib.ami_nlp import AmiNLP
 from test.resources import Resources
+from test.test_all import AmiAnyTest
 
-class TestStat:
-    """
-    test statistics and ML (small at present)
-    """
 
-def test_plot_scatter_noel_oboyle_STAT_PLOT():
+class TestStat(AmiAnyTest):
     """
-    computes labelled 2-D projection of points from distance matrix
-    :return:
+    test statistics and ML (small at present)
     """
 
-    # Distance file available from RMDS project:
-    #    https://github.com/cheind/rmds/blob/master/examples/european_city_distances.csv
-
-    show_plot = False  # set True if plot wanted, BUT blocks on displaying
-    data = []
-    inputx = Path(Resources.TEST_RESOURCES_DIR, "misc", "european_city_distances.csv")
-    delimiter = ';'
-    reader = csv.reader(open(inputx, "r"), delimiter=delimiter)
-    data = list(reader)
-
-    dists = []
-    labels = []
-    for dt in data:
-        labels.append(dt[0])
-        dists.append([float(dd) for dd in dt[1:-1]])
+    def test_plot_scatter_noel_oboyle_STAT_PLOT(self):
+        """
+        computes labelled 2-D projection of points from distance matrix
+        :return:
+        """
+
+        # Distance file available from RMDS project:
+        #    https://github.com/cheind/rmds/blob/master/examples/european_city_distances.csv
+
+        show_plot = False  # set True if plot wanted, BUT blocks on displaying
+        data = []
+        inputx = Path(Resources.TEST_RESOURCES_DIR, "misc", "european_city_distances.csv")
+        delimiter = ';'
+        reader = csv.reader(open(inputx, "r"), delimiter=delimiter)
+        data = list(reader)
+
+        dists = []
+        labels = []
+        for dt in data:
+            labels.append(dt[0])
+            dists.append([float(dd) for dd in dt[1:-1]])
 
-    AmiNLP.plot_points_labels(dists, labels, show_plot=show_plot)
+        AmiNLP.plot_points_labels(dists, labels, show_plot=show_plot)
```

### Comparing `amilib-0.0.6/test/test_svg.py` & `amilib-0.0.7/test/test_svg.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/test/test_util.py` & `amilib-0.0.7/test/test_util.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/test/test_wikidata.py` & `amilib-0.0.7/test/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `amilib-0.0.6/test/test_xml.py` & `amilib-0.0.7/test/test_xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import lxml.etree as ET
 
 from amilib.ami_html import HtmlStyle
 from amilib.xml_lib import XmlLib, HtmlLib
 
 from test.test_all import AmiAnyTest
+from test.test_wikidata import WikimediaTests
 
 
 class TestXml(AmiAnyTest):
 
     def test_is_integer(self):
         span = ET.Element("span")
         span.text = "12"
@@ -71,28 +72,28 @@
     <m><r/> and some text after.</m>
     <m><r/></m>
     <m>Text before <r/> and after</m>
     <m><b/> Text after a sibling <r/> Text before a sibling<b/></m>
     </everything>
     '''
         result = XmlLib.replace_nodes_with_text(data, "//r", "DELETED")
-        print(etree.tostring(result))
+        print(ET.tostring(result))
 
     @classmethod
     def test_replace_nodenames(cls):
         data = '''<p>essential oil extracted from
  <italic>T. bovei</italic> was comprised ... on the
  <italic>T. bovei</italic> activities ... activity.
 </p>'''
 
-        doc = etree.fromstring(data)
+        doc = ET.fromstring(data)
         italics = doc.findall("italic")
         for node in italics:
             node.tag = "i"
-        print(etree.tostring(doc))
+        print(ET.tostring(doc))
 
     """transform = etree.XSLT(xslt_tree)
 >>> result = transform(doc, a="'A'")
 >>> bytes(result)
 b'<?xml version="1.0"?>\n<foo>A</foo>\n'
     """
```

