# Comparing `tmp/django_microsoft_sso-3.3.1.tar.gz` & `tmp/django_microsoft_sso-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_microsoft_sso-3.3.1.tar", max compression
+gzip compressed data, was "django_microsoft_sso-3.4.0.tar", max compression
```

## Comparing `django_microsoft_sso-3.3.1.tar` & `django_microsoft_sso-3.4.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1072 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/LICENSE
--rw-r--r--   0        0        0     3082 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/README.md
--rw-r--r--   0        0        0       22 2024-04-09 19:46:03.178920 django_microsoft_sso-3.3.1/django_microsoft_sso/__init__.py
--rw-r--r--   0        0        0     1967 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/admin.py
--rw-r--r--   0        0        0      347 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/apps.py
--rw-r--r--   0        0        0        0 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/checks/__init__.py
--rw-r--r--   0        0        0     1324 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/checks/warnings.py
--rw-r--r--   0        0        0     2762 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/conf.py
--rw-r--r--   0        0        0      625 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/hooks.py
--rw-r--r--   0        0        0    10397 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/main.py
--rw-r--r--   0        0        0     1083 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0      433 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/0002_microsoftssouser_user_principal_name.py
--rw-r--r--   0        0        0        0 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/__init__.py
--rw-r--r--   0        0        0     1128 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/models.py
--rw-r--r--   0        0        0     2283 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css
--rw-r--r--   0        0        0     1207 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login.html
--rw-r--r--   0        0        0     1421 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-04-09 19:45:54.334997 django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1451 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/__init__.py
--rw-r--r--   0        0        0     3968 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/conftest.py
--rw-r--r--   0        0        0      257 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_conf.py
--rw-r--r--   0        0        0     2365 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_microsoft_auth.py
--rw-r--r--   0        0        0      549 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_models.py
--rw-r--r--   0        0        0     5562 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     6893 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_views.py
--rw-r--r--   0        0        0      322 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/urls.py
--rw-r--r--   0        0        0     6042 2024-04-09 19:45:54.338997 django_microsoft_sso-3.3.1/django_microsoft_sso/views.py
--rw-r--r--   0        0        0     2306 2024-04-09 19:46:03.178920 django_microsoft_sso-3.3.1/pyproject.toml
--rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 django_microsoft_sso-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/LICENSE
+-rw-r--r--   0        0        0     3082 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-23 20:06:26.337994 django_microsoft_sso-3.4.0/django_microsoft_sso/__init__.py
+-rw-r--r--   0        0        0     1967 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/admin.py
+-rw-r--r--   0        0        0      347 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1324 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/checks/warnings.py
+-rw-r--r--   0        0        0     3080 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/conf.py
+-rw-r--r--   0        0        0      625 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/hooks.py
+-rw-r--r--   0        0        0    10397 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/main.py
+-rw-r--r--   0        0        0     1083 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0      433 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/migrations/0002_microsoftssouser_user_principal_name.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/migrations/__init__.py
+-rw-r--r--   0        0        0     1128 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/models.py
+-rw-r--r--   0        0        0     2283 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css
+-rw-r--r--   0        0        0     1207 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/templates/microsoft_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1451 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/tests/__init__.py
+-rw-r--r--   0        0        0     3968 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/tests/conftest.py
+-rw-r--r--   0        0        0      257 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     2365 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_microsoft_auth.py
+-rw-r--r--   0        0        0      549 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_models.py
+-rw-r--r--   0        0        0     5562 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     6893 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_views.py
+-rw-r--r--   0        0        0      322 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/urls.py
+-rw-r--r--   0        0        0      415 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/utils.py
+-rw-r--r--   0        0        0     6157 2024-04-23 20:06:16.109888 django_microsoft_sso-3.4.0/django_microsoft_sso/views.py
+-rw-r--r--   0        0        0     2306 2024-04-23 20:06:26.337994 django_microsoft_sso-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 django_microsoft_sso-3.4.0/PKG-INFO
```

### Comparing `django_microsoft_sso-3.3.1/LICENSE` & `django_microsoft_sso-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/README.md` & `django_microsoft_sso-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/admin.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/admin.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/checks/warnings.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/conf.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.conf import settings
+from loguru import logger
 
 MICROSOFT_SSO_APPLICATION_ID = getattr(settings, "MICROSOFT_SSO_APPLICATION_ID", None)
 MICROSOFT_SSO_CLIENT_SECRET = getattr(settings, "MICROSOFT_SSO_CLIENT_SECRET", None)
 MICROSOFT_SSO_SCOPES = getattr(
     settings,
     "MICROSOFT_SSO_SCOPES",
     ["User.ReadBasic.All"],
@@ -63,7 +64,14 @@
 SSO_USE_ALTERNATE_W003 = getattr(settings, "SSO_USE_ALTERNATE_W003", False)
 
 if SSO_USE_ALTERNATE_W003:
     from django_microsoft_sso.checks.warnings import register_sso_check  # noqa
 
 MICROSOFT_SSO_AUTHORITY = getattr(settings, "MICROSOFT_SSO_AUTHORITY", None)
 MICROSOFT_SSO_UNIQUE_EMAIL = getattr(settings, "MICROSOFT_SSO_UNIQUE_EMAIL", False)
+MICROSOFT_SSO_ENABLE_LOGS = getattr(settings, "MICROSOFT_SSO_ENABLE_LOGS", True)
+MICROSOFT_SSO_ENABLE_MESSAGES = getattr(settings, "MICROSOFT_SSO_ENABLE_MESSAGES", True)
+
+if MICROSOFT_SSO_ENABLE_LOGS:
+    logger.enable("django_microsoft_sso")
+else:
+    logger.disable("django_microsoft_sso")
```

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/hooks.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/hooks.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/main.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/main.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/migrations/0001_initial.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/models.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css` & `django_microsoft_sso-3.4.0/django_microsoft_sso/static/django_microsoft_sso/microsoft_button.css`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login.html` & `django_microsoft_sso-3.4.0/django_microsoft_sso/templates/microsoft_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/templates/microsoft_sso/login_sso.html` & `django_microsoft_sso-3.4.0/django_microsoft_sso/templates/microsoft_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/templatetags/sso_tags.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/conftest.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_microsoft_auth.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_microsoft_auth.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_models.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_user_helper.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/tests/test_views.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_microsoft_sso-3.3.1/django_microsoft_sso/views.py` & `django_microsoft_sso-3.4.0/django_microsoft_sso/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import importlib
 from urllib.parse import urlparse
 
-from django.contrib import messages
 from django.contrib.auth import login
 from django.contrib.auth.views import LogoutView
 from django.http import HttpRequest, HttpResponseRedirect
 from django.shortcuts import resolve_url
 from django.template.response import TemplateResponse
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_http_methods
+from loguru import logger
 
 from django_microsoft_sso import conf
 from django_microsoft_sso.main import MicrosoftAuth, UserHelper
+from django_microsoft_sso.utils import send_message, show_credential
 
 
 @require_http_methods(["GET"])
 def start_login(request: HttpRequest) -> HttpResponseRedirect:
     # Get the next url
     next_param = request.GET.get(key="next")
     if next_param:
@@ -49,66 +50,65 @@
     login_failed_url = reverse(conf.MICROSOFT_SSO_LOGIN_FAILED_URL)
     microsoft = MicrosoftAuth(request)
     code = request.GET.get("code")
     state = request.GET.get("state")
 
     # Check if Microsoft SSO is enabled
     if not conf.MICROSOFT_SSO_ENABLED:
-        messages.add_message(request, messages.ERROR, _("Microsoft SSO not enabled."))
+        send_message(request, _("Microsoft SSO not enabled."))
         return HttpResponseRedirect(login_failed_url)
 
     # First, check for authorization code
     if not code:
-        messages.add_message(
-            request, messages.ERROR, _("Authorization Code not received from SSO.")
-        )
+        send_message(request, _("Authorization Code not received from SSO."))
         return HttpResponseRedirect(login_failed_url)
 
     # Then, check the state.
     request_state = request.session.get("msal_graph_info", {}).get("state")
     next_url = request.session.get("sso_next_url")
 
     if not request_state or state != request_state:
-        messages.add_message(request, messages.ERROR, _("State Mismatch. Time expired?"))
+        send_message(request, _("State Mismatch. Time expired?"))
         return HttpResponseRedirect(login_failed_url)
 
     # Get Access Token from Microsoft Graph
     auth_result = microsoft.get_user_token()
     if not auth_result:
-        messages.add_message(
-            request, messages.ERROR, _("Authorization Data not received from SSO.")
-        )
+        send_message(request, _("Access Token not received from SSO."))
         return HttpResponseRedirect(login_failed_url)
     if "error" in auth_result:
-        messages.add_message(
-            request,
-            messages.ERROR,
-            _(f"Authorization Error received from SSO: {auth_result['error']}."),
+        send_message(
+            request, _(f"Authorization Error received from SSO: {auth_result['error']}.")
         )
         if auth_result["error"] == "invalid_client":
-            messages.add_message(
-                request,
-                messages.ERROR,
-                _("Please check your Client Credentials for MS Entra App."),
+            send_message(
+                request, _("Please check your Client Credentials for MS Entra App.")
+            )
+            logger.debug(
+                f"MICROSOFT_SSO_APPLICATION_ID: "
+                f"{show_credential(conf.MICROSOFT_SSO_APPLICATION_ID)}"
+            )
+            logger.debug(
+                f"MICROSOFT_SSO_CLIENT_SECRET: "
+                f"{show_credential(conf.MICROSOFT_SSO_CLIENT_SECRET)}"
             )
         return HttpResponseRedirect(login_failed_url)
 
     try:
         user_result = microsoft.get_user_info()
     except Exception as error:
-        messages.add_message(request, messages.ERROR, str(error))
+        send_message(request, _(f"Error while processing callback from SSO: {error}."))
         return HttpResponseRedirect(login_failed_url)
 
     user_helper = UserHelper(user_result, request)
 
     # Check if User Info is valid to login
     if not user_helper.email_is_valid:
-        messages.add_message(
+        send_message(
             request,
-            messages.ERROR,
             _(
                 f"Email address not allowed: {user_helper.user_email}. "
                 f"Please contact your administrator."
             ),
         )
         return HttpResponseRedirect(login_failed_url)
```

### Comparing `django_microsoft_sso-3.3.1/pyproject.toml` & `django_microsoft_sso-3.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-microsoft-sso"
-version = "3.3.1"
+version = "3.4.0"
 description = "Easily add Microsoft Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-microsoft-sso"
 keywords = ["microsoft", "django", "sso"]
 license = "MIT"
 classifiers = [
```

### Comparing `django_microsoft_sso-3.3.1/PKG-INFO` & `django_microsoft_sso-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-microsoft-sso
-Version: 3.3.1
+Version: 3.4.0
 Summary: Easily add Microsoft Authentication to your Django Projects
 Home-page: https://github.com/megalus/django-microsoft-sso
 License: MIT
 Keywords: microsoft,django,sso
 Author: Chris Maillefaud
 Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-microsoft-sso Version: 3.3.1 Summary: Easily
+Metadata-Version: 2.1 Name: django-microsoft-sso Version: 3.4.0 Summary: Easily
 add Microsoft Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-microsoft-sso License: MIT Keywords:
 microsoft,django,sso Author: Chris Maillefaud Author-email:
 chrismaille@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Plugins Classifier:
 Framework :: Django Classifier: Framework :: Django :: 4.1 Classifier:
 Framework :: Django :: 4.2 Classifier: Framework :: Django :: 5.0 Classifier:
```

