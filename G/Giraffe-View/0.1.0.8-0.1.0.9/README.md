# Comparing `tmp/Giraffe_View-0.1.0.8.tar.gz` & `tmp/Giraffe_View-0.1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Giraffe_View-0.1.0.8.tar", last modified: Thu Apr  4 03:51:12 2024, max compression
+gzip compressed data, was "Giraffe_View-0.1.0.9.tar", last modified: Thu Apr  4 04:00:54 2024, max compression
```

## Comparing `Giraffe_View-0.1.0.8.tar` & `Giraffe_View-0.1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 03:51:12.332606 Giraffe_View-0.1.0.8/
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 03:51:12.332606 Giraffe_View-0.1.0.8/Giraffe_View/
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)       57 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/__init__.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3882 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/estimated_read_accuracy.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3698 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/function.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4924 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/gc_bias.py
--rwxr--r--   0 xudongliu  (1000) xudongliu  (1000)     6181 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/giraffe
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5674 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/homopolymer.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5537 2024-04-04 03:49:45.000000 Giraffe_View-0.1.0.8/Giraffe_View/observed_read_accuracy.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11011 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/plot.py
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2171 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/Giraffe_View/regional_modification.py
-drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 03:51:12.332606 Giraffe_View-0.1.0.8/Giraffe_View.egg-info/
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-04-04 03:51:12.000000 Giraffe_View-0.1.0.8/Giraffe_View.egg-info/PKG-INFO
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2024-04-04 03:51:12.000000 Giraffe_View-0.1.0.8/Giraffe_View.egg-info/SOURCES.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-04-04 03:51:12.000000 Giraffe_View-0.1.0.8/Giraffe_View.egg-info/dependency_links.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       99 2024-04-04 03:51:12.000000 Giraffe_View-0.1.0.8/Giraffe_View.egg-info/requires.txt
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2024-04-04 03:51:12.000000 Giraffe_View-0.1.0.8/Giraffe_View.egg-info/top_level.txt
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/LICENSE
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-04-04 03:51:12.332606 Giraffe_View-0.1.0.8/PKG-INFO
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11560 2024-04-04 03:21:44.000000 Giraffe_View-0.1.0.8/README.md
--rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2024-04-04 03:51:12.332606 Giraffe_View-0.1.0.8/setup.cfg
--rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1003 2024-04-04 03:50:57.000000 Giraffe_View-0.1.0.8/setup.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 04:00:54.309566 Giraffe_View-0.1.0.9/
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 04:00:54.309566 Giraffe_View-0.1.0.9/Giraffe_View/
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)       57 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/__init__.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3882 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/estimated_read_accuracy.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     3698 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/function.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     4924 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/gc_bias.py
+-rwxr--r--   0 xudongliu  (1000) xudongliu  (1000)     6181 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/giraffe
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5674 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/homopolymer.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     5441 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/observed_read_accuracy.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11011 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/plot.py
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     2171 2024-04-04 04:00:04.000000 Giraffe_View-0.1.0.9/Giraffe_View/regional_modification.py
+drwxrwxr-x   0 xudongliu  (1000) xudongliu  (1000)        0 2024-04-04 04:00:54.309566 Giraffe_View-0.1.0.9/Giraffe_View.egg-info/
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-04-04 04:00:54.000000 Giraffe_View-0.1.0.9/Giraffe_View.egg-info/PKG-INFO
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)      466 2024-04-04 04:00:54.000000 Giraffe_View-0.1.0.9/Giraffe_View.egg-info/SOURCES.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)        1 2024-04-04 04:00:54.000000 Giraffe_View-0.1.0.9/Giraffe_View.egg-info/dependency_links.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       99 2024-04-04 04:00:54.000000 Giraffe_View-0.1.0.9/Giraffe_View.egg-info/requires.txt
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       13 2024-04-04 04:00:54.000000 Giraffe_View-0.1.0.9/Giraffe_View.egg-info/top_level.txt
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1064 2024-04-04 03:52:45.000000 Giraffe_View-0.1.0.9/LICENSE
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)    11832 2024-04-04 04:00:54.309566 Giraffe_View-0.1.0.9/PKG-INFO
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)    11560 2024-04-04 03:52:45.000000 Giraffe_View-0.1.0.9/README.md
+-rw-rw-r--   0 xudongliu  (1000) xudongliu  (1000)       38 2024-04-04 04:00:54.309566 Giraffe_View-0.1.0.9/setup.cfg
+-rw-r--r--   0 xudongliu  (1000) xudongliu  (1000)     1003 2024-04-04 04:00:50.000000 Giraffe_View-0.1.0.9/setup.py
```

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/estimated_read_accuracy.py` & `Giraffe_View-0.1.0.9/Giraffe_View/estimated_read_accuracy.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/function.py` & `Giraffe_View-0.1.0.9/Giraffe_View/function.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/gc_bias.py` & `Giraffe_View-0.1.0.9/Giraffe_View/gc_bias.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/giraffe` & `Giraffe_View-0.1.0.9/Giraffe_View/giraffe`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/homopolymer.py` & `Giraffe_View-0.1.0.9/Giraffe_View/homopolymer.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/observed_read_accuracy.py` & `Giraffe_View-0.1.0.9/Giraffe_View/observed_read_accuracy.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 from Giraffe_View.function import *
 
 def data_process(sample_ID, data_type, data_path, ref, threads=10):
     # Define the commands as a list of strings to avoid issues with spaces
     # in file names or command arguments
     # path =  os.getcwd()
 
