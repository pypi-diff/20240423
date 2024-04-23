# Comparing `tmp/tendril_interests-0.6.0.tar.gz` & `tmp/tendril_interests-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_interests-0.6.0.tar", last modified: Tue Apr 16 18:43:30 2024, max compression
+gzip compressed data, was "tendril_interests-0.6.1.tar", last modified: Tue Apr 23 06:24:10 2024, max compression
```

## Comparing `tendril_interests-0.6.0.tar` & `tendril_interests-0.6.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.595836 tendril_interests-0.6.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5728 2024-04-16 18:43:30.595836 tendril_interests-0.6.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_interests-0.6.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-16 18:43:30.599836 tendril_interests-0.6.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3589 2024-04-16 18:42:17.000000 tendril_interests-0.6.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.555837 tendril_interests-0.6.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.559837 tendril_interests-0.6.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.6.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/apiserver/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/apiserver/routers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/routers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4661 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/routers/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/apiserver/templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2023-08-18 07:16:44.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    21600 2024-04-05 09:10:59.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7508 2023-08-11 05:59:31.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1498 2024-04-15 15:41:13.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_graphs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2942 2023-08-22 05:43:50.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3414 2024-03-29 16:57:52.000000 tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.563837 tendril_interests-0.6.0/src/tendril/authz/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril_interests-0.6.0/src/tendril/authz/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/authz/approvals/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril_interests-0.6.0/src/tendril/authz/approvals/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril_interests-0.6.0/src/tendril/authz/approvals/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      936 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/authz/approvals/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/authz/roles/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril_interests-0.6.0/src/tendril/authz/roles/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13891 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/authz/roles/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril_interests-0.6.0/src/tendril/authz/roles/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      362 2024-03-26 07:23:29.000000 tendril_interests-0.6.0/src/tendril/authz/roles/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/authz/scopes/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril_interests-0.6.0/src/tendril/authz/scopes/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/authz/scopes/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.567837 tendril_interests-0.6.0/src/tendril/common/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/common/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/common/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/common/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril_interests-0.6.0/src/tendril/common/interests/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril_interests-0.6.0/src/tendril/common/interests/exceptions.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8613 2023-07-20 19:30:39.000000 tendril_interests-0.6.0/src/tendril/common/interests/memberships.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-08-07 18:32:43.000000 tendril_interests-0.6.0/src/tendril/common/interests/representations.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril_interests-0.6.0/src/tendril/common/states.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril_interests-0.6.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1749 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/config/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_interests-0.6.0/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/core/topology/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_interests-0.6.0/src/tendril/core/topology/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      363 2024-04-16 18:10:38.000000 tendril_interests-0.6.0/src/tendril/core/topology/monitors.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.571837 tendril_interests-0.6.0/src/tendril/db/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.6.0/src/tendril/db/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/db/controllers/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril_interests-0.6.0/src/tendril/db/controllers/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9931 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/db/controllers/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4544 2024-03-26 04:43:47.000000 tendril_interests-0.6.0/src/tendril/db/controllers/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3426 2024-03-29 16:32:48.000000 tendril_interests-0.6.0/src/tendril/db/controllers/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/db/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril_interests-0.6.0/src/tendril/db/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril_interests-0.6.0/src/tendril/db/mixins/interests.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/db/models/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril_interests-0.6.0/src/tendril/db/models/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4996 2024-03-26 05:37:17.000000 tendril_interests-0.6.0/src/tendril/db/models/interests.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril_interests-0.6.0/src/tendril/db/models/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1282 2024-03-26 05:36:15.000000 tendril_interests-0.6.0/src/tendril/db/models/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.575837 tendril_interests-0.6.0/src/tendril/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril_interests-0.6.0/src/tendril/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    20607 2024-03-26 07:48:05.000000 tendril_interests-0.6.0/src/tendril/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8346 2024-04-10 20:05:40.000000 tendril_interests-0.6.0/src/tendril/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.579837 tendril_interests-0.6.0/src/tendril/interests/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17963 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      472 2023-08-09 04:17:18.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5947 2024-04-05 09:10:45.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/export.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3044 2024-04-15 11:57:14.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/graphs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2492 2024-04-05 09:09:51.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/localizers.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    20185 2024-04-16 18:31:53.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4396 2024-04-01 10:19:01.000000 tendril_interests-0.6.0/src/tendril/interests/mixins/policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.579837 tendril_interests-0.6.0/src/tendril/libraries/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril_interests-0.6.0/src/tendril/libraries/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.579837 tendril_interests-0.6.0/src/tendril/libraries/interests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril_interests-0.6.0/src/tendril/libraries/interests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5996 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/libraries/interests/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2845 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/libraries/interests/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.583837 tendril_interests-0.6.0/src/tendril/libraries/mixins/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_approvals.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2024-04-09 21:11:30.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_graphs.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      198 2023-08-12 09:54:17.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_monitors.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      192 2024-03-26 09:21:29.000000 tendril_interests-0.6.0/src/tendril/libraries/mixins/interests_policies.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.583837 tendril_interests-0.6.0/src/tendril/monitors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril_interests-0.6.0/src/tendril/monitors/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7723 2023-09-18 05:12:31.000000 tendril_interests-0.6.0/src/tendril/monitors/spec.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.587837 tendril_interests-0.6.0/src/tendril/policies/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      238 2023-10-31 15:16:36.000000 tendril_interests-0.6.0/src/tendril/policies/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2024-04-01 08:59:10.000000 tendril_interests-0.6.0/src/tendril/policies/base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2166 2024-03-27 02:50:01.000000 tendril_interests-0.6.0/src/tendril/policies/manager.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.587837 tendril_interests-0.6.0/src/tendril_interests.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5728 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3368 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      736 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-16 18:43:30.000000 tendril_interests-0.6.0/src/tendril_interests.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:43:30.587837 tendril_interests-0.6.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril_interests-0.6.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.130798 tendril_interests-0.6.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5728 2024-04-23 06:24:10.130798 tendril_interests-0.6.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2224 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.098798 tendril_interests-0.6.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.102798 tendril_interests-0.6.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.102798 tendril_interests-0.6.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_interests-0.6.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.102798 tendril_interests-0.6.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13464 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1548 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.102798 tendril_interests-0.6.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-23 06:24:10.130798 tendril_interests-0.6.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3589 2024-04-16 18:42:17.000000 tendril_interests-0.6.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.094798 tendril_interests-0.6.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.102798 tendril_interests-0.6.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.6.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.102798 tendril_interests-0.6.1/src/tendril/apiserver/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.6.1/src/tendril/apiserver/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.102798 tendril_interests-0.6.1/src/tendril/apiserver/routers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-17 10:57:31.000000 tendril_interests-0.6.1/src/tendril/apiserver/routers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4661 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/apiserver/routers/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.106798 tendril_interests-0.6.1/src/tendril/apiserver/templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-04-28 03:48:56.000000 tendril_interests-0.6.1/src/tendril/apiserver/templates/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      858 2023-08-18 07:16:44.000000 tendril_interests-0.6.1/src/tendril/apiserver/templates/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    21940 2024-04-23 05:39:18.000000 tendril_interests-0.6.1/src/tendril/apiserver/templates/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7508 2023-08-11 05:59:31.000000 tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1498 2024-04-15 15:41:13.000000 tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2942 2023-08-22 05:43:50.000000 tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3414 2024-03-29 16:57:52.000000 tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.106798 tendril_interests-0.6.1/src/tendril/authz/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-18 15:03:05.000000 tendril_interests-0.6.1/src/tendril/authz/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.106798 tendril_interests-0.6.1/src/tendril/authz/approvals/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      249 2023-07-19 03:39:36.000000 tendril_interests-0.6.1/src/tendril/authz/approvals/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1649 2023-07-19 03:44:45.000000 tendril_interests-0.6.1/src/tendril/authz/approvals/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      936 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/authz/approvals/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.110798 tendril_interests-0.6.1/src/tendril/authz/roles/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-21 10:50:52.000000 tendril_interests-0.6.1/src/tendril/authz/roles/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13891 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/authz/roles/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      620 2023-07-19 07:05:51.000000 tendril_interests-0.6.1/src/tendril/authz/roles/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      362 2024-03-26 07:23:29.000000 tendril_interests-0.6.1/src/tendril/authz/roles/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.110798 tendril_interests-0.6.1/src/tendril/authz/scopes/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      232 2023-02-27 20:56:18.000000 tendril_interests-0.6.1/src/tendril/authz/scopes/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-03-15 16:01:38.000000 tendril_interests-0.6.1/src/tendril/authz/scopes/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.110798 tendril_interests-0.6.1/src/tendril/common/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.6.1/src/tendril/common/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.110798 tendril_interests-0.6.1/src/tendril/common/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-03-15 16:01:38.000000 tendril_interests-0.6.1/src/tendril/common/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3581 2023-07-21 17:21:15.000000 tendril_interests-0.6.1/src/tendril/common/interests/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4287 2023-07-21 16:56:09.000000 tendril_interests-0.6.1/src/tendril/common/interests/exceptions.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9381 2024-04-23 06:19:51.000000 tendril_interests-0.6.1/src/tendril/common/interests/memberships.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      371 2023-08-07 18:32:43.000000 tendril_interests-0.6.1/src/tendril/common/interests/representations.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2023-04-12 09:49:34.000000 tendril_interests-0.6.1/src/tendril/common/states.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.110798 tendril_interests-0.6.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2023-03-15 16:01:38.000000 tendril_interests-0.6.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1749 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/config/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.110798 tendril_interests-0.6.1/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-04 21:22:00.000000 tendril_interests-0.6.1/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.114798 tendril_interests-0.6.1/src/tendril/core/topology/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2024-04-10 10:26:08.000000 tendril_interests-0.6.1/src/tendril/core/topology/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      363 2024-04-16 18:10:38.000000 tendril_interests-0.6.1/src/tendril/core/topology/monitors.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.114798 tendril_interests-0.6.1/src/tendril/db/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:43:23.000000 tendril_interests-0.6.1/src/tendril/db/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.114798 tendril_interests-0.6.1/src/tendril/db/controllers/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:16.000000 tendril_interests-0.6.1/src/tendril/db/controllers/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9931 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/db/controllers/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4544 2024-03-26 04:43:47.000000 tendril_interests-0.6.1/src/tendril/db/controllers/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3426 2024-03-29 16:32:48.000000 tendril_interests-0.6.1/src/tendril/db/controllers/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.114798 tendril_interests-0.6.1/src/tendril/db/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-06-30 15:19:11.000000 tendril_interests-0.6.1/src/tendril/db/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      429 2023-06-30 17:10:42.000000 tendril_interests-0.6.1/src/tendril/db/mixins/interests.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.118798 tendril_interests-0.6.1/src/tendril/db/models/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 08:44:31.000000 tendril_interests-0.6.1/src/tendril/db/models/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4996 2024-03-26 05:37:17.000000 tendril_interests-0.6.1/src/tendril/db/models/interests.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2069 2023-07-21 16:00:50.000000 tendril_interests-0.6.1/src/tendril/db/models/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1282 2024-03-26 05:36:15.000000 tendril_interests-0.6.1/src/tendril/db/models/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.118798 tendril_interests-0.6.1/src/tendril/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      233 2023-02-18 16:44:31.000000 tendril_interests-0.6.1/src/tendril/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    20607 2024-03-26 07:48:05.000000 tendril_interests-0.6.1/src/tendril/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8346 2024-04-10 20:05:40.000000 tendril_interests-0.6.1/src/tendril/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.122798 tendril_interests-0.6.1/src/tendril/interests/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-19 16:39:46.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17963 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      472 2023-08-09 04:17:18.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5947 2024-04-05 09:10:45.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/export.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3044 2024-04-15 11:57:14.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2492 2024-04-05 09:09:51.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/localizers.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    20185 2024-04-16 18:31:53.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4396 2024-04-01 10:19:01.000000 tendril_interests-0.6.1/src/tendril/interests/mixins/policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.122798 tendril_interests-0.6.1/src/tendril/libraries/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-02-16 19:15:51.000000 tendril_interests-0.6.1/src/tendril/libraries/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.122798 tendril_interests-0.6.1/src/tendril/libraries/interests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      237 2023-02-16 22:18:24.000000 tendril_interests-0.6.1/src/tendril/libraries/interests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     6176 2024-04-23 06:19:51.000000 tendril_interests-0.6.1/src/tendril/libraries/interests/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2845 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/libraries/interests/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.122798 tendril_interests-0.6.1/src/tendril/libraries/mixins/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-14 15:54:08.000000 tendril_interests-0.6.1/src/tendril/libraries/mixins/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      418 2023-07-18 18:38:25.000000 tendril_interests-0.6.1/src/tendril/libraries/mixins/interests_approvals.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      190 2024-04-09 21:11:30.000000 tendril_interests-0.6.1/src/tendril/libraries/mixins/interests_graphs.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      198 2023-08-12 09:54:17.000000 tendril_interests-0.6.1/src/tendril/libraries/mixins/interests_monitors.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      192 2024-03-26 09:21:29.000000 tendril_interests-0.6.1/src/tendril/libraries/mixins/interests_policies.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.122798 tendril_interests-0.6.1/src/tendril/monitors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-07-29 05:37:59.000000 tendril_interests-0.6.1/src/tendril/monitors/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7723 2023-09-18 05:12:31.000000 tendril_interests-0.6.1/src/tendril/monitors/spec.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.126798 tendril_interests-0.6.1/src/tendril/policies/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      238 2023-10-31 15:16:36.000000 tendril_interests-0.6.1/src/tendril/policies/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1704 2024-04-01 08:59:10.000000 tendril_interests-0.6.1/src/tendril/policies/base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2166 2024-03-27 02:50:01.000000 tendril_interests-0.6.1/src/tendril/policies/manager.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.126798 tendril_interests-0.6.1/src/tendril_interests.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5728 2024-04-23 06:24:09.000000 tendril_interests-0.6.1/src/tendril_interests.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3368 2024-04-23 06:24:10.000000 tendril_interests-0.6.1/src/tendril_interests.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-23 06:24:09.000000 tendril_interests-0.6.1/src/tendril_interests.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      736 2024-04-23 06:24:09.000000 tendril_interests-0.6.1/src/tendril_interests.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-23 06:24:09.000000 tendril_interests-0.6.1/src/tendril_interests.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-23 06:24:10.126798 tendril_interests-0.6.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2022-12-12 13:44:35.000000 tendril_interests-0.6.1/tox.ini
```

### Comparing `tendril_interests-0.6.0/.gitignore` & `tendril_interests-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/.readthedocs.yml` & `tendril_interests-0.6.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/.travis.yml` & `tendril_interests-0.6.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/LICENSE` & `tendril_interests-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/PKG-INFO` & `tendril_interests-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.6.0
+Version: 0.6.1
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril_interests-0.6.0/README.rst` & `tendril_interests-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/Makefile` & `tendril_interests-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/_static/custom.css` & `tendril_interests-0.6.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/_static/favicon.ico` & `tendril_interests-0.6.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/_static/logo.png` & `tendril_interests-0.6.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/_static/logo_packed.png` & `tendril_interests-0.6.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/_templates/about.html` & `tendril_interests-0.6.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/conf.py` & `tendril_interests-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/index.rst` & `tendril_interests-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/docs/installation.rst` & `tendril_interests-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/setup.py` & `tendril_interests-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/apiserver/routers/interests.py` & `tendril_interests-0.6.1/src/tendril/apiserver/routers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/apiserver/templates/base.py` & `tendril_interests-0.6.1/src/tendril/apiserver/templates/base.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests.py` & `tendril_interests-0.6.1/src/tendril/apiserver/templates/interests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
 
 from typing import List
 from typing import Dict
 from typing import Union
 from typing import Optional
