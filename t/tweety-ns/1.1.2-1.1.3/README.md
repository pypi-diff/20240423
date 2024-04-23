# Comparing `tmp/tweety-ns-1.1.2.tar.gz` & `tmp/tweety_ns-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-1.1.2.tar", last modified: Wed Apr 10 16:36:42 2024, max compression
+gzip compressed data, was "tweety_ns-1.1.3.tar", last modified: Tue Apr 23 08:18:05 2024, max compression
```

## Comparing `tweety-ns-1.1.2.tar` & `tweety_ns-1.1.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety-ns-1.1.2/README.md
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-1.1.2/pyproject.toml
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/setup.cfg
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-10 16:36:05.000000 tweety-ns-1.1.2/setup.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.181096 tweety-ns-1.1.2/src/
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.185096 tweety-ns-1.1.2/src/tweety/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-10 16:35:52.000000 tweety-ns-1.1.2/src/tweety/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7504 2024-03-04 12:19:25.000000 tweety-ns-1.1.2/src/tweety/auth.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31876 2024-04-10 16:30:28.000000 tweety-ns-1.1.2/src/tweety/bot.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    95767 2024-03-20 11:19:15.000000 tweety-ns-1.1.2/src/tweety/builder.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.185096 tweety-ns-1.1.2/src/tweety/events/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety-ns-1.1.2/src/tweety/events/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2119 2024-03-31 11:29:17.000000 tweety-ns-1.1.2/src/tweety/events/newmessage.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22014 2024-04-10 16:25:45.000000 tweety-ns-1.1.2/src/tweety/exceptions_.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2341 2024-03-03 15:25:23.000000 tweety-ns-1.1.2/src/tweety/filters.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20098 2024-03-20 05:50:42.000000 tweety-ns-1.1.2/src/tweety/http.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety-ns-1.1.2/src/tweety/session.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/src/tweety/types/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety-ns-1.1.2/src/tweety/types/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3039 2024-02-12 12:06:11.000000 tweety-ns-1.1.2/src/tweety/types/base.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety-ns-1.1.2/src/tweety/types/bookmarks.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety-ns-1.1.2/src/tweety/types/community.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety-ns-1.1.2/src/tweety/types/follow.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety-ns-1.1.2/src/tweety/types/gifs.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    17540 2024-04-04 20:48:50.000000 tweety-ns-1.1.2/src/tweety/types/inbox.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety-ns-1.1.2/src/tweety/types/likes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety-ns-1.1.2/src/tweety/types/lists.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety-ns-1.1.2/src/tweety/types/mentions.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9022 2024-04-10 16:29:13.000000 tweety-ns-1.1.2/src/tweety/types/n_types.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety-ns-1.1.2/src/tweety/types/notification.py
--rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety-ns-1.1.2/src/tweety/types/places.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety-ns-1.1.2/src/tweety/types/retweets.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety-ns-1.1.2/src/tweety/types/search.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety-ns-1.1.2/src/tweety/types/topic.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58413 2024-03-27 06:41:42.000000 tweety-ns-1.1.2/src/tweety/types/twDataTypes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-03-18 07:58:43.000000 tweety-ns-1.1.2/src/tweety/types/usertweet.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety-ns-1.1.2/src/tweety/updates.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36036 2024-03-20 05:54:31.000000 tweety-ns-1.1.2/src/tweety/user.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6192 2024-03-04 11:48:15.000000 tweety-ns-1.1.2/src/tweety/utils.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-10 16:36:42.189096 tweety-ns-1.1.2/src/tweety_ns.egg-info/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/SOURCES.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/dependency_links.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/requires.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-10 16:36:42.000000 tweety-ns-1.1.2/src/tweety_ns.egg-info/top_level.txt
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety_ns-1.1.3/README.md
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety_ns-1.1.3/pyproject.toml
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/setup.cfg
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-23 07:11:33.000000 tweety_ns-1.1.3/setup.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.697319 tweety_ns-1.1.3/src/
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.701319 tweety_ns-1.1.3/src/tweety/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-23 07:11:42.000000 tweety_ns-1.1.3/src/tweety/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7486 2024-04-12 13:05:42.000000 tweety_ns-1.1.3/src/tweety/auth.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31953 2024-04-23 07:05:13.000000 tweety_ns-1.1.3/src/tweety/bot.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    96143 2024-04-23 07:05:23.000000 tweety_ns-1.1.3/src/tweety/builder.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.701319 tweety_ns-1.1.3/src/tweety/events/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety_ns-1.1.3/src/tweety/events/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2119 2024-03-31 11:29:17.000000 tweety_ns-1.1.3/src/tweety/events/newmessage.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    22029 2024-04-14 08:52:30.000000 tweety_ns-1.1.3/src/tweety/exceptions_.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2343 2024-04-23 07:03:34.000000 tweety_ns-1.1.3/src/tweety/filters.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20431 2024-04-23 06:55:33.000000 tweety_ns-1.1.3/src/tweety/http.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2362 2024-04-10 16:34:41.000000 tweety_ns-1.1.3/src/tweety/session.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.701319 tweety_ns-1.1.3/src/tweety/types/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety_ns-1.1.3/src/tweety/types/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3039 2024-02-12 12:06:11.000000 tweety_ns-1.1.3/src/tweety/types/base.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety_ns-1.1.3/src/tweety/types/bookmarks.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety_ns-1.1.3/src/tweety/types/community.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety_ns-1.1.3/src/tweety/types/follow.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety_ns-1.1.3/src/tweety/types/gifs.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    17540 2024-04-04 20:48:50.000000 tweety_ns-1.1.3/src/tweety/types/inbox.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety_ns-1.1.3/src/tweety/types/likes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety_ns-1.1.3/src/tweety/types/lists.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety_ns-1.1.3/src/tweety/types/mentions.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9022 2024-04-10 16:29:13.000000 tweety_ns-1.1.3/src/tweety/types/n_types.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety_ns-1.1.3/src/tweety/types/notification.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety_ns-1.1.3/src/tweety/types/places.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety_ns-1.1.3/src/tweety/types/retweets.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety_ns-1.1.3/src/tweety/types/search.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety_ns-1.1.3/src/tweety/types/topic.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58815 2024-04-14 08:56:44.000000 tweety_ns-1.1.3/src/tweety/types/twDataTypes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-04-12 07:15:06.000000 tweety_ns-1.1.3/src/tweety/types/usertweet.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety_ns-1.1.3/src/tweety/updates.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36382 2024-04-23 03:37:43.000000 tweety_ns-1.1.3/src/tweety/user.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6531 2024-04-23 07:05:23.000000 tweety_ns-1.1.3/src/tweety/utils.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-23 08:18:05.705319 tweety_ns-1.1.3/src/tweety_ns.egg-info/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/requires.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-23 08:18:05.000000 tweety_ns-1.1.3/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-1.1.2/PKG-INFO` & `tweety_ns-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.2
+Version: 1.1.3
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-1.1.2/README.md` & `tweety_ns-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/setup.cfg` & `tweety_ns-1.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tweety-ns
-version = 1.1.2
+version = 1.1.3
 author = Tayyab Kharl
 author_email = tayyabmahr@gmail.com
 description = An easy Twitter Scraper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mahrtayyab/tweety
 project_urls =
