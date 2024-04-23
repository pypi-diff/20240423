# Comparing `tmp/pangea_django-1.0.0.tar.gz` & `tmp/pangea_django-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangea_django-1.0.0.tar", max compression
+gzip compressed data, was "pangea_django-1.0.1.tar", max compression
```

## Comparing `pangea_django-1.0.0.tar` & `pangea_django-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     3327 2023-12-20 19:57:38.695060 pangea_django-1.0.0/README.md
--rw-r--r--   0        0        0      110 2023-12-20 22:34:19.193433 pangea_django-1.0.0/pangea_django/__init__.py
--rw-r--r--   0        0        0     5223 2023-12-20 22:34:19.193433 pangea_django-1.0.0/pangea_django/pangea_django_auth.py
--rw-r--r--   0        0        0      780 2023-12-20 22:13:44.864576 pangea_django-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 pangea_django-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      429 2024-04-23 20:03:57.085644 pangea_django-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3326 2024-04-23 20:03:57.085644 pangea_django-1.0.1/README.md
+-rw-r--r--   0        0        0      110 2024-04-23 20:03:57.086644 pangea_django-1.0.1/pangea_django/__init__.py
+-rw-r--r--   0        0        0     5258 2024-04-23 20:03:57.086644 pangea_django-1.0.1/pangea_django/pangea_django_auth.py
+-rw-r--r--   0        0        0      868 2024-04-23 20:03:57.087644 pangea_django-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4271 1970-01-01 00:00:00.000000 pangea_django-1.0.1/PKG-INFO
```

### Comparing `pangea_django-1.0.0/README.md` & `pangea_django-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,7 @@
 * This auth backend is designed to use the hosted login method provided by Pangea. You will need to do the following to authenticate
     - From the Django view(s) where you want to kick off a login process, redirect to your hosted login link.`redirect(f"<link you copied from the Pangea Console>?state={generate_state_param(request)}")`. Note the use of the `generate_state_param` helper function from the pangea_django module. This creates a secure state param for this purpose.
     - From the Django view where the user was redirected from the login process, use the pangea_django.PangeaAuthentication class to authenticate the request `PangeaAuthentication().authenticate(request=request)`. If authentication was successful you will get a UserModel object representing the user (`None` otherwise).
     - From views where you wish to check if the user is logged in you can use the normal Django patterns of checking `request.user.is_authenticated` or using the `login_required` decorator etc.
     - You can log the user out with `PangeaAuthentication().logout(request)`
     - The `authenticate` call will create a user based on the email(username) address in Pangea if that user does not exist, it will also populate basic info (first name, last name, email address and last login time).
     - The user will be logged out automatically once the user's active token has expired and their refresh token can no longer refresh the session.
-
```

### Comparing `pangea_django-1.0.0/pangea_django/pangea_django_auth.py` & `pangea_django-1.0.1/pangea_django/pangea_django_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # Copyright 2023 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 
-from datetime import datetime
 import os
-import traceback
-import string
 import secrets
+import string
+import traceback
+from datetime import datetime
 
-from django.contrib.auth.backends import BaseBackend
 from django.contrib.auth import get_user_model
+from django.contrib.auth.backends import BaseBackend
 from django.contrib.auth.models import AnonymousUser
-
-from pangea.services.authn.authn import AuthN
+from django.http import HttpRequest
 from pangea.config import PangeaConfig
+from pangea.services.authn.authn import AuthN
 
 UserModel = get_user_model()
 
+
 def generate_state_param(request: HttpRequest) -> str:
     alphabet = string.ascii_letters + string.digits
-    state = ''.join(secrets.choice(alphabet) for i in range(12))
+    state = "".join(secrets.choice(alphabet) for i in range(12))
     request.session["PANGEA_LOGIN_STATE"] = state
     return state
 
 
-class PangeaAuthMiddleware():
+class PangeaAuthMiddleware:
     class InvalidSessionException(Exception):
         pass
 
     def __init__(self, get_response):
         self.authn = PangeaAuthentication()
         self.get_response = get_response
 
@@ -41,47 +42,48 @@
                     expires = datetime.fromisoformat(expires)
                 except ValueError:
                     # support older python that doesn't understand the trailing Z
                     expires = datetime.fromisoformat(expires.rstrip("Z"))
                 if expires < datetime.utcnow():
                     refresh_token = request.session["PANGEA_REFRESH_TOKEN"]["token"]
                     response = self.authn.client.refresh(refresh_token=refresh_token)
-                    if not response.status == 'Success':
+                    if not response.status == "Success":
                         raise self.InvalidSessionException
                     active_token = response["active_token"]
                     response.session["PANGEA_ACTIVE_TOKEN"] = active_token
             else:
                 raise self.InvalidSessionException
         except self.InvalidSessionException as e:
             request.user = AnonymousUser()
         else:
             request.user = self.authn.get_user(username=active_token["email"])
 
         return self.get_response(request)
 
