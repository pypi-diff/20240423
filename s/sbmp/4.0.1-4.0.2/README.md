# Comparing `tmp/sbmp-4.0.1.tar.gz` & `tmp/sbmp-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmp-4.0.1.tar", last modified: Tue Apr 23 12:07:04 2024, max compression
+gzip compressed data, was "sbmp-4.0.2.tar", last modified: Tue Apr 23 17:25:31 2024, max compression
```

## Comparing `sbmp-4.0.1.tar` & `sbmp-4.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 12:07:04.318740 sbmp-4.0.1/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-4.0.1/LICENSE
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 12:07:04.318429 sbmp-4.0.1/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-4.0.1/README.txt
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 12:07:04.317468 sbmp-4.0.1/sbmp/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       37 2024-04-23 10:25:06.000000 sbmp-4.0.1/sbmp/__init__.py
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)    20983 2024-04-23 12:05:01.000000 sbmp-4.0.1/sbmp/awt.py
--rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-4.0.1/sbmp/iss.py
-drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 12:07:04.318237 sbmp-4.0.1/sbmp.egg-info/
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 12:07:04.000000 sbmp-4.0.1/sbmp.egg-info/PKG-INFO
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      180 2024-04-23 12:07:04.000000 sbmp-4.0.1/sbmp.egg-info/SOURCES.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-23 12:07:04.000000 sbmp-4.0.1/sbmp.egg-info/dependency_links.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-23 12:07:04.000000 sbmp-4.0.1/sbmp.egg-info/top_level.txt
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-23 12:07:04.318796 sbmp-4.0.1/setup.cfg
--rw-r--r--   0 jainambarbhaya   (501) staff       (20)      991 2024-04-23 12:06:58.000000 sbmp-4.0.1/setup.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 17:25:31.057424 sbmp-4.0.2/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)     1075 2024-01-08 11:37:56.000000 sbmp-4.0.2/LICENSE
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 17:25:31.057021 sbmp-4.0.2/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        6 2024-01-08 11:39:16.000000 sbmp-4.0.2/README.txt
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 17:25:31.055794 sbmp-4.0.2/sbmp/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       37 2024-04-23 10:25:06.000000 sbmp-4.0.2/sbmp/__init__.py
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)    21244 2024-04-23 17:25:15.000000 sbmp-4.0.2/sbmp/awt.py
+-rw-------   0 jainambarbhaya   (501) staff       (20)    14742 2024-04-12 17:13:38.000000 sbmp-4.0.2/sbmp/iss.py
+drwxr-xr-x   0 jainambarbhaya   (501) staff       (20)        0 2024-04-23 17:25:31.056724 sbmp-4.0.2/sbmp.egg-info/
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      570 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/PKG-INFO
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      180 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/SOURCES.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        1 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/dependency_links.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)        5 2024-04-23 17:25:31.000000 sbmp-4.0.2/sbmp.egg-info/top_level.txt
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)       38 2024-04-23 17:25:31.057487 sbmp-4.0.2/setup.cfg
+-rw-r--r--   0 jainambarbhaya   (501) staff       (20)      991 2024-04-23 17:25:23.000000 sbmp-4.0.2/setup.py
```

### Comparing `sbmp-4.0.1/LICENSE` & `sbmp-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmp-4.0.1/PKG-INFO` & `sbmp-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmp
-Version: 4.0.1
+Version: 4.0.2
 Summary: SBMP
 Home-page: 
 Author: Jainam Barbhaya
 Author-email: jainambarbhaya1509@gmail.com
 License: MIT
 Keywords: sbmp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sbmp-4.0.1/sbmp/awt.py` & `sbmp-4.0.2/sbmp/awt.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,25 @@
                StringSplitOptions.RemoveEmptyEntries);
         foreach (String s in strlist)
         {
             Console.WriteLine(s+"\n");
         }
 '''
 
+email ='''
+var smtpClient = new SmtpClient("smtp.gmail.com")
+{
+    Port = 587,
+    Credentials = new NetworkCredential("username", "password"),
+    EnableSsl = true,
+};
+    
+smtpClient.Send("email", "recipient", "subject", "body");
+'''
+
 empregfrom_db_connectivity_insert = '''
 // file-extension: aspx.cs
 
 
 using System;
 using System.Collections.Generic;
 using System.Configuration;
@@ -591,15 +602,16 @@
     "data_grid1.txt": data_grid1,
     "data_grid2.txt": data_grid2,
     "without_data_grid.txt": without_data_grid,
     "file_handling1.txt": file_handling1,
     "validators.txt": validators,
     "validators2.txt": validators2,
     "validators3.txt": validators3,
-    "validators4.txt": validators4
+    "validators4.txt": validators4,
+    "email.txt": email
 }
 
 def awtcodes_():
     for file,code in awt_codes.items():
         print(file)
     filename = input("Enter filename: ")
     with open(filename, 'w') as f:
```

### Comparing `sbmp-4.0.1/sbmp/iss.py` & `sbmp-4.0.2/sbmp/iss.py`

 * *Files identical despite different names*

### Comparing `sbmp-4.0.1/sbmp.egg-info/PKG-INFO` & `sbmp-4.0.2/sbmp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmp
-Version: 4.0.1
+Version: 4.0.2
 Summary: SBMP
 Home-page: 
 Author: Jainam Barbhaya
 Author-email: jainambarbhaya1509@gmail.com
 License: MIT
 Keywords: sbmp
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sbmp-4.0.1/setup.py` & `sbmp-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     with open('CHANGELOG.txt', 'r') as changelog_file:
         changelog_content = changelog_file.read()
 except FileNotFoundError:
     changelog_content = 'No changelog available.'
 
 setup(
   name='sbmp',
-  version='4.0.1',
+  version='4.0.2',
   description='SBMP',
   long_description=readme_content + '\n\n' + changelog_content,
   url='',  
   author='Jainam Barbhaya',
   author_email='jainambarbhaya1509@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