```

### Comparing `tweety-ns-1.1.2/setup.py` & `tweety_ns-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types', 'tweety.events'],
-    version='1.1.2',
+    version='1.1.3',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
```

### Comparing `tweety-ns-1.1.2/src/tweety/auth.py` & `tweety_ns-1.1.3/src/tweety/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import getpass
-import traceback
 from http.cookiejar import MozillaCookieJar
 from typing import Union
 from .exceptions_ import InvalidCredentials, DeniedLogin, ActionRequired
 from .builder import FlowData
 from .types.n_types import Cookies
 from .utils import find_objects
```

### Comparing `tweety-ns-1.1.2/src/tweety/bot.py` & `tweety_ns-1.1.3/src/tweety/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import traceback
 import warnings
 from typing import Union
-from .utils import find_objects, AuthRequired, get_user_from_typehead, get_tweet_id
+from .utils import find_objects, AuthRequired, get_user_from_typehead, get_tweet_id, check_translation_lang
 from .types import (Proxy, TweetComments, UserTweets, Search, User, Tweet, Trends, Community, CommunityTweets,
                     CommunityMembers, UserFollowers, UserFollowings, TweetHistory, UserMedia, GifSearch,
                     ShortUser, TypeHeadSearch, TweetTranslate, AudioSpace, UserHighlights, UserLikes, Places)
 from .exceptions_ import *
 from .session import Session, MemorySession, FileSession
 from .http import Request
 
