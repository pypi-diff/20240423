# Comparing `tmp/django_azure_auth-1.2.1.tar.gz` & `tmp/django_azure_auth-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.2.1.tar", max compression
+gzip compressed data, was "django_azure_auth-1.2.2.tar", max compression
```

## Comparing `django_azure_auth-1.2.1.tar` & `django_azure_auth-1.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/LICENSE
--rw-r--r--   0        0        0     5080 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/backends.py
--rw-r--r--   0        0        0      529 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/exceptions.py
--rw-r--r--   0        0        0     6434 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/handlers.py
--rw-r--r--   0        0        0     1148 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     2000 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3943 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1329 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     1805 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    11068 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/urls.py
--rw-r--r--   0        0        0      732 2024-04-17 22:59:59.792786 django_azure_auth-1.2.1/azure_auth/views.py
--rw-r--r--   0        0        0     1451 2024-04-17 22:59:59.796786 django_azure_auth-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     6046 1970-01-01 00:00:00.000000 django_azure_auth-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 08:03:57.407501 django_azure_auth-1.2.2/LICENSE
+-rw-r--r--   0        0        0     5327 2024-04-23 08:03:57.407501 django_azure_auth-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 08:03:57.407501 django_azure_auth-1.2.2/azure_auth/__init__.py
+-rw-r--r--   0        0        0      151 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/apps.py
+-rw-r--r--   0        0        0      415 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/backends.py
+-rw-r--r--   0        0        0      529 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/decorators.py
+-rw-r--r--   0        0        0      333 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/exceptions.py
+-rw-r--r--   0        0        0     6575 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/handlers.py
+-rw-r--r--   0        0        0     1148 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/middleware.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2029 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/conftest.py
+-rw-r--r--   0        0        0     3943 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/settings.py
+-rw-r--r--   0        0        0     1409 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/test_decorators.py
+-rw-r--r--   0        0        0     1885 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0    11498 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/test_views.py
+-rw-r--r--   0        0        0     1017 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/tests/urls.py
+-rw-r--r--   0        0        0      324 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/urls.py
+-rw-r--r--   0        0        0      732 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/azure_auth/views.py
+-rw-r--r--   0        0        0     1464 2024-04-23 08:03:57.411501 django_azure_auth-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6308 1970-01-01 00:00:00.000000 django_azure_auth-1.2.2/PKG-INFO
```

### Comparing `django_azure_auth-1.2.1/LICENSE` & `django_azure_auth-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.1/README.md` & `django_azure_auth-1.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/push-actions.yml/badge.svg)
+![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/ci.yml/badge.svg)
+![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)
 
 # Django Azure Auth
 
-### A simple Django app for user authentication with Azure Active Directory.
+### A simple Django app for user authentication with Azure Active Directory/Entra ID.
 
 by Weird Sheep Labs
 
 <a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="50" width="50" /></a>
 
+#### Naming update
+
+In March 2024, [Microsoft renamed Azure Active Directory (Azure AD) to Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/fundamentals/new-name).
+
 ## Description
 
 `django-azure-auth` is a Django app which wraps the great [MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-python)
 package to enable authentication against Microsoft's Azure Active Directory in Django projects.
 
 The app includes `login`, `logout` and `callback` authentication views, a decorator
 to protect individual views, and middleware which allows the entire site to require user
```

### Comparing `django_azure_auth-1.2.1/azure_auth/decorators.py` & `django_azure_auth-1.2.2/azure_auth/decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.1/azure_auth/handlers.py` & `django_azure_auth-1.2.2/azure_auth/handlers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from http import HTTPStatus
+from typing import cast
 
 import msal
 import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
-from django.contrib.auth.models import Group
+from django.contrib.auth.models import AbstractBaseUser, Group
+from django.http import HttpRequest
 
 from azure_auth.exceptions import DjangoAzureAuthException, TokenError
 
-UserModel = get_user_model()
+UserModel = cast(AbstractBaseUser, get_user_model())
 
 
 class AuthHandler:
     """
     Class to interface with `msal` package and execute authentication process.
     """
 
-    def __init__(self, request=None):
+    def __init__(self, request: HttpRequest):
         """
 
         :param request: HttpRequest
         """
         self.request = request
         self.graph_user_endpoint = "https://graph.microsoft.com/v1.0/me"
         self.auth_flow_session_key = "auth_flow"
