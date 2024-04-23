# Comparing `tmp/django-google-spanner-3.0.2.tar.gz` & `tmp/django-google-spanner-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-google-spanner-3.0.2.tar", last modified: Thu Aug 25 07:12:23 2022, max compression
+gzip compressed data, was "django-google-spanner-3.1.0.tar", last modified: Tue Apr 23 13:03:04 2024, max compression
```

## Comparing `django-google-spanner-3.0.2.tar` & `django-google-spanner-3.1.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.195632 django-google-spanner-3.0.2/
--rw-rw-r--   0 root         (0)     1003     1448 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/LICENSE
--rw-r--r--   0 root         (0)     1003     9112 2022-08-25 07:12:23.195632 django-google-spanner-3.0.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     8103 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.187629 django-google-spanner-3.0.2/django_google_spanner.egg-info/
--rw-r--r--   0 root         (0)     1003     9112 2022-08-25 07:12:23.000000 django-google-spanner-3.0.2/django_google_spanner.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1788 2022-08-25 07:12:23.000000 django-google-spanner-3.0.2/django_google_spanner.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-08-25 07:12:23.000000 django-google-spanner-3.0.2/django_google_spanner.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003      144 2022-08-25 07:12:23.000000 django-google-spanner-3.0.2/django_google_spanner.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       21 2022-08-25 07:12:23.000000 django-google-spanner-3.0.2/django_google_spanner.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.191630 django-google-spanner-3.0.2/django_spanner/
--rw-rw-r--   0 root         (0)     1003     3559 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1635 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/_opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003     7964 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/base.py
--rw-rw-r--   0 root         (0)     1003      509 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/client.py
--rw-rw-r--   0 root         (0)     1003     5023 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/compiler.py
--rw-rw-r--   0 root         (0)     1003     4197 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/creation.py
--rw-rw-r--   0 root         (0)     1003     1098 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/expressions.py
--rw-rw-r--   0 root         (0)     1003   184988 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/features.py
--rw-rw-r--   0 root         (0)     1003    15053 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/functions.py
--rw-rw-r--   0 root         (0)     1003    13575 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/introspection.py
--rw-rw-r--   0 root         (0)     1003    11510 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/lookups.py
--rw-rw-r--   0 root         (0)     1003    23263 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/operations.py
--rw-rw-r--   0 root         (0)     1003    21534 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/schema.py
--rw-rw-r--   0 root         (0)     1003     1351 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/django_spanner/utils.py
--rw-rw-r--   0 root         (0)     1003       30 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/pyproject.toml
--rw-rw-r--   0 root         (0)     1003      561 2022-08-25 07:12:23.195632 django-google-spanner-3.0.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2321 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.187629 django-google-spanner-3.0.2/tests/
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.191630 django-google-spanner-3.0.2/tests/performance/
--rw-rw-r--   0 root         (0)     1003      194 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/performance/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.191630 django-google-spanner-3.0.2/tests/performance/django_spanner/
--rw-rw-r--   0 root         (0)     1003      194 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/performance/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003      443 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/performance/django_spanner/models.py
--rw-rw-r--   0 root         (0)     1003     9090 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/performance/django_spanner/test_benchmark.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.191630 django-google-spanner-3.0.2/tests/system/
--rw-rw-r--   0 root         (0)     1003      194 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.191630 django-google-spanner-3.0.2/tests/system/django_spanner/
--rw-rw-r--   0 root         (0)     1003        0 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1021 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/django_spanner/models.py
--rw-rw-r--   0 root         (0)     1003     2024 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/django_spanner/test_check_constraint.py
--rw-rw-r--   0 root         (0)     1003     3402 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/django_spanner/test_decimal.py
--rw-rw-r--   0 root         (0)     1003     1576 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/django_spanner/test_json_field.py
--rw-rw-r--   0 root         (0)     1003     1521 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/django_spanner/test_queries.py
--rw-rw-r--   0 root         (0)     1003     4193 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/system/django_spanner/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.195632 django-google-spanner-3.0.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003        0 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-08-25 07:12:23.195632 django-google-spanner-3.0.2/tests/unit/django_spanner/
--rw-rw-r--   0 root         (0)     1003        0 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/__init__.py
--rw-rw-r--   0 root         (0)     1003     1557 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/models.py
--rw-rw-r--   0 root         (0)     1003     1247 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/simple_test.py
--rw-rw-r--   0 root         (0)     1003     4528 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test__opentelemetry_tracing.py
--rw-rw-r--   0 root         (0)     1003     3372 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_base.py
--rw-rw-r--   0 root         (0)     1003      528 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_client.py
--rw-rw-r--   0 root         (0)     1003     6961 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_compiler.py
--rw-rw-r--   0 root         (0)     1003     1777 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_expressions.py
--rw-rw-r--   0 root         (0)     1003     8591 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_functions.py
--rw-rw-r--   0 root         (0)     1003     8637 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_introspection.py
--rw-rw-r--   0 root         (0)     1003    15614 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_lookups.py
--rw-rw-r--   0 root         (0)     1003     8459 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_operations.py
--rw-rw-r--   0 root         (0)     1003    16626 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_schema.py
--rw-rw-r--   0 root         (0)     1003     1987 2022-08-25 07:09:43.000000 django-google-spanner-3.0.2/tests/unit/django_spanner/test_utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/
+-rw-rw-r--   0 root         (0)     1003     1448 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/LICENSE
+-rw-r--r--   0 root         (0)     1003     9380 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     8103 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/django_google_spanner.egg-info/
+-rw-r--r--   0 root         (0)     1003     9380 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1788 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003      144 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       21 2024-04-23 13:03:04.000000 django-google-spanner-3.1.0/django_google_spanner.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/django_spanner/
+-rw-rw-r--   0 root         (0)     1003     3559 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1635 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/_opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003     7964 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/base.py
+-rw-rw-r--   0 root         (0)     1003      509 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/client.py
+-rw-rw-r--   0 root         (0)     1003     5023 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/compiler.py
+-rw-rw-r--   0 root         (0)     1003     4197 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/creation.py
+-rw-rw-r--   0 root         (0)     1003     1098 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/expressions.py
+-rw-rw-r--   0 root         (0)     1003   185105 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/features.py
+-rw-rw-r--   0 root         (0)     1003    15053 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/functions.py
+-rw-rw-r--   0 root         (0)     1003    13750 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/introspection.py
+-rw-rw-r--   0 root         (0)     1003    11510 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/lookups.py
+-rw-rw-r--   0 root         (0)     1003    23263 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/operations.py
+-rw-rw-r--   0 root         (0)     1003    21797 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/schema.py
+-rw-rw-r--   0 root         (0)     1003     1350 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/django_spanner/utils.py
+-rw-rw-r--   0 root         (0)     1003       30 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/pyproject.toml
+-rw-rw-r--   0 root         (0)     1003      561 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2321 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.476238 django-google-spanner-3.1.0/tests/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/tests/performance/
+-rw-rw-r--   0 root         (0)     1003      194 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/tests/performance/django_spanner/
+-rw-rw-r--   0 root         (0)     1003      194 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003      443 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/django_spanner/models.py
+-rw-rw-r--   0 root         (0)     1003     9090 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/performance/django_spanner/test_benchmark.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.480239 django-google-spanner-3.1.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003      194 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.484239 django-google-spanner-3.1.0/tests/system/django_spanner/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1021 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/models.py
+-rw-rw-r--   0 root         (0)     1003     2024 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_check_constraint.py
+-rw-rw-r--   0 root         (0)     1003     3402 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_decimal.py
+-rw-rw-r--   0 root         (0)     1003     1576 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_json_field.py
+-rw-rw-r--   0 root         (0)     1003     1521 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/test_queries.py
+-rw-rw-r--   0 root         (0)     1003     4193 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/system/django_spanner/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.484239 django-google-spanner-3.1.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-23 13:03:04.488239 django-google-spanner-3.1.0/tests/unit/django_spanner/
+-rw-rw-r--   0 root         (0)     1003        0 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1557 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/models.py
+-rw-rw-r--   0 root         (0)     1003     1247 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/simple_test.py
+-rw-rw-r--   0 root         (0)     1003     4528 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test__opentelemetry_tracing.py
+-rw-rw-r--   0 root         (0)     1003     3372 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_base.py
+-rw-rw-r--   0 root         (0)     1003      528 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_client.py
+-rw-rw-r--   0 root         (0)     1003     6961 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_compiler.py
+-rw-rw-r--   0 root         (0)     1003     1777 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_expressions.py
+-rw-rw-r--   0 root         (0)     1003     8591 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_functions.py
+-rw-rw-r--   0 root         (0)     1003     8637 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_introspection.py
+-rw-rw-r--   0 root         (0)     1003    15614 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_lookups.py
+-rw-rw-r--   0 root         (0)     1003     8459 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_operations.py
+-rw-rw-r--   0 root         (0)     1003    16626 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_schema.py
+-rw-rw-r--   0 root         (0)     1003     1987 2024-04-23 13:00:20.000000 django-google-spanner-3.1.0/tests/unit/django_spanner/test_utils.py
```

### Comparing `django-google-spanner-3.0.2/LICENSE` & `django-google-spanner-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/PKG-INFO` & `django-google-spanner-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-google-spanner
-Version: 3.0.2
+Version: 3.1.0
 Summary: Bridge to enable using Django with Spanner.
 Home-page: https://github.com/googleapis/python-spanner-django
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,16 +18,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Requires-Python: >=3.6
-Provides-Extra: tracing
 License-File: LICENSE
