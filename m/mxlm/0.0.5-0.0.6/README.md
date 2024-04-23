# Comparing `tmp/mxlm-0.0.5.tar.gz` & `tmp/mxlm-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxlm-0.0.5.tar", last modified: Wed Apr 10 04:03:43 2024, max compression
+gzip compressed data, was "mxlm-0.0.6.tar", last modified: Tue Apr 23 14:00:02 2024, max compression
```

## Comparing `mxlm-0.0.5.tar` & `mxlm-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-10 04:03:43.966522 mxlm-0.0.5/
--rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.5/MANIFEST.in
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-10 04:03:43.966522 mxlm-0.0.5/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)     1078 2024-04-10 04:01:47.000000 mxlm-0.0.5/README.md
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-10 04:03:43.962522 mxlm-0.0.5/mxlm/
--rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-10 04:02:31.000000 mxlm-0.0.5/mxlm/__info__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)      171 2024-04-09 06:51:51.000000 mxlm-0.0.5/mxlm/__init__.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     4999 2024-04-10 03:15:58.000000 mxlm-0.0.5/mxlm/chat_api.py
--rw-rw-r--   0 yl        (1000) yl        (1000)     2397 2024-04-10 03:59:44.000000 mxlm-0.0.5/mxlm/chatmd_utils.py
-drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-10 04:03:43.966522 mxlm-0.0.5/mxlm.egg-info/
--rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-10 04:03:43.000000 mxlm-0.0.5/mxlm.egg-info/PKG-INFO
--rw-rw-r--   0 yl        (1000) yl        (1000)      258 2024-04-10 04:03:43.000000 mxlm-0.0.5/mxlm.egg-info/SOURCES.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-10 04:03:43.000000 mxlm-0.0.5/mxlm.egg-info/dependency_links.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-10 04:03:43.000000 mxlm-0.0.5/mxlm.egg-info/requires.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-10 04:03:43.000000 mxlm-0.0.5/mxlm.egg-info/top_level.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.5/requirements.txt
--rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-10 04:03:43.966522 mxlm-0.0.5/setup.cfg
--rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.5/setup.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-23 14:00:02.320421 mxlm-0.0.6/
+-rw-rw-r--   0 yl        (1000) yl        (1000)       35 2024-03-21 10:12:22.000000 mxlm-0.0.6/MANIFEST.in
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-23 14:00:02.320421 mxlm-0.0.6/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)     1078 2024-04-10 04:01:47.000000 mxlm-0.0.6/README.md
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-23 14:00:02.320421 mxlm-0.0.6/mxlm/
+-rw-rw-r--   0 yl        (1000) yl        (1000)      585 2024-04-23 13:59:46.000000 mxlm-0.0.6/mxlm/__info__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)      171 2024-04-09 06:51:51.000000 mxlm-0.0.6/mxlm/__init__.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     5941 2024-04-23 13:57:15.000000 mxlm-0.0.6/mxlm/chat_api.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2397 2024-04-10 03:59:44.000000 mxlm-0.0.6/mxlm/chatmd_utils.py
+-rw-rw-r--   0 yl        (1000) yl        (1000)     2265 2024-04-23 13:57:54.000000 mxlm-0.0.6/mxlm/dialog_format_conversion.py
+drwxrwxr-x   0 yl        (1000) yl        (1000)        0 2024-04-23 14:00:02.320421 mxlm-0.0.6/mxlm.egg-info/
+-rw-r--r--   0 yl        (1000) yl        (1000)      481 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/PKG-INFO
+-rw-rw-r--   0 yl        (1000) yl        (1000)      291 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/SOURCES.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        1 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/dependency_links.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        7 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/requires.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        5 2024-04-23 14:00:02.000000 mxlm-0.0.6/mxlm.egg-info/top_level.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)        8 2024-03-24 13:30:54.000000 mxlm-0.0.6/requirements.txt
+-rw-rw-r--   0 yl        (1000) yl        (1000)       38 2024-04-23 14:00:02.320421 mxlm-0.0.6/setup.cfg
+-rw-rw-r--   0 yl        (1000) yl        (1000)      962 2024-03-24 13:17:50.000000 mxlm-0.0.6/setup.py
```

### Comparing `mxlm-0.0.5/README.md` & `mxlm-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.5/mxlm/__info__.py` & `mxlm-0.0.6/mxlm/__info__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 __description__ = "Language Model Utils"
 __license__ = "MIT"
 __author__ = "DIYer22"
 __author_email__ = "ylxx@live.com"
 __maintainer__ = "DIYer22"
 __maintainer_email__ = "ylxx@live.com"
 __github_username__ = "DIYer22"
```

### Comparing `mxlm-0.0.5/mxlm/chat_api.py` & `mxlm-0.0.6/mxlm/chat_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,25 +8,25 @@
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "Just repeat `mxlm`."},
     ]
     default_base_url = None
 
     def __init__(
         self,
-        base_url=None,
+        base_url=None,  # try get OPENAI_BASE_URL env
         api_key=None,  # try get OPENAI_API_KEY env
         model=None,
         temperature=0.5,
         max_tokens=1024,
         top_p=0.9,
         **default_kwargs,
     ):
         from openai import OpenAI
 
