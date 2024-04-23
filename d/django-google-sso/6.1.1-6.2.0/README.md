# Comparing `tmp/django_google_sso-6.1.1.tar.gz` & `tmp/django_google_sso-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_google_sso-6.1.1.tar", max compression
+gzip compressed data, was "django_google_sso-6.2.0.tar", max compression
```

## Comparing `django_google_sso-6.1.1.tar` & `django_google_sso-6.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1072 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/LICENSE
--rw-r--r--   0        0        0     2849 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/README.md
--rw-r--r--   0        0        0       22 2024-04-09 19:46:30.891042 django_google_sso-6.1.1/django_google_sso/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/admin.py
--rw-r--r--   0        0        0      346 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/apps.py
--rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/checks/__init__.py
--rw-r--r--   0        0        0     1321 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/checks/warnings.py
--rw-r--r--   0        0        0     2527 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/conf.py
--rw-r--r--   0        0        0      693 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/hooks.py
--rw-r--r--   0        0        0     6482 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/main.py
--rw-r--r--   0        0        0     1324 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
--rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/migrations/__init__.py
--rw-r--r--   0        0        0      915 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/models.py
--rw-r--r--   0        0        0     1195 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/static/django_google_sso/google_button.css
--rw-r--r--   0        0        0     1198 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templates/google_sso/login.html
--rw-r--r--   0        0        0     1421 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templates/google_sso/login_sso.html
--rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templatetags/__init__.py
--rw-r--r--   0        0        0      218 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templatetags/show_form.py
--rw-r--r--   0        0        0     1559 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/templatetags/sso_tags.py
--rw-r--r--   0        0        0        0 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/conftest.py
--rw-r--r--   0        0        0      248 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_conf.py
--rw-r--r--   0        0        0     2579 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_google_auth.py
--rw-r--r--   0        0        0      839 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_models.py
--rw-r--r--   0        0        0     4316 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_user_helper.py
--rw-r--r--   0        0        0     5957 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/tests/test_views.py
--rw-r--r--   0        0        0      313 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/urls.py
--rw-r--r--   0        0        0     4610 2024-04-09 19:46:22.222922 django_google_sso-6.1.1/django_google_sso/views.py
--rw-r--r--   0        0        0     2238 2024-04-09 19:46:30.891042 django_google_sso-6.1.1/pyproject.toml
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 django_google_sso-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/LICENSE
+-rw-r--r--   0        0        0     2849 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-23 20:23:44.122602 django_google_sso-6.2.0/django_google_sso/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/admin.py
+-rw-r--r--   0        0        0      346 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/apps.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/checks/__init__.py
+-rw-r--r--   0        0        0     1321 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/checks/warnings.py
+-rw-r--r--   0        0        0     2822 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/conf.py
+-rw-r--r--   0        0        0      693 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/hooks.py
+-rw-r--r--   0        0        0     6482 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/main.py
+-rw-r--r--   0        0        0     1324 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/migrations/0002_alter_googlessouser_picture_url.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/migrations/__init__.py
+-rw-r--r--   0        0        0      915 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/models.py
+-rw-r--r--   0        0        0     1195 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/static/django_google_sso/google_button.css
+-rw-r--r--   0        0        0     1198 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/templates/google_sso/login.html
+-rw-r--r--   0        0        0     1421 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/templates/google_sso/login_sso.html
+-rw-r--r--   0        0        0        0 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/templatetags/__init__.py
+-rw-r--r--   0        0        0      218 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/templatetags/show_form.py
+-rw-r--r--   0        0        0     1559 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/templatetags/sso_tags.py
+-rw-r--r--   0        0        0        0 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/tests/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/tests/conftest.py
+-rw-r--r--   0        0        0      248 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/tests/test_conf.py
+-rw-r--r--   0        0        0     2579 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/tests/test_google_auth.py
+-rw-r--r--   0        0        0      839 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/tests/test_models.py
+-rw-r--r--   0        0        0     4316 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/tests/test_user_helper.py
+-rw-r--r--   0        0        0     5957 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/tests/test_views.py
+-rw-r--r--   0        0        0      313 2024-04-23 20:23:36.226663 django_google_sso-6.2.0/django_google_sso/urls.py
+-rw-r--r--   0        0        0      442 2024-04-23 20:23:36.230663 django_google_sso-6.2.0/django_google_sso/utils.py
+-rw-r--r--   0        0        0     4905 2024-04-23 20:23:36.230663 django_google_sso-6.2.0/django_google_sso/views.py
+-rw-r--r--   0        0        0     2238 2024-04-23 20:23:44.122602 django_google_sso-6.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 django_google_sso-6.2.0/PKG-INFO
```

### Comparing `django_google_sso-6.1.1/LICENSE` & `django_google_sso-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/README.md` & `django_google_sso-6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/admin.py` & `django_google_sso-6.2.0/django_google_sso/admin.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/checks/warnings.py` & `django_google_sso-6.2.0/django_google_sso/checks/warnings.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/conf.py` & `django_google_sso-6.2.0/django_google_sso/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.conf import settings
+from loguru import logger
 
 GOOGLE_SSO_CLIENT_ID = getattr(settings, "GOOGLE_SSO_CLIENT_ID", None)
 
 GOOGLE_SSO_PROJECT_ID = getattr(settings, "GOOGLE_SSO_PROJECT_ID", None)
 GOOGLE_SSO_CLIENT_SECRET = getattr(settings, "GOOGLE_SSO_CLIENT_SECRET", None)
 GOOGLE_SSO_SCOPES = getattr(
     settings,
@@ -56,8 +57,16 @@
 GOOGLE_SSO_ALWAYS_UPDATE_USER_DATA = getattr(
     settings, "GOOGLE_SSO_ALWAYS_UPDATE_USER_DATA", False
 )
 GOOGLE_SSO_DEFAULT_LOCALE = getattr(settings, "GOOGLE_SSO_DEFAULT_LOCALE", "en")
 SSO_USE_ALTERNATE_W003 = getattr(settings, "SSO_USE_ALTERNATE_W003", False)
 
 if SSO_USE_ALTERNATE_W003:
-    from django_microsoft_sso.checks.warnings import register_sso_check  # noqa
+    from django_google_sso.checks.warnings import register_sso_check  # noqa
+
+GOOGLE_SSO_ENABLE_LOGS = getattr(settings, "GOOGLE_SSO_ENABLE_LOGS", True)
+GOOGLE_SSO_ENABLE_MESSAGES = getattr(settings, "GOOGLE_SSO_ENABLE_MESSAGES", True)
+
+if GOOGLE_SSO_ENABLE_LOGS:
+    logger.enable("django_google_sso")
+else:
+    logger.disable("django_google_sso")
```

### Comparing `django_google_sso-6.1.1/django_google_sso/hooks.py` & `django_google_sso-6.2.0/django_google_sso/hooks.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/main.py` & `django_google_sso-6.2.0/django_google_sso/main.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/migrations/0001_initial.py` & `django_google_sso-6.2.0/django_google_sso/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/models.py` & `django_google_sso-6.2.0/django_google_sso/models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/static/django_google_sso/google_button.css` & `django_google_sso-6.2.0/django_google_sso/static/django_google_sso/google_button.css`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/templates/google_sso/login.html` & `django_google_sso-6.2.0/django_google_sso/templates/google_sso/login.html`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/templates/google_sso/login_sso.html` & `django_google_sso-6.2.0/django_google_sso/templates/google_sso/login_sso.html`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/templatetags/sso_tags.py` & `django_google_sso-6.2.0/django_google_sso/templatetags/sso_tags.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/tests/conftest.py` & `django_google_sso-6.2.0/django_google_sso/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/tests/test_google_auth.py` & `django_google_sso-6.2.0/django_google_sso/tests/test_google_auth.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/tests/test_models.py` & `django_google_sso-6.2.0/django_google_sso/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/tests/test_user_helper.py` & `django_google_sso-6.2.0/django_google_sso/tests/test_user_helper.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/tests/test_views.py` & `django_google_sso-6.2.0/django_google_sso/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_google_sso-6.1.1/django_google_sso/views.py` & `django_google_sso-6.2.0/django_google_sso/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import importlib
 from urllib.parse import urlparse
 
-from django.contrib import messages
 from django.contrib.auth import login
 from django.http import HttpRequest, HttpResponseRedirect
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 from django.views.decorators.http import require_http_methods
+from loguru import logger
 
 from django_google_sso import conf
 from django_google_sso.main import GoogleAuth, UserHelper
+from django_google_sso.utils import send_message, show_credential
 
 
 @require_http_methods(["GET"])
 def start_login(request: HttpRequest) -> HttpResponseRedirect:
     # Get the next url
     next_param = request.GET.get(key="next")
     if next_param:
@@ -47,50 +48,55 @@
     login_failed_url = reverse(conf.GOOGLE_SSO_LOGIN_FAILED_URL)
     google = GoogleAuth(request)
     code = request.GET.get("code")
     state = request.GET.get("state")
 
     # Check if Google SSO is enabled
     if not conf.GOOGLE_SSO_ENABLED:
-        messages.add_message(request, messages.ERROR, _("Google SSO not enabled."))
+        send_message(request, _("Google SSO not enabled."))
         return HttpResponseRedirect(login_failed_url)
 
     # First, check for authorization code
     if not code:
-        messages.add_message(
-            request, messages.ERROR, _("Authorization Code not received from SSO.")
-        )
+        send_message(request, _("Authorization Code not received from SSO."))
         return HttpResponseRedirect(login_failed_url)
 
     # Then, check state.
     request_state = request.session.get("sso_state")
     next_url = request.session.get("sso_next_url")
 
     if not request_state or state != request_state:
-        messages.add_message(
-            request, messages.ERROR, _("State Mismatch. Time expired?")
-        )
+        send_message(request, _("State Mismatch. Time expired?"))
         return HttpResponseRedirect(login_failed_url)
 
     # Get Access Token from Google
     try:
         google.flow.fetch_token(code=code)
     except Exception as error:
-        messages.add_message(request, messages.ERROR, str(error))
+        send_message(request, _(f"Error while fetching token from SSO: {error}."))
+        logger.debug(
+            f"GOOGLE_SSO_CLIENT_ID: {show_credential(conf.GOOGLE_SSO_CLIENT_ID)}"
+        )
+        logger.debug(
+            f"GOOGLE_SSO_PROJECT_ID: {show_credential(conf.GOOGLE_SSO_PROJECT_ID)}"
+        )
+        logger.debug(
+            f"GOOGLE_SSO_CLIENT_SECRET: "
+            f"{show_credential(conf.GOOGLE_SSO_CLIENT_SECRET)}"
+        )
         return HttpResponseRedirect(login_failed_url)
 
     # Get User Info from Google
     google_user_data = google.get_user_info()
     user_helper = UserHelper(google_user_data, request)
 
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

### Comparing `django_google_sso-6.1.1/pyproject.toml` & `django_google_sso-6.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "python -m pip install -U twine poetry && poetry build"
 
 [tool.poetry]
 name = "django-google-sso"
-version = "6.1.1"
+version = "6.2.0"
 description = "Easily add Google Authentication to your Django Projects"
 authors = ["Chris Maillefaud <chrismaille@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/megalus/django-google-sso"
 keywords = ["google", "django", "sso"]
 license = "MIT"
 classifiers = [
```

### Comparing `django_google_sso-6.1.1/PKG-INFO` & `django_google_sso-6.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-google-sso
-Version: 6.1.1
+Version: 6.2.0
 Summary: Easily add Google Authentication to your Django Projects
 Home-page: https://github.com/megalus/django-google-sso
 License: MIT
 Keywords: google,django,sso
 Author: Chris Maillefaud
 Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-google-sso Version: 6.1.1 Summary: Easily
+Metadata-Version: 2.1 Name: django-google-sso Version: 6.2.0 Summary: Easily
 add Google Authentication to your Django Projects Home-page: https://
 github.com/megalus/django-google-sso License: MIT Keywords: google,django,sso
 Author: Chris Maillefaud Author-email: chrismaille@users.noreply.github.com
 Requires-Python: >=3.10,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Environment :: Plugins Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django :: 4.2
 Classifier: Framework :: Django :: 5.0 Classifier: Intended Audience ::
```

