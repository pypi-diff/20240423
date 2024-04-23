# Comparing `tmp/django-pydantic-field-0.3.7.tar.gz` & `tmp/django_pydantic_field-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pydantic-field-0.3.7.tar", last modified: Mon Apr  1 08:24:31 2024, max compression
+gzip compressed data, was "django_pydantic_field-0.3.8.tar", last modified: Tue Apr 23 13:46:24 2024, max compression
```

## Comparing `django-pydantic-field-0.3.7.tar` & `django_pydantic_field-0.3.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.783787 django-pydantic-field-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-01 08:24:31.783787 django-pydantic-field-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.775787 django-pydantic-field-0.3.7/django_pydantic_field/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/_migration_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.775787 django-pydantic-field-0.3.7/django_pydantic_field/compat/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/compat/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/compat/django.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/compat/functools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/compat/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/compat/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/compat/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/forms.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/rest_framework.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.775787 django-pydantic-field-0.3.7/django_pydantic_field/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v1/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v1/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v1/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v1/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v1/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.779787 django-pydantic-field-0.3.7/django_pydantic_field/v2/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11038 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.779787 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/coreapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/django_pydantic_field/v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.779787 django-pydantic-field-0.3.7/django_pydantic_field.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-01 08:24:31.000000 django-pydantic-field-0.3.7/django_pydantic_field.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-01 08:24:31.000000 django-pydantic-field-0.3.7/django_pydantic_field.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 08:24:31.000000 django-pydantic-field-0.3.7/django_pydantic_field.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-01 08:24:31.000000 django-pydantic-field-0.3.7/django_pydantic_field.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 08:24:31.000000 django-pydantic-field-0.3.7/django_pydantic_field.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 08:24:31.783787 django-pydantic-field-0.3.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 08:24:31.779787 django-pydantic-field-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/tests/test_e2e_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/tests/test_migration_serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/tests/test_model_admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-01 08:24:21.000000 django-pydantic-field-0.3.7/tests/test_sample_app_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.165186 django_pydantic_field-0.3.8/django_pydantic_field/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/_migration_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.165186 django_pydantic_field-0.3.8/django_pydantic_field/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/functools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/compat/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/forms.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/rest_framework.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.169186 django_pydantic_field-0.3.8/django_pydantic_field/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v1/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.169186 django_pydantic_field-0.3.8/django_pydantic_field/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.169186 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/coreapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/django_pydantic_field/v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12985 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 13:46:24.000000 django_pydantic_field-0.3.8/django_pydantic_field.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:46:24.173186 django_pydantic_field-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_e2e_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_migration_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_model_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-23 13:46:17.000000 django_pydantic_field-0.3.8/tests/test_sample_app_migrations.py
```

### Comparing `django-pydantic-field-0.3.7/LICENSE` & `django_pydantic_field-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/PKG-INFO` & `django_pydantic_field-0.3.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.3.7
+Version: 0.3.8
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2024 Savva Surenkov and django-pydantic-field contributors.
         See the contributors at https://github.com/surenkov/django-pydantic-field/contributors
         
@@ -62,27 +62,29 @@
 Requires-Dist: django<6,>=3.1
 Requires-Dist: typing_extensions
 Provides-Extra: openapi
 Requires-Dist: uritemplate; extra == "openapi"
 Requires-Dist: inflection; extra == "openapi"
 Provides-Extra: coreapi
 Requires-Dist: coreapi; extra == "coreapi"
+Provides-Extra: jsonform
+Requires-Dist: django_jsonform<3,>=2.0; extra == "jsonform"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: djangorestframework<4,>=3.11; extra == "dev"
 Requires-Dist: django-stubs[compatible-mypy]~=4.2; extra == "dev"
 Requires-Dist: djangorestframework-stubs[compatible-mypy]~=3.14; extra == "dev"
 Requires-Dist: pytest-django<5,>=4.5; extra == "dev"
 Provides-Extra: test
