# Comparing `tmp/kiwitcms-tenants-2.6.1.tar.gz` & `tmp/kiwitcms-tenants-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-tenants-2.6.1.tar", last modified: Fri Mar  8 22:51:10 2024, max compression
+gzip compressed data, was "kiwitcms-tenants-2.7.0.tar", last modified: Tue Apr 23 21:48:49 2024, max compression
```

## Comparing `kiwitcms-tenants-2.6.1.tar` & `kiwitcms-tenants-2.7.0.tar`

### file list

```diff
@@ -1,76 +1,82 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.6.1/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      205 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.6.1/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)    16519 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)    15701 2024-03-08 22:50:39.000000 kiwitcms-tenants-2.6.1/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.379619 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)    16519 2024-03-08 22:51:10.000000 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     1899 2024-03-08 22:51:10.000000 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-03-08 22:51:10.000000 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       51 2024-03-08 22:51:10.000000 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-03-08 22:51:10.000000 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       22 2024-03-08 22:51:10.000000 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       45 2024-03-08 22:51:10.000000 kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       22 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/requirements.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)       70 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1738 2024-03-08 22:50:39.000000 kiwitcms-tenants-2.6.1/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.379619 kiwitcms-tenants-2.6.1/tcms_settings_dir/
--rw-r--r--   0 senko     (1001) senko     (1001)       65 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_settings_dir/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     2455 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_settings_dir/multi_tenant.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.380619 kiwitcms-tenants-2.6.1/tcms_tenants/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:16.000000 kiwitcms-tenants-2.6.1/tcms_tenants/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     7410 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tcms_tenants/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      303 2022-01-24 11:23:06.000000 kiwitcms-tenants-2.6.1/tcms_tenants/apps.py
--rw-r--r--   0 senko     (1001) senko     (1001)      713 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tcms_tenants/backends.py
--rw-r--r--   0 senko     (1001) senko     (1001)      628 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/checks.py
--rw-r--r--   0 senko     (1001) senko     (1001)      821 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tcms_tenants/context_processors.py
--rw-r--r--   0 senko     (1001) senko     (1001)     3133 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/forms.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.378619 kiwitcms-tenants-2.6.1/tcms_tenants/locale/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.378619 kiwitcms-tenants-2.6.1/tcms_tenants/locale/en/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.380619 kiwitcms-tenants-2.6.1/tcms_tenants/locale/en/LC_MESSAGES/
--rw-r--r--   0 senko     (1001) senko     (1001)     4016 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tcms_tenants/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 senko     (1001) senko     (1001)      711 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/menu.py
--rw-r--r--   0 senko     (1001) senko     (1001)     2323 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/middleware.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.380619 kiwitcms-tenants-2.6.1/tcms_tenants/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     2394 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/migrations/0001_initial.py
--rw-r--r--   0 senko     (1001) senko     (1001)      617 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/migrations/0002_tenant_owner.py
--rw-r--r--   0 senko     (1001) senko     (1001)      596 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/migrations/0003_use_datetime_fields.py
--rw-r--r--   0 senko     (1001) senko     (1001)      434 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/migrations/0004_tenant_organization.py
--rw-r--r--   0 senko     (1001) senko     (1001)      553 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.6.1/tcms_tenants/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1350 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/models.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1133 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tcms_tenants/oss_utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1439 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/storage.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.378619 kiwitcms-tenants-2.6.1/tcms_tenants/templates/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.380619 kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.380619 kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/email/
--rw-rw-r--   0 senko     (1001) senko     (1001)      293 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/email/invite_user.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      151 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/email/new.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      904 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/invite_users.html
--rw-r--r--   0 senko     (1001) senko     (1001)     3614 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/new.html
--rw-r--r--   0 senko     (1001) senko     (1001)      297 2024-03-08 22:50:39.000000 kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/tenant_name.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.380619 kiwitcms-tenants-2.6.1/tcms_tenants/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.6.1/tcms_tenants/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      445 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.6.1/tcms_tenants/templatetags/tcms_tenants.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.380619 kiwitcms-tenants-2.6.1/tcms_tenants/tests/
--rw-r--r--   0 senko     (1001) senko     (1001)     3990 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/tests/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/tcms_tenants/tests/__pycache__/
--rw-rw-r--   0 senko     (1001) senko     (1001)     4446 2022-09-14 16:59:05.000000 kiwitcms-tenants-2.6.1/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 senko     (1001) senko     (1001)      599 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/urls.py
--rw-r--r--   0 senko     (1001) senko     (1001)     8010 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tcms_tenants/utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)     5408 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tcms_tenants/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/tenant_groups/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.6.1/tenant_groups/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2502 2022-04-27 19:02:16.000000 kiwitcms-tenants-2.6.1/tenant_groups/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      310 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.6.1/tenant_groups/apps.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1414 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tenant_groups/backends.py
--rw-r--r--   0 senko     (1001) senko     (1001)      722 2023-10-23 20:40:59.000000 kiwitcms-tenants-2.6.1/tenant_groups/checks.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/tenant_groups/management/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.6.1/tenant_groups/management/__init__.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/tenant_groups/management/commands/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.6.1/tenant_groups/management/commands/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1396 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tenant_groups/management/commands/refresh_tenant_permissions.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-03-08 22:51:10.381619 kiwitcms-tenants-2.6.1/tenant_groups/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     4132 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tenant_groups/migrations/0001_initial.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.6.1/tenant_groups/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1365 2024-01-13 22:40:48.000000 kiwitcms-tenants-2.6.1/tenant_groups/models.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      205 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)    17995 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)    17177 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.412761 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)    17995 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     2087 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       51 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       38 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       45 2024-04-23 21:48:49.000000 kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      103 2024-04-17 18:56:27.000000 kiwitcms-tenants-2.7.0/requirements.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      102 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1738 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.412761 kiwitcms-tenants-2.7.0/tcms_settings_dir/
+-rw-r--r--   0 senko     (1001) senko     (1001)       65 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_settings_dir/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2508 2024-04-22 20:07:06.000000 kiwitcms-tenants-2.7.0/tcms_settings_dir/multi_tenant.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:16.000000 kiwitcms-tenants-2.7.0/tcms_tenants/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     7647 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      303 2022-01-24 11:23:06.000000 kiwitcms-tenants-2.7.0/tcms_tenants/apps.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      713 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/backends.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      664 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/checks.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      821 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/context_processors.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     3171 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/forms.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.410761 kiwitcms-tenants-2.7.0/tcms_tenants/locale/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.410761 kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/LC_MESSAGES/
+-rw-r--r--   0 senko     (1001) senko     (1001)     4016 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/management/
+-rw-r--r--   0 senko     (1001) senko     (1001)        0 2024-04-23 20:52:30.000000 kiwitcms-tenants-2.7.0/tcms_tenants/management/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/management/commands/
+-rw-r--r--   0 senko     (1001) senko     (1001)        0 2024-04-23 20:52:30.000000 kiwitcms-tenants-2.7.0/tcms_tenants/management/commands/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2175 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/management/commands/initialize_tenants.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      766 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/menu.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2265 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/middleware.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     2782 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0001_initial.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      608 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0002_tenant_owner.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      596 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0003_use_datetime_fields.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      434 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0004_tenant_organization.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      553 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      476 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0006_tenant_extra_emails.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.7.0/tcms_tenants/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1409 2024-04-23 21:48:21.000000 kiwitcms-tenants-2.7.0/tcms_tenants/models.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1168 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/oss_utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1411 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/storage.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.410761 kiwitcms-tenants-2.7.0/tcms_tenants/templates/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/email/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      293 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/email/invite_user.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      151 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/email/new.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      904 2021-04-27 19:26:50.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/invite_users.html
+-rw-r--r--   0 senko     (1001) senko     (1001)     3614 2024-04-23 19:00:56.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/new.html
+-rw-r--r--   0 senko     (1001) senko     (1001)      297 2024-04-17 13:35:28.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/tenant_name.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      445 2021-05-19 13:48:39.000000 kiwitcms-tenants-2.7.0/tcms_tenants/templatetags/tcms_tenants.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.413761 kiwitcms-tenants-2.7.0/tcms_tenants/tests/
+-rw-r--r--   0 senko     (1001) senko     (1001)     3999 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/tests/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tcms_tenants/tests/__pycache__/
+-rw-rw-r--   0 senko     (1001) senko     (1001)     4446 2022-09-14 16:59:05.000000 kiwitcms-tenants-2.7.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 senko     (1001) senko     (1001)      618 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/urls.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     8255 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     5331 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tcms_tenants/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.7.0/tenant_groups/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2502 2022-04-27 19:02:16.000000 kiwitcms-tenants-2.7.0/tenant_groups/admin.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      310 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.7.0/tenant_groups/apps.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1405 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/backends.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      754 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/checks.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/management/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.7.0/tenant_groups/management/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/management/commands/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-25 17:51:43.000000 kiwitcms-tenants-2.7.0/tenant_groups/management/commands/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1434 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/management/commands/refresh_tenant_permissions.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-04-23 21:48:49.414761 kiwitcms-tenants-2.7.0/tenant_groups/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     4427 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/migrations/0001_initial.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2022-04-17 20:01:15.000000 kiwitcms-tenants-2.7.0/tenant_groups/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1380 2024-04-18 17:27:02.000000 kiwitcms-tenants-2.7.0/tenant_groups/models.py
```

### Comparing `kiwitcms-tenants-2.6.1/LICENSE` & `kiwitcms-tenants-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/PKG-INFO` & `kiwitcms-tenants-2.7.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: kiwitcms-tenants
-Version: 2.6.1
-Summary: Multi-tenant support for Kiwi TCMS
-Home-page: https://github.com/kiwitcms/tenants/
-Author: Kiwi TCMS
-Author-email: info@kiwitcms.org
-License: GPLv3+
-Classifier: Framework :: Django
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
-
 Multi-tenant support for Kiwi TCMS
 ==================================
 
 .. image:: https://travis-ci.org/kiwitcms/tenants.svg?branch=master
     :target: https://travis-ci.org/kiwitcms/tenants
 
 .. image:: https://coveralls.io/repos/github/kiwitcms/tenants/badge.svg?branch=master
