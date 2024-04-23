# Comparing `tmp/mypy-boto3-workspaces-web-1.34.0.tar.gz` & `tmp/mypy_boto3_workspaces_web-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-workspaces-web-1.34.0.tar", last modified: Wed Dec 13 21:24:09 2023, max compression
+gzip compressed data, was "mypy_boto3_workspaces_web-1.34.90.tar", last modified: Tue Apr 23 19:34:22 2024, max compression
```

## Comparing `mypy-boto3-workspaces-web-1.34.0.tar` & `mypy_boto3_workspaces_web-1.34.90.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:09.287424 mypy-boto3-workspaces-web-1.34.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2023-12-13 21:24:09.287424 mypy-boto3-workspaces-web-1.34.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:09.287424 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38211 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38208 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8890 2023-12-13 21:21:29.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2023-12-13 21:21:29.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    36107 2023-12-13 21:21:30.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    36106 2023-12-13 21:21:29.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:24:09.287424 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12456 2023-12-13 21:24:09.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-13 21:24:09.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:09.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:24:09.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:24:09.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 21:24:09.000000 mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:24:09.287424 mypy-boto3-workspaces-web-1.34.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-12-13 21:21:26.000000 mypy-boto3-workspaces-web-1.34.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:22.280584 mypy_boto3_workspaces_web-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-04-23 19:34:22.280584 mypy_boto3_workspaces_web-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:22.280584 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38440 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38437 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-23 19:34:08.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    37029 2024-04-23 19:34:08.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37029 2024-04-23 19:34:08.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:22.280584 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-04-23 19:34:22.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-23 19:34:22.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:22.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:22.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:22.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 19:34:22.000000 mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:22.280584 mypy_boto3_workspaces_web-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-23 19:34:07.000000 mypy_boto3_workspaces_web-1.34.90/setup.py
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/LICENSE` & `mypy_boto3_workspaces_web-1.34.90/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/PKG-INFO` & `mypy_boto3_workspaces_web-1.34.90/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.34.0
-Summary: Type annotations for boto3.WorkSpacesWeb 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.90
+Summary: Type annotations for boto3.WorkSpacesWeb 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/README.md` & `mypy_boto3_workspaces_web-1.34.90/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/__main__.py` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WorkSpacesWeb 1.34.0\nVersion:         1.34.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
-        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web//\nBoto3 docs:     "
-        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\nOther"
-        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
-        " https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.WorkSpacesWeb 1.34.90\n"
+        "Version:         1.34.90\n"
+        "Builder version: 7.23.2\n"
+        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web//\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb\n"
+        "Other services:  https://pypi.org/project/boto3-stubs/\n"
+        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.0")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/client.py` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
+from .literals import (
+    AuthenticationTypeType,
+    EnabledTypeType,
+    IdentityProviderTypeType,
+    InstanceTypeType,
+)
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
@@ -187,15 +192,15 @@
     def create_browser_settings(
         self,
         *,
         browserPolicy: str,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBrowserSettingsResponseTypeDef:
         """
         Creates a browser settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_browser_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_browser_settings)
         """
@@ -203,15 +208,15 @@
     def create_identity_provider(
         self,
         *,
         identityProviderDetails: Mapping[str, str],
         identityProviderName: str,
         identityProviderType: IdentityProviderTypeType,
         portalArn: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an identity provider resource that is then associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_identity_provider)
         """
@@ -221,15 +226,15 @@
         *,
         ipRules: Sequence[IpRuleTypeDef],
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         description: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIpAccessSettingsResponseTypeDef:
         """
         Creates an IP access settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_ip_access_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_ip_access_settings)
         """
@@ -237,15 +242,15 @@
     def create_network_settings(
         self,
         *,
         securityGroupIds: Sequence[str],
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNetworkSettingsResponseTypeDef:
         """
         Creates a network settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_network_settings)
         """
@@ -254,29 +259,31 @@
         self,
         *,
         additionalEncryptionContext: Mapping[str, str] = ...,
         authenticationType: AuthenticationTypeType = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        instanceType: InstanceTypeType = ...,
+        maxConcurrentSessions: int = ...,
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePortalResponseTypeDef:
         """
         Creates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_portal)
         """
 
     def create_trust_store(
         self,
         *,
         certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_trust_store)
         """