+Requires-Dist: sqlparse>=0.3.0
+Requires-Dist: google-cloud-spanner>=3.13.0
+Provides-Extra: tracing
+Requires-Dist: opentelemetry-api>=1.1.0; extra == "tracing"
+Requires-Dist: opentelemetry-sdk>=1.1.0; extra == "tracing"
+Requires-Dist: opentelemetry-instrumentation>=0.20b0; extra == "tracing"
 
 Cloud Spanner support for Django
 ================================
 
 |GA| |pypi| |versions|
 
 `Cloud Spanner`_ is the world's first fully managed relational database service
```

### Comparing `django-google-spanner-3.0.2/README.rst` & `django-google-spanner-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_google_spanner.egg-info/PKG-INFO` & `django-google-spanner-3.1.0/django_google_spanner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-google-spanner
-Version: 3.0.2
+Version: 3.1.0
 Summary: Bridge to enable using Django with Spanner.
 Home-page: https://github.com/googleapis/python-spanner-django
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,16 +18,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Requires-Python: >=3.6
-Provides-Extra: tracing
 License-File: LICENSE
+Requires-Dist: sqlparse>=0.3.0
+Requires-Dist: google-cloud-spanner>=3.13.0
+Provides-Extra: tracing
+Requires-Dist: opentelemetry-api>=1.1.0; extra == "tracing"
+Requires-Dist: opentelemetry-sdk>=1.1.0; extra == "tracing"
+Requires-Dist: opentelemetry-instrumentation>=0.20b0; extra == "tracing"
 
 Cloud Spanner support for Django
 ================================
 
 |GA| |pypi| |versions|
 
 `Cloud Spanner`_ is the world's first fully managed relational database service
