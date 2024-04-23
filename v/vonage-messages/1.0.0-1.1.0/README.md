# Comparing `tmp/vonage-messages-1.0.0.tar.gz` & `tmp/vonage_messages-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage-messages-1.0.0.tar", last modified: Wed Apr 10 20:20:27 2024, max compression
+gzip compressed data, was "vonage_messages-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
```

## Comparing `vonage-messages-1.0.0.tar` & `vonage_messages-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-10 20:20:27.142377 vonage-messages-1.0.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-10 20:20:27.139045 vonage-messages-1.0.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     2510 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      836 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-10 20:20:27.142649 vonage-messages-1.0.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-10 20:20:27.113054 vonage-messages-1.0.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-10 20:20:27.118771 vonage-messages-1.0.0/src/vonage_messages/
--rw-r--r--   0 mkahan     (503) staff       (20)      152 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1344 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/messages.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-10 20:20:27.136695 vonage-messages-1.0.0/src/vonage_messages/models/
--rw-r--r--   0 mkahan     (503) staff       (20)     2136 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      361 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/base_message.py
--rw-r--r--   0 mkahan     (503) staff       (20)      548 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/enums.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1490 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/messenger.py
--rw-r--r--   0 mkahan     (503) staff       (20)      955 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/mms.py
--rw-r--r--   0 mkahan     (503) staff       (20)      685 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/sms.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2485 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/viber.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2400 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/models/whatsapp.py
--rw-r--r--   0 mkahan     (503) staff       (20)      226 2024-04-10 20:20:25.000000 vonage-messages-1.0.0/src/vonage_messages/responses.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-10 20:20:27.137946 vonage-messages-1.0.0/src/vonage_messages.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-10 20:20:27.000000 vonage-messages-1.0.0/src/vonage_messages.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      652 2024-04-10 20:20:27.000000 vonage-messages-1.0.0/src/vonage_messages.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-10 20:20:27.000000 vonage-messages-1.0.0/src/vonage_messages.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-10 20:20:27.000000 vonage-messages-1.0.0/src/vonage_messages.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       16 2024-04-10 20:20:27.000000 vonage-messages-1.0.0/src/vonage_messages.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.251484 vonage_messages-1.1.0/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-23 14:16:53.250993 vonage_messages-1.1.0/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2510 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      836 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.251541 vonage_messages-1.1.0/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.228661 vonage_messages-1.1.0/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.233991 vonage_messages-1.1.0/src/vonage_messages/
+-rw-r--r--   0 mkahan     (503) staff       (20)      152 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1616 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/messages.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.249880 vonage_messages-1.1.0/src/vonage_messages/models/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2136 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      348 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/base_message.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      548 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/enums.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1490 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/messenger.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      942 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/mms.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      672 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/sms.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2485 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/viber.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2387 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/whatsapp.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      221 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/responses.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.250434 vonage_messages-1.1.0/src/vonage_messages.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      652 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       16 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/top_level.txt
```

### Comparing `vonage-messages-1.0.0/PKG-INFO` & `vonage_messages-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-messages
-Version: 1.0.0
+Version: 1.1.0
 Summary: Vonage messages package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.2.1
