# Comparing `tmp/disdat-1.0.2.tar.gz` & `tmp/disdat-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disdat-1.0.2.tar", last modified: Sat Mar  9 23:43:10 2024, max compression
+gzip compressed data, was "disdat-1.1.0.tar", last modified: Tue Apr 23 00:44:27 2024, max compression
```

## Comparing `disdat-1.0.2.tar` & `disdat-1.1.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.384588 disdat-1.0.2/
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.338472 disdat-1.0.2/.github/
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.350643 disdat-1.0.2/.github/workflows/
--rwxrwxrwx   0 kyocum     (503) staff       (20)     1538 2021-06-18 01:03:37.000000 disdat-1.0.2/.github/workflows/python-publish.yml
--rwxrwxrwx   0 kyocum     (503) staff       (20)      106 2021-06-18 01:03:37.000000 disdat-1.0.2/.gitignore
--rwxrwxrwx   0 kyocum     (503) staff       (20)    11388 2018-01-16 21:55:45.000000 disdat-1.0.2/LICENSE.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)      164 2022-01-20 01:37:06.000000 disdat-1.0.2/MANIFEST.in
--rwxrwxrwx   0 kyocum     (503) staff       (20)      661 2022-01-20 01:37:06.000000 disdat-1.0.2/NOTICE.txt
--rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-03-09 23:43:10.384202 disdat-1.0.2/PKG-INFO
--rwxrwxrwx   0 kyocum     (503) staff       (20)     2230 2022-04-18 17:07:06.000000 disdat-1.0.2/README.rst
--rwxr-xr-x   0 kyocum     (503) staff       (20)      575 2024-03-09 23:18:32.000000 disdat-1.0.2/build-dist.sh
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.360680 disdat-1.0.2/disdat/
--rwxrwxrwx   0 kyocum     (503) staff       (20)       18 2022-01-07 19:22:09.000000 disdat-1.0.2/disdat/.gitignore
--rw-r--r--   0 kyocum     (503) staff       (20)      739 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2027 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/add.py
--rw-r--r--   0 kyocum     (503) staff       (20)    50170 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/api.py
--rw-r--r--   0 kyocum     (503) staff       (20)     8251 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/common.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.364745 disdat-1.0.2/disdat/config/
--rwxrwxrwx   0 kyocum     (503) staff       (20)       85 2022-01-07 19:22:09.000000 disdat-1.0.2/disdat/config/README.md
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.0.2/disdat/config/__init__.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.365711 disdat-1.0.2/disdat/config/disdat/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.0.2/disdat/config/disdat/.exclude-from-modeler-docker-image
--rwxrwxrwx   0 kyocum     (503) staff       (20)       70 2022-01-20 01:37:06.000000 disdat-1.0.2/disdat/config/disdat/disdat.cfg
--rw-r--r--   0 kyocum     (503) staff       (20)      702 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/constants.py
--rw-r--r--   0 kyocum     (503) staff       (20)    55549 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/data_context.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.366157 disdat-1.0.2/disdat/entrypoints/
--rw-r--r--   0 kyocum     (503) staff       (20)     4015 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/entrypoints/cli_ep.py
--rw-r--r--   0 kyocum     (503) staff       (20)      589 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/exceptions.py
--rw-r--r--   0 kyocum     (503) staff       (20)    67262 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/fs.py
--rw-r--r--   0 kyocum     (503) staff       (20)    73610 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/hyperframe.py
--rw-r--r--   0 kyocum     (503) staff       (20)    56763 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/hyperframe_pb2.py
--rw-r--r--   0 kyocum     (503) staff       (20)     4480 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/lineage.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2129 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/log.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1899 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/resource.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.367120 disdat-1.0.2/disdat/utility/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-20 01:37:06.000000 disdat-1.0.2/disdat/utility/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)    19080 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/utility/aws_s3.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1623 2024-03-09 22:00:21.000000 disdat-1.0.2/disdat/utility/bundle_helpers.py
--rwxrwxrwx   0 kyocum     (503) staff       (20)       21 2024-03-09 23:43:10.000000 disdat-1.0.2/disdat/version.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.363841 disdat-1.0.2/disdat.egg-info/
--rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-03-09 23:43:10.000000 disdat-1.0.2/disdat.egg-info/PKG-INFO
--rwxrwxrwx   0 kyocum     (503) staff       (20)     1996 2024-03-09 23:43:10.000000 disdat-1.0.2/disdat.egg-info/SOURCES.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)        1 2024-03-09 23:43:10.000000 disdat-1.0.2/disdat.egg-info/dependency_links.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)       56 2024-03-09 23:43:10.000000 disdat-1.0.2/disdat.egg-info/entry_points.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)      234 2024-03-09 23:43:10.000000 disdat-1.0.2/disdat.egg-info/requires.txt
--rwxrwxrwx   0 kyocum     (503) staff       (20)        7 2024-03-09 23:43:10.000000 disdat-1.0.2/disdat.egg-info/top_level.txt
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.367484 disdat-1.0.2/docs/
--rwxrwxrwx   0 kyocum     (503) staff       (20)     5120 2021-06-18 01:03:37.000000 disdat-1.0.2/docs/DisdatTitleFig.jpg
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.367797 disdat-1.0.2/infrastructure/
--rwxrwxrwx   0 kyocum     (503) staff       (20)      754 2022-01-20 01:37:06.000000 disdat-1.0.2/infrastructure/.gitignore
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.368075 disdat-1.0.2/infrastructure/Dockerfiles/
--rwxrwxrwx   0 kyocum     (503) staff       (20)      292 2022-01-20 01:37:06.000000 disdat-1.0.2/infrastructure/Dockerfiles/Makefile
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.369573 disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/
--rwxrwxrwx   0 kyocum     (503) staff       (20)      285 2022-01-20 01:37:06.000000 disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/Dockerfile
--rwxrwxrwx   0 kyocum     (503) staff       (20)      270 2022-01-20 01:37:06.000000 disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/Makefile
--rwxrwxrwx   0 kyocum     (503) staff       (20)      264 2022-01-20 01:37:06.000000 disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/README.md
--rwxrwxrwx   0 kyocum     (503) staff       (20)     2327 2022-01-20 01:37:06.000000 disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/bundle.proto
--rwxrwxrwx   0 kyocum     (503) staff       (20)     6190 2022-01-20 01:37:06.000000 disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto
--rw-r--r--   0 kyocum     (503) staff       (20)       38 2024-03-09 23:43:10.384651 disdat-1.0.2/setup.cfg
--rw-r--r--   0 kyocum     (503) staff       (20)     3804 2024-03-09 22:00:21.000000 disdat-1.0.2/setup.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.370277 disdat-1.0.2/tests/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.0.2/tests/__init__.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.371485 disdat-1.0.2/tests/bundles/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2020-05-15 07:06:53.000000 disdat-1.0.2/tests/bundles/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1332 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/bundles/test_arg_capture.py
--rw-r--r--   0 kyocum     (503) staff       (20)     4739 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/bundles/test_file_bundle_api.py
--rw-r--r--   0 kyocum     (503) staff       (20)    11110 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/bundles/test_hframe.py
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.376706 disdat-1.0.2/tests/data/
--rwxrwxrwx   0 kyocum     (503) staff       (20)  8918348 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/US_chronic_disease_indicators_CDI_2012.csv
--rwxrwxrwx   0 kyocum     (503) staff       (20)      485 2019-05-18 00:15:09.000000 disdat-1.0.2/tests/data/test_bundle_file.csv
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.379506 disdat-1.0.2/tests/data/testfiles/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/A
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/B
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/C
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/D
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/E
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/F
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/G
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/H
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/I
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.0.2/tests/data/testfiles/J
-drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-03-09 23:43:10.382990 disdat-1.0.2/tests/functional/
--rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.0.2/tests/functional/__init__.py
--rw-r--r--   0 kyocum     (503) staff       (20)      398 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/common.py
--rw-r--r--   0 kyocum     (503) staff       (20)     7255 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_add.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2710 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_add_remote.py
--rw-r--r--   0 kyocum     (503) staff       (20)     2159 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_cat.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1742 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_context.py
--rw-r--r--   0 kyocum     (503) staff       (20)     1067 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_hyperframe.py
--rw-r--r--   0 kyocum     (503) staff       (20)     8793 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_link_localization.py
--rw-r--r--   0 kyocum     (503) staff       (20)     4157 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_output_types.py
--rw-r--r--   0 kyocum     (503) staff       (20)     3109 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/functional/test_remote.py
--rw-r--r--   0 kyocum     (503) staff       (20)      217 2024-03-09 22:00:21.000000 disdat-1.0.2/tests/setup.py
--rw-r--r--   0 kyocum     (503) staff       (20)      736 2024-03-09 22:00:21.000000 disdat-1.0.2/tox.ini
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.799659 disdat-1.1.0/
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.746262 disdat-1.1.0/.github/
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.755483 disdat-1.1.0/.github/workflows/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     1538 2021-06-18 01:03:37.000000 disdat-1.1.0/.github/workflows/python-publish.yml
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      106 2021-06-18 01:03:37.000000 disdat-1.1.0/.gitignore
+-rwxrwxrwx   0 kyocum     (503) staff       (20)    11388 2018-01-16 21:55:45.000000 disdat-1.1.0/LICENSE.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      164 2022-01-20 01:37:06.000000 disdat-1.1.0/MANIFEST.in
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      661 2022-01-20 01:37:06.000000 disdat-1.1.0/NOTICE.txt
+-rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-04-23 00:44:27.798350 disdat-1.1.0/PKG-INFO
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     2230 2022-04-18 17:07:06.000000 disdat-1.1.0/README.rst
+-rwxr-xr-x   0 kyocum     (503) staff       (20)      575 2024-03-09 23:18:32.000000 disdat-1.1.0/build-dist.sh
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.763751 disdat-1.1.0/disdat/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       18 2022-01-07 19:22:09.000000 disdat-1.1.0/disdat/.gitignore
+-rw-r--r--   0 kyocum     (503) staff       (20)      739 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2027 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/add.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    50178 2024-04-23 00:27:52.000000 disdat-1.1.0/disdat/api.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     8241 2024-04-23 00:27:52.000000 disdat-1.1.0/disdat/common.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.769657 disdat-1.1.0/disdat/config/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       85 2022-01-07 19:22:09.000000 disdat-1.1.0/disdat/config/README.md
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.1.0/disdat/config/__init__.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.770821 disdat-1.1.0/disdat/config/disdat/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-07 19:22:09.000000 disdat-1.1.0/disdat/config/disdat/.exclude-from-modeler-docker-image
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       70 2022-01-20 01:37:06.000000 disdat-1.1.0/disdat/config/disdat/disdat.cfg
+-rw-r--r--   0 kyocum     (503) staff       (20)      702 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/constants.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    55557 2024-04-23 00:27:52.000000 disdat-1.1.0/disdat/data_context.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.771284 disdat-1.1.0/disdat/entrypoints/
+-rw-r--r--   0 kyocum     (503) staff       (20)     4015 2024-04-18 00:02:53.000000 disdat-1.1.0/disdat/entrypoints/cli_ep.py
+-rw-r--r--   0 kyocum     (503) staff       (20)      589 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/exceptions.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    67416 2024-04-23 00:27:52.000000 disdat-1.1.0/disdat/fs.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    73618 2024-04-23 00:27:52.000000 disdat-1.1.0/disdat/hyperframe.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    56763 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/hyperframe_pb2.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     4480 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/lineage.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2129 2024-04-17 22:38:16.000000 disdat-1.1.0/disdat/log.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1899 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/resource.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.772767 disdat-1.1.0/disdat/utility/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2022-01-20 01:37:06.000000 disdat-1.1.0/disdat/utility/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    17841 2024-04-23 00:38:16.000000 disdat-1.1.0/disdat/utility/asyncio_aws_s3.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1623 2024-04-17 16:18:22.000000 disdat-1.1.0/disdat/utility/bundle_helpers.py
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       21 2024-04-23 00:44:27.000000 disdat-1.1.0/disdat/version.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.797070 disdat-1.1.0/disdat.egg-info/
+-rw-r--r--   0 kyocum     (503) staff       (20)     1275 2024-04-23 00:44:27.000000 disdat-1.1.0/disdat.egg-info/PKG-INFO
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     2004 2024-04-23 00:44:27.000000 disdat-1.1.0/disdat.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        1 2024-04-23 00:44:27.000000 disdat-1.1.0/disdat.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)       56 2024-04-23 00:44:27.000000 disdat-1.1.0/disdat.egg-info/entry_points.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      234 2024-04-23 00:44:27.000000 disdat-1.1.0/disdat.egg-info/requires.txt
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        7 2024-04-23 00:44:27.000000 disdat-1.1.0/disdat.egg-info/top_level.txt
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.773218 disdat-1.1.0/docs/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     5120 2021-06-18 01:03:37.000000 disdat-1.1.0/docs/DisdatTitleFig.jpg
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.773798 disdat-1.1.0/infrastructure/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      754 2022-01-20 01:37:06.000000 disdat-1.1.0/infrastructure/.gitignore
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.774290 disdat-1.1.0/infrastructure/Dockerfiles/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      292 2022-01-20 01:37:06.000000 disdat-1.1.0/infrastructure/Dockerfiles/Makefile
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.776706 disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      285 2022-01-20 01:37:06.000000 disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/Dockerfile
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      270 2022-01-20 01:37:06.000000 disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/Makefile
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      264 2022-01-20 01:37:06.000000 disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/README.md
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     2327 2022-01-20 01:37:06.000000 disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/bundle.proto
+-rwxrwxrwx   0 kyocum     (503) staff       (20)     6190 2022-01-20 01:37:06.000000 disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto
+-rw-r--r--   0 kyocum     (503) staff       (20)       38 2024-04-23 00:44:27.799723 disdat-1.1.0/setup.cfg
+-rw-r--r--   0 kyocum     (503) staff       (20)     3804 2024-04-17 16:18:22.000000 disdat-1.1.0/setup.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.777604 disdat-1.1.0/tests/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.1.0/tests/__init__.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.779635 disdat-1.1.0/tests/bundles/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2020-05-15 07:06:53.000000 disdat-1.1.0/tests/bundles/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1332 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/bundles/test_arg_capture.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     4752 2024-04-23 00:27:52.000000 disdat-1.1.0/tests/bundles/test_file_bundle_api.py
+-rw-r--r--   0 kyocum     (503) staff       (20)    11110 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/bundles/test_hframe.py
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.786348 disdat-1.1.0/tests/data/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)  8918348 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/US_chronic_disease_indicators_CDI_2012.csv
+-rwxrwxrwx   0 kyocum     (503) staff       (20)      485 2019-05-18 00:15:09.000000 disdat-1.1.0/tests/data/test_bundle_file.csv
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.791399 disdat-1.1.0/tests/data/testfiles/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/A
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/B
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/C
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/D
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/E
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/F
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/G
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/H
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/I
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2018-01-16 21:55:45.000000 disdat-1.1.0/tests/data/testfiles/J
+drwxr-xr-x   0 kyocum     (503) staff       (20)        0 2024-04-23 00:44:27.796179 disdat-1.1.0/tests/functional/
+-rwxrwxrwx   0 kyocum     (503) staff       (20)        0 2019-02-25 22:58:22.000000 disdat-1.1.0/tests/functional/__init__.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     3201 2024-04-23 00:27:52.000000 disdat-1.1.0/tests/functional/common.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     7255 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/functional/test_add.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2695 2024-04-23 00:27:52.000000 disdat-1.1.0/tests/functional/test_add_remote.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     2159 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/functional/test_cat.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1742 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/functional/test_context.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     1067 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/functional/test_hyperframe.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     8801 2024-04-23 00:27:52.000000 disdat-1.1.0/tests/functional/test_link_localization.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     4157 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/functional/test_output_types.py
+-rw-r--r--   0 kyocum     (503) staff       (20)     3109 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/functional/test_remote.py
+-rw-r--r--   0 kyocum     (503) staff       (20)      217 2024-04-17 16:18:22.000000 disdat-1.1.0/tests/setup.py
+-rw-r--r--   0 kyocum     (503) staff       (20)      736 2024-04-17 16:18:22.000000 disdat-1.1.0/tox.ini
```

### Comparing `disdat-1.0.2/.github/workflows/python-publish.yml` & `disdat-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/LICENSE.txt` & `disdat-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/NOTICE.txt` & `disdat-1.1.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/PKG-INFO` & `disdat-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdat
-Version: 1.0.2
+Version: 1.1.0
 Summary: Disdat: data versioning
 Home-page: https://github.com/kyocum/disdat
 Author: Ken Yocum
 Author-email: kyocum@gmail.com
 License: Apache License, version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `disdat-1.0.2/README.rst` & `disdat-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/build-dist.sh` & `disdat-1.1.0/build-dist.sh`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/__init__.py` & `disdat-1.1.0/disdat/__init__.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/add.py` & `disdat-1.1.0/disdat/add.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/api.py` & `disdat-1.1.0/disdat/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import urllib
 
 import disdat.common as common
 import disdat.fs
 from disdat import logger as _logger
 from disdat.data_context import DataContext
 from disdat.hyperframe import HyperFrameRecord, LineageRecord, parse_return_val
