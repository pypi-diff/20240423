# Comparing `tmp/django-tastypie-0.9.7.tar.gz` & `tmp/django-tastypie-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-tastypie-0.9.7.tar", last modified: Wed Mar  9 08:18:26 2011, max compression
+gzip compressed data, was "dist/django-tastypie-0.9.9.tar", last modified: Sat May 21 01:10:30 2011, max compression
```

## Comparing `django-tastypie-0.9.7.tar` & `django-tastypie-0.9.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-03-09 08:18:26.000000 django-tastypie-0.9.7/
--rw-r--r--   0 daniel     (501) staff       (20)      666 2011-03-09 08:18:26.000000 django-tastypie-0.9.7/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      968 2011-03-09 08:17:46.000000 django-tastypie-0.9.7/setup.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-03-09 08:18:26.000000 django-tastypie-0.9.7/tastypie/
--rw-r--r--   0 daniel     (501) staff       (20)       83 2011-03-09 08:17:59.000000 django-tastypie-0.9.7/tastypie/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)      251 2011-02-19 20:49:18.000000 django-tastypie-0.9.7/tastypie/admin.py
--rw-r--r--   0 daniel     (501) staff       (20)     6259 2011-02-19 20:49:18.000000 django-tastypie-0.9.7/tastypie/api.py
--rw-r--r--   0 daniel     (501) staff       (20)     5063 2011-02-19 20:49:18.000000 django-tastypie-0.9.7/tastypie/authentication.py
--rw-r--r--   0 daniel     (501) staff       (20)     2299 2011-02-19 20:49:18.000000 django-tastypie-0.9.7/tastypie/authorization.py
--rw-r--r--   0 daniel     (501) staff       (20)      501 2011-02-19 20:49:18.000000 django-tastypie-0.9.7/tastypie/bundle.py
--rw-r--r--   0 daniel     (501) staff       (20)      926 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/cache.py
--rw-r--r--   0 daniel     (501) staff       (20)      168 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/constants.py
--rw-r--r--   0 daniel     (501) staff       (20)     1809 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/exceptions.py
--rw-r--r--   0 daniel     (501) staff       (20)    23824 2011-03-09 07:25:25.000000 django-tastypie-0.9.7/tastypie/fields.py
--rw-r--r--   0 daniel     (501) staff       (20)     1162 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/http.py
--rw-r--r--   0 daniel     (501) staff       (20)     1906 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/models.py
--rw-r--r--   0 daniel     (501) staff       (20)     5842 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/paginator.py
--rw-r--r--   0 daniel     (501) staff       (20)    60677 2011-03-09 08:05:51.000000 django-tastypie-0.9.7/tastypie/resources.py
--rw-r--r--   0 daniel     (501) staff       (20)    14955 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/serializers.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-03-09 08:18:26.000000 django-tastypie-0.9.7/tastypie/templates/
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-03-09 08:18:26.000000 django-tastypie-0.9.7/tastypie/templates/tastypie/
--rw-r--r--   0 daniel     (501) staff       (20)      846 2011-03-09 07:48:07.000000 django-tastypie-0.9.7/tastypie/templates/tastypie/basic.html
--rw-r--r--   0 daniel     (501) staff       (20)       71 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/templates/tastypie/detail.html
--rw-r--r--   0 daniel     (501) staff       (20)       71 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/templates/tastypie/list.html
--rw-r--r--   0 daniel     (501) staff       (20)     4560 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/throttle.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-03-09 08:18:26.000000 django-tastypie-0.9.7/tastypie/utils/
--rw-r--r--   0 daniel     (501) staff       (20)      268 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/utils/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)      291 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/utils/dict.py
--rw-r--r--   0 daniel     (501) staff       (20)      984 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/utils/formatting.py
--rw-r--r--   0 daniel     (501) staff       (20)     1763 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/utils/mime.py
--rw-r--r--   0 daniel     (501) staff       (20)      162 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/utils/urls.py
--rw-r--r--   0 daniel     (501) staff       (20)     6223 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/utils/validate_jsonp.py
--rw-r--r--   0 daniel     (501) staff       (20)     2006 2011-02-19 20:49:19.000000 django-tastypie-0.9.7/tastypie/validation.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-05-21 01:10:30.000000 django-tastypie-0.9.9/
+-rw-r--r--   0 daniel     (501) staff       (20)      704 2011-05-21 01:10:30.000000 django-tastypie-0.9.9/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)     1047 2011-05-20 17:46:49.000000 django-tastypie-0.9.9/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-05-21 01:10:30.000000 django-tastypie-0.9.9/tastypie/
+-rw-r--r--   0 daniel     (501) staff       (20)       83 2011-05-20 17:46:49.000000 django-tastypie-0.9.9/tastypie/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)      251 2011-02-19 20:49:18.000000 django-tastypie-0.9.9/tastypie/admin.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6274 2011-05-20 16:58:46.000000 django-tastypie-0.9.9/tastypie/api.py
+-rw-r--r--   0 daniel     (501) staff       (20)     9091 2011-05-20 16:39:43.000000 django-tastypie-0.9.9/tastypie/authentication.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2299 2011-02-19 20:49:18.000000 django-tastypie-0.9.9/tastypie/authorization.py
+-rw-r--r--   0 daniel     (501) staff       (20)      501 2011-02-19 20:49:18.000000 django-tastypie-0.9.9/tastypie/bundle.py
+-rw-r--r--   0 daniel     (501) staff       (20)      926 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/cache.py
+-rw-r--r--   0 daniel     (501) staff       (20)      168 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/constants.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1806 2011-05-14 03:33:07.000000 django-tastypie-0.9.9/tastypie/exceptions.py
+-rw-r--r--   0 daniel     (501) staff       (20)    24112 2011-05-20 17:44:18.000000 django-tastypie-0.9.9/tastypie/fields.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1162 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/http.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1906 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/models.py
+-rw-r--r--   0 daniel     (501) staff       (20)     5842 2011-05-14 03:33:07.000000 django-tastypie-0.9.9/tastypie/paginator.py
+-rw-r--r--   0 daniel     (501) staff       (20)    64989 2011-05-19 03:09:37.000000 django-tastypie-0.9.9/tastypie/resources.py
+-rw-r--r--   0 daniel     (501) staff       (20)    14955 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/serializers.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-05-21 01:10:29.000000 django-tastypie-0.9.9/tastypie/templates/
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-05-21 01:10:30.000000 django-tastypie-0.9.9/tastypie/templates/tastypie/
+-rw-r--r--   0 daniel     (501) staff       (20)      846 2011-05-14 03:33:07.000000 django-tastypie-0.9.9/tastypie/templates/tastypie/basic.html
+-rw-r--r--   0 daniel     (501) staff       (20)       71 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/templates/tastypie/detail.html
+-rw-r--r--   0 daniel     (501) staff       (20)       71 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/templates/tastypie/list.html
+-rw-r--r--   0 daniel     (501) staff       (20)     4560 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/throttle.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2011-05-21 01:10:30.000000 django-tastypie-0.9.9/tastypie/utils/
+-rw-r--r--   0 daniel     (501) staff       (20)      268 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/utils/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)      291 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/utils/dict.py
+-rw-r--r--   0 daniel     (501) staff       (20)      997 2011-05-14 03:33:07.000000 django-tastypie-0.9.9/tastypie/utils/formatting.py
+-rw-r--r--   0 daniel     (501) staff       (20)     1763 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/utils/mime.py
+-rw-r--r--   0 daniel     (501) staff       (20)      162 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/utils/urls.py
+-rw-r--r--   0 daniel     (501) staff       (20)     6223 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/utils/validate_jsonp.py
+-rw-r--r--   0 daniel     (501) staff       (20)     2006 2011-02-19 20:49:19.000000 django-tastypie-0.9.9/tastypie/validation.py
```

### Comparing `django-tastypie-0.9.7/PKG-INFO` & `django-tastypie-0.9.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-tastypie
-Version: 0.9.7
+Version: 0.9.9
 Summary: A flexible & capable API layer for Django.
 Home-page: http://github.com/toastdriven/django-tastypie/
 Author: Daniel Lindsley
 Author-email: daniel@toastdriven.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
