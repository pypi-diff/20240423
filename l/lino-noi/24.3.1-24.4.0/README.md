# Comparing `tmp/lino-noi-24.3.1.tar.gz` & `tmp/lino-noi-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-noi-24.3.1.tar", last modified: Mon Mar 25 09:13:59 2024, max compression
+gzip compressed data, was "lino-noi-24.4.0.tar", last modified: Tue Apr 23 12:43:46 2024, max compression
```

## Comparing `lino-noi-24.3.1.tar` & `lino-noi-24.4.0.tar`

### file list

```diff
@@ -1,120 +1,117 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/.idea/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-24.3.1/.idea/encodings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1839 2015-09-19 04:08:02.000000 lino-noi-24.3.1/.idea/misc.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2015-09-19 04:08:02.000000 lino-noi-24.3.1/.idea/modules.xml
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/.idea/scopes/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      139 2015-09-19 04:08:02.000000 lino-noi-24.3.1/.idea/scopes/scope_settings.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-24.3.1/.idea/vcs.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2202 2015-09-19 04:08:02.000000 lino-noi-24.3.1/.idea/workspace.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:54:16.000000 lino-noi-24.3.1/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      109 2016-08-14 01:22:00.000000 lino-noi-24.3.1/MANIFEST.in
--rw-r--r--   0 luc       (1000) www-data    (33)     1504 2024-03-25 09:13:59.334345 lino-noi-24.3.1/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-03-29 14:44:08.000000 lino-noi-24.3.1/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2022-08-17 01:06:46.000000 lino-noi-24.3.1/lino_noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-noi-24.3.1/lino_noi/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/cal/
--rw-rw-r--   0 luc       (1000) www-data    (33)      342 2024-01-27 12:43:19.000000 lino-noi-24.3.1/lino_noi/lib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-04 14:35:11.000000 lino-noi-24.3.1/lino_noi/lib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2017-04-04 14:35:11.000000 lino-noi-24.3.1/lino_noi/lib/cal/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3552 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      274 2021-04-07 10:22:54.000000 lino-noi-24.3.1/lino_noi/lib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      244 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2020-04-04 06:56:19.000000 lino-noi-24.3.1/lino_noi/lib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-05-26 22:13:00.000000 lino-noi-24.3.1/lino_noi/lib/contacts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3226 2024-02-14 17:21:06.000000 lino-noi-24.3.1/lino_noi/lib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/courses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      813 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/courses/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      719 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/courses/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2553 2024-03-24 06:38:16.000000 lino-noi-24.3.1/lino_noi/lib/courses/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/groups/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      320 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/groups/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1363 2024-03-24 15:32:39.000000 lino-noi-24.3.1/lino_noi/lib/groups/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      328 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/noi/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/noi/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:02.000000 lino-noi-24.3.1/lino_noi/lib/noi/fixtures/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    20370 2024-03-24 12:31:43.000000 lino-noi-24.3.1/lino_noi/lib/noi/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6601 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/noi/fixtures/linotickets.py
--rw-rw-r--   0 luc       (1000) www-data    (33)      198 2024-01-27 15:28:56.000000 lino-noi-24.3.1/lino_noi/lib/noi/fixtures/minimal_ledger.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2153 2024-03-24 17:19:41.000000 lino-noi-24.3.1/lino_noi/lib/noi/help_texts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      545 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/noi/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.326345 lino-noi-24.3.1/lino_noi/lib/noi/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.326345 lino-noi-24.3.1/lino_noi/lib/noi/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.330345 lino-noi-24.3.1/lino_noi/lib/noi/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-noi-24.3.1/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    14514 2019-03-29 11:25:54.000000 lino-noi-24.3.1/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.326345 lino-noi-24.3.1/lino_noi/lib/noi/locale/et/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/noi/locale/et/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-noi-24.3.1/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13858 2019-03-29 11:25:55.000000 lino-noi-24.3.1/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.326345 lino-noi-24.3.1/lino_noi/lib/noi/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-noi-24.3.1/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13846 2019-03-29 11:25:54.000000 lino-noi-24.3.1/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)    22981 2024-02-14 17:21:06.000000 lino-noi-24.3.1/lino_noi/lib/noi/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1128 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/noi/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     6343 2024-03-24 14:38:39.000000 lino-noi-24.3.1/lino_noi/lib/noi/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3219 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/noi/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      383 2023-05-12 19:27:14.000000 lino-noi-24.3.1/lino_noi/lib/noi/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/products/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      301 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/products/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      974 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/products/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/public/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1139 2024-02-14 17:21:06.000000 lino-noi-24.3.1/lino_noi/lib/public/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.326345 lino-noi-24.3.1/lino_noi/lib/public/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/public/config/noi/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2019-11-25 17:29:52.000000 lino-noi-24.3.1/lino_noi/lib/public/config/noi/index.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      720 2022-09-01 18:33:50.000000 lino-noi-24.3.1/lino_noi/lib/public/config/noi/tickets.Ticket.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      581 2024-02-14 17:21:06.000000 lino-noi-24.3.1/lino_noi/lib/public/renderer.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1561 2024-02-14 17:21:06.000000 lino-noi-24.3.1/lino_noi/lib/public/views.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/sales/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      309 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/sales/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.326345 lino-noi-24.3.1/lino_noi/lib/sales/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.326345 lino-noi-24.3.1/lino_noi/lib/sales/config/sales/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/sales/config/sales/VatProductInvoice/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1413 2023-02-15 06:31:52.000000 lino-noi-24.3.1/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/sales/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-05-09 16:04:58.000000 lino-noi-24.3.1/lino_noi/lib/sales/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2017-02-26 08:07:55.000000 lino-noi-24.3.1/lino_noi/lib/sales/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      984 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/sales/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/subscriptions/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2023-01-06 20:30:18.000000 lino-noi-24.3.1/lino_noi/lib/subscriptions/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      401 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/subscriptions/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/tickets/
--rw-rw-r--   0 luc       (1000) www-data    (33)     1728 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/tickets/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    15274 2024-03-24 14:26:30.000000 lino-noi-24.3.1/lino_noi/lib/tickets/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3967 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/tickets/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/topics/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      213 2021-04-07 10:22:54.000000 lino-noi-24.3.1/lino_noi/lib/topics/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      622 2021-04-07 10:22:54.000000 lino-noi-24.3.1/lino_noi/lib/topics/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)       37 2023-03-06 06:43:39.000000 lino-noi-24.3.1/lino_noi/lib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi/lib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:00.000000 lino-noi-24.3.1/lino_noi/lib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:49.000000 lino-noi-24.3.1/lino_noi/lib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       47 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:50.000000 lino-noi-24.3.1/lino_noi/lib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      247 2024-02-14 17:21:05.000000 lino-noi-24.3.1/lino_noi/lib/users/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1709 2024-02-14 17:21:06.000000 lino-noi-24.3.1/lino_noi/lib/users/ui.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     3067 2024-03-25 09:13:46.000000 lino-noi-24.3.1/lino_noi/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/lino_noi.egg-info/
--rw-r--r--   0 luc       (1000) www-data    (33)     1504 2024-03-25 09:13:59.000000 lino-noi-24.3.1/lino_noi.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2585 2024-03-25 09:13:59.000000 lino-noi-24.3.1/lino_noi.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-03-25 09:13:59.000000 lino-noi-24.3.1/lino_noi.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-08-31 16:13:18.000000 lino-noi-24.3.1/lino_noi.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2024-03-25 09:13:59.000000 lino-noi-24.3.1/lino_noi.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2024-03-25 09:13:59.000000 lino-noi-24.3.1/lino_noi.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)      328 2023-12-03 03:21:00.000000 lino-noi-24.3.1/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-03-25 09:13:59.334345 lino-noi-24.3.1/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:21:05.000000 lino-noi-24.3.1/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      492 2024-02-14 17:21:05.000000 lino-noi-24.3.1/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-03-25 09:13:59.334345 lino-noi-24.3.1/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-18 18:50:53.000000 lino-noi-24.3.1/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:21:06.000000 lino-noi-24.3.1/tests/test_docs.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      187 2024-02-14 17:21:06.000000 lino-noi-24.3.1/tests/test_packages.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.838096 lino-noi-24.4.0/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/.idea/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-24.4.0/.idea/encodings.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1839 2015-09-19 04:08:02.000000 lino-noi-24.4.0/.idea/misc.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      260 2015-09-19 04:08:02.000000 lino-noi-24.4.0/.idea/modules.xml
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/.idea/scopes/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      139 2015-09-19 04:08:02.000000 lino-noi-24.4.0/.idea/scopes/scope_settings.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      166 2015-09-19 04:08:02.000000 lino-noi-24.4.0/.idea/vcs.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2202 2015-09-19 04:08:02.000000 lino-noi-24.4.0/.idea/workspace.xml
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:54:16.000000 lino-noi-24.4.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      109 2016-08-14 01:22:00.000000 lino-noi-24.4.0/MANIFEST.in
+-rw-r--r--   0 luc       (1000) www-data    (33)     1504 2024-04-23 12:43:46.838096 lino-noi-24.4.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      716 2023-03-29 14:44:08.000000 lino-noi-24.4.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2022-08-17 01:06:46.000000 lino-noi-24.4.0/lino_noi/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      286 2024-04-22 19:44:43.000000 lino-noi-24.4.0/lino_noi/lib/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/cal/
+-rw-rw-r--   0 luc       (1000) www-data    (33)      342 2024-01-27 12:43:19.000000 lino-noi-24.4.0/lino_noi/lib/cal/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/cal/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2017-04-04 14:35:11.000000 lino-noi-24.4.0/lino_noi/lib/cal/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2017-04-04 14:35:11.000000 lino-noi-24.4.0/lino_noi/lib/cal/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3552 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/cal/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/contacts/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      274 2021-04-07 10:22:54.000000 lino-noi-24.4.0/lino_noi/lib/contacts/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/contacts/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      244 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/contacts/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       55 2020-04-04 06:56:19.000000 lino-noi-24.4.0/lino_noi/lib/contacts/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-05-26 22:13:00.000000 lino-noi-24.4.0/lino_noi/lib/contacts/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3226 2024-02-14 17:21:06.000000 lino-noi-24.4.0/lino_noi/lib/contacts/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/courses/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      813 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/courses/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      719 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/courses/models.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2553 2024-03-24 06:38:16.000000 lino-noi-24.4.0/lino_noi/lib/courses/ui.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/groups/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      320 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/groups/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1363 2024-03-24 15:32:39.000000 lino-noi-24.4.0/lino_noi/lib/groups/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      332 2024-03-29 17:15:07.000000 lino-noi-24.4.0/lino_noi/lib/noi/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/noi/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:02.000000 lino-noi-24.4.0/lino_noi/lib/noi/fixtures/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20952 2024-04-22 13:57:16.000000 lino-noi-24.4.0/lino_noi/lib/noi/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     6601 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/noi/fixtures/linotickets.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)      198 2024-01-27 15:28:56.000000 lino-noi-24.4.0/lino_noi/lib/noi/fixtures/minimal_ledger.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2153 2024-04-22 19:49:02.000000 lino-noi-24.4.0/lino_noi/lib/noi/help_texts.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      545 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/noi/layouts.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.826094 lino-noi-24.4.0/lino_noi/lib/noi/locale/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.826094 lino-noi-24.4.0/lino_noi/lib/noi/locale/de/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2008 2017-04-04 14:35:11.000000 lino-noi-24.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    14514 2019-03-29 11:25:54.000000 lino-noi-24.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.826094 lino-noi-24.4.0/lino_noi/lib/noi/locale/et/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      660 2017-04-04 14:35:11.000000 lino-noi-24.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13858 2019-03-29 11:25:55.000000 lino-noi-24.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.826094 lino-noi-24.4.0/lino_noi/lib/noi/locale/fr/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      490 2017-04-04 14:35:11.000000 lino-noi-24.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13846 2019-03-29 11:25:54.000000 lino-noi-24.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    22981 2024-02-14 17:21:06.000000 lino-noi-24.4.0/lino_noi/lib/noi/migrate.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1128 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/noi/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     6438 2024-04-22 12:54:34.000000 lino-noi-24.4.0/lino_noi/lib/noi/settings.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3219 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/noi/user_types.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      383 2024-03-29 09:13:57.000000 lino-noi-24.4.0/lino_noi/lib/noi/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/products/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      301 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/products/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      976 2024-03-25 11:04:19.000000 lino-noi-24.4.0/lino_noi/lib/products/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/public/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1139 2024-02-14 17:21:06.000000 lino-noi-24.4.0/lino_noi/lib/public/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/public/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/public/config/noi/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      474 2019-11-25 17:29:52.000000 lino-noi-24.4.0/lino_noi/lib/public/config/noi/index.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      720 2022-09-01 18:33:50.000000 lino-noi-24.4.0/lino_noi/lib/public/config/noi/tickets.Ticket.html
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      581 2024-02-14 17:21:06.000000 lino-noi-24.4.0/lino_noi/lib/public/renderer.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1561 2024-02-14 17:21:06.000000 lino-noi-24.4.0/lino_noi/lib/public/views.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/subscriptions/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      189 2023-01-06 20:30:18.000000 lino-noi-24.4.0/lino_noi/lib/subscriptions/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      401 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/subscriptions/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/tickets/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1728 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/tickets/__init__.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    15387 2024-04-22 09:55:22.000000 lino-noi-24.4.0/lino_noi/lib/tickets/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3967 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/tickets/workflows.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/trading/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      313 2024-03-25 11:16:15.000000 lino-noi-24.4.0/lino_noi/lib/trading/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/trading/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.830094 lino-noi-24.4.0/lino_noi/lib/trading/config/trading/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/trading/config/trading/VatProductInvoice/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1413 2023-02-15 06:31:52.000000 lino-noi-24.4.0/lino_noi/lib/trading/config/trading/VatProductInvoice/default.weasy.html
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/trading/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-05-09 16:04:58.000000 lino-noi-24.4.0/lino_noi/lib/trading/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       53 2024-03-25 11:04:19.000000 lino-noi-24.4.0/lino_noi/lib/trading/fixtures/std.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      986 2024-03-25 11:04:19.000000 lino-noi-24.4.0/lino_noi/lib/trading/models.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/users/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       37 2023-03-06 06:43:39.000000 lino-noi-24.4.0/lino_noi/lib/users/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.834095 lino-noi-24.4.0/lino_noi/lib/users/fixtures/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 04:09:00.000000 lino-noi-24.4.0/lino_noi/lib/users/fixtures/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:56:49.000000 lino-noi-24.4.0/lino_noi/lib/users/fixtures/demo.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       47 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/users/fixtures/demo2.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:56:50.000000 lino-noi-24.4.0/lino_noi/lib/users/fixtures/demo_users.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      247 2024-02-14 17:21:05.000000 lino-noi-24.4.0/lino_noi/lib/users/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1503 2024-04-22 13:07:29.000000 lino-noi-24.4.0/lino_noi/lib/users/ui.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3045 2024-04-23 12:43:33.000000 lino-noi-24.4.0/lino_noi/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.838096 lino-noi-24.4.0/lino_noi.egg-info/
+-rw-r--r--   0 luc       (1000) www-data    (33)     1504 2024-04-23 12:43:46.000000 lino-noi-24.4.0/lino_noi.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2535 2024-04-23 12:43:46.000000 lino-noi-24.4.0/lino_noi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2024-04-23 12:43:46.000000 lino-noi-24.4.0/lino_noi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-08-31 16:13:18.000000 lino-noi-24.4.0/lino_noi.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        8 2024-04-23 12:43:46.000000 lino-noi-24.4.0/lino_noi.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        9 2024-04-23 12:43:46.000000 lino-noi-24.4.0/lino_noi.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)      328 2023-12-03 03:21:00.000000 lino-noi-24.4.0/requirements.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2024-04-23 12:43:46.838096 lino-noi-24.4.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:21:05.000000 lino-noi-24.4.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      492 2024-02-14 17:21:05.000000 lino-noi-24.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2024-04-23 12:43:46.838096 lino-noi-24.4.0/tests/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-12-18 18:50:53.000000 lino-noi-24.4.0/tests/__init__.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      180 2024-02-14 17:21:06.000000 lino-noi-24.4.0/tests/test_docs.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      187 2024-02-14 17:21:06.000000 lino-noi-24.4.0/tests/test_packages.py
```

### Comparing `lino-noi-24.3.1/.idea/misc.xml` & `lino-noi-24.4.0/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/.idea/workspace.xml` & `lino-noi-24.4.0/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/COPYING` & `lino-noi-24.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/PKG-INFO` & `lino-noi-24.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 24.3.1
+Version: 24.4.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lino-noi-24.3.1/README.rst` & `lino-noi-24.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/cal/models.py` & `lino-noi-24.4.0/lino_noi/lib/cal/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/contacts/models.py` & `lino-noi-24.4.0/lino_noi/lib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/courses/__init__.py` & `lino-noi-24.4.0/lino_noi/lib/courses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/courses/models.py` & `lino-noi-24.4.0/lino_noi/lib/courses/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/courses/ui.py` & `lino-noi-24.4.0/lino_noi/lib/courses/ui.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/groups/models.py` & `lino-noi-24.4.0/lino_noi/lib/groups/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/fixtures/demo.py` & `lino-noi-24.4.0/lino_noi/lib/noi/fixtures/demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 def tickets_objects():
     # was previously in tickets
     User = rt.models.users.User
     Company = rt.models.contacts.Company
     Person = rt.models.contacts.Person
     TT = rt.models.tickets.TicketType
     Ticket = rt.models.tickets.Ticket