@@ -303,15 +310,15 @@
         uploadAllowed: EnabledTypeType,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         customerManagedKey: str = ...,
         disconnectTimeoutInMinutes: int = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserSettingsResponseTypeDef:
         """
         Creates a user settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_user_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_user_settings)
         """
@@ -663,15 +670,15 @@
     def update_identity_provider(
         self,
         *,
         identityProviderArn: str,
         clientToken: str = ...,
         identityProviderDetails: Mapping[str, str] = ...,
         identityProviderName: str = ...,
-        identityProviderType: IdentityProviderTypeType = ...
+        identityProviderType: IdentityProviderTypeType = ...,
     ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_identity_provider)
         """
@@ -679,15 +686,15 @@
     def update_ip_access_settings(
         self,
         *,
         ipAccessSettingsArn: str,
         clientToken: str = ...,
         description: str = ...,
         displayName: str = ...,
-        ipRules: Sequence[IpRuleTypeDef] = ...
+        ipRules: Sequence[IpRuleTypeDef] = ...,
     ) -> UpdateIpAccessSettingsResponseTypeDef:
         """
         Updates IP access settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_ip_access_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_ip_access_settings)
         """
@@ -695,58 +702,60 @@
     def update_network_settings(
         self,
         *,
         networkSettingsArn: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
-        vpcId: str = ...
+        vpcId: str = ...,
     ) -> UpdateNetworkSettingsResponseTypeDef:
         """
         Updates network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_network_settings)
         """
 
     def update_portal(
         self,
         *,
         portalArn: str,
         authenticationType: AuthenticationTypeType = ...,
-        displayName: str = ...
+        displayName: str = ...,
+        instanceType: InstanceTypeType = ...,
+        maxConcurrentSessions: int = ...,
     ) -> UpdatePortalResponseTypeDef:
         """
         Updates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_portal)
         """
 
     def update_trust_store(
         self,
         *,
         trustStoreArn: str,
         certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_trust_store)
         """
 
     def update_user_access_logging_settings(
         self,
         *,
         userAccessLoggingSettingsArn: str,
         clientToken: str = ...,
-        kinesisStreamArn: str = ...
+        kinesisStreamArn: str = ...,
     ) -> UpdateUserAccessLoggingSettingsResponseTypeDef:
         """
         Updates the user access logging settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_access_logging_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_user_access_logging_settings)
         """
@@ -759,15 +768,15 @@
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         copyAllowed: EnabledTypeType = ...,
         disconnectTimeoutInMinutes: int = ...,
         downloadAllowed: EnabledTypeType = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
         pasteAllowed: EnabledTypeType = ...,
         printAllowed: EnabledTypeType = ...,
