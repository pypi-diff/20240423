# Comparing `tmp/q_alchemy_sdk_py-0.2.5.tar.gz` & `tmp/q_alchemy_sdk_py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q_alchemy_sdk_py-0.2.5.tar", last modified: Fri Apr 19 14:09:07 2024, max compression
+gzip compressed data, was "q_alchemy_sdk_py-0.2.6.tar", last modified: Tue Apr 23 18:44:12 2024, max compression
```

## Comparing `q_alchemy_sdk_py-0.2.5.tar` & `q_alchemy_sdk_py-0.2.6.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0    11556 2024-03-19 19:59:43.321774 q_alchemy_sdk_py-0.2.5/LICENSE
--rw-r--r--   0        0        0     3132 2024-04-19 13:35:07.213197 q_alchemy_sdk_py-0.2.5/README.md
--rw-r--r--   0        0        0      684 2024-04-19 14:09:06.994537 q_alchemy_sdk_py-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      599 2024-04-19 13:35:07.228950 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/__init__.py
--rw-r--r--   0        0        0      844 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/__init__.py
--rw-r--r--   0        0        0      771 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/base_relations.py
--rw-r--r--   0        0        0     1237 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/enterapi.py
--rw-r--r--   0        0        0      645 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/exceptions.py
--rw-r--r--   0        0        0      599 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/__init__.py
--rw-r--r--   0        0        0     2955 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/action_hco.py
--rw-r--r--   0        0        0     3906 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/action_with_parameters_hco.py
--rw-r--r--   0        0        0     2002 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/download_link_hco.py
--rw-r--r--   0        0        0     4062 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/hco_base.py
--rw-r--r--   0        0        0     2573 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/link_hco.py
--rw-r--r--   0        0        0     5287 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/upload_action_hco.py
--rw-r--r--   0        0        0      793 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/http_headers.py
--rw-r--r--   0        0        0     1225 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/media_types.py
--rw-r--r--   0        0        0      599 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/model/__init__.py
--rw-r--r--   0        0        0      825 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/model/error.py
--rw-r--r--   0        0        0     6303 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/model/sirenmodels.py
--rw-r--r--   0        0        0     1715 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/polling.py
--rw-r--r--   0        0        0     7752 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/sirenaccess.py
--rw-r--r--   0        0        0      745 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/__init__.py
--rw-r--r--   0        0        0     2118 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/enterjma.py
--rw-r--r--   0        0        0     1009 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/__init__.py
--rw-r--r--   0        0        0     3006 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/entrypoint_hco.py
--rw-r--r--   0        0        0     1991 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/info_hco.py
--rw-r--r--   0        0        0     3704 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py
--rw-r--r--   0        0        0     8200 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/job_hco.py
--rw-r--r--   0        0        0     3678 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/job_query_result_hco.py
--rw-r--r--   0        0        0     1591 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py
--rw-r--r--   0        0        0     4361 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/jobsroot_hco.py
--rw-r--r--   0        0        0     2149 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py
--rw-r--r--   0        0        0     3727 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processing_step_hco.py
--rw-r--r--   0        0        0     1714 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py
--rw-r--r--   0        0        0     3937 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py
--rw-r--r--   0        0        0     4471 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py
--rw-r--r--   0        0        0     1749 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/user_hco.py
--rw-r--r--   0        0        0     5694 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdata_hco.py
--rw-r--r--   0        0        0     3616 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py
--rw-r--r--   0        0        0     1734 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py
--rw-r--r--   0        0        0     4772 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdataroot_hco.py
--rw-r--r--   0        0        0     1223 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/known_relations.py
--rw-r--r--   0        0        0      636 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/model/__init__.py
--rw-r--r--   0        0        0    29427 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/model/open_api_generated.py
--rw-r--r--   0        0        0     3923 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/model/sirenentities.py
--rw-r--r--   0        0        0      623 2024-04-19 13:35:07.245525 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/tool/__init__.py
--rw-r--r--   0        0        0    14505 2024-04-19 13:45:00.838479 q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/tool/job.py
--rw-r--r--   0        0        0        0 2024-04-19 13:35:07.245525 q_alchemy_sdk_py-0.2.5/src/q_alchemy/__init__.py
--rw-r--r--   0        0        0     8056 2024-04-19 13:38:48.367907 q_alchemy_sdk_py-0.2.5/src/q_alchemy/qiskit_integration.py
--rw-r--r--   0        0        0     4354 2024-04-19 13:38:48.367907 q_alchemy_sdk_py-0.2.5/src/q_alchemy/qiskit_to_pennylane.py
--rw-r--r--   0        0        0      603 2024-03-19 19:59:43.347535 q_alchemy_sdk_py-0.2.5/tests/__init__.py
--rw-r--r--   0        0        0    16512 2024-03-19 19:59:43.350535 q_alchemy_sdk_py-0.2.5/tests/data/test_baa_state.10.1.npy
--rw-r--r--   0        0        0    65664 2024-03-19 19:59:43.351535 q_alchemy_sdk_py-0.2.5/tests/data/test_baa_state.12.1.npy
--rw-r--r--   0        0        0     2176 2024-03-19 19:59:43.352534 q_alchemy_sdk_py-0.2.5/tests/data/test_baa_state.7.1.npy
--rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 q_alchemy_sdk_py-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11556 2024-03-19 19:59:43.321774 q_alchemy_sdk_py-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3132 2024-04-19 13:35:07.213197 q_alchemy_sdk_py-0.2.6/README.md
+-rw-r--r--   0        0        0      707 2024-04-23 18:44:12.380690 q_alchemy_sdk_py-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      599 2024-04-19 13:35:07.228950 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/__init__.py
+-rw-r--r--   0        0        0      844 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-19 13:35:07.230172 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/base_relations.py
+-rw-r--r--   0        0        0     1634 2024-04-23 13:34:36.299390 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/enterapi.py
+-rw-r--r--   0        0        0      986 2024-04-23 13:32:49.546732 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/exceptions.py
+-rw-r--r--   0        0        0      599 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/__init__.py
+-rw-r--r--   0        0        0     2955 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/action_hco.py
+-rw-r--r--   0        0        0     3906 2024-04-19 13:35:07.231275 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/action_with_parameters_hco.py
+-rw-r--r--   0        0        0     2002 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/download_link_hco.py
+-rw-r--r--   0        0        0     4062 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/hco_base.py
+-rw-r--r--   0        0        0     2573 2024-04-23 11:21:12.137955 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/link_hco.py
+-rw-r--r--   0        0        0     5287 2024-04-19 13:35:07.232592 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/upload_action_hco.py
+-rw-r--r--   0        0        0      793 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/http_headers.py
+-rw-r--r--   0        0        0     1225 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/media_types.py
+-rw-r--r--   0        0        0      599 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/model/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/model/error.py
+-rw-r--r--   0        0        0     6303 2024-04-19 13:35:07.233729 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/model/sirenmodels.py
+-rw-r--r--   0        0        0     1715 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/polling.py
+-rw-r--r--   0        0        0     1207 2024-04-23 14:22:00.345881 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/resilience_handling.py
+-rw-r--r--   0        0        0     8483 2024-04-23 18:32:15.617402 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/sirenaccess.py
+-rw-r--r--   0        0        0      745 2024-04-19 13:35:07.235133 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/__init__.py
+-rw-r--r--   0        0        0     2118 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/enterjma.py
+-rw-r--r--   0        0        0     1009 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/__init__.py
+-rw-r--r--   0        0        0     3006 2024-04-19 13:35:07.236487 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/entrypoint_hco.py
+-rw-r--r--   0        0        0     1991 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/info_hco.py
+-rw-r--r--   0        0        0     3704 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py
+-rw-r--r--   0        0        0     8200 2024-04-19 13:35:07.237685 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/job_hco.py
+-rw-r--r--   0        0        0     3678 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/job_query_result_hco.py
+-rw-r--r--   0        0        0     1591 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py
+-rw-r--r--   0        0        0     4361 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/jobsroot_hco.py
+-rw-r--r--   0        0        0     2149 2024-04-19 13:35:07.239096 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py
+-rw-r--r--   0        0        0     3727 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processing_step_hco.py
+-rw-r--r--   0        0        0     1714 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py
+-rw-r--r--   0        0        0     3937 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py
+-rw-r--r--   0        0        0     4471 2024-04-19 13:35:07.240528 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py
+-rw-r--r--   0        0        0     1749 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/user_hco.py
+-rw-r--r--   0        0        0     5694 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdata_hco.py
+-rw-r--r--   0        0        0     3616 2024-04-19 13:35:07.241868 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py
+-rw-r--r--   0        0        0     1734 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py
+-rw-r--r--   0        0        0     4772 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdataroot_hco.py
+-rw-r--r--   0        0        0     1223 2024-04-19 13:35:07.242875 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/known_relations.py
+-rw-r--r--   0        0        0      636 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/model/__init__.py
+-rw-r--r--   0        0        0    29427 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/model/open_api_generated.py
+-rw-r--r--   0        0        0     3923 2024-04-19 13:35:07.244338 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/model/sirenentities.py
+-rw-r--r--   0        0        0      623 2024-04-19 13:35:07.245525 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/tool/__init__.py
+-rw-r--r--   0        0        0    14505 2024-04-19 13:45:00.838479 q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/tool/job.py
+-rw-r--r--   0        0        0        0 2024-04-19 13:35:07.245525 q_alchemy_sdk_py-0.2.6/src/q_alchemy/__init__.py
+-rw-r--r--   0        0        0     8187 2024-04-21 14:53:11.167990 q_alchemy_sdk_py-0.2.6/src/q_alchemy/qiskit_integration.py
+-rw-r--r--   0        0        0     4354 2024-04-19 13:38:48.367907 q_alchemy_sdk_py-0.2.6/src/q_alchemy/qiskit_to_pennylane.py
+-rw-r--r--   0        0        0      603 2024-03-19 19:59:43.347535 q_alchemy_sdk_py-0.2.6/tests/__init__.py
+-rw-r--r--   0        0        0    16512 2024-03-19 19:59:43.350535 q_alchemy_sdk_py-0.2.6/tests/data/test_baa_state.10.1.npy
+-rw-r--r--   0        0        0    65664 2024-03-19 19:59:43.351535 q_alchemy_sdk_py-0.2.6/tests/data/test_baa_state.12.1.npy
+-rw-r--r--   0        0        0     2176 2024-03-19 19:59:43.352534 q_alchemy_sdk_py-0.2.6/tests/data/test_baa_state.7.1.npy
+-rw-r--r--   0        0        0     3406 1970-01-01 00:00:00.000000 q_alchemy_sdk_py-0.2.6/PKG-INFO
```

### Comparing `q_alchemy_sdk_py-0.2.5/LICENSE` & `q_alchemy_sdk_py-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/README.md` & `q_alchemy_sdk_py-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/pyproject.toml` & `q_alchemy_sdk_py-0.2.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "q-alchemy-sdk-py"
-version = "0.2.5"
+version = "0.2.6"
 description = ""
 authors = [
     { name = "Carsten Blank", email = "blank@data-cybernetics.com" },
 ]
 dependencies = [
     "qiskit>=1.0.2",
     "pydantic>=2.6.4",
     "httpx<1.0.0,>=0.25.0",
     "pennylane>=0.35.1",
+    "tenacity>=8.2.3",
 ]
 requires-python = "<4,>=3.11"
 readme = "README.md"
 
 [project.license]
 text = "Apache"
