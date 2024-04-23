# Comparing `tmp/NbRisk-35.1.1.tar.gz` & `tmp/nbrisk-35.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NbRisk-35.1.1.tar", last modified: Fri Apr  5 18:54:29 2024, max compression
+gzip compressed data, was "nbrisk-35.1.2.tar", last modified: Mon Apr 22 02:15:04 2024, max compression
```

## Comparing `NbRisk-35.1.1.tar` & `nbrisk-35.1.2.tar`

### file list

```diff
@@ -1,74 +1,77 @@
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.389345 NbRisk-35.1.1/
--rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 NbRisk-35.1.1/LICENSE
--rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 NbRisk-35.1.1/MANIFEST.in
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.385345 NbRisk-35.1.1/NbRisk.egg-info/
--rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2091 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/SOURCES.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        1 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/dependency_links.txt
--rw-rw-r--   0 renato    (1000) renato    (1000)        8 2024-04-05 18:54:29.000000 NbRisk-35.1.1/NbRisk.egg-info/top_level.txt
--rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-05 18:54:29.385345 NbRisk-35.1.1/PKG-INFO
--rw-rw-r--   0 renato    (1000) renato    (1000)     2780 2024-04-05 18:53:39.000000 NbRisk-35.1.1/README.md
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.353345 NbRisk-35.1.1/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)      715 2024-04-05 18:50:37.000000 NbRisk-35.1.1/nb_risk/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 NbRisk-35.1.1/nb_risk/admin.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.357345 NbRisk-35.1.1/nb_risk/api/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.1/nb_risk/api/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      988 2023-04-21 01:31:32.000000 NbRisk-35.1.1/nb_risk/api/nested_serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5107 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/api/serializers.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 NbRisk-35.1.1/nb_risk/api/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 NbRisk-35.1.1/nb_risk/api/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 NbRisk-35.1.1/nb_risk/choices.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2023-04-25 01:55:31.000000 NbRisk-35.1.1/nb_risk/columns.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2023-04-25 01:50:42.000000 NbRisk-35.1.1/nb_risk/cve.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1975 2024-04-05 18:31:15.000000 NbRisk-35.1.1/nb_risk/filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     5607 2024-03-23 01:17:05.000000 NbRisk-35.1.1/nb_risk/forms.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.1/nb_risk/middleware.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.361345 NbRisk-35.1.1/nb_risk/migrations/
--rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 NbRisk-35.1.1/nb_risk/migrations/0001_initial.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 NbRisk-35.1.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 NbRisk-35.1.1/nb_risk/migrations/0003_control.py
--rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 NbRisk-35.1.1/nb_risk/migrations/0004_alter_vulnerability_options.py
--rw-r--r--   0 renato    (1000) renato    (1000)      434 2023-05-13 16:13:09.000000 NbRisk-35.1.1/nb_risk/migrations/0005_alter_vulnerability_cvssbasescore.py
--rw-r--r--   0 renato    (1000) renato    (1000)      424 2023-05-13 17:11:12.000000 NbRisk-35.1.1/nb_risk/migrations/0006_vulnerability_unique_vuln_name.py
--rw-r--r--   0 renato    (1000) renato    (1000)      615 2023-08-20 02:18:04.000000 NbRisk-35.1.1/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py
--rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 NbRisk-35.1.1/nb_risk/migrations/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     8712 2023-08-20 02:17:50.000000 NbRisk-35.1.1/nb_risk/models.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2023-05-10 13:19:51.000000 NbRisk-35.1.1/nb_risk/navigation.py
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 NbRisk-35.1.1/nb_risk/signals.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4050 2023-05-12 20:01:49.000000 NbRisk-35.1.1/nb_risk/tables.py
--rw-rw-r--   0 renato    (1000) renato    (1000)      803 2023-08-20 02:15:03.000000 NbRisk-35.1.1/nb_risk/template_content.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.337345 NbRisk-35.1.1/nb_risk/templates/
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.377345 NbRisk-35.1.1/nb_risk/templates/nb_risk/
--rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/control.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/control_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/control_risks.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/generic_vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/risk.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/threatevent.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/threatsource.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
--rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_list.html
--rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2023-02-14 23:17:46.000000 NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_search.html
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.377345 NbRisk-35.1.1/nb_risk/tests/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 00:49:42.000000 NbRisk-35.1.1/nb_risk/tests/__init__.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.377345 NbRisk-35.1.1/nb_risk/tests/control/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:28.000000 NbRisk-35.1.1/nb_risk/tests/control/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1133 2024-03-23 00:50:09.000000 NbRisk-35.1.1/nb_risk/tests/custom.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.381345 NbRisk-35.1.1/nb_risk/tests/threatsource/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:12.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1900 2024-04-05 18:41:28.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/test_api.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2158 2024-03-31 19:52:14.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/test_filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     2359 2024-04-05 18:34:59.000000 NbRisk-35.1.1/nb_risk/tests/threatsource/test_views.py
-drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-05 18:54:29.385345 NbRisk-35.1.1/nb_risk/tests/vulnerability/
--rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-05 18:16:40.000000 NbRisk-35.1.1/nb_risk/tests/vulnerability/__init__.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1809 2024-04-05 18:28:15.000000 NbRisk-35.1.1/nb_risk/tests/vulnerability/test_filters.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     1982 2024-04-05 18:35:09.000000 NbRisk-35.1.1/nb_risk/tests/vulnerability/test_views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)     4410 2024-03-23 01:58:21.000000 NbRisk-35.1.1/nb_risk/urls.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       23 2024-04-05 18:53:47.000000 NbRisk-35.1.1/nb_risk/version.py
--rw-rw-r--   0 renato    (1000) renato    (1000)    10772 2024-03-23 01:43:26.000000 NbRisk-35.1.1/nb_risk/views.py
--rw-rw-r--   0 renato    (1000) renato    (1000)       38 2024-04-05 18:54:29.389345 NbRisk-35.1.1/setup.cfg
--rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 NbRisk-35.1.1/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.758740 nbrisk-35.1.2/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10174 2022-08-15 01:26:39.000000 nbrisk-35.1.2/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)       43 2022-08-15 01:38:51.000000 nbrisk-35.1.2/MANIFEST.in
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.758740 nbrisk-35.1.2/NbRisk.egg-info/
+-rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-22 02:15:04.000000 nbrisk-35.1.2/NbRisk.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2191 2024-04-22 02:15:04.000000 nbrisk-35.1.2/NbRisk.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2024-04-22 02:15:04.000000 nbrisk-35.1.2/NbRisk.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        8 2024-04-22 02:15:04.000000 nbrisk-35.1.2/NbRisk.egg-info/top_level.txt
+-rw-r--r--   0 renato    (1000) renato    (1000)     3209 2024-04-22 02:15:04.758740 nbrisk-35.1.2/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2780 2024-04-05 18:53:39.000000 nbrisk-35.1.2/README.md
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.750740 nbrisk-35.1.2/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      715 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-01-19 18:35:20.000000 nbrisk-35.1.2/nb_risk/admin.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.750740 nbrisk-35.1.2/nb_risk/api/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 nbrisk-35.1.2/nb_risk/api/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1467 2024-04-22 02:10:22.000000 nbrisk-35.1.2/nb_risk/api/nested_serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5376 2024-04-22 02:09:48.000000 nbrisk-35.1.2/nb_risk/api/serializers.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      489 2023-04-21 01:34:23.000000 nbrisk-35.1.2/nb_risk/api/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1179 2023-04-21 01:34:15.000000 nbrisk-35.1.2/nb_risk/api/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3213 2023-04-21 01:04:22.000000 nbrisk-35.1.2/nb_risk/choices.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2108 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/columns.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3295 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/cve.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1975 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5607 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/forms.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2022-08-15 01:38:51.000000 nbrisk-35.1.2/nb_risk/middleware.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.754740 nbrisk-35.1.2/nb_risk/migrations/
+-rw-r--r--   0 renato    (1000) renato    (1000)     6544 2023-01-25 19:11:25.000000 nbrisk-35.1.2/nb_risk/migrations/0001_initial.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1558 2023-04-21 00:03:25.000000 nbrisk-35.1.2/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)     1391 2023-04-21 01:36:32.000000 nbrisk-35.1.2/nb_risk/migrations/0003_control.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      394 2023-05-10 13:39:08.000000 nbrisk-35.1.2/nb_risk/migrations/0004_alter_vulnerability_options.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      434 2023-05-13 16:13:09.000000 nbrisk-35.1.2/nb_risk/migrations/0005_alter_vulnerability_cvssbasescore.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      424 2023-05-13 17:11:12.000000 nbrisk-35.1.2/nb_risk/migrations/0006_vulnerability_unique_vuln_name.py
+-rw-r--r--   0 renato    (1000) renato    (1000)      615 2023-08-20 02:18:04.000000 nbrisk-35.1.2/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py
+-rw-r--r--   0 renato    (1000) renato    (1000)        0 2023-01-25 19:11:25.000000 nbrisk-35.1.2/nb_risk/migrations/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     8712 2023-08-20 02:17:50.000000 nbrisk-35.1.2/nb_risk/models.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4078 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/navigation.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-08 01:05:57.000000 nbrisk-35.1.2/nb_risk/signals.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4050 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/tables.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      803 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/template_content.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.746740 nbrisk-35.1.2/nb_risk/templates/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.754740 nbrisk-35.1.2/nb_risk/templates/nb_risk/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1199 2023-05-12 19:59:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/control.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/control_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      235 2023-05-12 19:59:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/control_risks.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      667 2023-01-19 19:51:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      269 2023-01-19 18:13:59.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/generic_vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2087 2023-01-25 21:22:56.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/risk.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1939 2023-05-12 19:59:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/threatevent.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/threatevent_vulnerabilities.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1694 2023-04-02 19:40:16.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/threatsource.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2455 2023-05-12 19:59:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/vulnerability.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      233 2023-05-12 19:59:37.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/vulnerability_affected_assets.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      296 2023-01-25 01:39:38.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/vulnerability_assignment_button.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)      236 2023-02-16 01:36:47.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/vulnerability_list.html
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1473 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/templates/nb_risk/vulnerability_search.html
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.754740 nbrisk-35.1.2/nb_risk/tests/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 00:49:42.000000 nbrisk-35.1.2/nb_risk/tests/__init__.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.754740 nbrisk-35.1.2/nb_risk/tests/control/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:28.000000 nbrisk-35.1.2/nb_risk/tests/control/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1133 2024-03-23 00:50:09.000000 nbrisk-35.1.2/nb_risk/tests/custom.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.758740 nbrisk-35.1.2/nb_risk/tests/threatsource/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-03-23 01:01:12.000000 nbrisk-35.1.2/nb_risk/tests/threatsource/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1900 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/tests/threatsource/test_api.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2158 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/tests/threatsource/test_filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2359 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/tests/threatsource/test_views.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.758740 nbrisk-35.1.2/nb_risk/tests/vulnerability/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-05 18:16:40.000000 nbrisk-35.1.2/nb_risk/tests/vulnerability/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1809 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/tests/vulnerability/test_filters.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1982 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/tests/vulnerability/test_views.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2024-04-22 02:15:04.758740 nbrisk-35.1.2/nb_risk/tests/vulnerabilityassignment/
+-rw-rw-r--   0 renato    (1000) renato    (1000)        0 2024-04-22 01:58:26.000000 nbrisk-35.1.2/nb_risk/tests/vulnerabilityassignment/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3510 2024-04-22 01:53:41.000000 nbrisk-35.1.2/nb_risk/tests/vulnerabilityassignment/test_api.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4410 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/urls.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       23 2024-04-22 02:12:44.000000 nbrisk-35.1.2/nb_risk/version.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10772 2024-04-22 01:37:47.000000 nbrisk-35.1.2/nb_risk/views.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       38 2024-04-22 02:15:04.758740 nbrisk-35.1.2/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1195 2023-01-19 04:15:27.000000 nbrisk-35.1.2/setup.py
```

### Comparing `NbRisk-35.1.1/LICENSE` & `nbrisk-35.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/NbRisk.egg-info/PKG-INFO` & `nbrisk-35.1.2/NbRisk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.1.1
+Version: 35.1.2
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-35.1.1/NbRisk.egg-info/SOURCES.txt` & `nbrisk-35.1.2/NbRisk.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -54,8 +54,10 @@
 nb_risk/tests/control/__init__.py
 nb_risk/tests/threatsource/__init__.py
 nb_risk/tests/threatsource/test_api.py
 nb_risk/tests/threatsource/test_filters.py
 nb_risk/tests/threatsource/test_views.py
 nb_risk/tests/vulnerability/__init__.py
 nb_risk/tests/vulnerability/test_filters.py
