# Comparing `tmp/ragdaemon-0.1.9.tar.gz` & `tmp/ragdaemon-0.2.0.tar.gz`

## Comparing `ragdaemon-0.1.9.tar` & `ragdaemon-0.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tutorial.ipynb
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/app.py
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/context.py
--rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/errors.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/get_paths.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/graph.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/llm.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/conftest.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_comments.py
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_daemon.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_database.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_get_paths.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/test_sample.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/app.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/context.py
+-rw-r--r--   0        0        0     5857 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/errors.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/get_paths.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3728 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_comments.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_daemon.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_database.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_get_paths.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/test_sample.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.2.0/PKG-INFO
```

### Comparing `ragdaemon-0.1.9/tutorial.ipynb` & `ragdaemon-0.2.0/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/.github/workflows/run-tests.yml` & `ragdaemon-0.2.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/app.py` & `ragdaemon-0.2.0/ragdaemon/app.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/context.py` & `ragdaemon-0.2.0/ragdaemon/context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/daemon.py` & `ragdaemon-0.2.0/ragdaemon/daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/get_paths.py` & `ragdaemon-0.2.0/ragdaemon/get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/graph.py` & `ragdaemon-0.2.0/ragdaemon/graph.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/utils.py` & `ragdaemon-0.2.0/ragdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/__init__.py` & `ragdaemon-0.2.0/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.2.0/ragdaemon/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/chunker.py` & `ragdaemon-0.2.0/ragdaemon/annotators/chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.2.0/ragdaemon/annotators/chunker_line.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.2.0/ragdaemon/annotators/chunker_llm.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/diff.py` & `ragdaemon-0.2.0/ragdaemon/annotators/diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.2.0/ragdaemon/annotators/hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.2.0/ragdaemon/annotators/layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/database/__init__.py` & `ragdaemon-0.2.0/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/database/chroma_database.py` & `ragdaemon-0.2.0/ragdaemon/database/chroma_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/database/database.py` & `ragdaemon-0.2.0/ragdaemon/database/database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/database/lite_database.py` & `ragdaemon-0.2.0/ragdaemon/database/lite_database.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/static/favicon.ico` & `ragdaemon-0.2.0/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.2.0/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/static/js/main.js` & `ragdaemon-0.2.0/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.2.0/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/static/js/three/node.js` & `ragdaemon-0.2.0/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.2.0/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/ragdaemon/templates/index.html` & `ragdaemon-0.2.0/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/conftest.py` & `ragdaemon-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/test_comments.py` & `ragdaemon-0.2.0/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/test_context.py` & `ragdaemon-0.2.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/test_daemon.py` & `ragdaemon-0.2.0/tests/test_daemon.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/test_get_paths.py` & `ragdaemon-0.2.0/tests/test_get_paths.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/test_sample.py` & `ragdaemon-0.2.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/annotators/test_chunker.py` & `ragdaemon-0.2.0/tests/annotators/test_chunker.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/annotators/test_diff.py` & `ragdaemon-0.2.0/tests/annotators/test_diff.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/annotators/test_hierarchy.py` & `ragdaemon-0.2.0/tests/annotators/test_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.2.0/tests/annotators/test_layout_hierarchy.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/data/chunker_graph.json` & `ragdaemon-0.2.0/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/data/context_message.txt` & `ragdaemon-0.2.0/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/data/diff_graph.json` & `ragdaemon-0.2.0/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/data/hierarchy_graph.json` & `ragdaemon-0.2.0/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.2.0/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/tests/sample/src/interface.py` & `ragdaemon-0.2.0/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/LICENSE` & `ragdaemon-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/README.md` & `ragdaemon-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.9/pyproject.toml` & `ragdaemon-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.1.9"
+version = "0.2.0"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
     "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
     "networkx==3.2.1",
-    "spiceai~=0.1.0",
+    "spiceai~=0.2.0",
     "starlette==0.36.3",
     "tqdm==4.66.2",
     "uvicorn==0.27.1",
 ]
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ragdaemon-0.1.9/PKG-INFO` & `ragdaemon-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.1.9
+Version: 0.2.0
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: dict2xml==1.7.5
 Requires-Dist: fastapi==0.109.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: networkx==3.2.1
-Requires-Dist: spiceai~=0.1.0
+Requires-Dist: spiceai~=0.2.0
 Requires-Dist: starlette==0.36.3
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: uvicorn==0.27.1
 Provides-Extra: dev
 Requires-Dist: pyright; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-asyncio; extra == 'dev'
```