```

### Comparing `django-google-spanner-3.0.2/django_google_spanner.egg-info/SOURCES.txt` & `django-google-spanner-3.1.0/django_google_spanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/__init__.py` & `django-google-spanner-3.1.0/django_spanner/__init__.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/_opentelemetry_tracing.py` & `django-google-spanner-3.1.0/django_spanner/_opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/base.py` & `django-google-spanner-3.1.0/django_spanner/base.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/compiler.py` & `django-google-spanner-3.1.0/django_spanner/compiler.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/creation.py` & `django-google-spanner-3.1.0/django_spanner/creation.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/expressions.py` & `django-google-spanner-3.1.0/django_spanner/expressions.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/features.py` & `django-google-spanner-3.1.0/django_spanner/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     # TIMESTAMP.
     can_introspect_time_field = False
     closed_cursor_error_class = InterfaceError
     # Spanner uses REGEXP_CONTAINS which is case-sensitive.
     has_case_insensitive_like = False
     # https://cloud.google.com/spanner/quotas#query_limits
     max_query_params = 900
-    supports_foreign_keys = False
+    if os.environ.get("RUNNING_SPANNER_BACKEND_TESTS") == "1":
+        supports_foreign_keys = False
+    else:
+        supports_foreign_keys = True
     can_create_inline_fk = False
     supports_ignore_conflicts = False
     supports_partial_indexes = False
     supports_regex_backreferencing = False
     supports_select_for_update_with_limit = False
     supports_sequence_reset = False
     supports_timezones = False