```

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/__init__.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/__init__.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/base_relations.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/base_relations.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/enterapi.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,24 +5,37 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import TypeVar, Type
+from typing import List, Self
 
 import httpx
 
-from hypermedia_client.core import Entity
-from hypermedia_client.core.hco.hco_base import Hco
+from hypermedia_client.core.hco.hco_base import Hco, Property
+from hypermedia_client.core.hco.link_hco import LinkHco
+from hypermedia_client.job_management.known_relations import Relations
+from hypermedia_client.job_management.model.sirenentities import ProcessingStepUsedTagsEntity
 
-THco = TypeVar('THco', bound=Hco)
 
+class ProcessingStepUsedTagsHco(Hco[{ProcessingStepUsedTagsEntity}]):
+    tags: List[str] | None = Property()
 
-def enter_api(client: httpx.Client, entrypoint_hco_type: Type[THco], entrypoint_entity_type: Type[Entity] = Entity,
-              entrypoint: str = "api/EntryPoint") -> THco:
-    entry_point_response = client.get(url=entrypoint)
-    entry_point_response.raise_for_status()
-    entrypoint_entity = entrypoint_entity_type.model_validate_json(entry_point_response.read())
+    self_link: 'ProcessingStepUsedTagsLink'
+
+    @classmethod
+    def from_entity(cls, entity: ProcessingStepUsedTagsEntity, client: httpx.Client) -> Self:
+        instance = cls(client, entity)
+
+        Hco.check_classes(instance._entity.class_, ["ProcessingStepUsedTags"])
+
+        instance.self_link = ProcessingStepUsedTagsLink.from_entity(instance._client, instance._entity, Relations.SELF)
+
+        return instance
+
+
+class ProcessingStepUsedTagsLink(LinkHco):
+    def navigate(self) -> ProcessingStepUsedTagsHco:
+        return ProcessingStepUsedTagsHco.from_entity(self._navigate_internal(ProcessingStepUsedTagsEntity), self._client)
 
-    return entrypoint_hco_type.from_entity(entrypoint_entity, client)
```

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/exceptions.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/tool/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,9 +5,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-class SirenException(Exception):
-    pass
+from .job import Job
```

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/__init__.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/action_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/action_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/action_with_parameters_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/action_with_parameters_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/download_link_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/download_link_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/hco_base.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/hco_base.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/link_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/link_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/hco/upload_action_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/hco/upload_action_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/http_headers.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/http_headers.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/media_types.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/media_types.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/model/__init__.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/model/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/model/error.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/model/error.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/model/sirenmodels.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/model/sirenmodels.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/polling.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/polling.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/core/sirenaccess.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/core/sirenaccess.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,32 +15,38 @@
 from typing import Any, BinaryIO, Iterable, AsyncIterable
 
 import httpx
 from httpx import Response
 from httpx import URL
 from pydantic import BaseModel
 
-from .exceptions import SirenException
+from tenacity import retry, retry_if_exception_type, stop_after_attempt
+
+from .exceptions import SirenException, RateLimitError
 from .http_headers import Headers
 from .base_relations import BaseRelations
 from .media_types import MediaTypes
 from .model.error import ProblemDetails
 from .model.sirenmodels import Entity, Link, Action, TEntity
+from .resilience_handling import wait_retry_generator
 
 logger = logging.getLogger(__name__)
 
 
 # for now, we do not support navigations to non siren links (e.g. external)
+@retry(retry=retry_if_exception_type(RateLimitError), wait=wait_retry_generator, stop=stop_after_attempt(4))
 def get_resource(client: httpx.Client, href: str, media_type: str = MediaTypes.SIREN,
                  parse_type: type[TEntity] = Entity) -> TEntity | ProblemDetails | Response:
     try:
         # assume get for links
         response = client.get(href)
     except (httpx.ConnectTimeout, httpx.ConnectError) as exc:
         raise SirenException(f"Http-client error requesting resource: {href}") from exc
+    if response.status_code == 429:
+        raise RateLimitError(response.headers)
     expected_type = media_type or MediaTypes.SIREN  # if not specified expect siren
 
     if response.status_code == httpx.codes.OK:
         if (media_type := response.headers.get(Headers.CONTENT_TYPE, MediaTypes.SIREN)) != expected_type:
             logger.warning(f"Expected type {expected_type} not matched by response: "
                            f"' got: '{media_type}'")
 
@@ -90,36 +96,40 @@
         # Fixme: iterable are not supported. Use the 'content' instead of the 'file' parameter of the request call?
         raise NotImplemented('Iterables are not supported as payload (yet)! Convert to bytes or string.')
 
     return upload_file(client, action, payload, filename, mediatype)
 
 
 # for now no support for multi file upload
+@retry(retry=retry_if_exception_type(RateLimitError), wait=wait_retry_generator, stop=stop_after_attempt(4))
 def upload_file(client: httpx.Client, action: Action, file: BinaryIO, filename: str,
                 mediatype: str = MediaTypes.OCTET_STREAM) -> None | URL | ProblemDetails | Response:
     if action.type != MediaTypes.MULTIPART_FORM_DATA:
         raise SirenException(
             f"Action with upload requires type: {MediaTypes.MULTIPART_FORM_DATA} but found: {action.type}")
 
     files = {'upload-file': (filename, file, mediatype)}
     try:
         response = client.request(method=action.method, url=action.href, files=files)
     except httpx.RequestError as exc:
         raise SirenException(f"Error from httpx while uploading data to: {action.href}") from exc
+    if response.status_code == 429:
+        raise RateLimitError(response.headers)
     return handle_action_result(response)
 
 
 def execute_action_on_entity(client: httpx.Client, entity: Entity, name: str, parameters: BaseModel | None = None):
     action = entity.find_first_action_with_name(name)
     if action is None:
         raise SirenException(f"Entity does not contain expected action: {name}")
 
     return execute_action(client, action, parameters)
 
 
+@retry(retry=retry_if_exception_type(RateLimitError), wait=wait_retry_generator, stop=stop_after_attempt(4))
 def execute_action(client: httpx.Client, action: Action,
                    parameters: BaseModel | None = None) -> None | URL | ProblemDetails | Response:
     if action.has_parameters() is False:
         # no parameters required
         if parameters is not None:
             raise SirenException(f"Action requires no parameters but got some")
     else:
@@ -136,14 +146,16 @@
             method=action.method,
             url=action.href,
             content=action_parameters,
             headers={Headers.CONTENT_TYPE.value: MediaTypes.APPLICATION_JSON.value}
         )
     except httpx.RequestError as exc:
         raise SirenException(f"Error from httpx while executing action: {action.href}") from exc
+    if response.status_code == 429:
+        raise RateLimitError(response.headers)
 
     return handle_action_result(response)
 
 
 def handle_action_result(response: Response) -> None | URL | ProblemDetails | Response:
     if response.status_code == httpx.codes.OK:
         return
```

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/__init__.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/enterjma.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/enterjma.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/__init__.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/entrypoint_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/entrypoint_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/info_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/info_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/input_dataslot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/job_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/job_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/job_query_result_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/job_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/job_used_tags_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/jobsroot_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/jobsroot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/output_dataslot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processing_step_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processing_step_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processing_step_used_tags_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/user_hco.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,37 +5,44 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import List, Self
+from typing import Self
+from uuid import UUID
 
 import httpx
 
 from hypermedia_client.core.hco.hco_base import Hco, Property
 from hypermedia_client.core.hco.link_hco import LinkHco
 from hypermedia_client.job_management.known_relations import Relations
