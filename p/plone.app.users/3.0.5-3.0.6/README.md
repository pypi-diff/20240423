# Comparing `tmp/plone.app.users-3.0.5.tar.gz` & `tmp/plone_app_users-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.users-3.0.5.tar", last modified: Tue Mar 19 21:36:12 2024, max compression
+gzip compressed data, was "plone_app_users-3.0.6.tar", last modified: Tue Apr 23 15:37:21 2024, max compression
```

## Comparing `plone.app.users-3.0.5.tar` & `plone_app_users-3.0.6.tar`

### file list

```diff
@@ -1,87 +1,89 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.215963 plone.app.users-3.0.5/
--rw-r--r--   0 maurits    (501) staff       (20)    21094 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    25974 2024-03-19 21:36:12.215265 plone.app.users-3.0.5/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2560 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.179835 plone.app.users-3.0.5/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      677 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.180288 plone.app.users-3.0.5/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.184571 plone.app.users-3.0.5/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.189162 plone.app.users-3.0.5/plone/app/users/
--rw-r--r--   0 maurits    (501) staff       (20)      637 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/TODO.txt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.199076 plone.app.users-3.0.5/plone/app/users/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2053 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/account-configlet.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1367 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/account-panel.pt
--rw-r--r--   0 maurits    (501) staff       (20)    13362 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/account.py
--rw-r--r--   0 maurits    (501) staff       (20)     3463 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2534 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1732 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/memberregistration.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3587 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/membersearch.py
--rw-r--r--   0 maurits    (501) staff       (20)     4405 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/membersearch_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/newuser_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5006 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/passwordpanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3390 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/personalpreferences.py
--rw-r--r--   0 maurits    (501) staff       (20)    29389 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/register.py
--rw-r--r--   0 maurits    (501) staff       (20)     1973 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/register_form.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5235 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/registered.pt
--rw-r--r--   0 maurits    (501) staff       (20)      573 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/registered.py
--rw-r--r--   0 maurits    (501) staff       (20)     2807 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/registersettingspanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     1892 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/schema_layout.pt
--rw-r--r--   0 maurits    (501) staff       (20)     9906 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/schemaeditor.py
--rw-r--r--   0 maurits    (501) staff       (20)     3820 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/browser/userdatapanel.py
--rw-r--r--   0 maurits    (501) staff       (20)     3050 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2282 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/field_extender.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.175722 plone.app.users-3.0.5/plone/app/users/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.199992 plone.app.users-3.0.5/plone/app/users/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)       85 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)     2085 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/profiles/default/userschema.xml
--rw-r--r--   0 maurits    (501) staff       (20)     5684 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/schema.py
--rw-r--r--   0 maurits    (501) staff       (20)      652 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/setuphandlers.py
--rw-r--r--   0 maurits    (501) staff       (20)     1415 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.212510 plone.app.users-3.0.5/plone/app/users/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5023 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     1997 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/duplicate_email.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4463 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/email_login.rst
--rw-r--r--   0 maurits    (501) staff       (20)     7625 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/flexible_user_registration.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2712 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/forms_navigationroot.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3275 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/member_search.rst
--rw-r--r--   0 maurits    (501) staff       (20)      306 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/onepixel.jpg
--rw-r--r--   0 maurits    (501) staff       (20)     5282 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/password.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4060 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/personal_preferences.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3645 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/personal_preferences_prefs_user_details.rst
--rw-r--r--   0 maurits    (501) staff       (20)     4246 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/plugins.rst
--rw-r--r--   0 maurits    (501) staff       (20)    15438 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/registration_forms.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1618 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_account.py
--rw-r--r--   0 maurits    (501) staff       (20)     1136 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)     8201 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_exportimport.py
--rw-r--r--   0 maurits    (501) staff       (20)     2372 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_loginname_generator.py
--rw-r--r--   0 maurits    (501) staff       (20)      530 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_member_search.py
--rw-r--r--   0 maurits    (501) staff       (20)     8501 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_new_user.py
--rw-r--r--   0 maurits    (501) staff       (20)     1642 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_pam.py
--rw-r--r--   0 maurits    (501) staff       (20)    12465 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_schema_types.py
--rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_user_data_panel.py
--rw-r--r--   0 maurits    (501) staff       (20)     5015 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/test_userid_generator.py
--rw-r--r--   0 maurits    (501) staff       (20)     6049 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/userdata.rst
--rw-r--r--   0 maurits    (501) staff       (20)     2730 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/tests/userdata_prefs_user_details.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3672 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/upgrades.py
--rw-r--r--   0 maurits    (501) staff       (20)      648 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     4459 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone/app/users/vocabularies.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-19 21:36:12.213096 plone.app.users-3.0.5/plone.app.users.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    25974 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone.app.users.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2729 2024-03-19 21:36:12.000000 plone.app.users-3.0.5/plone.app.users.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone.app.users.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone.app.users.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone.app.users.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone.app.users.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      629 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone.app.users.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/plone.app.users.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4414 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-03-19 21:36:12.216091 plone.app.users-3.0.5/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2719 2024-03-19 21:36:11.000000 plone.app.users-3.0.5/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.201921 plone_app_users-3.0.6/
+-rw-r--r--   0 maurits    (501) staff       (20)    21385 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    26287 2024-04-23 15:37:21.201504 plone_app_users-3.0.6/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2560 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.176431 plone_app_users-3.0.6/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      677 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.176698 plone_app_users-3.0.6/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.179551 plone_app_users-3.0.6/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.182812 plone_app_users-3.0.6/plone/app/users/
+-rw-r--r--   0 maurits    (501) staff       (20)      637 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/TODO.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.189745 plone_app_users-3.0.6/plone/app/users/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2053 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/account-configlet.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1367 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/account-panel.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    14468 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/account.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3463 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2534 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1732 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/memberregistration.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3587 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/membersearch.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4405 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/membersearch_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/newuser_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5006 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/passwordpanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3390 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/personalpreferences.py
+-rw-r--r--   0 maurits    (501) staff       (20)    29389 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/register.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1973 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/register_form.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5235 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/registered.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      573 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/registered.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2807 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/registersettingspanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1892 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/schema_layout.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     9906 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/schemaeditor.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3820 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/browser/userdatapanel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3050 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2282 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/field_extender.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.173262 plone_app_users-3.0.6/plone/app/users/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.190293 plone_app_users-3.0.6/plone/app/users/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     2085 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/profiles/default/userschema.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     5684 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)      652 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1415 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.199953 plone_app_users-3.0.6/plone/app/users/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5071 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1997 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/duplicate_email.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4463 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/email_login.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     7625 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/flexible_user_registration.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2712 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/forms_navigationroot.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3275 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/member_search.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      306 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/onepixel.jpg
+-rw-r--r--   0 maurits    (501) staff       (20)     5282 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/password.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4060 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/personal_preferences.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3645 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/personal_preferences_prefs_user_details.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     4246 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/plugins.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    15438 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/registration_forms.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1618 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_account.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1136 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8201 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_exportimport.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2372 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_loginname_generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)      530 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_member_search.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8501 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_new_user.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1642 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_pam.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2137 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_portrait.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12465 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_schema_types.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1031 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_user_data_panel.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5015 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/test_userid_generator.py
+-rw-r--r--   0 maurits    (501) staff       (20)      124 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/transparent_square.svg
+-rw-r--r--   0 maurits    (501) staff       (20)     6049 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/userdata.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     2730 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/tests/userdata_prefs_user_details.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3672 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/upgrades.py
+-rw-r--r--   0 maurits    (501) staff       (20)      648 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4459 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/plone/app/users/vocabularies.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:37:21.200314 plone_app_users-3.0.6/plone.app.users.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    26287 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2813 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      636 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 15:37:21.000000 plone_app_users-3.0.6/plone.app.users.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4431 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-23 15:37:21.201999 plone_app_users-3.0.6/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2737 2024-04-23 15:37:20.000000 plone_app_users-3.0.6/setup.py
```

### Comparing `plone.app.users-3.0.5/CHANGES.rst` & `plone_app_users-3.0.6/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Fix #122 validating if image is supported by PIL showing a validation error if not.
+  Include Pillow dependency in setup.py.
+  Fix ValueError: User could not be found in BaseTest setUp adding a transaction.commit().
+  [rber474] (#122)
+
+
 3.0.5 (2024-03-19)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.users-3.0.5/PKG-INFO` & `plone_app_users-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.users
-Version: 3.0.5
+Version: 3.0.6
 Summary: A package for all things users and groups related (specific to plone)
 Home-page: https://pypi.org/project/plone.app.users
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Zope CMF Plone Users Groups
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: Acquisition
+Requires-Dist: Pillow
 Requires-Dist: Products.GenericSetup
 Requires-Dist: Products.PlonePAS>=5.0.1
 Requires-Dist: Products.statusmessages
 Requires-Dist: Zope
 Requires-Dist: plone.app.layout
 Requires-Dist: plone.autoform>=1.2
 Requires-Dist: plone.app.event
@@ -129,14 +130,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Fix #122 validating if image is supported by PIL showing a validation error if not.
+  Include Pillow dependency in setup.py.
+  Fix ValueError: User could not be found in BaseTest setUp adding a transaction.commit().
+  [rber474] (#122)
+
+
 3.0.5 (2024-03-19)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.users-3.0.5/README.rst` & `plone_app_users-3.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/docs/LICENSE.GPL` & `plone_app_users-3.0.6/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/docs/LICENSE.txt` & `plone_app_users-3.0.6/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/TODO.txt` & `plone_app_users-3.0.6/plone/app/users/TODO.txt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/account-configlet.pt` & `plone_app_users-3.0.6/plone/app/users/browser/account-configlet.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/account-panel.pt` & `plone_app_users-3.0.6/plone/app/users/browser/account-panel.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/account.py` & `plone_app_users-3.0.6/plone/app/users/browser/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from AccessControl import Unauthorized
 from Acquisition import aq_inner
+from PIL import Image
+from PIL import UnidentifiedImageError
 from plone.app.layout.navigation.interfaces import INavigationRoot
 from plone.app.users.browser.interfaces import IAccountPanelForm
 from plone.app.users.browser.schemaeditor import getFromBaseSchema
 from plone.app.users.utils import notifyWidgetActionExecutionError
 from plone.autoform.form import AutoExtensibleForm
 from plone.base import PloneMessageFactory as _
 from plone.base.interfaces import IPloneSiteRoot
@@ -40,14 +42,19 @@
     default=(
         "The email address you selected is "
         "already in use or is not valid as login "
         "name. Please choose another."
     ),
 )
 
+MESSAGE_IMAGE_NOT_SUPPORTED = _(
+    "message_image_not_supported",
+    "The file you selected is not supported by Pillow. " "Please choose another.",
+)
+
 
 def getSchema(schema_interface, schema_adapter, form_name=None):
     request = getRequest()
     form_name_to_request_attr_name = {
         "In User Profile": "_userdata_schema",
         "On Registration": "_register_schema",
         None: "_userdata_manager_schema",
@@ -255,24 +262,46 @@
                     if not id_allowed:
                         # only allow if unchanged
                         if self._differentEmail(data["email"]):
                             err_str = MESSAGE_EMAIL_IN_USE
                 if err_str:
                     notifyWidgetActionExecutionError(action, "email", err_str)
 
+    def validate_portrait(self, action, data):
+        """Portrait validation.
+        Checks if image is supported by Pillow.
+        SVG files are not yet supported.
+        """
+        error_keys = [error.field.getName() for error in action.form.widgets.errors]
+        if "portrait" not in error_keys and data["portrait"] is not None:
+            portrait = data["portrait"].open()
+            try:
+                Image.open(portrait)
+            except UnidentifiedImageError:
+                notifyWidgetActionExecutionError(
+                    action, "portrait", MESSAGE_IMAGE_NOT_SUPPORTED
+                )
+            except Exception as exc:
+                raise exc
+
     @button.buttonAndHandler(_("Save"))
     def handleSave(self, action):
         CheckAuthenticator(self.request)
         data, errors = self.extractData()
 
         # Extra validation for email, when it is there.  email is not in the
         # data when you are at the personal-preferences page.
         if "email" in data:
             self.validate_email(action, data)
 
+        # Validate portrait, upload image could be not supported
+        # by PIL what raises an exception when scaling image.
+        if "portrait" in data:
+            self.validate_portrait(action, data)
+
         if action.form.widgets.errors:
             self.status = self.formErrorsMessage
             return
         if self.applyChanges(data):
             IStatusMessage(self.request).addStatusMessage(
                 self.successMessage, type="info"
             )
```

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/configure.zcml` & `plone_app_users-3.0.6/plone/app/users/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/interfaces.py` & `plone_app_users-3.0.6/plone/app/users/browser/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/memberregistration.pt` & `plone_app_users-3.0.6/plone/app/users/browser/memberregistration.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/membersearch.py` & `plone_app_users-3.0.6/plone/app/users/browser/membersearch.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/membersearch_form.pt` & `plone_app_users-3.0.6/plone/app/users/browser/membersearch_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/newuser_form.pt` & `plone_app_users-3.0.6/plone/app/users/browser/newuser_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/passwordpanel.py` & `plone_app_users-3.0.6/plone/app/users/browser/passwordpanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/personalpreferences.py` & `plone_app_users-3.0.6/plone/app/users/browser/personalpreferences.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/register.py` & `plone_app_users-3.0.6/plone/app/users/browser/register.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/register_form.pt` & `plone_app_users-3.0.6/plone/app/users/browser/register_form.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/registered.pt` & `plone_app_users-3.0.6/plone/app/users/browser/registered.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/registered.py` & `plone_app_users-3.0.6/plone/app/users/browser/registered.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/registersettingspanel.py` & `plone_app_users-3.0.6/plone/app/users/browser/registersettingspanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/schema_layout.pt` & `plone_app_users-3.0.6/plone/app/users/browser/schema_layout.pt`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/schemaeditor.py` & `plone_app_users-3.0.6/plone/app/users/browser/schemaeditor.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/browser/userdatapanel.py` & `plone_app_users-3.0.6/plone/app/users/browser/userdatapanel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/configure.zcml` & `plone_app_users-3.0.6/plone/app/users/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/field_extender.py` & `plone_app_users-3.0.6/plone/app/users/field_extender.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/profiles/default/userschema.xml` & `plone_app_users-3.0.6/plone/app/users/profiles/default/userschema.xml`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/schema.py` & `plone_app_users-3.0.6/plone/app/users/schema.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/setuphandlers.py` & `plone_app_users-3.0.6/plone/app/users/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/testing.py` & `plone_app_users-3.0.6/plone/app/users/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/base.py` & `plone_app_users-3.0.6/plone/app/users/tests/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from Products.PluggableAuthService.interfaces.plugins import IValidationPlugin
 from Products.PluggableAuthService.plugins.BasePlugin import BasePlugin
 from Products.PluggableAuthService.utils import classImplements
 from transaction import commit
 from zope.component import getSiteManager
 from zope.component import getUtility
 
+import transaction
 import unittest
 
 
 class BaseTestCase(unittest.TestCase):
     """base test case which adds amin user"""
 
     layer = PLONE_APP_USERS_FUNCTIONAL_TESTING
@@ -39,14 +40,15 @@
         self.portal.acl_users._doAddUser("admin", TEST_USER_PASSWORD, ["Manager"], [])
         set_mock_mailhost(self.portal)
         self.membership = self.portal.portal_membership
         self.security_settings = get_security_settings()
 
         self.browser = Browser(self.layer["app"])
         self.request = self.layer["request"]
+        transaction.commit()
 
     def tearDown(self):
         login(self.portal, "admin")
         unset_mock_mailhost(self.portal)
         pas_instance = self.portal.acl_users
         plugin = getattr(pas_instance, "test", None)
         if plugin is not None:
```

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/duplicate_email.rst` & `plone_app_users-3.0.6/plone/app/users/tests/duplicate_email.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/email_login.rst` & `plone_app_users-3.0.6/plone/app/users/tests/email_login.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/flexible_user_registration.rst` & `plone_app_users-3.0.6/plone/app/users/tests/flexible_user_registration.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/forms_navigationroot.rst` & `plone_app_users-3.0.6/plone/app/users/tests/forms_navigationroot.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/member_search.rst` & `plone_app_users-3.0.6/plone/app/users/tests/member_search.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/password.rst` & `plone_app_users-3.0.6/plone/app/users/tests/password.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/personal_preferences.rst` & `plone_app_users-3.0.6/plone/app/users/tests/personal_preferences.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/personal_preferences_prefs_user_details.rst` & `plone_app_users-3.0.6/plone/app/users/tests/personal_preferences_prefs_user_details.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/plugins.rst` & `plone_app_users-3.0.6/plone/app/users/tests/plugins.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/registration_forms.rst` & `plone_app_users-3.0.6/plone/app/users/tests/registration_forms.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_account.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_doctests.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_exportimport.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_exportimport.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_loginname_generator.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_loginname_generator.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_member_search.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_member_search.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_new_user.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_new_user.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_pam.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_pam.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_schema_types.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_schema_types.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_user_data_panel.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_user_data_panel.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/test_userid_generator.py` & `plone_app_users-3.0.6/plone/app/users/tests/test_userid_generator.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/userdata.rst` & `plone_app_users-3.0.6/plone/app/users/tests/userdata.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/tests/userdata_prefs_user_details.rst` & `plone_app_users-3.0.6/plone/app/users/tests/userdata_prefs_user_details.rst`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/upgrades.py` & `plone_app_users-3.0.6/plone/app/users/upgrades.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/utils.py` & `plone_app_users-3.0.6/plone/app/users/utils.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone/app/users/vocabularies.py` & `plone_app_users-3.0.6/plone/app/users/vocabularies.py`

 * *Files identical despite different names*

### Comparing `plone.app.users-3.0.5/plone.app.users.egg-info/PKG-INFO` & `plone_app_users-3.0.6/plone.app.users.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.users
-Version: 3.0.5
+Version: 3.0.6
 Summary: A package for all things users and groups related (specific to plone)
 Home-page: https://pypi.org/project/plone.app.users
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: Zope CMF Plone Users Groups
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Requires-Dist: Acquisition
+Requires-Dist: Pillow
 Requires-Dist: Products.GenericSetup
 Requires-Dist: Products.PlonePAS>=5.0.1
 Requires-Dist: Products.statusmessages
 Requires-Dist: Zope
 Requires-Dist: plone.app.layout
 Requires-Dist: plone.autoform>=1.2
 Requires-Dist: plone.app.event
@@ -129,14 +130,26 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.6 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Fix #122 validating if image is supported by PIL showing a validation error if not.
+  Include Pillow dependency in setup.py.
+  Fix ValueError: User could not be found in BaseTest setUp adding a transaction.commit().
+  [rber474] (#122)
+
+
 3.0.5 (2024-03-19)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.users-3.0.5/plone.app.users.egg-info/SOURCES.txt` & `plone_app_users-3.0.6/plone.app.users.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,12 +64,14 @@
 plone/app/users/tests/test_account.py
 plone/app/users/tests/test_doctests.py
 plone/app/users/tests/test_exportimport.py
 plone/app/users/tests/test_loginname_generator.py
 plone/app/users/tests/test_member_search.py
 plone/app/users/tests/test_new_user.py
 plone/app/users/tests/test_pam.py
+plone/app/users/tests/test_portrait.py
 plone/app/users/tests/test_schema_types.py
 plone/app/users/tests/test_user_data_panel.py
 plone/app/users/tests/test_userid_generator.py
+plone/app/users/tests/transparent_square.svg
 plone/app/users/tests/userdata.rst
 plone/app/users/tests/userdata_prefs_user_details.rst
```

### Comparing `plone.app.users-3.0.5/plone.app.users.egg-info/requires.txt` & `plone_app_users-3.0.6/plone.app.users.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 Acquisition
+Pillow
 Products.GenericSetup
 Products.PlonePAS>=5.0.1
 Products.statusmessages
 Zope
 plone.app.layout
 plone.autoform>=1.2
 plone.app.event
```

### Comparing `plone.app.users-3.0.5/pyproject.toml` & `plone_app_users-3.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 ]
 'plone.base' = [
   'plone.batching', 'plone.registry', 'plone.schema','plone.z3cform',
   'Products.CMFCore', 'Products.CMFDynamicViewFTI',
 ]
 python-dateutil = ['dateutil']
 ignore-packages = ['Products.CMFPlone']
+Pillow = ['PIL']
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
 #    "gitpython = ['git']",
```

### Comparing `plone.app.users-3.0.5/setup.py` & `plone_app_users-3.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.5"
+version = "3.0.6"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 extras_require = {
     "test": [
@@ -55,14 +55,15 @@
     namespace_packages=["plone", "plone.app"],
     include_package_data=True,
     zip_safe=False,
     python_requires=">=3.8",
     extras_require=extras_require,
     install_requires=[
         "Acquisition",
+        "Pillow",
         "Products.GenericSetup",
         "Products.PlonePAS >= 5.0.1",
         "Products.statusmessages",
         "Zope",
         "plone.app.layout",
         "plone.autoform >= 1.2",
         "plone.app.event",
```

