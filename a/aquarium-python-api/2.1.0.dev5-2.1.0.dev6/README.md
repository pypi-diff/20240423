# Comparing `tmp/aquarium-python-api-2.1.0.dev5.tar.gz` & `tmp/aquarium-python-api-2.1.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aquarium-python-api-2.1.0.dev5.tar", last modified: Mon Mar 11 21:54:56 2024, max compression
+gzip compressed data, was "dist/aquarium-python-api-2.1.0.dev6.tar", last modified: Mon Mar 18 08:45:14 2024, max compression
```

## Comparing `aquarium-python-api-2.1.0.dev5.tar` & `aquarium-python-api-2.1.0.dev6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-11 21:54:56.240327 aquarium-python-api-2.1.0.dev5/
--rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.1.0.dev5/LICENSE.md
--rw-r--r--   0 yann       (501) staff       (20)     3243 2024-03-11 21:54:56.240699 aquarium-python-api-2.1.0.dev5/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.1.0.dev5/README.md
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-11 21:54:56.177102 aquarium-python-api-2.1.0.dev5/aquarium/
--rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.1.0.dev5/aquarium/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)    14256 2024-03-11 18:14:00.000000 aquarium-python-api-2.1.0.dev5/aquarium/aquarium.py
--rw-r--r--   0 yann       (501) staff       (20)      364 2023-06-05 08:31:35.000000 aquarium-python-api-2.1.0.dev5/aquarium/auth.py
--rw-r--r--   0 yann       (501) staff       (20)     3750 2024-03-11 18:52:24.000000 aquarium-python-api-2.1.0.dev5/aquarium/edge.py
--rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.1.0.dev5/aquarium/element.py
--rw-r--r--   0 yann       (501) staff       (20)     3299 2024-03-11 18:52:24.000000 aquarium-python-api-2.1.0.dev5/aquarium/entity.py
--rw-r--r--   0 yann       (501) staff       (20)    12140 2024-03-11 21:54:05.000000 aquarium-python-api-2.1.0.dev5/aquarium/events.py
--rw-r--r--   0 yann       (501) staff       (20)     1206 2023-08-28 15:25:27.000000 aquarium-python-api-2.1.0.dev5/aquarium/exceptions.py
--rw-r--r--   0 yann       (501) staff       (20)    28205 2024-03-11 18:52:24.000000 aquarium-python-api-2.1.0.dev5/aquarium/item.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-11 21:54:56.233837 aquarium-python-api-2.1.0.dev5/aquarium/items/
--rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/__init__.py
--rw-r--r--   0 yann       (501) staff       (20)     6707 2024-03-05 10:14:43.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/asset.py
--rw-r--r--   0 yann       (501) staff       (20)     2348 2024-03-05 10:14:47.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/bot.py
--rw-r--r--   0 yann       (501) staff       (20)     5364 2023-09-19 10:22:45.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/organisation.py
--rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/playlist.py
--rw-r--r--   0 yann       (501) staff       (20)     3318 2024-03-11 18:14:00.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/project.py
--rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/shot.py
--rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/task.py
--rw-r--r--   0 yann       (501) staff       (20)     1055 2023-04-15 08:53:33.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/template.py
--rw-r--r--   0 yann       (501) staff       (20)     7151 2023-09-19 10:22:45.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/user.py
--rw-r--r--   0 yann       (501) staff       (20)     1559 2023-06-05 10:10:25.000000 aquarium-python-api-2.1.0.dev5/aquarium/items/usergroup.py
--rw-r--r--   0 yann       (501) staff       (20)     2332 2024-03-11 18:14:00.000000 aquarium-python-api-2.1.0.dev5/aquarium/tools.py
--rw-r--r--   0 yann       (501) staff       (20)     4981 2024-03-05 10:14:47.000000 aquarium-python-api-2.1.0.dev5/aquarium/utils.py
-drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-11 21:54:56.239562 aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/
--rw-r--r--   0 yann       (501) staff       (20)     3243 2024-03-11 21:54:55.000000 aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/PKG-INFO
--rw-r--r--   0 yann       (501) staff       (20)      744 2024-03-11 21:54:55.000000 aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 yann       (501) staff       (20)        1 2024-03-11 21:54:55.000000 aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 yann       (501) staff       (20)      123 2024-03-11 21:54:55.000000 aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/requires.txt
--rw-r--r--   0 yann       (501) staff       (20)        9 2024-03-11 21:54:55.000000 aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/top_level.txt
--rw-r--r--   0 yann       (501) staff       (20)     1286 2024-03-11 21:54:56.242589 aquarium-python-api-2.1.0.dev5/setup.cfg
--rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.1.0.dev5/setup.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-18 08:45:14.429362 aquarium-python-api-2.1.0.dev6/
+-rw-r--r--   0 yann       (501) staff       (20)    34915 2021-02-18 17:12:41.000000 aquarium-python-api-2.1.0.dev6/LICENSE.md
+-rw-r--r--   0 yann       (501) staff       (20)     3243 2024-03-18 08:45:14.429740 aquarium-python-api-2.1.0.dev6/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)     1813 2022-11-05 09:19:19.000000 aquarium-python-api-2.1.0.dev6/README.md
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-18 08:45:14.409089 aquarium-python-api-2.1.0.dev6/aquarium/
+-rw-r--r--   0 yann       (501) staff       (20)      917 2023-06-05 09:29:23.000000 aquarium-python-api-2.1.0.dev6/aquarium/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)    14531 2024-03-18 08:44:57.000000 aquarium-python-api-2.1.0.dev6/aquarium/aquarium.py
+-rw-r--r--   0 yann       (501) staff       (20)      364 2024-03-14 15:08:32.000000 aquarium-python-api-2.1.0.dev6/aquarium/auth.py
+-rw-r--r--   0 yann       (501) staff       (20)     3750 2024-03-18 08:44:53.000000 aquarium-python-api-2.1.0.dev6/aquarium/edge.py
+-rw-r--r--   0 yann       (501) staff       (20)     1542 2022-11-09 16:11:01.000000 aquarium-python-api-2.1.0.dev6/aquarium/element.py
+-rw-r--r--   0 yann       (501) staff       (20)     3347 2024-03-18 08:44:57.000000 aquarium-python-api-2.1.0.dev6/aquarium/entity.py
+-rw-r--r--   0 yann       (501) staff       (20)    12200 2024-03-18 08:44:57.000000 aquarium-python-api-2.1.0.dev6/aquarium/events.py
+-rw-r--r--   0 yann       (501) staff       (20)     1206 2024-03-14 15:08:32.000000 aquarium-python-api-2.1.0.dev6/aquarium/exceptions.py
+-rw-r--r--   0 yann       (501) staff       (20)    28205 2024-03-18 08:44:53.000000 aquarium-python-api-2.1.0.dev6/aquarium/item.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-18 08:45:14.422879 aquarium-python-api-2.1.0.dev6/aquarium/items/
+-rw-r--r--   0 yann       (501) staff       (20)       24 2021-02-01 10:01:25.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/__init__.py
+-rw-r--r--   0 yann       (501) staff       (20)     6707 2024-03-14 15:08:32.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/asset.py
+-rw-r--r--   0 yann       (501) staff       (20)     2348 2024-03-18 08:44:53.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/bot.py
+-rw-r--r--   0 yann       (501) staff       (20)     5364 2024-03-14 15:08:32.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/organisation.py
+-rw-r--r--   0 yann       (501) staff       (20)     5070 2022-11-10 09:26:31.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/playlist.py
+-rw-r--r--   0 yann       (501) staff       (20)     3318 2024-03-18 08:44:53.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/project.py
+-rw-r--r--   0 yann       (501) staff       (20)      271 2021-02-18 12:06:41.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/shot.py
+-rw-r--r--   0 yann       (501) staff       (20)     6578 2023-01-12 08:03:01.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/task.py
+-rw-r--r--   0 yann       (501) staff       (20)     1055 2024-03-14 15:08:32.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/template.py
+-rw-r--r--   0 yann       (501) staff       (20)     7151 2024-03-14 15:08:32.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/user.py
+-rw-r--r--   0 yann       (501) staff       (20)     1559 2024-03-14 15:08:32.000000 aquarium-python-api-2.1.0.dev6/aquarium/items/usergroup.py
+-rw-r--r--   0 yann       (501) staff       (20)     2331 2024-03-18 08:44:57.000000 aquarium-python-api-2.1.0.dev6/aquarium/tools.py
+-rw-r--r--   0 yann       (501) staff       (20)     4981 2024-03-14 15:08:37.000000 aquarium-python-api-2.1.0.dev6/aquarium/utils.py
+drwxr-xr-x   0 yann       (501) staff       (20)        0 2024-03-18 08:45:14.428630 aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/
+-rw-r--r--   0 yann       (501) staff       (20)     3243 2024-03-18 08:45:13.000000 aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 yann       (501) staff       (20)      744 2024-03-18 08:45:13.000000 aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 yann       (501) staff       (20)        1 2024-03-18 08:45:13.000000 aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 yann       (501) staff       (20)      123 2024-03-18 08:45:13.000000 aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/requires.txt
+-rw-r--r--   0 yann       (501) staff       (20)        9 2024-03-18 08:45:13.000000 aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/top_level.txt
+-rw-r--r--   0 yann       (501) staff       (20)     1286 2024-03-18 08:45:14.431509 aquarium-python-api-2.1.0.dev6/setup.cfg
+-rw-r--r--   0 yann       (501) staff       (20)       37 2021-01-12 10:42:28.000000 aquarium-python-api-2.1.0.dev6/setup.py
```

### Comparing `aquarium-python-api-2.1.0.dev5/LICENSE.md` & `aquarium-python-api-2.1.0.dev6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/PKG-INFO` & `aquarium-python-api-2.1.0.dev6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.1.0.dev5
+Version: 2.1.0.dev6
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.1.0.dev5/README.md` & `aquarium-python-api-2.1.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/__init__.py` & `aquarium-python-api-2.1.0.dev6/aquarium/__init__.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/aquarium.py` & `aquarium-python-api-2.1.0.dev6/aquarium/aquarium.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     :type api_url: string
     :param token: Specify the authentication token, to avoid :func:`~aquarium.aquarium.Aquarium.signin`
     :type token: string, optional
     :param api_version: Specify the API version you want to use (default : `v1`).
     :type api_version: string, optional
     :param domain: Specify the domain used for unauthenticated requests. Mainly for Aquarium Fatfish Lab dev or local Aquarium server without DNS
     :type domain: string, optional
