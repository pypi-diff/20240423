# Comparing `tmp/chiasmodon-1.1.8.tar.gz` & `tmp/chiasmodon-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.1.8.tar", last modified: Thu Apr 18 23:44:05 2024, max compression
+gzip compressed data, was "chiasmodon-1.1.9.tar", last modified: Thu Apr 18 23:54:08 2024, max compression
```

## Comparing `chiasmodon-1.1.8.tar` & `chiasmodon-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:44:05.029685 chiasmodon-1.1.8/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.8/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 23:44:05.029685 chiasmodon-1.1.8/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13873 2024-04-18 03:14:25.000000 chiasmodon-1.1.8/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:44:05.029685 chiasmodon-1.1.8/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 23:44:04.000000 chiasmodon-1.1.8/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 23:44:05.000000 chiasmodon-1.1.8/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 23:44:04.000000 chiasmodon-1.1.8/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 23:44:04.000000 chiasmodon-1.1.8/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 23:44:04.000000 chiasmodon-1.1.8/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:44:05.029685 chiasmodon-1.1.8/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21181 2024-04-18 23:43:55.000000 chiasmodon-1.1.8/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18598 2024-04-18 23:43:45.000000 chiasmodon-1.1.8/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 23:44:05.029685 chiasmodon-1.1.8/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 23:43:47.000000 chiasmodon-1.1.8/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.9/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13873 2024-04-18 03:14:25.000000 chiasmodon-1.1.9/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    14419 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 23:54:08.000000 chiasmodon-1.1.9/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21181 2024-04-18 23:43:55.000000 chiasmodon-1.1.9/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18945 2024-04-18 23:53:55.000000 chiasmodon-1.1.9/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 23:54:08.209658 chiasmodon-1.1.9/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 23:53:53.000000 chiasmodon-1.1.9/setup.py
```

### Comparing `chiasmodon-1.1.8/LICENSE.txt` & `chiasmodon-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.8/PKG-INFO` & `chiasmodon-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.8
+Version: 1.1.9
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.8/README.md` & `chiasmodon-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.8/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.1.9/chiasmodon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.8
+Version: 1.1.9
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.8/cli/chiasmodon_cli.py` & `chiasmodon-1.1.9/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.8/pychiasmodon.py` & `chiasmodon-1.1.9/pychiasmodon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner 
 
-VERSION = "1.1.8"
+VERSION = "1.1.9"
 _API_URL = 'https://chiasmodon.com/v2/api/beta'
 _API_HEADERS = {'user-agent':'cli/python'}
 _VIEW_TYPE = {
     'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
     'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
     'subdomain':['domain'],
     'email':['domain', 'cidr', 'asn', 'app' ,'endpoint', 'phone', 'password'],
@@ -99,20 +99,31 @@
 
     def __request(self, data:dict,timeout=60):
 
         try:
             resp = requests.post(_API_URL, data=data, headers=_API_HEADERS, timeout=timeout)
             resp.close()
             resp = resp.json()
+
             try:
                 if resp.get('err'):
                     self.err = True 
                     self.msg = resp['msg']
             except:pass
+
             return resp
+
+        except requests.exceptions.ReadTimeout:
+            self.print(f"{T.RED}Error: timeout !\nPlease try agine later.{T.RESET}")
+            sys.exit()
+
+        except requests.exceptions.InvalidJSONError:
+            self.print(f"{T.RED}Error: Server send wrong data.\nPlease try agine later.{T.RESET}")
+            sys.exit()
+
         except Exception as e:
             self.print(f"{T.RED}Request error: {e}\nPlease try agine later.{T.RESET}")
             sys.exit()
 
 
     def __proc_query(self, 
                     method:str,
```

### Comparing `chiasmodon-1.1.8/setup.py` & `chiasmodon-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.1.8',
+      version='1.1.9',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

