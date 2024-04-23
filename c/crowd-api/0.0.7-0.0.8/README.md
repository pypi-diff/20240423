# Comparing `tmp/crowd-api-0.0.7.tar.gz` & `tmp/crowd-api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crowd-api-0.0.7.tar", last modified: Thu Nov 28 14:17:21 2019, max compression
+gzip compressed data, was "dist/crowd-api-0.0.8.tar", last modified: Tue Jun  8 19:10:59 2021, max compression
```

## Comparing `crowd-api-0.0.7.tar` & `crowd-api-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxr-xr-x   0 m4ce       (501) staff       (20)        0 2019-11-28 14:17:21.000000 crowd-api-0.0.7/
-drwxr-xr-x   0 m4ce       (501) staff       (20)        0 2019-11-28 14:17:21.000000 crowd-api-0.0.7/crowd_api/
--rw-r--r--   0 m4ce       (501) staff       (20)    10838 2019-11-28 14:14:09.000000 crowd-api-0.0.7/crowd_api/__init__.py
--rw-r--r--   0 m4ce       (501) staff       (20)      356 2019-11-28 14:17:21.000000 crowd-api-0.0.7/PKG-INFO
--rw-r--r--   0 m4ce       (501) staff       (20)      480 2019-11-28 14:14:18.000000 crowd-api-0.0.7/setup.py
--rw-r--r--   0 m4ce       (501) staff       (20)       40 2019-11-28 14:14:09.000000 crowd-api-0.0.7/setup.cfg
+drwxr-xr-x   0 m4ce       (501) staff       (20)        0 2021-06-08 19:10:59.000000 crowd-api-0.0.8/
+drwxr-xr-x   0 m4ce       (501) staff       (20)        0 2021-06-08 19:10:59.000000 crowd-api-0.0.8/crowd_api/
+-rw-r--r--   0 m4ce       (501) staff       (20)    13559 2021-06-08 19:09:32.000000 crowd-api-0.0.8/crowd_api/__init__.py
+-rw-r--r--   0 m4ce       (501) staff       (20)      356 2021-06-08 19:10:59.000000 crowd-api-0.0.8/PKG-INFO
+-rw-r--r--   0 m4ce       (501) staff       (20)      480 2021-06-08 19:09:40.000000 crowd-api-0.0.8/setup.py
+-rw-r--r--   0 m4ce       (501) staff       (20)       40 2021-01-25 09:18:37.000000 crowd-api-0.0.8/setup.cfg
```

### Comparing `crowd-api-0.0.7/crowd_api/__init__.py` & `crowd-api-0.0.8/crowd_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,28 +41,48 @@
                                                           "Accept": "application/json"}, auth=self.auth, verify=self.verify_ssl, timeout=self.timeout)
         return req
 
     def api_post(self, query, data):
         req = requests.post(self.api_url + query, headers={"Content-Type": "application/json", "Accept": "application/json"},
                             auth=self.auth, data=json.dumps(data), verify=self.verify_ssl, timeout=self.timeout)
         return req
+    
+    def api_put(self, query, data):
+        req = requests.put(self.api_url + query, headers={"Content-Type": "application/json", "Accept": "application/json"},
+                            auth=self.auth, data=json.dumps(data), verify=self.verify_ssl, timeout=self.timeout)
+        return req
+
+    def api_delete(self, query, data):
+        req = requests.delete(self.api_url + query, headers={"Content-Type": "application/json", "Accept": "application/json"},
+                              auth=self.auth, data=json.dumps(data), verify=self.verify_ssl, timeout=self.timeout)
+        return req
 
     def get_user(self, **kwargs):
         if "username" not in kwargs:
             raise ValueError("Must pass username")
 
         req = self.api_get(
             "/user?username={}&expand=attributes".format(kwargs['username']))
         if req.status_code == 200:
             return {"status": True, "user": req.json()}
         if req.status_code == 404:
             return {"status": False, "user": None}
         else:
             return {"status": False, "code": req.status_code, "reason": req.content}
 
