# Comparing `tmp/mypy_boto3_bedrock_agent-1.34.89.tar.gz` & `tmp/mypy_boto3_bedrock_agent-1.34.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_bedrock_agent-1.34.89.tar", last modified: Mon Apr 22 19:19:11 2024, max compression
+gzip compressed data, was "mypy_boto3_bedrock_agent-1.34.90.tar", last modified: Tue Apr 23 19:34:19 2024, max compression
```

## Comparing `mypy_boto3_bedrock_agent-1.34.89.tar` & `mypy_boto3_bedrock_agent-1.34.90.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:11.631683 mypy_boto3_bedrock_agent-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-22 19:19:11.631683 mypy_boto3_bedrock_agent-1.34.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:11.631683 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34255 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34252 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42036 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42036 2024-04-22 19:18:32.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:11.631683 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 19:19:11.000000 mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:19:11.631683 mypy_boto3_bedrock_agent-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-22 19:18:31.000000 mypy_boto3_bedrock_agent-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.312555 mypy_boto3_bedrock_agent-1.34.90/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-23 19:34:19.312555 mypy_boto3_bedrock_agent-1.34.90/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12503 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.308555 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34395 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34392 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11585 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9988 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42365 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42365 2024-04-23 19:33:10.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:34:19.308555 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14085 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 19:34:19.000000 mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:34:19.312555 mypy_boto3_bedrock_agent-1.34.90/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 19:33:09.000000 mypy_boto3_bedrock_agent-1.34.90/setup.py
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/LICENSE` & `mypy_boto3_bedrock_agent-1.34.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.89/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.89
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/README.md` & `mypy_boto3_bedrock_agent-1.34.90/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/__init__.py` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/__init__.pyi` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/__main__.py` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AgentsforBedrock 1.34.89\n"
-        "Version:         1.34.89\n"
+        "Type annotations for boto3.AgentsforBedrock 1.34.90\n"
+        "Version:         1.34.90\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.89")
+    print("1.34.90")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/client.py` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ActionGroupStateType, KnowledgeBaseStateType
+from .literals import ActionGroupStateType, DataDeletionPolicyType, KnowledgeBaseStateType
 from .paginator import (
     ListAgentActionGroupsPaginator,
     ListAgentAliasesPaginator,
     ListAgentKnowledgeBasesPaginator,
     ListAgentsPaginator,
     ListAgentVersionsPaginator,
     ListDataSourcesPaginator,
@@ -222,14 +222,15 @@
     def create_data_source(
         self,
         *,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         knowledgeBaseId: str,
         name: str,
         clientToken: str = ...,
+        dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Sets up a data source to be added to a knowledge base.
 
@@ -631,14 +632,15 @@
     def update_data_source(
         self,
         *,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         dataSourceId: str,
         knowledgeBaseId: str,
         name: str,
+        dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates configurations for a data source.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/client.pyi` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
-from .literals import ActionGroupStateType, KnowledgeBaseStateType
+from .literals import ActionGroupStateType, DataDeletionPolicyType, KnowledgeBaseStateType
 from .paginator import (
     ListAgentActionGroupsPaginator,
     ListAgentAliasesPaginator,
     ListAgentKnowledgeBasesPaginator,
     ListAgentsPaginator,
     ListAgentVersionsPaginator,
     ListDataSourcesPaginator,
@@ -219,14 +219,15 @@
     def create_data_source(
         self,
         *,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         knowledgeBaseId: str,
         name: str,
         clientToken: str = ...,
+        dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Sets up a data source to be added to a knowledge base.
 
@@ -628,14 +629,15 @@
     def update_data_source(
         self,
         *,
         dataSourceConfiguration: DataSourceConfigurationTypeDef,
         dataSourceId: str,
         knowledgeBaseId: str,
         name: str,
+        dataDeletionPolicy: DataDeletionPolicyType = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates configurations for a data source.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/literals.py` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "ActionGroupSignatureType",
     "ActionGroupStateType",
     "AgentAliasStatusType",
     "AgentStatusType",
     "ChunkingStrategyType",
     "CreationModeType",
     "CustomControlMethodType",
+    "DataDeletionPolicyType",
     "DataSourceStatusType",
     "DataSourceTypeType",
     "IngestionJobFilterAttributeType",
     "IngestionJobFilterOperatorType",
     "IngestionJobSortByAttributeType",
     "IngestionJobStatusType",
     "KnowledgeBaseStateType",
@@ -67,22 +68,25 @@
     "PREPARING",
     "UPDATING",
     "VERSIONING",
 ]
 ChunkingStrategyType = Literal["FIXED_SIZE", "NONE"]
 CreationModeType = Literal["DEFAULT", "OVERRIDDEN"]
 CustomControlMethodType = Literal["RETURN_CONTROL"]
-DataSourceStatusType = Literal["AVAILABLE", "DELETING"]
+DataDeletionPolicyType = Literal["DELETE", "RETAIN"]
+DataSourceStatusType = Literal["AVAILABLE", "DELETE_UNSUCCESSFUL", "DELETING"]
 DataSourceTypeType = Literal["S3"]
 IngestionJobFilterAttributeType = Literal["STATUS"]
 IngestionJobFilterOperatorType = Literal["EQ"]
 IngestionJobSortByAttributeType = Literal["STARTED_AT", "STATUS"]
 IngestionJobStatusType = Literal["COMPLETE", "FAILED", "IN_PROGRESS", "STARTING"]
 KnowledgeBaseStateType = Literal["DISABLED", "ENABLED"]
-KnowledgeBaseStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
+KnowledgeBaseStatusType = Literal[
+    "ACTIVE", "CREATING", "DELETE_UNSUCCESSFUL", "DELETING", "FAILED", "UPDATING"
+]
 KnowledgeBaseStorageTypeType = Literal[
     "OPENSEARCH_SERVERLESS", "PINECONE", "RDS", "REDIS_ENTERPRISE_CLOUD"
 ]
 KnowledgeBaseTypeType = Literal["VECTOR"]
 ListAgentActionGroupsPaginatorName = Literal["list_agent_action_groups"]
 ListAgentAliasesPaginatorName = Literal["list_agent_aliases"]
 ListAgentKnowledgeBasesPaginatorName = Literal["list_agent_knowledge_bases"]
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/literals.pyi` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "ActionGroupSignatureType",
     "ActionGroupStateType",
     "AgentAliasStatusType",
     "AgentStatusType",
     "ChunkingStrategyType",
     "CreationModeType",
     "CustomControlMethodType",
+    "DataDeletionPolicyType",
     "DataSourceStatusType",
     "DataSourceTypeType",
     "IngestionJobFilterAttributeType",
     "IngestionJobFilterOperatorType",
     "IngestionJobSortByAttributeType",
     "IngestionJobStatusType",
     "KnowledgeBaseStateType",
@@ -67,22 +68,25 @@
     "PREPARING",
     "UPDATING",
     "VERSIONING",
 ]
 ChunkingStrategyType = Literal["FIXED_SIZE", "NONE"]
 CreationModeType = Literal["DEFAULT", "OVERRIDDEN"]
 CustomControlMethodType = Literal["RETURN_CONTROL"]
-DataSourceStatusType = Literal["AVAILABLE", "DELETING"]
+DataDeletionPolicyType = Literal["DELETE", "RETAIN"]
+DataSourceStatusType = Literal["AVAILABLE", "DELETE_UNSUCCESSFUL", "DELETING"]
 DataSourceTypeType = Literal["S3"]
 IngestionJobFilterAttributeType = Literal["STATUS"]
 IngestionJobFilterOperatorType = Literal["EQ"]
 IngestionJobSortByAttributeType = Literal["STARTED_AT", "STATUS"]
 IngestionJobStatusType = Literal["COMPLETE", "FAILED", "IN_PROGRESS", "STARTING"]
 KnowledgeBaseStateType = Literal["DISABLED", "ENABLED"]
-KnowledgeBaseStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED", "UPDATING"]
+KnowledgeBaseStatusType = Literal[
+    "ACTIVE", "CREATING", "DELETE_UNSUCCESSFUL", "DELETING", "FAILED", "UPDATING"
+]
 KnowledgeBaseStorageTypeType = Literal[
     "OPENSEARCH_SERVERLESS", "PINECONE", "RDS", "REDIS_ENTERPRISE_CLOUD"
 ]
 KnowledgeBaseTypeType = Literal["VECTOR"]
 ListAgentActionGroupsPaginatorName = Literal["list_agent_action_groups"]
 ListAgentAliasesPaginatorName = Literal["list_agent_aliases"]
 ListAgentKnowledgeBasesPaginatorName = Literal["list_agent_knowledge_bases"]
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/paginator.py` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/paginator.pyi` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/type_defs.py` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .literals import (
     ActionGroupStateType,
     AgentAliasStatusType,
     AgentStatusType,
     ChunkingStrategyType,
     CreationModeType,
+    DataDeletionPolicyType,
     DataSourceStatusType,
     IngestionJobSortByAttributeType,
     IngestionJobStatusType,
     KnowledgeBaseStateType,
     KnowledgeBaseStatusType,
     KnowledgeBaseStorageTypeType,
     PromptStateType,
@@ -289,14 +290,15 @@
         "kmsKeyArn": NotRequired[str],
     },
 )
 S3DataSourceConfigurationTypeDef = TypedDict(
     "S3DataSourceConfigurationTypeDef",
     {
         "bucketArn": str,
+        "bucketOwnerAccountId": NotRequired[str],
         "inclusionPrefixes": NotRequired[Sequence[str]],
     },
 )
 DataSourceSummaryTypeDef = TypedDict(
     "DataSourceSummaryTypeDef",
     {
         "dataSourceId": str,
@@ -1071,14 +1073,15 @@
 CreateDataSourceRequestRequestTypeDef = TypedDict(
     "CreateDataSourceRequestRequestTypeDef",
     {
         "dataSourceConfiguration": DataSourceConfigurationTypeDef,
         "knowledgeBaseId": str,
         "name": str,
         "clientToken": NotRequired[str],
+        "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
         "serverSideEncryptionConfiguration": NotRequired[ServerSideEncryptionConfigurationTypeDef],
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
@@ -1086,26 +1089,29 @@
         "createdAt": datetime,
         "dataSourceConfiguration": DataSourceConfigurationTypeDef,
         "dataSourceId": str,
         "knowledgeBaseId": str,
         "name": str,
         "status": DataSourceStatusType,
         "updatedAt": datetime,
+        "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
+        "failureReasons": NotRequired[List[str]],
         "serverSideEncryptionConfiguration": NotRequired[ServerSideEncryptionConfigurationTypeDef],
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 UpdateDataSourceRequestRequestTypeDef = TypedDict(
     "UpdateDataSourceRequestRequestTypeDef",
     {
         "dataSourceConfiguration": DataSourceConfigurationTypeDef,
         "dataSourceId": str,
         "knowledgeBaseId": str,
         "name": str,
+        "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
         "serverSideEncryptionConfiguration": NotRequired[ServerSideEncryptionConfigurationTypeDef],
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 AgentActionGroupTypeDef = TypedDict(
     "AgentActionGroupTypeDef",
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent/type_defs.pyi` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .literals import (
     ActionGroupStateType,
     AgentAliasStatusType,
     AgentStatusType,
     ChunkingStrategyType,
     CreationModeType,
+    DataDeletionPolicyType,
     DataSourceStatusType,
     IngestionJobSortByAttributeType,
     IngestionJobStatusType,
     KnowledgeBaseStateType,
     KnowledgeBaseStatusType,
     KnowledgeBaseStorageTypeType,
     PromptStateType,
@@ -289,14 +290,15 @@
         "kmsKeyArn": NotRequired[str],
     },
 )
 S3DataSourceConfigurationTypeDef = TypedDict(
     "S3DataSourceConfigurationTypeDef",
     {
         "bucketArn": str,
+        "bucketOwnerAccountId": NotRequired[str],
         "inclusionPrefixes": NotRequired[Sequence[str]],
     },
 )
 DataSourceSummaryTypeDef = TypedDict(
     "DataSourceSummaryTypeDef",
     {
         "dataSourceId": str,
@@ -1071,14 +1073,15 @@
 CreateDataSourceRequestRequestTypeDef = TypedDict(
     "CreateDataSourceRequestRequestTypeDef",
     {
         "dataSourceConfiguration": DataSourceConfigurationTypeDef,
         "knowledgeBaseId": str,
         "name": str,
         "clientToken": NotRequired[str],
+        "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
         "serverSideEncryptionConfiguration": NotRequired[ServerSideEncryptionConfigurationTypeDef],
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
@@ -1086,26 +1089,29 @@
         "createdAt": datetime,
         "dataSourceConfiguration": DataSourceConfigurationTypeDef,
         "dataSourceId": str,
         "knowledgeBaseId": str,
         "name": str,
         "status": DataSourceStatusType,
         "updatedAt": datetime,
+        "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
+        "failureReasons": NotRequired[List[str]],
         "serverSideEncryptionConfiguration": NotRequired[ServerSideEncryptionConfigurationTypeDef],
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 UpdateDataSourceRequestRequestTypeDef = TypedDict(
     "UpdateDataSourceRequestRequestTypeDef",
     {
         "dataSourceConfiguration": DataSourceConfigurationTypeDef,
         "dataSourceId": str,
         "knowledgeBaseId": str,
         "name": str,
+        "dataDeletionPolicy": NotRequired[DataDeletionPolicyType],
         "description": NotRequired[str],
         "serverSideEncryptionConfiguration": NotRequired[ServerSideEncryptionConfigurationTypeDef],
         "vectorIngestionConfiguration": NotRequired[VectorIngestionConfigurationTypeDef],
     },
 )
 AgentActionGroupTypeDef = TypedDict(
     "AgentActionGroupTypeDef",
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/PKG-INFO` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-bedrock-agent
-Version: 1.34.89
-Summary: Type annotations for boto3.AgentsforBedrock 1.34.89 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.90
+Summary: Type annotations for boto3.AgentsforBedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-bedrock-agent.svg?color=blue)](https://pypi.org/project/mypy-boto3-bedrock-agent)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_bedrock_agent/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-bedrock-agent)](https://pepy.tech/project/mypy-boto3-bedrock-agent)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AgentsforBedrock 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
+[boto3.AgentsforBedrock 1.34.90](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_bedrock_agent-1.34.89/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt` & `mypy_boto3_bedrock_agent-1.34.90/mypy_boto3_bedrock_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_bedrock_agent-1.34.89/setup.py` & `mypy_boto3_bedrock_agent-1.34.90/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-bedrock-agent",
-    version="1.34.89",
+    version="1.34.90",
     packages=["mypy_boto3_bedrock_agent"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.AgentsforBedrock 1.34.89 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.AgentsforBedrock 1.34.90 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