@@ -13,8 +13,9 @@
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Utilities
 Requires: mimeparse
-Requires: python_dateutil
+Requires: python_dateutil(>=1.5, < 2.0)
+Requires: python_digest
```

### Comparing `django-tastypie-0.9.7/tastypie/api.py` & `django-tastypie-0.9.9/tastypie/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def __init__(self, api_name="v1"):
         self.api_name = api_name
         self._registry = {}
         self._canonicals = {}
     
     def register(self, resource, canonical=True):
         """
-        Registers a ``Resource`` subclass with the API.
+        Registers an instance of a ``Resource`` subclass with the API.
         
         Optionally accept a ``canonical`` argument, which indicates that the
         resource being registered is the canonical variant. Defaults to
         ``True``.
         """
         resource_name = getattr(resource._meta, 'resource_name', None)
```

### Comparing `django-tastypie-0.9.7/tastypie/authentication.py` & `django-tastypie-0.9.9/tastypie/throttle.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,132 @@
-import base64
-import hmac
-from django.contrib.auth import authenticate
-from http import HttpUnauthorized
+import time
+from django.core.cache import cache
 
 
-class Authentication(object):
+class BaseThrottle(object):
     """
-    A simple base class to establish the protocol for auth.
+    A simplified, swappable base class for throttling.
     
-    By default, this indicates the user is always authenticated.
+    Does nothing save for simulating the throttling API and implementing
+    some common bits for the subclasses.
+    
+    Accepts a number of optional kwargs::
+    
+        * ``throttle_at`` - the number of requests at which the user should
+          be throttled. Default is 150 requests.
+        * ``timeframe`` - the length of time (in seconds) in which the user
+          make up to the ``throttle_at`` requests. Default is 3600 seconds (
+          1 hour).
+        * ``expiration`` - the length of time to retain the times the user
+          has accessed the api in the cache. Default is 604800 (1 week).
     """
-    def is_authenticated(self, request, **kwargs):
-        """
-        Identifies if the user is authenticated to continue or not.
+    def __init__(self, throttle_at=150, timeframe=3600, expiration=None):
+        self.throttle_at = throttle_at
+        # In seconds, please.
+        self.timeframe = timeframe
         
-        Should return either ``True`` if allowed, ``False`` if not or an
-        ``HttpResponse`` if you need something custom.
-        """
-        return True
+        if expiration is None:
+            # Expire in a week.
+            expiration = 604800
+        
+        self.expiration = int(expiration)
     
-    def get_identifier(self, request):
+    def convert_identifier_to_key(self, identifier):
         """
-        Provides a unique string identifier for the requestor.
-        
-        This implementation returns a combination of IP address and hostname.
+        Takes an identifier (like a username or IP address) and converts it
+        into a key usable by the cache system.
         """
-        return "%s_%s" % (request.META.get('REMOTE_ADDR', 'noaddr'), request.META.get('REMOTE_HOST', 'nohost'))
-
-
-class BasicAuthentication(Authentication):
-    """
-    Handles HTTP Basic auth against a specific auth backend if provided,
-    or against all configured authentication backends using the
-    ``authenticate`` method from ``django.contrib.auth``.
+        bits = []
+        
+        for char in identifier:
+            if char.isalnum() or char in ['_', '.', '-']:
+                bits.append(char)
+        
+        safe_string = ''.join(bits)
+        return "%s_accesses" % safe_string
     
-    Optional keyword arguments:
-
-    ``backend``
-        If specified, use a specific ``django.contrib.auth`` backend instead
-        of checking all backends specified in the ``AUTHENTICATION_BACKENDS``
-        setting.
-    ``realm``
-        The realm to use in the ``HttpUnauthorized`` response.  Default:
-        ``django-tastypie``.
-    """
-    def __init__(self, backend=None, realm='django-tastypie'):
-        self.backend = backend
-        self.realm = realm
-
-    def _unauthorized(self):
-        response = HttpUnauthorized()
-        # FIXME: Sanitize realm.
-        response['WWW-Authenticate'] = 'Basic Realm="%s"' % self.realm
-        return response
-
-    def is_authenticated(self, request, **kwargs):
+    def should_be_throttled(self, identifier, **kwargs):
         """
-        Checks a user's basic auth credentials against the current
-        Django auth backend.
+        Returns whether or not the user has exceeded their throttle limit.
         
-        Should return either ``True`` if allowed, ``False`` if not or an
-        ``HttpResponse`` if you need something custom.
+        Always returns ``False``, as this implementation does not actually
+        throttle the user.
         """
