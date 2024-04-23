# Comparing `tmp/chess-notation-0.1.7.tar.gz` & `tmp/chess_notation-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chess-notation-0.1.7.tar", last modified: Thu Apr  4 08:50:30 2024, max compression
+gzip compressed data, was "chess_notation-0.1.8.tar", last modified: Tue Apr 23 08:41:43 2024, max compression
```

## Comparing `chess-notation-0.1.7.tar` & `chess_notation-0.1.8.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-31 08:32:00.000000 chess-notation-0.1.7/MANIFEST.in
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      422 2024-04-04 08:50:30.919821 chess-notation-0.1.7/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-03-31 08:21:38.000000 chess-notation-0.1.7/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-04-04 08:50:07.000000 chess-notation-0.1.7/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-04 08:50:30.919821 chess-notation-0.1.7/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.909821 chess-notation-0.1.7/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       85 2024-03-31 08:24:21.000000 chess-notation-0.1.7/src/chess_notation/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/language/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-03-31 08:26:21.000000 chess-notation-0.1.7/src/chess_notation/language/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      629 2024-03-31 13:25:28.000000 chess-notation-0.1.7/src/chess_notation/language/language.py
--rwxrwxrwx   0 m4rs      (1000) m4rs      (1000)     1641 2024-03-31 08:31:52.000000 chess-notation-0.1.7/src/chess_notation/language/translations.json
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/represent/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-03-31 13:29:36.000000 chess-notation-0.1.7/src/chess_notation/represent/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2000 2024-03-31 13:29:43.000000 chess-notation-0.1.7/src/chess_notation/represent/represent.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation/styles/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      363 2024-03-31 16:21:10.000000 chess-notation-0.1.7/src/chess_notation/styles/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1329 2024-04-04 08:49:59.000000 chess-notation-0.1.7/src/chess_notation/styles/apply.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1057 2024-03-31 16:04:06.000000 chess-notation-0.1.7/src/chess_notation/styles/classify.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2364 2024-04-04 08:49:34.000000 chess-notation-0.1.7/src/chess_notation/styles/map.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-03-31 16:04:09.000000 chess-notation-0.1.7/src/chess_notation/styles/styles.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-04 08:50:30.919821 chess-notation-0.1.7/src/chess_notation.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      422 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       21 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-04 08:50:30.000000 chess-notation-0.1.7/src/chess_notation.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       53 2024-03-31 08:32:00.000000 chess_notation-0.1.8/MANIFEST.in
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-23 08:41:43.668373 chess_notation-0.1.8/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       65 2024-03-31 08:21:38.000000 chess_notation-0.1.8/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      495 2024-04-23 08:41:40.000000 chess_notation-0.1.8/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-23 08:41:43.668373 chess_notation-0.1.8/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.658373 chess_notation-0.1.8/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.658373 chess_notation-0.1.8/src/chess_notation/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      181 2024-04-23 08:41:04.000000 chess_notation-0.1.8/src/chess_notation/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-23 08:41:35.000000 chess_notation-0.1.8/src/chess_notation/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.658373 chess_notation-0.1.8/src/chess_notation/language/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       55 2024-03-31 08:26:21.000000 chess_notation-0.1.8/src/chess_notation/language/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      629 2024-03-31 13:25:28.000000 chess_notation-0.1.8/src/chess_notation/language/language.py
+-rwxrwxrwx   0 m4rs      (1000) m4rs      (1000)     1641 2024-03-31 08:31:52.000000 chess_notation-0.1.8/src/chess_notation/language/translations.json
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/src/chess_notation/represent/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-03-31 13:29:36.000000 chess_notation-0.1.8/src/chess_notation/represent/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1873 2024-04-16 06:53:54.000000 chess_notation-0.1.8/src/chess_notation/represent/represent.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/src/chess_notation/styles/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      363 2024-03-31 16:21:10.000000 chess_notation-0.1.8/src/chess_notation/styles/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1329 2024-04-04 08:49:59.000000 chess_notation-0.1.8/src/chess_notation/styles/apply.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1057 2024-03-31 16:04:06.000000 chess_notation-0.1.8/src/chess_notation/styles/classify.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2364 2024-04-04 08:49:34.000000 chess_notation-0.1.8/src/chess_notation/styles/map.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      248 2024-03-31 16:04:09.000000 chess_notation-0.1.8/src/chess_notation/styles/styles.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-23 08:41:43.668373 chess_notation-0.1.8/src/chess_notation.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      449 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      697 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       33 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-23 08:41:43.000000 chess_notation-0.1.8/src/chess_notation.egg-info/top_level.txt
```

### Comparing `chess-notation-0.1.7/src/chess_notation/language/language.py` & `chess_notation-0.1.8/src/chess_notation/language/language.py`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.7/src/chess_notation/language/translations.json` & `chess_notation-0.1.8/src/chess_notation/language/translations.json`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.7/src/chess_notation/represent/represent.py` & `chess_notation-0.1.8/src/chess_notation/represent/represent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 from pydantic import BaseModel
 from ..styles import Check, Mate, Castle, PawnCapture, PieceCapture, CapturedPiece, \
   is_castle, is_pawn_capture, is_piece_capture, is_check, is_mate, \
   castle, pawn_capture, piece_capture, check, mate
 from ..language import Language, translate
 
 class KingEffectStyles(BaseModel):
