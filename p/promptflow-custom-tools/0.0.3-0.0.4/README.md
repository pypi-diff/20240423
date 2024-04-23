# Comparing `tmp/promptflow_custom_tools-0.0.3.tar.gz` & `tmp/promptflow_custom_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptflow_custom_tools-0.0.3.tar", last modified: Mon Apr 22 20:29:54 2024, max compression
+gzip compressed data, was "promptflow_custom_tools-0.0.4.tar", last modified: Mon Apr 22 21:18:26 2024, max compression
```

## Comparing `promptflow_custom_tools-0.0.3.tar` & `promptflow_custom_tools-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 20:29:54.683211 promptflow_custom_tools-0.0.3/
--rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      128 2024-04-22 20:29:54.682206 promptflow_custom_tools-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 20:29:54.649014 promptflow_custom_tools-0.0.3/promptflow_custom_tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:29:54.678190 promptflow_custom_tools-0.0.3/promptflow_custom_tools/tools/
--rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools/tools/__init__.py
--rw-rw-rw-   0        0        0     2142 2024-04-19 20:30:44.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools/tools/claude.py
--rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools/tools/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:29:54.678190 promptflow_custom_tools-0.0.3/promptflow_custom_tools/yamls/
--rw-rw-rw-   0        0        0     6657 2024-04-22 20:11:06.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools/yamls/claude.yaml
-drwxrwxrwx   0        0        0        0 2024-04-22 20:29:54.675684 promptflow_custom_tools-0.0.3/promptflow_custom_tools.egg-info/
--rw-rw-rw-   0        0        0      128 2024-04-22 20:29:54.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-04-22 20:29:54.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 20:29:54.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-22 20:29:54.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2024-04-22 20:29:54.000000 promptflow_custom_tools-0.0.3/promptflow_custom_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-22 20:29:54.683211 promptflow_custom_tools-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      442 2024-04-22 20:29:38.000000 promptflow_custom_tools-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:29:54.680204 promptflow_custom_tools-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.3/tests/__init__.py
--rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.3/tests/test_claude.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:18:26.433355 promptflow_custom_tools-0.0.4/
+-rw-rw-rw-   0        0        0     1072 2024-04-22 20:09:19.000000 promptflow_custom_tools-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       44 2024-04-22 20:28:40.000000 promptflow_custom_tools-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      128 2024-04-22 21:18:26.433355 promptflow_custom_tools-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2024-04-22 20:28:57.000000 promptflow_custom_tools-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 21:18:26.406030 promptflow_custom_tools-0.0.4/promptflow_custom_tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:18:26.429658 promptflow_custom_tools-0.0.4/promptflow_custom_tools/tools/
+-rw-rw-rw-   0        0        0       82 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools/tools/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-04-22 21:17:52.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools/tools/claude.py
+-rw-rw-rw-   0        0        0      553 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools/tools/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:18:26.430176 promptflow_custom_tools-0.0.4/promptflow_custom_tools/yamls/
+-rw-rw-rw-   0        0        0     6657 2024-04-22 20:11:06.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools/yamls/claude.yaml
+drwxrwxrwx   0        0        0        0 2024-04-22 21:18:26.427003 promptflow_custom_tools-0.0.4/promptflow_custom_tools.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-04-22 21:18:26.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-04-22 21:18:26.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 21:18:26.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-22 21:18:26.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2024-04-22 21:18:26.000000 promptflow_custom_tools-0.0.4/promptflow_custom_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 21:18:26.433355 promptflow_custom_tools-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      442 2024-04-22 21:18:24.000000 promptflow_custom_tools-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 21:18:26.432339 promptflow_custom_tools-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-19 13:18:32.000000 promptflow_custom_tools-0.0.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      709 2024-04-22 20:27:24.000000 promptflow_custom_tools-0.0.4/tests/test_claude.py
```

### Comparing `promptflow_custom_tools-0.0.3/LICENSE` & `promptflow_custom_tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.3/promptflow_custom_tools/tools/claude.py` & `promptflow_custom_tools-0.0.4/promptflow_custom_tools/tools/claude.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,19 +14,14 @@
     :type api_key: Secret
     :param api_base: The api base.
     :type api_base: String
     """
     api_key: Secret
     api_base: str = "This is a fake api base."
 
-def get_models(prefix: str = "", size: int = 10, **kwargs) -> List[Dict[str, Union[str, int, float, list, Dict]]]:
-    words = ["apple", "banana", "cherry", "date", "elderberry", "fig", "grape", "honeydew", "kiwi", "lemon"]
-
-    return words
-
 @tool
 def generate(
     connection: ClaudeConnection,
     prompt: PromptTemplate,
     model: str = "claude-3-opus-20240229",
     temperature: float  = 1,
     top_p: float = 1.0,
```

### Comparing `promptflow_custom_tools-0.0.3/promptflow_custom_tools/tools/utils.py` & `promptflow_custom_tools-0.0.4/promptflow_custom_tools/tools/utils.py`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.3/promptflow_custom_tools/yamls/claude.yaml` & `promptflow_custom_tools-0.0.4/promptflow_custom_tools/yamls/claude.yaml`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.3/promptflow_custom_tools.egg-info/SOURCES.txt` & `promptflow_custom_tools-0.0.4/promptflow_custom_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptflow_custom_tools-0.0.3/tests/test_claude.py` & `promptflow_custom_tools-0.0.4/tests/test_claude.py`

 * *Files identical despite different names*

