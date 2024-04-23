# Comparing `tmp/connect_four_lib-1.3.0.tar.gz` & `tmp/connect_four_lib-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connect_four_lib-1.3.0.tar", max compression
+gzip compressed data, was "connect_four_lib-1.3.1.tar", max compression
```

## Comparing `connect_four_lib-1.3.0.tar` & `connect_four_lib-1.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      472 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/README.md
--rw-r--r--   0        0        0      557 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/__init__.py
--rw-r--r--   0        0        0       67 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/config.py
--rw-r--r--   0        0        0     3887 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/connect_four_engine.py
--rw-r--r--   0        0        0     2371 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/connect_four_heuristic.py
--rw-r--r--   0        0        0     4578 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/connect_four_judge.py
--rw-r--r--   0        0        0      721 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/connect_four_player.py
--rw-r--r--   0        0        0      643 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/point.py
--rw-r--r--   0        0        0      426 2024-04-12 16:33:43.928784 connect_four_lib-1.3.0/src/connect_four_lib/utils/speed.py
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 connect_four_lib-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      472 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/README.md
+-rw-r--r--   0        0        0      557 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/config.py
+-rw-r--r--   0        0        0     3887 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/connect_four_engine.py
+-rw-r--r--   0        0        0     2371 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/connect_four_heuristic.py
+-rw-r--r--   0        0        0     4578 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/connect_four_judge.py
+-rw-r--r--   0        0        0      747 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/connect_four_player.py
+-rw-r--r--   0        0        0      643 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/point.py
+-rw-r--r--   0        0        0      426 2024-04-23 12:36:13.087720 connect_four_lib-1.3.1/src/connect_four_lib/utils/speed.py
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 connect_four_lib-1.3.1/PKG-INFO
```

### Comparing `connect_four_lib-1.3.0/pyproject.toml` & `connect_four_lib-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "connect-four-lib"
-version = "1.3.0"
+version = "1.3.1"
 description = "A library for connect 4 game"
 authors = ["game-ai-platform-team"]
 readme = "README.md"
 packages = [{ include = "connect_four_lib/**/*.py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `connect_four_lib-1.3.0/src/connect_four_lib/connect_four_engine.py` & `connect_four_lib-1.3.1/src/connect_four_lib/connect_four_engine.py`

 * *Files identical despite different names*

### Comparing `connect_four_lib-1.3.0/src/connect_four_lib/connect_four_heuristic.py` & `connect_four_lib-1.3.1/src/connect_four_lib/connect_four_heuristic.py`

 * *Files identical despite different names*

### Comparing `connect_four_lib-1.3.0/src/connect_four_lib/connect_four_judge.py` & `connect_four_lib-1.3.1/src/connect_four_lib/connect_four_judge.py`

 * *Files identical despite different names*

### Comparing `connect_four_lib-1.3.0/src/connect_four_lib/connect_four_player.py` & `connect_four_lib-1.3.1/src/connect_four_lib/connect_four_player.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 class ConnectFourPlayer(Player):
     def __init__(self, elo) -> None:
         super().__init__()
 
         self.engine: ConnectFourEngine = ConnectFourEngine()
         self.elo: int = elo
 
-    def play(self, move) -> str:
-        self.engine.add_move(move)
+    def play(self, move: str) -> str:
+        if move:
+            self.engine.add_move(move)
 
         new_move = self.engine.get_best_move()
 
         if not new_move:
             new_move = self.engine.get_random_move()
             print("random move")
```

### Comparing `connect_four_lib-1.3.0/src/connect_four_lib/point.py` & `connect_four_lib-1.3.1/src/connect_four_lib/point.py`

 * *Files identical despite different names*

### Comparing `connect_four_lib-1.3.0/PKG-INFO` & `connect_four_lib-1.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connect-four-lib
-Version: 1.3.0
+Version: 1.3.1
 Summary: A library for connect 4 game
 Author: game-ai-platform-team
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

