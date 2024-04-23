# Comparing `tmp/uac-api-0.2.0.tar.gz` & `tmp/uac-api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uac-api-0.2.0.tar", last modified: Tue Apr 23 03:36:38 2024, max compression
+gzip compressed data, was "uac-api-0.2.1.tar", last modified: Tue Apr 23 04:58:04 2024, max compression
```

## Comparing `uac-api-0.2.0.tar` & `uac-api-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-23 03:36:38.855628 uac-api-0.2.0/
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      442 2024-04-23 03:36:38.855431 uac-api-0.2.0/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403       58 2024-04-22 13:04:30.000000 uac-api-0.2.0/README.md
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 17:21:03.000000 uac-api-0.2.0/pyproject.toml
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403       38 2024-04-23 03:36:38.855671 uac-api-0.2.0/setup.cfg
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      904 2024-04-22 21:21:10.000000 uac-api-0.2.0/setup.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-23 03:36:38.841625 uac-api-0.2.0/uac_api.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      442 2024-04-23 03:36:38.000000 uac-api-0.2.0/uac_api.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      834 2024-04-23 03:36:38.000000 uac-api-0.2.0/uac_api.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        1 2024-04-23 03:36:38.000000 uac-api-0.2.0/uac_api.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        9 2024-04-23 03:36:38.000000 uac-api-0.2.0/uac_api.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        7 2024-04-23 03:36:38.000000 uac-api-0.2.0/uac_api.egg-info/top_level.txt
-drwxr-xr-x   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-23 03:36:38.855129 uac-api-0.2.0/uacapi/
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     5077 2024-04-23 03:18:38.000000 uac-api-0.2.0/uacapi/__init__.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     2138 2024-04-23 03:28:39.000000 uac-api-0.2.0/uacapi/agents.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     1764 2024-04-23 03:35:23.000000 uac-api-0.2.0/uacapi/audits.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/bundles.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      350 2024-04-22 21:45:13.000000 uac-api-0.2.0/uacapi/business_services.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/calendars.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/connections.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      110 2024-04-22 15:25:41.000000 uac-api-0.2.0/uacapi/credentials.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      818 2024-04-22 21:44:23.000000 uac-api-0.2.0/uacapi/custom_days.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/groups.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/ldap.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/metrics.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/oauth_clients.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/oms_servers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     3257 2024-04-22 12:58:51.000000 uac-api-0.2.0/uacapi/payload.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/properties.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/reports.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 13:00:05.000000 uac-api-0.2.0/uacapi/requirements.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     1244 2024-04-22 21:48:18.000000 uac-api-0.2.0/uacapi/scripts.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/simulations.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/system.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     1483 2024-04-22 22:02:43.000000 uac-api-0.2.0/uacapi/task_instances.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     2517 2024-04-22 21:57:22.000000 uac-api-0.2.0/uacapi/tasks.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      107 2024-04-22 15:25:48.000000 uac-api-0.2.0/uacapi/triggers.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 16:29:41.000000 uac-api-0.2.0/uacapi/uc.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      491 2024-04-22 16:25:20.000000 uac-api-0.2.0/uacapi/universal_events.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/universal_templates.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/users.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403     5036 2024-04-22 13:05:09.000000 uac-api-0.2.0/uacapi/utils.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/variables.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403      342 2024-04-22 22:03:55.000000 uac-api-0.2.0/uacapi/virtual_resources.py
--rw-r--r--   0 h.gomleksizoglu (612458557) 287026403        0 2024-04-22 15:23:03.000000 uac-api-0.2.0/uacapi/webhooks.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-23 04:58:04.549392 uac-api-0.2.1/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      442 2024-04-23 04:58:04.549206 uac-api-0.2.1/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       58 2024-04-22 13:04:30.000000 uac-api-0.2.1/README.md
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 17:21:03.000000 uac-api-0.2.1/pyproject.toml
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-23 04:58:04.549435 uac-api-0.2.1/setup.cfg
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      904 2024-04-22 21:21:10.000000 uac-api-0.2.1/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-23 04:58:04.533429 uac-api-0.2.1/uac_api.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      442 2024-04-23 04:58:04.000000 uac-api-0.2.1/uac_api.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      834 2024-04-23 04:58:04.000000 uac-api-0.2.1/uac_api.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-23 04:58:04.000000 uac-api-0.2.1/uac_api.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        9 2024-04-23 04:58:04.000000 uac-api-0.2.1/uac_api.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        7 2024-04-23 04:58:04.000000 uac-api-0.2.1/uac_api.egg-info/top_level.txt
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-23 04:58:04.548908 uac-api-0.2.1/uacapi/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5077 2024-04-23 03:51:29.000000 uac-api-0.2.1/uacapi/__init__.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2138 2024-04-23 03:28:39.000000 uac-api-0.2.1/uacapi/agents.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1764 2024-04-23 03:35:23.000000 uac-api-0.2.1/uacapi/audits.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/bundles.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      350 2024-04-22 21:45:13.000000 uac-api-0.2.1/uacapi/business_services.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/calendars.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/connections.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      110 2024-04-22 15:25:41.000000 uac-api-0.2.1/uacapi/credentials.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      818 2024-04-22 21:44:23.000000 uac-api-0.2.1/uacapi/custom_days.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/groups.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/ldap.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/metrics.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/oauth_clients.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/oms_servers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     3257 2024-04-22 12:58:51.000000 uac-api-0.2.1/uacapi/payload.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/properties.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/reports.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 13:00:05.000000 uac-api-0.2.1/uacapi/requirements.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1244 2024-04-22 21:48:18.000000 uac-api-0.2.1/uacapi/scripts.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/simulations.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/system.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1483 2024-04-22 22:02:43.000000 uac-api-0.2.1/uacapi/task_instances.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2517 2024-04-22 21:57:22.000000 uac-api-0.2.1/uacapi/tasks.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      107 2024-04-22 15:25:48.000000 uac-api-0.2.1/uacapi/triggers.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 16:29:41.000000 uac-api-0.2.1/uacapi/uc.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      491 2024-04-22 16:25:20.000000 uac-api-0.2.1/uacapi/universal_events.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/universal_templates.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/users.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5036 2024-04-22 13:05:09.000000 uac-api-0.2.1/uacapi/utils.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/variables.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      342 2024-04-22 22:03:55.000000 uac-api-0.2.1/uacapi/virtual_resources.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-22 15:23:03.000000 uac-api-0.2.1/uacapi/webhooks.py
```

### Comparing `uac-api-0.2.0/setup.py` & `uac-api-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uac_api.egg-info/SOURCES.txt` & `uac-api-0.2.1/uac_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/__init__.py` & `uac-api-0.2.1/uacapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .tasks import Tasks
 from .task_instances import TaskInstances
 from .scripts import Scripts
 from .universal_events import UniversalEvents
 from .virtual_resources import VirtualResources
 from .utils import strip_url
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 class UniversalController():
     def __init__(self, base_url, credential=None, token=None, ssl_verify=True, logger=None, headers=None) -> None:
         self.log = logger
         self.base_url = strip_url(base_url)
         self.token = token
         self.ssl_verify = ssl_verify
```

### Comparing `uac-api-0.2.0/uacapi/agents.py` & `uac-api-0.2.1/uacapi/agents.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/audits.py` & `uac-api-0.2.1/uacapi/audits.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/custom_days.py` & `uac-api-0.2.1/uacapi/custom_days.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/payload.py` & `uac-api-0.2.1/uacapi/payload.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/scripts.py` & `uac-api-0.2.1/uacapi/scripts.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/task_instances.py` & `uac-api-0.2.1/uacapi/task_instances.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/tasks.py` & `uac-api-0.2.1/uacapi/tasks.py`

 * *Files identical despite different names*

### Comparing `uac-api-0.2.0/uacapi/utils.py` & `uac-api-0.2.1/uacapi/utils.py`

 * *Files identical despite different names*

