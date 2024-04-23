# Comparing `tmp/lino-amici-24.3.1.tar.gz` & `tmp/lino-amici-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-amici-24.3.1.tar", last modified: Mon Mar 25 09:12:08 2024, max compression
+gzip compressed data, was "lino-amici-24.4.0.tar", last modified: Tue Apr 23 12:45:49 2024, max compression
```

## Comparing `lino-amici-24.3.1.tar` & `lino-amici-24.4.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.946657 lino-amici-24.3.1/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:28.000000 lino-amici-24.3.1/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      190 2022-10-19 14:04:22.000000 lino-amici-24.3.1/MANIFEST.in
--rw-r--r--   0 luc       (1000) www-data    (33)     1568 2024-03-25 09:12:08.942657 lino-amici-24.3.1/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      674 2024-02-22 07:31:03.000000 lino-amici-24.3.1/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.938657 lino-amici-24.3.1/lino_amici/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      464 2021-04-25 16:07:31.000000 lino-amici-24.3.1/lino_amici/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.938657 lino-amici-24.3.1/lino_amici/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      242 2021-04-07 10:22:53.000000 lino-amici-24.3.1/lino_amici/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.938657 lino-amici-24.3.1/lino_amici/lib/amici/
--rw-rw-r--   0 luc       (1000) www-data    (33)      307 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/amici/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      544 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/amici/custom_layouts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      769 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/amici/help_texts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.934657 lino-amici-24.3.1/lino_amici/lib/amici/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.934657 lino-amici-24.3.1/lino_amici/lib/amici/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.938657 lino-amici-24.3.1/lino_amici/lib/amici/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-amici-24.3.1/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    14175 2019-03-29 11:27:30.000000 lino-amici-24.3.1/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.934657 lino-amici-24.3.1/lino_amici/lib/amici/locale/et/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.938657 lino-amici-24.3.1/lino_amici/lib/amici/locale/et/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-amici-24.3.1/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13385 2019-03-29 11:27:31.000000 lino-amici-24.3.1/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.934657 lino-amici-24.3.1/lino_amici/lib/amici/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.938657 lino-amici-24.3.1/lino_amici/lib/amici/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-amici-24.3.1/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13352 2019-03-29 11:27:30.000000 lino-amici-24.3.1/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-06-12 03:05:36.000000 lino-amici-24.3.1/lino_amici/lib/amici/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     4952 2024-03-25 09:02:16.000000 lino-amici-24.3.1/lino_amici/lib/amici/settings.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     2382 2024-03-25 07:48:12.000000 lino-amici-24.3.1/lino_amici/lib/amici/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      915 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/amici/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.938657 lino-amici-24.3.1/lino_amici/lib/cal/
--rw-rw-r--   0 luc       (1000) www-data    (33)      305 2023-09-01 13:27:30.000000 lino-amici-24.3.1/lino_amici/lib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/lib/cal/fixtures/
--rw-rw-r--   0 luc       (1000) www-data    (33)       50 2023-11-12 11:43:07.000000 lino-amici-24.3.1/lino_amici/lib/cal/fixtures/demo.py
--rw-rw-r--   0 luc       (1000) www-data    (33)       51 2023-11-12 11:43:14.000000 lino-amici-24.3.1/lino_amici/lib/cal/fixtures/demo2.py
--rw-rw-r--   0 luc       (1000) www-data    (33)       49 2023-11-12 11:42:58.000000 lino-amici-24.3.1/lino_amici/lib/cal/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      693 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/lib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      318 2023-03-25 08:39:35.000000 lino-amici-24.3.1/lino_amici/lib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/lib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-30 02:04:04.000000 lino-amici-24.3.1/lino_amici/lib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2017-04-30 02:04:26.000000 lino-amici-24.3.1/lino_amici/lib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       54 2017-05-03 12:11:20.000000 lino-amici-24.3.1/lino_amici/lib/contacts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6555 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/lib/households/
--rw-rw-rw-   0 luc       (1000) www-data    (33)       42 2020-12-24 02:38:08.000000 lino-amici-24.3.1/lino_amici/lib/households/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/lib/households/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2020-12-29 13:26:01.000000 lino-amici-24.3.1/lino_amici/lib/households/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       57 2020-12-24 02:41:05.000000 lino-amici-24.3.1/lino_amici/lib/households/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2020-12-24 02:38:56.000000 lino-amici-24.3.1/lino_amici/lib/households/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      576 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/households/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      271 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-amici-24.3.1/lino_amici/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:52.000000 lino-amici-24.3.1/lino_amici/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       47 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:53.000000 lino-amici-24.3.1/lino_amici/lib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      199 2023-12-09 04:17:34.000000 lino-amici-24.3.1/lino_amici/lib/users/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      902 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/lib/users/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/projects/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-05-05 02:54:41.000000 lino-amici-24.3.1/lino_amici/projects/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/projects/amici1/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      229 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/projects/amici1/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      277 2023-01-10 07:35:25.000000 lino-amici-24.3.1/lino_amici/projects/amici1/manage.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/projects/amici1/settings/
--rw-rw-r--   0 luc       (1000) www-data    (33)     1168 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/projects/amici1/settings/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1004 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/projects/amici1/settings/demo.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/projects/amici1/settings/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-03-26 04:42:38.000000 lino-amici-24.3.1/lino_amici/projects/amici1/settings/fixtures/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      945 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/projects/amici1/settings/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       86 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/projects/amici1/settings/memory.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      824 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/projects/amici1/show_birthdays.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici/projects/amici1/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-11-17 06:49:05.000000 lino-amici-24.3.1/lino_amici/projects/amici1/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2577 2024-02-14 17:36:57.000000 lino-amici-24.3.1/lino_amici/projects/amici1/tests/test_insert_person.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     2879 2024-03-25 09:11:46.000000 lino-amici-24.3.1/lino_amici/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/lino_amici.egg-info/
--rw-r--r--   0 luc       (1000) www-data    (33)     1568 2024-03-25 09:12:08.000000 lino-amici-24.3.1/lino_amici.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2326 2024-03-25 09:12:08.000000 lino-amici-24.3.1/lino_amici.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-03-25 09:12:08.000000 lino-amici-24.3.1/lino_amici.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2017-05-03 11:30:38.000000 lino-amici-24.3.1/lino_amici.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       16 2024-03-25 09:12:08.000000 lino-amici-24.3.1/lino_amici.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2024-03-25 09:12:08.000000 lino-amici-24.3.1/lino_amici.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-12-03 20:13:34.000000 lino-amici-24.3.1/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-03-25 09:12:08.946657 lino-amici-24.3.1/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      182 2024-02-14 17:36:57.000000 lino-amici-24.3.1/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      541 2024-02-14 17:36:57.000000 lino-amici-24.3.1/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:12:08.942657 lino-amici-24.3.1/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-02 05:37:16.000000 lino-amici-24.3.1/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      113 2021-03-30 02:28:55.000000 lino-amici-24.3.1/tests/import_test.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      272 2021-02-15 13:04:51.000000 lino-amici-24.3.1/tests/test_demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:36:57.000000 lino-amici-24.3.1/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      418 2024-02-14 17:36:57.000000 lino-amici-24.3.1/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.245574 lino-amici-24.4.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:56:28.000000 lino-amici-24.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      190 2022-10-19 14:04:22.000000 lino-amici-24.4.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     1568 2024-04-23 12:45:49.241574 lino-amici-24.4.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      674 2024-02-22 07:31:03.000000 lino-amici-24.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      464 2021-04-25 16:07:31.000000 lino-amici-24.4.0/lino_amici/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      242 2021-04-07 10:22:53.000000 lino-amici-24.4.0/lino_amici/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/lib/amici/
+-rw-rw-r--   0 luc       (1000) www-data    (33)      307 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/amici/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      544 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/amici/custom_layouts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      769 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/amici/help_texts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/lib/amici/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/lib/amici/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-amici-24.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    14175 2019-03-29 11:27:30.000000 lino-amici-24.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/lib/amici/locale/et/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-amici-24.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13385 2019-03-29 11:27:31.000000 lino-amici-24.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.237574 lino-amici-24.4.0/lino_amici/lib/amici/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-amici-24.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13352 2019-03-29 11:27:30.000000 lino-amici-24.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2021-06-12 03:05:36.000000 lino-amici-24.4.0/lino_amici/lib/amici/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     4958 2024-03-27 08:42:23.000000 lino-amici-24.4.0/lino_amici/lib/amici/settings.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2382 2024-03-25 07:48:12.000000 lino-amici-24.4.0/lino_amici/lib/amici/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      915 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/amici/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/cal/
+-rw-rw-r--   0 luc       (1000) www-data    (33)      305 2023-09-01 13:27:30.000000 lino-amici-24.4.0/lino_amici/lib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/cal/fixtures/
+-rw-rw-r--   0 luc       (1000) www-data    (33)       50 2023-11-12 11:43:07.000000 lino-amici-24.4.0/lino_amici/lib/cal/fixtures/demo.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)       51 2023-11-12 11:43:14.000000 lino-amici-24.4.0/lino_amici/lib/cal/fixtures/demo2.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)       49 2023-11-12 11:42:58.000000 lino-amici-24.4.0/lino_amici/lib/cal/fixtures/std.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      693 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      318 2023-03-25 08:39:35.000000 lino-amici-24.4.0/lino_amici/lib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-30 02:04:04.000000 lino-amici-24.4.0/lino_amici/lib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2017-04-30 02:04:26.000000 lino-amici-24.4.0/lino_amici/lib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       54 2017-05-03 12:11:20.000000 lino-amici-24.4.0/lino_amici/lib/contacts/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6555 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/households/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       42 2020-12-24 02:38:08.000000 lino-amici-24.4.0/lino_amici/lib/households/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/households/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2020-12-29 13:26:01.000000 lino-amici-24.4.0/lino_amici/lib/households/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       57 2020-12-24 02:41:05.000000 lino-amici-24.4.0/lino_amici/lib/households/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       56 2020-12-24 02:38:56.000000 lino-amici-24.4.0/lino_amici/lib/households/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      576 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/households/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      271 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/lib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-amici-24.4.0/lino_amici/lib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:52.000000 lino-amici-24.4.0/lino_amici/lib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       47 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:53.000000 lino-amici-24.4.0/lino_amici/lib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      199 2023-12-09 04:17:34.000000 lino-amici-24.4.0/lino_amici/lib/users/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      902 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/lib/users/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/projects/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-05-05 02:54:41.000000 lino-amici-24.4.0/lino_amici/projects/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/projects/amici1/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      229 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/projects/amici1/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      277 2023-01-10 07:35:25.000000 lino-amici-24.4.0/lino_amici/projects/amici1/manage.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/projects/amici1/settings/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1174 2024-03-27 08:42:23.000000 lino-amici-24.4.0/lino_amici/projects/amici1/settings/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1004 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/projects/amici1/settings/demo.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/projects/amici1/settings/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-03-26 04:42:38.000000 lino-amici-24.4.0/lino_amici/projects/amici1/settings/fixtures/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      937 2024-04-22 19:14:22.000000 lino-amici-24.4.0/lino_amici/projects/amici1/settings/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       86 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/projects/amici1/settings/memory.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      824 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/projects/amici1/show_birthdays.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici/projects/amici1/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-11-17 06:49:05.000000 lino-amici-24.4.0/lino_amici/projects/amici1/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2577 2024-02-14 17:36:57.000000 lino-amici-24.4.0/lino_amici/projects/amici1/tests/test_insert_person.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2879 2024-04-23 12:45:38.000000 lino-amici-24.4.0/lino_amici/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/lino_amici.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     1568 2024-04-23 12:45:49.000000 lino-amici-24.4.0/lino_amici.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2326 2024-04-23 12:45:49.000000 lino-amici-24.4.0/lino_amici.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-04-23 12:45:49.000000 lino-amici-24.4.0/lino_amici.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2017-05-03 11:30:38.000000 lino-amici-24.4.0/lino_amici.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       16 2024-04-23 12:45:49.000000 lino-amici-24.4.0/lino_amici.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2024-04-23 12:45:49.000000 lino-amici-24.4.0/lino_amici.egg-info/top_level.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2022-12-03 20:13:34.000000 lino-amici-24.4.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-04-23 12:45:49.245574 lino-amici-24.4.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      182 2024-02-14 17:36:57.000000 lino-amici-24.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      541 2024-02-14 17:36:57.000000 lino-amici-24.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:45:49.241574 lino-amici-24.4.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-02 05:37:16.000000 lino-amici-24.4.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      113 2021-03-30 02:28:55.000000 lino-amici-24.4.0/tests/import_test.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      272 2021-02-15 13:04:51.000000 lino-amici-24.4.0/tests/test_demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:36:57.000000 lino-amici-24.4.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      418 2024-02-14 17:36:57.000000 lino-amici-24.4.0/tests/test_packages.py
```

### Comparing `lino-amici-24.3.1/COPYING` & `lino-amici-24.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/PKG-INFO` & `lino-amici-24.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-amici
-Version: 24.3.1
+Version: 24.4.0
 Summary: Manage your family contacts
 Home-page: https://gitlab.com/lino-framework/amici
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lino-amici-24.3.1/README.rst` & `lino-amici-24.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/custom_layouts.py` & `lino-amici-24.4.0/lino_amici/lib/amici/custom_layouts.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/help_texts.py` & `lino-amici-24.4.0/lino_amici/lib/amici/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo` & `lino-amici-24.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po` & `lino-amici-24.4.0/lino_amici/lib/amici/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo` & `lino-amici-24.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po` & `lino-amici-24.4.0/lino_amici/lib/amici/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po` & `lino-amici-24.4.0/lino_amici/lib/amici/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/settings.py` & `lino-amici-24.4.0/lino_amici/lib/amici/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     default_build_method = 'weasy2pdf'
     default_ui = 'lino_react.react'
 
     # migration_class = 'lino_amici.lib.amici.migrate.Migrator'
 
     auto_configure_logger_names = "lino lino_xl lino_amici"
 
