# Comparing `tmp/python_dev_utils-1.3.1.tar.gz` & `tmp/python_dev_utils-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.3.1.tar", last modified: Fri Apr 19 13:44:52 2024, max compression
+gzip compressed data, was "python_dev_utils-1.4.0.tar", last modified: Tue Apr 23 09:10:19 2024, max compression
```

## Comparing `python_dev_utils-1.3.1.tar` & `python_dev_utils-1.4.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.3.1/LICENCE
--rw-r--r--   0        0        0     4373 2024-04-15 09:42:56.043729 python_dev_utils-1.3.1/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.3.1/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.3.1/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.3.1/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.3.1/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.3.1/dev_utils/core/results.py
--rw-r--r--   0        0        0      215 2024-04-16 09:16:58.960481 python_dev_utils-1.3.1/dev_utils/core/utils/__init__.py
--rw-r--r--   0        0        0      293 2024-04-16 09:15:43.772084 python_dev_utils-1.3.1/dev_utils/core/utils/datetime.py
--rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.3.1/dev_utils/core/utils/inspect.py
--rw-r--r--   0        0        0      209 2024-04-16 09:13:36.355106 python_dev_utils-1.3.1/dev_utils/core/utils/text.py
--rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.3.1/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.3.1/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/handlers.py
--rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.3.1/dev_utils/py.typed
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.3.1/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0     2349 2024-04-16 10:07:40.662627 python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/pydantic.py
--rw-r--r--   0        0        0    12968 2024-04-19 13:44:02.168069 python_dev_utils-1.3.1/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     3113 2024-04-19 13:44:52.349383 python_dev_utils-1.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.3.1/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/core/test_abstract.py
--rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.3.1/tests/core/test_guards.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/core/test_results.py
--rw-r--r--   0        0        0     1278 2024-04-16 09:18:12.890888 python_dev_utils-1.3.1/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.3.1/tests/fastapi/__init__.py
--rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.3.1/tests/fastapi/conftest.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions_handlers.py
--rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions_utils.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.3.1/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.3.1/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.3.1/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.3.1/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0     2103 2024-04-17 07:02:19.144904 python_dev_utils-1.3.1/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     7086 2024-04-16 09:18:34.220718 python_dev_utils-1.3.1/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.3.1/tests/types.py
--rw-r--r--   0        0        0     7726 2024-04-16 09:37:08.400872 python_dev_utils-1.3.1/tests/utils.py
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 python_dev_utils-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.4.0/LICENCE
+-rw-r--r--   0        0        0     5120 2024-04-23 09:09:42.701197 python_dev_utils-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.4.0/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.4.0/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.4.0/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.4.0/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.4.0/dev_utils/core/results.py
+-rw-r--r--   0        0        0      215 2024-04-16 09:16:58.960481 python_dev_utils-1.4.0/dev_utils/core/utils/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-16 09:15:43.772084 python_dev_utils-1.4.0/dev_utils/core/utils/datetime.py
+-rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.4.0/dev_utils/core/utils/inspect.py
+-rw-r--r--   0        0        0      209 2024-04-16 09:13:36.355106 python_dev_utils-1.4.0/dev_utils/core/utils/text.py
+-rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.4.0/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.4.0/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.4.0/dev_utils/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.4.0/dev_utils/fastapi/openapi/exporter.py
+-rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0     3474 2024-04-22 09:15:05.523504 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/constants.py
+-rw-r--r--   0        0        0    12499 2024-04-22 09:09:07.827456 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0     3724 2024-04-22 13:05:32.395150 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py
+-rw-r--r--   0        0        0     2184 2024-04-22 12:42:55.028588 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/openapi_override.py
+-rw-r--r--   0        0        0     1265 2024-04-22 09:31:33.905990 python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.4.0/dev_utils/py.typed
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.4.0/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16338 2024-04-16 06:54:27.234711 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.4.0/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-16 07:24:43.054226 python_dev_utils-1.4.0/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0    12968 2024-04-23 07:39:23.870346 python_dev_utils-1.4.0/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     3222 2024-04-23 09:10:19.654825 python_dev_utils-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.4.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.4.0/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/core/test_results.py
+-rw-r--r--   0        0        0     1278 2024-04-16 09:18:12.890888 python_dev_utils-1.4.0/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.4.0/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0     1409 2024-04-22 12:43:33.722241 python_dev_utils-1.4.0/tests/fastapi/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions_handlers.py
+-rw-r--r--   0        0        0     1609 2024-04-22 13:12:15.337384 python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions_utils.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.4.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.4.0/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.4.0/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.4.0/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0     1423 2024-04-22 12:17:27.599234 python_dev_utils-1.4.0/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     7531 2024-04-23 07:55:54.751248 python_dev_utils-1.4.0/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.4.0/tests/types.py
+-rw-r--r--   0        0        0     7568 2024-04-22 12:17:42.133100 python_dev_utils-1.4.0/tests/utils.py
+-rw-r--r--   0        0        0     5823 1970-01-01 00:00:00.000000 python_dev_utils-1.4.0/PKG-INFO
```

### Comparing `python_dev_utils-1.3.1/LICENCE` & `python_dev_utils-1.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/README.md` & `python_dev_utils-1.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 
 For FastAPI verbose HTTP exceptions:
 
 ```bash
 pip install "python-dev-utils[fastapi_exceptions]"
 ```
 
