# Comparing `tmp/youtube_comment_downloader-0.1.74.tar.gz` & `tmp/youtube_comment_downloader-0.1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube_comment_downloader-0.1.74.tar", last modified: Tue Apr 23 16:13:25 2024, max compression
+gzip compressed data, was "youtube_comment_downloader-0.1.75.tar", last modified: Tue Apr 23 17:12:59 2024, max compression
```

## Comparing `youtube_comment_downloader-0.1.74.tar` & `youtube_comment_downloader-0.1.75.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:25.852496 youtube_comment_downloader-0.1.74/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-23 16:13:25.852496 youtube_comment_downloader-0.1.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-23 16:13:25.852496 youtube_comment_downloader-0.1.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:25.852496 youtube_comment_downloader-0.1.74/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/tests/test_search_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:25.852496 youtube_comment_downloader-0.1.74/youtube_comment_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8022 2024-04-23 16:13:17.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 16:13:25.852496 youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-23 16:13:25.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 16:13:25.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 16:13:25.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 16:13:25.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 16:13:25.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 16:13:25.000000 youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:12:59.203582 youtube_comment_downloader-0.1.75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-23 17:12:59.203582 youtube_comment_downloader-0.1.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-23 17:12:59.207582 youtube_comment_downloader-0.1.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:12:59.203582 youtube_comment_downloader-0.1.75/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/tests/test_search_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:12:59.203582 youtube_comment_downloader-0.1.75/youtube_comment_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8024 2024-04-23 17:12:47.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:12:59.203582 youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-23 17:12:59.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 17:12:59.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:12:59.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-23 17:12:59.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 17:12:59.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 17:12:59.000000 youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/top_level.txt
```

### Comparing `youtube_comment_downloader-0.1.74/LICENSE` & `youtube_comment_downloader-0.1.75/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube_comment_downloader-0.1.74/PKG-INFO` & `youtube_comment_downloader-0.1.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-comment-downloader
-Version: 0.1.74
+Version: 0.1.75
 Summary: Simple script for downloading Youtube comments without using the Youtube API
 Home-page: https://github.com/egbertbouman/youtube-comment-downloader
 Author: Egbert Bouman
 Author-email: ebouman@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

### Comparing `youtube_comment_downloader-0.1.74/README.md` & `youtube_comment_downloader-0.1.75/README.md`

 * *Files identical despite different names*

### Comparing `youtube_comment_downloader-0.1.74/setup.cfg` & `youtube_comment_downloader-0.1.75/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = youtube-comment-downloader
-version = 0.1.74
+version = 0.1.75
 description = Simple script for downloading Youtube comments without using the Youtube API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license-file = LICENSE
 url = https://github.com/egbertbouman/youtube-comment-downloader
 author = Egbert Bouman
```

### Comparing `youtube_comment_downloader-0.1.74/tests/test_search_dict.py` & `youtube_comment_downloader-0.1.75/tests/test_search_dict.py`

 * *Files identical despite different names*

### Comparing `youtube_comment_downloader-0.1.74/youtube_comment_downloader/__init__.py` & `youtube_comment_downloader-0.1.75/youtube_comment_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube_comment_downloader-0.1.74/youtube_comment_downloader/downloader.py` & `youtube_comment_downloader-0.1.75/youtube_comment_downloader/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
                 toolbar = comment['toolbar']
                 toolbar_state = toolbar_states[properties['toolbarStateKey']]
                 result = {'cid': cid,
                           'text': properties['content']['content'],
                           'time': properties['publishedTime'],
                           'author': author['displayName'],
                           'channel': author['channelId'],
-                          'votes': toolbar['likeCountNotliked'].strip() or 0,
+                          'votes': toolbar['likeCountNotliked'].strip() or `0`,
                           'replies': toolbar['replyCount'],
                           'photo': author['avatarThumbnailUrl'],
                           'heart': toolbar_state.get('heartState', '') == 'TOOLBAR_HEART_STATE_HEARTED',
                           'reply': '.' in cid}
 
                 try:
                     result['time_parsed'] = dateparser.parse(result['time'].split('(')[0].strip()).timestamp()
```

### Comparing `youtube_comment_downloader-0.1.74/youtube_comment_downloader.egg-info/PKG-INFO` & `youtube_comment_downloader-0.1.75/youtube_comment_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-comment-downloader
-Version: 0.1.74
+Version: 0.1.75
 Summary: Simple script for downloading Youtube comments without using the Youtube API
 Home-page: https://github.com/egbertbouman/youtube-comment-downloader
 Author: Egbert Bouman
 Author-email: ebouman@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