+    :param strict_dotmap: Specify if the dotmap should create new property dynamically (default : `False`). Set to `True` to have default Python behaviour like on Dict()
+    :type strict_dotmap: boolean, optional
 
     :var token: Get the current token (populated after a first :func:`~aquarium.aquarium.Aquarium.signin`)
     :var edge: Access to Edge class
     :vartype edge: :class:`~aquarium.edge.Edge`
     :var item: Access to Item class
     :vartype item: :class:`~aquarium.item.Item`
     :var asset: Access to Asset subclass
@@ -73,25 +75,26 @@
     :vartype usergroup: :class:`~aquarium.items.usergroup.Usergroup`
     :var organisation: Access to Organisation subclass
     :vartype organisation: :class:`~aquarium.items.organisation.Organisation`
     :var utils: Access to Utils class
     :vartype utils: :class:`~aquarium.utils.Utils`
     """
 
-    def __init__(self, api_url='', token=None, api_version='v1', domain=None):
+    def __init__(self, api_url='', token=None, api_version='v1', domain=None, strict_dotmap=False):
         """
         Constructs a new instance.
         """
         # Session
         self.session=requests.Session()
 
         self.api_url=api_url
         self.api_version=api_version
         self.token=token
         self.domain=domain
+        self.strict_dotmap=strict_dotmap
 
         # Classes
         self.events=Events(parent=self)
         self.element=Element(parent=self)
         self.item=Item(parent=self)
         self.edge=Edge(parent=self)
         self.utils=Utils()
```

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/edge.py` & `aquarium-python-api-2.1.0.dev6/aquarium/edge.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/element.py` & `aquarium-python-api-2.1.0.dev6/aquarium/element.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/entity.py` & `aquarium-python-api-2.1.0.dev6/aquarium/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self.createdAt=data.get('createdAt')
         self.updatedAt=data.get('updatedAt')
         self.createdBy=data.get('createdBy')
         self.updatedBy=data.get('updatedBy')
 
         entity_data=data.get('data')
         if entity_data:
-            self.data=DotMap(entity_data)
+            self.data=DotMap(entity_data, _dynamic=(not bool(self.parent.strict_dotmap)))
 
     def do_request(self, *args, **kwargs):
         """
         Execute a request
 
         :param      args:    The arguments used to launch the process
         :type       args:    tuple