-nb_risk/tests/vulnerability/test_views.py
+nb_risk/tests/vulnerability/test_views.py
+nb_risk/tests/vulnerabilityassignment/__init__.py
+nb_risk/tests/vulnerabilityassignment/test_api.py
```

### Comparing `NbRisk-35.1.1/PKG-INFO` & `nbrisk-35.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NbRisk
-Version: 35.1.1
+Version: 35.1.2
 Summary: NIST 800-30 Risk Management for Netbox
 Home-page: https://github.com/renatoalmeidaoliveira/nbrisk
 Author: Renato Almdida Oliveira
 Author-email: renato.almeida.oliveira@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

### Comparing `NbRisk-35.1.1/README.md` & `nbrisk-35.1.2/README.md`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/__init__.py` & `nbrisk-35.1.2/nb_risk/__init__.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/api/nested_serializers.py` & `nbrisk-35.1.2/nb_risk/api/nested_serializers.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,8 +27,23 @@
     display = serializers.SerializerMethodField('get_display')
     
     def get_display(self, obj):
         return obj.name
 
     class Meta:
         model = models.Risk
-        fields = ["id", "url", "display", "name"]
+        fields = ["id", "url", "display", "name"]
+
+# VulnerabilityAssignment Nested Serializers
+
+class NestedVulnerabilityAssignmentSerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name="plugins-api:nb_risk-api:vulnerabilityassignment-detail"
+    )
+    display = serializers.SerializerMethodField('get_display')
+    
+    def get_display(self, obj):
+        return obj.name
+
+    class Meta:
+        model = models.VulnerabilityAssignment
+        fields = ["id", "url", "display"]
```

### Comparing `NbRisk-35.1.1/nb_risk/api/serializers.py` & `nbrisk-35.1.2/nb_risk/api/serializers.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from utilities.api import get_serializer_for_model
 
 
 from netbox.api.serializers import NetBoxModelSerializer
 from nb_risk.api.nested_serializers import (
     NestedThreatSourceSerializer,
     NestedRiskSerializer,
+    NestedVulnerabilityAssignmentSerializer,
 )
 from .. import models, choices
 
 # ThreatSource Serializers
 
 class ThreatSourceSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nb_risk-api:threatsource-detail")
