# Comparing `tmp/ecv-python-development-0.0.24.tar.gz` & `tmp/ecv-python-development-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecv-python-development-0.0.24.tar", last modified: Tue Apr 23 19:40:29 2024, max compression
+gzip compressed data, was "ecv-python-development-0.0.25.tar", last modified: Tue Apr 23 20:53:55 2024, max compression
```

## Comparing `ecv-python-development-0.0.24.tar` & `ecv-python-development-0.0.25.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/LICENSE
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/MANIFEST.in
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/README.md
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.846895 ecv-python-development-0.0.24/ecv_python_development/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.846895 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.846895 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/events_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/events_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/events_module/base.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.846895 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/handler.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/logger.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/response.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3447 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/validator.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/aws_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/cognito_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/exceptions.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/kms_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/lambda_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/s3_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/ses_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/sns_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/sqs_service.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/ssm_service.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/database/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.24/ecv_python_development/database/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/database/_pynamodb/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.24/ecv_python_development/database/_pynamodb/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.24/ecv_python_development/database/_pynamodb/base.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5817 2024-04-23 19:38:03.000000 ecv-python-development-0.0.24/ecv_python_development/database/base_model.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/database/py.typed
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1131 2024-04-23 19:37:40.000000 ecv-python-development-0.0.24/ecv_python_development/database/test.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/helpers/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/__init__.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/helpers/datetime/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/datetime/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/datetime/standard.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/helpers/debugger/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/debugger/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      128 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/debugger/debugging.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/helpers/files/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/files/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/files/file.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/helpers/formatter/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/formatter/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/formatter/formatter.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/formatter/regex.py
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/helpers/http/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/http/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/http/requests.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/ecv_python_development/helpers/strings/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/strings/__init__.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/strings/passwords.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/helpers/strings/uuid.py
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.24/ecv_python_development/py.typed
-drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 19:40:29.846895 ecv-python-development-0.0.24/ecv_python_development.egg-info/
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-23 19:40:29.000000 ecv-python-development-0.0.24/ecv_python_development.egg-info/PKG-INFO
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-23 19:40:29.000000 ecv-python-development-0.0.24/ecv_python_development.egg-info/SOURCES.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-23 19:40:29.000000 ecv-python-development-0.0.24/ecv_python_development.egg-info/dependency_links.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-23 19:40:29.000000 ecv-python-development-0.0.24/ecv_python_development.egg-info/requires.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-23 19:40:29.000000 ecv-python-development-0.0.24/ecv_python_development.egg-info/top_level.txt
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-23 19:40:29.856895 ecv-python-development-0.0.24/setup.cfg
--rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-23 19:40:09.000000 ecv-python-development-0.0.24/setup.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.686633 ecv-python-development-0.0.25/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1082 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/LICENSE
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       39 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/MANIFEST.in
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-23 20:53:55.686633 ecv-python-development-0.0.25/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      297 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/README.md
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.656633 ecv-python-development-0.0.25/ecv_python_development/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.656633 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      420 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.656633 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/events_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       53 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/events_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3065 2024-04-22 17:56:33.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/events_module/base.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.656633 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      846 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1231 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1583 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/handler.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      406 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/logger.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      255 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/metrics.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1471 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/response.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      109 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/tracer.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3447 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/validator.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.666633 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      169 2024-04-22 17:59:36.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      616 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/aws_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     4599 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/cognito_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     7693 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/dynamodb_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      683 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/eventbridge_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       87 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/exceptions.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      986 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/kms_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1452 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/lambda_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2339 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/s3_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      806 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1090 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/ses_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      578 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/sns_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3232 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/sqs_service.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      830 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/ssm_service.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.666633 ecv-python-development-0.0.25/ecv_python_development/database/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      267 2024-04-23 12:38:43.000000 ecv-python-development-0.0.25/ecv_python_development/database/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.676633 ecv-python-development-0.0.25/ecv_python_development/database/_pynamodb/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      121 2024-04-23 10:40:28.000000 ecv-python-development-0.0.25/ecv_python_development/database/_pynamodb/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      486 2024-04-23 10:36:40.000000 ecv-python-development-0.0.25/ecv_python_development/database/_pynamodb/base.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     5751 2024-04-23 20:19:19.000000 ecv-python-development-0.0.25/ecv_python_development/database/base_model.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/database/py.typed
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1213 2024-04-23 20:20:42.000000 ecv-python-development-0.0.25/ecv_python_development/database/test.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.676633 ecv-python-development-0.0.25/ecv_python_development/helpers/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      308 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/__init__.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.676633 ecv-python-development-0.0.25/ecv_python_development/helpers/datetime/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       55 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/datetime/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2458 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/datetime/standard.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.676633 ecv-python-development-0.0.25/ecv_python_development/helpers/debugger/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       48 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/debugger/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      128 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/debugger/debugging.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.676633 ecv-python-development-0.0.25/ecv_python_development/helpers/files/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       43 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/files/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      477 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/files/file.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.676633 ecv-python-development-0.0.25/ecv_python_development/helpers/formatter/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      576 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/formatter/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     2658 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/formatter/formatter.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      149 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/formatter/regex.py
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.676633 ecv-python-development-0.0.25/ecv_python_development/helpers/http/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      111 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/http/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      729 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/http/requests.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.686633 ecv-python-development-0.0.25/ecv_python_development/helpers/strings/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      123 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/strings/__init__.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      932 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/strings/passwords.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       71 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/helpers/strings/uuid.py
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-22 17:32:49.000000 ecv-python-development-0.0.25/ecv_python_development/py.typed
+drwxr-xr-x   0 webpjaudian  (1000) webpjaudian  (1000)        0 2024-04-23 20:53:55.656633 ecv-python-development-0.0.25/ecv_python_development.egg-info/
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      698 2024-04-23 20:53:55.000000 ecv-python-development-0.0.25/ecv_python_development.egg-info/PKG-INFO
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     3025 2024-04-23 20:53:55.000000 ecv-python-development-0.0.25/ecv_python_development.egg-info/SOURCES.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)        1 2024-04-23 20:53:55.000000 ecv-python-development-0.0.25/ecv_python_development.egg-info/dependency_links.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)      592 2024-04-23 20:53:55.000000 ecv-python-development-0.0.25/ecv_python_development.egg-info/requires.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       23 2024-04-23 20:53:55.000000 ecv-python-development-0.0.25/ecv_python_development.egg-info/top_level.txt
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)       38 2024-04-23 20:53:55.686633 ecv-python-development-0.0.25/setup.cfg
+-rw-r--r--   0 webpjaudian  (1000) webpjaudian  (1000)     1708 2024-04-23 20:53:53.000000 ecv-python-development-0.0.25/setup.py
```

### Comparing `ecv-python-development-0.0.24/LICENSE` & `ecv-python-development-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/PKG-INFO` & `ecv-python-development-0.0.25/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.24
+Version: 0.0.25
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/events_module/base.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/events_module/base.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/__init__.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/exceptions.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/handler.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/handler.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/response.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/response.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/lambda_module/validator.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/lambda_module/validator.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/aws_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/aws_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/cognito_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/cognito_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/dynamodb_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/dynamodb_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/eventbridge_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/eventbridge_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/kms_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/kms_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/lambda_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/lambda_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/s3_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/s3_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/secretsmanager_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/ses_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/ses_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/sns_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/sns_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/sqs_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/sqs_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/aws_cloud_native/services/ssm_service.py` & `ecv-python-development-0.0.25/ecv_python_development/aws_cloud_native/services/ssm_service.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/database/base_model.py` & `ecv-python-development-0.0.25/ecv_python_development/database/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import annotations
 
 import os