-from hypermedia_client.job_management.model.sirenentities import ProcessingStepUsedTagsEntity
+from hypermedia_client.job_management.model.sirenentities import UserEntity
 
 
-class ProcessingStepUsedTagsHco(Hco[{ProcessingStepUsedTagsEntity}]):
-    tags: List[str] | None = Property()
+class UserLink(LinkHco):
+    def navigate(self) -> "UserHco":
+        return UserHco.from_entity(self._navigate_internal(UserEntity), self._client)
 
-    self_link: 'ProcessingStepUsedTagsLink'
+
+class UserHco(Hco[UserEntity]):
+    user_id: UUID = Property()
+    user_groups: list[str] = Property()
+
+    self_link: UserLink
 
     @classmethod
-    def from_entity(cls, entity: ProcessingStepUsedTagsEntity, client: httpx.Client) -> Self:
+    def from_entity(cls, entity: UserEntity, client: httpx.Client) -> Self:
         instance = cls(client, entity)
 
-        Hco.check_classes(instance._entity.class_, ["ProcessingStepUsedTags"])
+        Hco.check_classes(instance._entity.class_, ["User"])
 
-        instance.self_link = ProcessingStepUsedTagsLink.from_entity(instance._client, instance._entity, Relations.SELF)
+        instance.self_link = UserLink.from_entity(
+            instance._client, instance._entity, Relations.SELF
+        )
 
         return instance
 
