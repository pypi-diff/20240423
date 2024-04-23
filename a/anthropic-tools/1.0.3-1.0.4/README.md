# Comparing `tmp/anthropic_tools-1.0.3.tar.gz` & `tmp/anthropic_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic_tools-1.0.3.tar", max compression
+gzip compressed data, was "anthropic_tools-1.0.4.tar", max compression
```

## Comparing `anthropic_tools-1.0.3.tar` & `anthropic_tools-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2024-04-22 16:46:31.037124 anthropic_tools-1.0.3/LICENSE
--rw-r--r--   0        0        0     3310 2024-04-22 22:09:43.914043 anthropic_tools-1.0.3/README.md
--rw-r--r--   0        0        0     1009 2024-04-23 06:28:43.226974 anthropic_tools-1.0.3/anthropic_tools/__init__.py
--rw-r--r--   0        0        0    12147 2024-04-23 07:03:38.304159 anthropic_tools-1.0.3/anthropic_tools/conversation.py
--rw-r--r--   0        0        0     2470 2024-04-22 20:39:52.045700 anthropic_tools-1.0.3/anthropic_tools/exceptions.py
--rw-r--r--   0        0        0      160 2024-04-22 20:40:05.815842 anthropic_tools-1.0.3/anthropic_tools/json_type.py
--rw-r--r--   0        0        0      159 2024-04-22 20:49:27.759652 anthropic_tools-1.0.3/anthropic_tools/parsers/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-22 20:48:40.778167 anthropic_tools-1.0.3/anthropic_tools/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2024-04-22 20:40:34.494139 anthropic_tools-1.0.3/anthropic_tools/parsers/bool_parser.py
--rw-r--r--   0        0        0     2412 2024-04-22 20:48:46.943230 anthropic_tools-1.0.3/anthropic_tools/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      763 2024-04-22 20:48:53.886302 anthropic_tools-1.0.3/anthropic_tools/parsers/default.py
--rw-r--r--   0        0        0     1246 2024-04-22 20:48:58.508350 anthropic_tools-1.0.3/anthropic_tools/parsers/dict_parser.py
--rw-r--r--   0        0        0     1444 2024-04-22 20:49:02.614393 anthropic_tools-1.0.3/anthropic_tools/parsers/enum_parser.py
--rw-r--r--   0        0        0      568 2024-04-22 20:40:34.495139 anthropic_tools-1.0.3/anthropic_tools/parsers/float_parser.py
--rw-r--r--   0        0        0      690 2024-04-22 20:40:34.495139 anthropic_tools-1.0.3/anthropic_tools/parsers/int_parser.py
--rw-r--r--   0        0        0     1045 2024-04-22 20:49:09.782467 anthropic_tools-1.0.3/anthropic_tools/parsers/list_parser.py
--rw-r--r--   0        0        0      737 2024-04-22 20:49:14.145512 anthropic_tools-1.0.3/anthropic_tools/parsers/none_parser.py
--rw-r--r--   0        0        0     2060 2024-04-22 20:48:20.336955 anthropic_tools-1.0.3/anthropic_tools/parsers/parser.py
--rw-r--r--   0        0        0      204 2024-04-22 20:40:34.494139 anthropic_tools-1.0.3/anthropic_tools/parsers/str_parser.py
--rw-r--r--   0        0        0     1306 2024-04-22 20:48:31.624072 anthropic_tools-1.0.3/anthropic_tools/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2024-04-22 16:46:31.041123 anthropic_tools-1.0.3/anthropic_tools/py.typed
--rw-r--r--   0        0        0      607 2024-04-23 06:27:38.362284 anthropic_tools-1.0.3/anthropic_tools/tools/__init__.py
--rw-r--r--   0        0        0     3681 2024-04-22 19:56:42.985960 anthropic_tools-1.0.3/anthropic_tools/tools/basic_set.py
--rw-r--r--   0        0        0     4617 2024-04-22 20:37:21.181140 anthropic_tools-1.0.3/anthropic_tools/tools/sets.py
--rw-r--r--   0        0        0     7887 2024-04-23 18:46:16.935345 anthropic_tools-1.0.3/anthropic_tools/tools/tools.py
--rw-r--r--   0        0        0     1666 2024-04-22 20:10:11.922359 anthropic_tools-1.0.3/anthropic_tools/tools/union.py
--rw-r--r--   0        0        0     6994 2024-04-22 21:28:58.204932 anthropic_tools-1.0.3/anthropic_tools/tools/wrapper.py
--rw-r--r--   0        0        0      823 2024-04-23 18:46:28.881462 anthropic_tools-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 anthropic_tools-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-22 16:46:31.037124 anthropic_tools-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3310 2024-04-22 22:09:43.914043 anthropic_tools-1.0.4/README.md
+-rw-r--r--   0        0        0     1009 2024-04-23 06:28:43.226974 anthropic_tools-1.0.4/anthropic_tools/__init__.py
+-rw-r--r--   0        0        0    11870 2024-04-23 20:55:37.008602 anthropic_tools-1.0.4/anthropic_tools/conversation.py
+-rw-r--r--   0        0        0     2470 2024-04-22 20:39:52.045700 anthropic_tools-1.0.4/anthropic_tools/exceptions.py
+-rw-r--r--   0        0        0      160 2024-04-22 20:40:05.815842 anthropic_tools-1.0.4/anthropic_tools/json_type.py
+-rw-r--r--   0        0        0      159 2024-04-22 20:49:27.759652 anthropic_tools-1.0.4/anthropic_tools/parsers/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-22 20:48:40.778167 anthropic_tools-1.0.4/anthropic_tools/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2024-04-22 20:40:34.494139 anthropic_tools-1.0.4/anthropic_tools/parsers/bool_parser.py
+-rw-r--r--   0        0        0     2412 2024-04-22 20:48:46.943230 anthropic_tools-1.0.4/anthropic_tools/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      763 2024-04-22 20:48:53.886302 anthropic_tools-1.0.4/anthropic_tools/parsers/default.py
+-rw-r--r--   0        0        0     1246 2024-04-22 20:48:58.508350 anthropic_tools-1.0.4/anthropic_tools/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1444 2024-04-22 20:49:02.614393 anthropic_tools-1.0.4/anthropic_tools/parsers/enum_parser.py
+-rw-r--r--   0        0        0      568 2024-04-22 20:40:34.495139 anthropic_tools-1.0.4/anthropic_tools/parsers/float_parser.py
+-rw-r--r--   0        0        0      690 2024-04-22 20:40:34.495139 anthropic_tools-1.0.4/anthropic_tools/parsers/int_parser.py
+-rw-r--r--   0        0        0     1045 2024-04-22 20:49:09.782467 anthropic_tools-1.0.4/anthropic_tools/parsers/list_parser.py
+-rw-r--r--   0        0        0      737 2024-04-22 20:49:14.145512 anthropic_tools-1.0.4/anthropic_tools/parsers/none_parser.py
+-rw-r--r--   0        0        0     2060 2024-04-22 20:48:20.336955 anthropic_tools-1.0.4/anthropic_tools/parsers/parser.py
+-rw-r--r--   0        0        0      204 2024-04-22 20:40:34.494139 anthropic_tools-1.0.4/anthropic_tools/parsers/str_parser.py
+-rw-r--r--   0        0        0     1306 2024-04-22 20:48:31.624072 anthropic_tools-1.0.4/anthropic_tools/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2024-04-22 16:46:31.041123 anthropic_tools-1.0.4/anthropic_tools/py.typed
+-rw-r--r--   0        0        0      607 2024-04-23 06:27:38.362284 anthropic_tools-1.0.4/anthropic_tools/tools/__init__.py
+-rw-r--r--   0        0        0     3681 2024-04-22 19:56:42.985960 anthropic_tools-1.0.4/anthropic_tools/tools/basic_set.py
+-rw-r--r--   0        0        0     4617 2024-04-22 20:37:21.181140 anthropic_tools-1.0.4/anthropic_tools/tools/sets.py
+-rw-r--r--   0        0        0     7946 2024-04-23 20:52:51.424946 anthropic_tools-1.0.4/anthropic_tools/tools/tools.py
+-rw-r--r--   0        0        0     1666 2024-04-22 20:10:11.922359 anthropic_tools-1.0.4/anthropic_tools/tools/union.py
+-rw-r--r--   0        0        0     6994 2024-04-22 21:28:58.204932 anthropic_tools-1.0.4/anthropic_tools/tools/wrapper.py
+-rw-r--r--   0        0        0      823 2024-04-23 20:57:20.680638 anthropic_tools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 anthropic_tools-1.0.4/PKG-INFO
```

### Comparing `anthropic_tools-1.0.3/LICENSE` & `anthropic_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/README.md` & `anthropic_tools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/__init__.py` & `anthropic_tools-1.0.4/anthropic_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/conversation.py` & `anthropic_tools-1.0.4/anthropic_tools/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,21 +239,15 @@
             list[ToolsBetaMessageParam]: The response messages,
                 both from Claude and tools.
         """
         generated = []
         while True:
             message = self.generate_message(retries=retries, max_tokens=max_tokens)
             generated.append(message)
-            if self._contains_call(message):
-                # Force tools to get used, so that the next message
-                # contains something other than tool results
-                generated.append(
-                    self.generate_message(retries=retries, max_tokens=max_tokens)
-                )
-            else:
+            if not self._contains_call(message):
                 return generated
 
     @overload
     def add_tool(self, tool: AnthropicTool) -> AnthropicTool:
         ...
 
     @overload
```

### Comparing `anthropic_tools-1.0.3/anthropic_tools/exceptions.py` & `anthropic_tools-1.0.4/anthropic_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/atomic_type_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/dataclass_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/default.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/default.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/dict_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/enum_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/float_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/int_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/list_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/none_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/parsers/union_parser.py` & `anthropic_tools-1.0.4/anthropic_tools/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/tools/__init__.py` & `anthropic_tools-1.0.4/anthropic_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/tools/basic_set.py` & `anthropic_tools-1.0.4/anthropic_tools/tools/basic_set.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/tools/sets.py` & `anthropic_tools-1.0.4/anthropic_tools/tools/sets.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/tools/tools.py` & `anthropic_tools-1.0.4/anthropic_tools/tools/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -207,37 +207,39 @@
                     content=[{"type": "text", "text": block.content}],
                     is_error=block.is_error,
                 )
                 if block.type == "text"
                 else ImageBlockParam(type="image", source=block.source)
                 for block in result
             ]
-            if not any(block.type == "text" for block in result):
+            if not any(block["type"] == "tool_result" for block in blocks):
                 blocks.insert(
                     0,
                     ToolResultBlockParam(
                         type="tool_result",
                         tool_use_id=self.use_id,
                     ),
                 )
-            if len([block for block in result if block.type == "tool_result"]) > 1:
+            if len([block for block in blocks if block["type"] == "tool_result"]) > 1:
                 # Replace the first result block with all concatenated results:
                 first_text_block = next(
                     block for block in blocks if block["type"] == "tool_result"
                 )
                 first_text_block["content"] = sum(
                     [
                         list(block.get("content", []))
                         for block in blocks
                         if block["type"] == "tool_result"
                     ],
                     [],
                 )
                 first_text_block["is_error"] = any(
-                    block.is_error for block in result if block.type == "tool_result"
+                    block["is_error"]
+                    for block in blocks
+                    if block["type"] == "tool_result"
                 )
                 # Delete all but the first one now:
                 new_blocks = []
                 first_done = False
                 for block in blocks:
                     if block["type"] == "tool_result":
                         if first_done:
```

### Comparing `anthropic_tools-1.0.3/anthropic_tools/tools/union.py` & `anthropic_tools-1.0.4/anthropic_tools/tools/union.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/anthropic_tools/tools/wrapper.py` & `anthropic_tools-1.0.4/anthropic_tools/tools/wrapper.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.3/pyproject.toml` & `anthropic_tools-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anthropic-tools"
-version = "1.0.3"
+version = "1.0.4"
 description = "Simplifies the usage of Anthropic Claude's tool use by generating the schemas and parsing the responses for you."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/rizerphe/anthropic-tools"
 documentation = "https://anthropic-tools.readthedocs.io/"
 keywords = ["nlp", "anthropic", "claude", "claude3", "claude-api", "wrapper", "functions", "typing", "docstring", "docstrings", "decorators", "signatures", "parsing"]
 license = "MIT"
```

### Comparing `anthropic_tools-1.0.3/PKG-INFO` & `anthropic_tools-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Simplifies the usage of Anthropic Claude's tool use by generating the schemas and parsing the responses for you.
 Home-page: https://github.com/rizerphe/anthropic-tools
 License: MIT
 Keywords: nlp,anthropic,claude,claude3,claude-api,wrapper,functions,typing,docstring,docstrings,decorators,signatures,parsing
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

