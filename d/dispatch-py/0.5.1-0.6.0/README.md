# Comparing `tmp/dispatch-py-0.5.1.tar.gz` & `tmp/dispatch_py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispatch-py-0.5.1.tar", last modified: Tue Apr  9 23:37:50 2024, max compression
+gzip compressed data, was "dispatch_py-0.6.0.tar", last modified: Tue Apr 23 01:46:46 2024, max compression
```

## Comparing `dispatch-py-0.5.1.tar` & `dispatch_py-0.6.0.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.543831 dispatch-py-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/buf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/buf/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/expression_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/expression_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/expression_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/buf/validate/priv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   136662 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25078 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/validate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/buf/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/dispatch/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/coroutine.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.547831 dispatch-py-0.5.1/src/dispatch/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.551831 dispatch-py-0.5.1/src/dispatch/experimental/durable/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.c
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame308.h
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame309.h
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame310.h
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame311.h
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame312.h
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/frame313.h
--rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/function.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/durable/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/experimental/lambda_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.551831 dispatch-py-0.5.1/src/dispatch/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/integrations/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    14317 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/proto.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.551831 dispatch-py-0.5.1/src/dispatch/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.555831 dispatch-py-0.5.1/src/dispatch/sdk/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.555831 dispatch-py-0.5.1/src/dispatch/signature/
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/key.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/signature/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/src/dispatch/test/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/src/dispatch/test/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/src/dispatch_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11549 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-09 23:37:50.000000 dispatch-py-0.5.1/src/dispatch_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 23:37:50.559831 dispatch-py-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21510 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/tests/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-09 23:37:45.000000 dispatch-py-0.5.1/tests/test_full.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.604666 dispatch_py-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-23 01:46:46.604666 dispatch_py-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:46:46.604666 dispatch_py-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.588666 dispatch_py-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.588666 dispatch_py-0.6.0/src/buf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.588666 dispatch_py-0.6.0/src/buf/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/expression_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/expression_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/expression_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.592666 dispatch_py-0.6.0/src/buf/validate/priv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/priv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/priv/private_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/priv/private_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   136662 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25078 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/validate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/buf/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.592666 dispatch_py-0.6.0/src/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/coroutine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.592666 dispatch_py-0.6.0/src/dispatch/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.596666 dispatch_py-0.6.0/src/dispatch/experimental/durable/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15258 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame308.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame309.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame310.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame311.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame312.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/frame313.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11109 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/durable/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/experimental/lambda_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.596666 dispatch_py-0.6.0/src/dispatch/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/integrations/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/integrations/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/integrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/integrations/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/integrations/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14755 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20657 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.596666 dispatch_py-0.6.0/src/dispatch/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.600666 dispatch_py-0.6.0/src/dispatch/sdk/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/call_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/call_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/call_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/dispatch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/dispatch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/dispatch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/error_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/exit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/exit_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/exit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/function_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/function_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/poll_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/poll_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/poll_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/sdk/v1/status_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.600666 dispatch_py-0.6.0/src/dispatch/signature/
+-rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/signature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/signature/digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/signature/key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/signature/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.600666 dispatch_py-0.6.0/src/dispatch/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/test/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/test/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/src/dispatch/test/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.600666 dispatch_py-0.6.0/src/dispatch_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-04-23 01:46:46.000000 dispatch_py-0.6.0/src/dispatch_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-23 01:46:46.000000 dispatch_py-0.6.0/src/dispatch_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:46:46.000000 dispatch_py-0.6.0/src/dispatch_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 01:46:46.000000 dispatch_py-0.6.0/src/dispatch_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 01:46:46.000000 dispatch_py-0.6.0/src/dispatch_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:46:46.600666 dispatch_py-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/tests/test_fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/tests/test_full.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-04-23 01:46:41.000000 dispatch_py-0.6.0/tests/test_http.py
```

### Comparing `dispatch-py-0.5.1/CONTRIBUTING.md` & `dispatch_py-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/LICENSE` & `dispatch_py-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/Makefile` & `dispatch_py-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/PKG-INFO` & `dispatch_py-0.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: dispatch-py
-Version: 0.5.1
+Version: 0.6.0
 Summary: Develop reliable distributed systems on the Dispatch platform.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio>=1.60.0
 Requires-Dist: protobuf>=4.24.0
 Requires-Dist: types-protobuf>=4.24.0.20240129
 Requires-Dist: grpc-stubs>=1.53.0.5
 Requires-Dist: http-message-signatures>=0.4.4
 Requires-Dist: tblib>=3.0.0
-Requires-Dist: docopt>=0.6.2
-Requires-Dist: types-docopt>=0.6.11.4
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: typing_extensions>=4.10
 Provides-Extra: fastapi
 Requires-Dist: fastapi; extra == "fastapi"
 Requires-Dist: httpx; extra == "fastapi"
 Provides-Extra: lambda
 Requires-Dist: awslambdaric; extra == "lambda"
