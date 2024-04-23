# Comparing `tmp/haskellian-0.3.6.tar.gz` & `tmp/haskellian-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haskellian-0.3.6.tar", last modified: Mon Apr 22 05:15:49 2024, max compression
+gzip compressed data, was "haskellian-0.3.7.tar", last modified: Mon Apr 22 10:09:38 2024, max compression
```

## Comparing `haskellian-0.3.6.tar` & `haskellian-0.3.7.tar`

### file list

```diff
@@ -1,62 +1,68 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.435969 haskellian-0.3.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-22 05:15:49.435969 haskellian-0.3.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1154 2024-04-21 19:18:11.000000 haskellian-0.3.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-22 05:15:46.000000 haskellian-0.3.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 05:15:49.435969 haskellian-0.3.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.415969 haskellian-0.3.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.415969 haskellian-0.3.6/src/haskellian/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      156 2024-04-21 08:31:50.000000 haskellian-0.3.6/src/haskellian/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-21 14:43:52.000000 haskellian-0.3.6/src/haskellian/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.425969 haskellian-0.3.6/src/haskellian/asyn_iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:25:49.000000 haskellian-0.3.6/src/haskellian/asyn_iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      441 2024-04-21 14:39:06.000000 haskellian-0.3.6/src/haskellian/asyn_iter/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2234 2024-04-21 14:39:41.000000 haskellian-0.3.6/src/haskellian/asyn_iter/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2125 2024-04-21 14:40:29.000000 haskellian-0.3.6/src/haskellian/asyn_iter/iter.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 14:38:54.000000 haskellian-0.3.6/src/haskellian/asyn_iter/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      886 2024-04-21 14:38:19.000000 haskellian-0.3.6/src/haskellian/asyn_iter/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      650 2024-04-21 14:40:28.000000 haskellian-0.3.6/src/haskellian/asyn_iter/prefetching.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.425969 haskellian-0.3.6/src/haskellian/classes/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 09:04:50.000000 haskellian-0.3.6/src/haskellian/classes/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-04-21 09:04:51.000000 haskellian-0.3.6/src/haskellian/classes/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      578 2024-04-21 10:23:51.000000 haskellian-0.3.6/src/haskellian/classes/applicative.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      413 2024-04-21 10:23:57.000000 haskellian-0.3.6/src/haskellian/classes/functor.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      832 2024-04-21 14:05:41.000000 haskellian-0.3.6/src/haskellian/classes/monad.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-21 15:09:01.000000 haskellian-0.3.6/src/haskellian/config.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.425969 haskellian-0.3.6/src/haskellian/either/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 10:31:26.000000 haskellian-0.3.6/src/haskellian/either/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      405 2024-04-21 10:39:57.000000 haskellian-0.3.6/src/haskellian/either/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-04-21 14:05:41.000000 haskellian-0.3.6/src/haskellian/either/either.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1285 2024-04-21 10:38:12.000000 haskellian-0.3.6/src/haskellian/either/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-21 10:36:36.000000 haskellian-0.3.6/src/haskellian/either/narrowing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-21 10:39:34.000000 haskellian-0.3.6/src/haskellian/either/pydantic.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.425969 haskellian-0.3.6/src/haskellian/iter/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 13:06:20.000000 haskellian-0.3.6/src/haskellian/iter/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      681 2024-04-22 05:13:35.000000 haskellian-0.3.6/src/haskellian/iter/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-21 13:51:48.000000 haskellian-0.3.6/src/haskellian/iter/basics.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-04-21 13:53:19.000000 haskellian-0.3.6/src/haskellian/iter/batching.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-21 13:53:13.000000 haskellian-0.3.6/src/haskellian/iter/indexing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2697 2024-04-22 05:12:09.000000 haskellian-0.3.6/src/haskellian/iter/iter.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      473 2024-04-21 13:52:51.000000 haskellian-0.3.6/src/haskellian/iter/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4144 2024-04-21 13:58:56.000000 haskellian-0.3.6/src/haskellian/iter/nested.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1140 2024-04-21 13:59:18.000000 haskellian-0.3.6/src/haskellian/iter/slicing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-04-21 19:17:41.000000 haskellian-0.3.6/src/haskellian/iter/transposing.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1003 2024-04-21 13:59:47.000000 haskellian-0.3.6/src/haskellian/iter/zipping.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.425969 haskellian-0.3.6/src/haskellian/pipe/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       22 2024-04-21 10:07:57.000000 haskellian-0.3.6/src/haskellian/pipe/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-04-21 14:05:41.000000 haskellian-0.3.6/src/haskellian/pipe/pipe.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.425969 haskellian-0.3.6/src/haskellian/promise/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:06:21.000000 haskellian-0.3.6/src/haskellian/promise/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      259 2024-04-21 17:53:58.000000 haskellian-0.3.6/src/haskellian/promise/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1144 2024-04-21 17:53:35.000000 haskellian-0.3.6/src/haskellian/promise/funcs.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-21 14:17:11.000000 haskellian-0.3.6/src/haskellian/promise/lifting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      600 2024-04-21 14:35:57.000000 haskellian-0.3.6/src/haskellian/promise/managed.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1053 2024-04-21 14:21:51.000000 haskellian-0.3.6/src/haskellian/promise/promise.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.425969 haskellian-0.3.6/src/haskellian/thunk/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-21 10:06:39.000000 haskellian-0.3.6/src/haskellian/thunk/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-04-21 14:05:41.000000 haskellian-0.3.6/src/haskellian/thunk/thunk.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 05:15:49.435969 haskellian-0.3.6/src/haskellian.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-22 05:15:49.000000 haskellian-0.3.6/src/haskellian.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1596 2024-04-22 05:15:49.000000 haskellian-0.3.6/src/haskellian.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 05:15:49.000000 haskellian-0.3.6/src/haskellian.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-22 05:15:49.000000 haskellian-0.3.6/src/haskellian.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-22 05:15:49.000000 haskellian-0.3.6/src/haskellian.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.126844 haskellian-0.3.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-22 10:09:38.126844 haskellian-0.3.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1154 2024-04-22 05:15:53.000000 haskellian-0.3.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      514 2024-04-22 10:09:32.000000 haskellian-0.3.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-22 10:09:38.126844 haskellian-0.3.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.086843 haskellian-0.3.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.096843 haskellian-0.3.7/src/haskellian/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      156 2024-04-21 08:31:50.000000 haskellian-0.3.7/src/haskellian/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      494 2024-04-22 10:03:32.000000 haskellian-0.3.7/src/haskellian/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.106843 haskellian-0.3.7/src/haskellian/asyn_iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:25:49.000000 haskellian-0.3.7/src/haskellian/asyn_iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      441 2024-04-21 14:39:06.000000 haskellian-0.3.7/src/haskellian/asyn_iter/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2234 2024-04-21 14:39:41.000000 haskellian-0.3.7/src/haskellian/asyn_iter/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2125 2024-04-21 14:40:29.000000 haskellian-0.3.7/src/haskellian/asyn_iter/iter.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      490 2024-04-21 14:38:54.000000 haskellian-0.3.7/src/haskellian/asyn_iter/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      886 2024-04-21 14:38:19.000000 haskellian-0.3.7/src/haskellian/asyn_iter/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      650 2024-04-21 14:40:28.000000 haskellian-0.3.7/src/haskellian/asyn_iter/prefetching.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.106843 haskellian-0.3.7/src/haskellian/classes/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 09:04:50.000000 haskellian-0.3.7/src/haskellian/classes/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      137 2024-04-21 09:04:51.000000 haskellian-0.3.7/src/haskellian/classes/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      578 2024-04-21 10:23:51.000000 haskellian-0.3.7/src/haskellian/classes/applicative.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      413 2024-04-21 10:23:57.000000 haskellian-0.3.7/src/haskellian/classes/functor.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      832 2024-04-21 14:05:41.000000 haskellian-0.3.7/src/haskellian/classes/monad.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-21 15:09:01.000000 haskellian-0.3.7/src/haskellian/config.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.106843 haskellian-0.3.7/src/haskellian/either/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 10:31:26.000000 haskellian-0.3.7/src/haskellian/either/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      405 2024-04-21 10:39:57.000000 haskellian-0.3.7/src/haskellian/either/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2644 2024-04-21 14:05:41.000000 haskellian-0.3.7/src/haskellian/either/either.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1285 2024-04-21 10:38:12.000000 haskellian-0.3.7/src/haskellian/either/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      381 2024-04-21 10:36:36.000000 haskellian-0.3.7/src/haskellian/either/narrowing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      464 2024-04-21 10:39:34.000000 haskellian-0.3.7/src/haskellian/either/pydantic.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.106843 haskellian-0.3.7/src/haskellian/funcs/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-22 09:49:11.000000 haskellian-0.3.7/src/haskellian/funcs/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      167 2024-04-22 10:08:12.000000 haskellian-0.3.7/src/haskellian/funcs/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1477 2024-04-22 09:57:25.000000 haskellian-0.3.7/src/haskellian/funcs/_flow.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1512 2024-04-22 10:00:34.000000 haskellian-0.3.7/src/haskellian/funcs/_pipe.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      996 2024-04-22 10:07:57.000000 haskellian-0.3.7/src/haskellian/funcs/curried.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.116843 haskellian-0.3.7/src/haskellian/iter/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 13:06:20.000000 haskellian-0.3.7/src/haskellian/iter/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      681 2024-04-22 05:13:35.000000 haskellian-0.3.7/src/haskellian/iter/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      799 2024-04-21 13:51:48.000000 haskellian-0.3.7/src/haskellian/iter/basics.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      680 2024-04-21 13:53:19.000000 haskellian-0.3.7/src/haskellian/iter/batching.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      485 2024-04-21 13:53:13.000000 haskellian-0.3.7/src/haskellian/iter/indexing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2928 2024-04-22 06:38:01.000000 haskellian-0.3.7/src/haskellian/iter/iter.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      473 2024-04-21 13:52:51.000000 haskellian-0.3.7/src/haskellian/iter/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4144 2024-04-21 13:58:56.000000 haskellian-0.3.7/src/haskellian/iter/nested.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1140 2024-04-21 13:59:18.000000 haskellian-0.3.7/src/haskellian/iter/slicing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      869 2024-04-21 19:17:41.000000 haskellian-0.3.7/src/haskellian/iter/transposing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1003 2024-04-21 13:59:47.000000 haskellian-0.3.7/src/haskellian/iter/zipping.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.116843 haskellian-0.3.7/src/haskellian/pipe/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       22 2024-04-21 10:07:57.000000 haskellian-0.3.7/src/haskellian/pipe/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      767 2024-04-21 14:05:41.000000 haskellian-0.3.7/src/haskellian/pipe/pipe.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.126844 haskellian-0.3.7/src/haskellian/promise/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-21 14:06:21.000000 haskellian-0.3.7/src/haskellian/promise/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      259 2024-04-21 17:53:58.000000 haskellian-0.3.7/src/haskellian/promise/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1173 2024-04-22 07:58:14.000000 haskellian-0.3.7/src/haskellian/promise/funcs.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-21 14:17:11.000000 haskellian-0.3.7/src/haskellian/promise/lifting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      600 2024-04-21 14:35:57.000000 haskellian-0.3.7/src/haskellian/promise/managed.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1053 2024-04-21 14:21:51.000000 haskellian-0.3.7/src/haskellian/promise/promise.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.126844 haskellian-0.3.7/src/haskellian/thunk/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       24 2024-04-21 10:06:39.000000 haskellian-0.3.7/src/haskellian/thunk/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      933 2024-04-21 14:05:41.000000 haskellian-0.3.7/src/haskellian/thunk/thunk.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-22 10:09:38.126844 haskellian-0.3.7/src/haskellian.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1539 2024-04-22 10:09:38.000000 haskellian-0.3.7/src/haskellian.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1755 2024-04-22 10:09:38.000000 haskellian-0.3.7/src/haskellian.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-22 10:09:38.000000 haskellian-0.3.7/src/haskellian.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-22 10:09:38.000000 haskellian-0.3.7/src/haskellian.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       11 2024-04-22 10:09:38.000000 haskellian-0.3.7/src/haskellian.egg-info/top_level.txt
```

### Comparing `haskellian-0.3.6/PKG-INFO` & `haskellian-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haskellian
-Version: 0.3.6
+Version: 0.3.7
 Summary: The functional programming library you need
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/haskellian.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: pydantic
```

### Comparing `haskellian-0.3.6/README.md` & `haskellian-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/pyproject.toml` & `haskellian-0.3.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "haskellian"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "The functional programming library you need"
 dependencies = [
   "lazy-loader"
 ]
