# Comparing `tmp/notemgmt-1.1.1.tar.gz` & `tmp/notemgmt-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notemgmt-1.1.1.tar", last modified: Sun Mar 17 06:20:04 2024, max compression
+gzip compressed data, was "notemgmt-1.2.0.tar", last modified: Tue Apr 23 03:20:06 2024, max compression
```

## Comparing `notemgmt-1.1.1.tar` & `notemgmt-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-03-17 06:20:04.236790 notemgmt-1.1.1/
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)    35129 2024-03-16 18:24:38.000000 notemgmt-1.1.1/LICENSE
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-03-16 18:23:06.000000 notemgmt-1.1.1/MANIFEST.in
--rw-r--r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      233 2024-03-17 06:20:04.236790 notemgmt-1.1.1/PKG-INFO
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)       79 2024-03-16 19:12:31.000000 notemgmt-1.1.1/README.md
-drwxrwxr-x   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-03-17 06:20:04.232790 notemgmt-1.1.1/notemgmt/
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        1 2024-03-17 06:04:51.000000 notemgmt-1.1.1/notemgmt/__init__.py
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)     3195 2024-03-17 06:19:09.000000 notemgmt-1.1.1/notemgmt/create_lecture_note.py
-drwxrwxr-x   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-03-17 06:20:04.236790 notemgmt-1.1.1/notemgmt.egg-info/
--rw-r--r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      233 2024-03-17 06:20:04.000000 notemgmt-1.1.1/notemgmt.egg-info/PKG-INFO
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      300 2024-03-17 06:20:04.000000 notemgmt-1.1.1/notemgmt.egg-info/SOURCES.txt
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        1 2024-03-17 06:20:04.000000 notemgmt-1.1.1/notemgmt.egg-info/dependency_links.txt
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)       74 2024-03-17 06:20:04.000000 notemgmt-1.1.1/notemgmt.egg-info/entry_points.txt
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        1 2024-03-16 18:42:06.000000 notemgmt-1.1.1/notemgmt.egg-info/not-zip-safe
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        9 2024-03-17 06:20:04.000000 notemgmt-1.1.1/notemgmt.egg-info/top_level.txt
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)       91 2024-03-17 05:55:33.000000 notemgmt-1.1.1/pyproject.toml
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)       38 2024-03-17 06:20:04.236790 notemgmt-1.1.1/setup.cfg
--rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      444 2024-03-17 06:19:59.000000 notemgmt-1.1.1/setup.py
+drwxrwxr-x   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-04-23 03:20:06.441015 notemgmt-1.2.0/
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)    35129 2024-03-16 18:24:38.000000 notemgmt-1.2.0/LICENSE
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-03-16 18:23:06.000000 notemgmt-1.2.0/MANIFEST.in
+-rw-r--r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      233 2024-04-23 03:20:06.441015 notemgmt-1.2.0/PKG-INFO
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      679 2024-03-17 06:29:45.000000 notemgmt-1.2.0/README.md
+drwxrwxr-x   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-04-23 03:20:06.441015 notemgmt-1.2.0/notemgmt/
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        1 2024-03-17 06:04:51.000000 notemgmt-1.2.0/notemgmt/__init__.py
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)     3314 2024-04-23 03:08:26.000000 notemgmt-1.2.0/notemgmt/create_lecture_note.py
+drwxrwxr-x   0 mikasaackerman  (1000) mikasaackerman  (1000)        0 2024-04-23 03:20:06.441015 notemgmt-1.2.0/notemgmt.egg-info/
+-rw-r--r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      233 2024-04-23 03:20:06.000000 notemgmt-1.2.0/notemgmt.egg-info/PKG-INFO
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      285 2024-04-23 03:20:06.000000 notemgmt-1.2.0/notemgmt.egg-info/SOURCES.txt
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        1 2024-04-23 03:20:06.000000 notemgmt-1.2.0/notemgmt.egg-info/dependency_links.txt
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)       74 2024-04-23 03:20:06.000000 notemgmt-1.2.0/notemgmt.egg-info/entry_points.txt
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        1 2024-03-16 18:42:06.000000 notemgmt-1.2.0/notemgmt.egg-info/not-zip-safe
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)        9 2024-04-23 03:20:06.000000 notemgmt-1.2.0/notemgmt.egg-info/top_level.txt
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)       38 2024-04-23 03:20:06.441015 notemgmt-1.2.0/setup.cfg
+-rw-rw-r--   0 mikasaackerman  (1000) mikasaackerman  (1000)      444 2024-04-23 03:18:55.000000 notemgmt-1.2.0/setup.py
```

### Comparing `notemgmt-1.1.1/LICENSE` & `notemgmt-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `notemgmt-1.1.1/notemgmt/create_lecture_note.py` & `notemgmt-1.2.0/notemgmt/create_lecture_note.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import argparse
 import os
 import shutil
 import re
 import datetime
 
+def lecstr2num(x):
+    doti = x.index('.')
+    dashi1 = x.index('_') + 1
+    dashi2 = x.index('l') - 1
+    part = int(x[doti-1])
+    lec_num = int(x[dashi1:dashi2])
+    return (lec_num, part)
+    
 def main():
 
     home_dir = os.path.expanduser('~')
     vim_templates_path = os.path.join(home_dir,".vim/templates")
     master_skeleton_path = os.path.join(vim_templates_path, "master_skeleton.tex")
     lec_skeleton_path = os.path.join(vim_templates_path, "lecture_skeleton.tex")
 
@@ -17,24 +25,23 @@
     args = parser.parse_args()
     mname = args.master_name
     r = r'lec\w*\.tex$'
     lec_date = datetime.date.today()
     lec_title = args.lecture_title
     lec_date_str = lec_date.strftime("%B %d, %Y")
     all_lec_files = list(filter(lambda f: re.search(r,f), os.listdir(os.getcwd())))
-    all_lec_files.sort()
+    print(all_lec_files)
+    all_lec_nums = [lecstr2num(x) for x in all_lec_files]
+    all_lec_nums.sort()
     #print('all lec files', all_lec_files)
-    if len(all_lec_files) > 0:
-        llec = all_lec_files[-1]
-        weeksi = llec.index('_')
-        weekei = llec.find('_',weeksi+1)
-        lecsi = llec.find('_', weekei+1)
-        lecei = llec.find('.',lecsi+1)
-        week = int(llec[weeksi+1:weekei])
-        lec = int(llec[lecsi+1:lecei])
+    if len(all_lec_nums) > 0:
+        llec = all_lec_nums[-1]
+        week = llec[0]
+        lec = llec[1]
+        print('week', week, lec)
         if lec == 2:
             lec = 1
             week += 1
         else:
             lec +=1
     else:
         week = 1
@@ -85,8 +92,7 @@
     tline = tline.replace("Lecture Title", lec_title)
     dline = dline.replace("\\today", lec_date_str)
     data[1] = tline
     data[8] = dline
     with open(lec_fn, "w", encoding="utf-8") as fp:
         fp.writelines(data)
            
-
```