-        uploadAllowed: EnabledTypeType = ...
+        uploadAllowed: EnabledTypeType = ...,
     ) -> UpdateUserSettingsResponseTypeDef:
         """
         Updates the user settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_user_settings)
         """
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/client.pyi` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,20 @@
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import AuthenticationTypeType, EnabledTypeType, IdentityProviderTypeType
+from .literals import (
+    AuthenticationTypeType,
+    EnabledTypeType,
+    IdentityProviderTypeType,
+    InstanceTypeType,
+)
 from .type_defs import (
     AssociateBrowserSettingsResponseTypeDef,
     AssociateIpAccessSettingsResponseTypeDef,
     AssociateNetworkSettingsResponseTypeDef,
     AssociateTrustStoreResponseTypeDef,
     AssociateUserAccessLoggingSettingsResponseTypeDef,
     AssociateUserSettingsResponseTypeDef,
@@ -184,15 +189,15 @@
     def create_browser_settings(
         self,
         *,
         browserPolicy: str,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBrowserSettingsResponseTypeDef:
         """
         Creates a browser settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_browser_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_browser_settings)
         """
@@ -200,15 +205,15 @@
     def create_identity_provider(
         self,
         *,
         identityProviderDetails: Mapping[str, str],
         identityProviderName: str,
         identityProviderType: IdentityProviderTypeType,
         portalArn: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateIdentityProviderResponseTypeDef:
         """
         Creates an identity provider resource that is then associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_identity_provider)
         """
@@ -218,15 +223,15 @@
         *,
         ipRules: Sequence[IpRuleTypeDef],
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         description: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateIpAccessSettingsResponseTypeDef:
         """
         Creates an IP access settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_ip_access_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_ip_access_settings)
         """
@@ -234,15 +239,15 @@
     def create_network_settings(
         self,
         *,
         securityGroupIds: Sequence[str],
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateNetworkSettingsResponseTypeDef:
         """
         Creates a network settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_network_settings)
         """
@@ -251,29 +256,31 @@
         self,
         *,
         additionalEncryptionContext: Mapping[str, str] = ...,
         authenticationType: AuthenticationTypeType = ...,
         clientToken: str = ...,
         customerManagedKey: str = ...,
         displayName: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        instanceType: InstanceTypeType = ...,
+        maxConcurrentSessions: int = ...,
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePortalResponseTypeDef:
         """
         Creates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_portal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_portal)
         """
 
     def create_trust_store(
         self,
         *,
         certificateList: Sequence[BlobTypeDef],
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrustStoreResponseTypeDef:
         """
         Creates a trust store that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_trust_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_trust_store)
         """
@@ -300,15 +307,15 @@
         uploadAllowed: EnabledTypeType,
         additionalEncryptionContext: Mapping[str, str] = ...,
         clientToken: str = ...,
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         customerManagedKey: str = ...,
         disconnectTimeoutInMinutes: int = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserSettingsResponseTypeDef:
         """
         Creates a user settings resource that can be associated with a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.create_user_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#create_user_settings)
         """
@@ -660,15 +667,15 @@
     def update_identity_provider(
         self,
         *,
         identityProviderArn: str,
         clientToken: str = ...,
         identityProviderDetails: Mapping[str, str] = ...,
         identityProviderName: str = ...,
-        identityProviderType: IdentityProviderTypeType = ...
+        identityProviderType: IdentityProviderTypeType = ...,
     ) -> UpdateIdentityProviderResponseTypeDef:
         """
         Updates the identity provider.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_identity_provider)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_identity_provider)
         """
@@ -676,15 +683,15 @@
     def update_ip_access_settings(
         self,
         *,
         ipAccessSettingsArn: str,
         clientToken: str = ...,
         description: str = ...,
         displayName: str = ...,
-        ipRules: Sequence[IpRuleTypeDef] = ...
+        ipRules: Sequence[IpRuleTypeDef] = ...,
     ) -> UpdateIpAccessSettingsResponseTypeDef:
         """
         Updates IP access settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_ip_access_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_ip_access_settings)
         """
@@ -692,58 +699,60 @@
     def update_network_settings(
         self,
         *,
         networkSettingsArn: str,
         clientToken: str = ...,
         securityGroupIds: Sequence[str] = ...,
         subnetIds: Sequence[str] = ...,
-        vpcId: str = ...
+        vpcId: str = ...,
     ) -> UpdateNetworkSettingsResponseTypeDef:
         """
         Updates network settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_network_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_network_settings)
         """
 
     def update_portal(
         self,
         *,
         portalArn: str,
         authenticationType: AuthenticationTypeType = ...,
-        displayName: str = ...
+        displayName: str = ...,
+        instanceType: InstanceTypeType = ...,
+        maxConcurrentSessions: int = ...,
     ) -> UpdatePortalResponseTypeDef:
         """
         Updates a web portal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_portal)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_portal)
         """
 
     def update_trust_store(
         self,
         *,
         trustStoreArn: str,
         certificatesToAdd: Sequence[BlobTypeDef] = ...,
         certificatesToDelete: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateTrustStoreResponseTypeDef:
         """
         Updates the trust store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_trust_store)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_trust_store)
         """
 
     def update_user_access_logging_settings(
         self,
         *,
         userAccessLoggingSettingsArn: str,
         clientToken: str = ...,
-        kinesisStreamArn: str = ...
+        kinesisStreamArn: str = ...,
     ) -> UpdateUserAccessLoggingSettingsResponseTypeDef:
         """
         Updates the user access logging settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_access_logging_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_user_access_logging_settings)
         """
@@ -756,15 +765,15 @@
         cookieSynchronizationConfiguration: CookieSynchronizationConfigurationTypeDef = ...,
         copyAllowed: EnabledTypeType = ...,
         disconnectTimeoutInMinutes: int = ...,
         downloadAllowed: EnabledTypeType = ...,
         idleDisconnectTimeoutInMinutes: int = ...,
         pasteAllowed: EnabledTypeType = ...,
         printAllowed: EnabledTypeType = ...,
-        uploadAllowed: EnabledTypeType = ...
+        uploadAllowed: EnabledTypeType = ...,
     ) -> UpdateUserSettingsResponseTypeDef:
         """
         Updates the user settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Client.update_user_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/client/#update_user_settings)
         """
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/literals.py` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AuthenticationTypeType",
     "BrowserTypeType",
     "EnabledTypeType",
     "IdentityProviderTypeType",