-from disdat.utility.aws_s3 import s3_path_exists
+from disdat.utility.asyncio_aws_s3 import s3_path_exists
 
 PROC_ID_TRUNCATE_HASH = 10  # 10 ls hex digits
 
 
 def _get_fs():
     """Initializing FS, which needs a config.
     These are both singletons.
```

### Comparing `disdat-1.0.2/disdat/common.py` & `disdat-1.1.0/disdat/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import configparser
 import importlib
 import logging
 import os
 import shutil
 import sys
+import urllib
 import uuid
 
-from six.moves import configparser, urllib
-
 import disdat.config
 from disdat import logger as _logger
 from disdat import resource
 
 SYSTEM_CONFIG_DIR = "~/.config/disdat"
 PACKAGE_CONFIG_DIR = "disdat"
 LOGGING_FILE = "logging.conf"
```

### Comparing `disdat-1.0.2/disdat/constants.py` & `disdat-1.1.0/disdat/constants.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/data_context.py` & `disdat-1.1.0/disdat/data_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import pandas as pd
 from sqlalchemy import create_engine
 
 import disdat.common as common
 import disdat.constants as constants
 import disdat.hyperframe as hyperframe
 import disdat.hyperframe_pb2 as hyperframe_pb2
-import disdat.utility.aws_s3 as aws_s3
+import disdat.utility.asyncio_aws_s3 as aws_s3
 from disdat import logger as _logger
 from disdat.common import DisdatConfig
 
 META_CTXT_FILE = "ctxt.json"
 DB_FILE = "ctxt.db"
 DEFAULT_LEN_UNCOMMITTED_HISTORY = 1
```

### Comparing `disdat-1.0.2/disdat/entrypoints/cli_ep.py` & `disdat-1.1.0/disdat/entrypoints/cli_ep.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/exceptions.py` & `disdat-1.1.0/disdat/exceptions.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/fs.py` & `disdat-1.1.0/disdat/fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from datetime import datetime
 from enum import Enum
 
 import pandas as pd
 
 import disdat.common as common
 import disdat.hyperframe as hyperframe
-import disdat.utility.aws_s3 as aws_s3
+import disdat.utility.asyncio_aws_s3 as aws_s3
 from disdat import logger as _logger
 from disdat.common import CatNoBundleError, DisdatConfig
 from disdat.data_context import DataContext
 
 CodeVersion = collections.namedtuple(
     "CodeVersion", "semver hash tstamp branch url dirty"
 )
@@ -80,23 +80,22 @@
         with open(os.devnull, "w") as null_file:
             output = subprocess.call(cmd, stdout=null_file, stderr=null_file)
 
     output = str(output)
 
     return output
 
-
-def determine_pipe_version(pipe_root):
     """