@@ -833,14 +833,15 @@
 
             :param tweet_id: Tweet ID of the Tweet to be translated
             :param language: In which Language you want to translate the Tweet (see tweety.filters.Language)
             :return: .types.twDataTypes.TweetTranslate
         """
 
         tweetId = get_tweet_id(tweet_id)
+        language = check_translation_lang(language)
         response = self.http.get_tweet_translation(tweetId, language)
         return TweetTranslate(self, response)
 
     def search_gifs(self, search_term, pages=1, cursor=None, wait_time=2):
         search = GifSearch(search_term, self, pages, cursor, wait_time)
         list(search.generator())
         return search
```

### Comparing `tweety-ns-1.1.2/src/tweety/builder.py` & `tweety_ns-1.1.3/src/tweety/builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
     URL_AUSER_CREATE_LIST = "https://twitter.com/i/api/graphql/nHFMQuE4PMED1R0JTN4d-Q/CreateList"  # noqa
     URL_AUSER_DELETE_LIST = "https://twitter.com/i/api/graphql/UnN9Th1BDbeLjpgjGSpL3Q/DeleteList"  # noqa
     URL_AUSER_GET_USER_FOLLOWERS = "https://twitter.com/i/api/graphql/ihMPm0x-pC35X86L_nUp_Q/Followers"  # noqa
     URL_AUSER_GET_USER_FOLLOWINGS = "https://twitter.com/i/api/graphql/bX-gXhcglOa--1gzgDlb8A/Following"  # noqa
     # URL_AUSER_GET_MUTUAL_FRIENDS = "https://twitter.com/i/api/1.1/friends/following/list.json"  # noqa
     URL_AUSER_GET_MUTUAL_FRIENDS = "https://twitter.com/i/api/graphql/35Y2QFmL84HIisnm-FHAng/FollowersYouKnow"  # noqa
     URL_AUSER_GET_BLOCKED_USERS = "https://twitter.com/i/api/graphql/f87G4V_l5E9rJ-Ylw0D-yQ/BlockedAccountsAll"  # noqa
+    URL_PIN_TWEET = "https://twitter.com/i/api/graphql/VIHsNu89pK-kW35JpHq7Xw/PinTweet"  # noqa
 
     def __init__(self):
         self.cookies = None
         self.user_id = None
         self.guest_token = None
         self.custom_headers = {}
 
@@ -1699,14 +1700,25 @@
 
         if cursor:
             variables['cursor'] = cursor
 
         params = {'variables': str(json.dumps(variables)), 'features': str(json.dumps(features))}
         return "GET", self._build(self.URL_TOPIC_LANDING, urlencode(params))
 
+    @return_with_headers
+    def pin_tweet(self, tweet_id):
+        json_data = {
+            'variables': {
+                'tweet_id': str(tweet_id),
+            },
+            'queryId': utils.create_query_id(),
+        }
+
+        return "POST", self.URL_PIN_TWEET, json_data
+
 
 class FlowData:
     IGNORE_MEMBERS = ['get']
 
     def __init__(self):
         self.initial_state = "startFlow"
```

### Comparing `tweety-ns-1.1.2/src/tweety/events/newmessage.py` & `tweety_ns-1.1.3/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/exceptions_.py` & `tweety_ns-1.1.3/src/tweety/exceptions_.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,30 @@
             message
     ):
         self.message = message
         self.error_code = error_code
         self.error_name = error_name
         self.response = response
 
-        if self.response is not None and not isinstance(self.response, dict) and not self.response.json_() and self.response.text:
+        if self.response is not None and not isinstance(self.response, dict) and not self.response.json() and self.response.text:
             self.message = self.response.text
         elif str(self.error_code) == "404":
             self.message = "Page not Found. Most likely you need elevated authorization to access this resource"
 
         super().__init__(self.message)
 
 
 class UserNotFound(TwitterError):
     """Exception raised when user isn't found.
 
     Attributes:
         message -- explanation of the error
     """
 
-    def __init__(self, error_code=50, error_name="GenericUserNotFound", response=None, message="The User Account wasn't Found", **kw):
+    def __init__(self, error_code=50, error_name="GenericUserNotFound", response=None, message="The User Account wasn't Found or is Protected", **kw):
         super().__init__(error_code, error_name, response, message)
 
 
 class GuestTokenNotFound(TwitterError):
     """
     Exception Raised when the guest token wasn't found after specific number of retires