+    "InstanceTypeType",
     "PortalStatusType",
     "RendererTypeType",
     "WorkSpacesWebServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AuthenticationTypeType = Literal["IAM_Identity_Center", "Standard"]
 BrowserTypeType = Literal["Chrome"]
 EnabledTypeType = Literal["Disabled", "Enabled"]
 IdentityProviderTypeType = Literal[
     "Facebook", "Google", "LoginWithAmazon", "OIDC", "SAML", "SignInWithApple"
 ]
+InstanceTypeType = Literal["standard.large", "standard.regular", "standard.xlarge"]
 PortalStatusType = Literal["Active", "Incomplete", "Pending"]
 RendererTypeType = Literal["AppStream"]
 WorkSpacesWebServiceName = Literal["workspaces-web"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -65,14 +65,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -83,14 +84,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -108,14 +110,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -128,24 +131,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -206,15 +211,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -286,17 +290,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -341,14 +347,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -386,19 +393,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/literals.pyi` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -20,28 +20,30 @@
     from typing_extensions import Literal
 
 __all__ = (
     "AuthenticationTypeType",
     "BrowserTypeType",
     "EnabledTypeType",
     "IdentityProviderTypeType",
+    "InstanceTypeType",
     "PortalStatusType",
     "RendererTypeType",
     "WorkSpacesWebServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 AuthenticationTypeType = Literal["IAM_Identity_Center", "Standard"]
 BrowserTypeType = Literal["Chrome"]
 EnabledTypeType = Literal["Disabled", "Enabled"]
 IdentityProviderTypeType = Literal[
     "Facebook", "Google", "LoginWithAmazon", "OIDC", "SAML", "SignInWithApple"
 ]
+InstanceTypeType = Literal["standard.large", "standard.regular", "standard.xlarge"]
 PortalStatusType = Literal["Active", "Incomplete", "Pending"]
 RendererTypeType = Literal["AppStream"]
 WorkSpacesWebServiceName = Literal["workspaces-web"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -63,14 +65,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -81,14 +84,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -106,14 +110,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -126,24 +131,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -204,15 +211,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -284,17 +290,19 @@
     "migrationhuborchestrator",
     "migrationhubstrategy",
     "mobile",
     "mq",
     "mturk",
     "mwaa",
     "neptune",
+    "neptune-graph",
     "neptunedata",
     "network-firewall",
     "networkmanager",
+    "networkmonitor",
     "nimble",
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
@@ -339,14 +347,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -384,19 +393,21 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
+    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/type_defs.py` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AuthenticationTypeType,
     EnabledTypeType,
     IdentityProviderTypeType,
+    InstanceTypeType,
     PortalStatusType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -34,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateBrowserSettingsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     "AssociateNetworkSettingsRequestRequestTypeDef",
     "AssociateTrustStoreRequestRequestTypeDef",
     "AssociateUserAccessLoggingSettingsRequestRequestTypeDef",
@@ -173,18 +173,18 @@
         "portalArn": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
         "portalArn": str,
@@ -225,16 +225,18 @@
         "browserSettingsArn": str,
     },
 )
 BrowserSettingsTypeDef = TypedDict(
     "BrowserSettingsTypeDef",
     {
         "browserSettingsArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "associatedPortalArns": NotRequired[List[str]],
         "browserPolicy": NotRequired[str],
+        "customerManagedKey": NotRequired[str],
     },
 )
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "issuer": NotRequired[str],
         "notValidAfter": NotRequired[datetime],