@@ -137,17 +116,52 @@
 See `Migrating Single-Tenant to Multi-Tenant
 <https://django-tenants.readthedocs.io/en/latest/use.html#migrating-single-tenant-to-multi-tenant>`_
 section in the official django-tenants documentation! It has been contributed by the Kiwi TCMS
 team and that was the procedure we've used to migrate the previous demo website (ST) to
 its new MT version!
 
 
+Local Development
+-----------------
+
+Starting with Kiwi TCMS v13.1 session and CSRF cookies are configured only on HTTPS
+connections which will prevent browsers from sending cookies over a plain text HTTP
+connection. This will result in not being able to login if you are using a local
+development server. To workaround this issue, first generate an SSL certificate::
+
+    /usr/bin/sscg -v -f --country BG --locality Sofia --organization "Kiwi TCMS" --organizational-unit "QA" --ca-file ssl/ca.crt --cert-file ssl/host.crt --cert-key-file ssl/host.key
+
+Then use the ``runerver_plus`` command to start Kiwi TCMS development server with HTTPS::
+
+    PYTHONPATH=../Kiwi/ KIWI_TENANTS_DOMAIN=tenant.example.bg ./manage.py runserver_plus --cert-file ssl/host.crt  --key-file ssl/host.key
+
+Then point your browser to https://tenant.example.bg:8000/.
+The SSL warning from the browser is expected!
+
+You can use ``/etc/hosts`` to configure DNS resolution during development::
+
+    127.0.0.1   localhost tenant.example.bg empty.tenant.example.bg
+
+
 Changelog
 ---------
 