+    Topic = rt.models.topics.Topic
+    Tag = rt.models.topics.Tag
     Group = rt.models.groups.Group
     Membership = rt.models.groups.Membership
     # Milestone = dd.plugins.tickets.milestone_model
     Site = dd.plugins.tickets.site_model
     List = rt.models.lists.List
     # InvoicingAreas = rt.models.invoicing.InvoicingAreas
     Subscription = rt.models.subscriptions.Subscription
@@ -99,17 +101,27 @@
     #     user_type=rt.models.users.UserTypes.user))
     reporter_types = [
         t for t in UserTypes.get_list_items()
         if t.has_required_roles([Reporter])
     ]
     REPORTERS = Cycler(User.objects.filter(user_type__in=reporter_types))
 
+    yield Topic(name=_("Front end"))
+    yield Topic(name=_("Database"))
+    yield Topic(name=_("Hosting"))
+    yield Topic(name=_("QA"))
+    yield Topic(name=_("Deployment"))
+
+    # yield named(Topic, _("Front end"))
+    # yield named(Topic, _("Database"))
+    # yield named(Topic, _("Public relations"))
+    #
     yield named(Group, _("Developers"))
     yield named(Group, _("Managers"), private=True)
-    yield named(Group, _("Front-end team"))
+    yield named(Group, _("Sales team"))
 
     yield named(TT, _("Bugfix"), reporting_type=ReportingTypes.regular)
     yield named(TT, _("Enhancement"), reporting_type=ReportingTypes.extra)
     yield named(TT, _("Upgrade"), reporting_type=ReportingTypes.regular)
 
     # sprint = named(Line, _("Sprint"))
     # yield sprint
