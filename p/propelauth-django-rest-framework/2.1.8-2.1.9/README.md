# Comparing `tmp/propelauth-django-rest-framework-2.1.8.tar.gz` & `tmp/propelauth-django-rest-framework-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "propelauth-django-rest-framework-2.1.8.tar", last modified: Sun Oct 15 04:26:25 2023, max compression
+gzip compressed data, was "propelauth-django-rest-framework-2.1.9.tar", last modified: Thu Oct 26 00:48:52 2023, max compression
```

## Comparing `propelauth-django-rest-framework-2.1.8.tar` & `propelauth-django-rest-framework-2.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:26:25.991885 propelauth-django-rest-framework-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-15 04:26:10.000000 propelauth-django-rest-framework-2.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-15 04:26:25.991885 propelauth-django-rest-framework-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-10-15 04:26:10.000000 propelauth-django-rest-framework-2.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:26:25.987885 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework/
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-10-15 04:26:10.000000 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2023-10-15 04:26:10.000000 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework/auth_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-15 04:26:25.987885 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-15 04:26:25.000000 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-10-15 04:26:25.000000 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-15 04:26:25.000000 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2023-10-15 04:26:25.000000 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-15 04:26:25.000000 propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-15 04:26:25.991885 propelauth-django-rest-framework-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-10-15 04:26:10.000000 propelauth-django-rest-framework-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 00:48:52.121590 propelauth-django-rest-framework-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-26 00:48:35.000000 propelauth-django-rest-framework-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-26 00:48:52.121590 propelauth-django-rest-framework-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-10-26 00:48:35.000000 propelauth-django-rest-framework-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 00:48:52.121590 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2023-10-26 00:48:35.000000 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2023-10-26 00:48:35.000000 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework/auth_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 00:48:52.121590 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-26 00:48:52.000000 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2023-10-26 00:48:52.000000 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 00:48:52.000000 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-26 00:48:52.000000 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-26 00:48:52.000000 propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 00:48:52.121590 propelauth-django-rest-framework-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-10-26 00:48:35.000000 propelauth-django-rest-framework-2.1.9/setup.py
```

### Comparing `propelauth-django-rest-framework-2.1.8/LICENSE` & `propelauth-django-rest-framework-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.8/PKG-INFO` & `propelauth-django-rest-framework-2.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.1.8
+Version: 2.1.9
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.8
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.9
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       _[_h_t_t_p_s_:_/_/_p_r_o_p_e_l_a_u_t_h_-_l_o_g_o_s_._s_3_._u_s_-_w_e_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_l_o_g_o_-_o_n_l_y_._p_n_g_]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.1.8/README.md` & `propelauth-django-rest-framework-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework/__init__.py` & `propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework/auth_helpers.py` & `propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `propelauth-django-rest-framework-2.1.8/propelauth_django_rest_framework.egg-info/PKG-INFO` & `propelauth-django-rest-framework-2.1.9/propelauth_django_rest_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propelauth-django-rest-framework
-Version: 2.1.8
+Version: 2.1.9
 Summary: A library for managing authentication in Django Rest Framework
 Home-page: https://github.com/propelauth/propelauth-django-rest-framework
 Author: PropelAuth
 Author-email: support@propelauth.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.8
+Metadata-Version: 2.1 Name: propelauth-django-rest-framework Version: 2.1.9
 Summary: A library for managing authentication in Django Rest Framework Home-
 page: https://github.com/propelauth/propelauth-django-rest-framework Author:
 PropelAuth Author-email: support@propelauth.com License: MIT Platform: UNKNOWN
 Description-Content-Type: text/markdown License-File: LICENSE # PropelAuth
 Django Rest Framework Library
       _[_h_t_t_p_s_:_/_/_p_r_o_p_e_l_a_u_t_h_-_l_o_g_o_s_._s_3_._u_s_-_w_e_s_t_-_2_._a_m_a_z_o_n_a_w_s_._c_o_m_/_l_o_g_o_-_o_n_l_y_._p_n_g_]
 A Django Rest Framework library for managing authentication, backed by
```

### Comparing `propelauth-django-rest-framework-2.1.8/setup.py` & `propelauth-django-rest-framework-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 
 # See https://pytest-runner.readthedocs.io/en/latest/#conditional-requirement
 needs_pytest = {"pytest", "test", "ptr"}.intersection(sys.argv)
 pytest_runner = ["pytest-runner"] if needs_pytest else []
 
 setup(
     name="propelauth-django-rest-framework",
-    version="2.1.8",
+    version="2.1.9",
     description="A library for managing authentication in Django Rest Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/propelauth/propelauth-django-rest-framework",
     packages=find_packages(include=["propelauth_django_rest_framework"]),
     author="PropelAuth",
     author_email="support@propelauth.com",
     license="MIT",
     install_requires=[
         "django",
         "djangorestframework",
-        "propelauth-py==3.1.9",
+        "propelauth-py==3.1.10",
         "requests",
     ],
     setup_requires=pytest_runner,
     tests_require=["pytest==4.4.1"],
     test_suite="tests",
 )
```