+def determine_pipe_version(pipe_root):
     Given a pipe file path, return the repo status. If they are set, use the environment variables,
     otherwise run the git commands.
 
+
     Args:
         pipe_root: path to the root of the pipeline
-
     Returns:
         CodeVersion: populated object with the git hash, branch, fetch url, last updated date
         and "dirty" status. A pipeline is considered to be dirty if there are modified files
         which haven't been checked in yet.
     """
 
     def _get_git_info_var(var_name, git_command):
@@ -547,15 +546,15 @@
 
         Returns:
 
         """
         if data_context is None:
             data_context = self.curr_context
             if data_context is None:
-                print("No current context.  `dsdt switch <othercontext>`")
+                _logger.info("No current context.  `dsdt switch <othercontext>`")
                 return None
         return data_context
 
     def ls(
         self,
         search_name,
         print_tags,
@@ -724,15 +723,15 @@
         else:
             hfr = self.get_hframe_by_uuid(uuid, tags=tags, data_context=data_context)
 
         if hfr is not None:
             other = data_context.present_hfr(hfr)
             if file is not None:
                 df = data_context.convert_hfr2df(hfr)
-                print("Saving to file {}".format(file))
+                _logger.info("Saving to file {}".format(file))
                 df.to_csv(file, sep=",", index=False)
             return other
         else:
             raise CatNoBundleError(
                 "No bundle found with name({}) uuid({})".format(human_name, uuid)
             )
 
@@ -895,15 +894,15 @@
         ctxt_dir = os.path.join(
             DisdatConfig.instance().get_context_dir(), local_context
         )
 
         if self.curr_context is not None and (
             fq_context_name == self.curr_context_name
         ):
-            print(
+            _logger.info(
                 "Disdat deleting the current context {}, remember to 'dsdt switch <otherbranch>' afterwords!".format(
                     fq_context_name
                 )
             )
             os.remove(
                 os.path.join(DisdatConfig.instance().get_meta_dir(), META_FS_FILE)
             )
@@ -979,17 +978,17 @@
                 )
             )
 
         new_context = self.get_context(local_context_name)
 
         if new_context is not None:
             self.curr_context = new_context