+
 class PangeaAuthentication(BaseBackend):
     def __init__(self):
         token = os.getenv("PANGEA_AUTHN_TOKEN")
         domain = os.getenv("PANGEA_DOMAIN")
         self.config = PangeaConfig(domain=domain)
         self.authn = AuthN(token, config=self.config, logger_name="pangea")
         super().__init__()
 
     def authenticate(self, request: HttpRequest):
-        code = request.GET.get('code')
-        state = request.GET.get('state')
+        code = request.GET.get("code")
+        state = request.GET.get("state")
         expected_state = request.session.get("PANGEA_LOGIN_STATE")
         user = None
         if not code or not expected_state or state != expected_state:
             return None
         resp = self.authn.client.userinfo(code=code)
         if resp and resp.status == "Success":
             try:
-                refresh = resp.raw_result['refresh_token']
-                active = resp.raw_result['active_token']
+                refresh = resp.raw_result["refresh_token"]
+                active = resp.raw_result["active_token"]
                 user, created = UserModel.objects.get_or_create(username=active["email"])
                 if created:
                     user.email = active["email"]
                     user.first_name = active["profile"]["first_name"]
                     user.last_name = active["profile"]["last_name"]
                     user.last_login = active["profile"]["Last-Login-Time"]
                     user.is_active = True
```

### Comparing `pangea_django-1.0.0/pyproject.toml` & `pangea_django-1.0.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-[tool.poetry]
-name = "pangea-django"
-version = "1.0.0"
-description = "Pangea Authentication Addon for Django"
-authors = ["Govind Salinas <govind.salinas@pangea.cloud>"]
-license = "MIT"
-readme = "README.md"
-homepage = "https://github.com/pangeacyber/pangea-python"
-repository = "https://github.com/pangeacyber/pangea-python"
-keywords = ["Pangea", "Django", "AutnN"]
-classifiers = [
-    "Topic :: Software Development",
-    "Topic :: Software Development :: Libraries",
-]
-packages = [
-    { include = "pangea_django" }
-]
-
-[tool.poetry.dependencies]
-python = "^3.8.0"
-"Django" = "^4.2.1"
-"pangea-sdk" = "^3.4.0"
-
-[tool.poetry.dev-dependencies]
-black = "^22.1.0"
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "pangea-django"
+version = "1.0.1"
+description = "Pangea Authentication Addon for Django"
+authors = ["Govind Salinas <govind.salinas@pangea.cloud>"]
+license = "MIT"
+readme = "README.md"
+homepage = "https://github.com/pangeacyber/pangea-python"
+repository = "https://github.com/pangeacyber/pangea-python"
+keywords = ["Pangea", "Django", "AutnN"]
+classifiers = [
+    "Topic :: Software Development",
+    "Topic :: Software Development :: Libraries",
+]
+packages = [
+    { include = "pangea_django" }
+]
+include = ["CHANGELOG.md"]
+
+[tool.poetry.dependencies]
+python = "^3.8.0"
+"Django" = "^4.2.11"
+"pangea-sdk" = "^3.7.1"
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.12.0"
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 120
+
+[tool.isort]
+profile = "black"
+line_length = 120
```

### Comparing `pangea_django-1.0.0/PKG-INFO` & `pangea_django-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: pangea-django
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pangea Authentication Addon for Django
 Home-page: https://github.com/pangeacyber/pangea-python
 License: MIT
 Keywords: Pangea,Django,AutnN
 Author: Govind Salinas
 Author-email: govind.salinas@pangea.cloud
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: Django (>=4.2.1,<5.0.0)
-Requires-Dist: pangea-sdk (>=3.4.0,<4.0.0)
+Requires-Dist: Django (>=4.2.11,<5.0.0)
+Requires-Dist: pangea-sdk (>=3.7.1,<4.0.0)
 Project-URL: Repository, https://github.com/pangeacyber/pangea-python
 Description-Content-Type: text/markdown
 
 # Pangea Django Setup
 
 Use Django as your authentication backend in a few simple steps.
 
@@ -52,8 +53,7 @@
     - From the Django view(s) where you want to kick off a login process, redirect to your hosted login link.`redirect(f"<link you copied from the Pangea Console>?state={generate_state_param(request)}")`. Note the use of the `generate_state_param` helper function from the pangea_django module. This creates a secure state param for this purpose.
     - From the Django view where the user was redirected from the login process, use the pangea_django.PangeaAuthentication class to authenticate the request `PangeaAuthentication().authenticate(request=request)`. If authentication was successful you will get a UserModel object representing the user (`None` otherwise).
     - From views where you wish to check if the user is logged in you can use the normal Django patterns of checking `request.user.is_authenticated` or using the `login_required` decorator etc.
     - You can log the user out with `PangeaAuthentication().logout(request)`
     - The `authenticate` call will create a user based on the email(username) address in Pangea if that user does not exist, it will also populate basic info (first name, last name, email address and last login time).
     - The user will be logged out automatically once the user's active token has expired and their refresh token can no longer refresh the session.
 
-
```

