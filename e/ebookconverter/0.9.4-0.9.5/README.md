# Comparing `tmp/ebookconverter-0.9.4.tar.gz` & `tmp/ebookconverter-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebookconverter-0.9.4.tar", last modified: Tue Feb 27 00:19:28 2024, max compression
+gzip compressed data, was "ebookconverter-0.9.5.tar", last modified: Tue Apr 23 02:21:46 2024, max compression
```

## Comparing `ebookconverter-0.9.4.tar` & `ebookconverter-0.9.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-02-27 00:19:28.635030 ebookconverter-0.9.4/
--rw-r--r--   0 eric       (501) staff       (20)    10482 2024-02-27 00:15:45.000000 ebookconverter-0.9.4/CHANGES
--rw-r--r--   0 eric       (501) staff       (20)    35149 2018-12-20 21:57:45.000000 ebookconverter-0.9.4/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     2760 2024-02-27 00:19:28.634645 ebookconverter-0.9.4/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1903 2022-11-18 17:54:42.000000 ebookconverter-0.9.4/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-02-27 00:19:28.624193 ebookconverter-0.9.4/ebookconverter/
--rwxr-xr-x   0 eric       (501) staff       (20)     2954 2021-09-02 06:13:21.000000 ebookconverter-0.9.4/ebookconverter/AutoDelete.py
--rw-r--r--   0 eric       (501) staff       (20)     1602 2021-08-11 20:29:59.000000 ebookconverter-0.9.4/ebookconverter/CSV.py
--rw-r--r--   0 eric       (501) staff       (20)     2626 2021-10-21 15:37:14.000000 ebookconverter-0.9.4/ebookconverter/Candidates.py
--rw-r--r--   0 eric       (501) staff       (20)    22828 2023-09-29 17:17:48.000000 ebookconverter-0.9.4/ebookconverter/EbookConverter.py
--rwxr-xr-x   0 eric       (501) staff       (20)    10715 2024-02-26 21:53:15.000000 ebookconverter-0.9.4/ebookconverter/FileInfo.py
--rw-r--r--   0 eric       (501) staff       (20)     5557 2023-03-06 20:45:09.000000 ebookconverter-0.9.4/ebookconverter/Notifier.py
--rw-r--r--   0 eric       (501) staff       (20)     2070 2022-09-14 19:47:10.000000 ebookconverter-0.9.4/ebookconverter/ReloadWorkflow.py
--rw-r--r--   0 eric       (501) staff       (20)     3444 2022-09-14 20:35:23.000000 ebookconverter-0.9.4/ebookconverter/UpdateFromWorkflow.py
--rw-r--r--   0 eric       (501) staff       (20)       18 2024-02-27 00:16:43.000000 ebookconverter-0.9.4/ebookconverter/Version.py
--rw-r--r--   0 eric       (501) staff       (20)       27 2014-08-23 15:53:05.000000 ebookconverter-0.9.4/ebookconverter/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-02-27 00:19:28.629757 ebookconverter-0.9.4/ebookconverter/writers/
--rw-r--r--   0 eric       (501) staff       (20)     1707 2021-10-18 22:59:45.000000 ebookconverter-0.9.4/ebookconverter/writers/CoverWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     3193 2022-04-28 19:36:11.000000 ebookconverter-0.9.4/ebookconverter/writers/FacebookWriter.py
--rwxr-xr-x   0 eric       (501) staff       (20)     2542 2024-02-27 00:08:52.000000 ebookconverter-0.9.4/ebookconverter/writers/HTMLWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     2863 2023-09-20 18:15:50.000000 ebookconverter-0.9.4/ebookconverter/writers/MastodonWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     1330 2021-09-02 06:13:21.000000 ebookconverter-0.9.4/ebookconverter/writers/QRCodeWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     7235 2023-11-30 19:30:16.000000 ebookconverter-0.9.4/ebookconverter/writers/RDFWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     3024 2019-09-17 19:12:37.000000 ebookconverter-0.9.4/ebookconverter/writers/TwitterWriter.py
--rw-r--r--   0 eric       (501) staff       (20)     1387 2022-09-29 19:43:00.000000 ebookconverter-0.9.4/ebookconverter/writers/UpdateWriter.py
--rw-r--r--   0 eric       (501) staff       (20)       10 2014-02-08 17:56:38.000000 ebookconverter-0.9.4/ebookconverter/writers/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-02-27 00:19:28.634108 ebookconverter-0.9.4/ebookconverter.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)     2760 2024-02-27 00:19:28.000000 ebookconverter-0.9.4/ebookconverter.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1121 2024-02-27 00:19:28.000000 ebookconverter-0.9.4/ebookconverter.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2024-02-27 00:19:28.000000 ebookconverter-0.9.4/ebookconverter.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)      124 2024-02-27 00:19:28.000000 ebookconverter-0.9.4/ebookconverter.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       15 2024-02-27 00:19:28.000000 ebookconverter-0.9.4/ebookconverter.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-02-27 00:19:28.633509 ebookconverter-0.9.4/scripts/
--rwxr-xr-x   0 eric       (501) staff       (20)      302 2021-09-02 06:13:21.000000 ebookconverter-0.9.4/scripts/autodelete
--rwxr-xr-x   0 eric       (501) staff       (20)      226 2023-09-20 18:15:50.000000 ebookconverter-0.9.4/scripts/cron-dopush-social.sh
--rwxr-xr-x   0 eric       (501) staff       (20)     1852 2022-08-18 12:51:16.000000 ebookconverter-0.9.4/scripts/cron-dopush.sh
--rwxr-xr--   0 eric       (501) staff       (20)     1043 2021-08-26 15:02:12.000000 ebookconverter-0.9.4/scripts/cron-jekyll.sh
--rwxr-xr-x   0 eric       (501) staff       (20)      428 2022-08-18 13:04:36.000000 ebookconverter-0.9.4/scripts/cron-rebuild-files.sh
--rwxr-xr-x   0 eric       (501) staff       (20)      244 2021-09-02 06:13:21.000000 ebookconverter-0.9.4/scripts/ebookconverter
--rwxr-xr-x   0 eric       (501) staff       (20)      294 2021-09-02 06:13:21.000000 ebookconverter-0.9.4/scripts/fileinfo
--rwxr-xr-x   0 eric       (501) staff       (20)      228 2021-09-02 06:13:21.000000 ebookconverter-0.9.4/scripts/make_csv
--rwxr-xr-x   0 eric       (501) staff       (20)      287 2022-07-26 15:05:15.000000 ebookconverter-0.9.4/scripts/reload_workflow
--rwxr-xr-x   0 eric       (501) staff       (20)      487 2023-09-29 17:18:19.000000 ebookconverter-0.9.4/scripts/txt-tarball
--rwxr-xr-x   0 eric       (501) staff       (20)      299 2022-09-14 21:30:51.000000 ebookconverter-0.9.4/scripts/update_from_backup_workflow
--rw-r--r--   0 eric       (501) staff       (20)       38 2024-02-27 00:19:28.635092 ebookconverter-0.9.4/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)     1674 2024-02-27 00:16:22.000000 ebookconverter-0.9.4/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-04-23 02:21:46.883701 ebookconverter-0.9.5/
+-rw-r--r--   0 eric       (501) staff       (20)    10877 2024-04-23 02:18:44.000000 ebookconverter-0.9.5/CHANGES
+-rw-r--r--   0 eric       (501) staff       (20)    35149 2018-12-20 21:57:45.000000 ebookconverter-0.9.5/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     2760 2024-04-23 02:21:46.883364 ebookconverter-0.9.5/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1903 2022-11-18 17:54:42.000000 ebookconverter-0.9.5/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-04-23 02:21:46.877345 ebookconverter-0.9.5/ebookconverter/
+-rwxr-xr-x   0 eric       (501) staff       (20)     2954 2021-09-02 06:13:21.000000 ebookconverter-0.9.5/ebookconverter/AutoDelete.py
+-rw-r--r--   0 eric       (501) staff       (20)     1602 2021-08-11 20:29:59.000000 ebookconverter-0.9.5/ebookconverter/CSV.py
+-rw-r--r--   0 eric       (501) staff       (20)     2626 2021-10-21 15:37:14.000000 ebookconverter-0.9.5/ebookconverter/Candidates.py
+-rw-r--r--   0 eric       (501) staff       (20)    22828 2024-04-01 17:15:37.000000 ebookconverter-0.9.5/ebookconverter/EbookConverter.py
+-rwxr-xr-x   0 eric       (501) staff       (20)    10715 2024-02-26 21:53:15.000000 ebookconverter-0.9.5/ebookconverter/FileInfo.py
+-rw-r--r--   0 eric       (501) staff       (20)     5557 2023-03-06 20:45:09.000000 ebookconverter-0.9.5/ebookconverter/Notifier.py
+-rw-r--r--   0 eric       (501) staff       (20)     2070 2022-09-14 19:47:10.000000 ebookconverter-0.9.5/ebookconverter/ReloadWorkflow.py
+-rw-r--r--   0 eric       (501) staff       (20)     3506 2024-04-16 21:46:40.000000 ebookconverter-0.9.5/ebookconverter/UpdateFromWorkflow.py
+-rw-r--r--   0 eric       (501) staff       (20)       18 2024-04-23 02:17:27.000000 ebookconverter-0.9.5/ebookconverter/Version.py
+-rw-r--r--   0 eric       (501) staff       (20)       27 2014-08-23 15:53:05.000000 ebookconverter-0.9.5/ebookconverter/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-04-23 02:21:46.880312 ebookconverter-0.9.5/ebookconverter/writers/
+-rw-r--r--   0 eric       (501) staff       (20)     1707 2021-10-18 22:59:45.000000 ebookconverter-0.9.5/ebookconverter/writers/CoverWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     3193 2024-04-18 16:30:06.000000 ebookconverter-0.9.5/ebookconverter/writers/FacebookWriter.py
+-rwxr-xr-x   0 eric       (501) staff       (20)     2542 2024-02-27 00:08:52.000000 ebookconverter-0.9.5/ebookconverter/writers/HTMLWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     2863 2023-09-20 18:15:50.000000 ebookconverter-0.9.5/ebookconverter/writers/MastodonWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     1330 2021-09-02 06:13:21.000000 ebookconverter-0.9.5/ebookconverter/writers/QRCodeWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     7235 2023-11-30 19:30:16.000000 ebookconverter-0.9.5/ebookconverter/writers/RDFWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     3024 2019-09-17 19:12:37.000000 ebookconverter-0.9.5/ebookconverter/writers/TwitterWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)     1387 2022-09-29 19:43:00.000000 ebookconverter-0.9.5/ebookconverter/writers/UpdateWriter.py
+-rw-r--r--   0 eric       (501) staff       (20)       10 2014-02-08 17:56:38.000000 ebookconverter-0.9.5/ebookconverter/writers/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-04-23 02:21:46.883003 ebookconverter-0.9.5/ebookconverter.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)     2760 2024-04-23 02:21:46.000000 ebookconverter-0.9.5/ebookconverter.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1114 2024-04-23 02:21:46.000000 ebookconverter-0.9.5/ebookconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2024-04-23 02:21:46.000000 ebookconverter-0.9.5/ebookconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)      124 2024-04-23 02:21:46.000000 ebookconverter-0.9.5/ebookconverter.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       15 2024-04-23 02:21:46.000000 ebookconverter-0.9.5/ebookconverter.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-04-23 02:21:46.882606 ebookconverter-0.9.5/scripts/
+-rwxr-xr-x   0 eric       (501) staff       (20)      302 2021-09-02 06:13:21.000000 ebookconverter-0.9.5/scripts/autodelete
+-rwxr-xr-x   0 eric       (501) staff       (20)      226 2023-09-20 18:15:50.000000 ebookconverter-0.9.5/scripts/cron-dopush-social.sh
+-rwxr-xr-x   0 eric       (501) staff       (20)     1852 2022-08-18 12:51:16.000000 ebookconverter-0.9.5/scripts/cron-dopush.sh
+-rwxr-xr--   0 eric       (501) staff       (20)     1043 2021-08-26 15:02:12.000000 ebookconverter-0.9.5/scripts/cron-jekyll.sh
+-rwxr-xr-x   0 eric       (501) staff       (20)      428 2022-08-18 13:04:36.000000 ebookconverter-0.9.5/scripts/cron-rebuild-files.sh
+-rwxr-xr-x   0 eric       (501) staff       (20)      244 2021-09-02 06:13:21.000000 ebookconverter-0.9.5/scripts/ebookconverter
+-rwxr-xr-x   0 eric       (501) staff       (20)      294 2021-09-02 06:13:21.000000 ebookconverter-0.9.5/scripts/fileinfo
+-rwxr-xr-x   0 eric       (501) staff       (20)      228 2021-09-02 06:13:21.000000 ebookconverter-0.9.5/scripts/make_csv
+-rwxr-xr-x   0 eric       (501) staff       (20)      287 2022-07-26 15:05:15.000000 ebookconverter-0.9.5/scripts/reload_workflow
+-rwxr-xr-x   0 eric       (501) staff       (20)      487 2023-09-29 17:18:19.000000 ebookconverter-0.9.5/scripts/txt-tarball
+-rwxr-xr-x   0 eric       (501) staff       (20)      299 2022-09-14 21:30:51.000000 ebookconverter-0.9.5/scripts/update_from_workflow
+-rw-r--r--   0 eric       (501) staff       (20)       38 2024-04-23 02:21:46.883766 ebookconverter-0.9.5/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)     1667 2024-04-23 02:21:09.000000 ebookconverter-0.9.5/setup.py
```

### Comparing `ebookconverter-0.9.4/CHANGES` & `ebookconverter-0.9.5/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+0.9.5 (April 22, 2024)
+- Change Facebook graph API version to 19.0. No changes affect us.
+- update_from_backup_workflow changed to update_from_workflow to add pubinfo from json files made before version 0.7.0 was turned on (~ August 2021)
+- ReparseCredits looks at books without credits and checks to see if parsing the pg header helps.
+- update libgutenberg to 0.10.24, fixes author ordering
+
+
 0.9.4 (February 26, 2024)
 - fix bad error handling in FileInfo
 - don't save new credit unless it's new
 - libgutenberg 0.10.22 
     - fixes bugs that resulted in duplicate credits
     - fixes a problem that scraped credits overwrote the changes from json file