-  checks: list[Check] = []
-  mates: list[Mate] = []
+  checks: list[Check] = ['NONE']
+  mates: list[Mate] = ['NONE']
 
 class MotionStyles(BaseModel):
-  castles: list[Castle] = []
-  pawn_captures: list[PawnCapture] = []
-  piece_captures: list[PieceCapture] = []
+  castles: list[Castle] = ['O-O', 'OO']
+  pawn_captures: list[PawnCapture] = ['de', 'de4', 'dxe', 'dxe4', 'PxN', 'xe4']
+  piece_captures: list[PieceCapture] = ['Ne4', 'Nxe4', 'NxN']
 
-
-default_motions = MotionStyles(castles=['O-O', 'OO'], piece_captures=['Ne4', 'Nxe4', 'NxN'], pawn_captures=['de', 'de4', 'dxe', 'dxe4', 'PxN', 'xe4'])
-default_effects = KingEffectStyles(checks=['NONE'], mates=['NONE'])
-
-def motion_representations(san: str, motions: MotionStyles = default_motions, captured_piece: CapturedPiece = None) -> set[str]:
+def motion_representations(san: str, motions: MotionStyles = MotionStyles(), captured_piece: CapturedPiece = None) -> set[str]:
   outputs = set([san])
 
   if is_castle(san):
     for style in motions.castles:
       outputs.add(castle(san, style))
   elif is_pawn_capture(san):
     for style in motions.pawn_captures:
       outputs.add(pawn_capture(san, style, captured_piece))
   elif is_piece_capture(san):
     for style in motions.piece_captures:
       outputs.add(piece_capture(san, style, captured_piece))
 
   return outputs
 
-def effect_representations(san: str, effects: KingEffectStyles = default_effects) -> set[str]:
+def effect_representations(san: str, effects: KingEffectStyles = KingEffectStyles()) -> set[str]:
   outputs = set([san])
 
   if is_check(san):
     for style in effects.checks:
       outputs.add(check(san, style))
   elif is_mate(san):
     for style in effects.mates:
       outputs.add(mate(san, style))
   
   return outputs
 
 def representations(
   san: str,
-  motions: MotionStyles = default_motions,
-  effects: KingEffectStyles = default_effects,
+  motions: MotionStyles = MotionStyles(),
+  effects: KingEffectStyles = KingEffectStyles(),
   languages: list[Language] = ['CA', 'EN'],
-  captured_piece: CapturedPiece = None
+  captured_piece: CapturedPiece | None = None
 ) -> set[str]:
   return {
     translate(styled, lang)
     for motioned in motion_representations(san, motions, captured_piece)
     for styled in effect_representations(motioned, effects)
     for lang in languages
   }
```

### Comparing `chess-notation-0.1.7/src/chess_notation/styles/apply.py` & `chess_notation-0.1.8/src/chess_notation/styles/apply.py`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.7/src/chess_notation/styles/classify.py` & `chess_notation-0.1.8/src/chess_notation/styles/classify.py`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.7/src/chess_notation/styles/map.py` & `chess_notation-0.1.8/src/chess_notation/styles/map.py`

 * *Files identical despite different names*

### Comparing `chess-notation-0.1.7/src/chess_notation.egg-info/SOURCES.txt` & `chess_notation-0.1.8/src/chess_notation.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/chess_notation/__init__.py
+src/chess_notation/__init__.pyi
 src/chess_notation.egg-info/PKG-INFO
 src/chess_notation.egg-info/SOURCES.txt
 src/chess_notation.egg-info/dependency_links.txt
 src/chess_notation.egg-info/requires.txt
 src/chess_notation.egg-info/top_level.txt
 src/chess_notation/language/__init__.py
 src/chess_notation/language/language.py
```

