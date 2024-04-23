# Comparing `tmp/ecv-python-development-0.0.8.tar.gz` & `tmp/ecv-python-development-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecv-python-development-0.0.8.tar", last modified: Mon Feb 19 05:03:28 2024, max compression
+gzip compressed data, was "ecv-python-development-0.0.9.tar", last modified: Mon Feb 19 05:20:10 2024, max compression
```

## Comparing `ecv-python-development-0.0.8.tar` & `ecv-python-development-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/LICENSE
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/MANIFEST.in
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      734 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-02-18 09:40:20.000000 ecv-python-development-0.0.8/README.md
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-02-18 09:21:58.000000 ecv-python-development-0.0.8/ecv_python_development/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-02-18 09:36:14.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/events_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/events_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3064 2024-02-18 09:25:31.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/events_module/base.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-02-19 04:43:35.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1404 2024-02-19 05:02:30.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/handler.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/logger.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-02-18 09:56:43.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/response.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3395 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/validator.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      659 2024-02-18 09:33:25.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      627 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/aws_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4610 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/cognito_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7722 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/kms_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1463 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/lambda_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2350 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/s3_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1100 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/ses_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/sns_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3243 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/sqs_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      841 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/ssm_service.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/database/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-02-18 09:30:49.000000 ecv-python-development-0.0.8/ecv_python_development/database/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/database/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/helpers/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-02-18 09:29:51.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/helpers/datetime/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/datetime/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-02-18 09:57:37.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/datetime/standard.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/helpers/debugger/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/debugger/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      128 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/debugger/debugging.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/helpers/files/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/files/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/files/file.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/helpers/formatter/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/formatter/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/formatter/formatter.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/formatter/regex.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/helpers/http/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/http/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      739 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/http/requests.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development/helpers/strings/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/strings/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/strings/passwords.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/helpers/strings/uuid.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-18 09:20:16.000000 ecv-python-development-0.0.8/ecv_python_development/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/ecv_python_development.egg-info/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      734 2024-02-19 05:03:28.000000 ecv-python-development-0.0.8/ecv_python_development.egg-info/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2835 2024-02-19 05:03:28.000000 ecv-python-development-0.0.8/ecv_python_development.egg-info/SOURCES.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-02-19 05:03:28.000000 ecv-python-development-0.0.8/ecv_python_development.egg-info/dependency_links.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      569 2024-02-19 05:03:28.000000 ecv-python-development-0.0.8/ecv_python_development.egg-info/requires.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-02-19 05:03:28.000000 ecv-python-development-0.0.8/ecv_python_development.egg-info/top_level.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-02-19 05:03:28.773315 ecv-python-development-0.0.8/setup.cfg
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1638 2024-02-19 05:02:47.000000 ecv-python-development-0.0.8/setup.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/LICENSE
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/MANIFEST.in
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      734 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-02-18 09:40:20.000000 ecv-python-development-0.0.9/README.md
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-02-18 09:21:58.000000 ecv-python-development-0.0.9/ecv_python_development/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-02-18 09:36:14.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/events_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/events_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3064 2024-02-18 09:25:31.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/events_module/base.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-02-19 04:43:35.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1404 2024-02-19 05:02:30.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/handler.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/logger.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-02-18 09:56:43.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/response.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3395 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/validator.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      659 2024-02-18 09:33:25.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      627 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/aws_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4610 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/cognito_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7722 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/kms_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1463 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/lambda_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2350 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/s3_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1100 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/ses_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/sns_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3243 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/sqs_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      841 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/ssm_service.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/database/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      217 2024-02-19 05:11:38.000000 ecv-python-development-0.0.9/ecv_python_development/database/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/database/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/database/pydantic/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      118 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/database/pydantic/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1493 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/database/pydantic/base.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/helpers/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-02-18 09:29:51.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/helpers/datetime/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/datetime/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-02-18 09:57:37.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/datetime/standard.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/helpers/debugger/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/debugger/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      128 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/debugger/debugging.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/helpers/files/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/files/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/files/file.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/helpers/formatter/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/formatter/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/formatter/formatter.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/formatter/regex.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/helpers/http/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/http/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      739 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/http/requests.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development/helpers/strings/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/strings/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/strings/passwords.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/helpers/strings/uuid.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-18 09:20:16.000000 ecv-python-development-0.0.9/ecv_python_development/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-02-19 05:20:10.173309 ecv-python-development-0.0.9/ecv_python_development.egg-info/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      734 2024-02-19 05:20:10.000000 ecv-python-development-0.0.9/ecv_python_development.egg-info/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2937 2024-02-19 05:20:10.000000 ecv-python-development-0.0.9/ecv_python_development.egg-info/SOURCES.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-02-19 05:20:10.000000 ecv-python-development-0.0.9/ecv_python_development.egg-info/dependency_links.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      569 2024-02-19 05:20:10.000000 ecv-python-development-0.0.9/ecv_python_development.egg-info/requires.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-02-19 05:20:10.000000 ecv-python-development-0.0.9/ecv_python_development.egg-info/top_level.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-02-19 05:20:10.183309 ecv-python-development-0.0.9/setup.cfg
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1673 2024-02-19 05:16:46.000000 ecv-python-development-0.0.9/setup.py
```

### Comparing `ecv-python-development-0.0.8/LICENSE` & `ecv-python-development-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/PKG-INFO` & `ecv-python-development-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.8
+Version: 0.0.9
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Description: # ECV Python Development Package
```

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/events_module/base.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/events_module/base.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/__init__.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/handler.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/handler.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/response.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/response.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/lambda_module/validator.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/lambda_module/validator.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/__init__.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/aws_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/aws_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/cognito_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/cognito_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/dynamodb_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/eventbridge_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/eventbridge_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/kms_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/kms_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/lambda_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/s3_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/s3_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/ses_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/ses_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/sns_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/sns_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/sqs_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/aws_cloud_native/services/ssm_service.py` & `ecv-python-development-0.0.9/ecv_python_development/aws_cloud_native/services/ssm_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/helpers/datetime/standard.py` & `ecv-python-development-0.0.9/ecv_python_development/helpers/datetime/standard.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/helpers/formatter/__init__.py` & `ecv-python-development-0.0.9/ecv_python_development/helpers/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/helpers/formatter/formatter.py` & `ecv-python-development-0.0.9/ecv_python_development/helpers/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/helpers/http/requests.py` & `ecv-python-development-0.0.9/ecv_python_development/helpers/http/requests.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development/helpers/strings/passwords.py` & `ecv-python-development-0.0.9/ecv_python_development/helpers/strings/passwords.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/ecv_python_development.egg-info/PKG-INFO` & `ecv-python-development-0.0.9/ecv_python_development.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.8
+Version: 0.0.9
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Description: # ECV Python Development Package
```

