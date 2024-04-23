# Comparing `tmp/django_ratelimiter-0.1.2.tar.gz` & `tmp/django_ratelimiter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ratelimiter-0.1.2.tar", max compression
+gzip compressed data, was "django_ratelimiter-0.2.0.tar", max compression
```

## Comparing `django_ratelimiter-0.1.2.tar` & `django_ratelimiter-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/LICENSE
--rw-r--r--   0        0        0     4038 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/README.md
--rw-r--r--   0        0        0      144 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/__init__.py
--rw-r--r--   0        0        0     4283 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/decorator.py
--rw-r--r--   0        0        0        0 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/py.typed
--rw-r--r--   0        0        0     1666 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/storage.py
--rw-r--r--   0        0        0      315 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/django_ratelimiter/types.py
--rw-r--r--   0        0        0      966 2024-04-22 07:51:12.805521 django_ratelimiter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 django_ratelimiter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4791 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/README.md
+-rw-r--r--   0        0        0      144 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/django_ratelimiter/__init__.py
+-rw-r--r--   0        0        0     2502 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/django_ratelimiter/decorator.py
+-rw-r--r--   0        0        0     2117 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/django_ratelimiter/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/django_ratelimiter/py.typed
+-rw-r--r--   0        0        0     1666 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/django_ratelimiter/storage.py
+-rw-r--r--   0        0        0      315 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/django_ratelimiter/types.py
+-rw-r--r--   0        0        0     1950 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/django_ratelimiter/utils.py
+-rw-r--r--   0        0        0     1184 2024-04-23 10:10:42.323579 django_ratelimiter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5683 1970-01-01 00:00:00.000000 django_ratelimiter-0.2.0/PKG-INFO
```

### Comparing `django_ratelimiter-0.1.2/LICENSE` & `django_ratelimiter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.1.2/README.md` & `django_ratelimiter-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -116,13 +116,39 @@
 from limits.storage import RedisStorage
 
 @ratelimit("5/minute", storage=RedisStorage(uri="redis://localhost:6379/0"))
 def view(request):
     return HttpResponse("OK")
 ```
 
+### Middleware
+
+Middleware can be used instead of decorators for more general cases.
+
+```py
+from typing import Optional
+
+from django.http import HttpRequest
+
+from django_ratelimiter.middleware import AbstractRateLimiterMiddleware
+
+
+class RateLimiterMiddleware(AbstractRateLimiterMiddleware):
+    def rate_for(self, request: HttpRequest) -> Optional[str]:
+        # allow only 100 POST requests per minute
+        if request.method == "POST":
+            return "100/minute"
+        # allow only 200 PUT requests per minute
+        if request.methid == "PUT":
+            return "200/minute"
+        # all other requests are not rate limited
+        return None
+```
+
+Middleware is customizable by overriding methods, see api reference for more details.
+
 ### DRF/ninja/class-based views
 
 `django-ratelimiter` is framework-agnostic, it should work with DRF/ninja out of the box.
 Class-based views are also supported with [method_decorator](https://docs.djangoproject.com/en/5.0/topics/class-based-views/intro/#decorating-the-class).
 
 See examples in [test_app](./test_app/views.py).
```

### Comparing `django_ratelimiter-0.1.2/django_ratelimiter/storage.py` & `django_ratelimiter-0.2.0/django_ratelimiter/storage.py`

 * *Files identical despite different names*

### Comparing `django_ratelimiter-0.1.2/PKG-INFO` & `django_ratelimiter-0.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: django-ratelimiter
-Version: 0.1.2
+Version: 0.2.0
 Summary: Rate-limiting for django
+Home-page: https://django-ratelimiter.readthedocs.io/
 License: MIT
+Keywords: rate-limit,django
 Author: Andrii Kohut
 Author-email: kogut.andriy@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django
 Requires-Dist: limits (>=3.10)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0) ; python_version == "3.9"
+Project-URL: Documentation, https://django-ratelimiter.readthedocs.io/
+Project-URL: Repository, https://github.com/andriykohut/django-ratelimiter
 Description-Content-Type: text/markdown
 
 # django-ratelimiter
 
 [![PyPI version](https://badge.fury.io/py/django-ratelimiter.svg)](https://pypi.org/project/django-ratelimiter/)
 [![CI](https://github.com/andriykohut/django-ratelimiter/actions/workflows/ci.yml/badge.svg)](https://github.com/andriykohut/django-ratelimiter/actions/workflows/ci.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/andriykohut/django-ratelimiter/branch/main/graph/badge.svg)](https://codecov.io/gh/andriykohut/django-ratelimiter)
@@ -135,14 +139,40 @@
 from limits.storage import RedisStorage
 
 @ratelimit("5/minute", storage=RedisStorage(uri="redis://localhost:6379/0"))
 def view(request):
     return HttpResponse("OK")
 ```
 
+### Middleware
+
+Middleware can be used instead of decorators for more general cases.
+
+```py
+from typing import Optional
+
+from django.http import HttpRequest
+
+from django_ratelimiter.middleware import AbstractRateLimiterMiddleware
+
+
+class RateLimiterMiddleware(AbstractRateLimiterMiddleware):
+    def rate_for(self, request: HttpRequest) -> Optional[str]:
+        # allow only 100 POST requests per minute
+        if request.method == "POST":
+            return "100/minute"
+        # allow only 200 PUT requests per minute
+        if request.methid == "PUT":
+            return "200/minute"
+        # all other requests are not rate limited
+        return None
+```
+
+Middleware is customizable by overriding methods, see api reference for more details.
+
 ### DRF/ninja/class-based views
 
 `django-ratelimiter` is framework-agnostic, it should work with DRF/ninja out of the box.
 Class-based views are also supported with [method_decorator](https://docs.djangoproject.com/en/5.0/topics/class-based-views/intro/#decorating-the-class).
 
 See examples in [test_app](./test_app/views.py).
```