+v2.7.0 (24 Apr 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Add the ``Tenant.extra_emails`` field for storing information like
+  technical email, billing email, etc. To be used by add-on tools
+- Add the ``initialize_tenants`` management command
+- Update local development instructions
+- Enable code formatting with ``black``
+- Start testing using upstream Postgres container
+- Execute CodeQL on pull request and branches
+- Adjust tests for Django 5.0
+
+
 v2.6.1 (08 Mar 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Remove use of ``non-existing.png`` file in tenant name area
   to avoid 404 responses which trigger rate limiting
```

### Comparing `kiwitcms-tenants-2.6.1/README.rst` & `kiwitcms-tenants-2.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: kiwitcms-tenants
+Version: 2.7.0
+Summary: Multi-tenant support for Kiwi TCMS
+Home-page: https://github.com/kiwitcms/tenants/
+Author: Kiwi TCMS
+Author-email: info@kiwitcms.org
+License: GPLv3+
+Classifier: Framework :: Django
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
 Multi-tenant support for Kiwi TCMS
 ==================================
 
 .. image:: https://travis-ci.org/kiwitcms/tenants.svg?branch=master
     :target: https://travis-ci.org/kiwitcms/tenants
 
 .. image:: https://coveralls.io/repos/github/kiwitcms/tenants/badge.svg?branch=master
@@ -116,17 +137,52 @@
 See `Migrating Single-Tenant to Multi-Tenant
 <https://django-tenants.readthedocs.io/en/latest/use.html#migrating-single-tenant-to-multi-tenant>`_
 section in the official django-tenants documentation! It has been contributed by the Kiwi TCMS
 team and that was the procedure we've used to migrate the previous demo website (ST) to
 its new MT version!
 
 
+Local Development
+-----------------
+
+Starting with Kiwi TCMS v13.1 session and CSRF cookies are configured only on HTTPS
+connections which will prevent browsers from sending cookies over a plain text HTTP
+connection. This will result in not being able to login if you are using a local
+development server. To workaround this issue, first generate an SSL certificate::
+
+    /usr/bin/sscg -v -f --country BG --locality Sofia --organization "Kiwi TCMS" --organizational-unit "QA" --ca-file ssl/ca.crt --cert-file ssl/host.crt --cert-key-file ssl/host.key
+
+Then use the ``runerver_plus`` command to start Kiwi TCMS development server with HTTPS::
+
+    PYTHONPATH=../Kiwi/ KIWI_TENANTS_DOMAIN=tenant.example.bg ./manage.py runserver_plus --cert-file ssl/host.crt  --key-file ssl/host.key
+
+Then point your browser to https://tenant.example.bg:8000/.
+The SSL warning from the browser is expected!
+
+You can use ``/etc/hosts`` to configure DNS resolution during development::
+
+    127.0.0.1   localhost tenant.example.bg empty.tenant.example.bg
+
+
 Changelog
 ---------
 
+v2.7.0 (24 Apr 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Add the ``Tenant.extra_emails`` field for storing information like
+  technical email, billing email, etc. To be used by add-on tools
+- Add the ``initialize_tenants`` management command
+- Update local development instructions
+- Enable code formatting with ``black``
+- Start testing using upstream Postgres container
+- Execute CodeQL on pull request and branches
+- Adjust tests for Django 5.0
+
+
 v2.6.1 (08 Mar 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Remove use of ``non-existing.png`` file in tenant name area
   to avoid 404 responses which trigger rate limiting
```

### Comparing `kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/PKG-INFO` & `kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-tenants
-Version: 2.6.1
+Version: 2.7.0
 Summary: Multi-tenant support for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/tenants/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -137,17 +137,52 @@
 See `Migrating Single-Tenant to Multi-Tenant
 <https://django-tenants.readthedocs.io/en/latest/use.html#migrating-single-tenant-to-multi-tenant>`_
 section in the official django-tenants documentation! It has been contributed by the Kiwi TCMS
 team and that was the procedure we've used to migrate the previous demo website (ST) to
 its new MT version!
 
 
+Local Development
+-----------------
+
+Starting with Kiwi TCMS v13.1 session and CSRF cookies are configured only on HTTPS
+connections which will prevent browsers from sending cookies over a plain text HTTP
+connection. This will result in not being able to login if you are using a local
+development server. To workaround this issue, first generate an SSL certificate::
+
+    /usr/bin/sscg -v -f --country BG --locality Sofia --organization "Kiwi TCMS" --organizational-unit "QA" --ca-file ssl/ca.crt --cert-file ssl/host.crt --cert-key-file ssl/host.key
+
+Then use the ``runerver_plus`` command to start Kiwi TCMS development server with HTTPS::
+
+    PYTHONPATH=../Kiwi/ KIWI_TENANTS_DOMAIN=tenant.example.bg ./manage.py runserver_plus --cert-file ssl/host.crt  --key-file ssl/host.key
+
+Then point your browser to https://tenant.example.bg:8000/.
+The SSL warning from the browser is expected!
+
+You can use ``/etc/hosts`` to configure DNS resolution during development::
+
+    127.0.0.1   localhost tenant.example.bg empty.tenant.example.bg
+
+
 Changelog
 ---------
 
+v2.7.0 (24 Apr 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Add the ``Tenant.extra_emails`` field for storing information like
+  technical email, billing email, etc. To be used by add-on tools
+- Add the ``initialize_tenants`` management command
+- Update local development instructions
+- Enable code formatting with ``black``
+- Start testing using upstream Postgres container
+- Execute CodeQL on pull request and branches
+- Adjust tests for Django 5.0
+
+
 v2.6.1 (08 Mar 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Remove use of ``non-existing.png`` file in tenant name area
   to avoid 404 responses which trigger rate limiting
```

### Comparing `kiwitcms-tenants-2.6.1/kiwitcms_tenants.egg-info/SOURCES.txt` & `kiwitcms-tenants-2.7.0/kiwitcms_tenants.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,19 +25,23 @@
 tcms_tenants/models.py
 tcms_tenants/oss_utils.py
 tcms_tenants/storage.py
 tcms_tenants/urls.py
 tcms_tenants/utils.py
 tcms_tenants/views.py
 tcms_tenants/locale/en/LC_MESSAGES/django.po
+tcms_tenants/management/__init__.py
+tcms_tenants/management/commands/__init__.py
+tcms_tenants/management/commands/initialize_tenants.py
 tcms_tenants/migrations/0001_initial.py
 tcms_tenants/migrations/0002_tenant_owner.py
 tcms_tenants/migrations/0003_use_datetime_fields.py
 tcms_tenants/migrations/0004_tenant_organization.py
 tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py
+tcms_tenants/migrations/0006_tenant_extra_emails.py
 tcms_tenants/migrations/__init__.py
 tcms_tenants/templates/tcms_tenants/invite_users.html
 tcms_tenants/templates/tcms_tenants/new.html
 tcms_tenants/templates/tcms_tenants/tenant_name.html
 tcms_tenants/templates/tcms_tenants/email/invite_user.txt
 tcms_tenants/templates/tcms_tenants/email/new.txt
 tcms_tenants/templatetags/__init__.py
```

### Comparing `kiwitcms-tenants-2.6.1/setup.py` & `kiwitcms-tenants-2.7.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,50 +4,50 @@
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 from setuptools import setup, find_packages
 
 
 def get_long_description():
-    with open('README.rst', 'r', encoding="utf-8") as file:
+    with open("README.rst", "r", encoding="utf-8") as file:
         return file.read()
 
 
 def get_install_requires(path):
     requires = []
 
-    with open(path, 'r', encoding="utf-8") as file:
+    with open(path, "r", encoding="utf-8") as file:
         for line in file:
-            if line.startswith('-r '):
+            if line.startswith("-r "):
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
-    name='kiwitcms-tenants',
-    version='2.6.1',
-    description='Multi-tenant support for Kiwi TCMS',
+    name="kiwitcms-tenants",
+    version="2.7.0",
+    description="Multi-tenant support for Kiwi TCMS",
     long_description=get_long_description(),
-    author='Kiwi TCMS',
-    author_email='info@kiwitcms.org',
-    url='https://github.com/kiwitcms/tenants/',
-    license='GPLv3+',
-    install_requires=get_install_requires('requirements.txt'),
+    author="Kiwi TCMS",
+    author_email="info@kiwitcms.org",
+    url="https://github.com/kiwitcms/tenants/",
+    license="GPLv3+",
+    install_requires=get_install_requires("requirements.txt"),
     include_package_data=True,
-    packages=find_packages(exclude=['test_project*', '*.tests']),
+    packages=find_packages(exclude=["test_project*", "*.tests"]),
     zip_safe=False,
     entry_points={"kiwitcms.plugins": ["kiwitcms_tenants = tcms_tenants"]},
     classifiers=[
-        'Framework :: Django',
-        'Development Status :: 5 - Production/Stable',
-        'Topic :: Software Development :: Quality Assurance',
-        'Topic :: Software Development :: Testing',
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.11',
+        "Framework :: Django",
+        "Development Status :: 5 - Production/Stable",
+        "Topic :: Software Development :: Quality Assurance",
+        "Topic :: Software Development :: Testing",
+        "Environment :: Web Environment",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_settings_dir/multi_tenant.py` & `kiwitcms-tenants-2.7.0/tcms_settings_dir/multi_tenant.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,60 +2,82 @@
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 # pylint: disable=undefined-variable
 import os
 
 
 # start multi-tenant settings override
-DATABASES['default']['ENGINE'] = 'django_tenants.postgresql_backend'  # noqa: F821
-DATABASE_ROUTERS = ['django_tenants.routers.TenantSyncRouter', ]
+DATABASES["default"]["ENGINE"] = "django_tenants.postgresql_backend"  # noqa: F821
+DATABASE_ROUTERS = [
+    "django_tenants.routers.TenantSyncRouter",
+]
 
 
 # attachments storage
 DEFAULT_FILE_STORAGE = "tcms_tenants.storage.TenantFileSystemStorage"
 MULTITENANT_RELATIVE_MEDIA_ROOT = "tenant/%s"
 
 
 # this always needs to be the first app
-if 'django_tenants' not in INSTALLED_APPS:      # noqa: F821
-    INSTALLED_APPS.insert(0, 'django_tenants')  # noqa: F821
+if "django_tenants" not in INSTALLED_APPS:  # noqa: F821
+    INSTALLED_APPS.insert(0, "django_tenants")  # noqa: F821
 
 for app_list in (INSTALLED_APPS, TENANT_APPS):  # noqa: F821
-    if 'tenant_groups' not in app_list:
-        app_list.append('tenant_groups')
+    if "tenant_groups" not in app_list:
+        app_list.append("tenant_groups")
 
 
-KIWI_TENANTS_DOMAIN = os.environ.get('KIWI_TENANTS_DOMAIN')
+KIWI_TENANTS_DOMAIN = os.environ.get("KIWI_TENANTS_DOMAIN")
 
 
 # TenantMainMiddleware always needs to be first
-if 'django_tenants.middleware.main.TenantMainMiddleware' not in MIDDLEWARE:      # noqa: F821
-    MIDDLEWARE.insert(0, 'django_tenants.middleware.main.TenantMainMiddleware')  # noqa: F821
-
-if 'tcms_tenants.middleware.BlockUnauthorizedUserMiddleware' not in MIDDLEWARE:   # noqa: F821
-    MIDDLEWARE.append('tcms_tenants.middleware.BlockUnauthorizedUserMiddleware')  # noqa: F821
+if (
+    "django_tenants.middleware.main.TenantMainMiddleware"
+    not in MIDDLEWARE  # noqa: F821
+):
+    MIDDLEWARE.insert(  # noqa: F821
+        0, "django_tenants.middleware.main.TenantMainMiddleware"
+    )
+
+if (
+    "tcms_tenants.middleware.BlockUnauthorizedUserMiddleware"
+    not in MIDDLEWARE  # noqa: F821
+):
+    MIDDLEWARE.append(  # noqa: F821
+        "tcms_tenants.middleware.BlockUnauthorizedUserMiddleware"
+    )
 
 # replace ModelBackend with GroupsBackend
-if 'django.contrib.auth.backends.ModelBackend' in AUTHENTICATION_BACKENDS:            # noqa: F821
-    idx = AUTHENTICATION_BACKENDS.index('django.contrib.auth.backends.ModelBackend')  # noqa: F821
-    AUTHENTICATION_BACKENDS[idx] = 'tenant_groups.backends.GroupsBackend'             # noqa: F821
-
-if 'tcms_tenants.backends.PubliclyReadableBackend' not in AUTHENTICATION_BACKENDS:   # noqa: F821
-    AUTHENTICATION_BACKENDS.append('tcms_tenants.backends.PubliclyReadableBackend')  # noqa: F821
+if "django.contrib.auth.backends.ModelBackend" in AUTHENTICATION_BACKENDS:  # noqa: F821
+    idx = AUTHENTICATION_BACKENDS.index(  # noqa: F821
+        "django.contrib.auth.backends.ModelBackend"
+    )
+    AUTHENTICATION_BACKENDS[idx] = "tenant_groups.backends.GroupsBackend"  # noqa: F821
+
+if (
+    "tcms_tenants.backends.PubliclyReadableBackend"
+    not in AUTHENTICATION_BACKENDS  # noqa: F821
+):
+    AUTHENTICATION_BACKENDS.append(  # noqa: F821
+        "tcms_tenants.backends.PubliclyReadableBackend"
+    )
 
 
 TENANT_MODEL = "tcms_tenants.Tenant"
 TENANT_DOMAIN_MODEL = "tcms_tenants.Domain"
 
 
 # share login session between tenants
 SESSION_COOKIE_DOMAIN = f".{KIWI_TENANTS_DOMAIN}"
 
 
 # everybody can access the main instance
 SHARED_APPS = INSTALLED_APPS  # noqa: F821
 
 # add tennants context processor
-if 'tcms_tenants.context_processors.tenant_navbar_processor' not in\
-        TEMPLATES[0]['OPTIONS']['context_processors']:              # noqa: F821
-    TEMPLATES[0]['OPTIONS']['context_processors'].append(           # noqa: F821
-        'tcms_tenants.context_processors.tenant_navbar_processor')  # noqa: F821
+if (
+    "tcms_tenants.context_processors.tenant_navbar_processor"
+    not in TEMPLATES[0]["OPTIONS"]["context_processors"]  # noqa: F821
+):
+    TEMPLATES[0]["OPTIONS"]["context_processors"].append(  # noqa: F821
+        "tcms_tenants.context_processors.tenant_navbar_processor"
+    )  # noqa: F821
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/admin.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2022 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 
 from django import forms
 from django.urls import reverse
 from django.contrib import admin
@@ -14,176 +14,221 @@
 
 from tcms_tenants.models import Tenant
 from tcms_tenants.utils import add_to_default_groups, owns_tenant, tenant_url
 
 
 class TenantAdmin(admin.ModelAdmin):
     """
-        Allows only super-user to see and delete tenants!
+    Allows only super-user to see and delete tenants!
     """
-    actions = ['delete_selected']
-    list_display = ('id', 'name', 'schema_name', 'domain_name', 'created_on', 'publicly_readable',
-                    'paid_until', 'owner', 'organization')
-    search_fields = ('name', 'schema_name', 'organization')
-    ordering = ['-created_on']
 
-    def add_view(self, request, form_url='', extra_context=None):
-        return HttpResponseRedirect(reverse('tcms_tenants:create-tenant'))
+    actions = ["delete_selected"]
+    list_display = (
+        "id",
+        "name",
+        "schema_name",
+        "domain_name",
+        "created_on",
+        "publicly_readable",
+        "paid_until",
+        "owner",
+        "extra_emails",
+        "organization",
+    )
+    search_fields = ("name", "schema_name", "organization")
+    ordering = ["-created_on"]
+
+    def add_view(self, request, form_url="", extra_context=None):
+        return HttpResponseRedirect(reverse("tcms_tenants:create-tenant"))
 
-    def change_view(self, request, object_id, form_url='', extra_context=None):
+    def change_view(self, request, object_id, form_url="", extra_context=None):
         tenant = Tenant.objects.get(pk=object_id)
-        target_url = tenant_url(request, tenant.schema_name) + reverse('tcms_tenants:edit-tenant')
+        target_url = tenant_url(request, tenant.schema_name) + reverse(
+            "tcms_tenants:edit-tenant"
+        )
         return HttpResponseRedirect(target_url)
 
     @admin.options.csrf_protect_m
     def changelist_view(self, request, extra_context=None):
         if request.user.is_superuser:
             return super().changelist_view(request, extra_context)
 
-        return HttpResponseForbidden(_('Unauthorized'))
+        return HttpResponseForbidden(_("Unauthorized"))
 
     @admin.options.csrf_protect_m
     def delete_view(self, request, object_id, extra_context=None):
         if request.user.is_superuser:
             return super().delete_view(request, object_id, extra_context)
 
-        return HttpResponseForbidden(_('Unauthorized'))
+        return HttpResponseForbidden(_("Unauthorized"))
 
     def domain_name(self, instance):  # pylint: disable=no-self-use
         return instance.domains.filter(is_primary=True).first().domain
 
 
 class AuthorizedUsersChangeForm(forms.ModelForm):
     """
-        A custom add/change form which will filter the available
-        values of the ``tenant`` field so that only the current
-        tenant is shown!
+    A custom add/change form which will filter the available
+    values of the ``tenant`` field so that only the current
+    tenant is shown!
     """
+
     # IMPORTANT NOTICE:
     # As a security concern we would like to have this queryset set to
     # Tenant.objects.none() instead of .all(). However ModelChoiceField.to_python()
     # is trying to self.queryset.get() the currently selected value! When the queryset
     # is empty this raises ValidationError!
     # The internal mechanics of this are in BaseForm._clean_fields()::L399(Django 2.1.7)
     # which calls field.clean(value) before any clean_<field_name>() methods on the form!
     tenant = forms.models.ModelChoiceField(
         queryset=Tenant.objects.all(),
     )
     user = UserField(  # pylint: disable=form-field-help-text-used
-        help_text=_('Existing username, email or user ID')
+        help_text=_("Existing username, email or user ID")
     )
 
-    def __init__(self,  # pylint: disable=too-many-arguments
-                 data=None, files=None, auto_id='id_%s', prefix=None,
-                 initial=None, error_class=ErrorList, label_suffix=None,
-                 empty_permitted=False, instance=None, use_required_attribute=None,
-                 renderer=None):
-        super().__init__(data, files, auto_id, prefix,
-                         initial, error_class, label_suffix,
-                         empty_permitted, instance, use_required_attribute,
-                         renderer)
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        data=None,
+        files=None,
+        auto_id="id_%s",
+        prefix=None,
+        initial=None,
+        error_class=ErrorList,
+        label_suffix=None,
+        empty_permitted=False,
+        instance=None,
+        use_required_attribute=None,
+        renderer=None,
+    ):
+        super().__init__(
+            data,
+            files,
+            auto_id,
+            prefix,
+            initial,
+            error_class,
+            label_suffix,
+            empty_permitted,
+            instance,
+            use_required_attribute,
+            renderer,
+        )
         # this is passed by ModelAdmin._chageform_view():L1578
         # when adding a new object
-        if initial and 'tenant' in initial:
-            self.fields['tenant'].queryset = Tenant.objects.filter(pk=initial['tenant'])
+        if initial and "tenant" in initial:
+            self.fields["tenant"].queryset = Tenant.objects.filter(pk=initial["tenant"])
         # this is passed by ModelAdmin._chageform_view():L1581
         # when changing an existing object
         elif instance:
-            self.fields['tenant'].queryset = Tenant.objects.filter(pk=instance.tenant.pk)
+            self.fields["tenant"].queryset = Tenant.objects.filter(
+                pk=instance.tenant.pk
+            )
 
     def save(self, commit=True):
         instance = super().save(commit=commit)
         instance.save()
 
         add_to_default_groups(self.instance.user)
         return instance
 
 
 class AuthorizedUsersAdmin(admin.ModelAdmin):
     """
-        Allows administering which users are authorized for tenants!
+    Allows administering which users are authorized for tenants!
     """
-    actions = ['delete_selected']
-    list_display = ('user_username', 'user_full_name', 'groups',)
-    search_fields = ('user__username',)
+
+    actions = ["delete_selected"]
+    list_display = (
+        "user_username",
+        "user_full_name",
+        "groups",
+    )
+    search_fields = ("user__username",)
 
     form = AuthorizedUsersChangeForm
 
     def user_username(self, instance):  # pylint: disable=no-self-use
         return instance.user.username
-    user_username.short_description = _('Username')
-    user_username.admin_order_field = 'user__username'
+
+    user_username.short_description = _("Username")
+    user_username.admin_order_field = "user__username"
 
     def user_full_name(self, instance):  # pylint: disable=no-self-use
         return instance.user.get_full_name()
-    user_full_name.short_description = _('Full name')
+
+    user_full_name.short_description = _("Full name")
 
     def groups(self, instance):  # pylint: disable=no-self-use
-        return list(instance.user.tenant_groups.values_list('name', flat=True))
-    groups.short_description = _('Groups')
+        return list(instance.user.tenant_groups.values_list("name", flat=True))
+
+    groups.short_description = _("Groups")
 
     def get_queryset(self, request):
         """
-            Show only users authorized for the current tenant!
+        Show only users authorized for the current tenant!
         """
         return super().get_queryset(request).filter(tenant=request.tenant)
 
     # pylint: disable=too-many-arguments
-    def render_change_form(self, request, context, add=False, change=False, form_url='', obj=None):
-        context[
-            'adminform'
-        ].form.fields['tenant'].queryset = Tenant.objects.filter(pk=request.tenant.pk)
+    def render_change_form(
+        self, request, context, add=False, change=False, form_url="", obj=None
+    ):
+        context["adminform"].form.fields["tenant"].queryset = Tenant.objects.filter(
+            pk=request.tenant.pk
+        )
 
         return super().render_change_form(
-            request, context, add=add, change=change, form_url=form_url, obj=obj)
+            request, context, add=add, change=change, form_url=form_url, obj=obj
+        )
 
     def get_changeform_initial_data(self, request):
         """
-            Pass the current tenant to AuthorizedUsersChangeForm.__init__()
-            which will filter the available tenants and only show the current
-            one when add/change objects!
+        Pass the current tenant to AuthorizedUsersChangeForm.__init__()
+        which will filter the available tenants and only show the current
+        one when add/change objects!
         """
-        return {'tenant': request.tenant.pk}
+        return {"tenant": request.tenant.pk}
 
     def has_add_permission(self, request):
         """
-            Allow to add new authorized users.
+        Allow to add new authorized users.
         """
         return owns_tenant(request.user, request.tenant)
 
     def has_change_permission(self, request, obj=None):
         """
-            Allow to display the list of of authorized users.
+        Allow to display the list of of authorized users.
         """
         return owns_tenant(request.user, request.tenant)
 
     def has_delete_permission(self, request, obj=None):
         """
-            Allow to delete selected users.
+        Allow to delete selected users.
         """
         return request.user.is_superuser or owns_tenant(request.user, request.tenant)
 
     def has_module_permission(self, request):
         """
-            Allow this module to be seen in main admin page.
+        Allow this module to be seen in main admin page.
         """
         return owns_tenant(request.user, request.tenant)
 
     def get_model_perms(self, request):
         """
-            Allow this module to be seen in main admin page.
+        Allow this module to be seen in main admin page.
         """
         if request.user.is_superuser:
             return super().get_model_perms(request)
 
-        return {'view': owns_tenant(request.user, request.tenant)}
+        return {"view": owns_tenant(request.user, request.tenant)}
 
     def delete_model(self, request, obj):
         """
-            Remove user from tenant groups before removing the authorization!
+        Remove user from tenant groups before removing the authorization!
         """
         for group in obj.user.tenant_groups.all():
             group.user_set.remove(obj.user)
 
         super().delete_model(request, obj)
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/backends.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/backends.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/checks.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/checks.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 import os
 
 from django.core import checks
 
 
 def tenants_env_check(app_configs, **kwargs):  # pylint: disable=unused-argument
     errors = []
-    if not os.environ.get('KIWI_TENANTS_DOMAIN'):
+    if not os.environ.get("KIWI_TENANTS_DOMAIN"):
         errors.append(
             checks.Error(
-                msg='KIWI_TENANTS_DOMAIN environment variable is not set!',
-                hint=('This variable is mandatory, '
-                      'see https://github.com/kiwitcms/tenants#installation'),
+                msg="KIWI_TENANTS_DOMAIN environment variable is not set!",
+                hint=(
+                    "This variable is mandatory, "
+                    "see https://github.com/kiwitcms/tenants#installation"
+                ),
             )
         )
     return errors
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/context_processors.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/context_processors.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/forms.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/forms.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,40 +10,48 @@
 
 from django_tenants.postgresql_backend import base as validators
 
 from tcms_tenants import models
 from tcms_tenants import utils
 
 
-VALIDATION_RE = re.compile(r'^[a-z0-9]{1,63}$')
+VALIDATION_RE = re.compile(r"^[a-z0-9]{1,63}$")
 
 
 def _check_domain_name(name):
     """
-        Because we use schema_name as sub-domains interchangeably
-        we impose additional restriction on input values:
-            alpha-numeric, 63 chars max
+    Because we use schema_name as sub-domains interchangeably
+    we impose additional restriction on input values:
+        alpha-numeric, 63 chars max
     """
     if not VALIDATION_RE.match(name):
-        raise ValidationError(_('Invalid string'))
+        raise ValidationError(_("Invalid string"))
 
 
 class NewTenantForm(forms.ModelForm):
     class Meta:
         model = models.Tenant
         exclude = ("authorized_users",)  # pylint: disable=modelform-uses-exclude
 
-    schema_name = forms.CharField(max_length=63,
-                                  # pylint: disable=protected-access
-                                  validators=[validators._check_schema_name,
-                                              _check_domain_name,
-                                              utils.schema_name_not_used])
+    schema_name = forms.CharField(
+        max_length=63,
+        # pylint: disable=protected-access
+        validators=[
+            validators._check_schema_name,
+            _check_domain_name,
+            utils.schema_name_not_used,
+        ],
+    )
     paid_until = forms.DateTimeField(required=False, widget=forms.HiddenInput)
-    organization = forms.CharField(max_length=64, required=False,
-                                   widget=forms.HiddenInput)
+    organization = forms.CharField(
+        max_length=64, required=False, widget=forms.HiddenInput
+    )
+    extra_emails = forms.CharField(
+        max_length=256, required=False, widget=forms.HiddenInput
+    )
 
 
 class InviteUsersForm(forms.Form):  # pylint: disable=must-inherit-from-model-form
     number_of_fields = 10
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -63,15 +71,19 @@
 
     @property
     def range(self):
         return range(self.number_of_fields)
 
 
 class UpdateTenantForm(NewTenantForm):
-    enabled_fields = ('name', 'publicly_readable',)
+    enabled_fields = (
+        "name",
+        "publicly_readable",
+        "extra_emails",
+    )
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         data=None,
         files=None,
         auto_id="id_%s",
         prefix=None,
@@ -97,8 +109,8 @@
             renderer,
         )
 
         for field in self.fields:
             self.fields[field].disabled = field not in self.enabled_fields
 
         # remove validator which only makes sense when creating new tenants
-        self.fields['schema_name'].validators.remove(utils.schema_name_not_used)
+        self.fields["schema_name"].validators.remove(utils.schema_name_not_used)
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/locale/en/LC_MESSAGES/django.po` & `kiwitcms-tenants-2.7.0/tcms_tenants/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/middleware.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,58 +10,63 @@
 from django.utils.translation import gettext_lazy as _
 
 from tcms_tenants.utils import can_access
 
 
 class BlockUnauthorizedUserMiddleware:
     """
-        Raises 403 if the user making the request is not authorized
-        explicitly to access the tenant instance!
+    Raises 403 if the user making the request is not authorized
+    explicitly to access the tenant instance!
 
-        .. warning:
+    .. warning:
 
-            This must be placed after
-            ``django_tenants.middleware.main.TenantMainMiddleware`` and
-            ``django.contrib.auth.middleware.AuthenticationMiddleware`` -
-            usually goes at the end
+        This must be placed after
+        ``django_tenants.middleware.main.TenantMainMiddleware`` and
+        ``django.contrib.auth.middleware.AuthenticationMiddleware`` -
+        usually goes at the end
     """
+
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request):  # pylint: disable=no-self-use
         if not can_access(request.user, request.tenant):
-            return HttpResponseForbidden(_('Unauthorized'))
+            return HttpResponseForbidden(_("Unauthorized"))
 
         return self.get_response(request)
 
 
 class BlockUnpaidTenantMiddleware:
     """
-        Blocks unpaid tenants or adds warning messages if tenant is about to
-        expire soon!
+    Blocks unpaid tenants or adds warning messages if tenant is about to
+    expire soon!
 
-        .. warning:
+    .. warning:
 
-            This must be placed after
-            ``tcms_tenants.middleware.BlockUnauthorizedUserMiddleware`` -
-            usually goes at the end.
+        This must be placed after
+        ``tcms_tenants.middleware.BlockUnauthorizedUserMiddleware`` -
+        usually goes at the end.
     """
+
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request):
-        if (request.tenant.paid_until is None) or \
-                (request.tenant.paid_until <= timezone.now()):
-            return HttpResponseForbidden(_('Unpaid'))
+        if (request.tenant.paid_until is None) or (
+            request.tenant.paid_until <= timezone.now()
+        ):
+            return HttpResponseForbidden(_("Unpaid"))
 
         if request.tenant.paid_until <= timezone.now() + timedelta(days=7):
             for msg in messages.get_messages(request):
-                if msg.level_tag == 'warning':
+                if msg.level_tag == "warning":
                     break
             else:
                 # will be shown only if no other warnings are present
-                messages.add_message(request,
-                                     messages.WARNING,
-                                     _('Tenant expires in less than 7 days'),
-                                     fail_silently=True)
+                messages.add_message(
+                    request,
+                    messages.WARNING,
+                    _("Tenant expires in less than 7 days"),
+                    fail_silently=True,
+                )
 
         return self.get_response(request)
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/migrations/0003_use_datetime_fields.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0003_use_datetime_fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('tcms_tenants', '0002_tenant_owner'),
+        ("tcms_tenants", "0002_tenant_owner"),
     ]
 
     operations = [
         migrations.AlterField(
-            model_name='tenant',
-            name='created_on',
+            model_name="tenant",
+            name="created_on",
             field=models.DateTimeField(auto_now_add=True, db_index=True),
         ),
         migrations.AlterField(
-            model_name='tenant',
-            name='paid_until',
+            model_name="tenant",
+            name="paid_until",
             field=models.DateTimeField(blank=True, db_index=True, null=True),
         ),
     ]
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/migrations/0005_rename_on_trial_to_public_read.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
-        ('tcms_tenants', '0004_tenant_organization'),
+        ("tcms_tenants", "0004_tenant_organization"),
     ]
 
     operations = [
         migrations.RenameField(
-            model_name='tenant',
-            old_name='on_trial',
-            new_name='publicly_readable',
+            model_name="tenant",
+            old_name="on_trial",
+            new_name="publicly_readable",
         ),
         # change the defaults
         migrations.AlterField(
             model_name="tenant",
             name="publicly_readable",
             field=models.BooleanField(default=False, db_index=True),
         ),
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/models.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-# Copyright (c) 2019-2021 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 import os
 
 from django.db import models
 from django.conf import settings
+
 from django_tenants.models import TenantMixin, DomainMixin
 
 
 class Tenant(TenantMixin):
-    auto_create_schema = bool(os.environ.get('AUTO_CREATE_SCHEMA', True))
+    auto_create_schema = bool(os.environ.get("AUTO_CREATE_SCHEMA", True))
     auto_drop_schema = True
 
     name = models.CharField(max_length=100, db_index=True)
     created_on = models.DateTimeField(auto_now_add=True, db_index=True)
     paid_until = models.DateTimeField(null=True, blank=True, db_index=True)
     publicly_readable = models.BooleanField(default=False, db_index=True)
     authorized_users = models.ManyToManyField(to=settings.AUTH_USER_MODEL)
-    owner = models.ForeignKey(settings.AUTH_USER_MODEL,
-                              on_delete=models.CASCADE,
-                              related_name='tenant_owner')
+    owner = models.ForeignKey(
+        settings.AUTH_USER_MODEL, on_delete=models.CASCADE, related_name="tenant_owner"
+    )
     organization = models.CharField(max_length=64, null=True, blank=True, db_index=True)
+    extra_emails = models.CharField(
+        null=True, blank=True, db_index=True, max_length=256
+    )
 
     def __str__(self):
         return f"[{self.schema_name}] {self.name}"
 
 
 def _authorized_user_str(self):
     return f"{self.user.username}@{self.tenant.name}"
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/oss_utils.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/oss_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 
 from tcms_tenants.forms import NewTenantForm
 from tcms_tenants.utils import create_tenant
 
 
 def create_oss_tenant(owner, name, schema_name, organization):
     """
-        Used to create tenants for our OSS program. Executed by the
-        instance administrator!
+    Used to create tenants for our OSS program. Executed by the
+    instance administrator!
     """
+
     class FakeRequest:  # pylint: disable=too-few-public-methods,nested-class-found
         is_secure = True
         user = None
 
         def __init__(self, username):
             self.user = get_user_model().objects.get(username=username)
 
     request = FakeRequest(owner)
 
-    form = NewTenantForm({
-        'owner': request.user.pk,
-        'name': name,
-        'schema_name': schema_name.lower(),
-        'organization': organization,
-        'publicly_readable': False,
-        'paid_until': datetime.datetime(2999, 12, 31),
-    })
+    form = NewTenantForm(
+        {
+            "owner": request.user.pk,
+            "name": name,
+            "schema_name": schema_name.lower(),
+            "organization": organization,
+            "publicly_readable": False,
+            "paid_until": datetime.datetime(2999, 12, 31),
+        }
+    )
     if form.is_valid():
         return create_tenant(form, request)
 
     raise RuntimeError(list(form.errors.items()))
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/storage.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 from django.core.files.storage import FileSystemStorage
 
 from django_tenants import utils
 
 
 class TenantFileSystemStorage(FileSystemStorage):
     """
-        Implementation that extends core Django's FileSystemStorage for multi-tenant setups,
-        storing files under induvidual directories. Workaround until
-        https://github.com/tomturner/django-tenants/pull/252 gets merged.
+    Implementation that extends core Django's FileSystemStorage for multi-tenant setups,
+    storing files under induvidual directories. Workaround until
+    https://github.com/tomturner/django-tenants/pull/252 gets merged.
     """
+
     @cached_property
     def relative_media_root(self):  # pylint: disable=no-self-use
-        return getattr(settings, 'MULTITENANT_RELATIVE_MEDIA_ROOT', "%s")
+        return getattr(settings, "MULTITENANT_RELATIVE_MEDIA_ROOT", "%s")
 
     @property  # not cached like in parent class
     def base_url(self):  # pylint: disable=invalid-overridden-method
         _url = super().base_url
-        _url = os.path.join(_url,
-                            utils.parse_tenant_config_path(self.relative_media_root))
-        if not _url.endswith('/'):
-            _url += '/'
+        _url = os.path.join(
+            _url, utils.parse_tenant_config_path(self.relative_media_root)
+        )
+        if not _url.endswith("/"):
+            _url += "/"
         return _url
 
     @property  # not cached like in parent class
     def location(self):  # pylint: disable=invalid-overridden-method
-        _location = os.path.join(super().location,
-                                 utils.parse_tenant_config_path(self.relative_media_root))
+        _location = os.path.join(
+            super().location, utils.parse_tenant_config_path(self.relative_media_root)
+        )
         return os.path.abspath(_location)
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/invite_users.html` & `kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/invite_users.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/templates/tcms_tenants/new.html` & `kiwitcms-tenants-2.7.0/tcms_tenants/templates/tcms_tenants/new.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/tests/__init__.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/tests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,43 +39,45 @@
 
     @classmethod
     def setup_tenant(cls, tenant):
         super().setup_tenant(tenant)
 
         tenant.publicly_readable = False
         tenant.owner = UserFactory()
-        tenant.owner.set_password('password')
+        tenant.owner.set_password("password")
         tenant.owner.save()
 
     @classmethod
     def setUpClass(cls):
         # b/c it may create a new tenant
-        with schema_context('public'):
+        with schema_context("public"):
             super().setUpClass()
 
         # authorize tenant owner
         cls.tenant.authorized_users.add(cls.tenant.owner)
 
         cls.tester = UserFactory()
-        cls.tester.set_password('password')
+        cls.tester.set_password("password")
         cls.tester.save()
 
         # authorize this user
         cls.tenant.authorized_users.add(cls.tester)
 
         # initial data
         with tenant_context(cls.tenant):
             cls.test_plan_by_owner = TestPlanFactory(author=cls.tenant.owner)
 
     def setUp(self):
         super().setUp()
 
         self.client = TenantClient(self.tenant)
-        self.client.login(username=self.tester.username,  # nosec:B106:hardcoded_password_funcarg
-                          password='password')
+        self.client.login(
+            username=self.tester.username,  # nosec:B106:hardcoded_password_funcarg
+            password="password",
+        )
 
 
 class TenantGroupsTestCase(LoggedInTestCase):
     original_value = None
 
     @classmethod
     def get_test_schema_name(cls):
@@ -94,15 +96,15 @@
     @classmethod
     def setUpClass(cls):
         # will create the actual schema
         cls.original_value = get_tenant_model().auto_create_schema
         get_tenant_model().auto_create_schema = True
 
         # execute before calling the parent class which will start a DB transaction
-        with schema_context('public'):
+        with schema_context("public"):
             cursor = connection.cursor()
 
             try:
                 cursor.execute("SELECT 'clone_schema'::regproc")
             except ProgrammingError:
                 CloneSchema()._create_clone_schema_function()  # pylint: disable=protected-access
                 transaction.commit()
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc` & `kiwitcms-tenants-2.7.0/tcms_tenants/tests/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/utils.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,63 +49,79 @@
     if not user.is_authenticated:
         return True
 
     return tenant.authorized_users.filter(pk=user.pk).exists()
 
 
 def owns_tenant(user, tenant):
-    return tenant.schema_name != get_public_schema_name() and \
-            tenant.authorized_users.filter(pk=user.pk).exists()
+    return (
+        tenant.schema_name != get_public_schema_name()
+        and tenant.authorized_users.filter(pk=user.pk).exists()
+    )
 
 
 def schema_name_not_used(name):
     if Tenant.objects.filter(schema_name=name).exists():
         raise ValidationError(_("Schema name already in use"))
 
 
 # warning: doesn't play well when the domain has a port number
 def tenant_domain(schema_name):
     # take into account the fact that some customers deploy their 'public' schema
     # without a prefix, e.g. tcms.example.com == KIWI_TENANTS_DOMAIN or could use a
     # different domain for their tenant(s)!
-    domain = Domain.objects.filter(tenant__schema_name=schema_name, is_primary=True).first()
+    domain = Domain.objects.filter(
+        tenant__schema_name=schema_name, is_primary=True
+    ).first()
     if domain:
         return domain.domain
 
     return f"{schema_name}.{settings.KIWI_TENANTS_DOMAIN}"
 
 
 def tenant_url(request, schema_name):
     url = tenant_domain(schema_name)
     if request.is_secure:
-        url = 'https://' + url
+        url = "https://" + url
     else:
-        url = 'http://' + url
+        url = "http://" + url
     return url
 
 
 def create_tenant(form, request):
-    with schema_context('public'):
+    with schema_context("public"):
         # If a schema with name "empty" exists then use it for
         # cloning b/c that's faster
-        if Tenant.objects.filter(schema_name='empty').first():
+        if Tenant.objects.filter(schema_name="empty").first():
             schema_name = form.cleaned_data["schema_name"]
-            paid_until = form.cleaned_data["paid_until"] or datetime.datetime(3000, 3, 31)
+            paid_until = form.cleaned_data["paid_until"] or datetime.datetime(
+                3000, 3, 31
+            )
             call_command(
                 "clone_tenant",
-                "--clone_from", "empty",
-                "--clone_tenant_fields", False,
-                "--schema_name", schema_name,
-                "--name", form.cleaned_data["name"],
-                "--paid_until", paid_until,
-                "--publicly_readable", form.cleaned_data["publicly_readable"],
-                "--owner_id", request.user.pk,
-                "--organization", form.cleaned_data["organization"] or "-",
-                "--domain-domain", tenant_domain(schema_name),
-                "--domain-is_primary", True,
+                "--clone_from",
+                "empty",
+                "--clone_tenant_fields",
+                False,
+                "--schema_name",
+                schema_name,
+                "--name",
+                form.cleaned_data["name"],
+                "--paid_until",
+                paid_until,
+                "--publicly_readable",
+                form.cleaned_data["publicly_readable"],
+                "--owner_id",
+                request.user.pk,
+                "--organization",
+                form.cleaned_data["organization"] or "-",
+                "--domain-domain",
+                tenant_domain(schema_name),
+                "--domain-is_primary",
+                True,
             )
             tenant = Tenant.objects.get(schema_name=schema_name)
             if not form.cleaned_data["paid_until"]:
                 tenant.paid_until = None
                 tenant.save()
 
             if not form.cleaned_data["organization"]:
@@ -141,49 +157,54 @@
         site.save()
 
         # add owner to default groups b/c they need certain permissions
         TenantGroup.objects.get(name="Administrator").user_set.add(tenant.owner)
         TenantGroup.objects.get(name="Tester").user_set.add(tenant.owner)
 
     mailto(
-        template_name='tcms_tenants/email/new.txt',
+        template_name="tcms_tenants/email/new.txt",
         recipients=[tenant.owner.email],
-        subject=str(_('New Kiwi TCMS tenant created')),
+        subject=str(_("New Kiwi TCMS tenant created")),
         context={
-            'tenant_url': tenant_url(request, tenant.schema_name),
-        }
+            "tenant_url": tenant_url(request, tenant.schema_name),
+        },
     )
     return tenant
 
 
 # NOTE: defined here to avoid circular imports with forms.py