+For extract OpenAPI cli.
+
+```bash
+pip install "python-dev-utils[extract_openapi]"
+```
+
 ## Profiling
 
 Profiling utils. Now available 2 profilers and 2 middlewares (FastAPI) for such profilers:
 
 1. SQLAlchemyQueryProfiler - profile entire sqlalchemy query - it text, params, duration.
 2. SQLAlchemyQueryCounter - count sqlalchemy queries.
 
@@ -201,7 +207,28 @@
             "message": "Field required",
             "attr": "b",
             "location": "query",
         }
     ]
 }
 ```
+
+`apply_all_handler` function also has `override_422_openapi` param (default True). You can turn
+it off to avoid overriding 422 errors in your application OpenAPI schema.
+
+## Export OpenAPI
+
+If you want to export your OpenAPI schema from FastAPI application via CLI, you can use
+OpenAPI exporter from this package.
+
+```bash
+python3 -m dev_utils.fastapi.openapi.exporter \
+    "main:app" \
+    --app-dir "my/path/to/main" \
+    --out "custom_name.json"
+```
+
+CLI params:
+
+- `"main:app"` - path to app with format "file_name:name_of_app_var"
+- `--app-dir`  - directory of app file contains.
+- `--out`      - custom file name and format (JSON and YAML available).
```

### Comparing `python_dev_utils-1.3.1/dev_utils/core/abstract.py` & `python_dev_utils-1.4.0/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/core/exc.py` & `python_dev_utils-1.4.0/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/core/guards.py` & `python_dev_utils-1.4.0/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/core/logging.py` & `python_dev_utils-1.4.0/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/core/results.py` & `python_dev_utils-1.4.0/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/core/utils/inspect.py` & `python_dev_utils-1.4.0/dev_utils/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/fastapi/__init__.py` & `python_dev_utils-1.4.0/dev_utils/fastapi/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-1.4.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/__init__.py` & `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/exc.py` & `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/exc.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 from string import Template
 from typing import Any, NotRequired, Self, TypedDict
 
 from fastapi import HTTPException, status
 
 from dev_utils.core.abstract import Abstract, abstract_class_property
 from dev_utils.core.utils import get_object_class_absolute_name
-
-ABSTRACT_PROPERTY_DEFAULT_VALUE = "<abstract property>"
-ABSTRACT_CLS_DEFAULT_VALUE = "<class with abstract properties>"
+from dev_utils.fastapi.verbose_http_exceptions.constants import (
+    ABSTRACT_CLS_DEFAULT_VALUE,
+    ABSTRACT_PROPERTY_DEFAULT_VALUE,
+)
 
 
 class VerboseHTTPExceptionDict(TypedDict):
     """TypedDict for verbose http exceptions."""
 
     code: str
     type: str  # noqa: A003