-        if not request.META.get('HTTP_AUTHORIZATION'):
-            return self._unauthorized()
-        
-        try:
-            (auth_type, data) = request.META['HTTP_AUTHORIZATION'].split()
-            if auth_type != 'Basic':
-                return self._unauthorized()
-            user_pass = base64.b64decode(data)
-        except:
-            return self._unauthorized()
-
-        bits = user_pass.split(':')
-        
-        if len(bits) != 2:
-            return self._unauthorized()
-
-        if self.backend:
-            user = self.backend.authenticate(username=bits[0], password=bits[1])
-        else:
-            user = authenticate(username=bits[0], password=bits[1])
-
-        if user is None:
-            return self._unauthorized()
-
-        request.user = user
-
-        return True
+        return False
     
-    def get_identifier(self, request):
+    def accessed(self, identifier, **kwargs):
         """
-        Provides a unique string identifier for the requestor.
+        Handles recording the user's access.
         
-        This implementation returns the user's basic auth username.
+        Does nothing in this implementation.
         """
-        return request.META.get('REMOTE_USER', 'nouser')
+        pass
 
 
-class ApiKeyAuthentication(Authentication):
+class CacheThrottle(BaseThrottle):
     """
-    Handles API key auth, in which a user provides a username & API key.
-    
-    Uses the ``ApiKey`` model that ships with tastypie. If you wish to use
-    a different model, override the ``get_key`` method to perform the key check
-    as suits your needs.
+    A throttling mechanism that uses just the cache.
     """
-    def _unauthorized(self):
-        return HttpUnauthorized()
-
-    def is_authenticated(self, request, **kwargs):
+    def should_be_throttled(self, identifier, **kwargs):
         """
-        Finds the user and checks their API key.
+        Returns whether or not the user has exceeded their throttle limit.
+        
+        Maintains a list of timestamps when the user accessed the api within
+        the cache.
         
-        Should return either ``True`` if allowed, ``False`` if not or an
-        ``HttpResponse`` if you need something custom.
+        Returns ``False`` if the user should NOT be throttled or ``True`` if
+        the user should be throttled.
         """
-        from django.contrib.auth.models import User
+        key = self.convert_identifier_to_key(identifier)
         
-        username = request.GET.get('username') or request.POST.get('username')
-        api_key = request.GET.get('api_key') or request.POST.get('api_key')
+        # Make sure something is there.
+        cache.add(key, [])
         
-        if not username or not api_key:
-            return self._unauthorized()
+        # Weed out anything older than the timeframe.
+        minimum_time = int(time.time()) - int(self.timeframe)
+        times_accessed = [access for access in cache.get(key) if access >= minimum_time]
+        cache.set(key, times_accessed, self.expiration)
         
-        try:
-            user = User.objects.get(username=username)
-        except (User.DoesNotExist, User.MultipleObjectsReturned):
-            return self._unauthorized()
-
-        request.user = user
-
-        return self.get_key(user, api_key)
+        if len(times_accessed) >= int(self.throttle_at):
+            # Throttle them.
+            return True
+        
+        # Let them through.
+        return False
     
-    def get_key(self, user, api_key):
-        """
-        Attempts to find the API key for the user. Uses ``ApiKey`` by default
-        but can be overridden.
+    def accessed(self, identifier, **kwargs):
         """
-        from tastypie.models import ApiKey
+        Handles recording the user's access.
         
-        try:
-            key = ApiKey.objects.get(user=user, key=api_key)
-        except ApiKey.DoesNotExist:
-            return self._unauthorized()
-        
-        return True
+        Stores the current timestamp in the "accesses" list within the cache.
+        """
+        key = self.convert_identifier_to_key(identifier)
+        times_accessed = cache.get(key, [])
+        times_accessed.append(int(time.time()))
+        cache.set(key, times_accessed, self.expiration)
+
+
+class CacheDBThrottle(CacheThrottle):
+    """
+    A throttling mechanism that uses the cache for actual throttling but
+    writes-through to the database.
     
-    def get_identifier(self, request):
+    This is useful for tracking/aggregating usage through time, to possibly
+    build a statistics interface or a billing mechanism.
+    """
+    def accessed(self, identifier, **kwargs):
         """
-        Provides a unique string identifier for the requestor.
+        Handles recording the user's access.
         
-        This implementation returns the user's username.
+        Does everything the ``CacheThrottle`` class does, plus logs the
+        access within the database using the ``ApiAccess`` model.
         """
-        return request.REQUEST.get('username', 'nouser')
+        # Do the import here, instead of top-level, so that the model is
+        # only required when using this throttling mechanism.
+        from tastypie.models import ApiAccess
+        super(CacheDBThrottle, self).accessed(identifier, **kwargs)
+        # Write out the access to the DB for logging purposes.
+        ApiAccess.objects.create(
+            identifier=identifier,
+            url=kwargs.get('url', ''),
+            request_method=kwargs.get('request_method', '')
+        )
```

### Comparing `django-tastypie-0.9.7/tastypie/authorization.py` & `django-tastypie-0.9.9/tastypie/authorization.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/cache.py` & `django-tastypie-0.9.9/tastypie/cache.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/exceptions.py` & `django-tastypie-0.9.9/tastypie/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     pass
 
 
 class BlueberryFillingFound(TastypieError):
     pass
 
 
-class InvalidFilterError(TastypieError):
+class InvalidFilterError(BadRequest):
     """
     Raised when the end user attempts to use a filter that has not be
     explicitly allowed.
     """
     pass
```

### Comparing `django-tastypie-0.9.7/tastypie/fields.py` & `django-tastypie-0.9.9/tastypie/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dateutil.parser import parse
+from decimal import Decimal
 import re
 from django.core.exceptions import ObjectDoesNotExist, MultipleObjectsReturned
 from django.utils import datetime_safe, importlib
 from tastypie.bundle import Bundle
 from tastypie.exceptions import ApiFieldError, NotFound
 from tastypie.utils import dict_strip_unicode_keys
 
@@ -94,31 +95,31 @@
                 previous_object = current_object
                 current_object = getattr(current_object, attr, None)
                 
                 if current_object is None:
                     if self.has_default():
                         current_object = self._default
                         # Fall out of the loop, given any further attempts at
-                        # accesses will fail misreably.
+                        # accesses will fail miserably.
                         break
                     elif self.null:
                         current_object = None
                         # Fall out of the loop, given any further attempts at
-                        # accesses will fail misreably.
+                        # accesses will fail miserably.
                         break
                     else:
                         raise ApiFieldError("The object '%r' has an empty attribute '%s' and doesn't allow a default or null value." % (previous_object, attr))
             
             if callable(current_object):
-                return current_object()
+                current_object = current_object()
             
-            return current_object
+            return self.convert(current_object)
         
         if self.has_default():
-            return self.default
+            return self.convert(self.default)
         else:
             return None
     
     def convert(self, value):
         """
         Handles conversion between the data found and the type of the field.
         