-Requires-Dist: vonage-utils>=1.0.1
+Requires-Dist: vonage-http-client>=1.3.0
+Requires-Dist: vonage-utils>=1.1.0
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage Messages Package
 
 This package contains the code to use [Vonage's Messages API](https://developer.vonage.com/en/messages/overview) in Python.
 
 ## Usage
```

### Comparing `vonage-messages-1.0.0/README.md` & `vonage_messages-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vonage-messages-1.0.0/backend_shim.py` & `vonage_messages-1.1.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage-messages-1.0.0/pyproject.toml` & `vonage_messages-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = 'vonage-messages'
-version = '1.0.0'
+version = '1.1.0'
 description = 'Vonage messages package'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-http-client>=1.2.1",
-  "vonage-utils>=1.0.1",
+  "vonage-http-client>=1.3.0",
+  "vonage-utils>=1.1.0",
   "pydantic>=2.6.1",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
```

### Comparing `vonage-messages-1.0.0/src/vonage_messages/messages.py` & `vonage_messages-1.1.0/src/vonage_messages/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,23 @@
     Args:
         http_client (HttpClient): An instance of the HttpClient class used to make HTTP requests.
     """
 
     def __init__(self, http_client: HttpClient) -> None:
         self._http_client = http_client
 
+    @property
+    def http_client(self) -> HttpClient:
+        """The HTTP client used to make requests to the Messages API.
+
+        Returns:
+            HttpClient: The HTTP client used to make requests to the Messages API.
+        """
+        return self._http_client
+
     @validate_call
     def send(self, message: BaseMessage) -> SendMessageResponse:
         """Send a message using Vonage's Messages API.
 
         Args:
             message (BaseMessage): The message to be sent as a Pydantic model.
                 Use the provided models (in `vonage_messages.models`) to create messages and pass them in to this method.
```

### Comparing `vonage-messages-1.0.0/src/vonage_messages/models/__init__.py` & `vonage_messages-1.1.0/src/vonage_messages/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vonage-messages-1.0.0/src/vonage_messages/models/enums.py` & `vonage_messages-1.1.0/src/vonage_messages/models/enums.py`

 * *Files identical despite different names*

### Comparing `vonage-messages-1.0.0/src/vonage_messages/models/messenger.py` & `vonage_messages-1.1.0/src/vonage_messages/models/messenger.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal, Optional
 
 from pydantic import BaseModel, Field, model_validator
 
-from .enums import ChannelType, MessageType
 from .base_message import BaseMessage
+from .enums import ChannelType, MessageType
 
 
 class MessengerResource(BaseModel):
     url: str
 
 
 class MessengerOptions(BaseModel):
```

### Comparing `vonage-messages-1.0.0/src/vonage_messages/models/mms.py` & `vonage_messages-1.1.0/src/vonage_messages/models/mms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Union
 
 from pydantic import BaseModel, Field
-from vonage_utils.types.phone_number import PhoneNumber
+from vonage_utils.types import PhoneNumber
 
-from .enums import ChannelType, MessageType
 from .base_message import BaseMessage
+from .enums import ChannelType, MessageType
 
 
 class MmsResource(BaseModel):
     url: str
     caption: Optional[str] = Field(None, min_length=1, max_length=2000)
```

### Comparing `vonage-messages-1.0.0/src/vonage_messages/models/viber.py` & `vonage_messages-1.1.0/src/vonage_messages/models/viber.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal, Optional
 
 from pydantic import BaseModel, Field, field_validator
 
-from .enums import ChannelType, MessageType
 from .base_message import BaseMessage
+from .enums import ChannelType, MessageType
 
 
 class ViberAction(BaseModel):
     url: str
     text: str = Field(..., max_length=30)
```

### Comparing `vonage-messages-1.0.0/src/vonage_messages/models/whatsapp.py` & `vonage_messages-1.1.0/src/vonage_messages/models/whatsapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Literal, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field
-from vonage_utils.types.phone_number import PhoneNumber
+from vonage_utils.types import PhoneNumber
 
-from .enums import ChannelType, MessageType
 from .base_message import BaseMessage
+from .enums import ChannelType, MessageType
 
 
 class WhatsappContext(BaseModel):
     message_uuid: str
 
 
 class BaseWhatsapp(BaseMessage):
```

### Comparing `vonage-messages-1.0.0/src/vonage_messages.egg-info/PKG-INFO` & `vonage_messages-1.1.0/src/vonage_messages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: vonage-messages
-Version: 1.0.0
+Version: 1.1.0
 Summary: Vonage messages package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.2.1
-Requires-Dist: vonage-utils>=1.0.1
+Requires-Dist: vonage-http-client>=1.3.0
+Requires-Dist: vonage-utils>=1.1.0
 Requires-Dist: pydantic>=2.6.1
 
 # Vonage Messages Package
 
 This package contains the code to use [Vonage's Messages API](https://developer.vonage.com/en/messages/overview) in Python.
 
 ## Usage
```

### Comparing `vonage-messages-1.0.0/src/vonage_messages.egg-info/SOURCES.txt` & `vonage_messages-1.1.0/src/vonage_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