-Requires-Dist: django_pydantic_field[coreapi,openapi]; extra == "test"
+Requires-Dist: django_pydantic_field[coreapi,jsonform,openapi]; extra == "test"
 Requires-Dist: dj-database-url~=2.0; extra == "test"
 Requires-Dist: djangorestframework<4,>=3; extra == "test"
 Requires-Dist: pyyaml; extra == "test"
 Requires-Dist: syrupy<5,>=3; extra == "test"
 Provides-Extra: ci
 Requires-Dist: psycopg[binary]<4,>=3.1; python_version >= "3.9" and extra == "ci"
 Requires-Dist: psycopg2-binary<3,>=2.7; python_version < "3.9" and extra == "ci"
@@ -130,15 +132,15 @@
     bar_list: typing.Sequence[Bar] = SchemaField(schema=list[Bar])
 
     # Pydantic exportable types are supported
     raw_date_map: dict[int, date] = SchemaField()
     raw_uids: set[UUID] = SchemaField()
 
 ...
-    
+
 model = MyModel(
     foo_field={"count": "5"},
     bar_list=[{}],
     raw_date_map={1: "1970-01-01"},
     raw_uids={"17a25db0-27a4-11ed-904a-5ffb17f92734"}
 )
 model.save()
@@ -209,35 +211,63 @@
 assert form.is_valid()
 assert form.cleaned_data["field"] == Foo(slug="asdf")
 ```
 
 `django_pydantic_field` also supports auto-generated fields for `ModelForm` and `modelform_factory`:
 
 ``` python
-class FooModelForm(forms.ModelForm):
+class MyModelForm(forms.ModelForm):
     class Meta:
-        model = Foo
-        fields = ["field"]
+        model = MyModel
+        fields = ["foo_field"]
 
-form = FooModelForm(data={"field": '{"slug": "asdf"}'})
+form = MyModelForm(data={"foo_field": '{"count": 5}'})
 assert form.is_valid()
-assert form.cleaned_data["field"] == Foo(slug="asdf")
+assert form.cleaned_data["foo_field"] == Foo(count=5)
 
 ...
 
 # ModelForm factory support
-AnotherFooModelForm = modelform_factory(Foo, fields=["field"])
-form = AnotherFooModelForm(data={"field": '{"slug": "bar_baz"}'})
+AnotherModelForm = modelform_factory(MyModel, fields=["foo_field"])
+form = AnotherModelForm(data={"foo_field": '{"count": 5}'})
 
 assert form.is_valid()
-assert form.cleaned_data["field"] == Foo(slug="bar_baz")
+assert form.cleaned_data["foo_field"] == Foo(count=5)
 ```
 
 Note, that forward references would be resolved until field is being bound to the form instance.
 
+### `django-jsonform` widgets
+[`django-jsonform`](https://django-jsonform.readthedocs.io) offers a dynamic form construction based on the specified JSONSchema.
+`django_pydantic_field.forms.SchemaField` plays nicely with its widgets, but only for Pydantic v2:
+
+``` python
+from django_pydantic_field.forms import SchemaField
+from django_jsonform.widgets import JSONFormWidget
+
+class FooForm(forms.Form):
+    field = SchemaField(Foo, widget=JSONFormWidget)
+```
+
+It is also possible to override the default form widget for Django Admin site, without writing custom admin forms:
+
+``` python
+from django.contrib import admin
+from django_jsonform.widgets import JSONFormWidget
+
+# NOTE: Importing direct field class instead of `SchemaField` wrapper.
+from django_pydantic_field.v2.fields import PydanticSchemaField
+
+@admin.site.register(MyModel)
+class MyModelAdmin(admin.ModelAdmin):
+    formfield_overrides = {
+        PydanticSchemaField: {"widget": JSONFormWidget},
+    }
+```
+
 ## Django REST Framework support
 
 ``` python
 from rest_framework import generics, serializers
 from django_pydantic_field.rest_framework import SchemaField, AutoSchema
 
 