@@ -132,15 +133,17 @@
         Takes data stored in the bundle for the field and returns it. Used for
         taking simple data and building a instance object.
         """
         if self.readonly:
             return None
         
         if not bundle.data.has_key(self.instance_name):
-            if hasattr(bundle.obj, self.instance_name):
+            if self.attribute and getattr(bundle.obj, self.attribute, None):
+                return getattr(bundle.obj, self.attribute)
+            elif self.instance_name and hasattr(bundle.obj, self.instance_name):
                 return getattr(bundle.obj, self.instance_name)
             elif self.has_default():
                 if callable(self._default):
                     return self._default()
                 
                 return self._default
             elif self.null:
@@ -156,17 +159,14 @@
     A text field of arbitrary length.
     
     Covers both ``models.CharField`` and ``models.TextField``.
     """
     dehydrated_type = 'string'
     help_text = 'Unicode string data. Ex: "Hello World"'
     
-    def dehydrate(self, obj):
-        return self.convert(super(CharField, self).dehydrate(obj))
-    
     def convert(self, value):
         if value is None:
             return None
         
         return unicode(value)
 
 
@@ -175,17 +175,14 @@
     A file-related field.
     
     Covers both ``models.FileField`` and ``models.ImageField``.
     """
     dehydrated_type = 'string'
     help_text = 'A file URL as a string. Ex: "http://media.example.com/media/photos/my_photo.jpg"'
     
-    def dehydrate(self, obj):
-        return self.convert(super(FileField, self).dehydrate(obj))
-    
     def convert(self, value):
         if value is None:
             return None
         
         try:
             # Try to return the URL if it's a ``File``, falling back to the string
             # itself if it's been overridden or is a default.
@@ -200,70 +197,100 @@
     
     Covers ``models.IntegerField``, ``models.PositiveIntegerField``,
     ``models.PositiveSmallIntegerField`` and ``models.SmallIntegerField``.
     """
     dehydrated_type = 'integer'
     help_text = 'Integer data. Ex: 2673'
     
-    def dehydrate(self, obj):
-        return self.convert(super(IntegerField, self).dehydrate(obj))
-    
     def convert(self, value):
         if value is None:
             return None
         
         return int(value)
 
 
 class FloatField(ApiField):
     """
     A floating point field.
     """
     dehydrated_type = 'float'
     help_text = 'Floating point numeric data. Ex: 26.73'
     
-    def dehydrate(self, obj):
-        return self.convert(super(FloatField, self).dehydrate(obj))
-    
     def convert(self, value):
         if value is None:
             return None
         
         return float(value)
 
 
+class DecimalField(ApiField):
+    """
+    A decimal field.
+    """
+    dehydrated_type = 'decimal'
+    help_text = 'Fixed precision numeric data. Ex: 26.73'
+    
+    def convert(self, value):
+        if value is None:
+            return None
+        
+        return Decimal(value)
+
+
 class BooleanField(ApiField):
     """
     A boolean field.
     
     Covers both ``models.BooleanField`` and ``models.NullBooleanField``.
     """
     dehydrated_type = 'boolean'
     help_text = 'Boolean data. Ex: True'
     
-    def dehydrate(self, obj):
-        return self.convert(super(BooleanField, self).dehydrate(obj))
-    
     def convert(self, value):
         if value is None:
             return None
         
         return bool(value)
 
 
+class ListField(ApiField):
+    """
+    A list field.
+    """
+    dehydrated_type = 'list'
+    help_text = "A list of data. Ex: ['abc', 26.73, 8]"
+    
+    def convert(self, value):
+        if value is None:
+            return None
+        
+        return list(value)
+
+
+class DictField(ApiField):
+    """
+    A dictionary field.
+    """
+    dehydrated_type = 'dict'
+    help_text = "A dictionary of data. Ex: {'price': 26.73, 'name': 'Daniel'}"
+    
+    def convert(self, value):
+        if value is None:
+            return None
+        
+        return dict(value)
+
+
 class DateField(ApiField):
     """
     A date field.
     """
     dehydrated_type = 'date'
     help_text = 'A date as a string. Ex: "2010-11-10"'
     
-    def dehydrate(self, obj):
-        return self.convert(super(DateField, self).dehydrate(obj))
-    
     def convert(self, value):
         if value is None:
             return None
         
         if isinstance(value, basestring):
             match = DATE_REGEX.search(value)
             
@@ -294,17 +321,14 @@
 class DateTimeField(ApiField):
     """
     A datetime field.
     """
     dehydrated_type = 'datetime'
     help_text = 'A date & time as a string. Ex: "2010-11-10T03:07:43"'
     
-    def dehydrate(self, obj):
-        return self.convert(super(DateTimeField, self).dehydrate(obj))
-    
     def convert(self, value):
         if value is None:
             return None
         
         if isinstance(value, basestring):
             match = DATETIME_REGEX.search(value)
             
@@ -329,16 +353,16 @@
         return value
 
 
 class RelatedField(ApiField):
     """
     Provides access to data that is related within the database.
     
-    A base class not intended for direct use but provides functionality that
-    ``ForeignKey`` and ``ManyToManyField`` build upon.
+    The ``RelatedField`` base class is not intended for direct use but provides
+    functionality that ``ToOneField`` and ``ToManyField`` build upon.
     
     The contents of this field actually point to another ``Resource``,
     rather than the related object. This allows the field to represent its data
     in different ways.
     
     The abstractions based around this are "leaky" in that, unlike the other
     fields provided by ``tastypie``, these fields don't handle arbitrary objects
@@ -346,15 +370,15 @@
     there is no ORM-specific code at this level.
     """
     dehydrated_type = 'related'
     is_related = True
     self_referential = False
     help_text = 'A related resource. Can be either a URI or set of nested resource data.'
     