@@ -334,22 +346,27 @@
 
     # n = Ticket.objects.count()
 
     for i in range(100):
         # yield ticket("Ticket {}".format(i+n+1))
         yield ticket(TEXTS.pop())
 
+    TOPICS = Cycler(rt.models.topics.Topic.objects.all())
+
     parent = None
     for t in Ticket.objects.all():
         if t.id % 6:
             t.parent = parent
             t.full_clean()
             t.save()
         if t.id % 13:
             parent = t
+        if t.id % 3:
+            for i in range(t.id % 3):
+                yield Tag(owner=t, topic=TOPICS.pop())
 
     # if dd.is_installed('meetings'):
     #     Deployment = rt.models.deploy.Deployment
     #     WishTypes = rt.models.deploy.WishTypes
     #     WTYPES = Cycler(WishTypes.objects())
     #     MILESTONES = Cycler(Milestone.objects.all())
     #     for t in Ticket.objects.all():
@@ -563,14 +580,14 @@
     TransferRule = rt.models.storage.TransferRule
     sls = rt.models.ledger.Journal.get_by_ref("SLS")
     srv = rt.models.ledger.Journal.get_by_ref("SRV")
     yield TransferRule(to_state=ProvisionStates.purchased, journal=sls)
     yield TransferRule(from_state=ProvisionStates.purchased, journal=srv)
 
     from lino_xl.lib.invoicing.utils import invoicing_task, invoicing_rule
