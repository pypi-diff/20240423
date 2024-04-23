# Comparing `tmp/django-authgw-2.0.tar.gz` & `tmp/django-authgw-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-authgw-2.0.tar", last modified: Mon Apr 22 20:58:17 2024, max compression
+gzip compressed data, was "dist/django-authgw-2.1.tar", last modified: Tue Apr 23 21:39:34 2024, max compression
```

## Comparing `django-authgw-2.0.tar` & `django-authgw-2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-22 20:58:17.416638 django-authgw-2.0/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2020-07-05 21:56:33.000000 django-authgw-2.0/LICENSE
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       87 2024-04-22 20:45:14.000000 django-authgw-2.0/MANIFEST.in
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     6278 2024-04-22 20:58:17.416638 django-authgw-2.0/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4852 2022-07-19 14:47:08.000000 django-authgw-2.0/README.md
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-22 20:58:17.416638 django-authgw-2.0/authgw/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2022-07-18 21:00:46.000000 django-authgw-2.0/authgw/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       63 2022-07-18 21:00:46.000000 django-authgw-2.0/authgw/admin.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1096 2022-07-18 21:14:45.000000 django-authgw-2.0/authgw/apps.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-22 20:58:17.416638 django-authgw-2.0/authgw/migrations/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2022-07-18 21:00:46.000000 django-authgw-2.0/authgw/migrations/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       57 2022-07-18 21:00:46.000000 django-authgw-2.0/authgw/models.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-22 20:58:17.412638 django-authgw-2.0/authgw/templates/
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-22 20:58:17.416638 django-authgw-2.0/authgw/templates/authgw/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     3157 2022-07-06 20:46:55.000000 django-authgw-2.0/authgw/templates/authgw/login.html
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       60 2022-07-18 21:00:46.000000 django-authgw-2.0/authgw/tests.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      268 2022-07-18 21:16:34.000000 django-authgw-2.0/authgw/urls.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-22 20:58:17.416638 django-authgw-2.0/authgw/utils/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2022-06-01 16:33:04.000000 django-authgw-2.0/authgw/utils/__init__.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4912 2022-07-18 22:25:02.000000 django-authgw-2.0/authgw/utils/authenticators.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7641 2024-04-22 20:45:14.000000 django-authgw-2.0/authgw/utils/django.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    13138 2024-04-22 20:45:14.000000 django-authgw-2.0/authgw/utils/ldap3.py
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4980 2022-07-18 22:46:22.000000 django-authgw-2.0/authgw/views.py
-drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-22 20:58:17.416638 django-authgw-2.0/django_authgw.egg-info/
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     6278 2024-04-22 20:58:17.000000 django-authgw-2.0/django_authgw.egg-info/PKG-INFO
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      538 2024-04-22 20:58:17.000000 django-authgw-2.0/django_authgw.egg-info/SOURCES.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-04-22 20:58:17.000000 django-authgw-2.0/django_authgw.egg-info/dependency_links.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-04-22 20:57:30.000000 django-authgw-2.0/django_authgw.egg-info/not-zip-safe
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       13 2024-04-22 20:58:17.000000 django-authgw-2.0/django_authgw.egg-info/requires.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        7 2024-04-22 20:58:17.000000 django-authgw-2.0/django_authgw.egg-info/top_level.txt
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2024-04-22 20:58:17.416638 django-authgw-2.0/setup.cfg
--rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1182 2024-04-22 20:45:14.000000 django-authgw-2.0/setup.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-23 21:39:34.732416 django-authgw-2.1/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1069 2020-07-05 21:56:33.000000 django-authgw-2.1/LICENSE
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       87 2024-04-22 20:45:14.000000 django-authgw-2.1/MANIFEST.in
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     6278 2024-04-23 21:39:34.732416 django-authgw-2.1/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4852 2022-07-19 14:47:08.000000 django-authgw-2.1/README.md
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-23 21:39:34.732416 django-authgw-2.1/authgw/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2022-07-18 21:00:46.000000 django-authgw-2.1/authgw/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       63 2022-07-18 21:00:46.000000 django-authgw-2.1/authgw/admin.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1096 2022-07-18 21:14:45.000000 django-authgw-2.1/authgw/apps.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-23 21:39:34.732416 django-authgw-2.1/authgw/migrations/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2022-07-18 21:00:46.000000 django-authgw-2.1/authgw/migrations/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       57 2022-07-18 21:00:46.000000 django-authgw-2.1/authgw/models.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-23 21:39:34.728416 django-authgw-2.1/authgw/templates/
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-23 21:39:34.732416 django-authgw-2.1/authgw/templates/authgw/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     3157 2022-07-06 20:46:55.000000 django-authgw-2.1/authgw/templates/authgw/login.html
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       60 2022-07-18 21:00:46.000000 django-authgw-2.1/authgw/tests.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      268 2022-07-18 21:16:34.000000 django-authgw-2.1/authgw/urls.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-23 21:39:34.732416 django-authgw-2.1/authgw/utils/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        0 2022-06-01 16:33:04.000000 django-authgw-2.1/authgw/utils/__init__.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4912 2022-07-18 22:25:02.000000 django-authgw-2.1/authgw/utils/authenticators.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     7641 2024-04-22 20:45:14.000000 django-authgw-2.1/authgw/utils/django.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)    13780 2024-04-23 21:38:15.000000 django-authgw-2.1/authgw/utils/ldap3.py
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     4980 2022-07-18 22:46:22.000000 django-authgw-2.1/authgw/views.py
+drwxrwxr-x   0 sstacha   (1001) sstacha   (1001)        0 2024-04-23 21:39:34.732416 django-authgw-2.1/django_authgw.egg-info/
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     6278 2024-04-23 21:39:34.000000 django-authgw-2.1/django_authgw.egg-info/PKG-INFO
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)      538 2024-04-23 21:39:34.000000 django-authgw-2.1/django_authgw.egg-info/SOURCES.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-04-23 21:39:34.000000 django-authgw-2.1/django_authgw.egg-info/dependency_links.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        1 2024-04-23 21:39:20.000000 django-authgw-2.1/django_authgw.egg-info/not-zip-safe
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       13 2024-04-23 21:39:34.000000 django-authgw-2.1/django_authgw.egg-info/requires.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)        7 2024-04-23 21:39:34.000000 django-authgw-2.1/django_authgw.egg-info/top_level.txt
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)       38 2024-04-23 21:39:34.732416 django-authgw-2.1/setup.cfg
+-rw-rw-r--   0 sstacha   (1001) sstacha   (1001)     1182 2024-04-23 21:37:54.000000 django-authgw-2.1/setup.py
```

### Comparing `django-authgw-2.0/LICENSE` & `django-authgw-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/PKG-INFO` & `django-authgw-2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authgw
-Version: 2.0
+Version: 2.1
 Summary: Authentication gateway application for the Django framework
 Home-page: http://github.com/sstacha/django-authgw
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # django-authgw
         django-authgw is a django application for developers who build, manage and maintain websites.  This app is intended to support various methods of authenticating and authorizing into a Django based site or application based on URL patterns.