```

### Comparing `tweety-ns-1.1.2/src/tweety/filters.py` & `tweety_ns-1.1.3/src/tweety/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,21 @@
         return "Community"
 
 class CommunityTweets:
     @staticmethod
     def Top():
         return "Top"
 
+
 class CommunityMembers:
     @staticmethod
     def Moderators():
         return "Mods"
 
+
 class Language:
     Urdu = URDU = "ur"
     Russian = RUSSIAN = "ru"
     Danish = DANISH = "da"
     Filipino = FILIPINO = "fil"
     Irish = IRISH = "ga"
     TraditionalChinese = TRADITIONAL_CHINESE = "zh-tw"
@@ -86,8 +88,8 @@
     Galician = GALICIAN = "gl"
     Korean = KOREAN = "ko"
     Serbian = SERBIAN = "sr"
     BritishEnglish = BRITISH_ENGLISH = "en-gb"
     Hindi = HINDI = "hi"
     Hebrew = HEBREW = "he"
     Malay = MALAY = "msa"
-    Bulgarian = BULGARIAN = "bg"
+    Bulgarian = BULGARIAN = "bg"
```

### Comparing `tweety-ns-1.1.2/src/tweety/http.py` & `tweety_ns-1.1.3/src/tweety/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import inspect
 import os
 import re
 import warnings
 from typing import Callable
 from urllib.parse import quote
-import httpx as s
+import httpx
 from .exceptions_ import GuestTokenNotFound, UnknownError, UserNotFound, InvalidCredentials
 from .types.n_types import GenericError
 from .utils import custom_json, GUEST_TOKEN_REGEX
 from .builder import UrlBuilder
 
-s.Response.json_ = custom_json
+httpx.Response.original_json = httpx.Response.json
+httpx.Response.json = custom_json
 
 
 class Request:
     def __init__(self, client, max_retries=10, proxy=None, **kwargs):
+
+        timeout = kwargs.pop("timeout", 60)
+
         self.user = None
         self.username = None
         self._client = client
         self._limits = {}
-        self.__session = s.Client(proxies=proxy, timeout=60, **kwargs)
+        self.__session = httpx.Client(proxies=proxy, timeout=timeout, **kwargs)
         self.__builder = UrlBuilder()
         self.__guest_token = self._get_guest_token(max_retries)
         self.__builder.guest_token = self.__guest_token
 
     @property
     def session(self):
         return self.__session
@@ -67,19 +71,19 @@
     def __get_response__(self, return_raw=False, ignore_none_data=False, is_document=False, **request_data):
 
         response = self.__session.request(**request_data)
         self._update_rate_limit(response, inspect.stack()[1][3])
         if is_document:
             return response
 