-    def get_installed_apps(self):
-        yield super(Site, self).get_installed_apps()
+    def get_installed_plugins(self):
+        yield super(Site, self).get_installed_plugins()
         # yield 'lino.modlib.extjs'
         # yield 'lino.modlib.bootstrap3'
         # yield 'lino.modlib.gfks'
         # yield 'lino.modlib.system'
         # yield 'lino.modlib.users'
         yield 'lino.modlib.help'
         yield 'lino_amici.lib.users'
```

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/user_types.py` & `lino-amici-24.4.0/lino_amici/lib/amici/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/amici/workflows.py` & `lino-amici-24.4.0/lino_amici/lib/amici/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/cal/models.py` & `lino-amici-24.4.0/lino_amici/lib/cal/models.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/contacts/models.py` & `lino-amici-24.4.0/lino_amici/lib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/households/models.py` & `lino-amici-24.4.0/lino_amici/lib/households/models.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/lib/users/ui.py` & `lino-amici-24.4.0/lino_amici/lib/users/ui.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/projects/amici1/settings/__init__.py` & `lino-amici-24.4.0/lino_amici/projects/amici1/settings/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,10 +35,10 @@
                 languages='et en de fr',
                 dbf_table_ext='.FOX',
                 use_dbf_py=True,
                 siteconfig_accounts={},
                 timloader_module='lino_xl.lib.tim2lino.timloader_herman')
             self.plugins.checkdata.configure(responsible_user='tim')
 
-        def get_installed_apps(self):
-            yield super().get_installed_apps()
+        def get_installed_plugins(self):
+            yield super().get_installed_plugins()
             yield 'lino_xl.lib.tim2lino'
```

