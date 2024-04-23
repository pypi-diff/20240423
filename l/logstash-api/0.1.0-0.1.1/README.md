# Comparing `tmp/logstash_api-0.1.0.tar.gz` & `tmp/logstash-api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logstash_api-0.1.0.tar", last modified: Fri Sep  7 17:41:01 2018, max compression
+gzip compressed data, was "dist/logstash-api-0.1.1.tar", last modified: Tue Apr 23 12:54:39 2024, max compression
```

## Comparing `logstash_api-0.1.0.tar` & `logstash-api-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-07 17:41:01.000000 logstash_api-0.1.0/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash/
--rw-r--r--   0 travis    (2000) travis    (2000)     1250 2018-09-07 17:40:14.000000 logstash_api-0.1.0/src/logstash/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     4226 2018-09-07 17:40:14.000000 logstash_api-0.1.0/src/logstash/base.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash_api.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)      963 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash_api.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      312 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash_api.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash_api.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash_api.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)        7 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash_api.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        9 2018-09-07 17:41:01.000000 logstash_api-0.1.0/src/logstash_api.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     1227 2018-09-07 17:40:14.000000 logstash_api-0.1.0/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)       67 2018-09-07 17:41:01.000000 logstash_api-0.1.0/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     2525 2018-09-07 17:40:14.000000 logstash_api-0.1.0/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)      963 2018-09-07 17:41:01.000000 logstash_api-0.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:54:39.000000 logstash-api-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     2454 2024-04-23 12:54:34.000000 logstash-api-0.1.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-04-23 12:54:34.000000 logstash-api-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-23 12:54:39.000000 logstash-api-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2982 2024-04-23 12:54:39.000000 logstash-api-0.1.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/logstash_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/logstash_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/logstash_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/logstash_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2982 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/logstash_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/logstash_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 12:54:35.000000 logstash-api-0.1.1/src/logstash_api.egg-info/not-zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 12:54:39.000000 logstash-api-0.1.1/src/logstash/
+-rw-r--r--   0 root         (0) root         (0)     4260 2024-04-23 12:54:34.000000 logstash-api-0.1.1/src/logstash/base.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 12:54:34.000000 logstash-api-0.1.1/src/logstash/__init__.py
```

### Comparing `logstash_api-0.1.0/src/logstash/__init__.py` & `logstash-api-0.1.1/src/logstash/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Logstash API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Logstash API.
 #
 # Hive Logstash API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -15,24 +15,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # Apache License for more details.
 #
 # You should have received a copy of the Apache License along with
 # Hive Logstash API. If not, see <http://www.apache.org/licenses/>.
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 from . import base
```

### Comparing `logstash_api-0.1.0/src/logstash/base.py` & `logstash-api-0.1.1/src/logstash/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Logstash API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Logstash API.
 #
 # Hive Logstash API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,99 +18,96 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Logstash API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import json
 import time
 
 import appier
 
 BASE_URL = "http://localhost:8080/"
 """ The default base URL for single operations to be used
 when no other base URL value is provided to the constructor """
 
-class API(
-    appier.API
-):
+
+class API(appier.API):
 
     def __init__(self, *args, **kwargs):
         appier.API.__init__(self, *args, **kwargs)
         self.base_url = appier.conf("LOGSTASH_BASE_URL", BASE_URL)
         self.buffer_size = appier.conf("LOGSTASH_BUFFER_SIZE", 128)
         self.timeout = appier.conf("LOGSTASH_TIMEOUT", 30)
         self.base_url = kwargs.get("base_url", self.base_url)
         self.buffer_size = kwargs.get("buffer_size", self.buffer_size)
         self.timeout = kwargs.get("timeout", self.timeout)
         self.delayer = kwargs.get("delayer", None)
         self._last_flush = time.time()
         self._buffer = []
 
-    def log(self, payload, tag = "default", silent = True):
+    def log(self, payload, tag="default", silent=True):
         url = self.base_url + "tags/%s" % tag
