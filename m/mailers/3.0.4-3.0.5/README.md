# Comparing `tmp/mailers-3.0.4.tar.gz` & `tmp/mailers-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailers-3.0.4.tar", max compression
+gzip compressed data, was "mailers-3.0.5.tar", max compression
```

## Comparing `mailers-3.0.4.tar` & `mailers-3.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1073 2024-04-16 19:54:26.363280 mailers-3.0.4/LICENSE
--rw-r--r--   0        0        0     9774 2024-04-16 19:54:26.363280 mailers-3.0.4/README.md
--rw-r--r--   0        0        0      829 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/__init__.py
--rw-r--r--   0        0        0       53 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/encrypters/__init__.py
--rw-r--r--   0        0        0      220 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/encrypters/base.py
--rw-r--r--   0        0        0      454 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/exceptions.py
--rw-r--r--   0        0        0     1930 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/factories.py
--rw-r--r--   0        0        0     5475 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/mailer.py
--rw-r--r--   0        0        0    12388 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/message.py
--rw-r--r--   0        0        0      159 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/preprocessors/__init__.py
--rw-r--r--   0        0        0      690 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/preprocessors/cssliner.py
--rw-r--r--   0        0        0        0 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/py.typed
--rw-r--r--   0        0        0      236 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/pytest_plugin.py
--rw-r--r--   0        0        0       47 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/signers/__init__.py
--rw-r--r--   0        0        0      214 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/signers/base.py
--rw-r--r--   0        0        0     1870 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/signers/dkim.py
--rw-r--r--   0        0        0      406 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/__init__.py
--rw-r--r--   0        0        0      250 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/base.py
--rw-r--r--   0        0        0      488 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/console.py
--rw-r--r--   0        0        0      709 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/file.py
--rw-r--r--   0        0        0      514 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/memory.py
--rw-r--r--   0        0        0      914 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/multi.py
--rw-r--r--   0        0        0      216 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/null.py
--rw-r--r--   0        0        0     1190 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/smtp.py
--rw-r--r--   0        0        0      304 2024-04-16 19:54:26.363280 mailers-3.0.4/mailers/transports/stream.py
--rw-r--r--   0        0        0     2379 2024-04-16 19:54:26.363280 mailers-3.0.4/pyproject.toml
--rw-r--r--   0        0        0    11154 1970-01-01 00:00:00.000000 mailers-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-23 17:30:13.993399 mailers-3.0.5/LICENSE
+-rw-r--r--   0        0        0     9768 2024-04-23 17:30:13.993399 mailers-3.0.5/README.md
+-rw-r--r--   0        0        0      829 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/__init__.py
+-rw-r--r--   0        0        0       53 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/encrypters/__init__.py
+-rw-r--r--   0        0        0      220 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/encrypters/base.py
+-rw-r--r--   0        0        0      454 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/exceptions.py
+-rw-r--r--   0        0        0     1930 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/factories.py
+-rw-r--r--   0        0        0     5475 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/mailer.py
+-rw-r--r--   0        0        0    12388 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/message.py
+-rw-r--r--   0        0        0      159 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/preprocessors/__init__.py
+-rw-r--r--   0        0        0      690 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/preprocessors/cssliner.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/py.typed
+-rw-r--r--   0        0        0      236 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/pytest_plugin.py
+-rw-r--r--   0        0        0       47 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/signers/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/signers/base.py
+-rw-r--r--   0        0        0     1870 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/signers/dkim.py
+-rw-r--r--   0        0        0      406 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/__init__.py
+-rw-r--r--   0        0        0      250 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/base.py
+-rw-r--r--   0        0        0      488 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/console.py
+-rw-r--r--   0        0        0      709 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/file.py
+-rw-r--r--   0        0        0      514 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/memory.py
+-rw-r--r--   0        0        0      914 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/multi.py
+-rw-r--r--   0        0        0      216 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/null.py
+-rw-r--r--   0        0        0     1199 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/smtp.py
+-rw-r--r--   0        0        0      304 2024-04-23 17:30:13.997399 mailers-3.0.5/mailers/transports/stream.py
+-rw-r--r--   0        0        0     2379 2024-04-23 17:30:13.997399 mailers-3.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11148 1970-01-01 00:00:00.000000 mailers-3.0.5/PKG-INFO
```

### Comparing `mailers-3.0.4/LICENSE` & `mailers-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/README.md` & `mailers-3.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * fallback transports
 * global From address
 * templated emails
 
 ## Usage
 
 ```bash
-pip install mailers[aiosmtplib]
+pip install mailers[smtp]
 ```
 
 Then create mailer:
 
 ```python
 from mailers import Mailer
```

### Comparing `mailers-3.0.4/mailers/__init__.py` & `mailers-3.0.5/mailers/__init__.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/factories.py` & `mailers-3.0.5/mailers/factories.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/mailer.py` & `mailers-3.0.5/mailers/mailer.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/message.py` & `mailers-3.0.5/mailers/message.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/preprocessors/cssliner.py` & `mailers-3.0.5/mailers/preprocessors/cssliner.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/signers/dkim.py` & `mailers-3.0.5/mailers/signers/dkim.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/transports/file.py` & `mailers-3.0.5/mailers/transports/file.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/transports/memory.py` & `mailers-3.0.5/mailers/transports/memory.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/transports/multi.py` & `mailers-3.0.5/mailers/transports/multi.py`

 * *Files identical despite different names*

### Comparing `mailers-3.0.4/mailers/transports/smtp.py` & `mailers-3.0.5/mailers/transports/smtp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import aiosmtplib
 import typing
 from email.message import Message
 
 from mailers.transports.base import Transport
 
 
 class SMTPTransport(Transport):
@@ -25,14 +24,16 @@
         self._password = password
         self._use_tls = use_tls or False
         self._timeout = timeout
         self._key_file = key_file
         self._cert_file = cert_file
 
     async def send(self, message: Message) -> None:
+        import aiosmtplib
+
         await aiosmtplib.send(
             message,
             hostname=self._host,
             port=self._port,
             use_tls=self._use_tls,
             username=self._user,
             password=self._password,
```

### Comparing `mailers-3.0.4/pyproject.toml` & `mailers-3.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mailers"
-version = "3.0.4"
+version = "3.0.5"
 description = "Email delivery for asyncio."
 authors = ["alex.oleshkevich <alex.oleshkevich@gmail.com>"]
 license = "MIT"
 readme = 'README.md'
 homepage = 'https://github.com/alex-oleshkevich/mailers'
 repository = 'https://github.com/alex-oleshkevich/mailers.git'
 documentation = "https://github.com/alex-oleshkevich/mailers"
```

### Comparing `mailers-3.0.4/PKG-INFO` & `mailers-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailers
-Version: 3.0.4
+Version: 3.0.5
 Summary: Email delivery for asyncio.
 Home-page: https://github.com/alex-oleshkevich/mailers
 License: MIT
 Keywords: asyncio,email,mailer,mail
 Author: alex.oleshkevich
 Author-email: alex.oleshkevich@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -58,15 +58,15 @@
 * fallback transports
 * global From address
 * templated emails
 
 ## Usage
 
 ```bash
-pip install mailers[aiosmtplib]
+pip install mailers[smtp]
 ```
 
 Then create mailer:
 
 ```python
 from mailers import Mailer
```