-    def __init__(self, to, attribute, related_name=None, null=False, full=False, unique=False, help_text=None):
+    def __init__(self, to, attribute, related_name=None, default=NOT_PROVIDED, null=False, full=False, unique=False, help_text=None):
         """
         Builds the field and prepares it to access to related data.
         
         The ``to`` argument should point to a ``Resource`` class, NOT
         to a ``Model``. Required.
         
         The ``attribute`` argument should specify what field/callable points to
@@ -374,14 +398,15 @@
         ``dehydrate`` will be included in full.
         """
         self.instance_name = None
         self._resource = None
         self.to = to
         self.attribute = attribute
         self.related_name = related_name
+        self._default = default
         self.null = null
         self.full = full
         self.readonly = False
         self.api_name = None
         self.resource_name = None
         self.unique = unique
         self._to_class = None
@@ -398,28 +423,14 @@
         
         # Check if we're self-referential and hook it up.
         # We can't do this quite like Django because there's no ``AppCache``
         # here (which I think we should avoid as long as possible).
         if self.self_referential or self.to == 'self':
             self._to_class = cls
     
-    def has_default(self):
-        """
-        Always returns ``False``, as there is no ``default`` available on
-        related fields.
-        """
-        return False
-    
-    @property
-    def default(self):
-        """
-        Raises an exception because related fields do not have a ``default``.
-        """
-        raise ApiFieldError("%r fields do not have default data." % self)
-    
     def get_related_resource(self, related_instance):
         """
         Instaniates the related resource.
         """
         related_resource = self.to_class()
         
         # Fix the ``api_name`` if it's not present.
@@ -511,54 +522,55 @@
                         raise NotFound()
                     
                     return self.fk_resource.obj_update(self.fk_bundle, **lookup_kwargs)
                 except NotFound:
                     return self.fk_resource.full_hydrate(self.fk_bundle)
             except MultipleObjectsReturned:
                 return self.fk_resource.full_hydrate(self.fk_bundle)
+        elif hasattr(value, 'pk'):
+            return self.fk_resource.full_dehydrate(value)
         else:
             raise ApiFieldError("The '%s' field has was given data that was not a URI and not a dictionary-alike: %s." % (self.instance_name, value))
 
 
 class ToOneField(RelatedField):
     """
     Provides access to related data via foreign key.
     
     This subclass requires Django's ORM layer to work properly.
     """
     help_text = 'A single related resource. Can be either a URI or set of nested resource data.'
     
-    def __init__(self, to, attribute, related_name=None, null=False, full=False, unique=False, help_text=None):
-        super(ToOneField, self).__init__(to, attribute, related_name, null=null, full=full, unique=unique, help_text=help_text)
+    def __init__(self, to, attribute, related_name=None, default=NOT_PROVIDED, null=False, full=False, unique=False, help_text=None):
+        super(ToOneField, self).__init__(to, attribute, related_name=related_name, default=default, null=null, full=full, unique=unique, help_text=help_text)
         self.fk_resource = None
     
     def dehydrate(self, bundle):
         try:
             foreign_obj = getattr(bundle.obj, self.attribute)
         except ObjectDoesNotExist:
             foreign_obj = None
+        
         if not foreign_obj:
             if not self.null:
                 raise ApiFieldError("The model '%r' has an empty attribute '%s' and doesn't allow a null value." % (bundle.obj, self.attribute))
             
             return None
         
         self.fk_resource = self.get_related_resource(foreign_obj)
         fk_bundle = Bundle(obj=foreign_obj)
         return self.dehydrate_related(fk_bundle, self.fk_resource)
     
     def hydrate(self, bundle):
-        if bundle.data.get(self.instance_name) is None:
-            if self.null:
-                return None
-            else:
-                raise ApiFieldError("The '%s' field has no data and doesn't allow a null value." % self.instance_name)
+        value = super(ToOneField, self).hydrate(bundle)
         
-        return self.build_related_resource(bundle.data.get(self.instance_name))
-
+        if value is None:
+            return value
+        
+        return self.build_related_resource(value)
 
 class ForeignKey(ToOneField):
     """
     A convenience subclass for those who prefer to mirror ``django.db.models``.
     """
     pass
 
@@ -579,37 +591,42 @@
     Note that the ``hydrate`` portions of this field are quite different than
     any other field. ``hydrate_m2m`` actually handles the data and relations.
     This is due to the way Django implements M2M relationships.
     """
     is_m2m = True
     help_text = 'Many related resources. Can be either a list of URIs or list of individually nested resource data.'
     
-    def __init__(self, to, attribute, related_name=None, null=False, full=False, unique=False, help_text=help_text):
-        super(ToManyField, self).__init__(to, attribute, related_name, null=null, full=full, unique=unique, help_text=help_text)
+    def __init__(self, to, attribute, related_name=None, default=NOT_PROVIDED, null=False, full=False, unique=False, help_text=None):
+        super(ToManyField, self).__init__(to, attribute, related_name=related_name, default=default, null=null, full=full, unique=unique, help_text=help_text)
         self.m2m_bundles = []
     
     def dehydrate(self, bundle):
         if not bundle.obj or not bundle.obj.pk:
             if not self.null:
                 raise ApiFieldError("The model '%r' does not have a primary key and can not be used in a ToMany context." % bundle.obj)
             
             return []
         
-        if not getattr(bundle.obj, self.attribute):
+        if isinstance(self.attribute, basestring):
+            the_m2ms = getattr(bundle.obj, self.attribute)
+        elif callable(self.attribute):
+            the_m2ms = self.attribute(bundle)
+        
+        if not the_m2ms:
             if not self.null:
                 raise ApiFieldError("The model '%r' has an empty attribute '%s' and doesn't allow a null value." % (bundle.obj, self.attribute))
             
             return []
         
         self.m2m_resources = []
         m2m_dehydrated = []
         
         # TODO: Also model-specific and leaky. Relies on there being a
         #       ``Manager`` there.
-        for m2m in getattr(bundle.obj, self.attribute).all():
+        for m2m in the_m2ms.all():
             m2m_resource = self.get_related_resource(m2m)
             m2m_bundle = Bundle(obj=m2m)
             self.m2m_resources.append(m2m_resource)
             m2m_dehydrated.append(self.dehydrate_related(m2m_bundle, m2m_resource))
         
         return m2m_dehydrated
     
@@ -622,14 +639,17 @@
                 return []
             else:
                 raise ApiFieldError("The '%s' field has no data and doesn't allow a null value." % self.instance_name)
         
         m2m_hydrated = []
         
         for value in bundle.data.get(self.instance_name):
+            if value is None:
+                continue
+            
             m2m_hydrated.append(self.build_related_resource(value))
         
         return m2m_hydrated
 
 
 class ManyToManyField(ToManyField):
     """