-    yield invoicing_task("SRV")
-    yield invoicing_task("SLS")
-    yield invoicing_task("SUB")
+    yield invoicing_task("SRV", user_id=1)
+    yield invoicing_task("SLS", user_id=1)
+    yield invoicing_task("SUB", user_id=1)
     yield invoicing_rule("SRV", rt.models.working.Session)
     yield invoicing_rule("SUB", rt.models.subscriptions.SubscriptionPeriod)
-    # yield invoicing_rule("SLS", rt.models.sales.InvoiceItem)
+    # yield invoicing_rule("SLS", rt.models.trading.InvoiceItem)
     yield invoicing_rule("SLS", rt.models.storage.Filler)
```

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/fixtures/linotickets.py` & `lino-noi-24.4.0/lino_noi/lib/noi/fixtures/linotickets.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/help_texts.py` & `lino-noi-24.4.0/lino_noi/lib/noi/help_texts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/layouts.py` & `lino-noi-24.4.0/lino_noi/lib/noi/layouts.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo` & `lino-noi-24.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po` & `lino-noi-24.4.0/lino_noi/lib/noi/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo` & `lino-noi-24.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po` & `lino-noi-24.4.0/lino_noi/lib/noi/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po` & `lino-noi-24.4.0/lino_noi/lib/noi/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/migrate.py` & `lino-noi-24.4.0/lino_noi/lib/noi/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/models.py` & `lino-noi-24.4.0/lino_noi/lib/noi/models.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/settings.py` & `lino-noi-24.4.0/lino_noi/lib/noi/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,35 +40,35 @@
     # root_urlconf = 'lino_book.projects.noi1e.urls'
 
     # TODO: move migrator to lino_noi.projects.team
     migration_class = 'lino_noi.lib.noi.migrate.Migrator'
 
     auto_configure_logger_names = "lino lino_xl lino_noi"
 
-    def get_installed_apps(self):
-        """Implements :meth:`lino.core.site.Site.get_installed_apps` for Lino
+    def get_installed_plugins(self):
+        """Implements :meth:`lino.core.site.Site.get_installed_plugins` for Lino
         Noi.
 
         """
-        yield super().get_installed_apps()
+        yield super().get_installed_plugins()
         # yield 'lino.modlib.extjs'
         # yield 'lino.modlib.bootstrap3'
         yield 'lino.modlib.gfks'
         yield 'lino.modlib.help'
         # yield 'lino.modlib.system'
         # yield 'lino.modlib.users'
         yield 'lino_noi.lib.contacts'
         yield 'lino_noi.lib.users'
         yield 'lino_noi.lib.cal'
         yield 'lino_xl.lib.calview'
         # yield 'lino_xl.lib.extensible'
         # yield 'lino_noi.lib.courses'
         # yield 'lino_noi.lib.products'
 
-        # yield 'lino_noi.lib.topics'
+        yield 'lino_xl.lib.topics'
         # yield 'lino_xl.lib.votes'
         # yield 'lino_xl.lib.stars'
         yield 'lino_noi.lib.tickets'
         yield 'lino_xl.lib.nicknames'
         # yield 'lino_xl.lib.skills'
         # yield 'lino_xl.lib.deploy'
         yield 'lino_xl.lib.working'
@@ -98,59 +98,41 @@
         # yield 'lino_xl.lib.github'
         # yield 'lino.modlib.social_auth'
         yield 'lino_xl.lib.userstats'
         yield 'lino_noi.lib.groups'
         # yield 'lino_noi.lib.groups'
 
         yield 'lino_noi.lib.products'
-        yield 'lino_noi.lib.sales'
+        yield 'lino_noi.lib.trading'
         yield 'lino_xl.lib.storage'
         # yield 'lino_xl.lib.invoicing'  # no need to mention since subscriptions needs it
         yield 'lino_noi.lib.subscriptions'
 
         # if self.has_feature('cms_functionality'):
         yield 'lino_xl.lib.pages'
         # yield 'lino.modlib.publisher'
 
     def get_plugin_configs(self):
         yield super().get_plugin_configs()
-        # self.plugins.topics.deactivate()
         yield 'linod', 'use_channels', True
-        yield 'topics', 'hidden', True
+        # yield 'topics', 'hidden', True
+        yield 'topics', 'partner_model', 'users.User'
         yield 'help', 'make_help_pages', True
         yield 'tickets', 'end_user_model', 'contacts.Person'
         yield 'working', 'ticket_model', 'tickets.Ticket'
         # yield ('system', 'use_dashboard_layouts', True)
         yield 'invoicing', 'order_model', 'subscriptions.Subscription'
         yield 'users', 'allow_online_registration', True
         yield 'summaries', 'duration_max_length', 10
         yield 'nicknames', 'named_model', 'tickets.Ticket'
         # yield 'pages', 'hidden', True
 
-    # def setup_quicklinks(self, user, tb):
-    #     super().setup_quicklinks(user, tb)
-    #     # tb.add_action(self.models.courses.MyActivities)
-    #     # tb.add_action(self.models.meetings.MyMeetings)
-    #     # tb.add_action(self.modules.deploy.MyMilestones)
-    #     # tb.add_action(self.models.tickets.MyTickets)
-    #     # tb.add_action(self.models.tickets.TicketsToTriage)
-    #     # tb.add_action(self.models.tickets.TicketsToTalk)
-    #     # tb.add_action(self.modules.tickets.TicketsToDo)
-    #     tb.add_action(self.models.tickets.RefTickets)
-    #     tb.add_action(self.models.tickets.ActiveTickets)
-    #     tb.add_action(self.models.tickets.AllTickets)
-    #     tb.add_action(
-    #         self.models.tickets.AllTickets.insert_action,
-    #         label=_("Submit a ticket"))
-
-    def do_site_startup(self):
-        super().do_site_startup()
-
-        from lino.utils.watch import watch_changes as wc
-
+    def setup_actions(self):
+        super().setup_actions()
+        from lino.modlib.changes.utils import watch_changes as wc
         wc(self.modules.tickets.Ticket, ignore=['_user_cache'])
         wc(self.modules.comments.Comment, master_key='owner')
         # wc(self.modules.tickets.Link, master_key='ticket')
         # wc(self.modules.working.Session, master_key='owner')
 
         if self.is_installed('votes'):
             wc(self.modules.votes.Vote, master_key='votable')
@@ -165,14 +147,34 @@
         # from lino_xl.lib.contacts.roles import ContactsStaff
         # lib = self.models
         # for m in (lib.contacts.Company, ):
         #     m.define_action(merge_row=MergeAction(
         #         m, required_roles=set([ContactsStaff])))
 
 
+    # def setup_quicklinks(self, user, tb):
+    #     super().setup_quicklinks(user, tb)
+    #     # tb.add_action(self.models.courses.MyActivities)
+    #     # tb.add_action(self.models.meetings.MyMeetings)
+    #     # tb.add_action(self.modules.deploy.MyMilestones)
+    #     # tb.add_action(self.models.tickets.MyTickets)
+    #     # tb.add_action(self.models.tickets.TicketsToTriage)
+    #     # tb.add_action(self.models.tickets.TicketsToTalk)
+    #     # tb.add_action(self.modules.tickets.TicketsToDo)
+    #     tb.add_action(self.models.tickets.RefTickets)
+    #     tb.add_action(self.models.tickets.ActiveTickets)
+    #     tb.add_action(self.models.tickets.AllTickets)
+    #     tb.add_action(
+    #         self.models.tickets.AllTickets.insert_action,
+    #         label=_("Submit a ticket"))
+
+    # def do_site_startup(self):
+    #     super().do_site_startup()
+
+
 # the following line should not be active in a checked-in version
 #~ DATABASES['default']['NAME'] = ':memory:'
 
 USE_TZ = True
 # TIME_ZONE = 'Europe/Brussels'
 # TIME_ZONE = 'Europe/Tallinn'
 TIME_ZONE = 'UTC'
```