@@ -50,193 +48,104 @@
 [![Test](https://github.com/stealthrocket/dispatch-py/actions/workflows/test.yml/badge.svg?branch=)](https://github.com/stealthrocket/dispatch-py/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/dispatch-py.svg)](https://badge.fury.io/py/dispatch-py)
 [![Reference](https://img.shields.io/badge/API-Reference-lightblue.svg)](https://python.dispatch.run/main/reference/dispatch/)
 
 Python package to develop applications with the Dispatch platform.
 
 [fastapi]: https://fastapi.tiangolo.com/tutorial/first-steps/
-[ngrok]:   https://ngrok.com/
 [pypi]:    https://pypi.org/project/dispatch-py/
 [signup]:  https://console.dispatch.run/
 
 - [What is Dispatch?](#what-is-dispatch)
 - [Installation](#installation)
+  - [Installing the Dispatch CLI](#installing-the-dispatch-cli)
+  - [Installing the Dispatch SDK](#installing-the-dispatch-sdk)
 - [Usage](#usage)
-  - [Configuration](#configuration)
+  - [Writing Dispatch Applications](#writing-dispatch-applications)
+  - [Running Dispatch Applications](#running-dispatch-applications)
+  - [Writing Transactional Applications with Dispatch](#writing-transactional-applications-with-dispatch)
   - [Integration with FastAPI](#integration-with-fastapi)
-  - [Local Testing](#local-testing)
-  - [Distributed Coroutines for Python](#distributed-coroutines-for-python)
+  - [Configuration](#configuration)
   - [Serialization](#serialization)
 - [Examples](#examples)
 - [Contributing](#contributing)
 
 ## What is Dispatch?
 
 Dispatch is a platform for developing scalable & reliable distributed systems.
 
-Dispatch provides a simple programming model based on *Distributed Coroutines*,
-allowing complex, dynamic workflows to be expressed with regular code and
-control flow.
-
-Dispatch schedules function calls across a fleet of service instances,
-incorporating **fair scheduling**, transparent **retry of failed operations**,
-and **durability**.
-
 To get started, follow the instructions to [sign up for Dispatch][signup] 🚀.
 
 ## Installation
 
-This package is published on [PyPI][pypi] as **dispatch-py**, to install:
-```sh
-pip install dispatch-py
-```
-
-## Usage
+### Installing the Dispatch CLI
 
-The SDK allows Python applications to declare functions that Dispatch can
-orchestrate:
+As a pre-requisite, we recommend installing the Dispatch CLI to simplify the
+configuration and execution of applications that use Dispatch. On macOS, this
+can be done easily using [Homebrew](https://docs.brew.sh/):
 
-```python
-@dispatch.function
-def action(msg):
-    ...
+```console
+brew tap stealthrocket/dispatch
+brew install dispatch
 ```
 
-The **@dispatch.function** decorator declares a function that can be run by
-Dispatch. The call has durable execution semantics; if the function fails
-with a temporary error, it is automatically retried, even if the program is
-restarted, or if multiple instances are deployed.
+Alternatively, you can download the latest `dispatch` binary from the
+[Releases](https://github.com/stealthrocket/dispatch/releases) page.
 
-The SDK adds a method to the `action` object, allowing the program to
-dispatch an asynchronous invocation of the function; for example:
+*Note that this step is optional, applications that use Dispatch can run without
+the CLI, passing configuration through environment variables or directly in the
+code. However, the CLI automates the onboarding flow and simplifies the
+configuration, so we recommend starting with it.*
 
-```python
-action.dispatch('hello')
-```
-
-### Configuration
+### Installing the Dispatch SDK
 
-In order for Dispatch to interact with functions remotely, the SDK needs to be
-configured with the address at which the server can be reached. The Dispatch
-API Key must also be set, and optionally, a public signing key should be
-configured to verify that requests originated from Dispatch. These
-configuration options can be passed as arguments to the
-the `Dispatch` constructor, but by default they will be loaded from environment
-variables:
+The Python package is published on [PyPI][pypi] as **dispatch-py**, to install:
+```console
+pip install dispatch-py
+```
 
-| Environment Variable        | Value Example                      |
-| :-------------------------- | :--------------------------------- |
-| `DISPATCH_API_KEY`          | `d4caSl21a5wdx5AxMjdaMeWehaIyXVnN` |
-| `DISPATCH_ENDPOINT_URL`     | `https://service.domain.com`       |
-| `DISPATCH_VERIFICATION_KEY` | `-----BEGIN PUBLIC KEY-----...`    |
+## Usage
 
-Finally, the `Dispatch` instance needs to mount a route on a HTTP server in to
-receive requests from Dispatch. At this time, the SDK integrates with
-FastAPI; adapters for other popular Python frameworks will be added in the
-future.
+### Writing Dispatch Applications
 
-### Integration with FastAPI
+The following snippet shows how to write a very simple Dispatch application
+that does the following:
 
-The following code snippet is a complete example showing how to install a
-`Dispatch` instance on a [FastAPI][fastapi] server:
+1. declare a dispatch function named `greet` which can run asynchronously
+2. schedule a call to `greet` with the argument `World`
+3. run until all dispatched calls have completed
 
 ```python
-from fastapi import FastAPI
-from dispatch.fastapi import Dispatch
-import requests
-
-app = FastAPI()
-dispatch = Dispatch(app)
+# main.py
+import dispatch
 
 @dispatch.function
-def publish(url, payload):
-    r = requests.post(url, data=payload)
-    r.raise_for_status()
+def greet(msg: str):
+    print(f"Hello, ${msg}!")
 
-@app.get('/')
-def root():
-    publish.dispatch('https://httpstat.us/200', {'hello': 'world'})
-    return {'answer': 42}
+dispatch.run(lambda: greet.dispatch('World'))
 ```
 
-In this example, GET requests on the HTTP server dispatch calls to the
-`publish` function. The function runs concurrently to the rest of the
-program, driven by the Dispatch SDK.
-
-The instantiation of the `Dispatch` object on the `FastAPI` application
-automatically installs the HTTP route needed for Dispatch to invoke functions.
+Obviously, this is just an example, a real application would perform much more
+interesting work, but it's a good start to get a sense of how to use Dispatch.
 
-### Local Testing
-
-#### Mock Dispatch
-
-The SDK ships with a mock Dispatch server. It can be used to quickly test your
-local functions, without requiring internet access.
-
-Note that the mock Dispatch server has very limited scheduling capabilities.
+### Running Dispatch Applications
 
+The simplest way to run a Dispatch application is to use the Dispatch CLI, first
+we need to login:
 ```console
-python -m dispatch.test $DISPATCH_ENDPOINT_URL
+dispatch login
 ```
 
-The command will start a mock Dispatch server and print the configuration
-for the SDK.
-
-For example, if your functions were exposed through a local endpoint
-listening on `http://127.0.0.1:8000`, you could run:
-
+Then we are ready to run the example program we wrote above:
 ```console
-$ python -m dispatch.test http://127.0.0.1:8000
-Spawned a mock Dispatch server on 127.0.0.1:4450
-
-Dispatching function calls to the endpoint at http://127.0.0.1:8000
-
-The Dispatch SDK can be configured with:
-
-  export DISPATCH_API_URL="http://127.0.0.1:4450"
-  export DISPATCH_API_KEY="test"
-  export DISPATCH_ENDPOINT_URL="http://127.0.0.1:8000"
-  export DISPATCH_VERIFICATION_KEY="Z+nTe2VRcw8t8Ihx++D+nXtbO28nwjWIOTLRgzrelYs="
-```
-
-#### Real Dispatch
-
-To test local functions with the production instance of Dispatch, it needs
-to be able to access your local endpoint.
-
-A common approach consists of using [ngrok][ngrok] to setup a public endpoint
-that forwards to the server running on localhost.
-
-For example, assuming the server is running on port 8000 (which is the default
-with FastAPI), the command to create a ngrok tunnel is:
-```sh
-ngrok http http://localhost:8000
+dispatch run -- python3 main.py
 ```
-Running this command opens a terminal interface that looks like this:
-```
-ngrok
 
-Build better APIs with ngrok. Early access: ngrok.com/early-access
-
-Session Status                online
-Account                       Alice (Plan: Free)
-Version                       3.6.0
-Region                        United States (California) (us-cal-1)
-Latency                       -
-Web Interface                 http://127.0.0.1:4040
-Forwarding                    https://f441-2600-1700-2802-e01f-6861-dbc9-d551-ecfb.ngrok-free.app -> http://localhost:8000
-```
-To configure the Dispatch SDK, set the endpoint URL to the endpoint for the
-**Forwarding** parameter; each ngrok instance is unique, so you would have a
-different value, but in this example it would be:
-```sh
-export DISPATCH_ENDPOINT_URL="https://f441-2600-1700-2802-e01f-6861-dbc9-d551-ecfb.ngrok-free.app"
-```
-
-### Distributed Coroutines for Python
+### Writing Transactional Applications with Dispatch
 
 The `@dispatch.function` decorator can also be applied to Python coroutines
 (a.k.a. *async* functions), in which case each `await` point becomes a
 durability step in the execution. If the awaited operation fails, it is
 automatically retried, and the parent function is paused until the result are
 available or a permanent error is raised.
 
@@ -280,19 +189,75 @@
 
 @dispatch.function
 async def transform(msg):
     ...
 ```
 
 Dispatch converts Python coroutines to *Distributed Coroutines*, which can be
-suspended and resumed on any instance of a service across a fleet.
+suspended and resumed on any instance of a service across a fleet. For a deep
+dive on these concepts, read our blog post on
+[*Distributed Coroutines with a Native Python Extension and Dispatch*](https://stealthrocket.tech/blog/distributed-coroutines-in-python).
+
+### Integration with FastAPI
+
+Many web applications written in Python are developed using [FastAPI][fastapi].
+Dispatch can integrate with these applications by instantiating a
+`dispatch.fastapi.Dispatch` object. When doing so, the Dispatch functions
+declared by the program can be invoked remotely over the same HTTP interface
+used for the [FastAPI][fastapi] handlers.
+
+The following code snippet is a complete example showing how to install a
+`Dispatch` instance on a [FastAPI][fastapi] server:
+
+```python
+from fastapi import FastAPI
+from dispatch.fastapi import Dispatch
+import requests
+
+app = FastAPI()
+dispatch = Dispatch(app)
+
+@dispatch.function
+def publish(url, payload):
+    r = requests.post(url, data=payload)
+    r.raise_for_status()
+
+@app.get('/')
+def root():
+    publish.dispatch('https://httpstat.us/200', {'hello': 'world'})
+    return {'answer': 42}
+```
+
+In this example, GET requests on the HTTP server dispatch calls to the
+`publish` function. The function runs concurrently to the rest of the
+program, driven by the Dispatch SDK.
+
+### Configuration
+
+The Dispatch CLI automatically configures the SDK, so manual configuration is
+usually not required when running Dispatch applications. However, in some
+advanced cases, it might be useful to explicitly set configuration options.
+
+In order for Dispatch to interact with functions remotely, the SDK needs to be
+configured with the address at which the server can be reached. The Dispatch
+API Key must also be set, and optionally, a public signing key should be
+configured to verify that requests originated from Dispatch. These
+configuration options can be passed as arguments to the
+the `Dispatch` constructor, but by default they will be loaded from environment
+variables:
+
+| Environment Variable        | Value Example                      |
+| :-------------------------- | :--------------------------------- |
+| `DISPATCH_API_KEY`          | `d4caSl21a5wdx5AxMjdaMeWehaIyXVnN` |
+| `DISPATCH_ENDPOINT_URL`     | `https://service.domain.com`       |
+| `DISPATCH_VERIFICATION_KEY` | `-----BEGIN PUBLIC KEY-----...`    |
 
 ### Serialization
 
-Dispatch uses the [pickle] library to serialize coroutines.
+Dispatch uses the [pickle][pickle] library to serialize coroutines.
 
 [pickle]: https://docs.python.org/3/library/pickle.html
 
 Serialization of coroutines is enabled by a CPython extension.
 
 The user must ensure that the contents of their stack frames are
 serializable. That is, users should avoid using variables inside
@@ -303,15 +268,14 @@
 stacks of coroutines and generators will be printed to stdout before
 the pickle library attempts serialization.
 
 For help with a serialization issues, please submit a [GitHub issue][issues].
 
 [issues]: https://github.com/stealthrocket/dispatch-py/issues
 
-
 ## Examples
 
 Check out the [examples](examples/) directory for code samples to help you get
 started with the SDK.
 
 ## Contributing
```

### Comparing `dispatch-py-0.5.1/README.md` & `dispatch_py-0.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,193 +9,104 @@
 [![Test](https://github.com/stealthrocket/dispatch-py/actions/workflows/test.yml/badge.svg?branch=)](https://github.com/stealthrocket/dispatch-py/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/dispatch-py.svg)](https://badge.fury.io/py/dispatch-py)
 [![Reference](https://img.shields.io/badge/API-Reference-lightblue.svg)](https://python.dispatch.run/main/reference/dispatch/)
 
 Python package to develop applications with the Dispatch platform.
 
 [fastapi]: https://fastapi.tiangolo.com/tutorial/first-steps/
-[ngrok]:   https://ngrok.com/
 [pypi]:    https://pypi.org/project/dispatch-py/
 [signup]:  https://console.dispatch.run/
 
 - [What is Dispatch?](#what-is-dispatch)
 - [Installation](#installation)
+  - [Installing the Dispatch CLI](#installing-the-dispatch-cli)
+  - [Installing the Dispatch SDK](#installing-the-dispatch-sdk)
 - [Usage](#usage)
-  - [Configuration](#configuration)
+  - [Writing Dispatch Applications](#writing-dispatch-applications)
+  - [Running Dispatch Applications](#running-dispatch-applications)
+  - [Writing Transactional Applications with Dispatch](#writing-transactional-applications-with-dispatch)
   - [Integration with FastAPI](#integration-with-fastapi)
-  - [Local Testing](#local-testing)
-  - [Distributed Coroutines for Python](#distributed-coroutines-for-python)
+  - [Configuration](#configuration)
   - [Serialization](#serialization)
 - [Examples](#examples)
 - [Contributing](#contributing)
 
 ## What is Dispatch?
 
 Dispatch is a platform for developing scalable & reliable distributed systems.
 
-Dispatch provides a simple programming model based on *Distributed Coroutines*,
-allowing complex, dynamic workflows to be expressed with regular code and
-control flow.
-
-Dispatch schedules function calls across a fleet of service instances,
-incorporating **fair scheduling**, transparent **retry of failed operations**,
-and **durability**.
-
 To get started, follow the instructions to [sign up for Dispatch][signup] 🚀.
 
 ## Installation
 
-This package is published on [PyPI][pypi] as **dispatch-py**, to install:
-```sh
-pip install dispatch-py
-```
-
-## Usage
+### Installing the Dispatch CLI
 
-The SDK allows Python applications to declare functions that Dispatch can
-orchestrate:
+As a pre-requisite, we recommend installing the Dispatch CLI to simplify the
+configuration and execution of applications that use Dispatch. On macOS, this
+can be done easily using [Homebrew](https://docs.brew.sh/):
 
-```python
-@dispatch.function
-def action(msg):
-    ...
+```console
+brew tap stealthrocket/dispatch
+brew install dispatch
 ```
 
-The **@dispatch.function** decorator declares a function that can be run by
-Dispatch. The call has durable execution semantics; if the function fails
-with a temporary error, it is automatically retried, even if the program is
-restarted, or if multiple instances are deployed.
+Alternatively, you can download the latest `dispatch` binary from the
+[Releases](https://github.com/stealthrocket/dispatch/releases) page.
 
-The SDK adds a method to the `action` object, allowing the program to
-dispatch an asynchronous invocation of the function; for example:
+*Note that this step is optional, applications that use Dispatch can run without
+the CLI, passing configuration through environment variables or directly in the
+code. However, the CLI automates the onboarding flow and simplifies the
+configuration, so we recommend starting with it.*
 
-```python
-action.dispatch('hello')
-```
-
-### Configuration
+### Installing the Dispatch SDK
 
-In order for Dispatch to interact with functions remotely, the SDK needs to be
-configured with the address at which the server can be reached. The Dispatch
-API Key must also be set, and optionally, a public signing key should be
-configured to verify that requests originated from Dispatch. These
-configuration options can be passed as arguments to the
-the `Dispatch` constructor, but by default they will be loaded from environment
-variables:
+The Python package is published on [PyPI][pypi] as **dispatch-py**, to install:
+```console
+pip install dispatch-py
+```
 
-| Environment Variable        | Value Example                      |
-| :-------------------------- | :--------------------------------- |
-| `DISPATCH_API_KEY`          | `d4caSl21a5wdx5AxMjdaMeWehaIyXVnN` |
-| `DISPATCH_ENDPOINT_URL`     | `https://service.domain.com`       |
-| `DISPATCH_VERIFICATION_KEY` | `-----BEGIN PUBLIC KEY-----...`    |
+## Usage
 
-Finally, the `Dispatch` instance needs to mount a route on a HTTP server in to
-receive requests from Dispatch. At this time, the SDK integrates with
-FastAPI; adapters for other popular Python frameworks will be added in the
-future.
+### Writing Dispatch Applications
 
-### Integration with FastAPI
+The following snippet shows how to write a very simple Dispatch application
+that does the following:
 
-The following code snippet is a complete example showing how to install a
-`Dispatch` instance on a [FastAPI][fastapi] server:
+1. declare a dispatch function named `greet` which can run asynchronously
+2. schedule a call to `greet` with the argument `World`
+3. run until all dispatched calls have completed
 
 ```python
-from fastapi import FastAPI
-from dispatch.fastapi import Dispatch
-import requests
-
-app = FastAPI()
-dispatch = Dispatch(app)
+# main.py
+import dispatch
 
 @dispatch.function
-def publish(url, payload):
-    r = requests.post(url, data=payload)
-    r.raise_for_status()
+def greet(msg: str):
+    print(f"Hello, ${msg}!")
 
-@app.get('/')
-def root():
-    publish.dispatch('https://httpstat.us/200', {'hello': 'world'})
-    return {'answer': 42}
+dispatch.run(lambda: greet.dispatch('World'))
 ```
 
-In this example, GET requests on the HTTP server dispatch calls to the
-`publish` function. The function runs concurrently to the rest of the
-program, driven by the Dispatch SDK.
-
-The instantiation of the `Dispatch` object on the `FastAPI` application
-automatically installs the HTTP route needed for Dispatch to invoke functions.
+Obviously, this is just an example, a real application would perform much more
+interesting work, but it's a good start to get a sense of how to use Dispatch.
 
-### Local Testing
-
-#### Mock Dispatch
-
-The SDK ships with a mock Dispatch server. It can be used to quickly test your
-local functions, without requiring internet access.
-
-Note that the mock Dispatch server has very limited scheduling capabilities.
+### Running Dispatch Applications
 
+The simplest way to run a Dispatch application is to use the Dispatch CLI, first
+we need to login:
 ```console
-python -m dispatch.test $DISPATCH_ENDPOINT_URL
+dispatch login
 ```
 
-The command will start a mock Dispatch server and print the configuration
-for the SDK.
-
-For example, if your functions were exposed through a local endpoint
-listening on `http://127.0.0.1:8000`, you could run:
-
+Then we are ready to run the example program we wrote above:
 ```console
-$ python -m dispatch.test http://127.0.0.1:8000
-Spawned a mock Dispatch server on 127.0.0.1:4450
-
-Dispatching function calls to the endpoint at http://127.0.0.1:8000
-
-The Dispatch SDK can be configured with:
-
-  export DISPATCH_API_URL="http://127.0.0.1:4450"
-  export DISPATCH_API_KEY="test"
-  export DISPATCH_ENDPOINT_URL="http://127.0.0.1:8000"
-  export DISPATCH_VERIFICATION_KEY="Z+nTe2VRcw8t8Ihx++D+nXtbO28nwjWIOTLRgzrelYs="
-```
-
-#### Real Dispatch
-
-To test local functions with the production instance of Dispatch, it needs
-to be able to access your local endpoint.
-
-A common approach consists of using [ngrok][ngrok] to setup a public endpoint
-that forwards to the server running on localhost.
-
-For example, assuming the server is running on port 8000 (which is the default
-with FastAPI), the command to create a ngrok tunnel is:
-```sh
-ngrok http http://localhost:8000
+dispatch run -- python3 main.py
 ```
-Running this command opens a terminal interface that looks like this:
-```
-ngrok
 
-Build better APIs with ngrok. Early access: ngrok.com/early-access
-
-Session Status                online
-Account                       Alice (Plan: Free)
-Version                       3.6.0
-Region                        United States (California) (us-cal-1)
-Latency                       -
-Web Interface                 http://127.0.0.1:4040
-Forwarding                    https://f441-2600-1700-2802-e01f-6861-dbc9-d551-ecfb.ngrok-free.app -> http://localhost:8000
-```
-To configure the Dispatch SDK, set the endpoint URL to the endpoint for the
-**Forwarding** parameter; each ngrok instance is unique, so you would have a
-different value, but in this example it would be:
-```sh
-export DISPATCH_ENDPOINT_URL="https://f441-2600-1700-2802-e01f-6861-dbc9-d551-ecfb.ngrok-free.app"
-```
-
-### Distributed Coroutines for Python
+### Writing Transactional Applications with Dispatch
 
 The `@dispatch.function` decorator can also be applied to Python coroutines
 (a.k.a. *async* functions), in which case each `await` point becomes a
 durability step in the execution. If the awaited operation fails, it is
 automatically retried, and the parent function is paused until the result are
 available or a permanent error is raised.
 
@@ -239,19 +150,75 @@
 
 @dispatch.function
 async def transform(msg):
     ...
 ```
 
 Dispatch converts Python coroutines to *Distributed Coroutines*, which can be
-suspended and resumed on any instance of a service across a fleet.
+suspended and resumed on any instance of a service across a fleet. For a deep
+dive on these concepts, read our blog post on
+[*Distributed Coroutines with a Native Python Extension and Dispatch*](https://stealthrocket.tech/blog/distributed-coroutines-in-python).
+
+### Integration with FastAPI
+
+Many web applications written in Python are developed using [FastAPI][fastapi].
+Dispatch can integrate with these applications by instantiating a
+`dispatch.fastapi.Dispatch` object. When doing so, the Dispatch functions
+declared by the program can be invoked remotely over the same HTTP interface
+used for the [FastAPI][fastapi] handlers.
+
+The following code snippet is a complete example showing how to install a
+`Dispatch` instance on a [FastAPI][fastapi] server:
+
+```python
+from fastapi import FastAPI
+from dispatch.fastapi import Dispatch
+import requests
+
+app = FastAPI()
+dispatch = Dispatch(app)
+
+@dispatch.function
+def publish(url, payload):
+    r = requests.post(url, data=payload)
+    r.raise_for_status()
+
+@app.get('/')
+def root():
+    publish.dispatch('https://httpstat.us/200', {'hello': 'world'})
+    return {'answer': 42}
+```
+
+In this example, GET requests on the HTTP server dispatch calls to the
+`publish` function. The function runs concurrently to the rest of the
+program, driven by the Dispatch SDK.
+
+### Configuration
+
+The Dispatch CLI automatically configures the SDK, so manual configuration is
+usually not required when running Dispatch applications. However, in some
+advanced cases, it might be useful to explicitly set configuration options.
+
+In order for Dispatch to interact with functions remotely, the SDK needs to be
+configured with the address at which the server can be reached. The Dispatch
+API Key must also be set, and optionally, a public signing key should be
+configured to verify that requests originated from Dispatch. These
+configuration options can be passed as arguments to the
+the `Dispatch` constructor, but by default they will be loaded from environment
+variables:
+
+| Environment Variable        | Value Example                      |
+| :-------------------------- | :--------------------------------- |
+| `DISPATCH_API_KEY`          | `d4caSl21a5wdx5AxMjdaMeWehaIyXVnN` |
+| `DISPATCH_ENDPOINT_URL`     | `https://service.domain.com`       |
+| `DISPATCH_VERIFICATION_KEY` | `-----BEGIN PUBLIC KEY-----...`    |
 
 ### Serialization
 
-Dispatch uses the [pickle] library to serialize coroutines.
+Dispatch uses the [pickle][pickle] library to serialize coroutines.
 
 [pickle]: https://docs.python.org/3/library/pickle.html
 
 Serialization of coroutines is enabled by a CPython extension.
 
 The user must ensure that the contents of their stack frames are
 serializable. That is, users should avoid using variables inside
@@ -262,15 +229,14 @@
 stacks of coroutines and generators will be printed to stdout before
 the pickle library attempts serialization.
 
 For help with a serialization issues, please submit a [GitHub issue][issues].
 
 [issues]: https://github.com/stealthrocket/dispatch-py/issues
 
-
 ## Examples
 
 Check out the [examples](examples/) directory for code samples to help you get
 started with the SDK.
 
 ## Contributing
```

### Comparing `dispatch-py-0.5.1/mkdocs.yml` & `dispatch_py-0.6.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/pyproject.toml` & `dispatch_py-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 dependencies = [
     "grpcio >= 1.60.0",
     "protobuf >= 4.24.0",
     "types-protobuf >= 4.24.0.20240129",
     "grpc-stubs >= 1.53.0.5",
     "http-message-signatures >= 0.4.4",
     "tblib >= 3.0.0",
-    "docopt >= 0.6.2",
-    "types-docopt >= 0.6.11.4",
     "httpx >= 0.27.0",
     "typing_extensions >= 4.10"
 ]
 
 [project.optional-dependencies]
 fastapi = ["fastapi", "httpx"]
 lambda = ["awslambdaric"]
```

### Comparing `dispatch-py-0.5.1/src/buf/validate/expression_pb2.py` & `dispatch_py-0.6.0/src/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/buf/validate/expression_pb2.pyi` & `dispatch_py-0.6.0/src/buf/validate/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.py` & `dispatch_py-0.6.0/src/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/buf/validate/priv/private_pb2.pyi` & `dispatch_py-0.6.0/src/buf/validate/priv/private_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/buf/validate/validate_pb2.py` & `dispatch_py-0.6.0/src/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/buf/validate/validate_pb2.pyi` & `dispatch_py-0.6.0/src/buf/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/coroutine.py` & `dispatch_py-0.6.0/src/dispatch/coroutine.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/__init__.py` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/__init__.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.c` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame.c`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame.pyi` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame308.h` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame308.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame309.h` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame309.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame310.h` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame310.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame311.h` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame311.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame312.h` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame312.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/frame313.h` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/frame313.h`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/function.py` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/function.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/durable/registry.py` & `dispatch_py-0.6.0/src/dispatch/experimental/durable/registry.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/experimental/lambda_handler.py` & `dispatch_py-0.6.0/src/dispatch/experimental/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/fastapi.py` & `dispatch_py-0.6.0/src/dispatch/fastapi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Integration of Dispatch programmable endpoints for FastAPI.
+"""Integration of Dispatch functions with FastAPI.
 
 Example:
 
     import fastapi
     from dispatch.fastapi import Dispatch
 
     app = fastapi.FastAPI()
@@ -14,15 +14,14 @@
 
     @app.get("/")
     def read_root():
         my_function.dispatch()
     """
 
 import asyncio
-import base64
 import logging
 import os
 from datetime import timedelta
 from typing import Optional, Union
 from urllib.parse import urlparse
 
 import fastapi
@@ -32,27 +31,24 @@
 from dispatch.function import Batch, Registry
 from dispatch.proto import Input
 from dispatch.sdk.v1 import function_pb2 as function_pb
 from dispatch.signature import (
     CaseInsensitiveDict,
     Ed25519PublicKey,
     Request,
-    public_key_from_bytes,
-    public_key_from_pem,
+    parse_verification_key,
     verify_request,
 )
 from dispatch.status import Status
 
 logger = logging.getLogger(__name__)
 
 
 class Dispatch(Registry):
-    """A Dispatch programmable endpoint, powered by FastAPI."""
-
-    __slots__ = ("client",)
+    """A Dispatch instance, powered by FastAPI."""
 
     def __init__(
         self,
         app: fastapi.FastAPI,
         endpoint: Optional[str] = None,
         verification_key: Optional[Union[Ed25519PublicKey, str, bytes]] = None,
         api_key: Optional[str] = None,
@@ -61,17 +57,17 @@
         """Initialize a Dispatch endpoint, and integrate it into a FastAPI app.
 
         It mounts a sub-app that implements the Dispatch gRPC interface.
 
         Args:
             app: The FastAPI app to configure.
 
-            endpoint: Full URL of the application the Dispatch programmable
-                endpoint will be running on. Uses the value of the
-                DISPATCH_ENDPOINT_URL environment variable by default.
+            endpoint: Full URL of the application the Dispatch instance will
+                be running on. Uses the value of the DISPATCH_ENDPOINT_URL
+                environment variable by default.
 
             verification_key: Key to use when verifying signed requests. Uses
                 the value of the DISPATCH_VERIFICATION_KEY environment variable
                 if omitted. The environment variable is expected to carry an
                 Ed25519 public key in base64 or PEM format.
                 If not set, request signature verification is disabled (a warning
                 will be logged by the constructor).
@@ -86,81 +82,20 @@
         Raises:
             ValueError: If any of the required arguments are missing.
         """
         if not app:
             raise ValueError(
                 "missing FastAPI app as first argument of the Dispatch constructor"
             )
-
-        endpoint_from = "endpoint argument"
-        if not endpoint:
-            endpoint = os.getenv("DISPATCH_ENDPOINT_URL")
-            endpoint_from = "DISPATCH_ENDPOINT_URL"
-        if not endpoint:
-            raise ValueError(
-                "missing application endpoint: set it with the DISPATCH_ENDPOINT_URL environment variable"
-            )
-
-        logger.info("configuring Dispatch endpoint %s", endpoint)
-
-        parsed_url = urlparse(endpoint)
-        if not parsed_url.netloc or not parsed_url.scheme:
-            raise ValueError(
-                f"{endpoint_from} must be a full URL with protocol and domain (e.g., https://example.com)"
-            )
-
-        verification_key = parse_verification_key(verification_key)
-        if verification_key:
-            base64_key = base64.b64encode(verification_key.public_bytes_raw()).decode()
-            logger.info("verifying request signatures using key %s", base64_key)
-        else:
-            logger.warning(
-                "request verification is disabled because DISPATCH_VERIFICATION_KEY is not set"
-            )
-
         super().__init__(endpoint, api_key=api_key, api_url=api_url)
-
+        verification_key = parse_verification_key(verification_key, endpoint=endpoint)
         function_service = _new_app(self, verification_key)
         app.mount("/dispatch.sdk.v1.FunctionService", function_service)
 
 
-def parse_verification_key(
-    verification_key: Optional[Union[Ed25519PublicKey, str, bytes]],
-) -> Optional[Ed25519PublicKey]:
-    if isinstance(verification_key, Ed25519PublicKey):
-        return verification_key
-
-    from_env = False
-    if not verification_key:
-        try:
-            verification_key = os.environ["DISPATCH_VERIFICATION_KEY"]
-        except KeyError:
-            return None
-        from_env = True
-
-    if isinstance(verification_key, bytes):
-        verification_key = verification_key.decode()
-
-    # Be forgiving when accepting keys in PEM format, which may span
-    # multiple lines. Users attempting to pass a PEM key via an environment
-    # variable may accidentally include literal "\n" bytes rather than a
-    # newline char (0xA).
-    try:
-        return public_key_from_pem(verification_key.replace("\\n", "\n"))
-    except ValueError:
-        pass
-
-    try:
-        return public_key_from_bytes(base64.b64decode(verification_key.encode()))
-    except ValueError:
-        if from_env:
-            raise ValueError(f"invalid DISPATCH_VERIFICATION_KEY '{verification_key}'")
-        raise ValueError(f"invalid verification key '{verification_key}'")
-
-
 class _ConnectResponse(fastapi.Response):
     media_type = "application/grpc+proto"
 
 
 class _ConnectError(fastapi.HTTPException):
     __slots__ = ("status", "code", "message")
 
@@ -242,47 +177,47 @@
             # that carries the Status and the error details. A failure to do
             # so indicates a problem, and we return a 500 rather than attempt
             # to catch and categorize the error here.
             logger.error("function '%s' fatal error", req.function, exc_info=True)
             raise _ConnectError(
                 500, "internal", f"function '{req.function}' fatal error"
             )
-        else:
-            response = output._message
-            status = Status(response.status)
 
-            if response.HasField("poll"):
-                logger.debug(
-                    "function '%s' polling with %d call(s)",
-                    req.function,
-                    len(response.poll.calls),
-                )
-            elif response.HasField("exit"):
-                exit = response.exit
-                if not exit.HasField("result"):
-                    logger.debug("function '%s' exiting with no result", req.function)
-                else:
-                    result = exit.result
-                    if result.HasField("output"):
-                        logger.debug(
-                            "function '%s' exiting with output value", req.function
-                        )
-                    elif result.HasField("error"):
-                        err = result.error
-                        logger.debug(
-                            "function '%s' exiting with error: %s (%s)",
-                            req.function,
-                            err.message,
-                            err.type,
-                        )
-                if exit.HasField("tail_call"):
+        response = output._message
+        status = Status(response.status)
+
+        if response.HasField("poll"):
+            logger.debug(
+                "function '%s' polling with %d call(s)",
+                req.function,
+                len(response.poll.calls),
+            )
+        elif response.HasField("exit"):
+            exit = response.exit
+            if not exit.HasField("result"):
+                logger.debug("function '%s' exiting with no result", req.function)
+            else:
+                result = exit.result
+                if result.HasField("output"):
                     logger.debug(
-                        "function '%s' tail calling function '%s'",
-                        exit.tail_call.function,
+                        "function '%s' exiting with output value", req.function
                     )
+                elif result.HasField("error"):
+                    err = result.error
+                    logger.debug(
+                        "function '%s' exiting with error: %s (%s)",
+                        req.function,
+                        err.message,
+                        err.type,
+                    )
+            if exit.HasField("tail_call"):
+                logger.debug(
+                    "function '%s' tail calling function '%s'",
+                    exit.tail_call.function,
+                )
 
         logger.debug("finished handling run request with status %s", status.name)
         return fastapi.Response(
             content=response.SerializeToString(), media_type="application/proto"
         )
 
     return app
```

### Comparing `dispatch-py-0.5.1/src/dispatch/function.py` & `dispatch_py-0.6.0/src/dispatch/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,32 +172,51 @@
 class Registry:
     """Registry of functions."""
 
     __slots__ = ("functions", "endpoint", "client")
 
     def __init__(
         self,
-        endpoint: str,
+        endpoint: Optional[str] = None,
         api_key: Optional[str] = None,
         api_url: Optional[str] = None,
     ):
         """Initialize a function registry.
 
         Args:
             endpoint: URL of the endpoint that the function is accessible from.
+                Uses the value of the DISPATCH_ENDPOINT_URL environment variable
+                by default.
 
             api_key: Dispatch API key to use for authentication when
                 dispatching calls to functions. Uses the value of the
                 DISPATCH_API_KEY environment variable by default.
 
             api_url: The URL of the Dispatch API to use when dispatching calls
                 to functions. Uses the value of the DISPATCH_API_URL environment
                 variable if set, otherwise defaults to the public Dispatch API
                 (DEFAULT_API_URL).
+
+        Raises:
+            ValueError: If any of the required arguments are missing.
         """
+        endpoint_from = "endpoint argument"
+        if not endpoint:
+            endpoint = os.getenv("DISPATCH_ENDPOINT_URL")
+            endpoint_from = "DISPATCH_ENDPOINT_URL"
+        if not endpoint:
+            raise ValueError(
+                "missing application endpoint: set it with the DISPATCH_ENDPOINT_URL environment variable"
+            )
+        parsed_url = urlparse(endpoint)
+        if not parsed_url.netloc or not parsed_url.scheme:
+            raise ValueError(
+                f"{endpoint_from} must be a full URL with protocol and domain (e.g., https://example.com)"
+            )
+        logger.info("configuring Dispatch endpoint %s", endpoint)
         self.functions: Dict[str, PrimitiveFunction] = {}
         self.endpoint = endpoint
         self.client = Client(api_key=api_key, api_url=api_url)
 
     @overload
     def function(self, func: Callable[P, Coroutine[Any, Any, T]]) -> Function[P, T]: ...
```

### Comparing `dispatch-py-0.5.1/src/dispatch/integrations/http.py` & `dispatch_py-0.6.0/src/dispatch/integrations/http.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/integrations/httpx.py` & `dispatch_py-0.6.0/src/dispatch/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/integrations/openai.py` & `dispatch_py-0.6.0/src/dispatch/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/integrations/requests.py` & `dispatch_py-0.6.0/src/dispatch/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/integrations/slack.py` & `dispatch_py-0.6.0/src/dispatch/integrations/slack.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/proto.py` & `dispatch_py-0.6.0/src/dispatch/proto.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import google.protobuf.any_pb2
 import google.protobuf.message
 import google.protobuf.wrappers_pb2
 import tblib  # type: ignore[import-untyped]
 from google.protobuf import descriptor_pool, duration_pb2, message_factory
 
+from dispatch.id import DispatchID
 from dispatch.sdk.v1 import call_pb2 as call_pb
 from dispatch.sdk.v1 import error_pb2 as error_pb
 from dispatch.sdk.v1 import exit_pb2 as exit_pb
 from dispatch.sdk.v1 import function_pb2 as function_pb
 from dispatch.sdk.v1 import poll_pb2 as poll_pb
 from dispatch.sdk.v1 import status_pb2 as status_pb
 from dispatch.status import Status, status_for_error, status_for_output
@@ -47,22 +48,29 @@
     directive. Use the is_first_call and is_resume properties to differentiate
     between the two cases.
 
     This class is intended to be used as read-only.
     """
 
     __slots__ = (
+        "dispatch_id",
+        "parent_dispatch_id",
+        "root_dispatch_id",
         "_has_input",
         "_input",
         "_coroutine_state",
         "_call_results",
         "_poll_error",
     )
 
     def __init__(self, req: function_pb.RunRequest):
+        self.dispatch_id = req.dispatch_id
+        self.parent_dispatch_id = req.parent_dispatch_id
+        self.root_dispatch_id = req.root_dispatch_id
+
         self._has_input = req.HasField("input")
         if self._has_input:
             if req.input.Is(google.protobuf.wrappers_pb2.BytesValue.DESCRIPTOR):
                 input_pb = google.protobuf.wrappers_pb2.BytesValue()
                 req.input.Unpack(input_pb)
                 input_bytes = input_pb.value
                 try:
@@ -281,38 +289,45 @@
 @dataclass
 class CallResult:
     """Result of a Call."""
 
     correlation_id: Optional[int] = None
     output: Optional[Any] = None
     error: Optional[Error] = None
+    dispatch_id: DispatchID = ""
 
     def _as_proto(self) -> call_pb.CallResult:
         output_any = None
         error_proto = None
         if self.output is not None:
             output_any = _pb_any_pickle(self.output)
         if self.error is not None:
             error_proto = self.error._as_proto()
 
         return call_pb.CallResult(
-            correlation_id=self.correlation_id, output=output_any, error=error_proto
+            correlation_id=self.correlation_id,
+            output=output_any,
+            error=error_proto,
+            dispatch_id=self.dispatch_id,
         )
 
     @classmethod
     def _from_proto(cls, proto: call_pb.CallResult) -> CallResult:
         output = None
         error = None
         if proto.HasField("output"):
             output = _any_unpickle(proto.output)
         if proto.HasField("error"):
             error = Error._from_proto(proto.error)
 
         return CallResult(
-            correlation_id=proto.correlation_id, output=output, error=error
+            correlation_id=proto.correlation_id,
+            output=output,
+            error=error,
+            dispatch_id=proto.dispatch_id,
         )
 
     @classmethod
     def from_value(
         cls, output: Any, correlation_id: Optional[int] = None
     ) -> CallResult:
         return CallResult(correlation_id=correlation_id, output=output)
```

### Comparing `dispatch-py-0.5.1/src/dispatch/scheduler.py` & `dispatch_py-0.6.0/src/dispatch/scheduler.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/call_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from dispatch.sdk.v1 import error_pb2 as dispatch_dot_sdk_dot_v1_dot_error__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1a\x64ispatch/sdk/v1/call.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1b\x64ispatch/sdk/v1/error.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto"\x87\x02\n\x04\x43\x61ll\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12$\n\x08\x65ndpoint\x18\x02 \x01(\tB\x08\xbaH\x05r\x03\x88\x01\x01R\x08\x65ndpoint\x12\x41\n\x08\x66unction\x18\x03 \x01(\tB%\xbaH"r\x1d\x32\x1b^[a-zA-Z_][a-zA-Z0-9_<>.]*$\xc8\x01\x01R\x08\x66unction\x12*\n\x05input\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05input\x12\x43\n\nexpiration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xbaH\x05\xaa\x01\x02\x32\x00R\nexpiration"\x8f\x01\n\nCallResult\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12,\n\x06output\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyR\x06output\x12,\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x16.dispatch.sdk.v1.ErrorR\x05\x65rrorB~\n\x13\x63om.dispatch.sdk.v1B\tCallProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3'
+    b'\n\x1a\x64ispatch/sdk/v1/call.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1b\x64ispatch/sdk/v1/error.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto"\x87\x02\n\x04\x43\x61ll\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12$\n\x08\x65ndpoint\x18\x02 \x01(\tB\x08\xbaH\x05r\x03\x88\x01\x01R\x08\x65ndpoint\x12\x41\n\x08\x66unction\x18\x03 \x01(\tB%\xbaH"r\x1d\x32\x1b^[a-zA-Z_][a-zA-Z0-9_<>.]*$\xc8\x01\x01R\x08\x66unction\x12*\n\x05input\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05input\x12\x43\n\nexpiration\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x08\xbaH\x05\xaa\x01\x02\x32\x00R\nexpiration"\xb0\x01\n\nCallResult\x12%\n\x0e\x63orrelation_id\x18\x01 \x01(\x04R\rcorrelationId\x12,\n\x06output\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyR\x06output\x12,\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x16.dispatch.sdk.v1.ErrorR\x05\x65rror\x12\x1f\n\x0b\x64ispatch_id\x18\x04 \x01(\tR\ndispatchIdB~\n\x13\x63om.dispatch.sdk.v1B\tCallProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "dispatch.sdk.v1.call_pb2", _globals
 )
@@ -44,9 +44,9 @@
     _globals["_CALL"].fields_by_name["expiration"]._options = None
     _globals["_CALL"].fields_by_name[
         "expiration"
     ]._serialized_options = b"\272H\005\252\001\0022\000"
     _globals["_CALL"]._serialized_start = 165
     _globals["_CALL"]._serialized_end = 428
     _globals["_CALLRESULT"]._serialized_start = 431
-    _globals["_CALLRESULT"]._serialized_end = 574
+    _globals["_CALLRESULT"]._serialized_end = 607
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/call_pb2.pyi` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/call_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -31,20 +31,23 @@
         endpoint: _Optional[str] = ...,
         function: _Optional[str] = ...,
         input: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...,
         expiration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...,
     ) -> None: ...
 
 class CallResult(_message.Message):
-    __slots__ = ("correlation_id", "output", "error")
+    __slots__ = ("correlation_id", "output", "error", "dispatch_id")
     CORRELATION_ID_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
+    DISPATCH_ID_FIELD_NUMBER: _ClassVar[int]
     correlation_id: int
     output: _any_pb2.Any
     error: _error_pb2.Error
+    dispatch_id: str
     def __init__(
         self,
         correlation_id: _Optional[int] = ...,
         output: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...,
         error: _Optional[_Union[_error_pb2.Error, _Mapping]] = ...,
+        dispatch_id: _Optional[str] = ...,
     ) -> None: ...
```

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/dispatch_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 _sym_db = _symbol_database.Default()
 
 
 from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from dispatch.sdk.v1 import call_pb2 as dispatch_dot_sdk_dot_v1_dot_call__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b"\n\x1e\x64ispatch/sdk/v1/dispatch.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1a\x64ispatch/sdk/v1/call.proto\"\xb7\x03\n\x0f\x44ispatchRequest\x12+\n\x05\x63\x61lls\x18\x01 \x03(\x0b\x32\x15.dispatch.sdk.v1.CallR\x05\x63\x61lls:\xf6\x02\xbaH\xf2\x02\x1as\n(dispatch.request.calls.endpoint.nonempty\x12\x1d\x43\x61ll endpoint cannot be empty\x1a(this.calls.all(call, has(call.endpoint))\x1a\xfa\x01\n&dispatch.request.calls.endpoint.scheme\x12>Call endpoint must be a http or https URL or an AWS Lambda ARN\x1a\x8f\x01this.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://') || call.endpoint.startsWith('arn:aws:lambda'))\"5\n\x10\x44ispatchResponse\x12!\n\x0c\x64ispatch_ids\x18\x01 \x03(\tR\x0b\x64ispatchIds2d\n\x0f\x44ispatchService\x12Q\n\x08\x44ispatch\x12 .dispatch.sdk.v1.DispatchRequest\x1a!.dispatch.sdk.v1.DispatchResponse\"\x00\x42\x82\x01\n\x13\x63om.dispatch.sdk.v1B\rDispatchProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3"
+    b"\n\x1e\x64ispatch/sdk/v1/dispatch.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1b\x62uf/validate/validate.proto\x1a\x1a\x64ispatch/sdk/v1/call.proto\"\x9d\x03\n\x0f\x44ispatchRequest\x12+\n\x05\x63\x61lls\x18\x01 \x03(\x0b\x32\x15.dispatch.sdk.v1.CallR\x05\x63\x61lls:\xdc\x02\xbaH\xd8\x02\x1as\n(dispatch.request.calls.endpoint.nonempty\x12\x1d\x43\x61ll endpoint cannot be empty\x1a(this.calls.all(call, has(call.endpoint))\x1a\xe0\x01\n&dispatch.request.calls.endpoint.scheme\x12)Call endpoint must be a http or https URL\x1a\x8a\x01this.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://') || call.endpoint.startsWith('bridge://'))\"5\n\x10\x44ispatchResponse\x12!\n\x0c\x64ispatch_ids\x18\x01 \x03(\tR\x0b\x64ispatchIds2d\n\x0f\x44ispatchService\x12Q\n\x08\x44ispatch\x12 .dispatch.sdk.v1.DispatchRequest\x1a!.dispatch.sdk.v1.DispatchResponse\"\x00\x42\x82\x01\n\x13\x63om.dispatch.sdk.v1B\rDispatchProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3"
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "dispatch.sdk.v1.dispatch_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals["DESCRIPTOR"]._options = None
     _globals["DESCRIPTOR"]._serialized_options = (
         b"\n\023com.dispatch.sdk.v1B\rDispatchProtoP\001\242\002\003DSX\252\002\017Dispatch.Sdk.V1\312\002\017Dispatch\\Sdk\\V1\342\002\033Dispatch\\Sdk\\V1\\GPBMetadata\352\002\021Dispatch::Sdk::V1"
     )
     _globals["_DISPATCHREQUEST"]._options = None
     _globals["_DISPATCHREQUEST"]._serialized_options = (
-        b"\272H\362\002\032s\n(dispatch.request.calls.endpoint.nonempty\022\035Call endpoint cannot be empty\032(this.calls.all(call, has(call.endpoint))\032\372\001\n&dispatch.request.calls.endpoint.scheme\022>Call endpoint must be a http or https URL or an AWS Lambda ARN\032\217\001this.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://') || call.endpoint.startsWith('arn:aws:lambda'))"
+        b"\272H\330\002\032s\n(dispatch.request.calls.endpoint.nonempty\022\035Call endpoint cannot be empty\032(this.calls.all(call, has(call.endpoint))\032\340\001\n&dispatch.request.calls.endpoint.scheme\022)Call endpoint must be a http or https URL\032\212\001this.calls.all(call, call.endpoint.startsWith('http://') || call.endpoint.startsWith('https://') || call.endpoint.startsWith('bridge://'))"
     )
     _globals["_DISPATCHREQUEST"]._serialized_start = 109
-    _globals["_DISPATCHREQUEST"]._serialized_end = 548
-    _globals["_DISPATCHRESPONSE"]._serialized_start = 550
-    _globals["_DISPATCHRESPONSE"]._serialized_end = 603
-    _globals["_DISPATCHSERVICE"]._serialized_start = 605
-    _globals["_DISPATCHSERVICE"]._serialized_end = 705
+    _globals["_DISPATCHREQUEST"]._serialized_end = 522
+    _globals["_DISPATCHRESPONSE"]._serialized_start = 524
+    _globals["_DISPATCHRESPONSE"]._serialized_end = 577
+    _globals["_DISPATCHSERVICE"]._serialized_start = 579
+    _globals["_DISPATCHSERVICE"]._serialized_end = 679
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2.pyi` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/dispatch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/dispatch_pb2_grpc.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/dispatch_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/error_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/error_pb2.pyi` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/exit_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/exit_pb2.pyi` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/exit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/function_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 from dispatch.sdk.v1 import exit_pb2 as dispatch_dot_sdk_dot_v1_dot_exit__pb2
 from dispatch.sdk.v1 import poll_pb2 as dispatch_dot_sdk_dot_v1_dot_poll__pb2
 from dispatch.sdk.v1 import status_pb2 as dispatch_dot_sdk_dot_v1_dot_status__pb2
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x1e\x64ispatch/sdk/v1/function.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1a\x64ispatch/sdk/v1/exit.proto\x1a\x1a\x64ispatch/sdk/v1/poll.proto\x1a\x1c\x64ispatch/sdk/v1/status.proto\x1a\x19google/protobuf/any.proto"\xa3\x01\n\nRunRequest\x12\x1a\n\x08\x66unction\x18\x01 \x01(\tR\x08\x66unction\x12,\n\x05input\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00R\x05input\x12>\n\x0bpoll_result\x18\x03 \x01(\x0b\x32\x1b.dispatch.sdk.v1.PollResultH\x00R\npollResultB\x0b\n\tdirective"\xa5\x01\n\x0bRunResponse\x12/\n\x06status\x18\x01 \x01(\x0e\x32\x17.dispatch.sdk.v1.StatusR\x06status\x12+\n\x04\x65xit\x18\x02 \x01(\x0b\x32\x15.dispatch.sdk.v1.ExitH\x00R\x04\x65xit\x12+\n\x04poll\x18\x03 \x01(\x0b\x32\x15.dispatch.sdk.v1.PollH\x00R\x04pollB\x0b\n\tdirective2U\n\x0f\x46unctionService\x12\x42\n\x03Run\x12\x1b.dispatch.sdk.v1.RunRequest\x1a\x1c.dispatch.sdk.v1.RunResponse"\x00\x42\x82\x01\n\x13\x63om.dispatch.sdk.v1B\rFunctionProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3'
+    b'\n\x1e\x64ispatch/sdk/v1/function.proto\x12\x0f\x64ispatch.sdk.v1\x1a\x1a\x64ispatch/sdk/v1/exit.proto\x1a\x1a\x64ispatch/sdk/v1/poll.proto\x1a\x1c\x64ispatch/sdk/v1/status.proto\x1a\x19google/protobuf/any.proto"\x9c\x02\n\nRunRequest\x12\x1a\n\x08\x66unction\x18\x01 \x01(\tR\x08\x66unction\x12,\n\x05input\x18\x02 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00R\x05input\x12>\n\x0bpoll_result\x18\x03 \x01(\x0b\x32\x1b.dispatch.sdk.v1.PollResultH\x00R\npollResult\x12\x1f\n\x0b\x64ispatch_id\x18\x04 \x01(\tR\ndispatchId\x12,\n\x12parent_dispatch_id\x18\x05 \x01(\tR\x10parentDispatchId\x12(\n\x10root_dispatch_id\x18\x06 \x01(\tR\x0erootDispatchIdB\x0b\n\tdirective"\xa5\x01\n\x0bRunResponse\x12/\n\x06status\x18\x01 \x01(\x0e\x32\x17.dispatch.sdk.v1.StatusR\x06status\x12+\n\x04\x65xit\x18\x02 \x01(\x0b\x32\x15.dispatch.sdk.v1.ExitH\x00R\x04\x65xit\x12+\n\x04poll\x18\x03 \x01(\x0b\x32\x15.dispatch.sdk.v1.PollH\x00R\x04pollB\x0b\n\tdirective2U\n\x0f\x46unctionService\x12\x42\n\x03Run\x12\x1b.dispatch.sdk.v1.RunRequest\x1a\x1c.dispatch.sdk.v1.RunResponse"\x00\x42\x82\x01\n\x13\x63om.dispatch.sdk.v1B\rFunctionProtoP\x01\xa2\x02\x03\x44SX\xaa\x02\x0f\x44ispatch.Sdk.V1\xca\x02\x0f\x44ispatch\\Sdk\\V1\xe2\x02\x1b\x44ispatch\\Sdk\\V1\\GPBMetadata\xea\x02\x11\x44ispatch::Sdk::V1b\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
     DESCRIPTOR, "dispatch.sdk.v1.function_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
     _globals["DESCRIPTOR"]._options = None
     _globals["DESCRIPTOR"]._serialized_options = (
         b"\n\023com.dispatch.sdk.v1B\rFunctionProtoP\001\242\002\003DSX\252\002\017Dispatch.Sdk.V1\312\002\017Dispatch\\Sdk\\V1\342\002\033Dispatch\\Sdk\\V1\\GPBMetadata\352\002\021Dispatch::Sdk::V1"
     )
     _globals["_RUNREQUEST"]._serialized_start = 165
-    _globals["_RUNREQUEST"]._serialized_end = 328
-    _globals["_RUNRESPONSE"]._serialized_start = 331
-    _globals["_RUNRESPONSE"]._serialized_end = 496
-    _globals["_FUNCTIONSERVICE"]._serialized_start = 498
-    _globals["_FUNCTIONSERVICE"]._serialized_end = 583
+    _globals["_RUNREQUEST"]._serialized_end = 449
+    _globals["_RUNRESPONSE"]._serialized_start = 452
+    _globals["_RUNRESPONSE"]._serialized_end = 617
+    _globals["_FUNCTIONSERVICE"]._serialized_start = 619
+    _globals["_FUNCTIONSERVICE"]._serialized_end = 704
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2.pyi` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/function_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -10,26 +10,42 @@
 from dispatch.sdk.v1 import exit_pb2 as _exit_pb2
 from dispatch.sdk.v1 import poll_pb2 as _poll_pb2
 from dispatch.sdk.v1 import status_pb2 as _status_pb2
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class RunRequest(_message.Message):
-    __slots__ = ("function", "input", "poll_result")
+    __slots__ = (
+        "function",
+        "input",
+        "poll_result",
+        "dispatch_id",
+        "parent_dispatch_id",
+        "root_dispatch_id",
+    )
     FUNCTION_FIELD_NUMBER: _ClassVar[int]
     INPUT_FIELD_NUMBER: _ClassVar[int]
     POLL_RESULT_FIELD_NUMBER: _ClassVar[int]
+    DISPATCH_ID_FIELD_NUMBER: _ClassVar[int]
+    PARENT_DISPATCH_ID_FIELD_NUMBER: _ClassVar[int]
+    ROOT_DISPATCH_ID_FIELD_NUMBER: _ClassVar[int]
     function: str
     input: _any_pb2.Any
     poll_result: _poll_pb2.PollResult
+    dispatch_id: str
+    parent_dispatch_id: str
+    root_dispatch_id: str
     def __init__(
         self,
         function: _Optional[str] = ...,
         input: _Optional[_Union[_any_pb2.Any, _Mapping]] = ...,
         poll_result: _Optional[_Union[_poll_pb2.PollResult, _Mapping]] = ...,
+        dispatch_id: _Optional[str] = ...,
+        parent_dispatch_id: _Optional[str] = ...,
+        root_dispatch_id: _Optional[str] = ...,
     ) -> None: ...
 
 class RunResponse(_message.Message):
     __slots__ = ("status", "exit", "poll")
     STATUS_FIELD_NUMBER: _ClassVar[int]
     EXIT_FIELD_NUMBER: _ClassVar[int]
     POLL_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/function_pb2_grpc.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/function_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/poll_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/poll_pb2.pyi` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/poll_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.py` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/status_pb2.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/sdk/v1/status_pb2.pyi` & `dispatch_py-0.6.0/src/dispatch/sdk/v1/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/signature/digest.py` & `dispatch_py-0.6.0/src/dispatch/signature/digest.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/signature/key.py` & `dispatch_py-0.6.0/src/dispatch/signature/key.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/status.py` & `dispatch_py-0.6.0/src/dispatch/status.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/test/client.py` & `dispatch_py-0.6.0/src/dispatch/test/client.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/test/server.py` & `dispatch_py-0.6.0/src/dispatch/test/server.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/src/dispatch/test/service.py` & `dispatch_py-0.6.0/src/dispatch/test/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,14 +106,16 @@
             for call in request.calls:
                 dispatch_id = self._make_dispatch_id()
                 logger.debug("enqueueing call to function: %s", call.function)
                 resp.dispatch_ids.append(dispatch_id)
                 run_request = function_pb.RunRequest(
                     function=call.function,
                     input=call.input,
+                    dispatch_id=dispatch_id,
+                    root_dispatch_id=dispatch_id,
                 )
                 self.queue.append((dispatch_id, run_request, CallType.CALL))
 
             self._work_signal.notify()
 
         return resp
 
@@ -203,26 +205,31 @@
                 logger.info("suspending function %s", request.function)
 
                 logger.debug("registering poller %s", dispatch_id)
 
                 assert dispatch_id not in self.pollers
                 poller = Poller(
                     id=dispatch_id,
+                    parent_id=request.parent_dispatch_id,
+                    root_id=request.root_dispatch_id,
                     function=request.function,
                     coroutine_state=response.poll.coroutine_state,
                     waiting={},
                     results={},
                 )
                 self.pollers[dispatch_id] = poller
 
                 for call in response.poll.calls:
                     child_dispatch_id = self._make_dispatch_id()
                     child_request = function_pb.RunRequest(
                         function=call.function,
                         input=call.input,
+                        dispatch_id=child_dispatch_id,
+                        parent_dispatch_id=request.dispatch_id,
+                        root_dispatch_id=request.root_dispatch_id,
                     )
 
                     _next_queue.append(
                         (child_dispatch_id, child_request, CallType.CALL)
                     )
                     self.parents[child_dispatch_id] = poller
                     poller.waiting[child_dispatch_id] = call
@@ -235,14 +242,17 @@
                     logger.debug(
                         "enqueueing tail call for %s",
                         tail_call.function,
                     )
                     tail_call_request = function_pb.RunRequest(
                         function=tail_call.function,
                         input=tail_call.input,
+                        dispatch_id=request.dispatch_id,
+                        parent_dispatch_id=request.parent_dispatch_id,
+                        root_dispatch_id=request.root_dispatch_id,
                     )
                     _next_queue.append((dispatch_id, tail_call_request, CallType.CALL))
 
                 elif dispatch_id in self.parents:
                     result = response.exit.result
                     poller = self.parents[dispatch_id]
                     logger.debug(
@@ -265,14 +275,17 @@
                     if not poller.waiting:
                         logger.debug(
                             "poller %s is now ready; enqueueing delivery of %d call result(s)",
                             poller.id,
                             len(poller.results),
                         )
                         poll_results_request = function_pb.RunRequest(
+                            dispatch_id=poller.id,
+                            parent_dispatch_id=poller.parent_id,
+                            root_dispatch_id=poller.root_id,
                             function=poller.function,
                             poll_result=poll_pb.PollResult(
                                 coroutine_state=poller.coroutine_state,
                                 results=poller.results.values(),
                             ),
                         )
                         del self.pollers[poller.id]
@@ -345,14 +358,17 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
 
 
 @dataclass
 class Poller:
     id: DispatchID
+    parent_id: DispatchID
+    root_id: DispatchID
+
     function: str
 
     coroutine_state: bytes
     # TODO: support max_wait/min_results/max_results
 
     waiting: Dict[DispatchID, call_pb.Call]
     results: Dict[DispatchID, call_pb.CallResult]
```

### Comparing `dispatch-py-0.5.1/src/dispatch_py.egg-info/PKG-INFO` & `dispatch_py-0.6.0/src/dispatch_py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: dispatch-py
-Version: 0.5.1
+Version: 0.6.0
 Summary: Develop reliable distributed systems on the Dispatch platform.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: grpcio>=1.60.0
 Requires-Dist: protobuf>=4.24.0
 Requires-Dist: types-protobuf>=4.24.0.20240129
 Requires-Dist: grpc-stubs>=1.53.0.5
 Requires-Dist: http-message-signatures>=0.4.4
 Requires-Dist: tblib>=3.0.0
-Requires-Dist: docopt>=0.6.2
-Requires-Dist: types-docopt>=0.6.11.4
 Requires-Dist: httpx>=0.27.0
 Requires-Dist: typing_extensions>=4.10
 Provides-Extra: fastapi
 Requires-Dist: fastapi; extra == "fastapi"
 Requires-Dist: httpx; extra == "fastapi"
 Provides-Extra: lambda
 Requires-Dist: awslambdaric; extra == "lambda"
@@ -50,193 +48,104 @@
 [![Test](https://github.com/stealthrocket/dispatch-py/actions/workflows/test.yml/badge.svg?branch=)](https://github.com/stealthrocket/dispatch-py/actions/workflows/test.yml)
 [![PyPI version](https://badge.fury.io/py/dispatch-py.svg)](https://badge.fury.io/py/dispatch-py)
 [![Reference](https://img.shields.io/badge/API-Reference-lightblue.svg)](https://python.dispatch.run/main/reference/dispatch/)
 
 Python package to develop applications with the Dispatch platform.
 
 [fastapi]: https://fastapi.tiangolo.com/tutorial/first-steps/
-[ngrok]:   https://ngrok.com/
 [pypi]:    https://pypi.org/project/dispatch-py/
 [signup]:  https://console.dispatch.run/
 
 - [What is Dispatch?](#what-is-dispatch)
 - [Installation](#installation)
+  - [Installing the Dispatch CLI](#installing-the-dispatch-cli)
+  - [Installing the Dispatch SDK](#installing-the-dispatch-sdk)
 - [Usage](#usage)
-  - [Configuration](#configuration)
+  - [Writing Dispatch Applications](#writing-dispatch-applications)
+  - [Running Dispatch Applications](#running-dispatch-applications)
+  - [Writing Transactional Applications with Dispatch](#writing-transactional-applications-with-dispatch)
   - [Integration with FastAPI](#integration-with-fastapi)
-  - [Local Testing](#local-testing)
-  - [Distributed Coroutines for Python](#distributed-coroutines-for-python)
+  - [Configuration](#configuration)
   - [Serialization](#serialization)
 - [Examples](#examples)
 - [Contributing](#contributing)
 
 ## What is Dispatch?
 
 Dispatch is a platform for developing scalable & reliable distributed systems.
 
-Dispatch provides a simple programming model based on *Distributed Coroutines*,
-allowing complex, dynamic workflows to be expressed with regular code and
-control flow.
-
-Dispatch schedules function calls across a fleet of service instances,
-incorporating **fair scheduling**, transparent **retry of failed operations**,
-and **durability**.
-
 To get started, follow the instructions to [sign up for Dispatch][signup] 🚀.
 
 ## Installation
 
-This package is published on [PyPI][pypi] as **dispatch-py**, to install:
-```sh
-pip install dispatch-py
-```
-
-## Usage
+### Installing the Dispatch CLI
 
-The SDK allows Python applications to declare functions that Dispatch can
-orchestrate:
+As a pre-requisite, we recommend installing the Dispatch CLI to simplify the
+configuration and execution of applications that use Dispatch. On macOS, this
+can be done easily using [Homebrew](https://docs.brew.sh/):
 
-```python
-@dispatch.function
-def action(msg):
-    ...
+```console
+brew tap stealthrocket/dispatch
+brew install dispatch
 ```
 
-The **@dispatch.function** decorator declares a function that can be run by
-Dispatch. The call has durable execution semantics; if the function fails
-with a temporary error, it is automatically retried, even if the program is
-restarted, or if multiple instances are deployed.
+Alternatively, you can download the latest `dispatch` binary from the
+[Releases](https://github.com/stealthrocket/dispatch/releases) page.
 
-The SDK adds a method to the `action` object, allowing the program to
-dispatch an asynchronous invocation of the function; for example:
+*Note that this step is optional, applications that use Dispatch can run without
+the CLI, passing configuration through environment variables or directly in the
+code. However, the CLI automates the onboarding flow and simplifies the
+configuration, so we recommend starting with it.*
 
-```python
-action.dispatch('hello')
-```
-
-### Configuration
+### Installing the Dispatch SDK
 
-In order for Dispatch to interact with functions remotely, the SDK needs to be
-configured with the address at which the server can be reached. The Dispatch
-API Key must also be set, and optionally, a public signing key should be
-configured to verify that requests originated from Dispatch. These
-configuration options can be passed as arguments to the
-the `Dispatch` constructor, but by default they will be loaded from environment
-variables:
+The Python package is published on [PyPI][pypi] as **dispatch-py**, to install:
+```console
+pip install dispatch-py
+```
 
-| Environment Variable        | Value Example                      |
-| :-------------------------- | :--------------------------------- |
-| `DISPATCH_API_KEY`          | `d4caSl21a5wdx5AxMjdaMeWehaIyXVnN` |
-| `DISPATCH_ENDPOINT_URL`     | `https://service.domain.com`       |
-| `DISPATCH_VERIFICATION_KEY` | `-----BEGIN PUBLIC KEY-----...`    |
+## Usage
 
-Finally, the `Dispatch` instance needs to mount a route on a HTTP server in to
-receive requests from Dispatch. At this time, the SDK integrates with
-FastAPI; adapters for other popular Python frameworks will be added in the
-future.
+### Writing Dispatch Applications
 
-### Integration with FastAPI
+The following snippet shows how to write a very simple Dispatch application
+that does the following:
 
-The following code snippet is a complete example showing how to install a
-`Dispatch` instance on a [FastAPI][fastapi] server:
+1. declare a dispatch function named `greet` which can run asynchronously
+2. schedule a call to `greet` with the argument `World`
+3. run until all dispatched calls have completed
 
 ```python
-from fastapi import FastAPI
-from dispatch.fastapi import Dispatch
-import requests
-
-app = FastAPI()
-dispatch = Dispatch(app)
+# main.py
+import dispatch
 
 @dispatch.function
-def publish(url, payload):
-    r = requests.post(url, data=payload)
-    r.raise_for_status()
+def greet(msg: str):
+    print(f"Hello, ${msg}!")
 
-@app.get('/')
-def root():
-    publish.dispatch('https://httpstat.us/200', {'hello': 'world'})
-    return {'answer': 42}
+dispatch.run(lambda: greet.dispatch('World'))
 ```
 
-In this example, GET requests on the HTTP server dispatch calls to the
-`publish` function. The function runs concurrently to the rest of the
-program, driven by the Dispatch SDK.
-
-The instantiation of the `Dispatch` object on the `FastAPI` application
-automatically installs the HTTP route needed for Dispatch to invoke functions.
+Obviously, this is just an example, a real application would perform much more
+interesting work, but it's a good start to get a sense of how to use Dispatch.
 
-### Local Testing
-
-#### Mock Dispatch
-
-The SDK ships with a mock Dispatch server. It can be used to quickly test your
-local functions, without requiring internet access.
-
-Note that the mock Dispatch server has very limited scheduling capabilities.
+### Running Dispatch Applications
 
+The simplest way to run a Dispatch application is to use the Dispatch CLI, first
+we need to login:
 ```console
-python -m dispatch.test $DISPATCH_ENDPOINT_URL
+dispatch login
 ```
 
-The command will start a mock Dispatch server and print the configuration
-for the SDK.
-
-For example, if your functions were exposed through a local endpoint
-listening on `http://127.0.0.1:8000`, you could run:
-
+Then we are ready to run the example program we wrote above:
 ```console
-$ python -m dispatch.test http://127.0.0.1:8000
-Spawned a mock Dispatch server on 127.0.0.1:4450
-
-Dispatching function calls to the endpoint at http://127.0.0.1:8000
-
-The Dispatch SDK can be configured with:
-
-  export DISPATCH_API_URL="http://127.0.0.1:4450"
-  export DISPATCH_API_KEY="test"
-  export DISPATCH_ENDPOINT_URL="http://127.0.0.1:8000"
-  export DISPATCH_VERIFICATION_KEY="Z+nTe2VRcw8t8Ihx++D+nXtbO28nwjWIOTLRgzrelYs="
-```
-
-#### Real Dispatch
-
-To test local functions with the production instance of Dispatch, it needs
-to be able to access your local endpoint.
-
-A common approach consists of using [ngrok][ngrok] to setup a public endpoint
-that forwards to the server running on localhost.
-
-For example, assuming the server is running on port 8000 (which is the default
-with FastAPI), the command to create a ngrok tunnel is:
-```sh
-ngrok http http://localhost:8000
+dispatch run -- python3 main.py
 ```
-Running this command opens a terminal interface that looks like this:
-```
-ngrok
 
-Build better APIs with ngrok. Early access: ngrok.com/early-access
-
-Session Status                online
-Account                       Alice (Plan: Free)
-Version                       3.6.0
-Region                        United States (California) (us-cal-1)
-Latency                       -
-Web Interface                 http://127.0.0.1:4040
-Forwarding                    https://f441-2600-1700-2802-e01f-6861-dbc9-d551-ecfb.ngrok-free.app -> http://localhost:8000
-```
-To configure the Dispatch SDK, set the endpoint URL to the endpoint for the
-**Forwarding** parameter; each ngrok instance is unique, so you would have a
-different value, but in this example it would be:
-```sh
-export DISPATCH_ENDPOINT_URL="https://f441-2600-1700-2802-e01f-6861-dbc9-d551-ecfb.ngrok-free.app"
-```
-
-### Distributed Coroutines for Python
+### Writing Transactional Applications with Dispatch
 
 The `@dispatch.function` decorator can also be applied to Python coroutines
 (a.k.a. *async* functions), in which case each `await` point becomes a
 durability step in the execution. If the awaited operation fails, it is
 automatically retried, and the parent function is paused until the result are
 available or a permanent error is raised.
 
@@ -280,19 +189,75 @@
 
 @dispatch.function
 async def transform(msg):
     ...
 ```
 
 Dispatch converts Python coroutines to *Distributed Coroutines*, which can be
-suspended and resumed on any instance of a service across a fleet.
+suspended and resumed on any instance of a service across a fleet. For a deep
+dive on these concepts, read our blog post on
+[*Distributed Coroutines with a Native Python Extension and Dispatch*](https://stealthrocket.tech/blog/distributed-coroutines-in-python).
+
+### Integration with FastAPI
+
+Many web applications written in Python are developed using [FastAPI][fastapi].
+Dispatch can integrate with these applications by instantiating a
+`dispatch.fastapi.Dispatch` object. When doing so, the Dispatch functions
+declared by the program can be invoked remotely over the same HTTP interface
+used for the [FastAPI][fastapi] handlers.
+
+The following code snippet is a complete example showing how to install a
+`Dispatch` instance on a [FastAPI][fastapi] server:
+
+```python
+from fastapi import FastAPI
+from dispatch.fastapi import Dispatch
+import requests
+
+app = FastAPI()
+dispatch = Dispatch(app)
+
+@dispatch.function
+def publish(url, payload):
+    r = requests.post(url, data=payload)
+    r.raise_for_status()
+
+@app.get('/')
+def root():
+    publish.dispatch('https://httpstat.us/200', {'hello': 'world'})
+    return {'answer': 42}
+```
+
+In this example, GET requests on the HTTP server dispatch calls to the
+`publish` function. The function runs concurrently to the rest of the
+program, driven by the Dispatch SDK.
+
+### Configuration
+
+The Dispatch CLI automatically configures the SDK, so manual configuration is
+usually not required when running Dispatch applications. However, in some
+advanced cases, it might be useful to explicitly set configuration options.
+
+In order for Dispatch to interact with functions remotely, the SDK needs to be
+configured with the address at which the server can be reached. The Dispatch
+API Key must also be set, and optionally, a public signing key should be
+configured to verify that requests originated from Dispatch. These
+configuration options can be passed as arguments to the
+the `Dispatch` constructor, but by default they will be loaded from environment
+variables:
+
+| Environment Variable        | Value Example                      |
+| :-------------------------- | :--------------------------------- |
+| `DISPATCH_API_KEY`          | `d4caSl21a5wdx5AxMjdaMeWehaIyXVnN` |
+| `DISPATCH_ENDPOINT_URL`     | `https://service.domain.com`       |
+| `DISPATCH_VERIFICATION_KEY` | `-----BEGIN PUBLIC KEY-----...`    |
 
 ### Serialization
 
-Dispatch uses the [pickle] library to serialize coroutines.
+Dispatch uses the [pickle][pickle] library to serialize coroutines.
 
 [pickle]: https://docs.python.org/3/library/pickle.html
 
 Serialization of coroutines is enabled by a CPython extension.
 
 The user must ensure that the contents of their stack frames are
 serializable. That is, users should avoid using variables inside
@@ -303,15 +268,14 @@
 stacks of coroutines and generators will be printed to stdout before
 the pickle library attempts serialization.
 
 For help with a serialization issues, please submit a [GitHub issue][issues].
 
 [issues]: https://github.com/stealthrocket/dispatch-py/issues
 
-
 ## Examples
 
 Check out the [examples](examples/) directory for code samples to help you get
 started with the SDK.
 
 ## Contributing
```

### Comparing `dispatch-py-0.5.1/src/dispatch_py.egg-info/SOURCES.txt` & `dispatch_py-0.6.0/src/dispatch_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/buf/validate/priv/private_pb2.pyi
 src/buf/validate/priv/private_pb2_grpc.py
 src/dispatch/__init__.py
 src/dispatch/coroutine.py
 src/dispatch/error.py
 src/dispatch/fastapi.py
 src/dispatch/function.py
+src/dispatch/http.py
 src/dispatch/id.py
 src/dispatch/proto.py
 src/dispatch/py.typed
 src/dispatch/scheduler.py
 src/dispatch/status.py
 src/dispatch/experimental/__init__.py
 src/dispatch/experimental/lambda_handler.py
@@ -76,19 +77,19 @@
 src/dispatch/sdk/v1/status_pb2.pyi
 src/dispatch/sdk/v1/status_pb2_grpc.py
 src/dispatch/signature/__init__.py
 src/dispatch/signature/digest.py
 src/dispatch/signature/key.py
 src/dispatch/signature/request.py
 src/dispatch/test/__init__.py
-src/dispatch/test/__main__.py
 src/dispatch/test/client.py
 src/dispatch/test/server.py
 src/dispatch/test/service.py
 src/dispatch_py.egg-info/PKG-INFO
 src/dispatch_py.egg-info/SOURCES.txt
 src/dispatch_py.egg-info/dependency_links.txt
 src/dispatch_py.egg-info/requires.txt
 src/dispatch_py.egg-info/top_level.txt
 tests/test_client.py
 tests/test_fastapi.py
-tests/test_full.py
+tests/test_full.py
+tests/test_http.py
```

### Comparing `dispatch-py-0.5.1/src/dispatch_py.egg-info/requires.txt` & `dispatch_py-0.6.0/src/dispatch_py.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 grpcio>=1.60.0
 protobuf>=4.24.0
 types-protobuf>=4.24.0.20240129
 grpc-stubs>=1.53.0.5
 http-message-signatures>=0.4.4
 tblib>=3.0.0
-docopt>=0.6.2
-types-docopt>=0.6.11.4
 httpx>=0.27.0
 typing_extensions>=4.10
 
 [dev]
 black>=24.1.0
 isort>=5.13.2
 mypy>=1.8.0
```

### Comparing `dispatch-py-0.5.1/tests/test_client.py` & `dispatch_py-0.6.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dispatch-py-0.5.1/tests/test_full.py` & `dispatch_py-0.6.0/tests/test_full.py`

 * *Files identical despite different names*