@@ -38,15 +40,15 @@
         flow = self.msal_app.initiate_auth_code_flow(
             scopes=settings.AZURE_AUTH["SCOPES"],
             redirect_uri=settings.AZURE_AUTH["REDIRECT_URI"],
         )
         self.request.session[self.auth_flow_session_key] = flow
         return flow["auth_uri"]
 
-    def get_token_from_flow(self) -> dict:
+    def get_token_from_flow(self):
         """
         Acquires the token from the auth flow on the session and the content of
         the redirect request from Active Directory.
 
         :return: Token result containing `access_token`/`id_token` and other
         claims, depending on scopes used
         """
@@ -66,15 +68,15 @@
             # Will return `None` if CCA cannot retrieve or generate new token
             token_result = self.msal_app.acquire_token_silent(
                 scopes=settings.AZURE_AUTH["SCOPES"], account=accounts[0]
             )
             self._save_cache()
             return token_result
 
-    def authenticate(self, token: dict) -> UserModel:
+    def authenticate(self, token: dict) -> AbstractBaseUser:
         """
         Helper method to authenticate the user. Gets the Azure user from the
         Microsoft Graph endpoint and gets/creates the associated Django user.
 
         :param token: MSAL auth token dictionary
         :return: Django user instance
         """
@@ -87,17 +89,17 @@
             if azure_user.get("mail", None)
             else azure_user["userPrincipalName"]
         )
 
         # Using `UserModel._default_manager.get_by_natural_key` handles custom
         # user model and `USERNAME_FIELD` setting
         try:
-            user = UserModel._default_manager.get_by_natural_key(email)
+            user = UserModel._default_manager.get_by_natural_key(email)  # type: ignore
         except UserModel.DoesNotExist:
-            user = UserModel._default_manager.create_user(username=email, email=email)
+            user = UserModel._default_manager.create_user(username=email, email=email)  # type: ignore
             user.first_name = attr if (attr := azure_user["givenName"]) else ""
             user.last_name = attr if (attr := azure_user["surname"]) else ""
             user.save()
 
         # Syncing azure token claim roles with django user groups
         # A role mapping in the AZURE_AUTH settings is expected.
         role_mappings = settings.AZURE_AUTH.get("ROLES")
```

### Comparing `django_azure_auth-1.2.1/azure_auth/middleware.py` & `django_azure_auth-1.2.2/azure_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.1/azure_auth/tests/conftest.py` & `django_azure_auth-1.2.2/azure_auth/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from typing import Any
+
 import pytest
 from django.contrib.auth import get_user_model
 from mixer.backend.django import mixer
 
 UserModel = get_user_model()
 
 
 @pytest.fixture(scope="function", autouse=True)
 def user(request):
-    _user = mixer.blend(UserModel)
+    _user: Any = mixer.blend(UserModel)
     _user.username = _user.email
     _user.save()
 
     if request.cls:
         request.cls.user = _user
     return _user
```

### Comparing `django_azure_auth-1.2.1/azure_auth/tests/settings.py` & `django_azure_auth-1.2.2/azure_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.1/azure_auth/tests/test_decorators.py` & `django_azure_auth-1.2.2/azure_auth/tests/test_middleware.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,28 +6,38 @@
 from django.test import TransactionTestCase
 from django.urls import reverse
 
 
 @pytest.mark.django_db
 @pytest.mark.usefixtures("token")
 @patch.object(msal, "ConfidentialClientApplication")