-        self.base_url = base_url or self.default_base_url
+        self.base_url = base_url or self.default_base_url or os.environ.get("OPENAI_BASE_URL")
         self.api_key = api_key or os.environ.get("OPENAI_API_KEY", "sk-NoneKey")
 
         # split kwargs to client's kwargs and call kwargs
         client_kwargs = {
             k: default_kwargs.pop(k)
             for k in list(default_kwargs)
             if k in OpenAI.__init__.__code__.co_varnames
@@ -43,15 +43,15 @@
         )
         self.default_kwargs.update(default_kwargs)
 
     def get_model_list(self):
         return self.client.models.list().dict()["data"]
 
     def get_default_model(self):
-        return self.get_model_list()[-1]["id"]
+        return self.get_model_list()[0]["id"]
 
     @staticmethod
     def convert_to_messages(msgs):
         if msgs is None:
             return None
         if isinstance(msgs, str):
             return [{"role": "user", "content": msgs}]
@@ -59,34 +59,15 @@
             messages = []
             for role in ["system", "context", "user", "assistant"]:
                 if role in msgs:
                     messages.append(dict(role=role, content=msgs[role]))
             return messages
         return msgs
 
-    def __call__(
-        self, messages=None, return_messages=False, return_dict=False, **kwargs_
-    ):
-        """
-        messages support str, dict for convenient single-round dialogue, e.g.:
-        >>> client("Tell me a joke.")
-        >>> client(
-            {
-                "system": "you are a helpful assistant.",
-                "user": "Tell me a joke."
-                }
-            )
-        Returns new message.content by default
-        """
-        messages = messages or self.default_messages
-        messages = self.convert_to_messages(messages)
-        kwargs = self.default_kwargs.copy()
-        kwargs.update(kwargs_)
-        if "stream" in kwargs:
-            kwargs["stream"] = bool(kwargs["stream"])
+    def get_dict_by_chat_completions(self, messages, **kwargs):
         response = self.client.chat.completions.create(messages=messages, **kwargs)
         if kwargs.get("stream"):
             content = ""
             chunki = -1
             for tryi in range(1, 6):
                 # TODO: remove this Temporary solution for empty stream
                 for chunki, chunk in enumerate(response):
@@ -115,22 +96,63 @@
             chunk.choices[0].message = chunk.choices[0].delta
             del chunk.choices[0].delta
             chunk.choices[0].message.content = content
             chunk.choices[0].message.role = role
             response = chunk
             print(f"<|{response.choices[0].finish_reason}|>")
         # assert response.status_code == 200, response.status_code
+        d = response.dict()
+        return d
+
+    def get_dict_by_completions(self, messages, **kwargs):
+        import requests
+
+        kwargs["prompt"] = messages[-1]["content"]
+        assert not kwargs.get("stream"), "NotImplementedError"
+        completion_url = os.path.join(self.base_url, "completions")
+        # stop_id: 2
+        rsp = requests.post(completion_url, json=kwargs)
+        d = rsp.json()
+        if "choices" in d:
+            if "message" not in d:
+                d["choices"][0]["message"] = dict(content=d["choices"][0]["text"])
+        return d
+
+    def __call__(
+        self, messages=None, return_messages=False, return_dict=False, **kwargs_
+    ):
+        """
+        messages support str, dict for convenient single-round dialogue, e.g.:
+        >>> client("Tell me a joke.")
+        >>> client(
+            {
+                "system": "you are a helpful assistant.",
+                "user": "Tell me a joke."
+                }
+            )
+        Returns new message.content by default
+        """
+        messages = messages or self.default_messages
+        messages = self.convert_to_messages(messages)
+        kwargs = self.default_kwargs.copy()
+        kwargs.update(kwargs_)
+        if "stream" in kwargs:
+            kwargs["stream"] = bool(kwargs["stream"])
+        is_completions = kwargs.pop("completions") if "completions" in kwargs else False
+        if is_completions:
+            d = self.get_dict_by_completions(messages, **kwargs)
+        else:
+            d = self.get_dict_by_chat_completions(messages, **kwargs)
         if return_messages or return_dict:
-            d = response.dict()
             d["new_messages"] = messages + [d["choices"][0]["message"]]
             if return_dict:
                 return d
             elif return_messages:
                 return d["new_messages"]
-        return response.choices[0].message.content
+        return d["choices"][0]["message"]["content"]
 
     @property
     def model(self):
         return self.default_kwargs.get("model")
 
     def __str__(self):
         import json
```

### Comparing `mxlm-0.0.5/mxlm/chatmd_utils.py` & `mxlm-0.0.6/mxlm/chatmd_utils.py`

 * *Files identical despite different names*

### Comparing `mxlm-0.0.5/setup.py` & `mxlm-0.0.6/setup.py`

 * *Files identical despite different names*

