# Comparing `tmp/prophet_tools-0.7.tar.gz` & `tmp/prophet_tools-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophet_tools-0.7.tar", last modified: Sat Mar 16 17:18:19 2024, max compression
+gzip compressed data, was "prophet_tools-0.8.tar", last modified: Tue Apr 23 19:48:57 2024, max compression
```

## Comparing `prophet_tools-0.7.tar` & `prophet_tools-0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 17:18:19.379100 prophet_tools-0.7/
--rw-rw-rw-   0        0        0      137 2024-03-16 17:18:19.379100 prophet_tools-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      179 2023-12-24 23:12:27.000000 prophet_tools-0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 17:18:19.375101 prophet_tools-0.7/prophet_tools/
--rw-rw-rw-   0        0        0        0 2024-02-12 01:43:39.000000 prophet_tools-0.7/prophet_tools/__init__.py
--rw-rw-rw-   0        0        0      149 2023-12-24 23:12:27.000000 prophet_tools-0.7/prophet_tools/auto_import.py
--rw-rw-rw-   0        0        0     1811 2024-03-16 17:13:15.000000 prophet_tools-0.7/prophet_tools/file_convertors.py
--rw-rw-rw-   0        0        0      268 2024-02-12 01:41:06.000000 prophet_tools-0.7/prophet_tools/how_to_import.py
--rw-rw-rw-   0        0        0     6437 2024-02-25 21:39:44.000000 prophet_tools-0.7/prophet_tools/my_functions.py
--rw-rw-rw-   0        0        0      463 2024-02-12 01:56:50.000000 prophet_tools-0.7/prophet_tools/parsing.py
--rw-rw-rw-   0        0        0     1294 2024-02-25 22:54:44.000000 prophet_tools-0.7/prophet_tools/terminal.py
--rw-rw-rw-   0        0        0     4164 2023-12-29 20:12:13.000000 prophet_tools-0.7/prophet_tools/всё_подряд.py
-drwxrwxrwx   0        0        0        0 2024-03-16 17:18:19.379100 prophet_tools-0.7/prophet_tools.egg-info/
--rw-rw-rw-   0        0        0      137 2024-03-16 17:18:19.000000 prophet_tools-0.7/prophet_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-03-16 17:18:19.000000 prophet_tools-0.7/prophet_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 17:18:19.000000 prophet_tools-0.7/prophet_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-02-12 01:48:06.000000 prophet_tools-0.7/prophet_tools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2024-03-16 17:18:19.000000 prophet_tools-0.7/prophet_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-16 17:18:19.380099 prophet_tools-0.7/setup.cfg
--rw-rw-rw-   0        0        0      232 2024-03-16 17:18:07.000000 prophet_tools-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:48:57.376551 prophet_tools-0.8/
+-rw-rw-rw-   0        0        0      137 2024-04-23 19:48:57.376551 prophet_tools-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2023-09-29 07:18:11.000000 prophet_tools-0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 19:48:57.373551 prophet_tools-0.8/prophet_tools/
+-rw-rw-rw-   0        0        0        0 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/__init__.py
+-rw-rw-rw-   0        0        0      149 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/auto_import.py
+-rw-rw-rw-   0        0        0     1811 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/file_convertors.py
+-rw-rw-rw-   0        0        0      268 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/how_to_import.py
+-rw-rw-rw-   0        0        0     6879 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/my_functions.py
+-rw-rw-rw-   0        0        0      463 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/parsing.py
+-rw-rw-rw-   0        0        0     1287 2024-04-23 19:45:43.000000 prophet_tools-0.8/prophet_tools/terminal.py
+-rw-rw-rw-   0        0        0     4164 2024-04-23 19:32:58.000000 prophet_tools-0.8/prophet_tools/всё_подряд.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:48:57.376551 prophet_tools-0.8/prophet_tools.egg-info/
+-rw-rw-rw-   0        0        0      137 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2024-04-23 19:48:57.000000 prophet_tools-0.8/prophet_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 19:48:57.377553 prophet_tools-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      240 2024-04-23 19:46:42.000000 prophet_tools-0.8/setup.py
```

### Comparing `prophet_tools-0.7/prophet_tools/file_convertors.py` & `prophet_tools-0.8/prophet_tools/file_convertors.py`

 * *Files identical despite different names*

### Comparing `prophet_tools-0.7/prophet_tools/my_functions.py` & `prophet_tools-0.8/prophet_tools/my_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     s = ppath.split('.')
     return '.' + s[-1]
 
 def get_property_from_file(filename, prop):
     from os.path import getmtime
     from datetime import datetime
 
+
     if prop == 'mod_time':
         return datetime.fromtimestamp(getmtime(filename))
 
 def list_of_folders_with_full_path(ppath, subfolders=False, debug=False):
     import os
     all_folders = []
     if debug:
@@ -192,10 +193,27 @@
         os.makedirs(path)
 
 def open_folder_in_explorer(folder):
     import os
     folder = folder.replace('/', '\\')
     os.popen(f'explorer {folder}')
 
+def check_in(what, where):
+    if type(what) is str:
+        for place in where:
+            if what in place:
+                return True
+
+    if type(where) is str:
+        for thing in what:
+            if thing in where:
+                return True
+
+    if type(what) is type(where) is list:
+        for thing in what:
+            for place in where:
+                if thing in place:
+                    return True
+
 if __name__ == '__main__':
     # print(list_of_files(r'C:\Users\Тарасов Никита\YandexDisk\проекты\_Постоянные\Учебный центр\Основы работы на ПК\Дети\1. Word\1. Текст, форматирование, таблицы'))
     open_folder_in_explorer('S:\Memories\Дом на Репинке\сорс\GoPro MAX')
```

### Comparing `prophet_tools-0.7/prophet_tools/всё_подряд.py` & `prophet_tools-0.8/prophet_tools/всё_подряд.py`

 * *Files identical despite different names*