+    def get_user_attributes(self, **kwargs):
+        if "username" not in kwargs:
+            raise ValueError("Must pass username")
+
+        req = self.api_get("/user/attribute?username={}".format(kwargs['username']))
+        if req.status_code == 200:
+            return {"status": True, "Attributes": req.content}
+        else:
+            return {"status": False, "code": req.status_code, "reason": req.content}
+
     def get_user_groups(self, **kwargs):
         groups = []
 
         if "username" not in kwargs:
             raise ValueError("Must pass username")
 
         req = self.api_get("/user/group/direct?username={}&max-results={}".format(
@@ -234,14 +254,36 @@
         req = self.api_post("/user/attribute?username={}".format(kwargs['username']), {
                             "attributes": [{"name": kwargs['attribute_name'], "values": kwargs['attribute_value']}]})
         if req.status_code == 204:
             return {"status": True}
         else:
             return {"status": False, "code": req.status_code, "reason": req.content}
 
+    def set_user_activity(self, **kwargs):
+        if "username" not in kwargs:
+            raise ValueError("Must pass username")
+
+        if "active" not in kwargs:
+            raise ValueError("Must pass active (true/false)")
+
+        # fetch current user document
+        user_document = self.api_get(
+            "/user?username={}".format(kwargs['username'])).json()
+
+        # set to active true/false
+        user_document["active"] = kwargs['active']
+
+        # update user object
+        req = self.api_put("/user?username={}".format(kwargs['username']), user_document )
+        if req.status_code == 204:
+            return {"status": True}
+        else:
+            return {"status": False, "code": req.status_code, "reason": req.content}
+
+
     def create_user(self, **kwargs):
         user = {}
 
         for k, v in kwargs.iteritems():
             user[k.replace('_', '-')] = v
 
         if 'password' not in kwargs:
@@ -270,14 +312,26 @@
         req = self.api_post(
             "/group", {"name": kwargs['name'], "type": "GROUP", "description": kwargs['description'], "active": True})
         if req.status_code == 201:
             return {"status": True}
         else:
             return {"status": False, "code": req.status_code, "reason": req.content}
 
+    def delete_group(self, **kwargs):
+
+        if "groupname" not in kwargs:
+            raise ValueError("Must pass groupname")
+
+        req = self.api_delete(
+            "/group?groupname={}".format(kwargs['groupname']), data={})
+        if req.status_code == 204:
+            return {"status": True}
+        else:
+            return {"status": False, "code": req.status_code, "reason": req.content}
+
     def add_user_to_group(self, **kwargs):
 
         if "username" not in kwargs:
             raise ValueError("Must pass username")
 
         if "groupname" not in kwargs:
             raise ValueError("Must pass groupname")
@@ -285,14 +339,29 @@
         req = self.api_post(
             "/user/group/direct?username={}".format(kwargs['username']), {"name": kwargs['groupname']})
         if req.status_code == 201:
             return {"status": True}
         else:
             return {"status": False, "code": req.status_code, "reason": req.content}
 
+    def remove_user_from_group(self, **kwargs):
+
+        if "username" not in kwargs:
+            raise ValueError("Must pass username")
+
+        if "groupname" not in kwargs:
+            raise ValueError("Must pass groupname")
+
+        req = self.api_delete(
+            "/user/group/direct?username={}&groupname={}".format(kwargs['username'], kwargs['groupname']), data={})
+        if req.status_code == 204:
+            return {"status": True}
+        else:
+            return {"status": False, "code": req.status_code, "reason": req.content}
+
     def get_group(self, **kwargs):
         req = self.api_get(
             "/group?groupname={}&expand=attributes".format(kwargs['name']))
         if req.status_code == 200:
             return {"status": True, "group": req.json()}
         else:
             return {"status": False, "code": req.status_code, "reason": req.content}
```