@@ -108,14 +111,16 @@
         "timezones.tests.NewDatabaseTests.test_cursor_execute_accepts_naive_datetime",
         "timezones.tests.AdminTests.test_change_editable",
         "timezones.tests.AdminTests.test_change_editable_in_other_timezone",
         "timezones.tests.AdminTests.test_change_readonly",
         "timezones.tests.AdminTests.test_change_readonly_in_other_timezone",
         "timezones.tests.AdminTests.test_changelist",
         "timezones.tests.AdminTests.test_changelist_in_other_timezone",
+        "timezones.tests.LegacyDatabaseTests.test_cursor_execute_returns_naive_datetime",
+        "timezones.tests.NewDatabaseTests.test_cursor_execute_returns_naive_datetime",
         "validation.test_custom_messages.CustomMessagesTests.test_custom_null_message",
         "validation.test_custom_messages.CustomMessagesTests.test_custom_simple_validator_message",
         "validation.test_unique.PerformUniqueChecksTest.test_primary_key_unique_check_not_performed_when_adding_and_pk_not_specified",  # noqa
         "validation.test_unique.PerformUniqueChecksTest.test_primary_key_unique_check_not_performed_when_not_adding",
         "validation.test_validators.TestModelsWithValidators.test_custom_validator_passes_for_correct_value",
         "validation.test_validators.TestModelsWithValidators.test_custom_validator_raises_error_for_incorrect_value",
         "validation.test_validators.TestModelsWithValidators.test_field_validators_can_be_any_iterable",