```

### Comparing `django-tastypie-0.9.7/tastypie/http.py` & `django-tastypie-0.9.9/tastypie/http.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/models.py` & `django-tastypie-0.9.9/tastypie/models.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/paginator.py` & `django-tastypie-0.9.9/tastypie/paginator.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/resources.py` & `django-tastypie-0.9.9/tastypie/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,24 @@
 from tastypie.utils import is_valid_jsonp_callback_value, dict_strip_unicode_keys, trailing_slash
 from tastypie.utils.mime import determine_format, build_content_type
 from tastypie.validation import Validation
 try:
     set
 except NameError:
     from sets import Set as set
-# The ``copy`` module was added in Python 2.5 and ``copycompat`` was added in
-# post 1.1.1 Django (r11901)
+# The ``copy`` module became function-friendly in Python 2.5 and
+# ``copycompat`` was added in post 1.1.1 Django (r11901)..
 try:
     from django.utils.copycompat import deepcopy
-    from django.views.decorators.csrf import csrf_exempt
 except ImportError:
     from copy import deepcopy
+# If ``csrf_exempt`` isn't present, stub it.
+try:
+    from django.views.decorators.csrf import csrf_exempt
+except ImportError:
     def csrf_exempt(func):
         return func
 
 
 class ResourceOptions(object):
     """
     A configuration class for ``Resource``.
@@ -153,15 +156,15 @@
         
         if not api_name is None:
             self._meta.api_name = api_name
     
     def __getattr__(self, name):
         if name in self.fields:
             return self.fields[name]
-        raise AttributeError
+        raise AttributeError(name)
     
     def wrap_view(self, view):
         """
         Wraps methods so they can be called in a more functional way as well
         as handling exceptions better.
         
         Note that if ``BadRequest`` or an exception with a ``response`` attr
@@ -318,15 +321,57 @@
         Given a request, data and a format, deserializes the given data.
         
         It relies on the request properly sending a ``CONTENT_TYPE`` header,
         falling back to ``application/json`` if not provided.
         
         Mostly a hook, this uses the ``Serializer`` from ``Resource._meta``.
         """
-        return self._meta.serializer.deserialize(data, format=request.META.get('CONTENT_TYPE', 'application/json'))
+        deserialized = self._meta.serializer.deserialize(data, format=request.META.get('CONTENT_TYPE', 'application/json'))
+        return deserialized
+    
+    def alter_list_data_to_serialize(self, request, data):
+        """
+        A hook to alter list data just before it gets serialized & sent to the user.
+        
+        Useful for restructuring/renaming aspects of the what's going to be
+        sent.
+        
+        Should accommodate for a list of objects, generally also including
+        meta data.
+        """
+        return data
+    
+    def alter_detail_data_to_serialize(self, request, data):
+        """
+        A hook to alter detail data just before it gets serialized & sent to the user.
+        
+        Useful for restructuring/renaming aspects of the what's going to be
+        sent.
+        
+        Should accommodate for receiving a single bundle of data.
+        """
+        return data
+    
+    def alter_deserialized_list_data(self, request, data):
+        """
+        A hook to alter list data just after it has been received from the user &
+        gets deserialized.
+        
+        Useful for altering the user data before any hydration is applied.
+        """
+        return data
+    
+    def alter_deserialized_detail_data(self, request, data):
+        """
+        A hook to alter detail data just after it has been received from the user &
+        gets deserialized.
+        
+        Useful for altering the user data before any hydration is applied.
+        """
+        return data
     
     def dispatch_list(self, request, **kwargs):
         """
         A view for handling the various HTTP methods (GET/POST/PUT/DELETE) over
         the entire list of resources.
         
         Relies on ``Resource.dispatch`` for the heavy-lifting.
@@ -619,15 +664,16 @@
                 
                 if value is not None or field_object.null:
                     # We need to avoid populating M2M data here as that will
                     # cause things to blow up.
                     if not getattr(field_object, 'is_related', False):
                         setattr(bundle.obj, field_object.attribute, value)
                     elif not getattr(field_object, 'is_m2m', False):
-                        setattr(bundle.obj, field_object.attribute, value.obj)
+                        if value is not None:
+                            setattr(bundle.obj, field_object.attribute, value.obj)
             
             # Check for an optional method to do further hydration.
             method = getattr(self, "hydrate_%s" % field_name, None)
             
             if method:
                 bundle = method(bundle)
         
@@ -935,14 +981,15 @@
         sorted_objects = self.apply_sorting(objects, options=request.GET)
         
         paginator = self._meta.paginator_class(request.GET, sorted_objects, resource_uri=self.get_resource_list_uri(), limit=self._meta.limit)
         to_be_serialized = paginator.page()
         
         # Dehydrate the bundles in preparation for serialization.
         to_be_serialized['objects'] = [self.full_dehydrate(obj=obj) for obj in to_be_serialized['objects']]
+        to_be_serialized = self.alter_list_data_to_serialize(request, to_be_serialized)
         return self.create_response(request, to_be_serialized)
     
     def get_detail(self, request, **kwargs):
         """
         Returns a single serialized resource.
         
         Calls ``cached_obj_get/obj_get`` to provide the data, then handles that result
@@ -954,26 +1001,28 @@
             obj = self.cached_obj_get(request=request, **self.remove_api_resource_names(kwargs))
         except ObjectDoesNotExist:
             return HttpGone()
         except MultipleObjectsReturned:
             return HttpMultipleChoices("More than one resource is found at this URI.")
         
         bundle = self.full_dehydrate(obj)
+        bundle = self.alter_detail_data_to_serialize(request, bundle)
         return self.create_response(request, bundle)
     
     def put_list(self, request, **kwargs):
         """
         Replaces a collection of resources with another collection.
         
         Calls ``delete_list`` to clear out the collection then ``obj_create``
         with the provided the data to create the new collection.
         
         Return ``HttpAccepted`` (204 No Content).
         """
         deserialized = self.deserialize(request, request.raw_post_data, format=request.META.get('CONTENT_TYPE', 'application/json'))
+        deserialized = self.alter_deserialized_list_data(request, deserialized)
         
         if not 'objects' in deserialized:
             raise BadRequest("Invalid data sent.")
         
         self.obj_delete_list(request=request, **self.remove_api_resource_names(kwargs))
         bundles_seen = []
         
@@ -1001,34 +1050,36 @@
         Calls ``obj_update`` with the provided data first, but falls back to
         ``obj_create`` if the object does not already exist.
         
         If a new resource is created, return ``HttpCreated`` (201 Created).
         If an existing resource is modified, return ``HttpAccepted`` (204 No Content).
         """
         deserialized = self.deserialize(request, request.raw_post_data, format=request.META.get('CONTENT_TYPE', 'application/json'))
