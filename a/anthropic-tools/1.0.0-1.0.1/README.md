# Comparing `tmp/anthropic_tools-1.0.0.tar.gz` & `tmp/anthropic_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic_tools-1.0.0.tar", max compression
+gzip compressed data, was "anthropic_tools-1.0.1.tar", max compression
```

## Comparing `anthropic_tools-1.0.0.tar` & `anthropic_tools-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2024-04-22 16:46:31.037124 anthropic_tools-1.0.0/LICENSE
--rw-r--r--   0        0        0     3310 2024-04-22 22:09:43.914043 anthropic_tools-1.0.0/README.md
--rw-r--r--   0        0        0      889 2024-04-22 20:16:31.859294 anthropic_tools-1.0.0/anthropic_tools/__init__.py
--rw-r--r--   0        0        0    12632 2024-04-22 21:56:29.098001 anthropic_tools-1.0.0/anthropic_tools/conversation.py
--rw-r--r--   0        0        0     2470 2024-04-22 20:39:52.045700 anthropic_tools-1.0.0/anthropic_tools/exceptions.py
--rw-r--r--   0        0        0      160 2024-04-22 20:40:05.815842 anthropic_tools-1.0.0/anthropic_tools/json_type.py
--rw-r--r--   0        0        0      159 2024-04-22 20:49:27.759652 anthropic_tools-1.0.0/anthropic_tools/parsers/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-22 20:48:40.778167 anthropic_tools-1.0.0/anthropic_tools/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2024-04-22 20:40:34.494139 anthropic_tools-1.0.0/anthropic_tools/parsers/bool_parser.py
--rw-r--r--   0        0        0     2412 2024-04-22 20:48:46.943230 anthropic_tools-1.0.0/anthropic_tools/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      763 2024-04-22 20:48:53.886302 anthropic_tools-1.0.0/anthropic_tools/parsers/default.py
--rw-r--r--   0        0        0     1246 2024-04-22 20:48:58.508350 anthropic_tools-1.0.0/anthropic_tools/parsers/dict_parser.py
--rw-r--r--   0        0        0     1444 2024-04-22 20:49:02.614393 anthropic_tools-1.0.0/anthropic_tools/parsers/enum_parser.py
--rw-r--r--   0        0        0      568 2024-04-22 20:40:34.495139 anthropic_tools-1.0.0/anthropic_tools/parsers/float_parser.py
--rw-r--r--   0        0        0      690 2024-04-22 20:40:34.495139 anthropic_tools-1.0.0/anthropic_tools/parsers/int_parser.py
--rw-r--r--   0        0        0     1045 2024-04-22 20:49:09.782467 anthropic_tools-1.0.0/anthropic_tools/parsers/list_parser.py
--rw-r--r--   0        0        0      737 2024-04-22 20:49:14.145512 anthropic_tools-1.0.0/anthropic_tools/parsers/none_parser.py
--rw-r--r--   0        0        0     2060 2024-04-22 20:48:20.336955 anthropic_tools-1.0.0/anthropic_tools/parsers/parser.py
--rw-r--r--   0        0        0      204 2024-04-22 20:40:34.494139 anthropic_tools-1.0.0/anthropic_tools/parsers/str_parser.py
--rw-r--r--   0        0        0     1306 2024-04-22 20:48:31.624072 anthropic_tools-1.0.0/anthropic_tools/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2024-04-22 16:46:31.041123 anthropic_tools-1.0.0/anthropic_tools/py.typed
--rw-r--r--   0        0        0      474 2024-04-22 19:50:54.869324 anthropic_tools-1.0.0/anthropic_tools/tools/__init__.py
--rw-r--r--   0        0        0     3681 2024-04-22 19:56:42.985960 anthropic_tools-1.0.0/anthropic_tools/tools/basic_set.py
--rw-r--r--   0        0        0     4617 2024-04-22 20:37:21.181140 anthropic_tools-1.0.0/anthropic_tools/tools/sets.py
--rw-r--r--   0        0        0     5022 2024-04-22 21:35:07.068691 anthropic_tools-1.0.0/anthropic_tools/tools/tools.py
--rw-r--r--   0        0        0     1666 2024-04-22 20:10:11.922359 anthropic_tools-1.0.0/anthropic_tools/tools/union.py
--rw-r--r--   0        0        0     6994 2024-04-22 21:28:58.204932 anthropic_tools-1.0.0/anthropic_tools/tools/wrapper.py
--rw-r--r--   0        0        0      823 2024-04-22 20:55:16.727243 anthropic_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 anthropic_tools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-22 16:46:31.037124 anthropic_tools-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3310 2024-04-22 22:09:43.914043 anthropic_tools-1.0.1/README.md
+-rw-r--r--   0        0        0     1009 2024-04-23 06:28:43.226974 anthropic_tools-1.0.1/anthropic_tools/__init__.py
+-rw-r--r--   0        0        0    12147 2024-04-23 07:03:38.304159 anthropic_tools-1.0.1/anthropic_tools/conversation.py
+-rw-r--r--   0        0        0     2470 2024-04-22 20:39:52.045700 anthropic_tools-1.0.1/anthropic_tools/exceptions.py
+-rw-r--r--   0        0        0      160 2024-04-22 20:40:05.815842 anthropic_tools-1.0.1/anthropic_tools/json_type.py
+-rw-r--r--   0        0        0      159 2024-04-22 20:49:27.759652 anthropic_tools-1.0.1/anthropic_tools/parsers/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-22 20:48:40.778167 anthropic_tools-1.0.1/anthropic_tools/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2024-04-22 20:40:34.494139 anthropic_tools-1.0.1/anthropic_tools/parsers/bool_parser.py
+-rw-r--r--   0        0        0     2412 2024-04-22 20:48:46.943230 anthropic_tools-1.0.1/anthropic_tools/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      763 2024-04-22 20:48:53.886302 anthropic_tools-1.0.1/anthropic_tools/parsers/default.py
+-rw-r--r--   0        0        0     1246 2024-04-22 20:48:58.508350 anthropic_tools-1.0.1/anthropic_tools/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1444 2024-04-22 20:49:02.614393 anthropic_tools-1.0.1/anthropic_tools/parsers/enum_parser.py
+-rw-r--r--   0        0        0      568 2024-04-22 20:40:34.495139 anthropic_tools-1.0.1/anthropic_tools/parsers/float_parser.py
+-rw-r--r--   0        0        0      690 2024-04-22 20:40:34.495139 anthropic_tools-1.0.1/anthropic_tools/parsers/int_parser.py
+-rw-r--r--   0        0        0     1045 2024-04-22 20:49:09.782467 anthropic_tools-1.0.1/anthropic_tools/parsers/list_parser.py
+-rw-r--r--   0        0        0      737 2024-04-22 20:49:14.145512 anthropic_tools-1.0.1/anthropic_tools/parsers/none_parser.py
+-rw-r--r--   0        0        0     2060 2024-04-22 20:48:20.336955 anthropic_tools-1.0.1/anthropic_tools/parsers/parser.py
+-rw-r--r--   0        0        0      204 2024-04-22 20:40:34.494139 anthropic_tools-1.0.1/anthropic_tools/parsers/str_parser.py
+-rw-r--r--   0        0        0     1306 2024-04-22 20:48:31.624072 anthropic_tools-1.0.1/anthropic_tools/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2024-04-22 16:46:31.041123 anthropic_tools-1.0.1/anthropic_tools/py.typed
+-rw-r--r--   0        0        0      607 2024-04-23 06:27:38.362284 anthropic_tools-1.0.1/anthropic_tools/tools/__init__.py
+-rw-r--r--   0        0        0     3681 2024-04-22 19:56:42.985960 anthropic_tools-1.0.1/anthropic_tools/tools/basic_set.py
+-rw-r--r--   0        0        0     4617 2024-04-22 20:37:21.181140 anthropic_tools-1.0.1/anthropic_tools/tools/sets.py
+-rw-r--r--   0        0        0     6356 2024-04-23 06:58:42.666208 anthropic_tools-1.0.1/anthropic_tools/tools/tools.py
+-rw-r--r--   0        0        0     1666 2024-04-22 20:10:11.922359 anthropic_tools-1.0.1/anthropic_tools/tools/union.py
+-rw-r--r--   0        0        0     6994 2024-04-22 21:28:58.204932 anthropic_tools-1.0.1/anthropic_tools/tools/wrapper.py
+-rw-r--r--   0        0        0      823 2024-04-23 06:30:25.243944 anthropic_tools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4339 1970-01-01 00:00:00.000000 anthropic_tools-1.0.1/PKG-INFO
```

### Comparing `anthropic_tools-1.0.0/LICENSE` & `anthropic_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/README.md` & `anthropic_tools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/__init__.py` & `anthropic_tools-1.0.1/anthropic_tools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,35 +7,41 @@
     NonSerializableOutputError,
     ToolNotFoundError,
 )
 from .parsers import ArgSchemaParser, defargparsers
 from .tools import (
     AnthropicTool,
     BasicToolSet,
+    ImageToolOutput,
     MutableToolSet,
     RawToolResult,
+    TextToolOutput,
+    ToolOutput,
     ToolResult,
     ToolSet,
     ToolWrapper,
     UnionSkillSet,
     WrapperConfig,
 )
 
 __all__ = [
     "AnthropicTool",
+    "AnthropicToolsError",
+    "ArgSchemaParser",
     "BasicToolSet",
+    "BrokenSchemaError",
+    "CannotParseTypeError",
+    "Conversation",
+    "ImageToolOutput",
+    "MutableToolSet",
+    "NonSerializableOutputError",
+    "RawToolResult",
+    "TextToolOutput",
+    "ToolNotFoundError",
+    "ToolOutput",
     "ToolResult",
     "ToolSet",
     "ToolWrapper",
-    "MutableToolSet",
-    "RawToolResult",
     "UnionSkillSet",
     "WrapperConfig",
-    "AnthropicToolsError",
-    "BrokenSchemaError",
-    "CannotParseTypeError",
-    "NonSerializableOutputError",
-    "ToolNotFoundError",
-    "ArgSchemaParser",
     "defargparsers",
-    "Conversation",
 ]