-
-class ProcessingStepUsedTagsLink(LinkHco):
-    def navigate(self) -> ProcessingStepUsedTagsHco:
-        return ProcessingStepUsedTagsHco.from_entity(self._navigate_internal(ProcessingStepUsedTagsEntity), self._client)
-
+    def _extract_current_user(self):
+        self.current_user = self._entity.find_all_entities_with_relation(
+            Relations.CURRENT_USER, UserEntity)
```

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processingstep_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/processingsteproot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdata_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdata_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdata_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdata_used_tags_query_result_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/hcos/workdataroot_hco.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/hcos/workdataroot_hco.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/known_relations.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/known_relations.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/model/__init__.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/model/__init__.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/model/open_api_generated.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/model/open_api_generated.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/model/sirenentities.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/model/sirenentities.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/tool/__init__.py` & `q_alchemy_sdk_py-0.2.6/tests/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022-2023 data cybernetics ssc GmbH.
+
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
+
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
-# limitations under the License.
-from .job import Job
+# limitations under the License.
```

### Comparing `q_alchemy_sdk_py-0.2.5/src/hypermedia_client/job_management/tool/job.py` & `q_alchemy_sdk_py-0.2.6/src/hypermedia_client/job_management/tool/job.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/src/q_alchemy/qiskit_integration.py` & `q_alchemy_sdk_py-0.2.6/src/q_alchemy/qiskit_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 import hashlib
 from dataclasses import dataclass, field
 from typing import List, Dict, Tuple
 
 import httpx
 import numpy as np