@@ -90,39 +91,46 @@
 
 class VulnerabilityAssignmentSerializer(NetBoxModelSerializer):
     url = serializers.HyperlinkedIdentityField(view_name="plugins-api:nb_risk-api:vulnerabilityassignment-detail")
     display = serializers.SerializerMethodField('get_display')
     asset_object_type = ContentTypeField(
         queryset=ContentType.objects.filter(choices.AssetTypes),
         required=True,
-        allow_null=True
     )
-    asset = serializers.SerializerMethodField(read_only=True)
+    asset = serializers.SerializerMethodField('get_asset')
     vulnerability = serializers.SlugRelatedField(slug_field="name", queryset=models.Vulnerability.objects.all())
 
-    asset_object_id = serializers.IntegerField(source='asset.id')
+    asset_id = serializers.IntegerField(source='asset.id')
+
+    def validate(self, data):
+        asset_id = data['asset']['id']
+        asset_object_type = data['asset_object_type']
+        asset = asset_object_type.get_object_for_this_type(id=asset_id)
+        data['asset'] = asset
+        return super().validate(data)
 
     def get_asset(self, obj):
         if obj.asset is None:
             return None
         serializer = get_serializer_for_model(obj.asset, prefix='Nested')
         context = {'request': self.context['request']}
         return serializer(obj.asset, context=context).data
 
     def get_display(self, obj):
         return obj.name
 