@@ -495,15 +500,15 @@
         skip_tests += (
             # Emulator doesn't support views.
             "inspectdb.tests.InspectDBTransactionalTests.test_include_views",
             "introspection.tests.IntrospectionTests.test_table_names_with_views",
             # Check constraints are not supported by Spanner emulator.
             "constraints.tests.CheckConstraintTests.test_database_constraint",  # noqa
             "constraints.tests.CheckConstraintTests.test_name",  # noqa
-            "admin_docs.test_views.AdminDocViewDefaultEngineOnly.test_template_detail_path_traversal",
+            "admin_docs.test_views.AdminDocViewDefaultEngineOnly.test_template_detail_path_traversal",  # noqa
             # Untyped parameters are not supported:
             # https://github.com/GoogleCloudPlatform/cloud-spanner-emulator#features-and-limitations
             "auth_tests.test_admin_multidb.MultiDatabaseTests.test_add_view",  # noqa
             "admin_changelist.test_date_hierarchy.DateHierarchyTests.test_bounded_params",  # noqa
             "admin_changelist.test_date_hierarchy.DateHierarchyTests.test_bounded_params_with_time_zone",  # noqa
             "admin_changelist.test_date_hierarchy.DateHierarchyTests.test_invalid_params",  # noqa
             "admin_changelist.tests.ChangeListTests.test_builtin_lookup_in_search_fields",  # noqa
@@ -1339,15 +1344,14 @@
             "m2o_recursive.tests.ManyToOneRecursiveTests.test_m2o_recursive",  # noqa
             "m2o_recursive.tests.MultipleManyToOneRecursiveTests.test_m2o_recursive2",  # noqa
             "managers_regress.tests.ManagersRegressionTests.test_field_can_be_called_exact",  # noqa
             "managers_regress.tests.ManagersRegressionTests.test_regress_3871",  # noqa
             "many_to_one.tests.ManyToOneTests.test_add_after_prefetch",  # noqa
             "many_to_one.tests.ManyToOneTests.test_add_then_remove_after_prefetch",  # noqa
             "many_to_one.tests.ManyToOneTests.test_cached_foreign_key_with_to_field_not_cleared_by_save",  # noqa
-            "many_to_one.tests.ManyToOneTests.test_multiple_foreignkeys",  # noqa
             "many_to_one.tests.ManyToOneTests.test_reverse_foreign_key_instance_to_field_caching",  # noqa
             "many_to_one.tests.ManyToOneTests.test_set_after_prefetch",  # noqa
             "many_to_one_null.tests.ManyToOneNullTests.test_add_efficiency",  # noqa
             "many_to_one_null.tests.ManyToOneNullTests.test_assign_clear_related_set",  # noqa
             "many_to_one_null.tests.ManyToOneNullTests.test_assign_with_queryset",  # noqa
             "many_to_one_null.tests.ManyToOneNullTests.test_clear_efficiency",  # noqa
             "many_to_one_null.tests.ManyToOneNullTests.test_created_via_related_set",  # noqa
@@ -1505,15 +1509,14 @@
             "ordering.tests.OrderingTests.test_orders_nulls_first_on_filtered_subquery",  # noqa
             "ordering.tests.OrderingTests.test_related_ordering_duplicate_table_reference",  # noqa
             "ordering.tests.OrderingTests.test_reverse_ordering_pure",  # noqa
             "ordering.tests.OrderingTests.test_reversed_ordering",  # noqa
             "ordering.tests.OrderingTests.test_stop_slicing",  # noqa
             "ordering.tests.OrderingTests.test_stop_start_slicing",  # noqa
             "queries.test_bulk_update.BulkUpdateNoteTests.test_batch_size",  # noqa
-            "queries.test_bulk_update.BulkUpdateNoteTests.test_foreign_keys_do_not_lookup",  # noqa
             "queries.test_bulk_update.BulkUpdateNoteTests.test_functions",  # noqa
             "queries.test_bulk_update.BulkUpdateNoteTests.test_set_field_to_null",  # noqa
             "queries.test_bulk_update.BulkUpdateNoteTests.test_set_mixed_fields_to_null",  # noqa
             "queries.test_bulk_update.BulkUpdateNoteTests.test_simple",  # noqa
             "queries.test_bulk_update.BulkUpdateTests.test_custom_db_columns",  # noqa
             "queries.test_bulk_update.BulkUpdateTests.test_field_references",  # noqa
             "queries.test_bulk_update.BulkUpdateTests.test_ipaddressfield",  # noqa
```

### Comparing `django-google-spanner-3.0.2/django_spanner/functions.py` & `django-google-spanner-3.1.0/django_spanner/functions.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/introspection.py` & `django-google-spanner-3.1.0/django_spanner/introspection.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,34 +25,22 @@
         TypeCode.FLOAT64: "FloatField",
         TypeCode.INT64: "IntegerField",
         TypeCode.STRING: "CharField",
         TypeCode.TIMESTAMP: "DateTimeField",
         TypeCode.NUMERIC: "DecimalField",
         TypeCode.JSON: "JSONField",
     }
-    if USE_EMULATOR:
-        # Emulator does not support table_type yet.
-        # https://github.com/GoogleCloudPlatform/cloud-spanner-emulator/issues/43
-        LIST_TABLE_SQL = """
-            SELECT
-                t.table_name, t.table_name
-            FROM
-                information_schema.tables AS t
-            WHERE
-                t.table_catalog = '' and t.table_schema = ''
-        """
-    else:
-        LIST_TABLE_SQL = """
-            SELECT
-                t.table_name, t.table_type
-            FROM
-                information_schema.tables AS t
-            WHERE
-                t.table_catalog = '' and t.table_schema = ''
-        """
+    LIST_TABLE_SQL = """
+        SELECT
+            t.table_name, t.table_type
+        FROM
+            information_schema.tables AS t
+        WHERE
+            t.table_catalog = '' and t.table_schema = @schema_name
+    """
 
     def get_field_type(self, data_type, description):
         """A hook for a Spanner database to use the cursor description to
         match a Django field type to the database column.
 
         :type data_type: int
         :param data_type: One of Spanner's standard data types.
@@ -72,15 +60,18 @@
 
         :type cursor: :class:`~google.cloud.spanner_dbapi.cursor.Cursor`
         :param cursor: A reference to a Spanner Database cursor.
 
         :rtype: list
         :returns: A list of table and view names in the current database.
         """