-class RegistrationForm(kiwi_auth_forms.RegistrationForm):  # pylint: disable=too-many-ancestors
+class RegistrationForm(
+    kiwi_auth_forms.RegistrationForm
+):  # pylint: disable=too-many-ancestors
     """
-        Override captcha field b/c Kiwi TCMS may be configured to
-        use reCAPTCHA and we don't want this to block automatic
-        creation of user accounts!
+    Override captcha field b/c Kiwi TCMS may be configured to
+    use reCAPTCHA and we don't want this to block automatic
+    creation of user accounts!
     """
+
     captcha = None
 
 
 def create_user_account(email_address):
     desired_username = username = email_address.split("@")[0]
     password = uuid.uuid4().hex
 
     i = 1
     while UserModel.objects.filter(username=username).exists():
         username = f"{desired_username}.{i}"
         i += 1
 
-    form = RegistrationForm(data={
-        "username": username,
-        "password1": password,
-        "password2": password,
-        "email": email_address,
-    })
+    form = RegistrationForm(
+        data={
+            "username": username,
+            "password1": password,
+            "password2": password,
+            "email": email_address,
+        }
+    )
 
     user = form.save()
 
     # activate their account instead of sending them email with activation key
     user.is_active = True
     user.save()
 
@@ -220,15 +241,15 @@
             continue
 
         request.tenant.authorized_users.add(user)
         with tenant_context(request.tenant):
             add_to_default_groups(user)
 
         mailto(
-            template_name='tcms_tenants/email/invite_user.txt',
+            template_name="tcms_tenants/email/invite_user.txt",
             recipients=[user.email],
-            subject=str(_('Invitation to join Kiwi TCMS')),
+            subject=str(_("Invitation to join Kiwi TCMS")),
             context={
                 "invited_by": request.user.get_full_name() or request.user.username,
                 "tenant_url": tenant_url(request, request.tenant.schema_name),
-            }
+            },
         )
