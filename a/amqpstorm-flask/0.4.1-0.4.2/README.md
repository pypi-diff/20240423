# Comparing `tmp/amqpstorm_flask-0.4.1.tar.gz` & `tmp/amqpstorm_flask-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqpstorm_flask-0.4.1.tar", last modified: Mon Apr 22 11:24:02 2024, max compression
+gzip compressed data, was "amqpstorm_flask-0.4.2.tar", last modified: Tue Apr 23 14:17:01 2024, max compression
```

## Comparing `amqpstorm_flask-0.4.1.tar` & `amqpstorm_flask-0.4.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:24:02.517534 amqpstorm_flask-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-22 11:23:57.000000 amqpstorm_flask-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-22 11:24:02.517534 amqpstorm_flask-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-22 11:23:57.000000 amqpstorm_flask-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-22 11:23:57.000000 amqpstorm_flask-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:24:02.517534 amqpstorm_flask-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:24:02.513534 amqpstorm_flask-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:24:02.517534 amqpstorm_flask-0.4.1/src/amqpstorm_flask/
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-04-22 11:23:57.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask/RabbitMQ.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 11:23:57.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 11:23:57.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask/exchange_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-22 11:23:57.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask/queue_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 11:24:02.517534 amqpstorm_flask-0.4.1/src/amqpstorm_flask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-22 11:24:02.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-22 11:24:02.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 11:24:02.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 11:24:02.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-22 11:24:02.000000 amqpstorm_flask-0.4.1/src/amqpstorm_flask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:17:01.147365 amqpstorm_flask-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-23 14:16:56.000000 amqpstorm_flask-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-23 14:17:01.143365 amqpstorm_flask-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-23 14:16:56.000000 amqpstorm_flask-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-23 14:16:56.000000 amqpstorm_flask-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:17:01.147365 amqpstorm_flask-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:17:01.143365 amqpstorm_flask-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:17:01.143365 amqpstorm_flask-0.4.2/src/amqpstorm_flask/
+-rw-r--r--   0 runner    (1001) docker     (127)     9450 2024-04-23 14:16:56.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask/RabbitMQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 14:16:56.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 14:16:56.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask/exchange_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-23 14:16:56.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask/queue_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:17:01.143365 amqpstorm_flask-0.4.2/src/amqpstorm_flask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22647 2024-04-23 14:17:01.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-23 14:17:01.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:17:01.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:17:01.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 14:17:01.000000 amqpstorm_flask-0.4.2/src/amqpstorm_flask.egg-info/top_level.txt
```

### Comparing `amqpstorm_flask-0.4.1/LICENSE` & `amqpstorm_flask-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amqpstorm_flask-0.4.1/PKG-INFO` & `amqpstorm_flask-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqpstorm-flask
-Version: 0.4.1
+Version: 0.4.2
 Summary: amqpstorm library for Flask
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `amqpstorm_flask-0.4.1/README.md` & `amqpstorm_flask-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `amqpstorm_flask-0.4.1/pyproject.toml` & `amqpstorm_flask-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amqpstorm-flask"
-version = "0.4.1"
+version = "0.4.2"
 description = "amqpstorm library for Flask"
 readme = "README.md"
 authors = [{ name = "Inuits", email = "developers@inuits.eu" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Intended Audience :: Developers",
```

### Comparing `amqpstorm_flask-0.4.1/src/amqpstorm_flask/RabbitMQ.py` & `amqpstorm_flask-0.4.2/src/amqpstorm_flask/RabbitMQ.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,17 +194,16 @@
         if queue_arguments is None:
             queue_arguments = {"x-queue-type": "quorum"}
 
         def decorator(f):
             queue = f.__name__.replace("_", getenv("MQ_DELIMITER", ".")) if queue_name is None else queue_name
 
             enabled_queues = None if getenv("MQ_QUEUES") is None else getenv("MQ_QUEUES").split(",")
-            all_queues_enabled = enabled_queues is None
 
-            if queue in enabled_queues or all_queues_enabled:
+            if enabled_queues is None or queue in enabled_queues:
                 @wraps(f)
                 def new_consumer():
                     retries = 0
                     while retries <= max_retries:
                         try:
                             self._validate_channel_connection()
                             self.channel.exchange.declare(
```

### Comparing `amqpstorm_flask-0.4.1/src/amqpstorm_flask.egg-info/PKG-INFO` & `amqpstorm_flask-0.4.2/src/amqpstorm_flask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqpstorm-flask
-Version: 0.4.1
+Version: 0.4.2
 Summary: amqpstorm library for Flask
 Author-email: Inuits <developers@inuits.eu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