-    # cmd0 = ["mkdir", "-p", "results/observed_quality"]
-    # cmd1 = ["seqkit", "seq", read, "-m", "200", "-Q", "7", "-g", "-j", str(threads), "-o", "results/observed_quality/clean.fastq"]
     output = "Giraffe_Results/2_Observed_quality/" + str(sample_ID) + ".bam"
     
     if data_type == "ONT":
         cmd1 = ["minimap2", "-ax", "map-ont", "-o", "Giraffe_Results/2_Observed_quality/tmp.sam", "--MD", \
         "--secondary=no", "-L", "-t", str(threads), ref, data_path]
 
+    elif data_type == "ONT_RNA":
+        cmd1 = ["minimap2", "-ax", "splice", "-uf", "-k14", "-o", "Giraffe_Results/2_Observed_quality/tmp.sam", "--MD", \
+        "--secondary=no", "-L", "-t", str(threads), ref, data_path]
+
     elif data_type == "Pacbio":
         cmd1 = ["minimap2", "-ax", "map-pb", "-o", "Giraffe_Results/2_Observed_quality/tmp.sam", "--MD", \
         "--secondary=no", "-L", "-t", str(threads), ref, data_path]
 
-    elif data_type == "ONTrna":
-        cmd1 = ["minimap2", "-ax", "splice", "-uf", "-k14", "-o", "Giraffe_Results/2_Observed_quality/tmp.sam", "--MD", \
-        "--secondary=no", "-L", "-t", str(threads), ref, data_path]
+    else:
+        error_with_color("Please check your data type!!! [ONT, Pacbio, ONT_RNA]")
 
     cmd2 = ["samtools", "view", "-bS", "-F4", "-@", str(threads), "-o", "Giraffe_Results/2_Observed_quality/tmp.bam", "Giraffe_Results/2_Observed_quality/tmp.sam"]
     cmd3 = ["samtools", "sort", "-@", str(threads), "-o", output, "Giraffe_Results/2_Observed_quality/tmp.bam"]
     cmd4 = ["samtools", "index", "-@", str(threads), output]
     cmd5 = ["rm", "-rf", "Giraffe_Results/2_Observed_quality/tmp.bam", "Giraffe_Results/2_Observed_quality/tmp.sam"]
 
     # Run each command and check the return code
```

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/plot.py` & `Giraffe_View-0.1.0.9/Giraffe_View/plot.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View/regional_modification.py` & `Giraffe_View-0.1.0.9/Giraffe_View/regional_modification.py`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/Giraffe_View.egg-info/PKG-INFO` & `Giraffe_View-0.1.0.9/Giraffe_View.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe-View
-Version: 0.1.0.8
+Version: 0.1.0.9
 Summary: Giraffe_View is specially designed to provide a comprehensive assessment of the accuracy of long-read sequencing datasets obtained from both the PacBio and Nanopore platforms.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.1.0.8/LICENSE` & `Giraffe_View-0.1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/PKG-INFO` & `Giraffe_View-0.1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Giraffe_View
-Version: 0.1.0.8
+Version: 0.1.0.9
 Summary: Giraffe_View is specially designed to provide a comprehensive assessment of the accuracy of long-read sequencing datasets obtained from both the PacBio and Nanopore platforms.
 Home-page: https://github.com/lxd98/Giraffe_View
 Author: Xudong Liu
 Author-email: xudongliu98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Giraffe_View-0.1.0.8/README.md` & `Giraffe_View-0.1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Giraffe_View-0.1.0.8/setup.py` & `Giraffe_View-0.1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="Giraffe_View",
-  version="0.1.0.8",
+  version="0.1.0.9",
   author="Xudong Liu",
   author_email="xudongliu98@gmail.com",
   description="Giraffe_View is specially designed to provide a comprehensive assessment of the accuracy of long-read sequencing datasets obtained from both the PacBio and Nanopore platforms.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/lxd98/Giraffe_View",
   packages=setuptools.find_packages(),
```