```

### Comparing `ebookconverter-0.9.4/LICENSE` & `ebookconverter-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/PKG-INFO` & `ebookconverter-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebookconverter
-Version: 0.9.4
+Version: 0.9.5
 Summary: The Project Gutenberg tool to orchestrate ebook generation.
 Home-page: https://github.com/gutenbergtools/ebookconverter/
 Author: Eric Hellman
 Author-email: eric@hellman.org
 License: GPL v3
 Platform: OS-independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 Requires-Dist: ebookmaker>=0.12.40
 Requires-Dist: setproctitle==1.1.10
 Requires-Dist: requests_oauthlib>=1.2.0
 Requires-Dist: rdflib>=4.2.2
 Requires-Dist: qrcode>=6.1
-Requires-Dist: libgutenberg[postgres]>=0.10.22
+Requires-Dist: libgutenberg[postgres]>=0.10.24
 
 # ebookconverter
 code that orchestrates ebook conversion for project gutenberg
 
 
 EbookConverter manages the creation and update of ebook assets for Project Gutenberg. It uses a postgres database to keep track of both ebook metadata and ebook files. the postgress database is managed by the libgutenberg package.
```

### Comparing `ebookconverter-0.9.4/README.md` & `ebookconverter-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/AutoDelete.py` & `ebookconverter-0.9.5/ebookconverter/AutoDelete.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/CSV.py` & `ebookconverter-0.9.5/ebookconverter/CSV.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/Candidates.py` & `ebookconverter-0.9.5/ebookconverter/Candidates.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/EbookConverter.py` & `ebookconverter-0.9.5/ebookconverter/EbookConverter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/FileInfo.py` & `ebookconverter-0.9.5/ebookconverter/FileInfo.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/Notifier.py` & `ebookconverter-0.9.5/ebookconverter/Notifier.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/ReloadWorkflow.py` & `ebookconverter-0.9.5/ebookconverter/ReloadWorkflow.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/UpdateFromWorkflow.py` & `ebookconverter-0.9.5/ebookconverter/UpdateFromWorkflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import stat
 
 from libgutenberg import Logger
 from libgutenberg.DublinCore import handle_dc_languages
 from libgutenberg.DublinCoreMapping import DublinCoreObject
 from libgutenberg.GutenbergGlobals import Struct
 