+from httpx import HTTPTransport
 from qiskit.circuit import QuantumCircuit
 from qiskit.circuit.instruction import Instruction
 from qiskit.quantum_info.states.statevector import Statevector
 
 from hypermedia_client.job_management import enter_jma, Job
 from hypermedia_client.core import MediaTypes
 from hypermedia_client.core.hco.upload_action_hco import UploadParameters
@@ -105,15 +106,19 @@
         headers = {"x-api-key": self.opt_params.api_key}
         headers.update(self.opt_params.added_headers)
         if label is None:
             label = "QAl"
         self.client = httpx.Client(
             base_url=f"{self.opt_params.schema}://{self.opt_params.host}",
             headers=headers,
-            timeout=httpx.Timeout(timeout=self.opt_params.job_completion_timeout_sec + 10.0, connect=10.0)
+            timeout=httpx.Timeout(
+                timeout=self.opt_params.job_completion_timeout_sec + 10.0,
+                connect=10.0
+            ),
+            transport=HTTPTransport(retries=3)
         )
         super().__init__("q-alchemy", num_qubits, 0, params=params, label=label)
         if self.opt_params.assign_data_hash:
             self.param_hash = hashlib.md5(np.asarray(self.params).tobytes()).hexdigest()
         else:
             self.param_hash = datetime.datetime.utcnow().timestamp()