-            print("Switched to context {}".format(self.curr_context_name))
+            _logger.info("Switched to context {}".format(self.curr_context_name))
         else:
-            print("In context {}".format(self.curr_context_name))
+            _logger.info("In context {}".format(self.curr_context_name))
 
     def commit(self, bundle_name, input_tags, uuid=None, data_context=None):
         """Commit indicates that this is a primary version of this bundle.
 
         Commit in place.  Re-use existing bundle and add the commit tag.
         Database links are special.  Commits materialize special views of the physical table.
 
@@ -1021,30 +1020,30 @@
         elif bundle_name is not None:
             hfr = self.get_latest_hframe(
                 str(bundle_name),
                 tags=input_tags if len(input_tags) > 0 else None,
                 data_context=data_context,
             )
         else:
-            print(
+            _logger.warn(
                 "Push requires either a human name or a uuid to identify the hyperframe."
             )
             return None
 
         if hfr is None:
-            print(
+            _logger.info(
                 "No bundle with human name [{}] or uuid [{}] found.".format(
                     bundle_name, uuid
                 )
             )
             return
 
         commit_tag = hfr.get_tag("committed")
         if commit_tag is not None and commit_tag == "True":
-            print(
+            _logger.info(
                 "Bundle human name [{}] uuid [{}] already committed.".format(
                     hfr.pb.human_name, hfr.pb.uuid
                 )
             )
             return
 
         tags = {"committed": "True"}
@@ -1218,15 +1217,15 @@
         """
 
         data_context = self.ensure_data_context(data_context)
         if data_context is None:
             return None
 
         if data_context.remote_ctxt_url is None:
-            print(
+            _logger.info(
                 "Push cannot execute.  Local context {} on remote {} not bound.".format(
                     data_context.local_ctxt, data_context.remote_ctxt
                 )
             )
             return None
 
         if tags is None:
@@ -1241,21 +1240,21 @@
         if uuid is not None:
             hfr = self.get_hframe_by_uuid(uuid, tags=tags, data_context=data_context)
         elif human_name is not None:
             hfr = self.get_latest_hframe(
                 human_name, tags=tags, data_context=data_context
             )
         else:
-            print(
+            _logger.info(
                 "Push requires either a human name or a uuid to identify the hyperframe."
             )
             return None
 
         if hfr is None:
-            print(
+            _logger.info(
                 "Push unable to find committed bundle name [{}] uuid [{}]".format(
                     human_name, uuid
                 )
             )
             return None
 
         # All bundles contain relative paths.  Copying is a simple
@@ -1263,29 +1262,29 @@
         to_delete = []
         try:
             src_dst_copies = self._copy_hfr_to_remote_branch(hfr, data_context)
             for src, dst in src_dst_copies:
                 if not hyperframe.is_hyperframe_pb_file(src):
                     to_delete.append(urllib.parse.urlparse(src).path)
         except Exception as e:
-            print("Push unable to copy bundle to branch: {}".format(e))
+            _logger.warn("Push unable to copy bundle to branch: {}".format(e))
             return None
 
         if delocalize:
             for f in to_delete:
                 try:
                     os.remove(f)
                 except IOError as e:
-                    print(
+                    _logger.warn(
                         "fast_push: during delocalization, unable to remove {} due to {}".format(
                             f, e
                         )
                     )
 
-        print(
+        _logger.info(
             "Pushed committed bundle {} uuid {} to remote {}".format(
                 human_name, hfr.pb.uuid, data_context.remote_ctxt_url
             )
         )
 
         return hfr
 
@@ -1352,15 +1351,15 @@
             len(results), len(push_tuples)
         )
         if delocalize:
             for f in to_delete:
                 try:
                     os.remove(f)
                 except IOError as e:
-                    print(
+                    _logger.warn(
                         "fast_push: during delocalization, unable to remove {} due to {}".format(
                             f, e
                         )
                     )
 
     @staticmethod
     def _localize_hfr(local_hfr, s3_uuid, data_context):
@@ -1449,21 +1448,20 @@
 
         Returns:
             None
 
         Raise:
             UserWarning: If we are not in a valid context.
         """
-
         data_context = self.ensure_data_context(data_context)
         if data_context is None:
             return
 
         if data_context.remote_ctxt_url is None:
-            print(
+            _logger.error(
                 "Pull cannot execute.  Local context {} on remote {} not bound.".format(
                     data_context.local_ctxt, data_context.remote_ctxt
                 )
             )
             raise UserWarning(
                 "Local context {} has no remote".format(data_context.local_ctxt)
             )
@@ -1502,15 +1500,15 @@
             # Note that this works because the UUID is prepended to the <uuid>_hframe.pb
             s3_uuid = hfr_basename.split("_")[0]
 
             if uuid is not None:  # filter by UUID
                 if s3_uuid != uuid:
                     continue
                 else:
-                    print(
+                    _logger.info(
                         "Found remote bundle with UUID {}, checking local context for duplicates ...".format(
                             uuid
                         )
                     )
 
             local_hfr = self.get_hframe_by_uuid(s3_uuid, data_context=data_context)
             if local_hfr is not None:
@@ -1521,15 +1519,15 @@
                         )
                     )
                 else:
                     if human_name is not None:
                         if human_name != local_hfr.pb.human_name:
                             continue
                         else:
-                            print(
+                            _logger.info(
                                 "Found remote bundle with human name {}, uuid {} localizing ...".format(
                                     local_hfr.pb.human_name, local_hfr.pb.uuid
                                 )
                             )
                     DisdatFS._localize_hfr(local_hfr, s3_uuid, data_context)
             else:
                 s3_bucket, _ = aws_s3.split_s3_url(data_context.remote_ctxt_url)
@@ -1539,28 +1537,28 @@
                 hfr_test = hyperframe.HyperFrameRecord.from_str_bytes(
                     obj["Body"].read()
                 )
                 if human_name is not None:
                     if human_name != hfr_test.pb.human_name:
                         continue
                     else:
-                        print(
+                        _logger.info(
                             "Found remote bundle with human name {}, uuid {} ...".format(
                                 hfr_test.pb.human_name, hfr_test.pb.uuid
                             )
                         )
 
                 _logger.info(
                     "Adding HyperFrame UUID {} to local context . . .".format(s3_uuid)
                 )
 
                 local_uuid_dir = os.path.join(data_context.get_object_dir(), s3_uuid)
                 local_hfr_path = os.path.join(local_uuid_dir, hfr_basename)
                 if os.path.exists(local_uuid_dir):
-                    print(
+                    _logger.info(
                         "Pull found existing data in local disdat db at UUID {}, overwriting . . .".format(
                             s3_uuid
                         )
                     )
                     shutil.rmtree(local_uuid_dir)
 
                 os.makedirs(local_uuid_dir)
@@ -1683,15 +1681,15 @@
     """
     try:
         if len(date_string.split(" ")) > 1:
             date = datetime.strptime(date_string, "%m-%d-%Y %X")
         else:
             date = datetime.strptime(date_string, "%m-%d-%Y")
     except ValueError as ve:
-        print(
+        _logger.info(
             "Unable to parse date, must be like '12-1-2008' or '\"12-1-2008 13:12:05\"'"
         )
         if not throw:
             return None
         else:
             raise
     return date
```

### Comparing `disdat-1.0.2/disdat/hyperframe.py` & `disdat-1.1.0/disdat/hyperframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 )
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.sql import text
 
 import disdat.common as common
 from disdat import hyperframe_pb2
 from disdat import logger as _logger
-from disdat.utility.aws_s3 import s3_path_exists
+from disdat.utility.asyncio_aws_s3 import s3_path_exists
 
 HyperFrameTuple = namedtuple("HyperFrameTuple", "columns, links, uuid, tags")
 
 # UPSERT policy for inserts that violate constraints (explicit or primary key uniqueness)
 # We can ROLLBACK, ABORT, FAIL, IGNORE, and REPLACE
 # Most cases we want to REPLACE (UPSERT)
 UPSERT_POLICY = "FAIL"
```

### Comparing `disdat-1.0.2/disdat/hyperframe_pb2.py` & `disdat-1.1.0/disdat/hyperframe_pb2.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/lineage.py` & `disdat-1.1.0/disdat/lineage.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/log.py` & `disdat-1.1.0/disdat/log.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/resource.py` & `disdat-1.1.0/disdat/resource.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat/utility/aws_s3.py` & `disdat-1.1.0/disdat/utility/asyncio_aws_s3.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import concurrent.futures as futures
 import os
-from multiprocessing import get_context
+import urllib
 
 import boto3 as b3
-from botocore.exceptions import ClientError
-from six.moves import urllib
 
+from disdat import log
 from disdat import logger as _logger
 
 S3_LS_USE_MP_THRESH = (
-    4000  # the threshold after which we should use MP to look up bundles on s3
+    2000  # the threshold after which we should use MP to look up bundles on s3
 )
 
-# Set to available MP contexts, such as forkserver, spawn, or fork.
-# We also support "singleprocess" -- in which case Disdat will not use MP
-SINGLE_PROCESS_MP_TYPE = "singleprocess"
-MP_CONTEXT_TYPE = os.environ.get("MP_CONTEXT_TYPE", "forkserver")
-MAX_TASKS_PER_CHILD = 100  # Force the pool to kill workers when they've done 100 tasks.
+# Note: one client for all threads.
+# You can use a client across multiple threads, but allocating the client in multiple threads
+# races on the shared default session in which they are created.
+# And you don't want to spend the time to create individual sessions for each thread.
+# https://medium.com/@life-is-short-so-enjoy-it/aws-boto3-misunderstanding-about-thread-safe-a7261d7391fd
 
 
 # Helper module-level access function to make sure resource is initialized
 def get_s3_resource():
     if get_s3_resource._s3_resource is None:
         get_s3_resource._s3_resource = b3.resource("s3")
     return get_s3_resource._s3_resource
@@ -52,32 +52,33 @@
 
 # Module global variable used to initialize and store process state for s3 client
 get_s3_client._s3_client = None
 
 
 def disdat_cpu_count():
     """
-    Turns out that Python doesn't do a great job of retrieving the number of available cpus
-    when running within a container.   As of 7-2020, it returns the actual count on the machine that's
-    hosting the container.   For Disdat, this can be very bad.  When we use multiprocessing, we use
-    the forkserver.  This tends to be memory intensive, especially when creating more workers than actual
-    CPUs.  To help avoid (but not completely avoid the out-of-memory exceptions that arise), we allow
-    the calling convention to include an environment variable called DISDAT_CPU_COUNT to be set.
-    For example in `dsdt.run`, we set this to be equal to the requested vcpu count.
+    The current version of the aws_s3 module (here) is based on multi-threading, not multi-processing.
+    Thus the concerns below do not apply.  However, I'm leaving the comment in the event that we wish to re-visit mp:
+        Python retrieves the physical cpu count when running within a container (as of 7-2020).
+        When we use multiprocessing (forkserver) this is memory intensive, possibly creating more workers than
+        vCPUs.  To help avoid OOM errors, we support an environment variable called DISDAT_CPU_COUNT to be set.
+        For example in `dsdt.run`, we set this to be equal to the requested vcpu count.
+    Note that we still support the environment variable, which can be useful for tests (moto does not support multithreading).
+
+    Finally, for multithreading, we scale up to 10 threads per available core.
 
     Returns:
         int: the number of available cpus
 
     """
-
     env_cpu_count = os.getenv("DISDAT_CPU_COUNT")
     if env_cpu_count is None:
-        return os.cpu_count()  # we did our best.
+        return os.cpu_count() * 2  # magic number of threads = 2 * core count
     else:
-        return int(env_cpu_count)
+        return int(env_cpu_count)  # just use the number in the env variable.
 
 
 def s3_path_exists(s3_url):
     """
     Given an entire path, does the key exist?
 
     If you're checking for partial key, make sure to end with '/'
@@ -119,15 +120,15 @@
     """
     Code from Amazon docs for checking bucket existence.
 
     Args:
         bucket:
 
     Returns:
-        booL: whether bucket exists
+        bool: whether bucket exists
 
     """
     import botocore
 
     s3 = get_s3_resource()
     exists = True
     try:
@@ -178,33 +179,30 @@
         _logger.error(
             "s3_list_objects_starting_hex: failed with exception {}".format(e)
         )
         raise
     return result
 
 
-def s3_list_objects_at_prefix_v2(bucket, prefix):
+def _s3_list_objects_at_prefix_v2(client, bucket, prefix):
     """List out the objects at this prefix
     Returns a list of the keys found at this bucket.
     We do so because boto objects aren't serializable under multiprocessing
 
     Note: Use v2 for multi-processing, since this filters on the server side!
 
     Args:
+        client(boto3.client): the boto3 s3 client
         bucket(str): The s3 bucket
         prefix(str): The s3 key prefix you wish to search
 
     Returns:
         (list): List of item keys
     """
     result = []
-    client = get_s3_client()
-
-    # print(f"s3_list_objects_at_prefix_v2 the b3[{b3}] and client[{b3.client} and resource[{b3.resource}]")
-
     try:
         paginator = client.get_paginator("list_objects_v2")
         page_iterator = paginator.paginate(Bucket=bucket, Prefix=prefix)
         for page in page_iterator:
             if "Contents" not in page:
                 continue
             result += [obj["Key"] for obj in page["Contents"]]
@@ -231,43 +229,41 @@
     Returns:
         list (str): list of keys under the bucket in the s3_path
     """
     if s3_url[-1] != "/":
         s3_url += "/"
 
     bucket, s3_path = split_s3_url(s3_url)
+    if s3_path is None:
+        s3_path = ""
 
     hexes = "0123456789abcdef"
 
     results = []
 
-    if is_object_directory and MP_CONTEXT_TYPE != SINGLE_PROCESS_MP_TYPE:
+    client = get_s3_client()
+
+    if is_object_directory:
         prefixes = [f"{c}{d}" for c in hexes for d in hexes]
-        multiple_results = []
-        mp_ctxt = get_context(MP_CONTEXT_TYPE)
         est_cpu_count = disdat_cpu_count()
         _logger.debug("ls_s3_url_keys using MP with cpu_count {}".format(est_cpu_count))
-        with mp_ctxt.Pool(
-            processes=est_cpu_count,
-            maxtasksperchild=MAX_TASKS_PER_CHILD,
-            initializer=get_s3_client,
-        ) as pool:
+
+        with futures.ThreadPoolExecutor(max_workers=disdat_cpu_count()) as pool:
+            result_futures = []
             for i, prefix in enumerate(prefixes):
                 prefix = os.path.join(s3_path, prefix)
-                multiple_results.append(
-                    pool.apply_async(
-                        s3_list_objects_at_prefix_v2,
-                        (bucket, prefix),
-                        callback=results.extend,
-                    )
+                result_futures.append(
+                    pool.submit(_s3_list_objects_at_prefix_v2, client, bucket, prefix)
                 )
-            pool.close()
-            pool.join()
+            results = [
+                r for f in futures.as_completed(result_futures) for r in f.result()
+            ]
+
     else:
-        results = s3_list_objects_at_prefix_v2(bucket, s3_path)
+        results = _s3_list_objects_at_prefix_v2(client, bucket, s3_path)
 
     return results
 
 
 def ls_s3_url_objects(s3_url):
     """
     List all objects under this s3_url.
@@ -329,59 +325,64 @@
     Args:
         s3_urls(list(str)): list of s3_urls we will remove
 
     Returns:
         number objects deleted (int)
 
     """
-    if MP_CONTEXT_TYPE == SINGLE_PROCESS_MP_TYPE:
-        results = []
+    client = get_s3_resource()
+
+    # The URLs may be "directories" or objects.
+    # if s3_url in to_delete:
+
+    with futures.ThreadPoolExecutor(max_workers=disdat_cpu_count()) as pool:
+        result_futures = []
         for s3_url in s3_urls:
-            results.append(delete_s3_dir(s3_url))
-    else:
-        mp_ctxt = get_context(
-            MP_CONTEXT_TYPE
-        )  # Using forkserver here causes moto / pytest failures
-        with mp_ctxt.Pool(
-            processes=disdat_cpu_count(),
-            maxtasksperchild=MAX_TASKS_PER_CHILD,
-            initializer=get_s3_resource,
-        ) as pool:
-            multiple_results = []
-            results = []
-            for s3_url in s3_urls:
-                multiple_results.append(
-                    pool.apply_async(delete_s3_dir, (s3_url,), callback=results.append)
-                )
-            pool.close()
-            pool.join()
+            result_futures.append(pool.submit(_delete_s3_dir, client, s3_url))
+        results = [f.result() for f in futures.as_completed(result_futures)]
 
     return sum([1 if r > 0 else 0 for r in results])
 
 
 def delete_s3_dir(s3_url):
     """
 
     Args:
-        s3_url:
+        s3_url(str): the directory to delete
 
     Returns:
         number deleted (int)
 
     """
+    return _delete_s3_dir(get_s3_resource(), s3_url)
+
+
+def _delete_s3_dir(s3_resource, s3_url):
+    """
+    Args:
+        resource(boto3.resource): The boto3 s3 resource
+        s3_url(str): the directory to delete
+    Returns:
+        number deleted (int)
+    """
 
-    s3 = get_s3_resource()
     bucket, s3_path = split_s3_url(s3_url)
 
-    bucket = s3.Bucket(bucket)
+    bucket = s3_resource.Bucket(bucket)
     objects_to_delete = []
     for obj in bucket.objects.filter(Prefix=s3_path):
         objects_to_delete.append({"Key": obj.key})
     if len(objects_to_delete) > 0:
-        bucket.delete_objects(Delete={"Objects": objects_to_delete})
+        try:
+            bucket.delete_objects(Delete={"Objects": objects_to_delete})
+        except Exception as e:
+            print(e)
+            print(f"FAILED DELETING OBJECTS: {objects_to_delete}")
+
+    # print(f"Deleted {len(objects_to_delete)} objects at prefix {s3_path}")
     return len(objects_to_delete)
 
 
 def cp_s3_file(s3_src_path, s3_root):
     """
     Copy an s3 file to an s3 location
     Keeps the original file name.
@@ -394,15 +395,14 @@
     """
     s3 = get_s3_resource()
     bucket, s3_path = split_s3_url(s3_root)
     filename = os.path.basename(s3_src_path)
     output_path = os.path.join(s3_path, filename)
 
     src_bucket, src_key = split_s3_url(s3_src_path)
-    # print "Trying to copy from bucket {} key {} to bucket {} key {}".format(src_bucket, src_key, bucket, output_path)
 
     s3.Object(bucket, output_path).copy_from(
         CopySource={"Bucket": src_bucket, "Key": src_key},
         ACL="bucket-owner-full-control",
         ServerSideEncryption="AES256",
     )
     return os.path.join("s3://", bucket, output_path)
@@ -415,20 +415,25 @@
     Args:
         local_file (str): Fully qualified path to local file
         s3_file (str): Fully qualified path to file on s3
 
     Returns:
         s3_file
     """
-    s3 = get_s3_resource()
+    s3 = get_s3_client()
+    return _cp_local_to_s3_file(s3, local_file, s3_file)
+
+
+def _cp_local_to_s3_file(s3_client, local_file, s3_file):
     bucket, s3_path = split_s3_url(s3_file)
     local_file = urllib.parse.urlparse(local_file).path
-    # print("AWS_S3: ----->>>>>>>\tCP s3 src {}  dst {}".format(local_file, s3_file))
-    s3.Object(bucket, s3_path).upload_file(
+    s3_client.upload_file(
         local_file,
+        bucket,
+        s3_path,
         ExtraArgs={
             "ServerSideEncryption": "AES256",
             "ACL": "bucket-owner-full-control",
         },
     )
     return s3_file
 
@@ -469,60 +474,44 @@
     Args:
         bucket_key_file_tuples (list[tuple]): (filename, s3_path)
 
     Returns:
         list: list of destination s3 paths
 
     """
+    s3_client = get_s3_client()
 
-    if MP_CONTEXT_TYPE == SINGLE_PROCESS_MP_TYPE:
-        results = []
+    with futures.ThreadPoolExecutor(max_workers=disdat_cpu_count()) as pool:
+        result_futures = []
         for local_object_path, s3_path in bucket_key_file_tuples:
-            results.append(cp_local_to_s3_file(local_object_path, s3_path))
-    else:
-        mp_ctxt = get_context(MP_CONTEXT_TYPE)
-        est_cpu_count = disdat_cpu_count()
-        _logger.debug(
-            "put_s3_key_many using MP with cpu_count {}".format(est_cpu_count)
-        )
-        with mp_ctxt.Pool(
-            processes=est_cpu_count,
-            maxtasksperchild=MAX_TASKS_PER_CHILD,
-            initializer=get_s3_resource,
-        ) as pool:
-            multiple_results = []
-            results = []
-            for local_object_path, s3_path in bucket_key_file_tuples:
-                multiple_results.append(
-                    pool.apply_async(
-                        cp_local_to_s3_file,
-                        (local_object_path, s3_path),
-                        callback=results.append,
-                    )
-                )
-            pool.close()
-            pool.join()
+            result_futures.append(
+                pool.submit(_cp_local_to_s3_file, s3_client, local_object_path, s3_path)
+            )
+        results = [f.result() for f in futures.as_completed(result_futures)]
+
     return results
 
 
 def get_s3_key(bucket, key, filename=None):
     """
 
     Args:
         bucket:
         key:
         file_name:
-        s3: A boto3.resource('s3')
 
     Returns:
 
     """
-    dl_retry = 3
     s3 = get_s3_resource()
+    return _get_s3_key(s3, bucket, key, filename)
+
 
+def _get_s3_key(s3_resource, bucket, key, filename=None):
+    dl_retry = 3
     if filename is None:
         filename = os.path.basename(key)
     else:
         path = os.path.dirname(filename)
         if not os.path.exists(path):
             try:
                 os.makedirs(path)
@@ -530,33 +519,31 @@
                 # swallow error -- likely directory already exists from other process
                 _logger.debug(
                     "aws_s3.get_s3_key: Error code {}".format(os.strerror(ose.errno))
                 )
 
     while dl_retry > 0:
         try:
-            s3.Bucket(bucket).download_file(key, filename)
+            s3_resource.Bucket(bucket).download_file(key, filename)
             dl_retry = -1
         except Exception as e:
-            _logger.warn(
+            _logger.warning(
                 "aws_s3.get_s3_key Retry Count [{}] on download_file raised exception {}".format(
                     dl_retry, e
                 )
             )
             dl_retry -= 1
             if dl_retry <= 0:
-                _logger.warn(
+                _logger.warning(
                     "aws_s3.get_s3_key Fail on downloading file after 3 retries with exception {}".format(
                         e
                     )
                 )
                 raise
 
-    # print "PID({}) STOP bkt[] key[{}] file[{}]".format(multiprocessing.current_process(),key,filename)
-
     return filename
 
 
 def get_s3_key_many(bucket_key_file_tuples):
     """Retrieve many s3 keys in parallel and copy to the filename
 
     This was done primarily because when testing from an external module, moto
@@ -566,43 +553,26 @@
     Args:
         bucket_key_file_tuples (tuple): (bucket:str, key:str, filename=None)
 
     Returns:
         filenames (list): list of filenames
 
     """
-    if MP_CONTEXT_TYPE == SINGLE_PROCESS_MP_TYPE:
-        results = []
+    s3_resource = get_s3_resource()
+
+    with futures.ThreadPoolExecutor(max_workers=disdat_cpu_count()) as pool:
+        result_futures = []
         for s3_bucket, s3_key, local_object_path in bucket_key_file_tuples:
-            results.append(get_s3_key(s3_bucket, s3_key, local_object_path))
-    else:
-        mp_ctxt = get_context(
-            MP_CONTEXT_TYPE
-        )  # Using forkserver here causes moto / pytest failures
-        est_cpu_count = disdat_cpu_count()
-        _logger.debug(
-            "get_s3_key_many using MP with cpu_count {}".format(est_cpu_count)
-        )
-        with mp_ctxt.Pool(
-            processes=est_cpu_count,
-            maxtasksperchild=MAX_TASKS_PER_CHILD,
-            initializer=get_s3_resource,
-        ) as pool:
-            multiple_results = []
-            results = []
-            for s3_bucket, s3_key, local_object_path in bucket_key_file_tuples:
-                multiple_results.append(
-                    pool.apply_async(
-                        get_s3_key,
-                        (s3_bucket, s3_key, local_object_path),
-                        callback=results.append,
-                    )
+            result_futures.append(
+                pool.submit(
+                    _get_s3_key, s3_resource, s3_bucket, s3_key, local_object_path
                 )
-            pool.close()
-            pool.join()
+            )
+        results = [f.result() for f in futures.as_completed(result_futures)]
+
     return results
 
 
 def get_s3_file(s3_url, filename=None):
     bucket, s3_path = split_s3_url(s3_url)
 
     return get_s3_key(bucket, s3_path, filename)
```

### Comparing `disdat-1.0.2/disdat/utility/bundle_helpers.py` & `disdat-1.1.0/disdat/utility/bundle_helpers.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/disdat.egg-info/PKG-INFO` & `disdat-1.1.0/disdat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disdat
-Version: 1.0.2
+Version: 1.1.0
 Summary: Disdat: data versioning
 Home-page: https://github.com/kyocum/disdat
 Author: Ken Yocum
 Author-email: kyocum@gmail.com
 License: Apache License, version 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `disdat-1.0.2/disdat.egg-info/SOURCES.txt` & `disdat-1.1.0/disdat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 disdat.egg-info/top_level.txt
 disdat/config/README.md
 disdat/config/__init__.py
 disdat/config/disdat/.exclude-from-modeler-docker-image
 disdat/config/disdat/disdat.cfg
 disdat/entrypoints/cli_ep.py
 disdat/utility/__init__.py
-disdat/utility/aws_s3.py
+disdat/utility/asyncio_aws_s3.py
 disdat/utility/bundle_helpers.py
 docs/DisdatTitleFig.jpg
 infrastructure/.gitignore
 infrastructure/Dockerfiles/Makefile
 infrastructure/Dockerfiles/hyperframe_def/Dockerfile
 infrastructure/Dockerfiles/hyperframe_def/Makefile
 infrastructure/Dockerfiles/hyperframe_def/README.md
```

### Comparing `disdat-1.0.2/docs/DisdatTitleFig.jpg` & `disdat-1.1.0/docs/DisdatTitleFig.jpg`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/infrastructure/.gitignore` & `disdat-1.1.0/infrastructure/.gitignore`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/bundle.proto` & `disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/bundle.proto`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto` & `disdat-1.1.0/infrastructure/Dockerfiles/hyperframe_def/hyperframe.proto`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/setup.py` & `disdat-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/bundles/test_arg_capture.py` & `disdat-1.1.0/tests/bundles/test_arg_capture.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/bundles/test_file_bundle_api.py` & `disdat-1.1.0/tests/bundles/test_file_bundle_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tempfile
 
 import boto3
 import moto
 import pytest
 
 import disdat.api as api
-from disdat.utility import aws_s3
+import disdat.utility.asyncio_aws_s3 as aws_s3
 from tests.functional.common import TEST_CONTEXT, run_test
 
 #
 # Copyright 2017 Human Longevity, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
```

### Comparing `disdat-1.0.2/tests/bundles/test_hframe.py` & `disdat-1.1.0/tests/bundles/test_hframe.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/data/US_chronic_disease_indicators_CDI_2012.csv` & `disdat-1.1.0/tests/data/US_chronic_disease_indicators_CDI_2012.csv`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/functional/test_add.py` & `disdat-1.1.0/tests/functional/test_add.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/functional/test_add_remote.py` & `disdat-1.1.0/tests/functional/test_add_remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,17 @@
 
 """
 import boto3
 import moto
 import pytest
 
 import disdat.api as api
-from tests.functional.common import TEST_CONTEXT
+from tests.functional.common import TEST_BUCKET, TEST_CONTEXT
 
 TEST_REMOTE = "__test_remote_context__"
-TEST_BUCKET = "test-bucket"
 TEST_BUCKET_URL = "s3://{}".format(TEST_BUCKET)
 TEST_BUCKET_KEY_URL = "s3://{}/somekey".format(TEST_BUCKET)
 
 
 @moto.mock_s3
 def test_add_remote():
     api.delete_context(TEST_CONTEXT)
```

### Comparing `disdat-1.0.2/tests/functional/test_cat.py` & `disdat-1.1.0/tests/functional/test_cat.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/functional/test_context.py` & `disdat-1.1.0/tests/functional/test_context.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/functional/test_hyperframe.py` & `disdat-1.1.0/tests/functional/test_hyperframe.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/functional/test_link_localization.py` & `disdat-1.1.0/tests/functional/test_link_localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import tempfile
 
 import boto3
 import moto
 import pytest
 
 import disdat.api as api
-import disdat.utility.aws_s3 as aws_s3
+import disdat.utility.asyncio_aws_s3 as aws_s3
 from tests.functional.common import TEST_CONTEXT
 
 TEST_REMOTE = "__test_remote_context__"
 TEST_BUCKET = "test-bucket"
 TEST_BUCKET_URL = "s3://{}".format(TEST_BUCKET)
```

### Comparing `disdat-1.0.2/tests/functional/test_output_types.py` & `disdat-1.1.0/tests/functional/test_output_types.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tests/functional/test_remote.py` & `disdat-1.1.0/tests/functional/test_remote.py`

 * *Files identical despite different names*

### Comparing `disdat-1.0.2/tox.ini` & `disdat-1.1.0/tox.ini`

 * *Files identical despite different names*