-        results = cursor.run_sql_in_snapshot(self.LIST_TABLE_SQL)
+        schema_name = self._get_schema_name(cursor)
+        results = cursor.run_sql_in_snapshot(
+            self.LIST_TABLE_SQL, params={"schema_name": schema_name}
+        )
         tables = []
         # The second TableInfo field is 't' for table or 'v' for view.
         for row in results:
             table_type = "t"
             if row[1] == "VIEW":
                 table_type = "v"
             tables.append(TableInfo(row[0], table_type))
@@ -155,31 +146,33 @@
 
         :type table_name: str
         :param table_name: The name of the Cloud Spanner Database.
 
         :rtype: dict
         :returns: A dictionary representing column relationships to other tables.
         """
+        schema_name = self._get_schema_name(cursor)
         results = cursor.run_sql_in_snapshot(
-            '''
+            """
             SELECT
                 tc.COLUMN_NAME as col, ccu.COLUMN_NAME as ref_col, ccu.TABLE_NAME as ref_table
             FROM
                 INFORMATION_SCHEMA.KEY_COLUMN_USAGE AS tc
             JOIN
                 INFORMATION_SCHEMA.REFERENTIAL_CONSTRAINTS as rc
             ON
                 tc.CONSTRAINT_NAME = rc.CONSTRAINT_NAME
             JOIN
                 INFORMATION_SCHEMA.CONSTRAINT_COLUMN_USAGE as ccu
             ON
                 rc.UNIQUE_CONSTRAINT_NAME = ccu.CONSTRAINT_NAME
             WHERE