-from ebookconverter.FileInfo import get_workflow_file, WORKFLOW_LOG_DIR
+from ebookconverter.FileInfo import get_workflow_file, WORKFLOW_LOG_DIR, archive_workflow_file
 
 WORKFLOW_BACKUP_DIR = os.path.join(WORKFLOW_LOG_DIR, 'backup')
 
 
 def update_from_workflow(dc, record):
     # check if there's a pubinfo, if so, don't update it.
     has_pubinfo = dc.pubinfo and bool(
@@ -70,16 +70,16 @@
         Logger.info('updated #%s', dc.project_gutenberg_id)
 
 
 def main():
     Logger.setup(Logger.LOGFORMAT, 'fileinfo.log')
     Logger.set_log_level(2)
 
-    for filename in sorted(os.listdir(WORKFLOW_BACKUP_DIR)):
-        workflow_file = os.path.join(WORKFLOW_BACKUP_DIR, filename)
+    for filename in sorted(os.listdir(WORKFLOW_LOG_DIR)):
+        workflow_file = os.path.join(WORKFLOW_LOG_DIR, filename)
         mode = os.stat(workflow_file)[stat.ST_MODE]
         if stat.S_ISDIR(mode):
             continue
         ebook_num = 0
         m = re.match(r'^(\d+)\.json$', filename)
         if m:
             ebook_num = int(m.group(1))
@@ -92,10 +92,11 @@
         data = json.loads(wf_data)
         record = data['DATA']
 
         dc = DublinCoreObject()
         dc.load_from_database(ebook_num)
         if dc.book:
             update_from_workflow(dc, record)
+        archive_workflow_file(workflow_file)
 
 if __name__ == '__main__':
     main()
```

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/CoverWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/CoverWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/FacebookWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/FacebookWriter.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from libgutenberg.Logger import exception, error, info, debug
 from libgutenberg.GutenbergGlobals import SkipOutputFormat
 
 from ebookmaker import writers
 
 PGURL = "https://www.gutenberg.org/"
 
-GRAPH = "https://graph.facebook.com/v13.0/"
+GRAPH = "https://graph.facebook.com/v19.0/"
 
 class Writer (writers.BaseWriter):
     """ Class to post about new ebooks.
 
     """
 
     __instance = None
```

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/HTMLWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/HTMLWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/MastodonWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/MastodonWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/QRCodeWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/QRCodeWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/RDFWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/RDFWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/TwitterWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/TwitterWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter/writers/UpdateWriter.py` & `ebookconverter-0.9.5/ebookconverter/writers/UpdateWriter.py`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/ebookconverter.egg-info/PKG-INFO` & `ebookconverter-0.9.5/ebookconverter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebookconverter
-Version: 0.9.4
+Version: 0.9.5
 Summary: The Project Gutenberg tool to orchestrate ebook generation.
 Home-page: https://github.com/gutenbergtools/ebookconverter/
 Author: Eric Hellman
 Author-email: eric@hellman.org
 License: GPL v3
 Platform: OS-independent
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.7
 License-File: LICENSE
 Requires-Dist: ebookmaker>=0.12.40
 Requires-Dist: setproctitle==1.1.10
 Requires-Dist: requests_oauthlib>=1.2.0
 Requires-Dist: rdflib>=4.2.2
 Requires-Dist: qrcode>=6.1
-Requires-Dist: libgutenberg[postgres]>=0.10.22
+Requires-Dist: libgutenberg[postgres]>=0.10.24
 
 # ebookconverter
 code that orchestrates ebook conversion for project gutenberg
 
 
 EbookConverter manages the creation and update of ebook assets for Project Gutenberg. It uses a postgres database to keep track of both ebook metadata and ebook files. the postgress database is managed by the libgutenberg package.
```

### Comparing `ebookconverter-0.9.4/ebookconverter.egg-info/SOURCES.txt` & `ebookconverter-0.9.5/ebookconverter.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 scripts/cron-jekyll.sh
 scripts/cron-rebuild-files.sh
 scripts/ebookconverter
 scripts/fileinfo
 scripts/make_csv
 scripts/reload_workflow
 scripts/txt-tarball
-scripts/update_from_backup_workflow
+scripts/update_from_workflow
```

### Comparing `ebookconverter-0.9.4/scripts/cron-dopush.sh` & `ebookconverter-0.9.5/scripts/cron-dopush.sh`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/scripts/cron-jekyll.sh` & `ebookconverter-0.9.5/scripts/cron-jekyll.sh`

 * *Files identical despite different names*

### Comparing `ebookconverter-0.9.4/setup.py` & `ebookconverter-0.9.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # ebookconverter distribution
 #
 
 from setuptools import setup
 
-VERSION = '0.9.4'
+VERSION = '0.9.5'
 
 setup (
     name = 'ebookconverter',
     version = VERSION,
 
     packages = [
         'ebookconverter',
@@ -17,29 +17,29 @@
 
     scripts = [
         'scripts/autodelete',
         'scripts/ebookconverter',
         'scripts/fileinfo',
         'scripts/make_csv',
         'scripts/reload_workflow',
-        'scripts/update_from_backup_workflow',
+        'scripts/update_from_workflow',
         'scripts/cron-rebuild-files.sh',
         'scripts/cron-dopush-social.sh',
         'scripts/cron-dopush.sh',
         'scripts/cron-jekyll.sh',
         'scripts/txt-tarball'
     ],
 
     install_requires = [
         'ebookmaker>=0.12.40',
         'setproctitle==1.1.10',
         'requests_oauthlib>=1.2.0',
         'rdflib>=4.2.2',
         'qrcode>=6.1',
-        'libgutenberg[postgres]>=0.10.22',
+        'libgutenberg[postgres]>=0.10.24',
     ],
     
     package_data = {
     },
 
     data_files = [
         ('', ['CHANGES', 'README.md']),
```