```

### Comparing `kiwitcms-tenants-2.6.1/tcms_tenants/views.py` & `kiwitcms-tenants-2.7.0/tcms_tenants/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,54 +19,55 @@
     NewTenantForm,
     UpdateTenantForm,
     VALIDATION_RE,
 )
 from tcms_tenants.models import Tenant
 
 
-@method_decorator(permission_required('tcms_tenants.add_tenant'), name='dispatch')
+@method_decorator(permission_required("tcms_tenants.add_tenant"), name="dispatch")
 class NewTenantView(FormView):
     """
-        Everybody is allowed to create new tenants.
-        Depending on additional configuration they may have to pay
-        for using them!
+    Everybody is allowed to create new tenants.
+    Depending on additional configuration they may have to pay
+    for using them!
     """
+
     form_class = NewTenantForm
 
     def get_template_names(self):
         """
-            Allow downstream installations to override the template. For example
-            to provide a link to SLA or hosting policy! The overriden template
-            can extend the base one if needed.
+        Allow downstream installations to override the template. For example
+        to provide a link to SLA or hosting policy! The overriden template
+        can extend the base one if needed.
         """
-        return ['tcms_tenants/override_new.html', 'tcms_tenants/new.html']
+        return ["tcms_tenants/override_new.html", "tcms_tenants/new.html"]
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['tcms_tenants_domain'] = settings.KIWI_TENANTS_DOMAIN
-        context['validation_pattern'] = VALIDATION_RE.pattern
+        context["tcms_tenants_domain"] = settings.KIWI_TENANTS_DOMAIN
+        context["validation_pattern"] = VALIDATION_RE.pattern
         return context
 
     def get_form_kwargs(self):
         kwargs = super().get_form_kwargs()
         kwargs["initial"]["owner"] = self.request.user.pk
         return kwargs
 
     def form_valid(self, form):
         tenant = utils.create_tenant(form, self.request)
         # all is successfull so redirect to the new tenant
         return HttpResponseRedirect(utils.tenant_url(self.request, tenant.schema_name))
 
 