### Comparing `lino-noi-24.3.1/lino_noi/lib/noi/user_types.py` & `lino-noi-24.4.0/lino_noi/lib/noi/user_types.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/products/models.py` & `lino-noi-24.4.0/lino_noi/lib/products/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     id product_type category delivery_unit
     body
     """, _("General"))
 
     sales = dd.Panel(
         """
     sales_price vat_class sales_account
-    sales.InvoiceItemsByProduct
+    trading.InvoiceItemsByProduct
     """, _("Sales"))
 
     storage = dd.Panel(
         """
     storage_management
     storage.MovementsByProduct
     """, _("Storage"))
```

### Comparing `lino-noi-24.3.1/lino_noi/lib/public/__init__.py` & `lino-noi-24.4.0/lino_noi/lib/public/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/public/config/noi/tickets.Ticket.html` & `lino-noi-24.4.0/lino_noi/lib/public/config/noi/tickets.Ticket.html`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/public/renderer.py` & `lino-noi-24.4.0/lino_noi/lib/public/renderer.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/public/views.py` & `lino-noi-24.4.0/lino_noi/lib/public/views.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html` & `lino-noi-24.4.0/lino_noi/lib/trading/config/trading/VatProductInvoice/default.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/sales/models.py` & `lino-noi-24.4.0/lino_noi/lib/trading/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2016-2022 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
-from lino_xl.lib.sales.models import *
+from lino_xl.lib.trading.models import *
 from lino.api import _
 
 # InvoicesByJournal.column_names = "number_with_year entry_date #due_date " \
 #     "invoicing_min_date invoicing_max_date " \
 #     "partner " \
 #     "#subject:10 total_incl " \
 #     "workflow_buttons *"
```

### Comparing `lino-noi-24.3.1/lino_noi/lib/tickets/__init__.py` & `lino-noi-24.4.0/lino_noi/lib/tickets/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/tickets/models.py` & `lino-noi-24.4.0/lino_noi/lib/tickets/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from lino import logger
 
 from lino.api import _
 from lino_xl.lib.tickets.models import *
 from lino_xl.lib.working.mixins import SummarizedFromSession
 from lino_xl.lib.working.choicelists import ReportingTypes
 from lino_xl.lib.nicknames.mixins import Nicknameable
+from lino_xl.lib.topics.mixins import Taggable
 from lino.modlib.search.mixins import ElasticSearchable
 
 
 def get_summary_fields():
     for t in ReportingTypes.get_list_items():
         yield t.name + '_hours'
 
@@ -30,15 +31,15 @@
 
     def get_change_observers(self, ar=None):
         for s in rt.models.groups.Group.objects.filter(site=self):
             for sub in s.members.all():
                 yield (sub.user, sub.user.mail_mode)
 
 
-class Ticket(Ticket, SummarizedFromSession, ElasticSearchable, Nicknameable):
+class Ticket(Ticket, SummarizedFromSession, ElasticSearchable, Nicknameable, Taggable):
 
     class Meta(Ticket.Meta):
         # app_label = 'tickets'
         abstract = dd.is_abstract_model(__name__, 'Ticket')
 
     ES_indexes = [('ticket', {
         "mappings": {
@@ -167,15 +168,15 @@
                 mt = rt.models.notify.MessageTypes.tickets
 
                 rt.models.notify.Message.emit_notification(
                     ar, self, mt, msg,
                     [(self.assigned_to, self.assigned_to.mail_mode)])
 
     # show_commits = dd.ShowSlaveTable('github.CommitsByTicket')
-    show_changes = dd.ShowSlaveTable('changes.ChangesByMaster')
+    # show_changes = dd.ShowSlaveTable('changes.ChangesByMaster')
 
     # show_wishes = dd.ShowSlaveTable('deploy.DeploymentsByTicket')
     # show_stars = dd.ShowSlaveTable('stars.AllStarsByController')
 
     def get_change_subject(self, ar, cw):
         ctx = dict(user=ar.user, what=str(self))
         if cw is None:
@@ -254,25 +255,28 @@
     # 50+6=56
     # in XL: label span is 4, so we have 8 units for the fields
     # 56.0/8 = 7
     # summary:  50/56*8 = 7.14 --> 7
     # id:  6/56*8 = 0.85 -> 1
     general1 = """
     overview
