# Comparing `tmp/ragdaemon-0.2.0.tar.gz` & `tmp/ragdaemon-0.2.1.tar.gz`

## Comparing `ragdaemon-0.2.0.tar` & `ragdaemon-0.2.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/app.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/context.py
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/llm.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_comments.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_database.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_sample.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0   103029 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tags
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/app.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/context.py
+-rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/test_comments.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/test_context.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/test_database.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/test_sample.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.1/PKG-INFO
```

### Comparing `ragdaemon-0.2.0/tutorial.ipynb` & `ragdaemon-0.2.1/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/.github/workflows/run-tests.yml` & `ragdaemon-0.2.1/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/app.py` & `ragdaemon-0.2.1/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/context.py` & `ragdaemon-0.2.1/ragdaemon/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Dict, Optional, Union
 
+from dict2xml import dict2xml
 from ragdaemon.annotators.diff import parse_diff_id
 from ragdaemon.database import Database
 from ragdaemon.graph import KnowledgeGraph
-from ragdaemon.errors import RagdaemonError
-from ragdaemon.utils import parse_path_ref, get_document, hash_str
-
-
-from typing import Union, Dict
-from dict2xml import dict2xml
+from ragdaemon.utils import get_document, hash_str, parse_path_ref
 
 NestedStrDict = Union[str, Dict[str, "NestedStrDict"]]
 
 
 class Comment:
     def __init__(
         self,
@@ -151,22 +147,31 @@
             return
         self.context[path_str]["diffs"].remove(id)
         self.context[path_str]["tags"].remove("diff")
         if not self.context[path_str]["lines"] and not self.context[path_str]["diffs"]:
             del self.context[path_str]
         return id
 
-    def render(self) -> str:
+    def render(self, use_xml: bool = False, use_tags: bool = False) -> str:
         """Return a formatted context message for the given nodes."""
         output = ""
         for path_str, data in self.context.items():
             if output:
                 output += "\n"
-            tags = "" if not data["tags"] else f" ({', '.join(sorted(data['tags']))})"
-            output += f"{path_str}{tags}\n"
+
+            if use_tags and data["tags"]:
+                tags = f" ({', '.join(sorted(data['tags']))})"
+            else:
+                tags = ""
+
+            if use_xml:
+                output += f"<{path_str}>{tags}\n"
+            else:
+                output += f"{path_str}{tags}\n"
+
             if 0 in data["comments"]:
                 output += render_comments(data["comments"][0]) + "\n"
             if data["lines"]:
                 file_lines = data["document"].splitlines()
                 last_rendered = 0
                 for line in sorted(data["lines"]):
                     if line - last_rendered > 1:
@@ -176,14 +181,16 @@
                         line_content += "\n" + render_comments(data["comments"][line])
                     output += line_content + "\n"
                     last_rendered = line
                 if last_rendered < len(file_lines) - 1:
                     output += "...\n"
             if data["diffs"]:
                 output += self.render_diffs(data["diffs"])
+            if use_xml:
+                output += f"</{path_str}>\n"
         return output
 
     def render_diffs(self, ids: set[str]) -> str:
         output = ""
         diff_str, _, _ = parse_diff_id(next(iter(ids)))
         git_command = "--git diff"
         if diff_str != "DEFAULT":
```

### Comparing `ragdaemon-0.2.0/ragdaemon/daemon.py` & `ragdaemon-0.2.1/ragdaemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,19 @@
                 last_updated = _last_updated
                 _update_task = asyncio.create_task(self.update())
 
     def search(self, query: str, n: Optional[int] = None) -> list[dict[str, Any]]:
         """Return a sorted list of nodes that match the query."""
         return self.db.query_graph(query, self.graph, n=n)
 
+    def get_document(self, filename: str) -> str:
+        checksum = self.graph.nodes[filename]["checksum"]
+        document = self.db.get(checksum)["documents"][0]
+        return document
+
     def get_context(
         self,
         query: str,
         context_builder: Optional[ContextBuilder] = None,
         max_tokens: int = 8000,
         auto_tokens: int = 0,
         model: str = DEFAULT_COMPLETION_MODEL,
```

### Comparing `ragdaemon-0.2.0/ragdaemon/get_paths.py` & `ragdaemon-0.2.1/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/graph.py` & `ragdaemon-0.2.1/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/utils.py` & `ragdaemon-0.2.1/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/__init__.py` & `ragdaemon-0.2.1/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.2.1/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/chunker.py` & `ragdaemon-0.2.1/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.2.1/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.2.1/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/diff.py` & `ragdaemon-0.2.1/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.2.1/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.2.1/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/database/__init__.py` & `ragdaemon-0.2.1/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/database/chroma_database.py` & `ragdaemon-0.2.1/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/database/database.py` & `ragdaemon-0.2.1/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/database/lite_database.py` & `ragdaemon-0.2.1/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/static/favicon.ico` & `ragdaemon-0.2.1/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.2.1/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/static/js/main.js` & `ragdaemon-0.2.1/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.2.1/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/static/js/three/node.js` & `ragdaemon-0.2.1/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.2.1/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/ragdaemon/templates/index.html` & `ragdaemon-0.2.1/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/conftest.py` & `ragdaemon-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/test_comments.py` & `ragdaemon-0.2.1/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/test_context.py` & `ragdaemon-0.2.1/tests/test_context.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             "lines": set([1, 2, 3, 4, 15]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
             "comments": dict(),
         }
     }
-    actual = context.render()
+    actual = context.render(use_tags=True)
     assert (
         actual
         == """\
 src/interface.py (test-flag)
 1:import argparse
 2:import re
 3:
@@ -41,15 +41,15 @@
             "lines": set([5, 6, 7, 8, 9, 10, 11, 12, 13, 14]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
             "comments": dict(),
         }
     }
-    actual = context.render()
+    actual = context.render(use_tags=True)
     assert (
         actual
         == """\
 src/interface.py (test-flag)
 ...
 5:def parse_arguments():
 6:    parser = argparse.ArgumentParser(description="Basic Calculator")
```

### Comparing `ragdaemon-0.2.0/tests/test_daemon.py` & `ragdaemon-0.2.1/tests/test_daemon.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,24 +13,26 @@
 @pytest.mark.asyncio
 async def test_daemon_get_context(cwd):
     # Full Context
     annotators = default_annotators()
     del annotators["diff"]
     daemon = Daemon(cwd.resolve(), annotators=annotators)
     await daemon.update()
-    actual = daemon.get_context("test", max_tokens=1000).render()
+    actual = daemon.get_context("test", max_tokens=1000).render(use_tags=True)
 
     with open("tests/data/context_message.txt", "r") as f:
         expected = f.read()
     assert get_message_chunk_set(actual) == get_message_chunk_set(expected)
 
     # Included Files
     context = daemon.get_context("test")
     context.add_ref("src/interface.py:11-12", tags=["user-included"])
-    actual = daemon.get_context("test", context_builder=context, auto_tokens=0).render()
+    actual = daemon.get_context("test", context_builder=context, auto_tokens=0).render(
+        use_tags=True
+    )
     assert (
         actual
         == """\
 src/interface.py (user-included)
 ...
 11:    match = re.match(r"(\\d+)(\\D)(\\d+)", args.operation)
 12:    if match is None:
```

### Comparing `ragdaemon-0.2.0/tests/test_get_paths.py` & `ragdaemon-0.2.1/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/test_sample.py` & `ragdaemon-0.2.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/annotators/test_chunker.py` & `ragdaemon-0.2.1/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/annotators/test_diff.py` & `ragdaemon-0.2.1/tests/annotators/test_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 import pytest
-
 from networkx.readwrite import json_graph
+
 from ragdaemon.annotators.diff import Diff, get_chunks_from_diff, parse_diff_id
 from ragdaemon.context import ContextBuilder
 from ragdaemon.daemon import Daemon
 from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import get_git_diff
 
 
@@ -59,15 +59,15 @@
     await daemon.update(refresh=True)
 
     # Only diffs
     context = ContextBuilder(daemon.graph, daemon.db)
     context.add_diff("DEFAULT:main.py")
     context.add_diff("DEFAULT:src/operations.py:1-5")
     context.add_diff("DEFAULT:src/operations.py:8-10")
-    actual = context.render()
+    actual = context.render(use_tags=True)
     assert (
         actual
         == """\
 main.py (diff)
 --git diff
 @@ -1,23 +0,0 @@
 -from src.interface import parse_arguments, render_response
@@ -113,15 +113,15 @@
 """
     )
 
     # Diffs with files and chunks
     context.remove_diff("DEFAULT:main.py")
     context.add_diff("DEFAULT:src/operations.py:1-5")
     context.add_ref("src/operations.py", tags=["user-included"])
-    actual = context.render()
+    actual = context.render(use_tags=True)
     assert (
         actual
         == """\
 src/operations.py (diff, user-included)
 1:import math
 2: #modified
 3: #modified
```

### Comparing `ragdaemon-0.2.0/tests/annotators/test_hierarchy.py` & `ragdaemon-0.2.1/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.2.1/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/data/chunker_graph.json` & `ragdaemon-0.2.1/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/data/context_message.txt` & `ragdaemon-0.2.1/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/data/diff_graph.json` & `ragdaemon-0.2.1/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/data/hierarchy_graph.json` & `ragdaemon-0.2.1/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.2.1/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/tests/sample/src/interface.py` & `ragdaemon-0.2.1/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/LICENSE` & `ragdaemon-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/README.md` & `ragdaemon-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.2.0/pyproject.toml` & `ragdaemon-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.2.0"
+version = "0.2.1"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
```

### Comparing `ragdaemon-0.2.0/PKG-INFO` & `ragdaemon-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