```

### Comparing `anthropic_tools-1.0.0/anthropic_tools/conversation.py` & `anthropic_tools-1.0.1/anthropic_tools/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """A conversation with Anthropic Claude."""
 from __future__ import annotations
 import time
-from typing import Any, Callable, Iterable, TYPE_CHECKING, overload
+from typing import Any, Callable, TYPE_CHECKING, overload
 
 from anthropic import Anthropic, RateLimitError
-from anthropic.types import ImageBlockParam, TextBlockParam
+from anthropic.types import TextBlockParam
 from anthropic.types.beta.tools import (
     ToolParam,
     ToolResultBlockParam,
-    ToolUseBlockParam,
-    ToolsBetaContentBlock,
     ToolsBetaMessage,
     ToolsBetaMessageParam,
 )
 
 from .tools.union import UnionSkillSet
 
 if TYPE_CHECKING:
@@ -136,25 +134,23 @@
         return self.client.beta.tools.messages.create(
             model=self.model,
             max_tokens=max_tokens,
             tools=self.tools_schema,
             messages=self.messages,
         )
 
-    def _add_tool_result(self, tool_result: ToolResult) -> bool:
+    def add_tool_result(self, tool_result: ToolResult) -> bool:
         """Add a tool result to the conversation.
 
         Args:
             tool_result (ToolResult): The tool result to add.
 
         Returns:
             bool: True if the tool result was added, False otherwise.
         """