@@ -308,15 +309,15 @@
 class NestedErrorsMainHTTPException(BaseVerboseHTTPException):
     """Main verbose response with nested errors."""
 
     __skip_abstract_raise_error__ = True
 
     code = "multiple"
     type_ = "multiple"
-    message = "Multiple exceptions ocurred. Please check list for details."
+    message = "Multiple errors ocurred. Please check list for nested_errors."
 
 
 class InfoVerboseHTTPException(BaseVerboseHTTPException):
     """Base info verbose response."""
 
     __skip_abstract_raise_error__ = True
```

### Comparing `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/handlers.py` & `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/handlers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,31 @@
 """Handlers for FastAPI."""
 
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING
 
 from fastapi import FastAPI, HTTPException, status
 from fastapi.exceptions import RequestValidationError
 from fastapi.responses import JSONResponse, Response
 
 from dev_utils.core.guards import all_dict_keys_are_str
+from dev_utils.fastapi.verbose_http_exceptions.constants import ERROR_MAPPING
 from dev_utils.fastapi.verbose_http_exceptions.exc import (
     BaseVerboseHTTPException,
     NestedErrorsMainHTTPException,
     RequestValidationVerboseHTTPException,
 )
-from dev_utils.fastapi.verbose_http_exceptions.utils import resolve_error_location_and_attr
+from dev_utils.fastapi.verbose_http_exceptions.openapi_override import (
+    override_422_error,
+)
+from dev_utils.fastapi.verbose_http_exceptions.utils import validation_error_from_error_dict
 
 if TYPE_CHECKING:
     from fastapi import Request
 
 
