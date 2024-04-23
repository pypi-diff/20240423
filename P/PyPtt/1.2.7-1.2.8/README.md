# Comparing `tmp/pyptt-1.2.7.tar.gz` & `tmp/pyptt-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyptt-1.2.7.tar", last modified: Sun Apr 21 13:21:35 2024, max compression
+gzip compressed data, was "pyptt-1.2.8.tar", last modified: Tue Apr 23 02:38:00 2024, max compression
```

## Comparing `pyptt-1.2.7.tar` & `pyptt-1.2.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:21:35.356844 pyptt-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-21 13:21:29.000000 pyptt-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-21 13:21:29.000000 pyptt-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-21 13:21:35.356844 pyptt-1.2.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:21:35.352844 pyptt-1.2.7/PyPtt/
--rw-r--r--   0 runner    (1001) docker     (127)    32101 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/PTT.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-21 13:21:35.000000 pyptt-1.2.7/PyPtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_call_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_change_pw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_del_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_board_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_board_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_bottom_post_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_favourite_board.py
--rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_newest_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_post_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_give_money.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_has_new_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_loginout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_mark_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_reply_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_search_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_set_board_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/_api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/check_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/connect_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:21:35.352844 pyptt-1.2.7/PyPtt/lang/
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/lang/en_US.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/lang/zh_TW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/lib_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    54872 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/screens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:21:35.356844 pyptt-1.2.7/PyPtt/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/ssl/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-21 13:21:29.000000 pyptt-1.2.7/PyPtt/ssl/key.pem
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:21:35.356844 pyptt-1.2.7/PyPtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-21 13:21:35.000000 pyptt-1.2.7/PyPtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-21 13:21:35.000000 pyptt-1.2.7/PyPtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:21:35.000000 pyptt-1.2.7/PyPtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 13:21:35.000000 pyptt-1.2.7/PyPtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 13:21:35.000000 pyptt-1.2.7/PyPtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-21 13:21:29.000000 pyptt-1.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 13:21:35.356844 pyptt-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-21 13:21:29.000000 pyptt-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.890526 pyptt-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-23 02:37:55.000000 pyptt-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 02:37:55.000000 pyptt-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-23 02:38:00.890526 pyptt-1.2.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.886526 pyptt-1.2.8/PyPtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    32101 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/PTT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_change_pw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_del_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_board_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_board_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_bottom_post_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_favourite_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_newest_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_post_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_give_money.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_has_new_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_loginout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_mark_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_reply_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_set_board_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/check_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/connect_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.886526 pyptt-1.2.8/PyPtt/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/lang/en_US.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/lang/zh_TW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/lib_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54872 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.890526 pyptt-1.2.8/PyPtt/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/ssl/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-23 02:37:55.000000 pyptt-1.2.8/PyPtt/ssl/key.pem
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:38:00.890526 pyptt-1.2.8/PyPtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 02:38:00.000000 pyptt-1.2.8/PyPtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-23 02:37:55.000000 pyptt-1.2.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 02:38:00.890526 pyptt-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-23 02:37:55.000000 pyptt-1.2.8/setup.py
```

### Comparing `pyptt-1.2.7/LICENSE` & `pyptt-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PKG-INFO` & `pyptt-1.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.7
+Version: 1.2.8
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `pyptt-1.2.7/PyPtt/PTT.py` & `pyptt-1.2.8/PyPtt/PTT.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_bucket.py` & `pyptt-1.2.8/PyPtt/_api_bucket.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_call_status.py` & `pyptt-1.2.8/PyPtt/_api_call_status.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_change_pw.py` & `pyptt-1.2.8/PyPtt/_api_change_pw.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_comment.py` & `pyptt-1.2.8/PyPtt/_api_comment.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_del_post.py` & `pyptt-1.2.8/PyPtt/_api_del_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_board_info.py` & `pyptt-1.2.8/PyPtt/_api_get_board_info.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_board_list.py` & `pyptt-1.2.8/PyPtt/_api_get_board_list.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_bottom_post_list.py` & `pyptt-1.2.8/PyPtt/_api_get_bottom_post_list.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_favourite_board.py` & `pyptt-1.2.8/PyPtt/_api_get_favourite_board.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_newest_index.py` & `pyptt-1.2.8/PyPtt/_api_get_newest_index.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_post.py` & `pyptt-1.2.8/PyPtt/_api_get_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_post_index.py` & `pyptt-1.2.8/PyPtt/_api_get_post_index.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_time.py` & `pyptt-1.2.8/PyPtt/_api_get_time.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_get_user.py` & `pyptt-1.2.8/PyPtt/_api_get_user.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_give_money.py` & `pyptt-1.2.8/PyPtt/_api_give_money.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_has_new_mail.py` & `pyptt-1.2.8/PyPtt/_api_has_new_mail.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_loginout.py` & `pyptt-1.2.8/PyPtt/_api_loginout.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_mail.py` & `pyptt-1.2.8/PyPtt/_api_mail.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_mark_post.py` & `pyptt-1.2.8/PyPtt/_api_mark_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_post.py` & `pyptt-1.2.8/PyPtt/_api_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_reply_post.py` & `pyptt-1.2.8/PyPtt/_api_reply_post.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_search_user.py` & `pyptt-1.2.8/PyPtt/_api_search_user.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_set_board_title.py` & `pyptt-1.2.8/PyPtt/_api_set_board_title.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/_api_util.py` & `pyptt-1.2.8/PyPtt/_api_util.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/check_value.py` & `pyptt-1.2.8/PyPtt/check_value.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/command.py` & `pyptt-1.2.8/PyPtt/command.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/config.py` & `pyptt-1.2.8/PyPtt/config.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/connect_core.py` & `pyptt-1.2.8/PyPtt/connect_core.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/data_type.py` & `pyptt-1.2.8/PyPtt/data_type.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/exceptions.py` & `pyptt-1.2.8/PyPtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/i18n.py` & `pyptt-1.2.8/PyPtt/i18n.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/lang/en_US.yaml` & `pyptt-1.2.8/PyPtt/lang/en_US.yaml`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/lang/zh_TW.yaml` & `pyptt-1.2.8/PyPtt/lang/zh_TW.yaml`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/lib_util.py` & `pyptt-1.2.8/PyPtt/lib_util.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/log.py` & `pyptt-1.2.8/PyPtt/log.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/screens.py` & `pyptt-1.2.8/PyPtt/screens.py`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt/service.py` & `pyptt-1.2.8/PyPtt/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import queue
 import threading
 import time