+    add_tag
+    topics.TagsByOwner
     """
+
     general2 = """
     order end_user ticket_type
     triager_panel
     priority:10 planned_time deadline
     SUMMARY_FIELDS
     working.SessionsByTicket
     """
 
     triager_panel = dd.Panel("""
-    group quick_assign_to private:10
+    group quick_assign_to
     """,
                              required_roles=dd.login_required(Triager))
 
     general3 = """
     workflow_buttons
     comment
     comments.CommentsByRFC:30
@@ -284,35 +288,34 @@
 
     # history_tab = dd.Panel("""
     # changes.ChangesByMaster #stars.StarsByController:20
     # github.CommitsByTicket
     # """, label=_("History"), required_roles=dd.login_required(Triager))
 
     more1 = """
-    id:6 my_nickname
-    summary
-    ref
+    id:6 summary
+    my_nickname
     # standby feedback closed
     description
     """
 
     more2 = """
-    site
+    ref
+    # site
     upgrade_notes
-    uploads.UploadsByController
     # tickets.CheckListItemsByTicket
     """
 
     more3 = """
     state
     assigned_to
-    user created
-    modified fixed_since
-    duplicate_of
-    DuplicatesByTicket:20
+    user
+    created modified #fixed_since
+    private
+    uploads.UploadsByController
     """
 
     # more1 = """
     # created modified fixed_since #reported_for #fixed_date #fixed_time
     # state assigned_to ref duplicate_of deadline
     # # standby feedback closed
     # """
