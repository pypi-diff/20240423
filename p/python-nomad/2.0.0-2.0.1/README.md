# Comparing `tmp/python-nomad-2.0.0.tar.gz` & `tmp/python_nomad-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-nomad-2.0.0.tar", last modified: Fri May 26 15:49:42 2023, max compression
+gzip compressed data, was "python_nomad-2.0.1.tar", last modified: Tue Apr 23 20:58:52 2024, max compression
```

## Comparing `python-nomad-2.0.0.tar` & `python_nomad-2.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.474536 python-nomad-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 15:49:31.000000 python-nomad-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-26 15:49:42.474536 python-nomad-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-26 15:49:31.000000 python-nomad-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.466536 python-nomad-2.0.0/nomad/
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.470536 python-nomad-2.0.0/nomad/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/allocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-26 15:49:31.000000 python-nomad-2.0.0/nomad/api/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.470536 python-nomad-2.0.0/python_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 15:49:42.000000 python-nomad-2.0.0/python_nomad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:49:42.474536 python-nomad-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-26 15:49:31.000000 python-nomad-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:49:42.474536 python-nomad-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_allocations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-26 15:49:31.000000 python-nomad-2.0.0/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:52.264097 python_nomad-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 20:58:46.000000 python_nomad-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-23 20:58:52.264097 python_nomad-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-04-23 20:58:46.000000 python_nomad-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:52.252097 python_nomad-2.0.1/nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:52.256097 python_nomad-2.0.1/nomad/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/allocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6733 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-23 20:58:46.000000 python_nomad-2.0.1/nomad/api/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:52.264097 python_nomad-2.0.1/python_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-04-23 20:58:52.000000 python_nomad-2.0.1/python_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-23 20:58:52.000000 python_nomad-2.0.1/python_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:58:52.000000 python_nomad-2.0.1/python_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 20:58:52.000000 python_nomad-2.0.1/python_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 20:58:52.000000 python_nomad-2.0.1/python_nomad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:58:52.264097 python_nomad-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 20:58:46.000000 python_nomad-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:52.264097 python_nomad-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_allocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8749 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-04-23 20:58:46.000000 python_nomad-2.0.1/tests/test_variables.py
```

### Comparing `python-nomad-2.0.0/LICENSE` & `python_nomad-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/PKG-INFO` & `python_nomad-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-nomad
-Version: 2.0.0
+Version: 2.0.1
 Summary: Client library for Hashicorp Nomad
 Home-page: http://github.com/jrxfive/python-nomad
 Author: jrxfive
 Author-email: jrxfive@gmail.com
 License: MIT
 Keywords: nomad hashicorp client
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # python-nomad
 
 
 [![Python Nomad Test and Publish](https://github.com/jrxFive/python-nomad/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/jrxFive/python-nomad/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/jrxFive/python-nomad/branch/master/graph/badge.svg)](https://codecov.io/gh/jrxFive/python-nomad)
 [![PyPI version](https://badge.fury.io/py/python-nomad.svg)](https://badge.fury.io/py/python-nomad)
```

### Comparing `python-nomad-2.0.0/README.md` & `python_nomad-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/nomad/__init__.py` & `python_nomad-2.0.1/nomad/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Python library"""
+
 import os
 from typing import Optional
 
 import requests
 
 from nomad import api
 
@@ -13,23 +14,23 @@
     """
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         host: str = "127.0.0.1",
         secure: bool = False,
         port: int = 4646,
-        address: Optional[str] = os.getenv("NOMAD_ADDR", None),
+        address: Optional[str] = None,
         user_agent: Optional[str] = None,
-        namespace: Optional[str] = os.getenv("NOMAD_NAMESPACE", None),
-        token: Optional[str] = os.getenv("NOMAD_TOKEN", None),
+        namespace: Optional[str] = None,
+        token: Optional[str] = None,
         timeout: int = 5,
-        region: Optional[str] = os.getenv("NOMAD_REGION", None),
+        region: Optional[str] = None,
         version: str = "v1",
         verify: bool = False,
-        cert: tuple = (os.getenv("NOMAD_CLIENT_CERT", None), os.getenv("NOMAD_CLIENT_KEY", None)),
+        cert: tuple = (),
         session: requests.Session = None,
     ):
         """Nomad api client
 
         https://github.com/jrxFive/python-nomad/
 
          optional arguments:
@@ -53,27 +54,32 @@
          returns: Nomad api client object
 
          raises:
            - nomad.api.exceptions.BaseNomadException
            - nomad.api.exceptions.URLNotFoundNomadException
            - nomad.api.exceptions.URLNotAuthorizedNomadException
         """
+        cert = cert or (
+            os.getenv("NOMAD_CLIENT_CERT", None),
+            os.getenv("NOMAD_CLIENT_KEY", None),
+        )
+
         self.host = host
         self.secure = secure
         self.port = port
-        self.address = address
+        self.address = address or os.getenv("NOMAD_ADDR", None)
         self.user_agent = user_agent
-        self.region = region
+        self.region = region or os.getenv("NOMAD_REGION", None)
         self.timeout = timeout
         self.version = version
-        self.token = token
+        self.token = token or os.getenv("NOMAD_TOKEN", None)
         self.verify = verify
         self.cert = cert if all(cert) else ()
         self.session = session
-        self.__namespace = namespace
+        self.__namespace = namespace or os.getenv("NOMAD_NAMESPACE", None)
 
         self.requester_settings = {
             "address": self.address,
             "uri": self.get_uri(),
             "port": self.port,
             "user_agent": self.user_agent,
             "namespace": self.__namespace,
```

### Comparing `python-nomad-2.0.0/nomad/api/__init__.py` & `python_nomad-2.0.1/nomad/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Python library"""
+
 import nomad.api.exceptions
 from nomad.api.acl import Acl
 from nomad.api.agent import Agent
 from nomad.api.allocation import Allocation
 from nomad.api.allocations import Allocations
 from nomad.api.base import Requester
 from nomad.api.client import Client
```

### Comparing `python-nomad-2.0.0/nomad/api/acl.py` & `python_nomad-2.0.1/nomad/api/acl.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/nomad/api/agent.py` & `python_nomad-2.0.1/nomad/api/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Agent: https://developer.hashicorp.com/nomad/api-docs/agent"""
+
 from nomad.api.base import Requester
 
 
 class Agent(Requester):
     """The self endpoint is used to query the state of the target agent."""
 
     ENDPOINT = "agent"
```

### Comparing `python-nomad-2.0.0/nomad/api/allocation.py` & `python_nomad-2.0.1/nomad/api/allocation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad allocation: https://developer.hashicorp.com/nomad/api-docs/allocations"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Allocation(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/allocations.py` & `python_nomad-2.0.1/nomad/api/allocations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad allocation: https://developer.hashicorp.com/nomad/api-docs/allocations"""
+
 from typing import Optional
 
 from nomad.api.base import Requester
 
 
 class Allocations(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/base.py` & `python_nomad-2.0.1/nomad/api/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Requester"""
+
 from typing import Optional
 
 import requests
 
 import nomad.api.exceptions
```

### Comparing `python-nomad-2.0.0/nomad/api/client.py` & `python_nomad-2.0.1/nomad/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     def __getattr__(self, item):
         msg = f"{item} does not exist"
         raise AttributeError(msg)
 
 
 class ls(Requester):
-
     """
     The /fs/ls endpoint is used to list files in an allocation directory.
     This API endpoint is hosted by the Nomad client and requests have to be
     made to the Nomad client where the particular allocation was placed.
 
     https://www.nomadproject.io/docs/http/client-fs-ls.html
     """
@@ -63,15 +62,14 @@
         if id_:
             return self.request(id_, params={"path": path}, method="get").json()
 
         return self.request(params={"path": path}, method="get").json()
 
 
 class cat(Requester):
-
     """
     The /fs/cat endpoint is used to read the contents of a file in an
     allocation directory. This API endpoint is hosted by the Nomad
     client and requests have to be made to the Nomad client where the
     particular allocation was placed.
 
     https://www.nomadproject.io/docs/http/client-fs-cat.html
@@ -98,15 +96,14 @@
         if id_:
             return self.request(id_, params={"path": path}, method="get").text
 
         return self.request(params={"path": path}, method="get").text
 
 
 class read_at(Requester):
-
     """
     This endpoint reads the contents of a file in an allocation directory at a particular offset and limit.
 
     https://www.nomadproject.io/api/client.html#read-file-at-offset
     """
 
     ENDPOINT = "client/fs/readat"
@@ -130,15 +127,14 @@
            - nomad.api.exceptions.BadRequestNomadException
         """
         params = {"path": path, "offset": offset, "limit": limit}
         return self.request(id_, params=params, method="get").text
 
 
 class stream_file(Requester):
-
     """
     This endpoint streams the contents of a file in an allocation directory.
 
     https://www.nomadproject.io/api/client.html#stream-file
     """
 
     ENDPOINT = "client/fs/stream"
@@ -162,15 +158,14 @@
           - nomad.api.exceptions.BadRequestNomadException
         """
         params = {"path": path, "offset": offset, "origin": origin}
         return self.request(id_, params=params, method="get").text
 
 
 class stream_logs(Requester):
-
     """
     This endpoint streams a task's stderr/stdout logs.
 
     https://www.nomadproject.io/api/client.html#stream-logs
     """
 
     ENDPOINT = "client/fs/logs"
@@ -192,15 +187,22 @@
           - origin: (str) either start|end, default "start"
           - plain: (bool) Return just the plain text without framing. default False
         returns: (str) text
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.BadRequestNomadException
         """
-        params = {"task": task, "type": type_, "follow": follow, "offset": offset, "origin": origin, "plain": plain}
+        params = {
+            "task": task,
+            "type": type_,
+            "follow": follow,
+            "offset": offset,
+            "origin": origin,
+            "plain": plain,
+        }
         return self.request(id_, params=params, method="get").text
 
 
 class stat(Requester):
     """
     The /fs/stat endpoint is used to show stat information
     This API endpoint is hosted by the Nomad client and requests have to be
@@ -300,15 +302,14 @@
            - nomad.api.exceptions.BaseNomadException
            - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(id_, "restart", method="post").json()
 
 
 class gc_allocation(Requester):
-
     """
     This endpoint forces a garbage collection of a particular, stopped allocation on a node.
 
     https://www.nomadproject.io/api/client.html#gc-allocation
     """
 
     ENDPOINT = "client/allocation"
```

### Comparing `python-nomad-2.0.0/nomad/api/deployment.py` & `python_nomad-2.0.1/nomad/api/deployment.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Nomad Deployment: https://developer.hashicorp.com/nomad/api-docs/deployments"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Deployment(Requester):
-
     """
     The /deployment endpoints are used to query for and interact with deployments.
 
     https://www.nomadproject.io/docs/http/deployments.html
     """
 
     ENDPOINT = "deployment"
```

### Comparing `python-nomad-2.0.0/nomad/api/deployments.py` & `python_nomad-2.0.1/nomad/api/deployments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Deployment: https://developer.hashicorp.com/nomad/api-docs/deployments"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Deployments(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/evaluation.py` & `python_nomad-2.0.1/nomad/api/evaluation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Evaluation: https://developer.hashicorp.com/nomad/api-docs/evaluations"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Evaluation(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/evaluations.py` & `python_nomad-2.0.1/nomad/api/evaluations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Evaluations: https://developer.hashicorp.com/nomad/api-docs/evaluations"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Evaluations(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/event.py` & `python_nomad-2.0.1/nomad/api/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Events: https://developer.hashicorp.com/nomad/api-docs/events"""
+
 import json
 import threading
 import queue
 
 import requests
 
 from nomad.api.base import Requester
```

### Comparing `python-nomad-2.0.0/nomad/api/exceptions.py` & `python_nomad-2.0.1/nomad/api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Internal library exceptions"""
+
 import requests
 
 
 class BaseNomadException(Exception):
     """General Error occurred when interacting with nomad API"""
 
     def __init__(self, nomad_resp):
```

### Comparing `python-nomad-2.0.0/nomad/api/job.py` & `python_nomad-2.0.1/nomad/api/job.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Nomad job: https://developer.hashicorp.com/nomad/api-docs/jobs"""
-import nomad.api.exceptions
+
+from typing import Union
 
 from nomad.api.base import Requester
+import nomad.api.exceptions
 
 
 class Job(Requester):
     """
     The job endpoint is used for CRUD on a single job.
     By default, the agent's local region is used.
 
@@ -77,41 +79,66 @@
         returns: list of dicts
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(id_, "versions", method="get").json()
 
-    def get_allocations(self, id_):
+    def get_allocations(
+        self,
+        id_: str,
+        all_: Union[bool, None] = None,
+        namespace: Union[str, None] = None,
+    ):
         """Query the allocations belonging to a single job.
 
         https://www.nomadproject.io/docs/http/job.html
 
         arguments:
-          - id_
+            - id_
+            - all (bool optional)
+            - namespace (str) optional.
+            Specifies the target namespace. If ACL is enabled, this value
+            must match a namespace that the token is allowed to access.
+            This is specified as a query string parameter.
         returns: list
         raises:
-          - nomad.api.exceptions.BaseNomadException
-          - nomad.api.exceptions.URLNotFoundNomadException
+            - nomad.api.exceptions.BaseNomadException
+            - nomad.api.exceptions.URLNotFoundNomadException
         """
-        return self.request(id_, "allocations", method="get").json()
-
-    def get_evaluations(self, id_):
+        params = {
+            "all": all_,
+            "namespace": namespace,
+        }
+        return self.request(id_, "allocations", params=params, method="get").json()
+
+    def get_evaluations(
+        self,
+        id_: str,
+        namespace: Union[str, None] = None,
+    ):
         """Query the evaluations belonging to a single job.
 
         https://www.nomadproject.io/docs/http/job.html
 
         arguments:
-          - id_
+            - id_
+            - namespace (str) optional.
+            Specifies the target namespace. If ACL is enabled, this value
+            must match a namespace that the token is allowed to access.
+            This is specified as a query string parameter.
         returns: dict
         raises:
-          - nomad.api.exceptions.BaseNomadException
-          - nomad.api.exceptions.URLNotFoundNomadException
-        """
-        return self.request(id_, "evaluations", method="get").json()
+            - nomad.api.exceptions.BaseNomadException
+            - nomad.api.exceptions.URLNotFoundNomadException
+        """
+        params = {
+            "namespace": namespace,
+        }
+        return self.request(id_, "evaluations", params=params, method="get").json()
 
     def get_deployments(self, id_):
         """This endpoint lists a single job's deployments
 
         https://www.nomadproject.io/docs/http/job.html
 
         arguments:
@@ -248,15 +275,19 @@
                                    This is checked and acts as a check-and-set value before reverting to the
                                    specified job.
         returns: dict
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
         """
-        revert_json = {"JobID": id_, "JobVersion": version, "EnforcePriorVersion": enforce_prior_version}
+        revert_json = {
+            "JobID": id_,
+            "JobVersion": version,
+            "EnforcePriorVersion": enforce_prior_version,
+        }
         return self.request(id_, "revert", json=revert_json, method="post").json()
 
     def stable_job(self, id_, version, stable):
         """This endpoint sets the job's stability.
 
         https://www.nomadproject.io/docs/http/job.html
 
@@ -268,32 +299,51 @@
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
         """
         revert_json = {"JobID": id_, "JobVersion": version, "Stable": stable}
         return self.request(id_, "stable", json=revert_json, method="post").json()
 
-    def deregister_job(self, id_, purge=None):
+    def deregister_job(
+        self,
+        id_: str,
+        eval_priority: Union[int, None] = None,
+        global_: Union[bool, None] = None,
+        namespace: Union[str, None] = None,
+        purge: Union[bool, None] = None,
+    ):  # pylint: disable=too-many-arguments
         """Deregisters a job, and stops all allocations part of it.
 
         https://www.nomadproject.io/docs/http/job.html
 
         arguments:
-          - id_
-          - purge (bool), optionally specifies whether the job should be
-            stopped and purged immediately (`purge=True`) or deferred to the
-            Nomad garbage collector (`purge=False`).
+            - id_
+            - eval_priority (int) optional.
+            Override the priority of the evaluations produced as a result
+            of this job deregistration. By default, this is set to the
+            priority of the job.
+            - global_ (bool) optional.
+            Stop a multi-region job in all its regions. By default, job
+            stop will stop only a single region at a time. Ignored for
+            single-region jobs.
+            - purge (bool) optional.
+            Specifies that the job should be stopped and purged immediately.
+            This means the job will not be queryable after being stopped.
+            If not set, the job will be purged by the garbage collector.
+            - namespace (str) optional.
+            Specifies the target namespace. If ACL is enabled, this value
+            must match a namespace that the token is allowed to access.
+            This is specified as a query string parameter.
 
         returns: dict
         raises:
-          - nomad.api.exceptions.BaseNomadException
-          - nomad.api.exceptions.URLNotFoundNomadException
-          - nomad.api.exceptions.InvalidParameters
-        """
-        params = None
-        if purge is not None:
-            if not isinstance(purge, bool):
-                raise nomad.api.exceptions.InvalidParameters(
-                    "purge is invalid " f"(expected type {type(bool())} but got {type(purge)})"
-                )
-            params = {"purge": purge}
+            - nomad.api.exceptions.BaseNomadException
+            - nomad.api.exceptions.URLNotFoundNomadException
+            - nomad.api.exceptions.InvalidParameters
+        """
+        params = {
+            "eval_priority": eval_priority,
+            "global": global_,
+            "namespace": namespace,
+            "purge": purge,
+        }
         return self.request(id_, params=params, method="delete").json()
```

### Comparing `python-nomad-2.0.0/nomad/api/jobs.py` & `python_nomad-2.0.1/nomad/api/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad job: https://developer.hashicorp.com/nomad/api-docs/jobs"""
+
 from typing import Optional
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Jobs(Requester):
@@ -115,9 +116,12 @@
 
         returns: dict
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
         """
         return self.request(
-            "parse", json={"JobHCL": hcl, "Canonicalize": canonicalize}, method="post", allow_redirects=True
+            "parse",
+            json={"JobHCL": hcl, "Canonicalize": canonicalize},
+            method="post",
+            allow_redirects=True,
         ).json()
```

### Comparing `python-nomad-2.0.0/nomad/api/metrics.py` & `python_nomad-2.0.1/nomad/api/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Metrics: https://developer.hashicorp.com/nomad/api-docs/metrics"""
+
 from nomad.api.base import Requester
 
 
 class Metrics(Requester):
     """
     The /metrics endpoint returns metrics for the current Nomad process.
```

### Comparing `python-nomad-2.0.0/nomad/api/namespace.py` & `python_nomad-2.0.1/nomad/api/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad namespace: https://developer.hashicorp.com/nomad/api-docs/namespaces"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Namespace(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/namespaces.py` & `python_nomad-2.0.1/nomad/api/namespaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad namespace: https://developer.hashicorp.com/nomad/api-docs/namespaces"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Namespaces(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/node.py` & `python_nomad-2.0.1/nomad/api/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Node: https://developer.hashicorp.com/nomad/api-docs/nodes"""
+
 from typing import Optional
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Node(Requester):
@@ -121,28 +122,37 @@
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
         """
         payload = {}
 
         if drain_spec and mark_eligible is not None:
-            payload = {"NodeID": id_, "DrainSpec": drain_spec, "MarkEligible": mark_eligible}
+            payload = {
+                "NodeID": id_,
+                "DrainSpec": drain_spec,
+                "MarkEligible": mark_eligible,
+            }
         elif drain_spec and mark_eligible is None:
             payload = {"NodeID": id_, "DrainSpec": drain_spec}
         elif not drain_spec and mark_eligible is not None:
             payload = {"NodeID": id_, "DrainSpec": None, "MarkEligible": mark_eligible}
         elif not drain_spec and mark_eligible is None:
             payload = {
                 "NodeID": id_,
                 "DrainSpec": None,
             }
 
         return self.request(id_, "drain", json=payload, method="post").json()
 
-    def eligible_node(self, id_: str, eligible: Optional[bool] = None, ineligible: Optional[bool] = None):
+    def eligible_node(
+        self,
+        id_: str,
+        eligible: Optional[bool] = None,
+        ineligible: Optional[bool] = None,
+    ):
         """Toggle the eligibility of the node.
 
         https://www.nomadproject.io/docs/http/node.html
 
         arguments:
           - id_ (str uuid): node id
           - eligible (bool): Set to True to mark node eligible
```

### Comparing `python-nomad-2.0.0/nomad/api/nodes.py` & `python_nomad-2.0.1/nomad/api/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Node: https://developer.hashicorp.com/nomad/api-docs/nodes"""
+
 from typing import Optional
 
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
@@ -83,12 +84,12 @@
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
         """
         params = {
             "prefix": prefix,
             "next_token": next_token,
             "per_page": per_page,
-            "filter_": filter_,
+            "filter": filter_,
             "resources": resources,
             "os": os,
         }
         return self.request(method="get", params=params).json()
```

### Comparing `python-nomad-2.0.0/nomad/api/operator.py` & `python_nomad-2.0.1/nomad/api/operator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Operator: https://developer.hashicorp.com/nomad/api-docs/operator"""
+
 from nomad.api.base import Requester
 
 
 class Operator(Requester):
     """
     The Operator endpoint provides cluster-level tools for
     Nomad operators, such as interacting with the Raft subsystem.
```

### Comparing `python-nomad-2.0.0/nomad/api/regions.py` & `python_nomad-2.0.1/nomad/api/regions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad region: https://developer.hashicorp.com/nomad/api-docs/regions"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Regions(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/scaling.py` & `python_nomad-2.0.1/nomad/api/scaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Scalling API: https://developer.hashicorp.com/nomad/api-docs/scaling-policies"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Scaling(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/search.py` & `python_nomad-2.0.1/nomad/api/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Search API: https://developer.hashicorp.com/nomad/api-docs/search"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Search(Requester):
     """
@@ -42,15 +43,24 @@
             "volumes" or "all", where "all" means every context will be searched.
         returns: dict
         raises:
           - nomad.api.exceptions.BaseNomadException
           - nomad.api.exceptions.URLNotFoundNomadException
           - nomad.api.exceptions.InvalidParameters
         """
-        accetaple_contexts = ("jobs", "evals", "allocs", "nodes", "deployment", "plugins", "volumes", "all")
+        accetaple_contexts = (
+            "jobs",
+            "evals",
+            "allocs",
+            "nodes",
+            "deployment",
+            "plugins",
+            "volumes",
+            "all",
+        )
         if context not in accetaple_contexts:
             raise nomad.api.exceptions.InvalidParameters(
                 "context is invalid " f"(expected values are {accetaple_contexts} but got {context})"
             )
         params = {"Prefix": prefix, "Context": context}
 
         return self.request(json=params, method="post").json()
```

### Comparing `python-nomad-2.0.0/nomad/api/sentinel.py` & `python_nomad-2.0.1/nomad/api/sentinel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Sentinel API: https://developer.hashicorp.com/nomad/api-docs/sentinel-policies"""
+
 from nomad.api.base import Requester
 
 
 class Sentinel(Requester):
     """
     The endpoint manage sentinel policies (Enterprise Only)
```

### Comparing `python-nomad-2.0.0/nomad/api/status.py` & `python_nomad-2.0.1/nomad/api/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Status API: https://developer.hashicorp.com/nomad/api-docs/status"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Status:
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/system.py` & `python_nomad-2.0.1/nomad/api/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad System API: https://developer.hashicorp.com/nomad/api-docs/system"""
+
 from nomad.api.base import Requester
 
 
 class System(Requester):
     """
     The system endpoint is used to for system maintenance
     and should not be necessary for most users.
```

### Comparing `python-nomad-2.0.0/nomad/api/validate.py` & `python_nomad-2.0.1/nomad/api/validate.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Nomad Validate API: https://developer.hashicorp.com/nomad/api-docs/validate"""
+
 from nomad.api.base import Requester
 
 
 class Validate(Requester):
-
     """
     The system endpoint is used to for system maintenance
     and should not be necessary for most users.
     By default, the agent's local region is used.
 
     https://www.nomadproject.io/docs/http/system.html
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/variable.py` & `python_nomad-2.0.1/nomad/api/variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Valiables API: https://developer.hashicorp.com/nomad/api-docs/variables"""
+
 import nomad.api.exceptions
 
 from nomad.api.base import Requester
 
 
 class Variable(Requester):
     """
```

### Comparing `python-nomad-2.0.0/nomad/api/variables.py` & `python_nomad-2.0.1/nomad/api/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Nomad Valiables API: https://developer.hashicorp.com/nomad/api-docs/variables"""
+
 from nomad.api.base import Requester
 
 
 class Variables(Requester):
     """
     The /vars endpoints are used to query for and interact with variables.
     https://developer.hashicorp.com/nomad/api-docs/variables
```

### Comparing `python-nomad-2.0.0/python_nomad.egg-info/PKG-INFO` & `python_nomad-2.0.1/python_nomad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-nomad
-Version: 2.0.0
+Version: 2.0.1
 Summary: Client library for Hashicorp Nomad
 Home-page: http://github.com/jrxfive/python-nomad
 Author: jrxfive
 Author-email: jrxfive@gmail.com
 License: MIT
 Keywords: nomad hashicorp client
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
 
 # python-nomad
 
 
 [![Python Nomad Test and Publish](https://github.com/jrxFive/python-nomad/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/jrxFive/python-nomad/actions/workflows/main.yml)
 [![codecov](https://codecov.io/gh/jrxFive/python-nomad/branch/master/graph/badge.svg)](https://codecov.io/gh/jrxFive/python-nomad)
 [![PyPI version](https://badge.fury.io/py/python-nomad.svg)](https://badge.fury.io/py/python-nomad)
```

### Comparing `python-nomad-2.0.0/python_nomad.egg-info/SOURCES.txt` & `python_nomad-2.0.1/python_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/setup.py` & `python_nomad-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='python-nomad',
-    version='2.0.0',
+    version='2.0.1',
     install_requires=['requests'],
     packages=['nomad', 'nomad.api'],
     url='http://github.com/jrxfive/python-nomad',
     license='MIT',
     author='jrxfive',
     author_email='jrxfive@gmail.com',
     description='Client library for Hashicorp Nomad',
```

### Comparing `python-nomad-2.0.0/tests/test_acl.py` & `python_nomad-2.0.1/tests/test_acl.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_agent.py` & `python_nomad-2.0.1/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_allocation.py` & `python_nomad-2.0.1/tests/test_allocation.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_allocations.py` & `python_nomad-2.0.1/tests/test_allocations.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_base.py` & `python_nomad-2.0.1/tests/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -157,7 +157,14 @@
     n = nomad.Nomad(
         address=nomad_address, host=common.IP, port=common.NOMAD_PORT, verify=False,
         token=common.NOMAD_TOKEN, user_agent=custom_agent_name
     )
     n.jobs.get_jobs()
 
     assert responses.calls[0].request.headers["User-Agent"] == custom_agent_name
+
+def test_env_variables():
+    # This ensures that the env variables are only read upon initialization of Nomad() instance,
+    # and not before.
+    with mock.patch.dict(os.environ, {"NOMAD_ADDR": "https://foo"}):
+        n = nomad.Nomad()
+        assert n.address == os.environ["NOMAD_ADDR"]
```

### Comparing `python-nomad-2.0.0/tests/test_client.py` & `python_nomad-2.0.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_deployment.py` & `python_nomad-2.0.1/tests/test_deployment.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_deployments.py` & `python_nomad-2.0.1/tests/test_deployments.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_evaluation.py` & `python_nomad-2.0.1/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_evaluations.py` & `python_nomad-2.0.1/tests/test_evaluations.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_event.py` & `python_nomad-2.0.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_job.py` & `python_nomad-2.0.1/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_jobs.py` & `python_nomad-2.0.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_metrics.py` & `python_nomad-2.0.1/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_namespace.py` & `python_nomad-2.0.1/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_namespaces.py` & `python_nomad-2.0.1/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_node.py` & `python_nomad-2.0.1/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_nodes.py` & `python_nomad-2.0.1/tests/test_nodes.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_operator.py` & `python_nomad-2.0.1/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_regions.py` & `python_nomad-2.0.1/tests/test_regions.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_search.py` & `python_nomad-2.0.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_sentinel.py` & `python_nomad-2.0.1/tests/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_status.py` & `python_nomad-2.0.1/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_validate.py` & `python_nomad-2.0.1/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_variable.py` & `python_nomad-2.0.1/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `python-nomad-2.0.0/tests/test_variables.py` & `python_nomad-2.0.1/tests/test_variables.py`

 * *Files identical despite different names*

