# Comparing `tmp/a3consul-0.1.0.tar.gz` & `tmp/a3consul-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a3consul-0.1.0.tar", last modified: Thu Apr 18 11:05:54 2024, max compression
+gzip compressed data, was "a3consul-0.1.1.tar", last modified: Tue Apr 23 03:33:39 2024, max compression
```

## Comparing `a3consul-0.1.0.tar` & `a3consul-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 11:05:54.845462 a3consul-0.1.0/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3consul-0.1.0/LICENSE
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       66 2024-04-18 08:54:48.000000 a3consul-0.1.0/MANIFEST.in
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-04-18 11:05:54.845462 a3consul-0.1.0/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      131 2024-04-18 08:56:18.000000 a3consul-0.1.0/README.md
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 11:05:54.845462 a3consul-0.1.0/a3consul/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-04-18 08:56:57.000000 a3consul-0.1.0/a3consul/__init__.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 11:05:54.845462 a3consul-0.1.0/a3consul/scene_cases/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       24 2024-03-21 02:01:29.000000 a3consul-0.1.0/a3consul/scene_cases/__init__.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 11:05:54.845462 a3consul-0.1.0/a3consul/scene_cases/watch_nodes/
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      169 2024-03-29 06:18:34.000000 a3consul-0.1.0/a3consul/scene_cases/watch_nodes/__init__.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1190 2024-04-18 10:41:58.000000 a3consul-0.1.0/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      720 2024-04-18 10:26:46.000000 a3consul-0.1.0/a3consul/scene_cases/watch_nodes/cmds.py
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     2292 2024-04-18 10:17:14.000000 a3consul-0.1.0/a3consul/scene_cases/watch_nodes/node_thread.py
-drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-18 11:05:54.845462 a3consul-0.1.0/a3consul.egg-info/
--rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-04-18 11:05:54.000000 a3consul-0.1.0/a3consul.egg-info/PKG-INFO
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      491 2024-04-18 11:05:54.000000 a3consul-0.1.0/a3consul.egg-info/SOURCES.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-18 11:05:54.000000 a3consul-0.1.0/a3consul.egg-info/dependency_links.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-18 11:05:54.000000 a3consul-0.1.0/a3consul.egg-info/not-zip-safe
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       29 2024-04-18 11:05:54.000000 a3consul-0.1.0/a3consul.egg-info/requires.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        9 2024-04-18 11:05:54.000000 a3consul-0.1.0/a3consul.egg-info/top_level.txt
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1144 2024-04-18 11:05:54.845462 a3consul-0.1.0/setup.cfg
--rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3consul-0.1.0/setup.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)    11357 2024-02-08 11:23:49.000000 a3consul-0.1.1/LICENSE
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       66 2024-04-18 08:54:48.000000 a3consul-0.1.1/MANIFEST.in
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-04-23 03:33:39.502809 a3consul-0.1.1/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      131 2024-04-18 08:56:18.000000 a3consul-0.1.1/README.md
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       47 2024-04-23 02:44:40.000000 a3consul-0.1.1/a3consul/__init__.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul/scene_cases/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       24 2024-03-21 02:01:29.000000 a3consul-0.1.1/a3consul/scene_cases/__init__.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      169 2024-03-29 06:18:34.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/__init__.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1190 2024-04-18 10:41:58.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      720 2024-04-18 10:26:46.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/cmds.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     2524 2024-04-23 03:28:26.000000 a3consul-0.1.1/a3consul/scene_cases/watch_nodes/node_thread.py
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      463 2024-04-23 03:28:26.000000 a3consul-0.1.1/a3consul/utils.py
+drwxrwxr-x   0 guqiang   (1000) guqiang   (1000)        0 2024-04-23 03:33:39.502809 a3consul-0.1.1/a3consul.egg-info/
+-rw-r--r--   0 guqiang   (1000) guqiang   (1000)     1253 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/PKG-INFO
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)      509 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/SOURCES.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/dependency_links.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        1 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/not-zip-safe
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       29 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/requires.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)        9 2024-04-23 03:33:39.000000 a3consul-0.1.1/a3consul.egg-info/top_level.txt
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)     1144 2024-04-23 03:33:39.502809 a3consul-0.1.1/setup.cfg
+-rw-rw-r--   0 guqiang   (1000) guqiang   (1000)       39 2024-02-08 11:23:49.000000 a3consul-0.1.1/setup.py
```

### Comparing `a3consul-0.1.0/LICENSE` & `a3consul-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `a3consul-0.1.0/PKG-INFO` & `a3consul-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3consul
-Version: 0.1.0
+Version: 0.1.1
 Summary: It is just a thin wrapper of py-consul.
 Home-page: https://github.com/three-kinds/a3consul
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3consul
 Project-URL: Source, https://github.com/three-kinds/a3consul
```

### Comparing `a3consul-0.1.0/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py` & `a3consul-0.1.1/a3consul/scene_cases/watch_nodes/abstract_node_change_service.py`

 * *Files identical despite different names*

### Comparing `a3consul-0.1.0/a3consul/scene_cases/watch_nodes/cmds.py` & `a3consul-0.1.1/a3consul/scene_cases/watch_nodes/cmds.py`

 * *Files identical despite different names*

### Comparing `a3consul-0.1.0/a3consul/scene_cases/watch_nodes/node_thread.py` & `a3consul-0.1.1/a3consul/scene_cases/watch_nodes/node_thread.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import time
 import uuid
 from typing import Optional
 from a3py.simplified.concurrence import force_exit_from_threads
 from threading import Thread
 from consul import Consul
 
+from a3consul.utils import patch_http_client_with_timeout
+
 
 class NodeThread(Thread):
     logger = logging.getLogger(__name__)
 
     def __init__(self, topic: str, conf: dict, nodes_path: str, should_force_exit: bool, *args, **kwargs):
         self._topic = topic
         self._conf = conf
@@ -36,26 +38,28 @@
         start_tick = time.time()
         while True:
             try:
                 self._client.session.renew(session_id=self._session_id)
                 self.logger.debug(f'[{self._topic}]renew成功')
                 return True
             except Exception as e:
-                self.logger.debug(f'[{self._topic}]renew出现异常: {e}')
+                self.logger.warning(f'[{self._topic}]renew出现异常: {e}')
 
             # 出现异常后，每秒重试一次
             time.sleep(1)
             if time.time() - start_tick > timeout_seconds:
                 return False
 
     def force_exit(self):
         force_exit_from_threads(f'[{self._topic}]因与服务端断开连接，所以整个进程退出')
 
     def run(self):
         conf = self._conf['renew']
+        per_request_timeout_seconds = conf.get('per_request_timeout_seconds', None) or 2
+        patch_http_client_with_timeout(self._client, per_request_timeout_seconds)
         while True:
             is_success = self._renew_session(timeout_seconds=conf['timeout_seconds'])
             if is_success:
                 sleep_seconds = conf['sleep_seconds']
                 time.sleep(sleep_seconds)
             else:
                 break
```

### Comparing `a3consul-0.1.0/a3consul.egg-info/PKG-INFO` & `a3consul-0.1.1/a3consul.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a3consul
-Version: 0.1.0
+Version: 0.1.1
 Summary: It is just a thin wrapper of py-consul.
 Home-page: https://github.com/three-kinds/a3consul
 Author: three-kinds
 Author-email: 3179158552@qq.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/three-kinds/a3consul
 Project-URL: Source, https://github.com/three-kinds/a3consul
```

### Comparing `a3consul-0.1.0/setup.cfg` & `a3consul-0.1.1/setup.cfg`

 * *Files identical despite different names*