### Comparing `lino-amici-24.3.1/lino_amici/projects/amici1/settings/demo.py` & `lino-amici-24.4.0/lino_amici/projects/amici1/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/projects/amici1/settings/fixtures/demo.py` & `lino-amici-24.4.0/lino_amici/projects/amici1/settings/fixtures/demo.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     training = named(EventType, _("Training"))
     yield training
     workshop = named(EventType, _("Travel"))
     yield workshop
     camp = named(EventType, _("Camp"))
     yield camp
 
-    nature = named(Topic, _("Nature"))
+    nature = Topic(name=_("Nature"))
     yield nature
-    folk = named(Topic, _("Folk"))
+    folk = Topic(name=_("Folk"))
     yield folk
-    health = named(Topic, _("Health"))
+    health = Topic(name=_("Health"))
     yield health
-    comp = named(Topic, _("Computer"))
+    comp = Topic(name=_("Computer"))
     yield comp
```

### Comparing `lino-amici-24.3.1/lino_amici/projects/amici1/show_birthdays.py` & `lino-amici-24.4.0/lino_amici/projects/amici1/show_birthdays.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/projects/amici1/tests/test_insert_person.py` & `lino-amici-24.4.0/lino_amici/projects/amici1/tests/test_insert_person.py`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/lino_amici/setup_info.py` & `lino-amici-24.4.0/lino_amici/setup_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright 2017-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 # $ python setup.py test -s tests.test_packages
 
 SETUP_INFO = dict(
     name='lino-amici',
-    version='24.3.1',
+    version='24.4.0',
     install_requires=['lino-xl', 'vobject'],
 
     # tests_require=['pytest', 'mock'],
     test_suite='tests',
     description=("Manage your family contacts"),
     long_description="""\
```

### Comparing `lino-amici-24.3.1/lino_amici.egg-info/PKG-INFO` & `lino-amici-24.4.0/lino_amici.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-amici
-Version: 24.3.1
+Version: 24.4.0
 Summary: Manage your family contacts
 Home-page: https://gitlab.com/lino-framework/amici
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
```

### Comparing `lino-amici-24.3.1/lino_amici.egg-info/SOURCES.txt` & `lino-amici-24.4.0/lino_amici.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lino-amici-24.3.1/tasks.py` & `lino-amici-24.4.0/tasks.py`

 * *Files identical despite different names*