-        response_json = response.json_()  # noqa
+        response_json = response.json()  # noqa
         if ignore_none_data and len(response.text) == 0:
             return None
 
-        if response.text and response.text.lower() == "rate limit exceeded":
+        if (not response_json and response.text and response.text.lower() == "rate limit exceeded") or response.status_code == 429:
             response_json = {"errors": [{"code": 88, "message": "Rate limit exceeded."}]}
 
         if not response_json:
             raise UnknownError(
                 error_code=response.status_code,
                 error_name="Server Error",
                 response=response,
@@ -475,14 +479,19 @@
         return response
 
     def add_group_member(self, member_ids, conversation_id):
         request_data = self.__builder.add_member_to_group(member_ids, conversation_id)
         response = self.__get_response__(**request_data)
         return response
 
+    def pin_tweet(self, tweet_id):
+        request_data = self.__builder.pin_tweet(tweet_id)
+        response = self.__get_response__(**request_data)
+        return response
+
     def download_media(self, media_url, filename: str = None,
                        progress_callback: Callable[[str, int, int], None] = None):
         filename = os.path.basename(media_url).split("?")[0] if not filename else filename
         headers = self.__builder._get_headers()
         oldReferer = headers.get('Referer')
 
         if media_url.startswith("https://ton.twitter.com"):
```

### Comparing `tweety-ns-1.1.2/src/tweety/session.py` & `tweety_ns-1.1.3/src/tweety/session.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/__init__.py` & `tweety_ns-1.1.3/src/tweety/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/base.py` & `tweety_ns-1.1.3/src/tweety/types/base.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/bookmarks.py` & `tweety_ns-1.1.3/src/tweety/types/bookmarks.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/community.py` & `tweety_ns-1.1.3/src/tweety/types/community.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/follow.py` & `tweety_ns-1.1.3/src/tweety/types/follow.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/gifs.py` & `tweety_ns-1.1.3/src/tweety/types/gifs.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/inbox.py` & `tweety_ns-1.1.3/src/tweety/types/inbox.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/likes.py` & `tweety_ns-1.1.3/src/tweety/types/likes.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/lists.py` & `tweety_ns-1.1.3/src/tweety/types/lists.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/mentions.py` & `tweety_ns-1.1.3/src/tweety/types/mentions.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/n_types.py` & `tweety_ns-1.1.3/src/tweety/types/n_types.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/notification.py` & `tweety_ns-1.1.3/src/tweety/types/notification.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/places.py` & `tweety_ns-1.1.3/src/tweety/types/places.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/retweets.py` & `tweety_ns-1.1.3/src/tweety/types/retweets.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/search.py` & `tweety_ns-1.1.3/src/tweety/types/search.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/topic.py` & `tweety_ns-1.1.3/src/tweety/types/topic.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/types/twDataTypes.py` & `tweety_ns-1.1.3/src/tweety/types/twDataTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 class _TwType(dict):
     def __new__(cls, client, data, *args, **kwargs):
         if not data:
             return None
 
         return super().__new__(cls)
 
+    def get_raw(self):
+        return self._raw
+
     def __init_subclass__(cls, *args, **kwargs):
         super().__init_subclass__(*args, **kwargs)
 
         def new_init(self, *_args, init=cls.__init__, **_kwargs):
             init(self, *_args, **_kwargs) # noqa
             super().__init__()
 
@@ -240,23 +243,28 @@
     def get_comments(self, pages=1, wait_time=2, cursor=None, get_hidden=False):
         return self._client.get_tweet_comments(self.id, pages, wait_time, cursor, get_hidden)
 
     def iter_comments(self, pages=1, wait_time=2, cursor=None, get_hidden=False):
         return self._client.iter_tweet_comments(self.id, pages, wait_time, cursor, get_hidden)
 
     def _check_if_protected(self):
-
-        is_protected = find_objects(self._raw, "__typename", "TweetUnavailable", recursive=False)
+        is_protected = find_objects(self._raw, "__typename", ["TweetUnavailable", "TweetTombstone"], recursive=False)
 
         if is_protected and is_protected.get('reason') == "Protected":
             raise ProtectedTweet(403, "TweetUnavailable", response=self._raw)
         elif is_protected and is_protected.get('reason') == "NsfwLoggedOut":
             raise AuthenticationRequired(401, "NsfwLoggedOut", response=self._raw, message="This Tweet is flagged as NSFW, make sure you are logged-in and brithday is updated in your account.")
         elif is_protected and is_protected.get('reason') == "Suspended":
             raise UserProtected(error_code="UserSuspended", response=self._raw, message="The Author of this Tweet is Suspended")
+        elif is_protected and is_protected.get("tombstone"):
+            error_message = is_protected.get("tombstone", {}).get("text", {}).get("text")
+            if error_message:
+                raise UserProtected(response=self._raw, message=error_message)
+            else:
+                raise UserProtected(response=self._raw)
 
     def _format_tweet(self):
         self._check_if_protected()
         self._tweet = find_objects(self._raw, "__typename", ["Tweet", "TweetWithVisibilityResults"], recursive=False)
 
         if self._tweet.get('tweet'):
             self._tweet = self._tweet['tweet']
```

### Comparing `tweety-ns-1.1.2/src/tweety/types/usertweet.py` & `tweety_ns-1.1.3/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.2/src/tweety/user.py` & `tweety_ns-1.1.3/src/tweety/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1023,14 +1023,27 @@
             :param cursor: (`str`) Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
             :return: (.types.follow.BlockedUsers, List[.types.twDataTypes.User])
         """
 
         blocked_users = BlockedUsers(self, pages, wait_time, cursor)
         return blocked_users.generator()
 
+    def pin_tweet(self, tweet_id):
+        """
+            Pin a Tweet
+
+        :param tweet_id: (`str`, `int`, `Tweet`)
+        :return: bool
+        """
+
+        tweetId = get_tweet_id(tweet_id)
+
+        response = self.request.pin_tweet(tweetId)
+        return True if find_objects(response, "message", "post pinned successfully") else False
+
     def _upload_media(self, files, _type="tweet_image"):
         if not isinstance(files, list):
             files = [files]
 
         uploaded = []
 
         for file in files:
```

### Comparing `tweety-ns-1.1.2/src/tweety/utils.py` & `tweety_ns-1.1.3/src/tweety/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import re
 import string
 import sys
 import uuid
 from dateutil import parser as date_parser
 from urllib.parse import urlparse
 from .exceptions_ import AuthenticationRequired
+from .filters import Language
 
 GUEST_TOKEN_REGEX = re.compile("gt=(.*?);")
 MIME_TYPES = {
     "png": "image/png",
     "jpg": "image/jpeg",
     "jfif": "image/jpeg",
     "jpeg": "image/jpeg",
@@ -72,15 +73,15 @@
         return random.randint(*wait_time)
 
     return int(wait_time)
 
 
 def custom_json(self):
     try:
-        return self.json()
+        return self.original_json()
     except:
         return None
 
 
 def create_request_id():
     return str(uuid.uuid1())
 
@@ -216,8 +217,17 @@
     return None
 
 
 def get_tweet_id(tweet_identifier):
     if str(tweet_identifier.__class__.__name__) == "Tweet":
         return tweet_identifier.id
     else:
-        return urlparse(str(tweet_identifier)).path.split("/")[-1]
+        return urlparse(str(tweet_identifier)).path.split("/")[-1]
+
+
+def check_translation_lang(lang):
+    for k, v in vars(Language).items():
+        if not str(k).startswith("_"):
+            if str(k).lower() == str(lang).lower() or str(v).lower() == str(lang).lower():
+                return v
+
+    raise ValueError(f"Language {lang} is not supported")
```

### Comparing `tweety-ns-1.1.2/src/tweety_ns.egg-info/PKG-INFO` & `tweety_ns-1.1.3/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.2
+Version: 1.1.3
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-1.1.2/src/tweety_ns.egg-info/SOURCES.txt` & `tweety_ns-1.1.3/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