-@method_decorator(permission_required('tcms_tenants.change_tenant'), name='dispatch')
+@method_decorator(permission_required("tcms_tenants.change_tenant"), name="dispatch")
 class UpdateTenantView(UpdateView):
     model = Tenant
     form_class = UpdateTenantForm
-    template_name = 'tcms_tenants/new.html'
-    success_url = '/'
+    template_name = "tcms_tenants/new.html"
+    success_url = "/"
 
     @staticmethod
     def check_owner(request):
         # super-user can edit all tenants
         if request.user.is_superuser:
             return None
 
@@ -75,82 +76,84 @@
             return None
 
         messages.add_message(
             request,
             messages.ERROR,
             _("Only super-user and tenant owner are allowed to edit tenant properties"),
         )
-        return HttpResponseRedirect('/')
+        return HttpResponseRedirect("/")
 
     def get(self, request, *args, **kwargs):
         return self.check_owner(request) or super().get(request, *args, **kwargs)
 
     def post(self, request, *args, **kwargs):
         return self.check_owner(request) or super().post(request, *args, **kwargs)
 
     def get_object(self, queryset=None):
         return self.request.tenant
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['tcms_tenants_domain'] = settings.KIWI_TENANTS_DOMAIN
-        context['validation_pattern'] = VALIDATION_RE.pattern
-        context['form_action_url'] = reverse('tcms_tenants:edit-tenant')
-        context['page_title'] = _('Edit tenant')
+        context["tcms_tenants_domain"] = settings.KIWI_TENANTS_DOMAIN
+        context["validation_pattern"] = VALIDATION_RE.pattern
+        context["form_action_url"] = reverse("tcms_tenants:edit-tenant")
+        context["page_title"] = _("Edit tenant")
         return context
 
 