```

### Comparing `haskellian-0.3.6/src/haskellian/asyn_iter/funcs.py` & `haskellian-0.3.7/src/haskellian/asyn_iter/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/asyn_iter/iter.py` & `haskellian-0.3.7/src/haskellian/asyn_iter/iter.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/asyn_iter/managed.py` & `haskellian-0.3.7/src/haskellian/asyn_iter/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/asyn_iter/prefetching.py` & `haskellian-0.3.7/src/haskellian/asyn_iter/prefetching.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/classes/applicative.py` & `haskellian-0.3.7/src/haskellian/classes/applicative.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/classes/monad.py` & `haskellian-0.3.7/src/haskellian/classes/monad.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/either/either.py` & `haskellian-0.3.7/src/haskellian/either/either.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/either/funcs.py` & `haskellian-0.3.7/src/haskellian/either/funcs.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/iter/__init__.pyi` & `haskellian-0.3.7/src/haskellian/iter/__init__.pyi`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/iter/basics.py` & `haskellian-0.3.7/src/haskellian/iter/basics.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/iter/batching.py` & `haskellian-0.3.7/src/haskellian/iter/batching.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/iter/iter.py` & `haskellian-0.3.7/src/haskellian/iter/iter.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,14 +36,18 @@
   
   def bind(self, f: Callable[[A], Iterable[B]]) -> 'Iter[B]':
     return I.flatmap(f, self)
   
   def flatmap(self, f: Callable[[A], Iterable[B]]) -> 'Iter[B]':
     return self.bind(f)
   
+  def iflatmap(self, f: Callable[[int, A], Iterable[B]]) -> 'Iter[B]':
+    """`flatmap` with indices"""
+    return self.enumerate().flatmap(lambda xs: f(*xs))
+  
   def map(self, f: Callable[[A], B]) -> 'Iter[B]':
     return Iter(map(f, self))
   
   fmap = map
 
   def __or__(self, f: Callable[[A], B]) -> 'Iter[B]':
     """Alias of `map`"""
@@ -71,14 +75,17 @@
   def split(self, n: int) -> 'tuple[Iter[A], Iter[A]]':
     xs, ys = I.split(n, self)
     return Iter(xs), Iter(ys)
   
   def take(self, n: int) -> 'Iter[A]':
     return I.take(n, self)
   
+  def skip(self, n: int) -> 'Iter[A]':
+    return I.skip(n, self)
+  
   def take_while(self, f: Callable[[A], bool]) -> 'Iter[A]':
     return I.take_while(f, self)
   
   def at(self, i: int) -> A | None:
     for x in islice(self, i, None):
       return x
```

