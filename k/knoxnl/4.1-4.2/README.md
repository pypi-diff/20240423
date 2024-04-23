# Comparing `tmp/knoxnl-4.1.tar.gz` & `tmp/knoxnl-4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knoxnl-4.1.tar", last modified: Mon Apr 22 14:02:27 2024, max compression
+gzip compressed data, was "knoxnl-4.2.tar", last modified: Tue Apr 23 20:48:19 2024, max compression
```

## Comparing `knoxnl-4.1.tar` & `knoxnl-4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-22 14:02:27.547397 knoxnl-4.1/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-12 20:07:00.000000 knoxnl-4.1/LICENSE
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    17171 2024-04-22 14:02:27.539694 knoxnl-4.1/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    16780 2024-04-04 17:13:37.000000 knoxnl-4.1/README.md
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-22 14:02:27.193728 knoxnl-4.1/knoxnl/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-04 14:07:43.000000 knoxnl-4.1/knoxnl/__init__.py
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    43488 2024-04-22 11:05:25.000000 knoxnl-4.1/knoxnl/knoxnl.py
-drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-22 14:02:27.525722 knoxnl-4.1/knoxnl.egg-info/
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)    17171 2024-04-22 14:02:26.000000 knoxnl-4.1/knoxnl.egg-info/PKG-INFO
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)      273 2024-04-22 14:02:27.000000 knoxnl-4.1/knoxnl.egg-info/SOURCES.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-22 14:02:26.000000 knoxnl-4.1/knoxnl.egg-info/dependency_links.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       46 2024-04-22 14:02:26.000000 knoxnl-4.1/knoxnl.egg-info/entry_points.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-03-15 11:47:02.000000 knoxnl-4.1/knoxnl.egg-info/not-zip-safe
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       44 2024-04-22 14:02:26.000000 knoxnl-4.1/knoxnl.egg-info/requires.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)        7 2024-04-22 14:02:26.000000 knoxnl-4.1/knoxnl.egg-info/top_level.txt
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-22 14:02:27.548937 knoxnl-4.1/setup.cfg
--rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2347 2024-04-04 20:24:25.000000 knoxnl-4.1/setup.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 20:48:19.374326 knoxnl-4.2/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     1068 2024-03-12 20:07:00.000000 knoxnl-4.2/LICENSE
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    17171 2024-04-23 20:48:19.361412 knoxnl-4.2/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    16780 2024-04-23 20:46:05.000000 knoxnl-4.2/README.md
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 20:48:19.078777 knoxnl-4.2/knoxnl/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       17 2024-04-23 20:45:59.000000 knoxnl-4.2/knoxnl/__init__.py
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    43489 2024-04-23 20:47:58.000000 knoxnl-4.2/knoxnl/knoxnl.py
+drwxrwxrwx   0 xnl       (1000) xnl       (1000)        0 2024-04-23 20:48:19.345332 knoxnl-4.2/knoxnl.egg-info/
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)    17171 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/PKG-INFO
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)      273 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       46 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/entry_points.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        1 2024-03-15 11:47:02.000000 knoxnl-4.2/knoxnl.egg-info/not-zip-safe
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       44 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/requires.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)        7 2024-04-23 20:48:18.000000 knoxnl-4.2/knoxnl.egg-info/top_level.txt
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)       38 2024-04-23 20:48:19.376408 knoxnl-4.2/setup.cfg
+-rwxrwxrwx   0 xnl       (1000) xnl       (1000)     2347 2024-04-04 20:24:25.000000 knoxnl-4.2/setup.py
```

### Comparing `knoxnl-4.1/LICENSE` & `knoxnl-4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `knoxnl-4.1/PKG-INFO` & `knoxnl-4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: knoxnl
-Version: 4.1
+Version: 4.2
 Summary: A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)
 Home-page: https://github.com/xnl-h4ck3r/knoxnl
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: termcolor
 Requires-Dist: pyaml
 Requires-Dist: urlparse3
 
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.1
+## About - v4.2
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
 ## Installation
```

### Comparing `knoxnl-4.1/README.md` & `knoxnl-4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.1
+## About - v4.2
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
 ## Installation
```

### Comparing `knoxnl-4.1/knoxnl/knoxnl.py` & `knoxnl-4.2/knoxnl/knoxnl.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,15 +301,15 @@
                      'User-Agent' : 'knoXnl tool by @xnl-h4ck3r'
                      }
         
         # Replace any & in the URL with encoded value so we can add other data using &
         targetData = targetUrl.replace('&', '%26')
     
         # Also encode + so it doesn't get converted to space
-        targetData = targetUrl.replace('+', '%2B')
+        targetData = targetData.replace('+', '%2B')
     
         # If processing a POST
         if method == 'POST' and args.http_method in ('POST','BOTH'):
             postData = ''
             
             # If the --post-data argument was passed, use those values
             if args.post_data != '':
```

### Comparing `knoxnl-4.1/knoxnl.egg-info/PKG-INFO` & `knoxnl-4.2/knoxnl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: knoxnl
-Version: 4.1
+Version: 4.2
 Summary: A python wrapper around the amazing KNOXSS API by Brute Logic (requires an API Key)
 Home-page: https://github.com/xnl-h4ck3r/knoxnl
 Author: @xnl-h4ck3r
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: argparse
 Requires-Dist: requests
 Requires-Dist: termcolor
 Requires-Dist: pyaml
 Requires-Dist: urlparse3
 
 <center><img src="https://github.com/xnl-h4ck3r/knoxnl/blob/main/knoxnl/images/title.png"></center>
 
-## About - v4.1
+## About - v4.2
 
 This is a python wrapper around the amazing [KNOXSS API](https://knoxss.me/?page_id=2729) by Brute Logic.
 To use this tool (and the underlying API), you must have a valid KNOXSS API key. Don't have one? Go visit https://knoxss.me and subscribe!
 This was inspired by the ["knoxssme" tool](https://github.com/edoardottt/lit-bb-hack-tools/tree/main/knoxssme) by @edoardottt2, but developed to allow for greater options.
 
 ## Installation
```

### Comparing `knoxnl-4.1/setup.py` & `knoxnl-4.2/setup.py`

 * *Files identical despite different names*