-class TestAzureAuthDecorator(TransactionTestCase):
+class TestAzureAuthMiddleware(TransactionTestCase):
     def test_invalid_token(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = None
-        resp = self.client.get(reverse("decorator_protected"))
+        resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == reverse("azure_auth:login")
+        assert resp.url == reverse("azure_auth:login")  # type: ignore
 
     def test_valid_token_unauthenticated_user(self, mocked_msal_app):
         # Not sure how this situation could arise but test anyway...
 
-        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token
-        resp = self.client.get(reverse("decorator_protected"))
+        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
+        resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == reverse("azure_auth:login")
+        assert resp.url == reverse("azure_auth:login")  # type: ignore
 
     def test_valid_token_authenticated_user(self, mocked_msal_app):
-        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token
-        self.client.force_login(self.user)
+        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
+        self.client.force_login(self.user)  # type: ignore
 
-        resp = self.client.get(reverse("decorator_protected"))
+        resp = self.client.get(reverse("middleware_protected"))
+        assert resp.status_code == HTTPStatus.OK
+
+    def test_public_view(self, mocked_msal_app):
+        mocked_msal_app.return_value.acquire_token_silent.return_value = None
+        resp = self.client.get(reverse("public"))
+        assert resp.status_code == HTTPStatus.OK
+
+    def test_public_external_view(self, mocked_msal_app):
+        mocked_msal_app.return_value.acquire_token_silent.return_value = None
+        resp = self.client.get(reverse("public_external"))
         assert resp.status_code == HTTPStatus.OK
```

### Comparing `django_azure_auth-1.2.1/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.2.2/azure_auth/tests/test_decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,38 +6,28 @@
 from django.test import TransactionTestCase
 from django.urls import reverse
 
 
 @pytest.mark.django_db
 @pytest.mark.usefixtures("token")
 @patch.object(msal, "ConfidentialClientApplication")
-class TestAzureAuthMiddleware(TransactionTestCase):
+class TestAzureAuthDecorator(TransactionTestCase):
     def test_invalid_token(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = None
-        resp = self.client.get(reverse("middleware_protected"))
+        resp = self.client.get(reverse("decorator_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == reverse("azure_auth:login")
+        assert resp.url == reverse("azure_auth:login")  # type: ignore
 
     def test_valid_token_unauthenticated_user(self, mocked_msal_app):
         # Not sure how this situation could arise but test anyway...
 
-        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token
-        resp = self.client.get(reverse("middleware_protected"))
+        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
+        resp = self.client.get(reverse("decorator_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == reverse("azure_auth:login")
+        assert resp.url == reverse("azure_auth:login")  # type: ignore
 
     def test_valid_token_authenticated_user(self, mocked_msal_app):
-        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token
-        self.client.force_login(self.user)
+        mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
+        self.client.force_login(self.user)  # type: ignore
 
-        resp = self.client.get(reverse("middleware_protected"))
-        assert resp.status_code == HTTPStatus.OK
-
-    def test_public_view(self, mocked_msal_app):
-        mocked_msal_app.return_value.acquire_token_silent.return_value = None
-        resp = self.client.get(reverse("public"))
-        assert resp.status_code == HTTPStatus.OK
-
-    def test_public_external_view(self, mocked_msal_app):
-        mocked_msal_app.return_value.acquire_token_silent.return_value = None
-        resp = self.client.get(reverse("public_external"))
+        resp = self.client.get(reverse("decorator_protected"))
         assert resp.status_code == HTTPStatus.OK
```

### Comparing `django_azure_auth-1.2.1/azure_auth/tests/test_views.py` & `django_azure_auth-1.2.2/azure_auth/tests/test_views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import copy
 from http import HTTPStatus
+from typing import cast
 from unittest.mock import patch
 
 import msal
 import pytest
 from django.conf import settings
 from django.contrib.auth import get_user_model
-from django.contrib.auth.models import Group
+from django.contrib.auth.models import AbstractUser, Group
 from django.test import TestCase, TransactionTestCase, override_settings
 from django.urls import reverse
 from mixer.backend.django import Mixer
 
 from azure_auth.exceptions import TokenError
 from azure_auth.handlers import AuthHandler
 
@@ -21,20 +22,20 @@
 @pytest.mark.usefixtures("auth_flow")
 @patch.object(msal, "ConfidentialClientApplication")
 class TestLoginView(TestCase):
     # TODO: What about if user is already logged in and hits this view
     # TODO: Any other breaking flows?
     def test_login(self, mocked_msal_app):
         mocked_msal_app.return_value.initiate_auth_code_flow.return_value = (
-            self.auth_flow
+            self.auth_flow  # type: ignore
         )
         resp = self.client.get(reverse("azure_auth:login"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == self.auth_flow["auth_uri"]
-        assert self.client.session._session == {"auth_flow": self.auth_flow}
+        assert resp.url == self.auth_flow["auth_uri"]  # type: ignore
+        assert self.client.session._session == {"auth_flow": self.auth_flow}  # type: ignore
 
         # MSAL calls
         mocked_msal_app.assert_called_once_with(
             client_id=settings.AZURE_AUTH["CLIENT_ID"],
             client_credential=settings.AZURE_AUTH["CLIENT_SECRET"],
             authority=settings.AZURE_AUTH["AUTHORITY"],
             # Don't care about the `token_cache` object so just pipe it in
@@ -55,21 +56,21 @@
 @patch.object(msal, "ConfidentialClientApplication")
 class TestCallbackView(TransactionTestCase):
     def setUp(self):
         super().setUp()
         # Store in variable first
         # https://docs.djangoproject.com/en/4.0/topics/testing/tools/
         session = self.client.session
-        session["auth_flow"] = self.auth_flow
+        session["auth_flow"] = self.auth_flow  # type: ignore
         session.save()
 
         # Adds a group to existing user that is not part of the token.
         # Should be removed automatically during authentication.
         dummy_group = Group.objects.get_or_create(name="GroupName2")[0]
-        self.user.groups.add(dummy_group)
+        self.user.groups.add(dummy_group)  # type: ignore
 
     def _mocked_response(self, code, json):
         class MockResponse:
             def __init__(self, status_code, data):
                 self.status_code = status_code
                 self.data = data
                 self.ok = True if self.status_code == 200 else False
@@ -94,84 +95,84 @@
             client_credential=settings.AZURE_AUTH["CLIENT_SECRET"],
             authority=settings.AZURE_AUTH["AUTHORITY"],
             # Don't care about the `token_cache` object so just pipe it in
             token_cache=mocked_msal_app.call_args.kwargs["token_cache"],
         )
         m_acf = mocked_msal_app.return_value.acquire_token_by_auth_code_flow
         m_acf.assert_called_once_with(
-            auth_code_flow=self.auth_flow,
+            auth_code_flow=self.auth_flow,  # type: ignore
             # The request for this view comes from the auth server so just pipe
             # `auth_response` in
             auth_response=m_acf.call_args.kwargs["auth_response"],
         )
 
     def _graph_asserts(self, mocked_requests):
         # Graph API calls
         mocked_requests.get.assert_called_once_with(
             "https://graph.microsoft.com/v1.0/me",
-            headers={"Authorization": f"Bearer {self.token['access_token']}"},
+            headers={"Authorization": f"Bearer {self.token['access_token']}"},  # type: ignore
         )
 
     def test_callback_existing_user(
         self, mocked_msal_app, mocked_requests, mocked_cache
     ):
         mocked_msal_app.return_value.acquire_token_by_auth_code_flow.return_value = (
-            self.token
+            self.token  # type: ignore
         )
         mocked_cache.has_state_changed = True
         mocked_cache.serialize = msal.SerializableTokenCache().serialize
         mocked_cache.deserialize = msal.SerializableTokenCache().deserialize
 
         # Graph API response
-        expected_response_json = self._get_graph_response(self.user)
+        expected_response_json = self._get_graph_response(self.user)  # type: ignore
         mocked_requests.get.side_effect = [
             self._mocked_response(HTTPStatus.OK, expected_response_json)
         ]
         resp = self.client.get(reverse("azure_auth:callback"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == settings.LOGIN_REDIRECT_URL
+        assert resp.url == settings.LOGIN_REDIRECT_URL  # type: ignore
         assert "id_token_claims" in self.client.session
 
         # Group creation checks in existing user
         assert Group.objects.filter(name="GroupName1").exists()
         assert Group.objects.filter(name="GroupName2").exists()
-        assert self.user.groups.filter(name="GroupName1").exists()
-        assert not self.user.groups.filter(name="GroupName2").exists()
+        assert self.user.groups.filter(name="GroupName1").exists()  # type: ignore
+        assert not self.user.groups.filter(name="GroupName2").exists()  # type: ignore
 
         self._msal_asserts(mocked_msal_app)
         self._graph_asserts(mocked_requests)
 
     def test_callback_new_user(self, mocked_msal_app, mocked_requests, mocked_cache):
         mocked_msal_app.return_value.acquire_token_by_auth_code_flow.return_value = (
-            self.token
+            self.token  # type: ignore
         )
         mocked_cache.has_state_changed = True
         mocked_cache.serialize = msal.SerializableTokenCache().serialize
         mocked_cache.deserialize = msal.SerializableTokenCache().deserialize
 
         # Generate unsaved new user instance
         custom_mixer = Mixer(commit=False)
-        new_user = custom_mixer.blend(UserModel)
+        new_user = cast(AbstractUser, custom_mixer.blend(UserModel))
         assert len(UserModel.objects.all()) == 1
 
         # Graph API response
         expected_response_json = self._get_graph_response(new_user)
         mocked_requests.get.side_effect = [
             self._mocked_response(HTTPStatus.OK, expected_response_json)
         ]
         resp = self.client.get(reverse("azure_auth:callback"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == settings.LOGIN_REDIRECT_URL
+        assert resp.url == settings.LOGIN_REDIRECT_URL  # type: ignore
         assert "id_token_claims" in self.client.session
 
         self._msal_asserts(mocked_msal_app)
         self._graph_asserts(mocked_requests)
 
         # User creation checks
-        created_user = UserModel.objects.get(email=new_user.email)
+        created_user = cast(AbstractUser, UserModel.objects.get(email=new_user.email))
         assert created_user.username == new_user.email
         assert created_user.first_name == new_user.first_name
         assert created_user.last_name == new_user.last_name
 
         # Group creation checks
         assert Group.objects.filter(name="GroupName1").exists()
         assert Group.objects.filter(name="GroupName2").exists()
@@ -190,15 +191,15 @@
 
         self._msal_asserts(mocked_msal_app)
 
     def test_callback_unauthorized(
         self, mocked_msal_app, mocked_requests, mocked_cache
     ):
         mocked_msal_app.return_value.acquire_token_by_auth_code_flow.return_value = (
-            self.token
+            self.token  # type: ignore
         )
         mocked_cache.has_state_changed = True
         mocked_cache.serialize = msal.SerializableTokenCache().serialize
         mocked_cache.deserialize = msal.SerializableTokenCache().deserialize
 
         # Graph API response
         mocked_requests.get.side_effect = [
@@ -215,56 +216,56 @@
         self._msal_asserts(mocked_msal_app)
         self._graph_asserts(mocked_requests)
 
     def test_callback_inactive_user(
         self, mocked_msal_app, mocked_requests, mocked_cache
     ):
         mocked_msal_app.return_value.acquire_token_by_auth_code_flow.return_value = (
-            self.token
+            self.token  # type: ignore
         )
         mocked_cache.has_state_changed = True
         mocked_cache.serialize = msal.SerializableTokenCache().serialize
         mocked_cache.deserialize = msal.SerializableTokenCache().deserialize
 
         # Graph API response
-        expected_response_json = self._get_graph_response(self.user)
+        expected_response_json = self._get_graph_response(self.user)  # type: ignore
         mocked_requests.get.side_effect = [
             self._mocked_response(HTTPStatus.OK, expected_response_json)
         ]
 
         # Make user inactive
-        self.user.is_active = False
-        self.user.save()
+        self.user.is_active = False  # type: ignore
+        self.user.save()  # type: ignore
         resp = self.client.get(reverse("azure_auth:callback"))
         assert resp.status_code == HTTPStatus.FORBIDDEN
         assert resp.content.decode() == "Invalid email for this app."
 
 
 @patch.object(msal, "ConfidentialClientApplication")
 class TestLogoutView(TestCase):
     # No redirect logout
     no_redirect_logout_settings = copy.deepcopy(settings.AZURE_AUTH)
     del no_redirect_logout_settings["LOGOUT_URI"]
 
     def setUp(self):
         super().setUp()
-        self.client.force_login(self.user)
+        self.client.force_login(self.user)  # type: ignore
 
     def test_logout_with_redirect(self, *args):
         # Check user has been correctly logged in
         assert all(
             [
                 key in self.client.session
                 for key in ["_auth_user_id", "_auth_user_backend", "_auth_user_hash"]
             ]
         )
         resp = self.client.get(reverse("azure_auth:logout"))
         assert resp.status_code == HTTPStatus.FOUND
         assert (
-            resp.url == f"{settings.AZURE_AUTH['AUTHORITY']}/oauth2/v2.0/logout"
+            resp.url == f"{settings.AZURE_AUTH['AUTHORITY']}/oauth2/v2.0/logout"  # type: ignore
             f"?post_logout_redirect_uri={settings.AZURE_AUTH['LOGOUT_URI']}"
         )
         assert not self.client.session.keys()
 
     @override_settings(AZURE_AUTH=no_redirect_logout_settings)
     def test_logout_without_redirect(self, *args):
         # Check user has been correctly logged in
@@ -272,9 +273,9 @@
             [
                 key in self.client.session
                 for key in ["_auth_user_id", "_auth_user_backend", "_auth_user_hash"]
             ]
         )
         resp = self.client.get(reverse("azure_auth:logout"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == f"{settings.AZURE_AUTH['AUTHORITY']}/oauth2/v2.0/logout"
+        assert resp.url == f"{settings.AZURE_AUTH['AUTHORITY']}/oauth2/v2.0/logout"  # type: ignore
         assert not self.client.session.keys()
```

### Comparing `django_azure_auth-1.2.1/azure_auth/tests/urls.py` & `django_azure_auth-1.2.2/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.1/azure_auth/views.py` & `django_azure_auth-1.2.2/azure_auth/views.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.2.1/pyproject.toml` & `django_azure_auth-1.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.2.1"
-description = "A simple Django app for user authentication with Azure Active Directory."
+version = "1.2.2"
+description = "A simple Django app for user authentication with Azure Active Directory/Entra ID."
 authors = ["Weird Sheep Labs <info@weirdsheeplabs.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Weird-Sheep-Labs/django-azure-auth"
-keywords = ['django', 'azure', 'authentication', 'microsoft']
+keywords = ['django', 'azure', 'authentication', 'microsoft', 'entra']
 classifiers = [
     "Framework :: Django",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Information Technology",
 ]
 packages = [
     { include = "azure_auth"},
@@ -19,19 +19,19 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 msal = "^1.18.0"
 Django = ">=3.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
-pre-commit = "^2.19.0"
 pytest-cov = "^3.0.0"
 coverage = {extras = ["toml"], version = "^6.4.1"}
 pytest-django = "^4.5.2"
 mixer = "^7.2.2"
+pre-commit = "~3"
 
 [tool.pytest.ini_options]
 addopts = "--cov . -v --cov-report=html"
 DJANGO_SETTINGS_MODULE = "azure_auth.tests.settings"
 python_files = ["tests.py", "test_*.py",  "*_tests.py"]
 
 [tool.coverage.run]
```

### Comparing `django_azure_auth-1.2.1/PKG-INFO` & `django_azure_auth-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: django-azure-auth
-Version: 1.2.1
-Summary: A simple Django app for user authentication with Azure Active Directory.
+Version: 1.2.2
+Summary: A simple Django app for user authentication with Azure Active Directory/Entra ID.
 Home-page: https://github.com/Weird-Sheep-Labs/django-azure-auth
 License: MIT
-Keywords: django,azure,authentication,microsoft
+Keywords: django,azure,authentication,microsoft,entra
 Author: Weird Sheep Labs
 Author-email: info@weirdsheeplabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
@@ -18,24 +18,29 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2)
 Requires-Dist: msal (>=1.18.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/push-actions.yml/badge.svg)
+![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/ci.yml/badge.svg)
+![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)
 
 # Django Azure Auth
 
-### A simple Django app for user authentication with Azure Active Directory.
+### A simple Django app for user authentication with Azure Active Directory/Entra ID.
 
 by Weird Sheep Labs
 
 <a target="_blank" href="https://weirdsheeplabs.com"><img src="https://weirdsheeplabs.com/android-chrome-192x192.png" height="50" width="50" /></a>
 
+#### Naming update
+
+In March 2024, [Microsoft renamed Azure Active Directory (Azure AD) to Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/fundamentals/new-name).
+
 ## Description
 
 `django-azure-auth` is a Django app which wraps the great [MSAL](https://github.com/AzureAD/microsoft-authentication-library-for-python)
 package to enable authentication against Microsoft's Azure Active Directory in Django projects.
 
 The app includes `login`, `logout` and `callback` authentication views, a decorator
 to protect individual views, and middleware which allows the entire site to require user
```