### Comparing `haskellian-0.3.6/src/haskellian/iter/nested.py` & `haskellian-0.3.7/src/haskellian/iter/nested.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/iter/slicing.py` & `haskellian-0.3.7/src/haskellian/iter/slicing.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/iter/transposing.py` & `haskellian-0.3.7/src/haskellian/iter/transposing.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/iter/zipping.py` & `haskellian-0.3.7/src/haskellian/iter/zipping.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/pipe/pipe.py` & `haskellian-0.3.7/src/haskellian/pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/promise/funcs.py` & `haskellian-0.3.7/src/haskellian/promise/funcs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from haskellian import DEBUG_IMPORTS, iter as I, promise as P
+from haskellian import DEBUG_IMPORTS, iter as I, promise as P, Promise
 if DEBUG_IMPORTS:
   print('Import:', __name__)
 from typing import TypeVar, Callable, Awaitable, Mapping, Iterable, overload
 from inspect import isawaitable
 import asyncio
 
 A = TypeVar('A')
@@ -23,21 +23,23 @@
   await asyncio.sleep(secs)
 
 @P.lift
 async def wait(x: A | Awaitable[A]) -> A:
   return await x if isawaitable(x) else x # type: ignore
 
 @overload
-async def all(xs: Iterable[Awaitable[A]]) -> list[A]: ...
+def all(xs: Iterable[Awaitable[A]]) -> Promise[list[A]]: ...
 @overload