@@ -321,23 +324,29 @@
     # # deploy.DeploymentsByTicket
     # # skills.DemandsByDemander
     # stars.AllStarsByController
     # uploads.UploadsByController
     # """, label=_("Even more"))
 
     links = dd.Panel("""
-    links_left comments.CommentsByMentioned #LinksByTicket
+    links1 links2
     """,
                      label=_("Links"))
 
-    links_left = """
+    links1 = """
     parent
     TicketsByParent
     """
 
+    links2 = """
+    duplicate_of
+    DuplicatesByTicket:20
+    comments.CommentsByMentioned
+    """
+
 
 class TicketInsertLayout(dd.InsertLayout):
     main = """
     summary #private:20
     right:30 left:50
     """
```

### Comparing `lino-noi-24.3.1/lino_noi/lib/tickets/workflows.py` & `lino-noi-24.4.0/lino_noi/lib/tickets/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-noi-24.3.1/lino_noi/lib/users/ui.py` & `lino-noi-24.4.0/lino_noi/lib/users/ui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2015-2023 Rumma & Ko Ltd
+# Copyright 2015-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
-"""Desktop UI for this plugin.
-
-"""
 
 from lino.modlib.users.ui import *
 
 from lino.api import _
 
 from lino.core import actions
 from lino_xl.lib.working.roles import Worker
@@ -19,50 +16,44 @@
 
 class UserDetail(UserDetail):
     """Layout of User Detail in Lino Noi."""
 
     main = "general #contact calendar dashboard.WidgetsByUser working.SummariesByUser memo.MentionsByOwner"
 
     general = dd.Panel("""
