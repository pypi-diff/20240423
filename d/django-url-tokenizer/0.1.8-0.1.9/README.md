# Comparing `tmp/django-url-tokenizer-0.1.8.tar.gz` & `tmp/django-url-tokenizer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-url-tokenizer-0.1.8.tar", last modified: Mon Feb 19 18:00:30 2024, max compression
+gzip compressed data, was "django-url-tokenizer-0.1.9.tar", last modified: Mon Feb 19 22:15:58 2024, max compression
```

## Comparing `django-url-tokenizer-0.1.8.tar` & `django-url-tokenizer-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 18:00:30.616082 django-url-tokenizer-0.1.8/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.1.8/LICENSE
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-url-tokenizer-0.1.8/MANIFEST.in
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      489 2024-02-19 18:00:30.616082 django-url-tokenizer-0.1.8/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.1.8/README.md
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 18:00:30.616082 django-url-tokenizer-0.1.8/django_url_tokenizer.egg-info/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      489 2024-02-19 18:00:30.000000 django-url-tokenizer-0.1.8/django_url_tokenizer.egg-info/PKG-INFO
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      582 2024-02-19 18:00:30.000000 django-url-tokenizer-0.1.8/django_url_tokenizer.egg-info/SOURCES.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-02-19 18:00:30.000000 django-url-tokenizer-0.1.8/django_url_tokenizer.egg-info/dependency_links.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       74 2024-02-19 18:00:30.000000 django-url-tokenizer-0.1.8/django_url_tokenizer.egg-info/requires.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2024-02-19 18:00:30.000000 django-url-tokenizer-0.1.8/django_url_tokenizer.egg-info/top_level.txt
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      384 2024-01-31 05:32:07.000000 django-url-tokenizer-0.1.8/pyproject.toml
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2024-02-19 18:00:30.616082 django-url-tokenizer-0.1.8/setup.cfg
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      952 2024-02-19 18:00:02.000000 django-url-tokenizer-0.1.8/setup.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 18:00:30.616082 django-url-tokenizer-0.1.8/urltokenizer/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.1.8/urltokenizer/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.1.8/urltokenizer/apps.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      123 2024-01-26 18:43:14.000000 django-url-tokenizer-0.1.8/urltokenizer/enums.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1333 2024-02-19 04:59:05.000000 django-url-tokenizer-0.1.8/urltokenizer/exceptions.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1440 2024-01-31 05:06:23.000000 django-url-tokenizer-0.1.8/urltokenizer/managers.py
-drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 18:00:30.616082 django-url-tokenizer-0.1.8/urltokenizer/migrations/
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.1.8/urltokenizer/migrations/__init__.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2150 2024-02-19 05:05:29.000000 django-url-tokenizer-0.1.8/urltokenizer/mixins.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      992 2024-02-19 06:29:22.000000 django-url-tokenizer-0.1.8/urltokenizer/models.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3642 2024-02-19 06:00:09.000000 django-url-tokenizer-0.1.8/urltokenizer/serializers.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)     5674 2024-02-19 05:47:26.000000 django-url-tokenizer-0.1.8/urltokenizer/token_generator.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)    13479 2024-02-19 17:59:42.000000 django-url-tokenizer-0.1.8/urltokenizer/tokenizer.py
--rw-r--r--   0 nibblex   (1000) nibblex   (1000)      419 2024-01-26 19:32:25.000000 django-url-tokenizer-0.1.8/urltokenizer/utils.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 22:15:58.233064 django-url-tokenizer-0.1.9/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1074 2023-07-13 01:29:20.000000 django-url-tokenizer-0.1.9/LICENSE
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       34 2023-07-14 23:44:42.000000 django-url-tokenizer-0.1.9/MANIFEST.in
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      489 2024-02-19 22:15:58.233064 django-url-tokenizer-0.1.9/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      144 2023-07-13 01:29:20.000000 django-url-tokenizer-0.1.9/README.md
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 22:15:58.233064 django-url-tokenizer-0.1.9/django_url_tokenizer.egg-info/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      489 2024-02-19 22:15:58.000000 django-url-tokenizer-0.1.9/django_url_tokenizer.egg-info/PKG-INFO
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      582 2024-02-19 22:15:58.000000 django-url-tokenizer-0.1.9/django_url_tokenizer.egg-info/SOURCES.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        1 2024-02-19 22:15:58.000000 django-url-tokenizer-0.1.9/django_url_tokenizer.egg-info/dependency_links.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       74 2024-02-19 22:15:58.000000 django-url-tokenizer-0.1.9/django_url_tokenizer.egg-info/requires.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       13 2024-02-19 22:15:58.000000 django-url-tokenizer-0.1.9/django_url_tokenizer.egg-info/top_level.txt
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      384 2024-01-31 05:32:07.000000 django-url-tokenizer-0.1.9/pyproject.toml
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)       38 2024-02-19 22:15:58.233064 django-url-tokenizer-0.1.9/setup.cfg
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      952 2024-02-19 21:53:19.000000 django-url-tokenizer-0.1.9/setup.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 22:15:58.233064 django-url-tokenizer-0.1.9/urltokenizer/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.1.9/urltokenizer/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      156 2023-07-13 00:48:39.000000 django-url-tokenizer-0.1.9/urltokenizer/apps.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      123 2024-01-26 18:43:14.000000 django-url-tokenizer-0.1.9/urltokenizer/enums.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1333 2024-02-19 04:59:05.000000 django-url-tokenizer-0.1.9/urltokenizer/exceptions.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     1440 2024-01-31 05:06:23.000000 django-url-tokenizer-0.1.9/urltokenizer/managers.py
+drwxr-xr-x   0 nibblex   (1000) nibblex   (1000)        0 2024-02-19 22:15:58.233064 django-url-tokenizer-0.1.9/urltokenizer/migrations/
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)        0 2023-07-13 00:48:39.000000 django-url-tokenizer-0.1.9/urltokenizer/migrations/__init__.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     2150 2024-02-19 05:05:29.000000 django-url-tokenizer-0.1.9/urltokenizer/mixins.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      992 2024-02-19 21:09:38.000000 django-url-tokenizer-0.1.9/urltokenizer/models.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     3642 2024-02-19 06:00:09.000000 django-url-tokenizer-0.1.9/urltokenizer/serializers.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)     5829 2024-02-19 21:51:41.000000 django-url-tokenizer-0.1.9/urltokenizer/token_generator.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)    13051 2024-02-19 22:05:20.000000 django-url-tokenizer-0.1.9/urltokenizer/tokenizer.py
+-rw-r--r--   0 nibblex   (1000) nibblex   (1000)      419 2024-01-26 19:32:25.000000 django-url-tokenizer-0.1.9/urltokenizer/utils.py
```

### Comparing `django-url-tokenizer-0.1.8/LICENSE` & `django-url-tokenizer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.1.8/django_url_tokenizer.egg-info/SOURCES.txt` & `django-url-tokenizer-0.1.9/django_url_tokenizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.1.8/setup.py` & `django-url-tokenizer-0.1.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name="django-url-tokenizer",
-    version="0.1.8",
+    version="0.1.9",
     author="Sergio Rodríguez",
     author_email="srodriguez3441@gmail.com",
     description="""A python package that provides a Django app that allows you to
     generate tokenized urls and send them to users via email.""",
     url="https://github.com/nibblex/django-url-tokenizer",
     packages=setuptools.find_packages(),
     license="MIT",