-async def all(xs: Mapping[str, Awaitable[A]]) -> dict[str, A]: ...
+def all(xs: Mapping[str, Awaitable[A]]) -> Promise[dict[str, A]]: ...
 
+@P.lift
 async def all(xs):
   if isinstance(xs, Mapping):
     keys, values = I.unzip(xs.items())
     results = await asyncio.gather(*values)
     return dict(zip(keys, results))
   else:
     return await asyncio.gather(*xs)
-  
+
+@P.lift
 async def all2d(xxs: Iterable[Iterable[Awaitable[A]]]) -> list[list[A]]:
   return await all([all(xs) for xs in xxs])
```

### Comparing `haskellian-0.3.6/src/haskellian/promise/managed.py` & `haskellian-0.3.7/src/haskellian/promise/managed.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/promise/promise.py` & `haskellian-0.3.7/src/haskellian/promise/promise.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian/thunk/thunk.py` & `haskellian-0.3.7/src/haskellian/thunk/thunk.py`

 * *Files identical despite different names*

### Comparing `haskellian-0.3.6/src/haskellian.egg-info/PKG-INFO` & `haskellian-0.3.7/src/haskellian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haskellian
-Version: 0.3.6
+Version: 0.3.7
 Summary: The functional programming library you need
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/haskellian.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Provides-Extra: pydantic
```

### Comparing `haskellian-0.3.6/src/haskellian.egg-info/SOURCES.txt` & `haskellian-0.3.7/src/haskellian.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,19 @@
 src/haskellian/classes/monad.py
 src/haskellian/either/__init__.py
 src/haskellian/either/__init__.pyi
 src/haskellian/either/either.py
 src/haskellian/either/funcs.py
 src/haskellian/either/narrowing.py
 src/haskellian/either/pydantic.py
+src/haskellian/funcs/__init__.py
+src/haskellian/funcs/__init__.pyi
+src/haskellian/funcs/_flow.py
+src/haskellian/funcs/_pipe.py
+src/haskellian/funcs/curried.py
 src/haskellian/iter/__init__.py
 src/haskellian/iter/__init__.pyi
 src/haskellian/iter/basics.py
 src/haskellian/iter/batching.py
 src/haskellian/iter/indexing.py
 src/haskellian/iter/iter.py
 src/haskellian/iter/lifting.py
```