```

### Comparing `django-authgw-2.0/README.md` & `django-authgw-2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/authgw/apps.py` & `django-authgw-2.1/authgw/apps.py`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/authgw/templates/authgw/login.html` & `django-authgw-2.1/authgw/templates/authgw/login.html`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/authgw/utils/authenticators.py` & `django-authgw-2.1/authgw/utils/authenticators.py`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/authgw/utils/django.py` & `django-authgw-2.1/authgw/utils/django.py`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/authgw/utils/ldap3.py` & `django-authgw-2.1/authgw/utils/ldap3.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,21 +59,20 @@
             - add guaranteed property for is_authenticated
             - add guaranteed private property _groups defaulted to empty list
             - add helper method to convert ldap group dn's to list of group names (more pythonic)
                 Ex: ["CN=MY_GROUP,OU=DALLAS,OU=OFFICES,OU=EXAMPLE,OU=ORG"] -> ["MY_GROUP"]
             - add helper method for returning if a group exists in the _groups list (True/False)
             - add helper method for returning if dn contains an organizational unit (OU=<stuff>) (True/False)
     """
-    # authenticated is marked after binding successfully with provided password
-    is_authenticated = False
-
     def __init__(self, user_field_dn: str = 'distinguishedName', user_field_groups_dn: str = 'memberOf'):
         # we need to know the dn field and groups field for this implementation (defaults to inetorg and inetorgperson)
         self._field_dn = user_field_dn
         self._field_groups_dn = user_field_groups_dn
+        # authenticated is marked after binding successfully with provided password
+        self.is_authenticated = False
 
     def get_groups(self) -> [str]:
         """
         parses a list of group_dn's and extracts them to a list of group names for the self._groups property
         :param group_dn_list: list of group_dn's
         :return: None
         """
@@ -168,14 +167,25 @@
         #   such we MUST bind using a bind_user_dn and bind_user_password.  We will then need to re-bind as
         #   the user once we get the users dn from searching.
         if not self.config.use_ntlm and not self.config.bind_user:
             raise LDAPConfigurationParameterError(f'LDAP_BIND_DN {missing_error}')
         if not self.config.use_ntlm and not self.config.bind_password:
             raise LDAPConfigurationParameterError(f'LDAP_BIND_PASSWORD {missing_error}')
 
+    def find_user(self, login: str) -> LdapUser:
+        # validate config
+        self.validate_config()
+        # validate credentials
+        if not login:
+            raise LDAPConfigurationParameterError('you must provide a login to authenticate')
+        # get a connection to the ldap server
+        server = Server(self.config.host, port=self.config.port, use_ssl=self.config.use_ssl, get_info=ALL)
+        # we will either search the Directory for this user/password using LDAP or overridden NTLM protocol
+        return self.search(server, login, "")
+
     def authenticate(self, login: str, password: str) -> LdapUser:
         # validate config
         self.validate_config()
         # validate credentials
         if not login:
             raise LDAPConfigurationParameterError('you must provide a login to authenticate')
         if not password:
@@ -195,19 +205,20 @@
                              attributes=self.config.user_attributes)
             # print(bind_conn)
             # print(bind_conn.entries)
             if bind_conn.entries:
                 user_dn = bind_conn.entries[0]
             if user_dn:
                 ldap_user.load(user_dn)
-            # one additional step that is not needed for AD; re-bind as user now that we have dn to set is_authenticated
-            #   since we originally bound as a bind user we haven't verified the password yet
-            with Connection(server, ldap_user.get_dn(), password) as conn:
-                if conn.bound:
-                    ldap_user.is_authenticated = True
+            if password and ldap_user.get_dn():
+                # one additional step that is not needed for AD; re-bind as user now that we have dn to set is_authenticated
+                #   since we originally bound as a bind user we haven't verified the password yet
+                with Connection(server, ldap_user.get_dn(), password) as conn:
+                    if conn.bound:
+                        ldap_user.is_authenticated = True
         return ldap_user
 
 
 # moving the operations for AD to a class
 class ActiveDirectoryAuthenticator(LdapAuthenticator):
     """
     ActiveDirectoryAuthenticator will use NTLM (users login) to connect and search instead of normal LDAP DN
```

### Comparing `django-authgw-2.0/authgw/views.py` & `django-authgw-2.1/authgw/views.py`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/django_authgw.egg-info/PKG-INFO` & `django-authgw-2.1/django_authgw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-authgw
-Version: 2.0
+Version: 2.1
 Summary: Authentication gateway application for the Django framework
 Home-page: http://github.com/sstacha/django-authgw
 Author: Steve Stacha
 Author-email: sstacha@gmail.com
 License: MIT
 Description: # django-authgw
         django-authgw is a django application for developers who build, manage and maintain websites.  This app is intended to support various methods of authenticating and authorizing into a Django based site or application based on URL patterns.
```

### Comparing `django-authgw-2.0/django_authgw.egg-info/SOURCES.txt` & `django-authgw-2.1/django_authgw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-authgw-2.0/setup.py` & `django-authgw-2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='django-authgw',
-      version='2.0',
+      version='2.1',
       description='Authentication gateway application for the Django framework',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='http://github.com/sstacha/django-authgw',
       author='Steve Stacha',
       author_email='sstacha@gmail.com',
       license='MIT',
```