+        deserialized = self.alter_deserialized_detail_data(request, deserialized)
         bundle = self.build_bundle(data=dict_strip_unicode_keys(deserialized))
         self.is_valid(bundle, request)
         
         try:
             updated_bundle = self.obj_update(bundle, request=request, pk=kwargs.get('pk'))
             return HttpAccepted()
-        except:
+        except (NotFound, MultipleObjectsReturned):
             updated_bundle = self.obj_create(bundle, request=request, pk=kwargs.get('pk'))
             return HttpCreated(location=self.get_resource_uri(updated_bundle))
     
     def post_list(self, request, **kwargs):
         """
         Creates a new resource/object with the provided data.
         
         Calls ``obj_create`` with the provided data and returns a response
         with the new resource's location.
         
         If a new resource is created, return ``HttpCreated`` (201 Created).
         """
         deserialized = self.deserialize(request, request.raw_post_data, format=request.META.get('CONTENT_TYPE', 'application/json'))
+        deserialized = self.alter_deserialized_list_data(request, deserialized)
         bundle = self.build_bundle(data=dict_strip_unicode_keys(deserialized))
         self.is_valid(bundle, request)
         updated_bundle = self.obj_create(bundle, request=request)
         return HttpCreated(location=self.get_resource_uri(updated_bundle))
     
     def post_detail(self, request, **kwargs):
         """
@@ -1257,14 +1308,56 @@
                 kwargs['default'] = f.default
             
             final_fields[f.name] = api_field_class(**kwargs)
             final_fields[f.name].instance_name = f.name
         
         return final_fields
     
+    def check_filtering(self, field_name, filter_type='exact', filter_bits=None):
+        """
+        Given a field name, a optional filter type and an optional list of
+        additional relations, determine if a field can be filtered on.
+        
+        If a filter does not meet the needed conditions, it should raise an
+        ``InvalidFilterError``.
+        
+        If the filter meets the conditions, a list of attribute names (not
+        field names) will be returned.
+        """
+        if filter_bits is None:
+            filter_bits = []
+        
+        if not field_name in self._meta.filtering:
+            raise InvalidFilterError("The '%s' field does not allow filtering." % field_name)
+        
+        # Check to see if it's an allowed lookup type.
+        if not self._meta.filtering[field_name] in (ALL, ALL_WITH_RELATIONS):
+            # Must be an explicit whitelist.
+            if not filter_type in self._meta.filtering[field_name]:
+                raise InvalidFilterError("'%s' is not an allowed filter on the '%s' field." % (filter_type, field_name))
+        
+        if self.fields[field_name].attribute is None:
+            raise InvalidFilterError("The '%s' field has no 'attribute' for searching with." % field_name)
+        
+        # Check to see if it's a relational lookup and if that's allowed.
+        if len(filter_bits):
+            if not getattr(self.fields[field_name], 'is_related', False):
+                raise InvalidFilterError("The '%s' field does not support relations." % field_name)
+            
+            if not self._meta.filtering[field_name] == ALL_WITH_RELATIONS:
+                raise InvalidFilterError("Lookups are not allowed more than one level deep on the '%s' field." % field_name)
+            
+            # Recursively descend through the remaining lookups in the filter,
+            # if any. We should ensure that all along the way, we're allowed
+            # to filter on that field by the related resource.
+            related_resource = self.fields[field_name].get_related_resource(None)
+            return [self.fields[field_name].attribute] + related_resource.check_filtering(filter_bits[0], filter_type, filter_bits[1:])
+        
+        return [self.fields[field_name].attribute]
+    
     def build_filters(self, filters=None):
         """
         Given a dictionary of filters, create the necessary ORM-level filters.
         
         Keys should be resource fields, **NOT** model fields.
         
         Valid values are either a list of Django filter types (i.e.
@@ -1283,49 +1376,38 @@
         if filters is None:
             filters = {}
         
         qs_filters = {}
         
         for filter_expr, value in filters.items():
             filter_bits = filter_expr.split(LOOKUP_SEP)
+            field_name = filter_bits.pop(0)
+            filter_type = 'exact'
             
-            if not filter_bits[0] in self.fields:
+            if not field_name in self.fields:
                 # It's not a field we know about. Move along citizen.
                 continue
             
-            if not filter_bits[0] in self._meta.filtering:
-                raise InvalidFilterError("The '%s' field does not allow filtering." % filter_bits[0])
-            
-            if filter_bits[-1] in QUERY_TERMS.keys():
+            if len(filter_bits) and filter_bits[-1] in QUERY_TERMS.keys():
                 filter_type = filter_bits.pop()
-            else:
-                filter_type = 'exact'
-            
-            # Check to see if it's allowed lookup type.
-            if not self._meta.filtering[filter_bits[0]] in (ALL, ALL_WITH_RELATIONS):
-                # Must be an explicit whitelist.
-                if not filter_type in self._meta.filtering[filter_bits[0]]:
-                    raise InvalidFilterError("'%s' is not an allowed filter on the '%s' field." % (filter_expr, filter_bits[0]))
-            
-            # Check to see if it's a relational lookup and if that's allowed.
-            if len(filter_bits) > 1:
-                if not self._meta.filtering[filter_bits[0]] == ALL_WITH_RELATIONS:
-                    raise InvalidFilterError("Lookups are not allowed more than one level deep on the '%s' field." % filter_bits[0])
             
-            if self.fields[filter_bits[0]].attribute is None:
-                raise InvalidFilterError("The '%s' field has no 'attribute' for searching with." % filter_bits[0])
+            lookup_bits = self.check_filtering(field_name, filter_type, filter_bits)
             
             if value in ['true', 'True', True]:
                 value = True
             elif value in ['false', 'False', False]:
                 value = False
             elif value in ('nil', 'none', 'None', None):
                 value = None
             
-            db_field_name = LOOKUP_SEP.join([self.fields[filter_bits[0]].attribute] + filter_bits[1:])
+            # Split on ',' if not empty string and either an in or range filter.
+            if filter_type in ('in', 'range') and len(value):
+                value = value.split(',')
+            
+            db_field_name = LOOKUP_SEP.join(lookup_bits)
             qs_filter = "%s%s%s" % (db_field_name, LOOKUP_SEP, filter_type)
             qs_filters[qs_filter] = value
         
         return dict_strip_unicode_keys(qs_filters)
     
     def apply_sorting(self, obj_list, options=None):
         """
@@ -1384,23 +1466,17 @@
         
         return obj_list.order_by(*order_by_args)
     
     def get_object_list(self, request):
         """
         An ORM-specific implementation of ``get_object_list``.
         
-        Returns a queryset that may have been limited by authorization or other
-        overrides.
+        Returns a queryset that may have been limited by other overrides.
         """
-        base_object_list = self._meta.queryset
-        
-        # Limit it as needed.
-        authed_object_list = self.apply_authorization_limits(request, base_object_list)
-        
-        return authed_object_list
+        return self._meta.queryset._clone()
     
     def obj_get_list(self, request=None, **kwargs):
         """
         A ORM-specific implementation of ``obj_get_list``.
         
         Takes an optional ``request`` object, whose ``GET`` dictionary can be
         used to narrow the query.
@@ -1412,27 +1488,37 @@
             filters = request.GET.copy()
         
         # Update with the provided kwargs.
         filters.update(kwargs)
         applicable_filters = self.build_filters(filters=filters)
         
         try:
-            return self.get_object_list(request).filter(**applicable_filters)
+            base_object_list = self.get_object_list(request).filter(**applicable_filters)
+            return self.apply_authorization_limits(request, base_object_list)
         except ValueError, e:
-            raise NotFound("Invalid resource lookup data provided (mismatched type).")
+            raise BadRequest("Invalid resource lookup data provided (mismatched type).")
     
     def obj_get(self, request=None, **kwargs):
         """
         A ORM-specific implementation of ``obj_get``.
         
         Takes optional ``kwargs``, which are used to narrow the query to find
         the instance.
         """
         try:
-            return self.get_object_list(request).get(**kwargs)
+            base_object_list = self.get_object_list(request).filter(**kwargs)
+            object_list = self.apply_authorization_limits(request, base_object_list)
+            stringified_kwargs = ', '.join(["%s=%s" % (k, v) for k, v in kwargs.items()])
+            
+            if len(object_list) <= 0:
+                raise self._meta.object_class.DoesNotExist("Couldn't find an instance of '%s' which matched '%s'." % (self._meta.object_class.__name__, stringified_kwargs))
+            elif len(object_list) > 1:
+                raise MultipleObjectsReturned("More than '%s' matched '%s'." % (self._meta.object_class.__name__, stringified_kwargs))
+            
+            return object_list[0]
         except ValueError, e:
             raise NotFound("Invalid resource lookup data provided (mismatched type).")
     
     def obj_create(self, bundle, request=None, **kwargs):
         """
         A ORM-specific implementation of ``obj_create``.
         """
@@ -1467,15 +1553,15 @@
                     if getattr(bundle.obj, k) is not None))
             except:
                 # if there is trouble hydrating the data, fall back to just
                 # using kwargs by itself (usually it only contains a "pk" key
                 # and this will work fine.
                 lookup_kwargs = kwargs
             try:
-                bundle.obj = self.get_object_list(request).get(**lookup_kwargs)
+                bundle.obj = self.obj_get(request, **lookup_kwargs)
             except ObjectDoesNotExist:
                 raise NotFound("A model instance matching the provided arguments could not be found.")
         
         bundle = self.full_hydrate(bundle)
         bundle.obj.save()
         
         # Now pick up the M2M bits.
@@ -1485,25 +1571,33 @@
     
     def obj_delete_list(self, request=None, **kwargs):
         """
         A ORM-specific implementation of ``obj_delete_list``.
         
         Takes optional ``kwargs``, which can be used to narrow the query.
         """
-        self.get_object_list(request).filter(**kwargs).delete()
+        base_object_list = self.get_object_list(request).filter(**kwargs)
+        authed_object_list = self.apply_authorization_limits(request, base_object_list)
+        
+        if hasattr(authed_object_list, 'delete'):
+            # It's likely a ``QuerySet``. Call ``.delete()`` for efficiency.
+            authed_object_list.delete()
+        else:
+            for authed_obj in authed_object_list:
+                authed_object_list.delete()
     
     def obj_delete(self, request=None, **kwargs):
         """
         A ORM-specific implementation of ``obj_delete``.
         
         Takes optional ``kwargs``, which are used to narrow the query to find
         the instance.
         """
         try:
-            obj = self.get_object_list(request).get(**kwargs)
+            obj = self.obj_get(request, **kwargs)
         except ObjectDoesNotExist:
             raise NotFound("A model instance matching the provided arguments could not be found.")
         
         obj.delete()
     
     def rollback(self, bundles):
         """
```

### Comparing `django-tastypie-0.9.7/tastypie/serializers.py` & `django-tastypie-0.9.9/tastypie/serializers.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/templates/tastypie/basic.html` & `django-tastypie-0.9.9/tastypie/templates/tastypie/basic.html`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/utils/formatting.py` & `django-tastypie-0.9.9/tastypie/utils/formatting.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import email
 import datetime
 from django.utils import dateformat
 
 # Try to use dateutil for maximum date-parsing niceness. Fall back to
 # hard-coded RFC2822 parsing if that's not possible.
 try:
     from dateutil.parser import parse as mk_datetime
```

### Comparing `django-tastypie-0.9.7/tastypie/utils/mime.py` & `django-tastypie-0.9.9/tastypie/utils/mime.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/utils/validate_jsonp.py` & `django-tastypie-0.9.9/tastypie/utils/validate_jsonp.py`

 * *Files identical despite different names*

### Comparing `django-tastypie-0.9.7/tastypie/validation.py` & `django-tastypie-0.9.9/tastypie/validation.py`

 * *Files identical despite different names*