-        if tool_result.content is None:
-            return False
         if tool_result.interpret_return_as_response:
             self.add_message(
                 {
                     "role": tool_result.response_role,
                     "content": tool_result.blocks or tool_result.content,
                 }
             )
@@ -172,25 +168,14 @@
                             is_error=False,
                         )
                     ],
                 )
             )
         return True
 
-    def add_tool_result(self, tool_result: ToolResult) -> bool:
-        """Add a tool result to the conversation.
-
-        Args:
-            tool_result (ToolResult): The tool result to add.
-
-        Returns:
-            bool: True if the tool result was added, False otherwise.
-        """
-        return self._add_tool_result(tool_result)
-
     def run_tool_if_needed(self) -> bool:
         """Run a tool if needed.
 
         Returns:
             bool: True if a tool was run, False otherwise.
         """
         if not self.messages:
```

### Comparing `anthropic_tools-1.0.0/anthropic_tools/exceptions.py` & `anthropic_tools-1.0.1/anthropic_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/atomic_type_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/dataclass_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/default.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/default.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/dict_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/enum_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/float_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/float_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/int_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/list_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/none_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/parsers/union_parser.py` & `anthropic_tools-1.0.1/anthropic_tools/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/tools/basic_set.py` & `anthropic_tools-1.0.1/anthropic_tools/tools/basic_set.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/tools/sets.py` & `anthropic_tools-1.0.1/anthropic_tools/tools/sets.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/tools/tools.py` & `anthropic_tools-1.0.1/anthropic_tools/tools/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """A definition of a tool set that can be used by Anthropic Claude."""
 from __future__ import annotations
 from dataclasses import dataclass
 import json
-from typing import Any, Iterable, Literal, Protocol, TYPE_CHECKING, runtime_checkable
+from typing import (
+    Any,
+    Iterable,
+    Literal,
+    Protocol,
+    TYPE_CHECKING,
+    TypeGuard,
+    runtime_checkable,
+)
 
 from anthropic.types import ImageBlockParam, TextBlockParam
 from anthropic.types.beta.tools import (
     ToolResultBlockParam,
     ToolUseBlockParam,
     ToolsBetaContentBlock,
 )
+from anthropic.types.image_block_param import Source
 
 from ..exceptions import NonSerializableOutputError
 
 if TYPE_CHECKING:
     from anthropic.types.beta.tools import ToolParam
     from ..json_type import JsonType
 