-@method_decorator(login_required, name='dispatch')
+@method_decorator(login_required, name="dispatch")
 class RedirectTo(RedirectView):  # pylint: disable=missing-permission-required
     """
-        Will redirect to tenant.domain.domain/path!
+    Will redirect to tenant.domain.domain/path!
 
-        Used together with GitHub logins and the ``tenant_url``
-        template tag!
+    Used together with GitHub logins and the ``tenant_url``
+    template tag!
 
-        When trying to do GitHub login on a tenant sub-domain
-        the HTML href will actually point to
+    When trying to do GitHub login on a tenant sub-domain
+    the HTML href will actually point to
 
-        https://public.tenants.localdomain/login/github?next=/tenants/go/to/tenant/path
+    https://public.tenants.localdomain/login/github?next=/tenants/go/to/tenant/path
 
-        instead of
+    instead of
 
-        http://tenant.tenants.localdomain/login/github?next=path
+    http://tenant.tenants.localdomain/login/github?next=path
 
-        This is to prevent redirect_uri mismatch errors!
+    This is to prevent redirect_uri mismatch errors!
     """
+
     def get_redirect_url(self, *args, **kwargs):
-        tenant = kwargs['tenant']
-        path = kwargs['path']
+        tenant = kwargs["tenant"]
+        path = kwargs["path"]
         tenant_url = utils.tenant_url(self.request, tenant)
         return f"{tenant_url}/{path}"
 
 
-@method_decorator(login_required, name='dispatch')
+@method_decorator(login_required, name="dispatch")
 class InviteUsers(FormView):  # pylint: disable=missing-permission-required
     """
-        Invite users to tenant via email.
+    Invite users to tenant via email.
 
-        .. important::
+    .. important::
 
-            Anyone who is authorized for this tenant can invite others
-            in the same way they can add them directly via the `Authorized users`
-            menu!
+        Anyone who is authorized for this tenant can invite others
+        in the same way they can add them directly via the `Authorized users`
+        menu!
     """