-                tc.TABLE_NAME="%s"'''
-            % self.connection.ops.quote_name(table_name)
+                tc.TABLE_SCHEMA=@schema_name AND tc.TABLE_NAME=@view_name
+            """,
+            params={"schema_name": schema_name, "view_name": table_name},
         )
         return {
             column: (referred_column, referred_table)
             for (column, referred_column, referred_table) in results
         }
 
     def get_primary_key_column(self, cursor, table_name):
@@ -190,28 +183,29 @@
 
         :type table_name: str
         :param table_name: The name of the table.
 
         :rtype: str
         :returns: The name of the PK column.
         """
+        schema_name = self._get_schema_name(cursor)
         results = cursor.run_sql_in_snapshot(
             """
             SELECT
                 ccu.COLUMN_NAME
             FROM
                 INFORMATION_SCHEMA.TABLE_CONSTRAINTS as tc
             RIGHT JOIN
                 INFORMATION_SCHEMA.KEY_COLUMN_USAGE
             AS
                 ccu ON tc.CONSTRAINT_NAME = ccu.CONSTRAINT_NAME
             WHERE
-                tc.TABLE_NAME="%s" AND tc.CONSTRAINT_TYPE='PRIMARY KEY' AND tc.TABLE_SCHEMA=''
-            """
-            % self.connection.ops.quote_name(table_name)
+                tc.TABLE_NAME=@table_name AND tc.CONSTRAINT_TYPE='PRIMARY KEY' AND tc.TABLE_SCHEMA=@schema_name
+            """,
+            params={"schema_name": schema_name, "table_name": table_name},
         )
         return results[0][0] if results else None
 
     def get_constraints(self, cursor, table_name):
         """Retrieve the Spanner Table column constraints.
 
         :type cursor: :class:`~google.cloud.spanner_dbapi.cursor.Cursor`
@@ -220,26 +214,25 @@
         :type table_name: str
         :param table_name: The name of the table.
 
         :rtype: dict
         :returns: A dictionary with constraints.
         """
         constraints = {}
-        quoted_table_name = self.connection.ops.quote_name(table_name)
+        schema_name = self._get_schema_name(cursor)
 
         # Firstly populate all available constraints and their columns.
         constraint_columns = cursor.run_sql_in_snapshot(
-            '''
+            """
             SELECT
                 CONSTRAINT_NAME, COLUMN_NAME
             FROM
                 INFORMATION_SCHEMA.CONSTRAINT_COLUMN_USAGE
-               WHERE TABLE_NAME="{table}"'''.format(
-                table=quoted_table_name
-            )
+               WHERE TABLE_NAME=@table AND TABLE_SCHEMA=@schema_name""",
+            params={"table": table_name, "schema_name": schema_name},
         )
         for constraint, column_name in constraint_columns:
             if constraint not in constraints:
                 constraints[constraint] = {
                     "check": False,
                     "columns": [],
                     "foreign_key": None,
@@ -250,23 +243,22 @@
                     "unique": False,
                 }
 
             constraints[constraint]["columns"].append(column_name)
 
         # Add the various constraints by type.
         constraint_types = cursor.run_sql_in_snapshot(
-            '''
+            """
             SELECT
                 CONSTRAINT_NAME, CONSTRAINT_TYPE
             FROM
                 INFORMATION_SCHEMA.TABLE_CONSTRAINTS
             WHERE
-                TABLE_NAME="{table}"'''.format(
-                table=quoted_table_name
-            )
+                TABLE_NAME=@table AND TABLE_SCHEMA=@schema_name""",
+            params={"table": table_name, "schema_name": schema_name},
         )
         for constraint, constraint_type in constraint_types:
             already_added = constraint in constraints
             if constraint_type == "FOREIGN KEY":
                 # We don't yet support anything related to FOREIGN KEY.
                 # See https://github.com/googleapis/python-spanner-django/issues/313.
                 if already_added:
@@ -299,22 +291,21 @@
             SELECT
                 idx.INDEX_NAME, idx_col.COLUMN_NAME, idx_col.COLUMN_ORDERING, idx.INDEX_TYPE, idx.IS_UNIQUE
             FROM
                 INFORMATION_SCHEMA.INDEXES AS idx
             RIGHT JOIN
                 INFORMATION_SCHEMA.INDEX_COLUMNS AS idx_col
             ON
-                idx_col.INDEX_NAME = idx.INDEX_NAME AND idx_col.TABLE_NAME="{table}"
+                idx_col.INDEX_NAME = idx.INDEX_NAME AND idx_col.TABLE_NAME=@table AND idx_col.TABLE_SCHEMA=idx.TABLE_SCHEMA
             WHERE
-                idx.TABLE_NAME="{table}"
+                idx.TABLE_NAME=@table AND idx.TABLE_SCHEMA=@schema_name
             ORDER BY
                 idx_col.ORDINAL_POSITION
-            """.format(
-                table=quoted_table_name
-            )
+            """,
+            params={"table": table_name, "schema_name": schema_name},
         )
         for (
             index_name,
             column_name,
             ordering,
             index_type,
             is_unique,
@@ -346,14 +337,15 @@
 
     def get_key_columns(self, cursor, table_name):
         """
         Return a list of (column_name, referenced_table, referenced_column)
         for all key columns in the given table.
         """
         key_columns = []
+        schema_name = self._get_schema_name(cursor)
         cursor.execute(
             """SELECT
                 tc.COLUMN_NAME as column_name,
                 ccu.TABLE_NAME as referenced_table,
                 ccu.COLUMN_NAME as referenced_column
             FROM
                 INFORMATION_SCHEMA.KEY_COLUMN_USAGE AS tc
@@ -362,14 +354,16 @@
             ON
                 tc.CONSTRAINT_NAME = rc.CONSTRAINT_NAME
             JOIN
                 INFORMATION_SCHEMA.CONSTRAINT_COLUMN_USAGE as ccu
             ON
                 rc.CONSTRAINT_NAME = ccu.CONSTRAINT_NAME
             WHERE
-                tc.TABLE_NAME="{table}"
-            """.format(
-                table=self.connection.ops.quote_name(table_name)
-            )
+                tc.TABLE_NAME=@table AND tc.TABLE_SCHEMA=@schema_name
+            """,
+            params={"table": table_name, "schema_name": schema_name},
         )
         key_columns.extend(cursor.fetchall())
         return key_columns