```

### Comparing `django-url-tokenizer-0.1.8/urltokenizer/exceptions.py` & `django-url-tokenizer-0.1.9/urltokenizer/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.1.8/urltokenizer/managers.py` & `django-url-tokenizer-0.1.9/urltokenizer/managers.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.1.8/urltokenizer/mixins.py` & `django-url-tokenizer-0.1.9/urltokenizer/mixins.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.1.8/urltokenizer/models.py` & `django-url-tokenizer-0.1.9/urltokenizer/models.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.1.8/urltokenizer/serializers.py` & `django-url-tokenizer-0.1.9/urltokenizer/serializers.py`

 * *Files identical despite different names*

### Comparing `django-url-tokenizer-0.1.8/urltokenizer/token_generator.py` & `django-url-tokenizer-0.1.9/urltokenizer/token_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 from datetime import datetime
 
 from django.conf import settings
 from django.utils.crypto import constant_time_compare, salted_hmac
 from django.utils.http import base36_to_int, int_to_base36
 
 from .exceptions import ErrorCode, URLTokenizerError
-from .utils import str_import
+from .utils import SETTINGS, str_import, from_config
 
 
 class TokenGenerator:
     """
     Strategy object used to generate and check tokens.
     """
 
     key_salt = "django.contrib.auth.tokens.PasswordResetTokenGenerator"
     algorithm = None
     _secret = None
 
-    def __init__(
-        self,
-        attributes: list = [],
-        check_preconditions: list = [],
-        callbacks: list = [],
-        timeout: int = 60,
-    ):
+    def __init__(self, token_config: dict = {}):
+        check_preconditions = str_import(
+            SETTINGS.get("CHECK_PRECONDITIONS", [])
+            + token_config.get("check_preconditions", [])
+        )
+
         self.algorithm = self.algorithm or "sha256"
-        self.attributes = attributes
-        self.check_preconditions = str_import(check_preconditions)
-        self.callbacks = callbacks
-        self.timeout = timeout
+        self.attributes = from_config(token_config, "attributes", [])
+        self.check_preconditions = check_preconditions
+        self.callbacks = from_config(token_config, "callbacks", [])
+        self.timeout = from_config(token_config, "timeout", 60)
 
     @property
     def secret(self):
         return self._secret or settings.SECRET_KEY
 
     @secret.setter
     def secret(self, value):
```

### Comparing `django-url-tokenizer-0.1.8/urltokenizer/tokenizer.py` & `django-url-tokenizer-0.1.9/urltokenizer/tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,20 +84,23 @@
         return get_user_model()
 
     def __init__(self, token_type: str | Enum | None = None):
         self.token_type = self._parse_token_type(token_type)
         # at this point token_type is either None or a string
 
         token_config = self._get_token_config(SETTINGS, self.token_type)