-    general1:30 general2:30 general3:30 #working:15
-    SocialAuthsByUser #tickets.SubscriptionsByUser groups.MembershipsByUser
+    general1:30 general2:30 general3:30
+    SocialAuthsByUser #tickets.SubscriptionsByUser groups.MembershipsByUser topics.InterestsByPartner
     """,
                        label=_("General"))
 
     # skills.OffersByEndUser
 
-    # if dd.is_installed('working'):
-    #     working = dd.Panel("""
-    #
-    #
-    #     """, label=_("Clocking"), required_roles=dd.login_required(Worker))
-    # else:
-    #     working = dd.DummyPanel()
-
     calendar = dd.Panel("""
     event_type
     cal.SubscriptionsByUser
     # cal.MembershipsByUser
     """,
                         label=dd.plugins.cal.verbose_name,
                         required_roles=dd.login_required(OfficeUser))
 
     general1 = """
     username user_type:20
-    first_name last_name initials
-    person partner #user_site
+    first_name last_name
+    initials nickname
+    person company #user_site
     """
 
     general2 = """
-    language:10 dashboard_layout
+    language:10 id #dashboard_layout
     email mail_mode
     notify_myself open_session_on_new_ticket
+    status
     """
 
     general3 = """
-    created:12 modified:12 id
+    created:12 modified:12
     date_format time_zone
     start_date end_date
     """
 
 
 # Users.detail_layout = UserDetail()
```

### Comparing `lino-noi-24.3.1/lino_noi/setup_info.py` & `lino-noi-24.4.0/lino_noi/setup_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2014-2024 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
-
-# python setup.py test -s tests.test_packages
+# python -m unittest tests.test_packages
 
 ATELIER_INFO = dict(
     nickname="noi",
     verbose_name="Lino Noi",
     # srcref_url='https://gitlab.com/lino-framework/cosi/blob/master/%s',
     intersphinx_urls=dict(docs="https://noi.lino-framework.org"))
 
 SETUP_INFO = dict(
     name='lino-noi',
-    version='24.3.1',
+    version='24.4.0',
     install_requires=['lino-xl'],
     # tests_require=['pytest', 'mock'],
     test_suite='tests',
     description=("Manage support tickets and working time."),
     long_description="""\
 
 Lino Noi is a customizable ticket management and time tracking
@@ -63,17 +62,16 @@
 lino_noi
 lino_noi.lib
 lino_noi.lib.noi
 lino_noi.lib.noi.fixtures
 lino_noi.lib.contacts
 lino_noi.lib.contacts.fixtures
 lino_noi.lib.public
-lino_noi.lib.sales
-lino_noi.lib.sales.fixtures
-lino_noi.lib.topics
+lino_noi.lib.trading
+lino_noi.lib.trading.fixtures
 lino_noi.lib.users
 lino_noi.lib.users.fixtures
 lino_noi.lib.products
 lino_noi.lib.subscriptions
 lino_noi.lib.groups
 lino_noi.lib.cal
 lino_noi.lib.cal.fixtures
```

### Comparing `lino-noi-24.3.1/lino_noi.egg-info/PKG-INFO` & `lino-noi-24.4.0/lino_noi.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-noi
-Version: 24.3.1
+Version: 24.4.0
 Summary: Manage support tickets and working time.
 Home-page: https://gitlab.com/lino-framework/noi
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lino-noi-24.3.1/lino_noi.egg-info/SOURCES.txt` & `lino-noi-24.4.0/lino_noi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -54,26 +54,24 @@
 lino_noi/lib/products/__init__.py
 lino_noi/lib/products/models.py
 lino_noi/lib/public/__init__.py
 lino_noi/lib/public/renderer.py
 lino_noi/lib/public/views.py
 lino_noi/lib/public/config/noi/index.html
 lino_noi/lib/public/config/noi/tickets.Ticket.html
-lino_noi/lib/sales/__init__.py
-lino_noi/lib/sales/models.py
-lino_noi/lib/sales/config/sales/VatProductInvoice/default.weasy.html
-lino_noi/lib/sales/fixtures/__init__.py
-lino_noi/lib/sales/fixtures/std.py
 lino_noi/lib/subscriptions/__init__.py
 lino_noi/lib/subscriptions/models.py
 lino_noi/lib/tickets/__init__.py
 lino_noi/lib/tickets/models.py
 lino_noi/lib/tickets/workflows.py
-lino_noi/lib/topics/__init__.py
-lino_noi/lib/topics/models.py
+lino_noi/lib/trading/__init__.py
+lino_noi/lib/trading/models.py
+lino_noi/lib/trading/config/trading/VatProductInvoice/default.weasy.html
+lino_noi/lib/trading/fixtures/__init__.py
+lino_noi/lib/trading/fixtures/std.py
 lino_noi/lib/users/__init__.py
 lino_noi/lib/users/models.py
 lino_noi/lib/users/ui.py
 lino_noi/lib/users/fixtures/__init__.py
 lino_noi/lib/users/fixtures/demo.py
 lino_noi/lib/users/fixtures/demo2.py
 lino_noi/lib/users/fixtures/demo_users.py
```

