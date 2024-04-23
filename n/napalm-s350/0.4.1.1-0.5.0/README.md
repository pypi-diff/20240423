# Comparing `tmp/napalm-s350-0.4.1.1.tar.gz` & `tmp/napalm_s350-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm-s350-0.4.1.1.tar", last modified: Fri Apr  5 06:17:16 2024, max compression
+gzip compressed data, was "napalm_s350-0.5.0.tar", last modified: Tue Apr 23 07:07:54 2024, max compression
```

## Comparing `napalm-s350-0.4.1.1.tar` & `napalm_s350-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.292621 napalm-s350-0.4.1.1/napalm_s350/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/s350.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/napalm_s350/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/napalm_s350/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/napalm_s350/utils/textfsm_templates/hosts.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/napalm_s350.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 06:17:16.000000 napalm-s350-0.4.1.1/napalm_s350.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-05 06:17:16.296621 napalm-s350-0.4.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-05 06:17:03.000000 napalm-s350-0.4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/s350.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350/utils/textfsm_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/utils/textfsm_templates/hosts.tpl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/setup.py
```

### Comparing `napalm-s350-0.4.1.1/LICENSE` & `napalm_s350-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm-s350-0.4.1.1/PKG-INFO` & `napalm_s350-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-s350
-Version: 0.4.1.1
+Version: 0.5.0
 Summary: NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)
 Home-page: https://github.com/napalm-automation-community/napalm-s350
 Author: Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher
 Author-email: j@jasper.la, qaxi@seznam.cz, mail@phill93.de
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,19 +25,20 @@
 Requires-Dist: netaddr>=1.2.1
 
 # Napalm-s350
 
 NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
 
 ## Status
-Master: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=master&event=push)
 
-Develop: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=develop&event=push)
+Master: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
-PyPi: [![Upload](https://github.com/napalm-automation-community/napalm-s350/workflows/Upload%20Python%20Package%20to%20PyPi.org/badge.svg)](https://github.com/napalm-automation-community/napalm-s350/actions?query=workflow%3A%22Upload+Python+Package+to+PyPi.org%22)
+Develop: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=develop)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
+
+PyPi.org: [![Publish To PyPi.org](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/PublishToPIP.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/PublishToPIP.yml)
 
 ## Requirements
 
 Python 3.8+, napalm 4
 
 ## Installation
```

### Comparing `napalm-s350-0.4.1.1/README.md` & `napalm_s350-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Napalm-s350
 
 NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
 
 ## Status
-Master: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=master&event=push)
 
-Develop: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=develop&event=push)
+Master: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
-PyPi: [![Upload](https://github.com/napalm-automation-community/napalm-s350/workflows/Upload%20Python%20Package%20to%20PyPi.org/badge.svg)](https://github.com/napalm-automation-community/napalm-s350/actions?query=workflow%3A%22Upload+Python+Package+to+PyPi.org%22)
+Develop: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=develop)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
+
+PyPi.org: [![Publish To PyPi.org](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/PublishToPIP.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/PublishToPIP.yml)
 
 ## Requirements
 
 Python 3.8+, napalm 4
 
 ## Installation
```

### Comparing `napalm-s350-0.4.1.1/napalm_s350/__init__.py` & `napalm_s350-0.5.0/napalm_s350/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm-s350-0.4.1.1/napalm_s350/s350.py` & `napalm_s350-0.5.0/napalm_s350/s350.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,21 @@
                 "age": 0.0,
             }
 
             arp_table.append(entry)
 
         return arp_table
 
-    def get_config(self, retrieve="all", full=False, sanitized=False):
+    def get_config(
+        self,
+        retrieve="all",
+        full=False,
+        sanitized=False,
+        format: str = "text",
+    ):
         """
         get_config for S350. Since this firmware doesn't support a candidate
         configuration we leave it empty.
         """
 
         configs = {
             "startup": "",
```

### Comparing `napalm-s350-0.4.1.1/napalm_s350.egg-info/PKG-INFO` & `napalm_s350-0.5.0/napalm_s350.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-s350
-Version: 0.4.1.1
+Version: 0.5.0
 Summary: NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)
 Home-page: https://github.com/napalm-automation-community/napalm-s350
 Author: Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher
 Author-email: j@jasper.la, qaxi@seznam.cz, mail@phill93.de
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,19 +25,20 @@
 Requires-Dist: netaddr>=1.2.1
 
 # Napalm-s350
 
 NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
 
 ## Status
-Master: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=master&event=push)
 
-Develop: ![Build](https://github.com/napalm-automation-community/napalm-s350/workflows/Test%20before%20push/badge.svg?branch=develop&event=push)
+Master: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
-PyPi: [![Upload](https://github.com/napalm-automation-community/napalm-s350/workflows/Upload%20Python%20Package%20to%20PyPi.org/badge.svg)](https://github.com/napalm-automation-community/napalm-s350/actions?query=workflow%3A%22Upload+Python+Package+to+PyPi.org%22)
+Develop: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=develop)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
+
+PyPi.org: [![Publish To PyPi.org](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/PublishToPIP.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/PublishToPIP.yml)
 
 ## Requirements
 
 Python 3.8+, napalm 4
 
 ## Installation
```

### Comparing `napalm-s350-0.4.1.1/setup.py` & `napalm_s350-0.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     reqs = [r for r in fs.read().splitlines() if (len(r) > 0 and not r.startswith("#"))]
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setup(
     name="napalm-s350",
-    version="0.4.1.1",
+    version="0.5.0",
     packages=find_packages(exclude=("test*",)),
     author="Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher",
     author_email="j@jasper.la, qaxi@seznam.cz, mail@phill93.de",
     description="NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)",
     license="Apache 2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