```

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/events.py` & `aquarium-python-api-2.1.0.dev6/aquarium/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         self.createdBy=data.get('createdBy')
         self.updatedAt=data.get('updatedAt')
         self.updatedBy=data.get('updatedBy')
         self.emittedFrom=data.get('emittedFrom')
 
         entity_data=data.get('data')
         if entity_data:
-            self.data=DotMap(entity_data)
+            self.data=DotMap(entity_data, _dynamic=(not bool(self.parent.strict_dotmap)))
 
         topicRegex = r"^(?:custom[.])?(?P<category>\w+)([.](?P<verb>\w+))?([.](\w+))*$"
         topicMatched = re.match(topicRegex, self.topic)
         if topicMatched.group('category'):
             self._category = topicMatched.group('category')
 
         if topicMatched.group('verb'):
@@ -347,32 +347,32 @@
             raise ValueError('The event has no key, so it is not possible to get it')
 
     def get_context(self):
         """
         Get the context of the event up to the project
 
         :returns:   The context of the event with the item Project and it's traversal path
-        :rtype:     dictionary with the item :class:`~aquarium.item.Item` and path as list of :class:`~aquarium.item.Item`
+        :rtype:     dictionary with the project :class:`~aquarium.item.Item` and path as list of :class:`~aquarium.item.Item`
         """
         endpoint = 'events/{key}/traverse'.format(key=self._key)
         payload = {
             "query": "# <($Emit)- 0,1 * <($Child, 10)- 0,1 item.type IN ['Project'] AND path.vertices[*].type NONE == 'User' SORT null VIEW $view",
             "aliases": {
                 "view": {
-                    "item": "item",
+                    "project": "item",
                     "path": "path.vertices"
                 }
             }
         }
         if (self.emittedFrom):
             payload['query'] = "# <($Child, 10)- 0,1 item.type IN ['Project'] AND path.vertices[*].type NONE == 'User' SORT null VIEW $view"
             endpoint = '{emittedFrom}/traverse'.format(emittedFrom=self.emittedFrom)
 
         context = self.do_request('POST', endpoint, json=payload)
         print(payload['query'])
         if (context and len(context) > 0):
             return {
-                'item': self.parent.cast(context[0]['item']),
+                'project': self.parent.cast(context[0]['project']),
                 'path': [self.parent.cast(item) for item in context[0]['path']]
             }
         else:
             raise ValueError('The event has emittedFrom attribute, but the context could not be found')
```

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/exceptions.py` & `aquarium-python-api-2.1.0.dev6/aquarium/exceptions.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/item.py` & `aquarium-python-api-2.1.0.dev6/aquarium/item.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/asset.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/asset.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/bot.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/bot.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/organisation.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/organisation.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/playlist.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/playlist.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/project.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/project.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/task.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/task.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/template.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/template.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/user.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/user.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/items/usergroup.py` & `aquarium-python-api-2.1.0.dev6/aquarium/items/usergroup.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/tools.py` & `aquarium-python-api-2.1.0.dev6/aquarium/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     :rtype:     boolean
 
     :raises     RuntimeError:  "error" value from response
     """
     status_code=response.status_code
     url=response.url
     logger.debug('Evaluate request response : status_code : %s / url : %s', status_code, url)
-    if status_code == 200:
+    if status_code < 300:
         return True
     elif status_code==400:
         raise RequestError(response)
     elif status_code==401:
         raise AuthentificationError(response)
     elif status_code==403:
         raise AutorisationError(response)
```

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium/utils.py` & `aquarium-python-api-2.1.0.dev6/aquarium/utils.py`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/PKG-INFO` & `aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aquarium-python-api
-Version: 2.1.0.dev5
+Version: 2.1.0.dev6
 Summary: Aquarium python package
 Home-page: https://docs.fatfish.app/dev/python/index.html
 Author: Fatfish Lab
 Author-email: lab@fatfi.sh
 License: gpl-3.0
 Project-URL: Documentation, https://docs.fatfish.app/dev/python/index.html
 Project-URL: Source, https://github.com/fatfish-lab/aquarium-python-api
```

### Comparing `aquarium-python-api-2.1.0.dev5/aquarium_python_api.egg-info/SOURCES.txt` & `aquarium-python-api-2.1.0.dev6/aquarium_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aquarium-python-api-2.1.0.dev5/setup.cfg` & `aquarium-python-api-2.1.0.dev6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://docs.fatfish.app/dev/python/index.html
 project_urls = 
 	Documentation = https://docs.fatfish.app/dev/python/index.html
 	Source = https://github.com/fatfish-lab/aquarium-python-api
 	Aquarium = https://fatfi.sh/aquarium
-version = 2.1.0-dev.5
+version = 2.1.0-dev.6
 author = Fatfish Lab
 author_email = lab@fatfi.sh
 keywords = fatfish, lab, aquarium, studio, project, management, nodal, sdk, rest, cgi, vfx, api, python
 license = gpl-3.0
 license_file = LICENSE.md
 platform = any
 python_requires = '>=2.4'
```