-        contents = self.post(url, data_j = payload, silent = silent)
+        contents = self.post(url, data_j=payload, silent=silent)
         return contents
 
-    def log_bulk(self, logs, tag = "default", silent = True):
+    def log_bulk(self, logs, tag="default", silent=True, raise_e=False, on_error=None):
         url = self.base_url + "tags/%s" % tag
         buffer = []
         for log in logs:
-            log_s = json.dumps(log)
-            log_s = appier.legacy.bytes(log_s, encoding = "utf-8")
-            buffer.append(log_s)
+            try:
+                log_s = json.dumps(log)
+                log_s = appier.legacy.bytes(log_s, encoding="utf-8")
+                buffer.append(log_s)
+            except Exception as exception:
+                if on_error:
+                    on_error(log, exception)
+                if raise_e:
+                    raise
         data = b"\n".join(buffer)
-        contents = self.post(
-            url,
-            data = data,
-            silent = silent,
-            mime = "application/x-ndjson"
-        )
+        contents = self.post(url, data=data, silent=silent, mime="application/x-ndjson")
         return contents
 
     def log_buffer(self, payload):
         self._buffer.append(payload)
-        should_flush = len(self._buffer) >= self.buffer_size or\
-            time.time() > self._last_flush + self.timeout
-        if should_flush: self._flush_buffer()
+        should_flush = (
+            len(self._buffer) >= self.buffer_size
+            or time.time() > self._last_flush + self.timeout
+        )
+        if should_flush:
+            self._flush_buffer()
 
-    def log_flush(self):
-        self._flush_buffer()
+    def log_flush(self, force=True):
+        self._flush_buffer(force=force)
 
-    def _flush_buffer(self, force = False):
+    def _flush_buffer(self, force=False):
         # retrieves some references from the current instance that
         # are going to be used in the flush operation
         buffer = self._buffer
 
         # verifies if the buffer is empty and if that's the case and
         # the force flag is not set, returns immediately
-        if not buffer and not force: return
+        if not buffer and not force:
+            return
 
         # creates the lambda function that is going to be used for the
         # bulk flushing operation of the buffer, this is going to be
         # called on a delayed (async fashion) so that no blocking occurs
         # in the current logical flow
-        call_log = lambda: self.log_bulk(buffer, tag = "default")
+        call_log = lambda: self.log_bulk(buffer, tag="default")
 
         # schedules the call log operation and then empties the buffer
         # so that it's no longer going to be used (flushed), notice that
         # in case there's no delayer available calls the method immediately
-        if self.delayer: self.delayer(call_log)
-        else: call_log()
+        if self.delayer and not force:
+            self.delayer(call_log)
+        else:
+            call_log()
         self._buffer = []
         self._last_flush = time.time()