@@ -299,8 +329,7 @@
 1. Install the project and its dependencies: `pip install -e .[dev,test]`;
 1. Setup `pre-commit`: `pre-commit install`.
 
 ## Acknowledgement
 
 * [Churkin Oleg](https://gist.github.com/Bahus/98a9848b1f8e2dcd986bf9f05dbf9c65) for his Gist as a source of inspiration;
 * Boutique Air Flight Operations platform as a test ground;
-
```

### Comparing `django-pydantic-field-0.3.7/README.md` & `django_pydantic_field-0.3.8/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     bar_list: typing.Sequence[Bar] = SchemaField(schema=list[Bar])
 
     # Pydantic exportable types are supported
     raw_date_map: dict[int, date] = SchemaField()
     raw_uids: set[UUID] = SchemaField()
 
 ...
-    
+
 model = MyModel(
     foo_field={"count": "5"},
     bar_list=[{}],
     raw_date_map={1: "1970-01-01"},
     raw_uids={"17a25db0-27a4-11ed-904a-5ffb17f92734"}
 )
 model.save()
@@ -119,35 +119,63 @@
 assert form.is_valid()
 assert form.cleaned_data["field"] == Foo(slug="asdf")
 ```
 
 `django_pydantic_field` also supports auto-generated fields for `ModelForm` and `modelform_factory`:
 
 ``` python
-class FooModelForm(forms.ModelForm):
+class MyModelForm(forms.ModelForm):
     class Meta:
-        model = Foo
-        fields = ["field"]
+        model = MyModel
+        fields = ["foo_field"]
 
-form = FooModelForm(data={"field": '{"slug": "asdf"}'})
+form = MyModelForm(data={"foo_field": '{"count": 5}'})
 assert form.is_valid()
-assert form.cleaned_data["field"] == Foo(slug="asdf")
+assert form.cleaned_data["foo_field"] == Foo(count=5)
 
 ...
 
 # ModelForm factory support
-AnotherFooModelForm = modelform_factory(Foo, fields=["field"])
-form = AnotherFooModelForm(data={"field": '{"slug": "bar_baz"}'})
+AnotherModelForm = modelform_factory(MyModel, fields=["foo_field"])
+form = AnotherModelForm(data={"foo_field": '{"count": 5}'})
 
 assert form.is_valid()
-assert form.cleaned_data["field"] == Foo(slug="bar_baz")
+assert form.cleaned_data["foo_field"] == Foo(count=5)
 ```
 
 Note, that forward references would be resolved until field is being bound to the form instance.
 
+### `django-jsonform` widgets
+[`django-jsonform`](https://django-jsonform.readthedocs.io) offers a dynamic form construction based on the specified JSONSchema.
+`django_pydantic_field.forms.SchemaField` plays nicely with its widgets, but only for Pydantic v2:
+
+``` python
+from django_pydantic_field.forms import SchemaField
+from django_jsonform.widgets import JSONFormWidget
+
+class FooForm(forms.Form):
+    field = SchemaField(Foo, widget=JSONFormWidget)
+```
+
+It is also possible to override the default form widget for Django Admin site, without writing custom admin forms:
+
+``` python
+from django.contrib import admin
+from django_jsonform.widgets import JSONFormWidget
+
+# NOTE: Importing direct field class instead of `SchemaField` wrapper.
+from django_pydantic_field.v2.fields import PydanticSchemaField
+
+@admin.site.register(MyModel)
+class MyModelAdmin(admin.ModelAdmin):
+    formfield_overrides = {
+        PydanticSchemaField: {"widget": JSONFormWidget},
+    }
+```
+
 ## Django REST Framework support
 
 ``` python
 from rest_framework import generics, serializers
 from django_pydantic_field.rest_framework import SchemaField, AutoSchema
 
 
@@ -209,8 +237,7 @@
 1. Install the project and its dependencies: `pip install -e .[dev,test]`;
 1. Setup `pre-commit`: `pre-commit install`.
 
 ## Acknowledgement
 
 * [Churkin Oleg](https://gist.github.com/Bahus/98a9848b1f8e2dcd986bf9f05dbf9c65) for his Gist as a source of inspiration;
 * Boutique Air Flight Operations platform as a test ground;
-
```

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/compat/deprecation.py` & `django_pydantic_field-0.3.8/django_pydantic_field/compat/deprecation.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/compat/django.py` & `django_pydantic_field-0.3.8/django_pydantic_field/compat/django.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/compat/imports.py` & `django_pydantic_field-0.3.8/django_pydantic_field/compat/imports.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/fields.pyi` & `django_pydantic_field-0.3.8/django_pydantic_field/fields.pyi`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/forms.pyi` & `django_pydantic_field-0.3.8/django_pydantic_field/forms.pyi`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/rest_framework.pyi` & `django_pydantic_field-0.3.8/django_pydantic_field/rest_framework.pyi`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v1/base.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v1/base.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v1/fields.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v1/fields.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v1/forms.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v1/forms.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v1/rest_framework.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v1/rest_framework.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v1/utils.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v1/utils.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/fields.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 class PydanticSchemaField(JSONField, ty.Generic[types.ST]):
     descriptor_class: type[DeferredAttribute] = SchemaAttribute
     adapter: types.SchemaAdapter
 
     def __init__(
         self,
         *args,
-        schema: type[types.ST] | BaseContainer | ty.ForwardRef | str | None = None,
+        schema: type[types.ST] | te.Annotated[type[types.ST], ...] | BaseContainer | ty.ForwardRef | str | None = None,
         config: pydantic.ConfigDict | None = None,
         **kwargs,
     ):
         kwargs.setdefault("encoder", DjangoJSONEncoder)
         self.export_kwargs = export_kwargs = types.SchemaAdapter.extract_export_kwargs(kwargs)
         super().__init__(*args, **kwargs)
 
@@ -112,21 +112,20 @@
         try:
             # Test that the schema could be resolved in runtime, even if it contains forward references.
             self.adapter.validate_schema()
         except types.ImproperlyConfiguredSchema as exc:
             message = f"Cannot resolve the schema. Original error: \n{exc.args[0]}"
             performed_checks.append(checks.Error(message, obj=self, id="pydantic.E001"))
 
-        if self.has_default():
-            try:
-                # Test that the default value conforms to the schema.
-                self.get_prep_value(self.get_default())
-            except pydantic.ValidationError as exc:
-                message = f"Default value cannot be adapted to the schema. Pydantic error: \n{str(exc)}"
-                performed_checks.append(checks.Error(message, obj=self, id="pydantic.E002"))
+        try:
+            # Test that the default value conforms to the schema.
+            self.get_prep_value(self.get_default())
+        except pydantic.ValidationError as exc:
+            message = f"Default value cannot be adapted to the schema. Pydantic error: \n{str(exc)}"
+            performed_checks.append(checks.Error(message, obj=self, id="pydantic.E002"))
 
         if {"include", "exclude"} & self.export_kwargs.keys():
             # Try to prepare the default value to test export ability against it.
             schema_default = self.get_default()
             if schema_default is None:
                 # If the default value is not set, try to get the default value from the schema.
                 prep_value = self.adapter.get_default_value()
```

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/__init__.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/coreapi.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/coreapi.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/fields.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/fields.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/mixins.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/mixins.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/openapi.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/openapi.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/parsers.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/rest_framework/renderers.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/types.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/types.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field/v2/utils.py` & `django_pydantic_field-0.3.8/django_pydantic_field/v2/utils.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field.egg-info/PKG-INFO` & `django_pydantic_field-0.3.8/django_pydantic_field.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pydantic-field
-Version: 0.3.7
+Version: 0.3.8
 Summary: Django JSONField with Pydantic models as a Schema
 Author-email: Savva Surenkov <savva@surenkov.space>
 License: MIT License
         
         Copyright (c) 2024 Savva Surenkov and django-pydantic-field contributors.
         See the contributors at https://github.com/surenkov/django-pydantic-field/contributors
         
@@ -62,27 +62,29 @@
 Requires-Dist: django<6,>=3.1
 Requires-Dist: typing_extensions
 Provides-Extra: openapi
 Requires-Dist: uritemplate; extra == "openapi"
 Requires-Dist: inflection; extra == "openapi"
 Provides-Extra: coreapi
 Requires-Dist: coreapi; extra == "coreapi"
+Provides-Extra: jsonform
+Requires-Dist: django_jsonform<3,>=2.0; extra == "jsonform"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest~=7.4; extra == "dev"
 Requires-Dist: djangorestframework<4,>=3.11; extra == "dev"
 Requires-Dist: django-stubs[compatible-mypy]~=4.2; extra == "dev"
 Requires-Dist: djangorestframework-stubs[compatible-mypy]~=3.14; extra == "dev"
 Requires-Dist: pytest-django<5,>=4.5; extra == "dev"
 Provides-Extra: test
-Requires-Dist: django_pydantic_field[coreapi,openapi]; extra == "test"
+Requires-Dist: django_pydantic_field[coreapi,jsonform,openapi]; extra == "test"
 Requires-Dist: dj-database-url~=2.0; extra == "test"
 Requires-Dist: djangorestframework<4,>=3; extra == "test"
 Requires-Dist: pyyaml; extra == "test"
 Requires-Dist: syrupy<5,>=3; extra == "test"
 Provides-Extra: ci
 Requires-Dist: psycopg[binary]<4,>=3.1; python_version >= "3.9" and extra == "ci"
 Requires-Dist: psycopg2-binary<3,>=2.7; python_version < "3.9" and extra == "ci"
@@ -130,15 +132,15 @@
     bar_list: typing.Sequence[Bar] = SchemaField(schema=list[Bar])
 
     # Pydantic exportable types are supported
     raw_date_map: dict[int, date] = SchemaField()
     raw_uids: set[UUID] = SchemaField()
 
 ...
-    
+
 model = MyModel(
     foo_field={"count": "5"},
     bar_list=[{}],
     raw_date_map={1: "1970-01-01"},
     raw_uids={"17a25db0-27a4-11ed-904a-5ffb17f92734"}
 )
 model.save()
@@ -209,35 +211,63 @@
 assert form.is_valid()
 assert form.cleaned_data["field"] == Foo(slug="asdf")
 ```
 
 `django_pydantic_field` also supports auto-generated fields for `ModelForm` and `modelform_factory`:
 
 ``` python
-class FooModelForm(forms.ModelForm):
+class MyModelForm(forms.ModelForm):
     class Meta:
-        model = Foo
-        fields = ["field"]
+        model = MyModel
+        fields = ["foo_field"]
 
-form = FooModelForm(data={"field": '{"slug": "asdf"}'})
+form = MyModelForm(data={"foo_field": '{"count": 5}'})
 assert form.is_valid()
-assert form.cleaned_data["field"] == Foo(slug="asdf")
+assert form.cleaned_data["foo_field"] == Foo(count=5)
 
 ...
 
 # ModelForm factory support
-AnotherFooModelForm = modelform_factory(Foo, fields=["field"])
-form = AnotherFooModelForm(data={"field": '{"slug": "bar_baz"}'})
+AnotherModelForm = modelform_factory(MyModel, fields=["foo_field"])
+form = AnotherModelForm(data={"foo_field": '{"count": 5}'})
 
 assert form.is_valid()
-assert form.cleaned_data["field"] == Foo(slug="bar_baz")
+assert form.cleaned_data["foo_field"] == Foo(count=5)
 ```
 
 Note, that forward references would be resolved until field is being bound to the form instance.
 
+### `django-jsonform` widgets
+[`django-jsonform`](https://django-jsonform.readthedocs.io) offers a dynamic form construction based on the specified JSONSchema.
+`django_pydantic_field.forms.SchemaField` plays nicely with its widgets, but only for Pydantic v2:
+
+``` python
+from django_pydantic_field.forms import SchemaField
+from django_jsonform.widgets import JSONFormWidget
+
+class FooForm(forms.Form):
+    field = SchemaField(Foo, widget=JSONFormWidget)
+```
+
+It is also possible to override the default form widget for Django Admin site, without writing custom admin forms:
+
+``` python
+from django.contrib import admin
+from django_jsonform.widgets import JSONFormWidget
+
+# NOTE: Importing direct field class instead of `SchemaField` wrapper.
+from django_pydantic_field.v2.fields import PydanticSchemaField
+
+@admin.site.register(MyModel)
+class MyModelAdmin(admin.ModelAdmin):
+    formfield_overrides = {
+        PydanticSchemaField: {"widget": JSONFormWidget},
+    }
+```
+
 ## Django REST Framework support
 
 ``` python
 from rest_framework import generics, serializers
 from django_pydantic_field.rest_framework import SchemaField, AutoSchema
 
 
@@ -299,8 +329,7 @@
 1. Install the project and its dependencies: `pip install -e .[dev,test]`;
 1. Setup `pre-commit`: `pre-commit install`.
 
 ## Acknowledgement
 
 * [Churkin Oleg](https://gist.github.com/Bahus/98a9848b1f8e2dcd986bf9f05dbf9c65) for his Gist as a source of inspiration;
 * Boutique Air Flight Operations platform as a test ground;
-
```

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field.egg-info/SOURCES.txt` & `django_pydantic_field-0.3.8/django_pydantic_field.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/django_pydantic_field.egg-info/requires.txt` & `django_pydantic_field-0.3.8/django_pydantic_field.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 pre-commit
 pytest~=7.4
 djangorestframework<4,>=3.11
 django-stubs[compatible-mypy]~=4.2
 djangorestframework-stubs[compatible-mypy]~=3.14
 pytest-django<5,>=4.5
 
+[jsonform]
+django_jsonform<3,>=2.0
+
 [openapi]
 uritemplate
 inflection
 
 [test]
-django_pydantic_field[coreapi,openapi]
+django_pydantic_field[coreapi,jsonform,openapi]
 dj-database-url~=2.0
 djangorestframework<4,>=3
 pyyaml
 syrupy<5,>=3
```

### Comparing `django-pydantic-field-0.3.7/pyproject.toml` & `django_pydantic_field-0.3.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-pydantic-field"
-version = "0.3.7"
+version = "0.3.8"
 description = "Django JSONField with Pydantic models as a Schema"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Savva Surenkov", email = "savva@surenkov.space" },
 ]
 
@@ -46,28 +46,29 @@
     "django>=3.1,<6",
     "typing_extensions",
 ]
 
 [project.optional-dependencies]
 openapi = ["uritemplate", "inflection"]
 coreapi = ["coreapi"]
+jsonform = ["django_jsonform>=2.0,<3"]
 dev = [
     "build",
     "black",
     "isort",
     "mypy",
     "pre-commit",
     "pytest~=7.4",
     "djangorestframework>=3.11,<4",
     "django-stubs[compatible-mypy]~=4.2",
     "djangorestframework-stubs[compatible-mypy]~=3.14",
     "pytest-django>=4.5,<5",
 ]
 test = [
-    "django_pydantic_field[openapi,coreapi]",
+    "django_pydantic_field[openapi,coreapi,jsonform]",
     "dj-database-url~=2.0",
     "djangorestframework>=3,<4",
     "pyyaml",
     "syrupy>=3,<5",
 ]
 ci = [
     'psycopg[binary]>=3.1,<4; python_version>="3.9"',
@@ -104,15 +105,14 @@
 
 [tool.mypy]
 plugins = [
     "mypy_django_plugin.main",
     "mypy_drf_plugin.main"
 ]
 exclude = [".env", ".venv", "tests"]
-enable_incomplete_feature = ["Unpack"]
 
 [tool.django-stubs]
 django_settings_module = "tests.settings.django_test_settings"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.settings.django_test_settings"
```

### Comparing `django-pydantic-field-0.3.7/tests/test_e2e_models.py` & `django_pydantic_field-0.3.8/tests/test_e2e_models.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/tests/test_fields.py` & `django_pydantic_field-0.3.8/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/tests/test_imports.py` & `django_pydantic_field-0.3.8/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/tests/test_migration_serializers.py` & `django_pydantic_field-0.3.8/tests/test_migration_serializers.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/tests/test_model_admin.py` & `django_pydantic_field-0.3.8/tests/test_model_admin.py`

 * *Files identical despite different names*

### Comparing `django-pydantic-field-0.3.7/tests/test_sample_app_migrations.py` & `django_pydantic_field-0.3.8/tests/test_sample_app_migrations.py`

 * *Files identical despite different names*