+
+    def _get_schema_name(self, cursor):
+        return cursor.connection.current_schema
```

### Comparing `django-google-spanner-3.0.2/django_spanner/lookups.py` & `django-google-spanner-3.1.0/django_spanner/lookups.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/operations.py` & `django-google-spanner-3.1.0/django_spanner/operations.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/django_spanner/schema.py` & `django-google-spanner-3.1.0/django_spanner/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2020 Google LLC
 #
 # Use of this source code is governed by a BSD-style
 # license that can be found in the LICENSE file or at
 # https://developers.google.com/open-source/licenses/bsd
-
+import os
 import uuid
+
 from django.db import NotSupportedError
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 from django_spanner._opentelemetry_tracing import trace_call
 from django_spanner import USE_EMULATOR, USING_DJANGO_3
 
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
@@ -17,15 +18,21 @@
     “delete a field” into SQL.
     """
 
     sql_create_table = (
         "CREATE TABLE %(table)s (%(definition)s) PRIMARY KEY(%(primary_key)s)"
     )
     sql_delete_table = "DROP TABLE %(table)s"
-    sql_create_fk = None
+    if os.environ.get("RUNNING_SPANNER_BACKEND_TESTS") == "1":
+        sql_create_fk = None
+    else:
+        sql_create_fk = (
+            "ALTER TABLE %(table)s ADD CONSTRAINT %(name)s FOREIGN KEY (%(column)s) "
+            "REFERENCES %(to_table)s (%(to_column)s)"
+        )
     # Spanner doesn't support partial indexes. This string omits the
     # %(condition)s placeholder so that partial indexes are ignored.
     sql_create_index = (
         "CREATE INDEX %(name)s ON %(table)s%(using)s (%(columns)s)%(extra)s"
     )
     sql_create_unique = (
         "CREATE UNIQUE NULL_FILTERED INDEX %(name)s ON %(table)s (%(columns)s)"
```

### Comparing `django-google-spanner-3.0.2/django_spanner/utils.py` & `django-google-spanner-3.1.0/django_spanner/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,9 +38,8 @@
     :returns: A SQL statement with dummy WHERE clause.
     """
     if any(
         isinstance(token, sqlparse.sql.Where)
         for token in sqlparse.parse(sql)[0]
     ):
         return sql
-
     return sql + " WHERE 1=1"
```

### Comparing `django-google-spanner-3.0.2/setup.cfg` & `django-google-spanner-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/setup.py` & `django-google-spanner-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/performance/django_spanner/test_benchmark.py` & `django-google-spanner-3.1.0/tests/performance/django_spanner/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/system/django_spanner/models.py` & `django-google-spanner-3.1.0/tests/system/django_spanner/models.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/system/django_spanner/test_check_constraint.py` & `django-google-spanner-3.1.0/tests/system/django_spanner/test_check_constraint.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/system/django_spanner/test_decimal.py` & `django-google-spanner-3.1.0/tests/system/django_spanner/test_decimal.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/system/django_spanner/test_json_field.py` & `django-google-spanner-3.1.0/tests/system/django_spanner/test_json_field.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/system/django_spanner/test_queries.py` & `django-google-spanner-3.1.0/tests/system/django_spanner/test_queries.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/system/django_spanner/utils.py` & `django-google-spanner-3.1.0/tests/system/django_spanner/utils.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/models.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/models.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/simple_test.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/simple_test.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test__opentelemetry_tracing.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test__opentelemetry_tracing.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_base.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_base.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_client.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_client.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_compiler.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_compiler.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_expressions.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_expressions.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_functions.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_functions.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_introspection.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_introspection.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_lookups.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_lookups.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_operations.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_operations.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_schema.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_schema.py`

 * *Files identical despite different names*

### Comparing `django-google-spanner-3.0.2/tests/unit/django_spanner/test_utils.py` & `django-google-spanner-3.1.0/tests/unit/django_spanner/test_utils.py`

 * *Files identical despite different names*