```

### Comparing `logstash_api-0.1.0/README.md` & `logstash-api-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # [Logstash API](http://logstash-api.hive.pt)
 
 Simple Python API client for [Logstash](https://www.elastic.co/products/logstash).
 
 ## Configuration
 
-* `LOSTASH_BASE_URL` (`str`) - The base URL value to be used to communicate using the Logstash API, should include username and password
-if HTTP Auth is used (defaults to `None`)
-* `LOSTASH_BUFFER_SIZE` (`int`) - The size of the buffer (in number of entries) until the buffer is flushed (defaults to `128`)
-* `LOSTASH_TIMEOUT` (`int`) - The timeout in seconds in seconds until the buffer is flushed (defaults to `30`)
+| Name                     | Type  | Description                                                                                                                                          |
+| ------------------------ | ----- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
+| **LOGSTASH_BASE_URL**    | `str` | The base URL value to be used to communicate using the Logstash API, should include username and password if HTTP Auth is used (defaults to `None`). |
+| **LOGSTASH_BUFFER_SIZE** | `int` | The size of the buffer (in number of entries) until the buffer is flushed (defaults to `128`).                                                       |
+| **LOGSTASH_TIMEOUT**     | `int` | The timeout in seconds in seconds until the buffer is flushed (defaults to `30`).                                                                    |
 
 ## License
 
 Logstash API is currently licensed under the [Apache License, Version 2.0](http://www.apache.org/licenses/).
 
 ## Build Automation
 
-[![Build Status](https://travis-ci.org/hivesolutions/logstash_api.svg?branch=master)](https://travis-ci.org/hivesolutions/logstash_api)
-[![Coverage Status](https://coveralls.io/repos/hivesolutions/logstash_api/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/logstash_api?branch=master)
-[![PyPi Status](https://img.shields.io/pypi/v/logstash_api.svg)](https://pypi.python.org/pypi/logstash_api)
+[![Build Status](https://app.travis-ci.com/hivesolutions/logstash-api.svg?branch=master)](https://travis-ci.com/github/hivesolutions/logstash-api)
+[![Coverage Status](https://coveralls.io/repos/hivesolutions/logstash-api/badge.svg?branch=master)](https://coveralls.io/r/hivesolutions/logstash-api?branch=master)
+[![PyPi Status](https://img.shields.io/pypi/v/logstash-api.svg)](https://pypi.python.org/pypi/logstash-api)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://www.apache.org/licenses/)
```

### Comparing `logstash_api-0.1.0/setup.py` & `logstash-api-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 # Hive Logstash API
-# Copyright (c) 2008-2018 Hive Solutions Lda.
+# Copyright (c) 2008-2024 Hive Solutions Lda.
 #
 # This file is part of Hive Logstash API.
 #
 # Hive Logstash API is free software: you can redistribute it and/or modify
 # it under the terms of the Apache License as published by the Apache
 # Foundation, either version 2.0 of the License, or (at your option) any
 # later version.
@@ -18,61 +18,51 @@
 #
 # You should have received a copy of the Apache License along with
 # Hive Logstash API. If not, see <http://www.apache.org/licenses/>.
 
 __author__ = "João Magalhães <joamag@hive.pt>"
 """ The author(s) of the module """
 
-__version__ = "1.0.0"
-""" The version of the module """
-
-__revision__ = "$LastChangedRevision$"
-""" The revision number of the module """
-
-__date__ = "$LastChangedDate$"
-""" The last change date of the module """
-
-__copyright__ = "Copyright (c) 2008-2018 Hive Solutions Lda."
+__copyright__ = "Copyright (c) 2008-2024 Hive Solutions Lda."
 """ The copyright for the module """
 
 __license__ = "Apache License, Version 2.0"
 """ The license for the module """
 
 import os
 import setuptools
 
 setuptools.setup(
-    name = "logstash_api",
-    version = "0.1.0",
-    author = "Hive Solutions Lda.",
-    author_email = "development@hive.pt",
-    description = "Logstash API Client",
-    license = "Apache License, Version 2.0",
-    keywords = "logstash api",
-    url = "http://logstash-api.hive.pt",
-    zip_safe = False,
-    packages = [
-        "logstash"
-    ],
-    package_dir = {
-        "" : os.path.normpath("src")
-    },
-    install_requires = [
-        "appier"
-    ],
-    classifiers = [
+    name="logstash-api",
+    version="0.1.1",
+    author="Hive Solutions Lda.",
+    author_email="development@hive.pt",
+    description="Logstash API Client",
+    license="Apache License, Version 2.0",
+    keywords="logstash api",
+    url="http://logstash-api.hive.pt",
+    zip_safe=False,
+    packages=["logstash"],
+    package_dir={"": os.path.normpath("src")},
+    install_requires=["appier"],
+    classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2.6",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6"
-    ]
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+    ],
+    long_description=open(os.path.join(os.path.dirname(__file__), "README.md"), "rb")
+    .read()
+    .decode("utf-8"),
+    long_description_content_type="text/markdown",
 )
```