+
     form_class = InviteUsersForm
     template_name = "tcms_tenants/invite_users.html"
 
     def get(self, request, *args, **kwargs):
         if not utils.owns_tenant(request.user, request.tenant):
             messages.add_message(
                 request,
                 messages.ERROR,
                 _("Only users who are authorized for this tenant can invite others"),
             )
-            return HttpResponseRedirect('/')
+            return HttpResponseRedirect("/")
 
         return super().get(self, request, *args, **kwargs)
 
     def form_valid(self, form):
         utils.invite_users(self.request, form.cleaned_data["emails"])
 
-        return HttpResponseRedirect('/')
+        return HttpResponseRedirect("/")
```

### Comparing `kiwitcms-tenants-2.6.1/tenant_groups/admin.py` & `kiwitcms-tenants-2.7.0/tenant_groups/admin.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-tenants-2.6.1/tenant_groups/backends.py` & `kiwitcms-tenants-2.7.0/tenant_groups/backends.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
     Backend which returns group permissions configured per-tenant but keeps
     individual user permissions!
 
     NOTE: Individually assigned permissions have higher priority
     (are valid across tenants) compared to group permissions.
     """
+
     public_schema_name = get_public_schema_name()
 
     @property
     def tenant(self):
         return get_current_tenant()
 
     def get_group_permissions(self, user_obj, obj=None):
@@ -26,15 +27,14 @@
         # django.contrib.auth.models.Group
         if self.tenant.schema_name == self.public_schema_name:
             return super().get_group_permissions(user_obj, obj)
 
         # permissions configured per-tenant via
         # tenant_groups.models.Group
         with tenant_context(self.tenant):
-            permissions = Permission.objects.filter(
-                tenant_groups__user_set__in=[user_obj]
-            ).values_list(
-                'content_type__app_label',
-                'codename'
-            ).order_by()
+            permissions = (
+                Permission.objects.filter(tenant_groups__user_set__in=[user_obj])
+                .values_list("content_type__app_label", "codename")
+                .order_by()
+            )
 
             return {f"{ct}.{name}" for ct, name in permissions}
```

### Comparing `kiwitcms-tenants-2.6.1/tenant_groups/checks.py` & `kiwitcms-tenants-2.7.0/tenant_groups/checks.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 
 def tenant_groups_backend(app_configs, **kwargs):  # pylint: disable=unused-argument
     errors = []
     if "tenant_groups.backends.GroupsBackend" not in settings.AUTHENTICATION_BACKENDS:
         errors.append(
             checks.Error(
-                msg='tenant_groups.backends.GroupsBackend '
-                    'is not pesent in AUTHENTICATION_BACKENDS!',
-                hint=('See '
-                      'https://kiwitcms.readthedocs.io/en/latest/admin.html#tenant-groups'),
+                msg="tenant_groups.backends.GroupsBackend "
+                "is not pesent in AUTHENTICATION_BACKENDS!",
+                hint=(
+                    "See "
+                    "https://kiwitcms.readthedocs.io/en/latest/admin.html#tenant-groups"
+                ),
             )
         )
     return errors
```

### Comparing `kiwitcms-tenants-2.6.1/tenant_groups/management/commands/refresh_tenant_permissions.py` & `kiwitcms-tenants-2.7.0/tenant_groups/management/commands/refresh_tenant_permissions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 # Copyright (c) 2022 Alexander Todorov <atodorov@otb.bg>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
-from django_tenants.utils import get_public_schema_name, get_tenant_model, tenant_context
+from django_tenants.utils import (
+    get_public_schema_name,
+    get_tenant_model,
+    tenant_context,
+)
 from tcms.core.management.commands import refresh_permissions
 
 from tenant_groups.models import Group as TenantGroup
 
 
 class Command(refresh_permissions.Command):
     help = "Refresh permissions for tenant groups 'Admin' & 'Tester'."
 
     group_model = TenantGroup
     admin_permissions_filter = {
-        'content_type__app_label__in': TenantGroup.relevant_apps,
+        "content_type__app_label__in": TenantGroup.relevant_apps,
     }
     tester_permissions_filter = {
-        'content_type__app_label__in': TenantGroup.relevant_apps,
+        "content_type__app_label__in": TenantGroup.relevant_apps,
     }
 
     def handle(self, *args, **kwargs):
         for tenant in get_tenant_model().objects.exclude(
             schema_name=get_public_schema_name(),
         ):
             output = None
             if kwargs["verbosity"]:
                 output = self.stdout
 
             with tenant_context(tenant):
                 if output:
                     output.write(
-                        f"\n\n === Refreshing permissions for tenant '{tenant.schema_name}' ===")
+                        f"\n\n === Refreshing permissions for tenant '{tenant.schema_name}' ==="
+                    )
 
                 self.execute_commands(*args, **kwargs)
 
                 if output:
                     output.write(
                         f"\n\n === End refreshing permissions for tenant '{tenant.schema_name}' ==="
                     )
```

### Comparing `kiwitcms-tenants-2.6.1/tenant_groups/migrations/0001_initial.py` & `kiwitcms-tenants-2.7.0/tenant_groups/migrations/0001_initial.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,17 +47,15 @@
         )
         tester.permissions.add(*app_perms)
 
     # Admin gets the same permissions as Tester + tenant_groups
     admin = group_model.objects.get(name="Administrator")
     admin.permissions.add(*tester.permissions.all())
     admin.permissions.add(
-        *permission_model.objects.filter(
-            content_type__app_label="tenant_groups"
-        )
+        *permission_model.objects.filter(content_type__app_label="tenant_groups")
     )
 
 
 def forwards_add_authorized_users_to_default_groups(apps, schema_editor):
     current_tenant = connections[get_tenant_database_alias()].tenant
     if current_tenant.schema_name in [get_public_schema_name(), "empty"]:
         return
@@ -78,36 +76,54 @@
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ('auth', '0012_alter_user_first_name_max_length'),
-        ('tcms_tenants', '0005_rename_on_trial_to_public_read'),
+        ("auth", "0012_alter_user_first_name_max_length"),
+        ("tcms_tenants", "0005_rename_on_trial_to_public_read"),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='Group',
+            name="Group",
             fields=[
-                ('id', models.AutoField(
-                                auto_created=True, primary_key=True,
-                                serialize=False, verbose_name='ID')),
-                ('name', models.CharField(max_length=150, unique=True, verbose_name='name')),
-                ('permissions', models.ManyToManyField(
-                                    blank=True, related_name='tenant_groups',
-                                    to='auth.Permission', verbose_name='permissions')),
-                ('user_set', models.ManyToManyField(
-                                to=settings.AUTH_USER_MODEL,
-                                related_name='tenant_groups')),
+                (
+                    "id",
+                    models.AutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                (
+                    "name",
+                    models.CharField(max_length=150, unique=True, verbose_name="name"),
+                ),
+                (
+                    "permissions",
+                    models.ManyToManyField(
+                        blank=True,
+                        related_name="tenant_groups",
+                        to="auth.Permission",
+                        verbose_name="permissions",
+                    ),
+                ),
+                (
+                    "user_set",
+                    models.ManyToManyField(
+                        to=settings.AUTH_USER_MODEL, related_name="tenant_groups"
+                    ),
+                ),
             ],
             options={
-                'verbose_name': 'group',
-                'verbose_name_plural': 'groups',
+                "verbose_name": "group",
+                "verbose_name_plural": "groups",
             },
         ),
         migrations.RunPython(
             code=forwards_add_default_groups_and_permissions,
             reverse_code=migrations.RunPython.noop,
         ),
         migrations.RunPython(
```

### Comparing `kiwitcms-tenants-2.6.1/tenant_groups/models.py` & `kiwitcms-tenants-2.7.0/tenant_groups/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,39 +12,42 @@
     """
     Per-tenant group definition! See
     https://github.com/kiwitcms/tenants/issues/104#issuecomment-949956789
 
     Note: essentially copy-pasted from django.contrib.auth b/c we need separate
     records inside tenant's schema.
     """
+
     relevant_apps = [
         "attachments",
         "bugs",
         "django_comments",
         "linkreference",
         "management",
         "testcases",
         "testplans",
         "testruns",
         "tenant_groups",
         "trackers_integration",
     ]
 
-    name = models.CharField(_('name'), max_length=150, unique=True)
+    name = models.CharField(_("name"), max_length=150, unique=True)
     permissions = models.ManyToManyField(
         Permission,
-        verbose_name=_('permissions'),
+        verbose_name=_("permissions"),
         blank=True,
         related_name="tenant_groups",
     )
 
-    user_set = models.ManyToManyField(to=settings.AUTH_USER_MODEL, related_name='tenant_groups')
+    user_set = models.ManyToManyField(
+        to=settings.AUTH_USER_MODEL, related_name="tenant_groups"
+    )
 
     class Meta:
-        verbose_name = _('group')
-        verbose_name_plural = _('groups')
+        verbose_name = _("group")
+        verbose_name_plural = _("groups")
 
     def __str__(self):
         return self.name
 
     def natural_key(self):
         return (self.name,)
```

