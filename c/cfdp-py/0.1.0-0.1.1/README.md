# Comparing `tmp/cfdp-py-0.1.0.tar.gz` & `tmp/cfdp_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdp-py-0.1.0.tar", last modified: Wed Jan 24 14:39:36 2024, max compression
+gzip compressed data, was "cfdp_py-0.1.1.tar", last modified: Tue Apr 23 08:42:25 2024, max compression
```

## Comparing `cfdp-py-0.1.0.tar` & `cfdp_py-0.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      383 2024-01-24 14:39:30.000000 cfdp-py-0.1.0/CHANGELOG.md
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11357 2024-01-24 11:30:38.000000 cfdp-py-0.1.0/LICENSE
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      154 2024-01-24 11:36:08.000000 cfdp-py-0.1.0/MANIFEST.in
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      181 2024-01-24 11:31:22.000000 cfdp-py-0.1.0/NOTICE
--rw-r--r--   0 rmueller  (1000) rmueller  (1000)     3074 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/PKG-INFO
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1879 2024-01-24 14:39:30.000000 cfdp-py-0.1.0/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.383513 cfdp-py-0.1.0/docs/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      634 2024-01-23 20:37:44.000000 cfdp-py-0.1.0/docs/Makefile
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.383513 cfdp-py-0.1.0/docs/api/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      632 2024-01-24 14:22:51.000000 cfdp-py-0.1.0/docs/api/cfdp.handler.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      989 2024-01-24 14:22:46.000000 cfdp-py-0.1.0/docs/api/cfdp.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       96 2024-01-24 11:05:53.000000 cfdp-py-0.1.0/docs/api.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2794 2024-01-24 14:20:03.000000 cfdp-py-0.1.0/docs/conf.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      923 2024-01-24 11:02:09.000000 cfdp-py-0.1.0/docs/examples.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1007 2024-01-24 14:23:29.000000 cfdp-py-0.1.0/docs/index.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4727 2024-01-24 11:01:29.000000 cfdp-py-0.1.0/docs/introduction.rst
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      800 2024-01-23 20:37:44.000000 cfdp-py-0.1.0/docs/make.bat
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       24 2024-01-24 11:18:14.000000 cfdp-py-0.1.0/docs/requirements.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1296 2024-01-24 14:34:35.000000 cfdp-py-0.1.0/pyproject.toml
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2024-01-24 11:31:44.000000 cfdp-py-0.1.0/requirements.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       38 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/setup.cfg
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.383513 cfdp-py-0.1.0/src/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2024-01-23 20:33:26.000000 cfdp-py-0.1.0/src/__init__.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/src/cfdp_py.egg-info/
--rw-r--r--   0 rmueller  (1000) rmueller  (1000)     3074 2024-01-24 14:39:36.000000 cfdp-py-0.1.0/src/cfdp_py.egg-info/PKG-INFO
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1392 2024-01-24 14:39:36.000000 cfdp-py-0.1.0/src/cfdp_py.egg-info/SOURCES.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        1 2024-01-24 14:39:36.000000 cfdp-py-0.1.0/src/cfdp_py.egg-info/dependency_links.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       72 2024-01-24 14:39:36.000000 cfdp-py-0.1.0/src/cfdp_py.egg-info/requires.txt
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       16 2024-01-24 14:39:36.000000 cfdp-py-0.1.0/src/cfdp_py.egg-info/top_level.txt
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.383513 cfdp-py-0.1.0/src/cfdppy/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      601 2024-01-24 14:00:51.000000 cfdp-py-0.1.0/src/cfdppy/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      509 2024-01-24 13:47:53.000000 cfdp-py-0.1.0/src/cfdppy/defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4847 2024-01-24 13:47:58.000000 cfdp-py-0.1.0/src/cfdppy/exceptions.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9641 2024-01-24 13:49:01.000000 cfdp-py-0.1.0/src/cfdppy/filestore.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/src/cfdppy/handler/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      439 2024-01-24 14:01:00.000000 cfdp-py-0.1.0/src/cfdppy/handler/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2560 2024-01-24 13:49:06.000000 cfdp-py-0.1.0/src/cfdppy/handler/common.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2754 2024-01-24 14:02:51.000000 cfdp-py-0.1.0/src/cfdppy/handler/crc.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      524 2024-01-23 20:46:54.000000 cfdp-py-0.1.0/src/cfdppy/handler/defs.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    54646 2024-01-24 14:02:41.000000 cfdp-py-0.1.0/src/cfdppy/handler/dest.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    43453 2024-01-24 14:01:17.000000 cfdp-py-0.1.0/src/cfdppy/handler/source.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12313 2024-01-24 10:21:55.000000 cfdp-py-0.1.0/src/cfdppy/mib.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5455 2024-01-24 13:48:56.000000 cfdp-py-0.1.0/src/cfdppy/request.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6209 2024-01-24 14:03:12.000000 cfdp-py-0.1.0/src/cfdppy/user.py
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/tests/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/tests/.pytest_cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2024-01-24 10:50:18.000000 cfdp-py-0.1.0/tests/.pytest_cache/.gitignore
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2024-01-24 10:50:18.000000 cfdp-py-0.1.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2024-01-24 10:50:18.000000 cfdp-py-0.1.0/tests/.pytest_cache/README.md
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.379513 cfdp-py-0.1.0/tests/.pytest_cache/v/
-drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-01-24 14:39:36.387513 cfdp-py-0.1.0/tests/.pytest_cache/v/cache/
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       30 2024-01-24 10:50:18.000000 cfdp-py-0.1.0/tests/.pytest_cache/v/cache/lastfailed
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2024-01-24 10:50:18.000000 cfdp-py-0.1.0/tests/.pytest_cache/v/cache/nodeids
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2024-01-24 10:50:18.000000 cfdp-py-0.1.0/tests/.pytest_cache/v/cache/stepwise
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2024-01-23 20:34:58.000000 cfdp-py-0.1.0/tests/__init__.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      735 2024-01-24 14:01:53.000000 cfdp-py-0.1.0/tests/cfdp_fault_handler_mock.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1532 2024-01-24 14:01:59.000000 cfdp-py-0.1.0/tests/cfdp_user_mock.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      883 2024-01-24 14:03:24.000000 cfdp-py-0.1.0/tests/common.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1753 2024-01-24 14:02:03.000000 cfdp-py-0.1.0/tests/test_checksum.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    13867 2024-01-24 14:02:06.000000 cfdp-py-0.1.0/tests/test_dest_handler.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    26271 2024-01-24 14:02:09.000000 cfdp-py-0.1.0/tests/test_dest_handler_acked.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    14312 2024-01-24 14:02:12.000000 cfdp-py-0.1.0/tests/test_dest_handler_naked.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4376 2024-01-24 14:02:16.000000 cfdp-py-0.1.0/tests/test_filestore.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3333 2024-01-24 14:02:19.000000 cfdp-py-0.1.0/tests/test_lost_seg_tracker.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2638 2024-01-24 14:02:22.000000 cfdp-py-0.1.0/tests/test_request.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    17093 2024-01-24 14:02:25.000000 cfdp-py-0.1.0/tests/test_src_handler.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    13726 2024-01-24 14:02:27.000000 cfdp-py-0.1.0/tests/test_src_handler_acked.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8244 2024-01-24 14:02:30.000000 cfdp-py-0.1.0/tests/test_src_handler_nak_closure.py
--rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11291 2024-01-24 14:02:36.000000 cfdp-py-0.1.0/tests/test_src_handler_nak_no_closure.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.701390 cfdp_py-0.1.1/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      458 2024-04-23 08:41:57.000000 cfdp_py-0.1.1/CHANGELOG.md
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11357 2024-01-24 11:30:38.000000 cfdp_py-0.1.1/LICENSE
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      154 2024-01-24 11:36:08.000000 cfdp_py-0.1.1/MANIFEST.in
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      181 2024-01-24 11:31:22.000000 cfdp_py-0.1.1/NOTICE
+-rw-r--r--   0 rmueller  (1000) rmueller  (1000)     3083 2024-04-23 08:42:25.697390 cfdp_py-0.1.1/PKG-INFO
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1882 2024-04-23 08:41:57.000000 cfdp_py-0.1.1/README.md
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.693390 cfdp_py-0.1.1/docs/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      634 2024-01-23 20:37:44.000000 cfdp_py-0.1.1/docs/Makefile
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.693390 cfdp_py-0.1.1/docs/api/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      632 2024-01-24 14:22:51.000000 cfdp_py-0.1.1/docs/api/cfdp.handler.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      989 2024-01-24 14:22:46.000000 cfdp_py-0.1.1/docs/api/cfdp.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       96 2024-01-24 11:05:53.000000 cfdp_py-0.1.1/docs/api.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2794 2024-01-24 14:20:03.000000 cfdp_py-0.1.1/docs/conf.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      915 2024-01-24 15:17:49.000000 cfdp_py-0.1.1/docs/examples.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1007 2024-01-24 14:23:29.000000 cfdp_py-0.1.1/docs/index.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4679 2024-01-24 15:17:49.000000 cfdp_py-0.1.1/docs/introduction.rst
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      800 2024-01-23 20:37:44.000000 cfdp_py-0.1.1/docs/make.bat
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       24 2024-01-24 11:18:14.000000 cfdp_py-0.1.1/docs/requirements.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1314 2024-04-23 08:42:13.000000 cfdp_py-0.1.1/pyproject.toml
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2024-01-24 11:31:44.000000 cfdp_py-0.1.1/requirements.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       38 2024-04-23 08:42:25.701390 cfdp_py-0.1.1/setup.cfg
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.693390 cfdp_py-0.1.1/src/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2024-01-23 20:33:26.000000 cfdp_py-0.1.1/src/__init__.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.697390 cfdp_py-0.1.1/src/cfdp_py.egg-info/
+-rw-r--r--   0 rmueller  (1000) rmueller  (1000)     3083 2024-04-23 08:42:25.000000 cfdp_py-0.1.1/src/cfdp_py.egg-info/PKG-INFO
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1392 2024-04-23 08:42:25.000000 cfdp_py-0.1.1/src/cfdp_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        1 2024-04-23 08:42:25.000000 cfdp_py-0.1.1/src/cfdp_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       78 2024-04-23 08:42:25.000000 cfdp_py-0.1.1/src/cfdp_py.egg-info/requires.txt
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       16 2024-04-23 08:42:25.000000 cfdp_py-0.1.1/src/cfdp_py.egg-info/top_level.txt
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.693390 cfdp_py-0.1.1/src/cfdppy/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      601 2024-01-24 14:00:51.000000 cfdp_py-0.1.1/src/cfdppy/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      509 2024-01-24 13:47:53.000000 cfdp_py-0.1.1/src/cfdppy/defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4847 2024-01-24 13:47:58.000000 cfdp_py-0.1.1/src/cfdppy/exceptions.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     9641 2024-01-24 13:49:01.000000 cfdp_py-0.1.1/src/cfdppy/filestore.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.697390 cfdp_py-0.1.1/src/cfdppy/handler/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      439 2024-01-24 14:01:00.000000 cfdp_py-0.1.1/src/cfdppy/handler/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2560 2024-01-24 13:49:06.000000 cfdp_py-0.1.1/src/cfdppy/handler/common.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2754 2024-02-05 10:05:30.000000 cfdp_py-0.1.1/src/cfdppy/handler/crc.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      524 2024-01-23 20:46:54.000000 cfdp_py-0.1.1/src/cfdppy/handler/defs.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    54646 2024-01-24 14:02:41.000000 cfdp_py-0.1.1/src/cfdppy/handler/dest.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    43453 2024-01-24 14:01:17.000000 cfdp_py-0.1.1/src/cfdppy/handler/source.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    12313 2024-01-24 10:21:55.000000 cfdp_py-0.1.1/src/cfdppy/mib.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     5455 2024-01-24 13:48:56.000000 cfdp_py-0.1.1/src/cfdppy/request.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     6209 2024-01-24 14:03:12.000000 cfdp_py-0.1.1/src/cfdppy/user.py
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.697390 cfdp_py-0.1.1/tests/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.697390 cfdp_py-0.1.1/tests/.pytest_cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       37 2024-01-24 10:50:18.000000 cfdp_py-0.1.1/tests/.pytest_cache/.gitignore
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      191 2024-01-24 10:50:18.000000 cfdp_py-0.1.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      302 2024-01-24 10:50:18.000000 cfdp_py-0.1.1/tests/.pytest_cache/README.md
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.693390 cfdp_py-0.1.1/tests/.pytest_cache/v/
+drwxrwxr-x   0 rmueller  (1000) rmueller  (1000)        0 2024-04-23 08:42:25.697390 cfdp_py-0.1.1/tests/.pytest_cache/v/cache/
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)       30 2024-01-24 10:50:18.000000 cfdp_py-0.1.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2024-01-24 10:50:18.000000 cfdp_py-0.1.1/tests/.pytest_cache/v/cache/nodeids
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        2 2024-01-24 10:50:18.000000 cfdp_py-0.1.1/tests/.pytest_cache/v/cache/stepwise
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)        0 2024-01-23 20:34:58.000000 cfdp_py-0.1.1/tests/__init__.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      735 2024-01-24 14:01:53.000000 cfdp_py-0.1.1/tests/cfdp_fault_handler_mock.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1532 2024-01-24 14:01:59.000000 cfdp_py-0.1.1/tests/cfdp_user_mock.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)      883 2024-01-24 14:03:24.000000 cfdp_py-0.1.1/tests/common.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     1915 2024-04-23 08:41:57.000000 cfdp_py-0.1.1/tests/test_checksum.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    13867 2024-01-24 14:02:06.000000 cfdp_py-0.1.1/tests/test_dest_handler.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    26271 2024-01-24 14:02:09.000000 cfdp_py-0.1.1/tests/test_dest_handler_acked.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    14312 2024-01-24 14:02:12.000000 cfdp_py-0.1.1/tests/test_dest_handler_naked.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     4376 2024-01-24 14:02:16.000000 cfdp_py-0.1.1/tests/test_filestore.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     3333 2024-01-24 14:02:19.000000 cfdp_py-0.1.1/tests/test_lost_seg_tracker.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     2638 2024-01-24 14:02:22.000000 cfdp_py-0.1.1/tests/test_request.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    17093 2024-01-24 14:02:25.000000 cfdp_py-0.1.1/tests/test_src_handler.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    13726 2024-01-24 14:02:27.000000 cfdp_py-0.1.1/tests/test_src_handler_acked.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)     8244 2024-01-24 14:02:30.000000 cfdp_py-0.1.1/tests/test_src_handler_nak_closure.py
+-rw-rw-r--   0 rmueller  (1000) rmueller  (1000)    11291 2024-01-24 14:02:36.000000 cfdp_py-0.1.1/tests/test_src_handler_nak_no_closure.py
```

### Comparing `cfdp-py-0.1.0/LICENSE` & `cfdp_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/PKG-INFO` & `cfdp_py-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdp-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for high level CCSDS File Delivery Protocol (CFDP) components
 Author-email: Robin Mueller <robin.mueller.m@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/us-irs/cfdp-py
 Keywords: ccsds,space,communication,packet,file-transfer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,24 +18,24 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