@@ -419,20 +421,24 @@
         "portalArn": str,
     },
 )
 PortalTypeDef = TypedDict(
     "PortalTypeDef",
     {
         "portalArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "authenticationType": NotRequired[AuthenticationTypeType],
         "browserSettingsArn": NotRequired[str],
         "browserType": NotRequired[Literal["Chrome"]],
         "creationDate": NotRequired[datetime],
+        "customerManagedKey": NotRequired[str],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
         "ipAccessSettingsArn": NotRequired[str],
+        "maxConcurrentSessions": NotRequired[int],
         "networkSettingsArn": NotRequired[str],
         "portalEndpoint": NotRequired[str],
         "portalStatus": NotRequired[PortalStatusType],
         "rendererType": NotRequired[Literal["AppStream"]],
         "statusReason": NotRequired[str],
         "trustStoreArn": NotRequired[str],
         "userAccessLoggingSettingsArn": NotRequired[str],
@@ -550,15 +556,17 @@
     {
         "portalArn": str,
         "authenticationType": NotRequired[AuthenticationTypeType],
         "browserSettingsArn": NotRequired[str],
         "browserType": NotRequired[Literal["Chrome"]],
         "creationDate": NotRequired[datetime],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
         "ipAccessSettingsArn": NotRequired[str],
+        "maxConcurrentSessions": NotRequired[int],
         "networkSettingsArn": NotRequired[str],
         "portalEndpoint": NotRequired[str],
         "portalStatus": NotRequired[PortalStatusType],
         "rendererType": NotRequired[Literal["AppStream"]],
         "trustStoreArn": NotRequired[str],
         "userAccessLoggingSettingsArn": NotRequired[str],
         "userSettingsArn": NotRequired[str],
@@ -649,14 +657,16 @@
 )
 UpdatePortalRequestRequestTypeDef = TypedDict(
     "UpdatePortalRequestRequestTypeDef",
     {
         "portalArn": str,
         "authenticationType": NotRequired[AuthenticationTypeType],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
+        "maxConcurrentSessions": NotRequired[int],
     },
 )
 UpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
         "clientToken": NotRequired[str],
@@ -862,14 +872,16 @@
     "CreatePortalRequestRequestTypeDef",
     {
         "additionalEncryptionContext": NotRequired[Mapping[str, str]],
         "authenticationType": NotRequired[AuthenticationTypeType],
         "clientToken": NotRequired[str],
         "customerManagedKey": NotRequired[str],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
+        "maxConcurrentSessions": NotRequired[int],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateTrustStoreRequestRequestTypeDef = TypedDict(
     "CreateTrustStoreRequestRequestTypeDef",
     {
         "certificateList": Sequence[BlobTypeDef],
@@ -912,16 +924,18 @@
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 IpAccessSettingsTypeDef = TypedDict(
     "IpAccessSettingsTypeDef",
     {
         "ipAccessSettingsArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "associatedPortalArns": NotRequired[List[str]],
         "creationDate": NotRequired[datetime],
+        "customerManagedKey": NotRequired[str],
         "description": NotRequired[str],
         "displayName": NotRequired[str],
         "ipRules": NotRequired[List[IpRuleTypeDef]],
     },
 )
 UpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "UpdateIpAccessSettingsRequestRequestTypeDef",
@@ -1096,19 +1110,21 @@
         "uploadAllowed": NotRequired[EnabledTypeType],
     },
 )
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "userSettingsArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "associatedPortalArns": NotRequired[List[str]],
         "cookieSynchronizationConfiguration": NotRequired[
             CookieSynchronizationConfigurationTypeDef
         ],
         "copyAllowed": NotRequired[EnabledTypeType],
+        "customerManagedKey": NotRequired[str],
         "disconnectTimeoutInMinutes": NotRequired[int],
         "downloadAllowed": NotRequired[EnabledTypeType],
         "idleDisconnectTimeoutInMinutes": NotRequired[int],
         "pasteAllowed": NotRequired[EnabledTypeType],
         "printAllowed": NotRequired[EnabledTypeType],
         "uploadAllowed": NotRequired[EnabledTypeType],
     },
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web/type_defs.pyi` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AuthenticationTypeType,
     EnabledTypeType,
     IdentityProviderTypeType,
+    InstanceTypeType,
     PortalStatusType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -172,18 +173,18 @@
         "portalArn": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 AssociateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "AssociateIpAccessSettingsRequestRequestTypeDef",
     {
         "ipAccessSettingsArn": str,
         "portalArn": str,
@@ -224,16 +225,18 @@
         "browserSettingsArn": str,
     },
 )
 BrowserSettingsTypeDef = TypedDict(
     "BrowserSettingsTypeDef",
     {
         "browserSettingsArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "associatedPortalArns": NotRequired[List[str]],
         "browserPolicy": NotRequired[str],
+        "customerManagedKey": NotRequired[str],
     },
 )
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "issuer": NotRequired[str],
         "notValidAfter": NotRequired[datetime],
@@ -418,20 +421,24 @@
         "portalArn": str,
     },
 )
 PortalTypeDef = TypedDict(
     "PortalTypeDef",
     {
         "portalArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "authenticationType": NotRequired[AuthenticationTypeType],
         "browserSettingsArn": NotRequired[str],
         "browserType": NotRequired[Literal["Chrome"]],
         "creationDate": NotRequired[datetime],
+        "customerManagedKey": NotRequired[str],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
         "ipAccessSettingsArn": NotRequired[str],
+        "maxConcurrentSessions": NotRequired[int],
         "networkSettingsArn": NotRequired[str],
         "portalEndpoint": NotRequired[str],
         "portalStatus": NotRequired[PortalStatusType],
         "rendererType": NotRequired[Literal["AppStream"]],
         "statusReason": NotRequired[str],
         "trustStoreArn": NotRequired[str],
         "userAccessLoggingSettingsArn": NotRequired[str],
@@ -549,15 +556,17 @@
     {
         "portalArn": str,
         "authenticationType": NotRequired[AuthenticationTypeType],
         "browserSettingsArn": NotRequired[str],
         "browserType": NotRequired[Literal["Chrome"]],
         "creationDate": NotRequired[datetime],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
         "ipAccessSettingsArn": NotRequired[str],
+        "maxConcurrentSessions": NotRequired[int],
         "networkSettingsArn": NotRequired[str],
         "portalEndpoint": NotRequired[str],
         "portalStatus": NotRequired[PortalStatusType],
         "rendererType": NotRequired[Literal["AppStream"]],
         "trustStoreArn": NotRequired[str],
         "userAccessLoggingSettingsArn": NotRequired[str],
         "userSettingsArn": NotRequired[str],
@@ -648,14 +657,16 @@
 )
 UpdatePortalRequestRequestTypeDef = TypedDict(
     "UpdatePortalRequestRequestTypeDef",
     {
         "portalArn": str,
         "authenticationType": NotRequired[AuthenticationTypeType],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
+        "maxConcurrentSessions": NotRequired[int],
     },
 )
 UpdateUserAccessLoggingSettingsRequestRequestTypeDef = TypedDict(
     "UpdateUserAccessLoggingSettingsRequestRequestTypeDef",
     {
         "userAccessLoggingSettingsArn": str,
         "clientToken": NotRequired[str],
@@ -861,14 +872,16 @@
     "CreatePortalRequestRequestTypeDef",
     {
         "additionalEncryptionContext": NotRequired[Mapping[str, str]],
         "authenticationType": NotRequired[AuthenticationTypeType],
         "clientToken": NotRequired[str],
         "customerManagedKey": NotRequired[str],
         "displayName": NotRequired[str],
+        "instanceType": NotRequired[InstanceTypeType],
+        "maxConcurrentSessions": NotRequired[int],
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 CreateTrustStoreRequestRequestTypeDef = TypedDict(
     "CreateTrustStoreRequestRequestTypeDef",
     {
         "certificateList": Sequence[BlobTypeDef],
@@ -911,16 +924,18 @@
         "tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 IpAccessSettingsTypeDef = TypedDict(
     "IpAccessSettingsTypeDef",
     {
         "ipAccessSettingsArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "associatedPortalArns": NotRequired[List[str]],
         "creationDate": NotRequired[datetime],
+        "customerManagedKey": NotRequired[str],
         "description": NotRequired[str],
         "displayName": NotRequired[str],
         "ipRules": NotRequired[List[IpRuleTypeDef]],
     },
 )
 UpdateIpAccessSettingsRequestRequestTypeDef = TypedDict(
     "UpdateIpAccessSettingsRequestRequestTypeDef",
@@ -1095,19 +1110,21 @@
         "uploadAllowed": NotRequired[EnabledTypeType],
     },
 )
 UserSettingsTypeDef = TypedDict(
     "UserSettingsTypeDef",
     {
         "userSettingsArn": str,
+        "additionalEncryptionContext": NotRequired[Dict[str, str]],
         "associatedPortalArns": NotRequired[List[str]],
         "cookieSynchronizationConfiguration": NotRequired[
             CookieSynchronizationConfigurationTypeDef
         ],
         "copyAllowed": NotRequired[EnabledTypeType],
+        "customerManagedKey": NotRequired[str],
         "disconnectTimeoutInMinutes": NotRequired[int],
         "downloadAllowed": NotRequired[EnabledTypeType],
         "idleDisconnectTimeoutInMinutes": NotRequired[int],
         "pasteAllowed": NotRequired[EnabledTypeType],
         "printAllowed": NotRequired[EnabledTypeType],
         "uploadAllowed": NotRequired[EnabledTypeType],
     },
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/PKG-INFO` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-workspaces-web
-Version: 1.34.0
-Summary: Type annotations for boto3.WorkSpacesWeb 1.34.0 service generated with mypy-boto3-builder 7.21.0
+Version: 1.34.90
+Summary: Type annotations for boto3.WorkSpacesWeb 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="mypy-boto3-workspaces-web"></a>
 
 # mypy-boto3-workspaces-web
 
 [![PyPI - mypy-boto3-workspaces-web](https://img.shields.io/pypi/v/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-workspaces-web.svg?color=blue)](https://pypi.org/project/mypy-boto3-workspaces-web)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-workspaces-web)](https://pepy.tech/project/mypy-boto3-workspaces-web)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WorkSpacesWeb 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
+[boto3.WorkSpacesWeb 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-workspaces-web docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-workspaces-web-1.34.0/mypy_boto3_workspaces_web.egg-info/SOURCES.txt` & `mypy_boto3_workspaces_web-1.34.90/mypy_boto3_workspaces_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-workspaces-web-1.34.0/setup.py` & `mypy_boto3_workspaces_web-1.34.90/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-workspaces-web",
-    version="1.34.0",
+    version="1.34.90",
     packages=["mypy_boto3_workspaces_web"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description=(
-        "Type annotations for boto3.WorkSpacesWeb 1.34.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
-    ),
+    description="Type annotations for boto3.WorkSpacesWeb 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="boto3 workspaces-web type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"mypy_boto3_workspaces_web": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_workspaces_web/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