-import uuid
+from queue import Queue
+from threading import Condition
 from typing import Optional
 
 from . import PTT
 from . import check_value
 from . import log
 
 
@@ -70,99 +72,96 @@
         self.logger = log.init(log_level, 'service')
 
         self.logger.info('init')
 
         self._api = None
         self._api_init_config = pyptt_init_config
 
-        self._call_queue = []
+        self._call_queue = Queue()
         self._call_result = {}
+        self._call_result_cv = Condition()
 
-        self._id_pool = set()
-        self._id_pool_lock = threading.Lock()
+        self._id_pool = {}
 
         self._close = False
 
         self._thread = threading.Thread(target=self._run, daemon=True)
         self._thread.start()
 
         while self._api is None:
             time.sleep(0.01)
 
     def _run(self):
-
         if self._api is not None:
             self._api.logout()
             self._api = None
 
         self._api = PTT.API(**self._api_init_config)
 
         self.logger.info('start')
 
         while not self._close:
-            if len(self._call_queue) == 0:
-                time.sleep(0.05)
+            try:
+                call = self._call_queue.get(timeout=0.05)
+            except queue.Empty:
                 continue
 
-            call = self._call_queue.pop(0)
-
             func = getattr(self._api, call['api'])
 
             api_result = None
             api_exception = None
             try:
                 api_result = func(**call['args'])
             except Exception as e:
                 api_exception = e
 
-            self._call_result[call['id']] = {
-                'result': api_result,
-                'exception': api_exception
-            }
+            with self._call_result_cv:
+                self._call_result[call['id']] = {
+                    'result': api_result,
+                    'exception': api_exception
+                }
+                self._call_result_cv.notify()
 
     def _get_call_id(self):
-        while True:
-            call_id = uuid.uuid4().hex
 
-            with self._id_pool_lock:
-                if call_id not in self._id_pool:
-                    self._id_pool.add(call_id)
-                    return call_id
+        call_id = f'{threading.get_ident()}_{int(time.time() * 1000000)}'
+        self._id_pool[call_id] = True
 
-    def call(self, api: str, args: Optional[dict] = None):
+        return call_id
 
+    def call(self, api: str, args: Optional[dict] = None):
         if args is None:
             args = {}
 
         check_value.check_type(api, str, 'api')
         check_value.check_type(args, dict, 'args')
 
         if api not in dir(self._api):
             raise ValueError(f'api {api} not found')
 
         call = {
             'api': api,
             'id': self._get_call_id(),
             'args': args
         }
-        self._call_queue.append(call)
+        self._call_queue.put(call)
 
-        while call['id'] not in self._call_result:
-            time.sleep(0.01)
+        with self._call_result_cv:
+            while call['id'] not in self._call_result:
+                self._call_result_cv.wait()
 
-        call_result = self._call_result[call['id']]
-        del self._call_result[call['id']]
+            call_result = self._call_result[call['id']]
+            del self._call_result[call['id']]
 
-        with self._id_pool_lock:
-            self._id_pool.remove(call['id'])
+        del self._id_pool[call['id']]
 
         if call_result['exception'] is not None:
             raise call_result['exception']
 
         return call_result['result']
 
     def close(self):
         self.logger.info('close')
         self._close = True
         self._thread.join()
 
-        self.logger.info('done')
+        self.logger.info('done')
```

### Comparing `pyptt-1.2.7/PyPtt/ssl/cert.pem` & `pyptt-1.2.8/PyPtt/ssl/cert.pem`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/PyPtt.egg-info/PKG-INFO` & `pyptt-1.2.8/PyPtt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.7
+Version: 1.2.8
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `pyptt-1.2.7/PyPtt.egg-info/SOURCES.txt` & `pyptt-1.2.8/PyPtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/README.md` & `pyptt-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pyptt-1.2.7/setup.py` & `pyptt-1.2.8/setup.py`

 * *Files identical despite different names*

