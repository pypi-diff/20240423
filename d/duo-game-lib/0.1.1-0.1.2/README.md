# Comparing `tmp/duo_game_lib-0.1.1.tar.gz` & `tmp/duo_game_lib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duo_game_lib-0.1.1.tar", max compression
+gzip compressed data, was "duo_game_lib-0.1.2.tar", max compression
```

## Comparing `duo_game_lib-0.1.1.tar` & `duo_game_lib-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      395 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/README.md
--rw-r--r--   0        0        0      526 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/__init__.py
--rw-r--r--   0        0        0     3124 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/game.py
--rw-r--r--   0        0        0      275 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/game_state.py
--rw-r--r--   0        0        0     1710 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/judge.py
--rw-r--r--   0        0        0     1409 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/move.py
--rw-r--r--   0        0        0      998 2024-04-16 10:57:31.966615 duo_game_lib-0.1.1/src/duo_game_lib/player.py
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 duo_game_lib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      395 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/README.md
+-rw-r--r--   0        0        0      526 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/src/duo_game_lib/__init__.py
+-rw-r--r--   0        0        0     3125 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/src/duo_game_lib/game.py
+-rw-r--r--   0        0        0      275 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/src/duo_game_lib/game_state.py
+-rw-r--r--   0        0        0     1710 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/src/duo_game_lib/judge.py
+-rw-r--r--   0        0        0     1409 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/src/duo_game_lib/move.py
+-rw-r--r--   0        0        0      998 2024-04-23 12:59:22.414043 duo_game_lib-0.1.2/src/duo_game_lib/player.py
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 duo_game_lib-0.1.2/PKG-INFO
```

### Comparing `duo_game_lib-0.1.1/pyproject.toml` & `duo_game_lib-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duo-game-lib"
-version = "0.1.1"
+version = "0.1.2"
 description = "Logic for turn-based duo game"
 authors = ["game-ai-platform-team"]
 readme = "README.md"
 packages = [{ include = "duo_game_lib/**/*.py", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `duo_game_lib-0.1.1/src/duo_game_lib/game.py` & `duo_game_lib-0.1.2/src/duo_game_lib/game.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             if i == turns:
                 state = GameState.MAX_TURNS
                 break
 
             player = self.__players[i % 2]
             move, elapsed_time = self.__play_one_move(player, previous_move)
 
-            if elapsed_time >= 1000:
+            if elapsed_time >= 60000:
                 state = GameState.TIMEOUT
                 continue
 
             state = self.__judge.validate(move)
 
             if state == GameState.CONTINUE:
                 self.__judge.add_move(move)
```

### Comparing `duo_game_lib-0.1.1/src/duo_game_lib/judge.py` & `duo_game_lib-0.1.2/src/duo_game_lib/judge.py`

 * *Files identical despite different names*

### Comparing `duo_game_lib-0.1.1/src/duo_game_lib/move.py` & `duo_game_lib-0.1.2/src/duo_game_lib/move.py`

 * *Files identical despite different names*

### Comparing `duo_game_lib-0.1.1/src/duo_game_lib/player.py` & `duo_game_lib-0.1.2/src/duo_game_lib/player.py`

 * *Files identical despite different names*

### Comparing `duo_game_lib-0.1.1/PKG-INFO` & `duo_game_lib-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duo-game-lib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Logic for turn-based duo game
 Author: game-ai-platform-team
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