-Requires-Dist: spacepackets~=0.23.0
+Requires-Dist: spacepackets<0.25,>=0.23.0
 Requires-Dist: crcmod~=1.7
 Requires-Dist: deprecation~=2.1
 Provides-Extra: test
 Requires-Dist: pyfakefs~=4.5; extra == "test"
 
 [![ci](https://github.com/us-irs/cfdp-py/actions/workflows/ci.yml/badge.svg)](https://github.com/us-irs/cfdp-py/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/cfdp-py/badge/?version=latest)](https://cfdp-py.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/us-irs/cfdp-py/graph/badge.svg?token=FBL1NR54BI)](https://codecov.io/gh/us-irs/cfdp-py)
-[![PyPI version](https://badge.fury.io/py/cfdppy.svg)](https://badge.fury.io/py/cfdppy)
+[![PyPI version](https://badge.fury.io/py/cfdp-py.svg)](https://badge.fury.io/py/cfdp-py)
 
 cfdp-py - High level Python library for CFDP components
 ======================
 
 The `cfdp-py` library offers some high-level CCSDS File Delivery Protocol (CFDP) components to
 perform file transfers according to the [CCSDS Blue Book 727.0-B-5](https://public.ccsds.org/Pubs/727x0b5.pdf).
 The underlying base packet library used to generate the packets to be sent is the
@@ -44,35 +44,35 @@
 # Install
 
 You can install this package from PyPI
 
 Linux:
 
 ```sh
-python3 -m pip install cfdppy 
+python3 -m pip install cfdp-py
 ```
 
 Windows:
 
 ```sh
-py -m pip install cfdppy 
+py -m pip install cfdp-py
 ```
 
 # Examples
 
 You can find all examples [inside the documentation](https://cfdp-py.readthedocs.io/en/latest/examples.html) and the `examples` directory of this repository.
 
 # Tests
 
 If you want to run the tests, it is recommended to install `pytest` and `coverage` (optional)
 first. You also have to install the package with the optional `test` feature:
 
 ```sh
 pip install coverage pytest
-pip install cfdppy[test]
+pip install cfdp-py[test]
 ```
 
 Running tests regularly:
 
 ```sh
 pytest .
 ```
```

### Comparing `cfdp-py-0.1.0/README.md` & `cfdp_py-0.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![ci](https://github.com/us-irs/cfdp-py/actions/workflows/ci.yml/badge.svg)](https://github.com/us-irs/cfdp-py/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/cfdp-py/badge/?version=latest)](https://cfdp-py.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/us-irs/cfdp-py/graph/badge.svg?token=FBL1NR54BI)](https://codecov.io/gh/us-irs/cfdp-py)
-[![PyPI version](https://badge.fury.io/py/cfdppy.svg)](https://badge.fury.io/py/cfdppy)
+[![PyPI version](https://badge.fury.io/py/cfdp-py.svg)](https://badge.fury.io/py/cfdp-py)
 
 cfdp-py - High level Python library for CFDP components
 ======================
 
 The `cfdp-py` library offers some high-level CCSDS File Delivery Protocol (CFDP) components to
 perform file transfers according to the [CCSDS Blue Book 727.0-B-5](https://public.ccsds.org/Pubs/727x0b5.pdf).
 The underlying base packet library used to generate the packets to be sent is the
@@ -14,35 +14,35 @@
 # Install
 
 You can install this package from PyPI
 
 Linux:
 
 ```sh
-python3 -m pip install cfdppy 
+python3 -m pip install cfdp-py
 ```
 
 Windows:
 
 ```sh
-py -m pip install cfdppy 
+py -m pip install cfdp-py
 ```
 
 # Examples
 
 You can find all examples [inside the documentation](https://cfdp-py.readthedocs.io/en/latest/examples.html) and the `examples` directory of this repository.
 
 # Tests
 
 If you want to run the tests, it is recommended to install `pytest` and `coverage` (optional)
 first. You also have to install the package with the optional `test` feature:
 
 ```sh
 pip install coverage pytest
-pip install cfdppy[test]
+pip install cfdp-py[test]
 ```
 
 Running tests regularly:
 
 ```sh
 pytest .
 ```
```

### Comparing `cfdp-py-0.1.0/docs/Makefile` & `cfdp_py-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/docs/api/cfdp.handler.rst` & `cfdp_py-0.1.1/docs/api/cfdp.handler.rst`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/docs/api/cfdp.rst` & `cfdp_py-0.1.1/docs/api/cfdp.rst`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/docs/conf.py` & `cfdp_py-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/docs/examples.rst` & `cfdp_py-0.1.1/docs/examples.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 =====================
 Example applications
 =====================
 
 You can find an example application inside the
-`example directory <https://github.com/robamu-org/tmtccmd/tree/main/examples/cfdp-simple>`_
+`example directory <https://github.com/us-irs/cfdp-py/tree/main/examples/cfdp-simple>`_
 which shows an end-to-end file transfer on a host computer. This should give you a general idea of
 how the source and destination handler work in practice.
 
 There is also a
 `test application <https://github.com/robamu-org/tmtccmd/tree/main/examples/cfdp-libre-cube-crosstest>`_
-which cross-tests the `tmtccmd` CFDP implementation with the
+which cross-tests the `cfdp-py` CFDP implementation with the
 `Libre Cube CFDP <https://gitlab.com/librecube/lib/python-cfdp>`_ implementation.
 
 Finally, you can see a more complex example also featuring more features of the CFDP state machines
-`here <https://github.com/robamu-org/tmtccmd/tree/main/examples/cfdp-cli-udp>`_. This example
+`here <https://github.com/us-irs/cfdp-py/tree/main/examples/cfdp-cli-udp>`_. This example
 uses UDP servers for communication and explicitely separates the local and remote entity
 application.
```

### Comparing `cfdp-py-0.1.0/docs/index.rst` & `cfdp_py-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/docs/introduction.rst` & `cfdp_py-0.1.1/docs/introduction.rst`

 * *Files 5% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 transaction closure is applicable for simplex communication paths, while the unacknowledged mode
 with closure is the easiest way to get a confirmation of a successfull file transfer, including a
 CRC check on the remote side to verify file integrity. The acknowledged mode is the most complex
 mode which includes multiple mechanism to ensure succesfull packet transaction even for unreliable
 connections, including lost segment detection. As such, it can be compared to a specialized TCP
 for file transfers with remote systems.
 
-The core of these high-level components are the :py:class:`tmtccmd.cfdp.handler.dest.DestHandler`
-and the :py:class:`tmtccmd.cfdp.handler.source.SourceHandler` component. These model the CFDP
+The core of these high-level components are the :py:class:`cfdppy.handler.dest.DestHandler`
+and the :py:class:`cfdppy.handler.source.SourceHandler` component. These model the CFDP
 destination and CFDP source entity respectively.
 
 CFDP source entity
 -------------------
 
-The :py:class:`tmtccmd.cfdp.handler.source.SourceHandler` converts a
-:py:class:`tmtccmd.cfdp.request.PutRequest` into all packet data units (PDUs) which need to be
+The :py:class:`cfdppy.handler.source.SourceHandler` converts a
+:py:class:`cfdppy.request.PutRequest` into all packet data units (PDUs) which need to be
 sent to a remote CFDP entity to perform a File Copy operation to a remote entity. The source entity
 allows freedom of communcation by only generating the packets required to be sent, and leaving the
 actual transmission of those packets to the user. The packet is returned to the user using
 the :py:class:`spacepackets.cfdp.pdu.helper.PduHolder` field of the
-:py:class:`tmtccmd.cfdp.handler.source.FsmResult` structure returned in the
-:py:meth:`tmtccmd.cfdp.handler.source.SourceHandler.state_machine` call.
+:py:class:`cfdppy.handler.source.FsmResult` structure returned in the
+:py:meth:`cfdppy.handler.source.SourceHandler.state_machine` call.
 
 The state machine of the source entity will generally perform the following steps, after
-a valid :py:class:`tmtccmd.cfdp.request.PutRequest` to perform a File Copy operation was received:
+a valid :py:class:`cfdppy.request.PutRequest` to perform a File Copy operation was received:
 
 1. Generate the Metadata PDU to be sent to a remote CFDP entity. The PDU will be returned as a
    :py:class:`spacepackets.cfdp.pdu.metadata.MetadataPdu` instance.
 2. Generate all File Data PDUs to be sent to a remote CFDP entity, if applicable (file not empty).
    The PDU(s) will be returned as a :py:class:`spacepackets.cfdp.pdu.file_data.FileDataPdu`
    instance(s).
 3. Generate an EOF PDU be sent to a remote CFDP entity.
@@ -51,15 +51,15 @@
 4. A EOF ACK packet will be awaited, for example one generated using :py:class:`spacepackets.cfdp.pdu.ack.AckPdu`.
 5. A Finished PDU will be awaited, for example one generated using :py:class:`spacepackets.cfdp.pdu.finished.FinishedPdu`.
 6. A Finished PDU ACK packet will be sent to the remote CFDP entity.
 
 CFDP destination entity
 ------------------------
 
-The :py:class:`tmtccmd.cfdp.handler.dest.DestHandler` can convert the PDUs sent from a remote
+The :py:class:`cfdppy.handler.dest.DestHandler` can convert the PDUs sent from a remote
 source entity ID back to a file. A file copy operation on the receiver side is started with
 the reception of a Metadata PDU, for example one generated by the
 :py:class:`spacepackets.cfdp.pdu.metadata.MetadataPdu` class . After that, file packet PDUs, for
 example generated by the :py:class:`spacepackets.cfdp.pdu.file_data.FileDataPdu`, can be inserted
 into the destination handler and will be assembled into a file. The transaction will be finished
 for the following conditions:
```

### Comparing `cfdp-py-0.1.0/docs/make.bat` & `cfdp_py-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/pyproject.toml` & `cfdp_py-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=0.62.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfdp-py"
 description = "Library for high level CCSDS File Delivery Protocol (CFDP) components"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.8"
 license = {text = "Apache-2.0"}
 authors = [
   {name = "Robin Mueller", email = "robin.mueller.m@gmail.com"}
 ]
 keywords = ["ccsds", "space", "communication", "packet", "file-transfer"]
 classifiers = [
@@ -24,24 +24,24 @@
   "Programming Language :: Python :: 3.9",
   "Topic :: Communications",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Scientific/Engineering"
 ]
 dependencies = [
-  "spacepackets~=0.23.0",
+  "spacepackets>=0.23.0, <0.25",
   "crcmod~=1.7",
-  "deprecation~=2.1"
+  "deprecation~=2.1",
 ]
 
 [project.optional-dependencies]
 test = [
     "pyfakefs~=4.5",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/us-irs/cfdp-py"
 
-[tool.ruff]
+[tool.ruff.lint]
 ignore = ["E501"]
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `cfdp-py-0.1.0/src/cfdp_py.egg-info/PKG-INFO` & `cfdp_py-0.1.1/src/cfdp_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdp-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for high level CCSDS File Delivery Protocol (CFDP) components
 Author-email: Robin Mueller <robin.mueller.m@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/us-irs/cfdp-py
 Keywords: ccsds,space,communication,packet,file-transfer
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,24 +18,24 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
-Requires-Dist: spacepackets~=0.23.0
+Requires-Dist: spacepackets<0.25,>=0.23.0
 Requires-Dist: crcmod~=1.7
 Requires-Dist: deprecation~=2.1
 Provides-Extra: test
 Requires-Dist: pyfakefs~=4.5; extra == "test"
 
 [![ci](https://github.com/us-irs/cfdp-py/actions/workflows/ci.yml/badge.svg)](https://github.com/us-irs/cfdp-py/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/cfdp-py/badge/?version=latest)](https://cfdp-py.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/us-irs/cfdp-py/graph/badge.svg?token=FBL1NR54BI)](https://codecov.io/gh/us-irs/cfdp-py)
-[![PyPI version](https://badge.fury.io/py/cfdppy.svg)](https://badge.fury.io/py/cfdppy)
+[![PyPI version](https://badge.fury.io/py/cfdp-py.svg)](https://badge.fury.io/py/cfdp-py)
 
 cfdp-py - High level Python library for CFDP components
 ======================
 
 The `cfdp-py` library offers some high-level CCSDS File Delivery Protocol (CFDP) components to
 perform file transfers according to the [CCSDS Blue Book 727.0-B-5](https://public.ccsds.org/Pubs/727x0b5.pdf).
 The underlying base packet library used to generate the packets to be sent is the
@@ -44,35 +44,35 @@
 # Install
 
 You can install this package from PyPI
 
 Linux:
 
 ```sh
-python3 -m pip install cfdppy 
+python3 -m pip install cfdp-py
 ```
 
 Windows:
 
 ```sh
-py -m pip install cfdppy 
+py -m pip install cfdp-py
 ```
 
 # Examples
 
 You can find all examples [inside the documentation](https://cfdp-py.readthedocs.io/en/latest/examples.html) and the `examples` directory of this repository.
 
 # Tests
 
 If you want to run the tests, it is recommended to install `pytest` and `coverage` (optional)
 first. You also have to install the package with the optional `test` feature:
 
 ```sh
 pip install coverage pytest
-pip install cfdppy[test]
+pip install cfdp-py[test]
 ```
 
 Running tests regularly:
 
 ```sh
 pytest .
 ```
```

### Comparing `cfdp-py-0.1.0/src/cfdp_py.egg-info/SOURCES.txt` & `cfdp_py-0.1.1/src/cfdp_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/__init__.py` & `cfdp_py-0.1.1/src/cfdppy/__init__.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/exceptions.py` & `cfdp_py-0.1.1/src/cfdppy/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/filestore.py` & `cfdp_py-0.1.1/src/cfdppy/filestore.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/handler/common.py` & `cfdp_py-0.1.1/src/cfdppy/handler/common.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/handler/crc.py` & `cfdp_py-0.1.1/src/cfdppy/handler/crc.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/handler/defs.py` & `cfdp_py-0.1.1/src/cfdppy/handler/defs.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/handler/dest.py` & `cfdp_py-0.1.1/src/cfdppy/handler/dest.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/handler/source.py` & `cfdp_py-0.1.1/src/cfdppy/handler/source.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/mib.py` & `cfdp_py-0.1.1/src/cfdppy/mib.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/request.py` & `cfdp_py-0.1.1/src/cfdppy/request.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/src/cfdppy/user.py` & `cfdp_py-0.1.1/src/cfdppy/user.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/cfdp_fault_handler_mock.py` & `cfdp_py-0.1.1/tests/cfdp_fault_handler_mock.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/cfdp_user_mock.py` & `cfdp_py-0.1.1/tests/cfdp_user_mock.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/common.py` & `cfdp_py-0.1.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_checksum.py` & `cfdp_py-0.1.1/tests/test_checksum.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,29 +32,30 @@
 class TestChecksumHelper(TestCase):
     def setUp(self):
         self.setUpPyfakefs()
         self.crc_helper = CrcHelper(ChecksumType.NULL_CHECKSUM, HostFilestore())
         self.file_path = Path(f"{gettempdir()}/crc_file")
         with open(self.file_path, "wb") as file:
             file.write(EXAMPLE_DATA_CFDP)
+        # Kind of re-writing the modular checksum impl here which we are trying to test, but the
+        # numbers/correctness were verified manually using calculators, so this is okay.
         segments_to_add = []
         for i in range(4):
             if (i + 1) * 4 > len(EXAMPLE_DATA_CFDP):
                 data_to_add = EXAMPLE_DATA_CFDP[i * 4 :].ljust(4, bytes([0]))
             else:
                 data_to_add = EXAMPLE_DATA_CFDP[i * 4 : (i + 1) * 4]
             segments_to_add.append(
                 int.from_bytes(
                     data_to_add,
                     byteorder="big",
                     signed=False,
                 )
             )
         full_sum = sum(segments_to_add)
-        print(full_sum)
         full_sum %= 2**32
 
         self.expected_checksum_for_example = struct.pack("!I", full_sum)
 
     def test_modular_checksum(self):
         self.assertEqual(
             calc_modular_checksum(self.file_path), self.expected_checksum_for_example
```

### Comparing `cfdp-py-0.1.0/tests/test_dest_handler.py` & `cfdp_py-0.1.1/tests/test_dest_handler.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_dest_handler_acked.py` & `cfdp_py-0.1.1/tests/test_dest_handler_acked.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_dest_handler_naked.py` & `cfdp_py-0.1.1/tests/test_dest_handler_naked.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_filestore.py` & `cfdp_py-0.1.1/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_lost_seg_tracker.py` & `cfdp_py-0.1.1/tests/test_lost_seg_tracker.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_request.py` & `cfdp_py-0.1.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_src_handler.py` & `cfdp_py-0.1.1/tests/test_src_handler.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_src_handler_acked.py` & `cfdp_py-0.1.1/tests/test_src_handler_acked.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_src_handler_nak_closure.py` & `cfdp_py-0.1.1/tests/test_src_handler_nak_closure.py`

 * *Files identical despite different names*

### Comparing `cfdp-py-0.1.0/tests/test_src_handler_nak_no_closure.py` & `cfdp_py-0.1.1/tests/test_src_handler_nak_no_closure.py`

 * *Files identical despite different names*