```

### Comparing `q_alchemy_sdk_py-0.2.5/src/q_alchemy/qiskit_to_pennylane.py` & `q_alchemy_sdk_py-0.2.6/src/q_alchemy/qiskit_to_pennylane.py`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/tests/data/test_baa_state.10.1.npy` & `q_alchemy_sdk_py-0.2.6/tests/data/test_baa_state.10.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/tests/data/test_baa_state.12.1.npy` & `q_alchemy_sdk_py-0.2.6/tests/data/test_baa_state.12.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/tests/data/test_baa_state.7.1.npy` & `q_alchemy_sdk_py-0.2.6/tests/data/test_baa_state.7.1.npy`

 * *Files identical despite different names*

### Comparing `q_alchemy_sdk_py-0.2.5/PKG-INFO` & `q_alchemy_sdk_py-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: q-alchemy-sdk-py
-Version: 0.2.5
+Version: 0.2.6
 Author-Email: Carsten Blank <blank@data-cybernetics.com>
 License: Apache
 Requires-Python: <4,>=3.11
 Requires-Dist: qiskit>=1.0.2
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: httpx<1.0.0,>=0.25.0
 Requires-Dist: pennylane>=0.35.1
+Requires-Dist: tenacity>=8.2.3
 Description-Content-Type: text/markdown
 
 # Q-Alchemy Python SDK
 
 This is the Python-SDK for using the data cybernetics [Q-Alchemy](https://www.q-alchemy.com) 
 API which helps quantum computing researchers to put classical data into the quantum computer.
 This is all also called: the loading problem, encoding problem, or quantum state preparation.
```

