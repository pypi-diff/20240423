# Comparing `tmp/clovers-0.1.4.tar.gz` & `tmp/clovers-0.1.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clovers-0.1.4.tar", max compression
+gzip compressed data, was "clovers-0.1.4.post1.tar", max compression
```

## Comparing `clovers-0.1.4.tar` & `clovers-0.1.4.post1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-15 12:37:36.317298 clovers-0.1.4/clovers/__init__.py
--rw-r--r--   0        0        0     4524 2024-04-23 16:15:55.123859 clovers-0.1.4/clovers/core/adapter.py
--rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.4/clovers/core/config.py
--rw-r--r--   0        0        0     6654 2024-04-23 16:16:46.779330 clovers-0.1.4/clovers/core/plugin.py
--rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.4/clovers/utils/library.py
--rw-r--r--   0        0        0    10961 2024-04-16 04:46:17.581644 clovers-0.1.4/clovers/utils/linecard.py
--rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.4/clovers/utils/tools.py
--rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.4/LICENSE
--rw-r--r--   0        0        0      645 2024-04-23 16:16:29.188815 clovers-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    10284 2024-04-23 16:13:55.973406 clovers-0.1.4/README.md
--rw-r--r--   0        0        0    10627 1970-01-01 00:00:00.000000 clovers-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 12:37:36.317298 clovers-0.1.4.post1/clovers/__init__.py
+-rw-r--r--   0        0        0     4524 2024-04-23 16:15:55.123859 clovers-0.1.4.post1/clovers/core/adapter.py
+-rw-r--r--   0        0        0      582 2024-04-15 03:01:44.120813 clovers-0.1.4.post1/clovers/core/config.py
+-rw-r--r--   0        0        0     6659 2024-04-23 17:07:21.079825 clovers-0.1.4.post1/clovers/core/plugin.py
+-rw-r--r--   0        0        0     2774 2024-04-15 02:23:00.885679 clovers-0.1.4.post1/clovers/utils/library.py
+-rw-r--r--   0        0        0    10961 2024-04-16 04:46:17.581644 clovers-0.1.4.post1/clovers/utils/linecard.py
+-rw-r--r--   0        0        0     1884 2024-04-15 08:48:00.582248 clovers-0.1.4.post1/clovers/utils/tools.py
+-rw-r--r--   0        0        0     1086 2024-04-15 03:18:25.255783 clovers-0.1.4.post1/LICENSE
+-rw-r--r--   0        0        0      647 2024-04-23 17:08:39.503342 clovers-0.1.4.post1/pyproject.toml
+-rw-r--r--   0        0        0    10284 2024-04-23 16:13:55.973406 clovers-0.1.4.post1/README.md
+-rw-r--r--   0        0        0    10633 1970-01-01 00:00:00.000000 clovers-0.1.4.post1/PKG-INFO
```

### Comparing `clovers-0.1.4/clovers/core/adapter.py` & `clovers-0.1.4.post1/clovers/core/adapter.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4/clovers/core/config.py` & `clovers-0.1.4.post1/clovers/core/config.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4/clovers/core/plugin.py` & `clovers-0.1.4.post1/clovers/core/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self,
         raw_command: str,
         args: Sequence[str],
     ):
         self.raw_command = raw_command
         self.args = args
         self.kwargs: dict = {}
-        self.get_kwargs: dict[str, Callable[..., Coroutine]]
+        self.get_kwargs: dict[str, Callable[..., Coroutine]] = {}
 
 
 class Handle:
     func: Callable[[Event], Coroutine[None, None, Result | None]]
 
     def __init__(self, extra_args: Iterable[str], get_extra_args: Iterable[str]):
         self.extra_args = extra_args
```

### Comparing `clovers-0.1.4/clovers/utils/library.py` & `clovers-0.1.4.post1/clovers/utils/library.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4/clovers/utils/linecard.py` & `clovers-0.1.4.post1/clovers/utils/linecard.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4/clovers/utils/tools.py` & `clovers-0.1.4.post1/clovers/utils/tools.py`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4/LICENSE` & `clovers-0.1.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4/pyproject.toml` & `clovers-0.1.4.post1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clovers"
-version = "0.1.4"
+version = "0.1.4r1"
 description = ""
 authors = ["KarisAya <1048827424@qq.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 toml = "^0.10.2"
```

### Comparing `clovers-0.1.4/README.md` & `clovers-0.1.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `clovers-0.1.4/PKG-INFO` & `clovers-0.1.4.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clovers
-Version: 0.1.4
+Version: 0.1.4.post1
 Summary: 
 Author: KarisAya
 Author-email: 1048827424@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