@@ -72,14 +81,34 @@
         """Check if the return value of the Anthropic Tool should be interpreted as
         the assistant's response.
         """
         ...  # pylint: disable=unnecessary-ellipsis
 
 
 @dataclass
+class TextToolOutput:
+    """The text output of a tool."""
+
+    content: str
+    is_error: bool = False
+    type: Literal["text"] = "text"
+
+
+@dataclass
+class ImageToolOutput:
+    """The image output of a tool."""
+
+    source: Source
+    type: Literal["image"] = "image"
+
+
+ToolOutput = TextToolOutput | ImageToolOutput
+
+
+@dataclass
 class RawToolResult:
     """The raw result of an Anthropic Tool.
 
     The raw result can be serialized and converted to content blocks.
     """
 
     result: Any
@@ -130,26 +159,26 @@
     """Represents the result of using an Anthropic Tool.
 
     The result can include the content blocks and the interpreted return value.
     """
 
     use_id: str
     name: str
-    raw_result: RawToolResult | None
+    raw_result: RawToolResult
     interpret_return_as_response: bool = False
     response_role: Literal["user", "assistant"] = "user"
 
     @property
-    def content(self) -> str | None:
+    def content(self) -> str:
         """Get the content of the Tool Result.
 
         Returns:
             The content of the Tool Result, or None if there is no raw result.
         """
-        return self.raw_result.serialized if self.raw_result else None
+        return self.raw_result.serialized
 
     @property
     def blocks(
         self,
     ) -> (
         str
         | Iterable[
@@ -157,26 +186,54 @@
             | TextBlockParam
             | ImageBlockParam
             | ToolUseBlockParam
             | ToolResultBlockParam
         ]
         | None
     ):
-        """Get the content blocks of the Tool Result. Only meaningful for tools that
-        have interpret_return_as_response set to True. An example use case is a tool
-        that returns image content blocks.
-
-        Returns:
-            The content blocks of the Tool Result, or None if there is no raw result.
-        """
-        return None if self.raw_result is None else self.raw_result.as_content
+        """Get the content blocks of the Tool Result. Only meaningful for tools
+        that have interpret_return_as_response set to True. An example use case
+        is a tool that returns image content blocks.
+
+        Returns:
+            The content blocks of the Tool Result,
+                or None if there is no raw result.
+        """
+        result = self.raw_result.as_content
+        if self._is_tool_output(result):
+            return [
+                ToolResultBlockParam(
+                    type="tool_result",
+                    tool_use_id=self.use_id,
+                    content=[{"type": "text", "text": block.content}],
+                    is_error=block.is_error,
+                )
+                if block.type == "text"
+                else ImageBlockParam(type="image", source=block.source)
+                for block in result
+            ]
+        return result
 
     @property
     def result(self) -> Any | None:
         """Get the result of the underlying function call.
 
         Returns:
             The raw result of the function call
         """
         if self.raw_result:
             return self.raw_result.result
         return None
+
+    def _is_tool_output(self, result: Any) -> TypeGuard[list[ToolOutput]]:
+        """Check if the result is a list of ToolOutput objects.
+
+        Args:
+            result: The result to check.
+
+        Returns:
+            True if the result is a list of ToolOutput objects,
+                False otherwise.
+        """
+        return isinstance(result, list) and all(
+            isinstance(item, (TextToolOutput, ImageToolOutput)) for item in result
+        )
```

### Comparing `anthropic_tools-1.0.0/anthropic_tools/tools/union.py` & `anthropic_tools-1.0.1/anthropic_tools/tools/union.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/anthropic_tools/tools/wrapper.py` & `anthropic_tools-1.0.1/anthropic_tools/tools/wrapper.py`

 * *Files identical despite different names*

### Comparing `anthropic_tools-1.0.0/pyproject.toml` & `anthropic_tools-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anthropic-tools"
-version = "1.0.0"
+version = "1.0.1"
 description = "Simplifies the usage of Anthropic Claude's tool use by generating the schemas and parsing the responses for you."
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/rizerphe/anthropic-tools"
 documentation = "https://anthropic-tools.readthedocs.io/"
 keywords = ["nlp", "anthropic", "claude", "claude3", "claude-api", "wrapper", "functions", "typing", "docstring", "docstrings", "decorators", "signatures", "parsing"]
 license = "MIT"
```

### Comparing `anthropic_tools-1.0.0/PKG-INFO` & `anthropic_tools-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic-tools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simplifies the usage of Anthropic Claude's tool use by generating the schemas and parsing the responses for you.
 Home-page: https://github.com/rizerphe/anthropic-tools
 License: MIT
 Keywords: nlp,anthropic,claude,claude3,claude-api,wrapper,functions,typing,docstring,docstrings,decorators,signatures,parsing
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