-INFO_START_DIGIT = 1
-SUCCESS_START_DIGIT = 2
-REDIRECT_START_DIGIT = 3
-CLIENT_ERROR_START_DIGIT = 4
-SERVER_ERROR_START_DIGIT = 5
-error_mapping: dict[int, dict[str, Any]] = {
-    INFO_START_DIGIT: {
-        "code": "info",
-        "type": "info",
-        "location": None,
-        "attr": None,
-    },
-    SUCCESS_START_DIGIT: {
-        "code": "success",
-        "type": "success",
-        "location": None,
-        "attr": None,
-    },
-    REDIRECT_START_DIGIT: {
-        "code": "redirect",
-        "type": "redirect",
-        "location": None,
-        "attr": None,
-    },
-    CLIENT_ERROR_START_DIGIT: {
-        "code": "client_error",
-        "type": "client_error",
-        "location": None,
-        "attr": None,
-    },
-    SERVER_ERROR_START_DIGIT: {
-        "code": "server_error",
-        "type": "server_error",
-        "location": None,
-        "attr": None,
-    },
-}
-
-
 async def verbose_http_exception_handler(
     _: "Request",
     exc: "BaseVerboseHTTPException",
 ) -> "Response":
     """Handle verbose HTTP exception output.
 
     Handle only BaseVerboseHTTPException inherited instances. For handling all exceptions use
@@ -72,26 +37,25 @@
 async def verbose_request_validation_error_handler(
     _: "Request",
     exc: "RequestValidationError",
 ) -> "Response":
     """Handle RequestValidationError to override 422 error."""
     main_error = NestedErrorsMainHTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY)
     nested_errors: list[RequestValidationVerboseHTTPException] = []
+    errors = exc.errors()
+    if len(errors) == 1:  # pragma: no coverage
+        error = errors[0]
+        return JSONResponse(
+            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+            content=validation_error_from_error_dict(error).as_dict(),
+        )
     for error in exc.errors():
         if not isinstance(error, dict) or not all_dict_keys_are_str(error):  # type: ignore  # pragma: no coverage
             continue
-        location, attribute = resolve_error_location_and_attr(error)
-        nested_errors.append(
-            RequestValidationVerboseHTTPException(
-                type_=error.get("type") or "not_known_type",
-                message=error.get("msg") or "not_known_message",
-                location=location,
-                attr_name=attribute,
-            ),
-        )
+        nested_errors.append(validation_error_from_error_dict(error))
     return JSONResponse(
         status_code=main_error.status_code,
         content=main_error.as_dict(nested_errors=nested_errors),
     )
 
 
 async def any_http_exception_handler(
@@ -100,15 +64,15 @@
 ) -> "Response":
     """Handle any HTTPException errors (BaseVerboseHTTPException too).
 
     Doesn't handle 422 request error. Use ``verbose_request_validation_error_handler`` for it.
     """
     if isinstance(exc, BaseVerboseHTTPException):
         return JSONResponse(status_code=exc.status_code, content=exc.as_dict(), headers=exc.headers)
-    content = error_mapping[exc.status_code // 100]
+    content = ERROR_MAPPING[exc.status_code // 100]
     content["message"] = exc.detail
     return JSONResponse(
         status_code=exc.status_code,
         content=content,
         headers=exc.headers,
     )
 
@@ -118,22 +82,24 @@
     app.add_exception_handler(
         BaseVerboseHTTPException,
         verbose_http_exception_handler,  # type: ignore
     )
     return app
 
 
-def apply_all_handlers(app: FastAPI) -> FastAPI:
+def apply_all_handlers(app: FastAPI, *, override_422_openapi: bool = True) -> FastAPI:
     """Apply all exception handlers on given FastAPI instance.
 
     not apply ``verbose_http_exception_handler`` because BaseVerboseHTTPException is handled by
     any_http_exception_handler.
     """
     app.add_exception_handler(
         HTTPException,
         any_http_exception_handler,  # type: ignore
     )
     app.add_exception_handler(
         RequestValidationError,
         verbose_request_validation_error_handler,  # type: ignore
     )
+    if override_422_openapi:  # pragma: no coverage
+        override_422_error(app)
     return app
```

### Comparing `python_dev_utils-1.3.1/dev_utils/fastapi/verbose_http_exceptions/utils.py` & `python_dev_utils-1.4.0/dev_utils/fastapi/verbose_http_exceptions/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 
 from dev_utils.core.guards import all_elements_in_sequence_are_str
+from dev_utils.fastapi.verbose_http_exceptions.exc import RequestValidationVerboseHTTPException
 
 Location = str | None
 Attribute = str | None
 
 
 def resolve_error_location_and_attr(error: dict[str, Any]) -> tuple[Location, Attribute]:
     """Resolve given fastapi error: get loc and attr fields info."""
@@ -17,7 +18,20 @@
     ):
         return loc, attr
     if len(location) == 1:
         loc = location[0]
         return loc, attr
     *loc, attr = location
     return " -> ".join(loc), attr
+
+
+def validation_error_from_error_dict(
+    error: dict[str, Any],
+) -> RequestValidationVerboseHTTPException:
+    """Convert error dict to RequestValidationVerboseHTTPException instance."""
+    location, attribute = resolve_error_location_and_attr(error)
+    return RequestValidationVerboseHTTPException(
+        type_=error.get("type") or "not_known_type",
+        message=error.get("msg") or "not_known_message",
+        location=location,
+        attr_name=attribute,
+    )
```

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/audit.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/general.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.4.0/dev_utils/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/pyproject.toml` & `python_dev_utils-1.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -117,21 +117,23 @@
 
 [tool.coverage.run]
 source = [
     "sqlrepo",
 ]
 branch = true
 omit = [
-    "",
+    "dev_utils/fastapi/openapi/*",
+    "*/__init__.py",
 ]
 
 [tool.coverage.report]
 exclude_lines = [
     "enum.Enum",
-    "(Protocol)",
+    "(Protocol):",
+    "(typing.Protocol):",
     "pragma: no cover",
     "pragma: no coverage",
     "raise NotImplementedError",
     "if TYPE_CHECKING:",
     "if typing.TYPE_CHECKING:",
     "@overload",
 ]
@@ -169,36 +171,40 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.3.1"
+version = "1.4.0"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 fastapi_exceptions = [
-    "fastapi>=0.110.0",
+    "fastapi",
 ]
 profiling = [
-    "fastapi>=0.110.0",
+    "fastapi",
     "sqlalchemy>=2.0.28",
 ]
 sqlalchemy_filters = [
     "sqlalchemy>=2.0.28",
 ]
+extract_openapi = [
+    "fastapi",
+    "uvicorn",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `python_dev_utils-1.3.1/tests/conftest.py` & `python_dev_utils-1.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/core/test_abstract.py` & `python_dev_utils-1.4.0/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/core/test_guards.py` & `python_dev_utils-1.4.0/tests/core/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/core/test_results.py` & `python_dev_utils-1.4.0/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/core/test_utils.py` & `python_dev_utils-1.4.0/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/fastapi/conftest.py` & `python_dev_utils-1.4.0/tests/fastapi/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,42 +13,44 @@
 if TYPE_CHECKING:
     from collections.abc import Generator
 
 
 @pytest.fixture()
 def test_app_only_verbose() -> "Generator[TestClient, None, None]":
     app = FastAPI()
-    apply_verbose_http_exception_handler(app)
 
     @app.get("/")
     def index():  # type: ignore  # noqa: ANN202
         raise ServerErrorVerboseHTTPException(reason="test")
 
+    apply_verbose_http_exception_handler(app)
+
     with TestClient(
         app=app,
         base_url="http://test/",
     ) as c:
         yield c
 
 
 @pytest.fixture()
 def test_app_all_verbose() -> "Generator[TestClient, None, None]":
     app = FastAPI()
-    apply_all_handlers(app)
 
     @app.get("/")
     def index(a: Literal[1, 2], b: Literal[25]):  # type: ignore  # noqa: ANN202
         return {"message": "abc"}
 
     @app.get("/error")
     def error():  # type: ignore  # noqa: ANN202
         raise HTTPException(status_code=500, detail="test detail")
 
     @app.get("/verbose_error")
     def verbose_error():  # type: ignore  # noqa: ANN202
         raise ServerErrorVerboseHTTPException(reason="test")
 
+    apply_all_handlers(app)
+
     with TestClient(
         app=app,
         base_url="http://test/",
     ) as c:
         yield c
```

### Comparing `python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions.py` & `python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/fastapi/test_verbose_http_exceptions_handlers.py` & `python_dev_utils-1.4.0/tests/fastapi/test_verbose_http_exceptions_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fastapi import status
 from fastapi.testclient import TestClient
 
 expected_error_422_result = {
     "code": "multiple",
     "type": "multiple",
-    "message": "Multiple exceptions ocurred. Please check list for details.",
+    "message": "Multiple errors ocurred. Please check list for nested_errors.",
     "attr": None,
     "location": None,
     "nested_errors": [
         {
             "code": "validation_error",
             "type": "literal_error",
             "message": "Input should be 1 or 2",
```

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/mixins/test_general.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/mixins/test_general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/test_types.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/test_types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import zoneinfo
 from typing import TYPE_CHECKING, Any
 
 import pytest
 from mimesis import Datetime
 
-from tests.utils import PydanticTestSchema, TableWithUTCDT, create_db_item_sync
+from tests.utils import TableWithUTCDT, create_db_item_sync
 
 if TYPE_CHECKING:
     from sqlalchemy.orm import Session
 
     from tests.types import SyncFactoryFunctionProtocol
 
 
@@ -24,15 +24,14 @@
         session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> TableWithUTCDT:
         params: dict[str, Any] = dict(
             dt_field=dt_faker.datetime(),
-            pydantic_field=PydanticTestSchema(a=2, b=3, c=4),
         )
         params.update(kwargs)
         return create_db_item_sync(session, TableWithUTCDT, params, commit=commit)
 
     return _create
 
 
@@ -51,24 +50,7 @@
 ) -> None:
     item = table_create(db_sync_session, dt_field=dt, commit=True)
     if tzinfo_presents:
         assert item.dt_field.tzinfo is not None
         assert item.dt_field.tzinfo == UTC
     else:
         assert item.dt_field.tzinfo is None
-
-
-@pytest.mark.parametrize(
-    ("field", "expected_value"),
-    [
-        (PydanticTestSchema(a=255, b=255, c=255), PydanticTestSchema(a=255, b=255, c=255)),
-        ({"a": 255, "b": 255, "c": 255}, PydanticTestSchema(a=255, b=255, c=255)),  # noqa: DTZ005
-    ],
-)
-def test_pydantic_field(
-    field: Any,  # noqa: ANN401
-    expected_value: Any,  # noqa: ANN401
-    db_sync_session: "Session",
-    table_create: "SyncFactoryFunctionProtocol[TableWithUTCDT]",
-) -> None:
-    item = table_create(db_sync_session, pydantic_field=field, commit=True)
-    assert item.pydantic_field == expected_value
```

### Comparing `python_dev_utils-1.3.1/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.4.0/tests/sqlalchemy/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,29 +19,44 @@
     ],
 )
 def test_is_declarative(obj: Any, expected_result: bool) -> None:  # noqa: D103, ANN401, FBT001
     assert utils.is_declarative(obj) == expected_result
 
 
 @pytest.mark.parametrize(
-    ("field", "expected_result"),
+    ("field", "only_columns", "expected_result"),
     [
-        ("id", MyModel.id),
-        ("name", MyModel.name),
-        ("full_name", MyModel.full_name),
-        ("get_full_name", MyModel.get_full_name()),
+        ("id", False, MyModel.id),
+        ("id", True, MyModel.id),
+        ("name", False, MyModel.name),
+        ("name", True, MyModel.name),
+        ("full_name", False, MyModel.full_name),
+        ("get_full_name", False, MyModel.get_full_name()),
     ],
 )
-def test_get_sqlalchemy_attribute(field: str, expected_result: Any) -> None:  # noqa
-    assert str(utils.get_sqlalchemy_attribute(MyModel, field)) == str(expected_result)
+def test_get_sqlalchemy_attribute(
+    field: str,
+    only_columns: bool,  # noqa: FBT001
+    expected_result: Any,  # noqa: ANN401
+) -> None:  # noqa
+    assert str(
+        utils.get_sqlalchemy_attribute(MyModel, field, only_columns=only_columns),  # type: ignore
+    ) == str(expected_result)
 
 
-def test_get_sqlalchemy_attribute_incorrect() -> None:  # noqa
+@pytest.mark.parametrize(
+    ("field", "only_columns"),
+    [
+        ('incorrect_field', False),
+        ('incorrect_field', True),
+    ],
+)
+def test_get_sqlalchemy_attribute_incorrect(field: str, only_columns: bool) -> None:  # noqa
     with pytest.raises(NoModelAttributeError):
-        utils.get_sqlalchemy_attribute(MyModel, "incorrect_field")
+        utils.get_sqlalchemy_attribute(MyModel, field, only_columns=only_columns)  # type: ignore
 
 
 def test_get_registry_class() -> None:  # noqa
     assert utils.get_registry_class(MyModel) == MyModel.registry._class_registry  # type: ignore
 
 
 @pytest.mark.parametrize(
```

### Comparing `python_dev_utils-1.3.1/tests/types.py` & `python_dev_utils-1.4.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.3.1/tests/utils.py` & `python_dev_utils-1.4.0/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from sqlalchemy import ForeignKey, inspect
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.hybrid import hybrid_method, hybrid_property
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
 from dev_utils.sqlalchemy.types.datetime import UTCDateTime
-from dev_utils.sqlalchemy.types.pydantic import PydanticType
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
@@ -236,8 +235,7 @@
 
 
 class TableWithUTCDT(Base):  # noqa: D101
     __tablename__ = "table_with_UTC_dt"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     dt_field: Mapped[datetime.datetime] = mapped_column(UTCDateTime)
-    pydantic_field: Mapped[PydanticTestSchema] = mapped_column(PydanticType(PydanticTestSchema))
```