+from typing import Annotated
 from inflection import singularize
 from inflection import titleize
 
 from fastapi import APIRouter
+from fastapi import Query
 from fastapi import Request
 from fastapi import Depends
 from fastapi import BackgroundTasks
 from fastapi.responses import JSONResponse
 
 from tendril.authn.users import auth_spec
 from tendril.authn.users import AuthUserModel
@@ -104,26 +106,31 @@
         """
         with get_session() as session:
             rv = self._actual.item(id=id, session=session).\
                 export(auth_user=user, session=session, export_level=export_level)
         return rv
 
     async def find_possible_parents(self, request: Request,
+                                    search_parent_types : Annotated[list[str] | None, Query()] = None,
+                                    first_only: Optional[bool] = False,
                                     user: AuthUserModel = auth_spec(),
                                     export_level: Optional[ExportLevel] = ExportLevel.STUB.value):
         """
         Get possible parents for new items in this library.
 
         All user memberships in possible parents for this library's interest
         type which allow creation of a child of this type are returned.
 
         - **user :* The requesting user, identified by the access token.
         """
         with get_session() as session:
-            result = self._actual.possible_parents(user=user, session=session)
+            result = self._actual.possible_parents(
+                search_parent_types=search_parent_types,
+                first_only=first_only, user=user, session=session
+            )
             return [x.export(auth_user=user, session=session,
                              export_level=export_level) for x in result]
 
     def _inject_create_model(self, ep):
         return self._inject_model(ep, param='item', model=self._actual.interest_class.tmodel_create)
 
     def create_item(self, item,
```

### Comparing `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_approvals.py` & `tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_graphs.py` & `tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_graphs.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_monitors.py` & `tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_monitors.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/apiserver/templates/interests_policies.py` & `tendril_interests-0.6.1/src/tendril/apiserver/templates/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/authz/approvals/interests.py` & `tendril_interests-0.6.1/src/tendril/authz/approvals/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/authz/approvals/manager.py` & `tendril_interests-0.6.1/src/tendril/authz/approvals/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/authz/roles/interests.py` & `tendril_interests-0.6.1/src/tendril/authz/roles/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/authz/roles/interests_approvals.py` & `tendril_interests-0.6.1/src/tendril/authz/roles/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/common/interests/approvals.py` & `tendril_interests-0.6.1/src/tendril/common/interests/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/common/interests/exceptions.py` & `tendril_interests-0.6.1/src/tendril/common/interests/exceptions.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/common/interests/memberships.py` & `tendril_interests-0.6.1/src/tendril/common/interests/memberships.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,27 +97,41 @@
 
     @with_db
     def _get_interest(self, iid, itype, session=None):
         interest_type = interests.type_codes[itype]
         return interest_type(get_interest(id=iid, type=interest_type.model, session=session))
 
     @with_db
-    def interests(self, filter_criteria=None, sort_heuristics=None, session=None):
+    def interests(self, filter_criteria=None, sort_heuristics=None, first_only=False, session=None):
         if not self.df.select(polars.count()).item():
             return []
         i_itype = self.df.select(polars.col(['interest.id', 'type'])).unique()
         cand_interests = [self._get_interest(iid=iid, itype=type_name, session=session)
                           for iid, type_name in i_itype.rows()]
+
+        if first_only:
+            # This is a highly specific optimization for use cases where it is only needed to
+            # know _if_ there are any possible_parents accessible to the user. This is used by
+            # the frontend in places where we need to decide what options to provide. In most cases,
+            # the user will need the full list later on. So, if the underlying list processing
+            # can be optimized, this special case could perhaps be removed.
+            if not filter_criteria:
+                return [cand_interests[0]]
+            for cand_interest in cand_interests:
+                if all([getattr(cand_interest, acc)(**kw) for acc, kw in filter_criteria]):
+                    return [cand_interest]
+
         if filter_criteria:
             cand_interests = [x for x in cand_interests
                               if all([getattr(x, acc)(**kw) for acc, kw in filter_criteria])]
         if sort_heuristics:
             for acc, reflist in sort_heuristics:
                 ranks = dict((value, idx) for idx, value in enumerate(reflist))
                 cand_interests = sorted(cand_interests, key=lambda x: ranks[x.type_name])
+
         return cand_interests
 
 
 def _rewrap_interest(model):
     type_name = model.type
     return interests.type_codes[type_name](model)
```

### Comparing `tendril_interests-0.6.0/src/tendril/config/__init__.py` & `tendril_interests-0.6.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/config/interests.py` & `tendril_interests-0.6.1/src/tendril/config/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/db/controllers/interests.py` & `tendril_interests-0.6.1/src/tendril/db/controllers/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/db/controllers/interests_approvals.py` & `tendril_interests-0.6.1/src/tendril/db/controllers/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/db/controllers/interests_policies.py` & `tendril_interests-0.6.1/src/tendril/db/controllers/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/db/models/interests.py` & `tendril_interests-0.6.1/src/tendril/db/models/interests.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/db/models/interests_approvals.py` & `tendril_interests-0.6.1/src/tendril/db/models/interests_approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/db/models/interests_policies.py` & `tendril_interests-0.6.1/src/tendril/db/models/interests_policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/base.py` & `tendril_interests-0.6.1/src/tendril/interests/base.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/manager.py` & `tendril_interests-0.6.1/src/tendril/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/mixins/approvals.py` & `tendril_interests-0.6.1/src/tendril/interests/mixins/approvals.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/mixins/export.py` & `tendril_interests-0.6.1/src/tendril/interests/mixins/export.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/mixins/graphs.py` & `tendril_interests-0.6.1/src/tendril/interests/mixins/graphs.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/mixins/localizers.py` & `tendril_interests-0.6.1/src/tendril/interests/mixins/localizers.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/mixins/monitors.py` & `tendril_interests-0.6.1/src/tendril/interests/mixins/monitors.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/interests/mixins/policies.py` & `tendril_interests-0.6.1/src/tendril/interests/mixins/policies.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/libraries/interests/base.py` & `tendril_interests-0.6.1/src/tendril/libraries/interests/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,24 +95,26 @@
         return created
 
     @with_db
     def delete_item(self, id=None, name=None, session=None):
         raise NotImplementedError
 
     @with_db
-    def possible_parents(self, user=None, session=None):
+    def possible_parents(self, user=None, search_parent_types=None, first_only=False, session=None):
         parent_types = interests.possible_parents[self.type_name]
         if self.type_name in self.interest_class.model.role_spec.allowed_children:
             parent_types.append(self.type_name)
+        if search_parent_types:
+            parent_types = [x for x in parent_types if x in search_parent_types]
         candidate_memberships = user_memberships(user_id=user, interest_types=parent_types,
                                                  session=session)
         candidate_interests = candidate_memberships.interests(
             filter_criteria=[('check_user_access', {'user': user, 'session': session,
                                                     'action': f'add_child:{self.type_name}'})],
-            sort_heuristics=[('type_name', parent_types)])
+            sort_heuristics=[('type_name', parent_types)], first_only=first_only)
         return candidate_interests
 
     @property
     def additional_api_generators(self):
         try:
             mro = list(self.__class__.__mro__)
         except AttributeError:
```

### Comparing `tendril_interests-0.6.0/src/tendril/libraries/interests/manager.py` & `tendril_interests-0.6.1/src/tendril/libraries/interests/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/monitors/spec.py` & `tendril_interests-0.6.1/src/tendril/monitors/spec.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/policies/base.py` & `tendril_interests-0.6.1/src/tendril/policies/base.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril/policies/manager.py` & `tendril_interests-0.6.1/src/tendril/policies/manager.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril_interests.egg-info/PKG-INFO` & `tendril_interests-0.6.1/src/tendril_interests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-interests
-Version: 0.6.0
+Version: 0.6.1
 Summary: Core Tendril Infrastructure for User Mapped Entitites
 Home-page: https://github.com/tendril-framework/tendril-interests
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-interests.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-interests/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-interests
```

### Comparing `tendril_interests-0.6.0/src/tendril_interests.egg-info/SOURCES.txt` & `tendril_interests-0.6.1/src/tendril_interests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/src/tendril_interests.egg-info/requires.txt` & `tendril_interests-0.6.1/src/tendril_interests.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/tests/coveralls.py` & `tendril_interests-0.6.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_interests-0.6.0/tox.ini` & `tendril_interests-0.6.1/tox.ini`

 * *Files identical despite different names*