-from typing import Any, Callable, List, Literal, Optional, Pattern
+from typing import Any, Callable, ClassVar, List, Literal, Optional, Pattern
 
+from _pynamodb.base import (
+    PYDANTIC_PYNAMO_MAPPING,
+    PynamoDBBaseModel,
+    PynamoDBModel,
+    UnicodeAttribute,
+)
+from ecv_python_development.helpers.datetime import DateTime
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic import (
     Field,
     PrivateAttr,
     StrictBool,
     StrictFloat,
     StrictInt,
     StrictStr,
     create_model,
 )
 
-from ..helpers.datetime import DateTime
-from ._pynamodb.base import (
-    PYDANTIC_PYNAMO_MAPPING,
-    PynamoDBBaseModel,
-    PynamoDBModel,
-    UnicodeAttribute,
-)
-
 """
 check full documentation for fields at: https://docs.pydantic.dev/latest/concepts/fields/
 
 """
 
 
 def field(
@@ -113,17 +112,15 @@
         db_type: Literal["dynamodb", "rds", "mongodb", "temporary"] = "dynamodb",
         table_name: Optional[str] = os.environ.get("METADATA_TABLE", None),
         **data,
     ):
         super().__init__(**data)
 
         if db_type == "dynamodb":
-            self.__PynamoDBModel__: PynamoDBModel = self.get_pynamodb_model(
-                table_name=table_name
-            )
+            pass
         elif db_type == "temporary":
             pass
         else:
             raise Exception("Other database not yet supported")
 
     @classmethod
     def get_pynamodb_model(cls, table_name: Optional[str] = None):