### Comparing `ecv-python-development-0.0.8/ecv_python_development.egg-info/SOURCES.txt` & `ecv-python-development-0.0.9/ecv_python_development.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
 ecv_python_development/aws_cloud_native/services/ses_service.py
 ecv_python_development/aws_cloud_native/services/sns_service.py
 ecv_python_development/aws_cloud_native/services/sqs_service.py
 ecv_python_development/aws_cloud_native/services/ssm_service.py
 ecv_python_development/database/__init__.py
 ecv_python_development/database/py.typed
+ecv_python_development/database/pydantic/__init__.py
+ecv_python_development/database/pydantic/base.py
 ecv_python_development/helpers/__init__.py
 ecv_python_development/helpers/py.typed
 ecv_python_development/helpers/datetime/__init__.py
 ecv_python_development/helpers/datetime/standard.py
 ecv_python_development/helpers/debugger/__init__.py
 ecv_python_development/helpers/debugger/debugging.py
 ecv_python_development/helpers/files/__init__.py
```

### Comparing `ecv-python-development-0.0.8/ecv_python_development.egg-info/requires.txt` & `ecv-python-development-0.0.9/ecv_python_development.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.8/setup.py` & `ecv-python-development-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="ecv-python-development",
-    version="0.0.8",
+    version="0.0.9",
     author="Warren Ezra Bruce Jaudian",
     author_email="warren.jaudian@ecloudvalley.com",
     packages=find_packages(),
     description="ECV Python Development Package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development",
@@ -47,10 +47,13 @@
         "boto3-stubs[lambda]",
         "boto3-stubs[events]",
         "boto3-stubs[kms]",
         "boto3-stubs[s3]",
         "boto3-stubs[dynamodb]",
     ],
     package_data={
-        "ecv_python_development": ["ecv_python_development/*", "py.typed"],
+        "ecv_python_development": [
+            "ecv_python_development/*",
+            "py.typed",
+        ],
     },
 )
```

