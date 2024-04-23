# Comparing `tmp/pellipop-0.8.1.tar.gz` & `tmp/pellipop-0.8.2.tar.gz`

## Comparing `pellipop-0.8.1.tar` & `pellipop-0.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/Video.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/__about__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/__init__.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/cli.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/file_finder.py
--rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/gui.py
--rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/main.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/path_fixer.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/whisper_from_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/speech_to_text/__init__.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pellipop-0.8.1/pellipop/speech_to_text/whisperMode.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pellipop-0.8.1/.gitignore
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pellipop-0.8.1/.hgignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pellipop-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pellipop-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pellipop-0.8.1/readme.md
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 pellipop-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/Video.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/__about__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/__init__.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/cli.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/file_finder.py
+-rw-r--r--   0        0        0    16483 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/gui.py
+-rw-r--r--   0        0        0    16528 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/main.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/path_fixer.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/whisper_from_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/speech_to_text/__init__.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pellipop-0.8.2/pellipop/speech_to_text/whisperMode.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pellipop-0.8.2/.gitignore
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pellipop-0.8.2/.hgignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pellipop-0.8.2/LICENSE.txt
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pellipop-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pellipop-0.8.2/readme.md
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 pellipop-0.8.2/PKG-INFO
```

### Comparing `pellipop-0.8.1/pellipop/Video.py` & `pellipop-0.8.2/pellipop/Video.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pellipop/cli.py` & `pellipop-0.8.2/pellipop/cli.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pellipop/file_finder.py` & `pellipop-0.8.2/pellipop/file_finder.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pellipop/gui.py` & `pellipop-0.8.2/pellipop/gui.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pellipop/main.py` & `pellipop-0.8.2/pellipop/main.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pellipop/path_fixer.py` & `pellipop-0.8.2/pellipop/path_fixer.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pellipop/whisper_from_url.py` & `pellipop-0.8.2/pellipop/whisper_from_url.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pellipop/speech_to_text/whisperMode.py` & `pellipop-0.8.2/pellipop/speech_to_text/whisperMode.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/.gitignore` & `pellipop-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/LICENSE.txt` & `pellipop-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/pyproject.toml` & `pellipop-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/readme.md` & `pellipop-0.8.2/readme.md`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.1/PKG-INFO` & `pellipop-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pellipop
-Version: 0.8.1
+Version: 0.8.2
 Summary: A graphical and command-line tool to extract key frames from videos along with their retranscription. It uses the Whisper API to transcribe the audio. It also generates a CSV file with the extracted key frames and their corresponding text.
 Project-URL: Homepage, https://github.com/CERES-Sorbonne/Pellipop
 Project-URL: Documentation, https://github.com/CERES-Sorbonne/Pellipop#readme
 Project-URL: Issues, https://github.com/CERES-Sorbonne/Pellipop/issues
 Project-URL: Source, https://github.com/CERES-Sorbonne/Pellipop
 Author: EdouardBoute
 Author-email: Marceau-h <pypi@marceau-h.fr>, Orion Alié <someonefefe@gmail.com>
```