@@ -142,15 +139,15 @@
                     field_info.annotation, UnicodeAttribute
                 )(null=field_info.exclude)
 
         model_name = f"{cls.__name__}PynamoDBModel"
         PynamoDBBaseModel.Meta.table_name = table_name
         PynamoDBModel = type(model_name, (PynamoDBBaseModel,), attributes)
 
-        return PynamoDBModel
+        cls.__PynamoDBModel__ = PynamoDBModel
 
     def to_pynamodb_model(
         self, include: Optional[list | str] = "all", exclude: Optional[list] = []
     ) -> PynamoDBBaseModel:
         return self.__PynamoDBModel__(
             **self.model_serialize(
                 include=include,
```

### Comparing `ecv-python-development-0.0.24/ecv_python_development/database/test.py` & `ecv-python-development-0.0.25/ecv_python_development/database/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-from base_model import BaseModel, field
+from base_model import BaseModel, ClassVar, field
 
 
 class UserModel(BaseModel):
     username: str = field(min_length=1, is_hash_key=True)
     email: str = field(min_length=1, is_range_key=True)
     datetime: str = field(pattern=r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$")
     test_frozen: str = field(default="", alias="test_frozen", frozen=True)
     new_field: str = field(validation_alias="check", serialization_alias="serial")
     updated_by: str = field(exclude=True)
 
+    __PynamoDBModel__: ClassVar = None
+
 
 user_data = {
     "username": "john_doe",
     "email": "john@example.com",
     "datetime": "2012-12-01 02:01:02",
     "check": "1",
     "created_by": "a",
     "updated_by": "a",
     "non_defined": "test",
 }
+
+UserModel.get_pynamodb_model()
 temp_model = UserModel.transform(include=["username"])
 temp = temp_model(database="dynamodb", table_name="test", **user_data)
 print(temp)
 print(temp.get_pynamodb_model())
 pydantic_user = UserModel(database="dynamodb", table_name="test", **user_data)
 print(pydantic_user)
 pynamo_db_model = pydantic_user.to_pynamodb_model()
```

### Comparing `ecv-python-development-0.0.24/ecv_python_development/helpers/datetime/standard.py` & `ecv-python-development-0.0.25/ecv_python_development/helpers/datetime/standard.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/helpers/formatter/__init__.py` & `ecv-python-development-0.0.25/ecv_python_development/helpers/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/helpers/formatter/formatter.py` & `ecv-python-development-0.0.25/ecv_python_development/helpers/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/helpers/http/requests.py` & `ecv-python-development-0.0.25/ecv_python_development/helpers/http/requests.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development/helpers/strings/passwords.py` & `ecv-python-development-0.0.25/ecv_python_development/helpers/strings/passwords.py`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development.egg-info/PKG-INFO` & `ecv-python-development-0.0.25/ecv_python_development.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecv-python-development
-Version: 0.0.24
+Version: 0.0.25
 Summary: ECV Python Development Package
 Home-page: https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development
 Author: Warren Ezra Bruce Jaudian
 Author-email: warren.jaudian@ecloudvalley.com
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `ecv-python-development-0.0.24/ecv_python_development.egg-info/SOURCES.txt` & `ecv-python-development-0.0.25/ecv_python_development.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecv-python-development-0.0.24/ecv_python_development.egg-info/requires.txt` & `ecv-python-development-0.0.25/ecv_python_development.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 mypy-boto3-lambda
 mypy-boto3-s3
 mypy-boto3-secretsmanager
 mypy-boto3-ses
 mypy-boto3-sns
 mypy-boto3-sqs
 mypy-boto3-ssm
-pydantic==2.6.1
+pydantic==2.7.1
 pydantic[email]
 pynamodb==6.0.0
 pytz==2022.7
 requests
 typing_extensions
```

### Comparing `ecv-python-development-0.0.24/setup.py` & `ecv-python-development-0.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setup(
     name="ecv-python-development",
-    version="0.0.24",
+    version="0.0.25",
     author="Warren Ezra Bruce Jaudian",
     author_email="warren.jaudian@ecloudvalley.com",
     packages=find_packages(),
     description="ECV Python Development Package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://git-codecommit.ap-southeast-1.amazonaws.com/v1/repos/ecv-python-development",
     license="MIT",
     python_requires=">=3.8",
     install_requires=[
         "aws-lambda-powertools",
         "pytz==2022.7",
         "aws_encryption_sdk",
-        "pydantic==2.6.1",
+        "pydantic==2.7.1",
         "pynamodb==6.0.0",
         "pydantic[email]",
         "requests",
         "cerberus",
         "jsonpickle",
         "typing_extensions",
         "mypy-boto3-cognito-idp",
```