+
     class Meta:
         model = models.VulnerabilityAssignment
         fields = [
             "id",
             "url",
             "display",
             "asset_object_type",
-            "asset_object_id",
+            "asset_id",
             "asset",
             "vulnerability",
         ]
 
 # Risk Serializers
 
 class RiskSerializer(NetBoxModelSerializer):
```

### Comparing `NbRisk-35.1.1/nb_risk/api/views.py` & `nbrisk-35.1.2/nb_risk/api/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/choices.py` & `nbrisk-35.1.2/nb_risk/choices.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/columns.py` & `nbrisk-35.1.2/nb_risk/columns.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/cve.py` & `nbrisk-35.1.2/nb_risk/cve.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/filters.py` & `nbrisk-35.1.2/nb_risk/filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/forms.py` & `nbrisk-35.1.2/nb_risk/forms.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/migrations/0001_initial.py` & `nbrisk-35.1.2/nb_risk/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py` & `nbrisk-35.1.2/nb_risk/migrations/0002_vulnerability_cvssaccesscomplexity_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/migrations/0003_control.py` & `nbrisk-35.1.2/nb_risk/migrations/0003_control.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py` & `nbrisk-35.1.2/nb_risk/migrations/0007_remove_vulnerability_unique_vuln_name_and_more.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/models.py` & `nbrisk-35.1.2/nb_risk/models.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/navigation.py` & `nbrisk-35.1.2/nb_risk/navigation.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/tables.py` & `nbrisk-35.1.2/nb_risk/tables.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/template_content.py` & `nbrisk-35.1.2/nb_risk/template_content.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/templates/nb_risk/control.html` & `nbrisk-35.1.2/nb_risk/templates/nb_risk/control.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html` & `nbrisk-35.1.2/nb_risk/templates/nb_risk/generic_vulnerability_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/templates/nb_risk/risk.html` & `nbrisk-35.1.2/nb_risk/templates/nb_risk/risk.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/templates/nb_risk/threatevent.html` & `nbrisk-35.1.2/nb_risk/templates/nb_risk/threatevent.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/templates/nb_risk/threatsource.html` & `nbrisk-35.1.2/nb_risk/templates/nb_risk/threatsource.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability.html` & `nbrisk-35.1.2/nb_risk/templates/nb_risk/vulnerability.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/templates/nb_risk/vulnerability_search.html` & `nbrisk-35.1.2/nb_risk/templates/nb_risk/vulnerability_search.html`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/tests/custom.py` & `nbrisk-35.1.2/nb_risk/tests/custom.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/tests/threatsource/test_api.py` & `nbrisk-35.1.2/nb_risk/tests/threatsource/test_api.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/tests/threatsource/test_filters.py` & `nbrisk-35.1.2/nb_risk/tests/threatsource/test_filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/tests/threatsource/test_views.py` & `nbrisk-35.1.2/nb_risk/tests/threatsource/test_views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/tests/vulnerability/test_filters.py` & `nbrisk-35.1.2/nb_risk/tests/vulnerability/test_filters.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/tests/vulnerability/test_views.py` & `nbrisk-35.1.2/nb_risk/tests/vulnerability/test_views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/urls.py` & `nbrisk-35.1.2/nb_risk/urls.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/nb_risk/views.py` & `nbrisk-35.1.2/nb_risk/views.py`

 * *Files identical despite different names*

### Comparing `NbRisk-35.1.1/setup.py` & `nbrisk-35.1.2/setup.py`

 * *Files identical despite different names*