-        self._token_generator = self._get_token_generator(token_config)
+        self._token_generator = TokenGenerator(token_config)
 
         # token
+        self.validate_token_type = SETTINGS.get("VALIDATE_TOKEN_TYPE", True)
         self.user_serializer = from_config(token_config, "user_serializer", None)
         self.encoding_field = from_config(token_config, "encoding_field", "pk")
         self.fail_silently = from_config(token_config, "fail_silently", False)
+
+        # logging
         self.logging_enabled = from_config(token_config, "logging_enabled", False)
         self.check_logs = from_config(token_config, "check_logs", False)
 
         # url
         self.path = from_config(token_config, "path", "").strip("/")
         self.domain = from_config(token_config, "domain", "localhost")
         self.protocol = from_config(token_config, "protocol", "http")
@@ -119,80 +122,79 @@
             "email_subject",
             "link generated with django-url-tokenizer",
         )
 
         # sms
         self.phone_field = from_config(token_config, "phone_field", "phone")
 
+    # initialization
+
     @staticmethod
     def _parse_token_type(token_type: str | Enum | None) -> str | None:
         if isinstance(token_type, str):
             token_type = token_type.strip().lower()
         elif isinstance(token_type, Enum):
             token_type = token_type.value.strip().lower()
         elif token_type is not None:
             raise ValueError(_("'token_type' must be either a string or Enum"))
 
         return token_type
 
-    @staticmethod
-    def _get_token_config(settings_: dict, token_type: str | None) -> dict:
+    def _get_token_config(self, settings_: dict, token_type: str | None) -> dict:
         TOKEN_CONFIG = settings_.get("TOKEN_CONFIG", {})
 
         # avoid empty token_type
         if any(key.strip() == "" for key in TOKEN_CONFIG.keys()):
             raise ImproperlyConfigured(
                 _("TOKEN_CONFIG cannot contain blank 'token_type'.")
             )
 
         if token_type is None:
             return TOKEN_CONFIG.get("default", {})
 
+        # validate token_type
         token_config = TOKEN_CONFIG.get(token_type, None)
-        validate_token_type = settings_.get("VALIDATE_TOKEN_TYPE", True)
-
-        if token_config is None and validate_token_type:
+        if token_config is None and self.validate_token_type:
             raise URLTokenizerError(ErrorCode.invalid_token_type, token_type=token_type)
 
         return token_config or TOKEN_CONFIG.get("default", {})
 
-    @staticmethod
-    def _get_token_generator(token_config: dict) -> TokenGenerator:
-        check_preconditions = str_import(
-            SETTINGS.get("CHECK_PRECONDITIONS", [])
-            + token_config.get("check_preconditions", [])
-        )
+    # helpers
 
-        return TokenGenerator(
-            attributes=from_config(token_config, "attributes", []),
-            check_preconditions=check_preconditions,
-            callbacks=from_config(token_config, "callbacks", []),
-            timeout=from_config(token_config, "timeout", 60),
-        )
+    def _check_log(self, uidb64: str, token: str) -> Log | None:
+        hash = hashlib.sha256(force_bytes(uidb64 + token)).hexdigest()
+        try:
+            log = Log.objects.filter(hash=hash).first()
+        except ProgrammingError:
+            return None
 
-    # helpers
+        if not log or log.checked:
+            return None
+
+        log.checked_at = timezone.now()
+        log.save(update_fields=["checked_at"])
+
+        return log
 
     def _update_user_data(self, user, user_data: dict | None):
         if user_data and self.user_serializer:
             user_serializer = import_string(self.user_serializer)
-            user = user_serializer(user, data=user_data, partial=True)
+            serializer = user_serializer(user, data=user_data, partial=True)
 
             try:
-                user.is_valid(raise_exception=True)
+                serializer.is_valid(raise_exception=True)
             except Exception as e:
                 if not self.fail_silently:
                     raise URLTokenizerError(
                         ErrorCode.user_serializer_error,
                         serializer=self.user_serializer,
                         context={"exception": e},
                     ) from e
             else:
-                user.save()
-
-        return user
+                serializer.save()
 
     # encoding
 
     @staticmethod
     def encode(s: Any) -> str:
         return urlsafe_base64_encode(force_bytes(s))
 
@@ -374,30 +376,17 @@
         # check token
         if not self._token_generator.check_token(
             user, token, fail_silently=fail_silently
         ):
             return None, None
 
         # check log
-        log = None
-        if self.check_logs:
-            hash = hashlib.sha256(force_bytes(uidb64 + token)).hexdigest()
-            try:
-                log = Log.objects.filter(hash=hash).first()
-            except ProgrammingError:
-                return user, None
-
-            if not log:
-                return None, None
-
-            if log.checked:
-                return None, log
-
-            log.checked_at = timezone.now()
-            log.save(update_fields=["checked_at"])
+        log = self._check_log(uidb64, token)
+        if not log and self.check_logs:
+            return None, None
 
         # update user data
         self._update_user_data(user, user_data)
 
         return user, log
 
     def run_callbacks(
```

