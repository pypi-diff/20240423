# Comparing `tmp/sts_lib-0.27.1.tar.gz` & `tmp/sts_lib-0.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sts_lib-0.27.1.tar", last modified: Tue Apr 23 08:28:03 2024, max compression
+gzip compressed data, was "sts_lib-0.27.2.tar", last modified: Tue Apr 23 09:35:01 2024, max compression
```

## Comparing `sts_lib-0.27.1.tar` & `sts_lib-0.27.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.696675 sts_lib-0.27.1/
--rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.27.1/LICENSE
--rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.27.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11018 2024-04-23 08:28:03.696675 sts_lib-0.27.1/PKG-INFO
--rw-rw-rw-   0        0        0     9565 2024-04-23 08:25:00.000000 sts_lib-0.27.1/README.md
--rw-rw-rw-   0        0        0     1728 2024-04-23 08:28:03.697674 sts_lib-0.27.1/setup.cfg
--rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.27.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.652673 sts_lib-0.27.1/sts/
--rw-rw-rw-   0        0        0    52645 2024-04-23 08:25:00.000000 sts_lib-0.27.1/sts/__init__.py
--rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.27.1/sts/__main__.py
--rw-rw-rw-   0        0        0     7551 2024-04-23 08:11:31.000000 sts_lib-0.27.1/sts/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.653672 sts_lib-0.27.1/sts/data/
-drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.670701 sts_lib-0.27.1/sts/data/config/
--rw-rw-rw-   0        0        0      915 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/_default.json
--rw-rw-rw-   0        0        0      608 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/hk2s.json
--rw-rw-rw-   0        0        0      346 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/hk2t.json
--rw-rw-rw-   0        0        0      410 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/jp2t.json
--rw-rw-rw-   0        0        0      419 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2hk.json
--rw-rw-rw-   0        0        0      267 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2t.json
--rw-rw-rw-   0        0        0      417 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2tw.json
--rw-rw-rw-   0        0        0      608 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/s2twp.json
--rw-rw-rw-   0        0        0      247 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2hk.json
--rw-rw-rw-   0        0        0      261 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2jp.json
--rw-rw-rw-   0        0        0      267 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2s.json
--rw-rw-rw-   0        0        0      245 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/t2tw.json
--rw-rw-rw-   0        0        0      606 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/tw2s.json
--rw-rw-rw-   0        0        0      670 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/tw2sp.json
--rw-rw-rw-   0        0        0      344 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/config/tw2t.json
-drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.684514 sts_lib-0.27.1/sts/data/dictionary/
--rw-rw-rw-   0        0        0      595 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/HKVariants.txt
--rw-rw-rw-   0        0        0     2865 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/HKVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0      103 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/JPShinjitaiCharacters.txt
--rw-rw-rw-   0        0        0     2720 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/JPShinjitaiPhrases.txt
--rw-rw-rw-   0        0        0     3307 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/JPVariants.txt
--rw-rw-rw-   0        0        0    38333 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/STCharacters.txt
--rw-rw-rw-   0        0        0  1053351 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/STPhrases.txt
--rw-rw-rw-   0        0        0    38740 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TSCharacters.txt
--rw-rw-rw-   0        0        0     5438 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TSPhrases.txt
--rw-rw-rw-   0        0        0     8014 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWPhrasesIT.txt
--rw-rw-rw-   0        0        0     2205 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWPhrasesName.txt
--rw-rw-rw-   0        0        0      608 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWPhrasesOther.txt
--rw-rw-rw-   0        0        0      351 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWVariants.txt
--rw-rw-rw-   0        0        0     1143 2024-04-23 08:17:38.000000 sts_lib-0.27.1/sts/data/dictionary/TWVariantsRevPhrases.txt
--rw-rw-rw-   0        0        0    22760 2024-04-23 08:00:20.000000 sts_lib-0.27.1/sts/data/htmlpage.tpl.html
-drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.687516 sts_lib-0.27.1/sts/data/scheme/
--rw-rw-rw-   0        0        0    21633 2024-04-23 08:11:43.000000 sts_lib-0.27.1/sts/data/scheme/st_multi.txt
--rw-rw-rw-   0        0        0      436 2024-04-23 08:11:43.000000 sts_lib-0.27.1/sts/data/scheme/ts_multi.txt
--rw-rw-rw-   0        0        0     2108 2024-04-23 08:11:43.000000 sts_lib-0.27.1/sts/data/scheme/variant.txt
-drwxrwxrwx   0        0        0        0 2024-04-23 08:28:03.693678 sts_lib-0.27.1/sts_lib.egg-info/
--rw-rw-rw-   0        0        0    11018 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1325 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      202 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-23 08:28:03.000000 sts_lib-0.27.1/sts_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:01.472256 sts_lib-0.27.2/
+-rw-rw-rw-   0        0        0    11358 2024-04-19 09:05:26.000000 sts_lib-0.27.2/LICENSE
+-rw-rw-rw-   0        0        0       13 2024-04-19 09:05:26.000000 sts_lib-0.27.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11018 2024-04-23 09:35:01.472256 sts_lib-0.27.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9565 2024-04-23 08:25:00.000000 sts_lib-0.27.2/README.md
+-rw-rw-rw-   0        0        0     1728 2024-04-23 09:35:01.473255 sts_lib-0.27.2/setup.cfg
+-rw-rw-rw-   0        0        0       65 2024-04-19 09:05:26.000000 sts_lib-0.27.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:01.430309 sts_lib-0.27.2/sts/
+-rw-rw-rw-   0        0        0    52664 2024-04-23 09:18:41.000000 sts_lib-0.27.2/sts/__init__.py
+-rw-rw-rw-   0        0        0       89 2024-04-19 09:05:26.000000 sts_lib-0.27.2/sts/__main__.py
+-rw-rw-rw-   0        0        0     7551 2024-04-23 08:11:31.000000 sts_lib-0.27.2/sts/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:01.431313 sts_lib-0.27.2/sts/data/
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:01.444303 sts_lib-0.27.2/sts/data/config/
+-rw-rw-rw-   0        0        0      915 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/_default.json
+-rw-rw-rw-   0        0        0      608 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/hk2s.json
+-rw-rw-rw-   0        0        0      346 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/hk2t.json
+-rw-rw-rw-   0        0        0      410 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/jp2t.json
+-rw-rw-rw-   0        0        0      419 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/s2hk.json
+-rw-rw-rw-   0        0        0      267 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/s2t.json
+-rw-rw-rw-   0        0        0      417 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/s2tw.json
+-rw-rw-rw-   0        0        0      608 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/s2twp.json
+-rw-rw-rw-   0        0        0      247 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/t2hk.json
+-rw-rw-rw-   0        0        0      261 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/t2jp.json
+-rw-rw-rw-   0        0        0      267 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/t2s.json
+-rw-rw-rw-   0        0        0      245 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/t2tw.json
+-rw-rw-rw-   0        0        0      606 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/tw2s.json
+-rw-rw-rw-   0        0        0      670 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/tw2sp.json
+-rw-rw-rw-   0        0        0      344 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/config/tw2t.json
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:01.460269 sts_lib-0.27.2/sts/data/dictionary/
+-rw-rw-rw-   0        0        0      595 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/HKVariants.txt
+-rw-rw-rw-   0        0        0     2865 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/HKVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0      103 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/JPShinjitaiCharacters.txt
+-rw-rw-rw-   0        0        0     2720 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/JPShinjitaiPhrases.txt
+-rw-rw-rw-   0        0        0     3307 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/JPVariants.txt
+-rw-rw-rw-   0        0        0    38333 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/STCharacters.txt
+-rw-rw-rw-   0        0        0  1053351 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/STPhrases.txt
+-rw-rw-rw-   0        0        0    38740 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/TSCharacters.txt
+-rw-rw-rw-   0        0        0     5438 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/TSPhrases.txt
+-rw-rw-rw-   0        0        0     8014 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/TWPhrasesIT.txt
+-rw-rw-rw-   0        0        0     2205 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/TWPhrasesName.txt
+-rw-rw-rw-   0        0        0      608 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/TWPhrasesOther.txt
+-rw-rw-rw-   0        0        0      351 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/TWVariants.txt
+-rw-rw-rw-   0        0        0     1143 2024-04-23 09:34:01.000000 sts_lib-0.27.2/sts/data/dictionary/TWVariantsRevPhrases.txt
+-rw-rw-rw-   0        0        0    22760 2024-04-23 08:00:20.000000 sts_lib-0.27.2/sts/data/htmlpage.tpl.html
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:01.462267 sts_lib-0.27.2/sts/data/scheme/
+-rw-rw-rw-   0        0        0    21633 2024-04-23 09:18:42.000000 sts_lib-0.27.2/sts/data/scheme/st_multi.txt
+-rw-rw-rw-   0        0        0      436 2024-04-23 09:18:42.000000 sts_lib-0.27.2/sts/data/scheme/ts_multi.txt
+-rw-rw-rw-   0        0        0     2108 2024-04-23 09:18:42.000000 sts_lib-0.27.2/sts/data/scheme/variant.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 09:35:01.470258 sts_lib-0.27.2/sts_lib.egg-info/
+-rw-rw-rw-   0        0        0    11018 2024-04-23 09:35:01.000000 sts_lib-0.27.2/sts_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1325 2024-04-23 09:35:01.000000 sts_lib-0.27.2/sts_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 09:35:01.000000 sts_lib-0.27.2/sts_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-04-23 09:35:01.000000 sts_lib-0.27.2/sts_lib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      202 2024-04-23 09:35:01.000000 sts_lib-0.27.2/sts_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-23 09:35:01.000000 sts_lib-0.27.2/sts_lib.egg-info/top_level.txt
```

### Comparing `sts_lib-0.27.1/LICENSE` & `sts_lib-0.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/PKG-INFO` & `sts_lib-0.27.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.27.1
+Version: 0.27.2
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.27.1/README.md` & `sts_lib-0.27.2/README.md`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/setup.cfg` & `sts_lib-0.27.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/__init__.py` & `sts_lib-0.27.2/sts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @_lazyprop.setter
         def _lazyprop(self, value):
             setattr(self, attr_name, value)
 
         return _lazyprop
 
 
-__version__ = '0.27.1'
+__version__ = '0.27.2'
 
 StsDictMatch = namedtuple('StsDictMatch', ['conv', 'start', 'end'])
 StsDictConv = namedtuple('StsDictConv', ['key', 'values'])
 
 
 class StreamList(list):
     """Convert an iterable into a serializable "list".
@@ -1086,15 +1086,15 @@
             A StsDict or str (for str scheme or when up-to-date).
         """
         if isinstance(dict_scheme, str):
             return dict_scheme
 
         dest = dict_scheme.get('file')
         if dest:
-            if not dict_scheme.get('_updated'):
+            if not skip_check and not dict_scheme.get('_updated'):
                 return dest
 
             format = os.path.splitext(dest)[1][1:].lower()
         else:
             format = '.list'
 
         mode = dict_scheme['mode']
```

### Comparing `sts_lib-0.27.1/sts/cli.py` & `sts_lib-0.27.2/sts/cli.py`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/config/_default.json` & `sts_lib-0.27.2/sts/data/config/_default.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/config/hk2s.json` & `sts_lib-0.27.2/sts/data/config/hk2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/config/s2twp.json` & `sts_lib-0.27.2/sts/data/config/s2twp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/config/tw2s.json` & `sts_lib-0.27.2/sts/data/config/tw2s.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/config/tw2sp.json` & `sts_lib-0.27.2/sts/data/config/tw2sp.json`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/HKVariants.txt` & `sts_lib-0.27.2/sts/data/dictionary/HKVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/HKVariantsRevPhrases.txt` & `sts_lib-0.27.2/sts/data/dictionary/HKVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/JPShinjitaiPhrases.txt` & `sts_lib-0.27.2/sts/data/dictionary/JPShinjitaiPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/JPVariants.txt` & `sts_lib-0.27.2/sts/data/dictionary/JPVariants.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/STCharacters.txt` & `sts_lib-0.27.2/sts/data/dictionary/STCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/STPhrases.txt` & `sts_lib-0.27.2/sts/data/dictionary/STPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/TSCharacters.txt` & `sts_lib-0.27.2/sts/data/dictionary/TSCharacters.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/TSPhrases.txt` & `sts_lib-0.27.2/sts/data/dictionary/TSPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/TWPhrasesIT.txt` & `sts_lib-0.27.2/sts/data/dictionary/TWPhrasesIT.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/TWPhrasesName.txt` & `sts_lib-0.27.2/sts/data/dictionary/TWPhrasesName.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/TWPhrasesOther.txt` & `sts_lib-0.27.2/sts/data/dictionary/TWPhrasesOther.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/dictionary/TWVariantsRevPhrases.txt` & `sts_lib-0.27.2/sts/data/dictionary/TWVariantsRevPhrases.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/htmlpage.tpl.html` & `sts_lib-0.27.2/sts/data/htmlpage.tpl.html`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/scheme/st_multi.txt` & `sts_lib-0.27.2/sts/data/scheme/st_multi.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts/data/scheme/variant.txt` & `sts_lib-0.27.2/sts/data/scheme/variant.txt`

 * *Files identical despite different names*

### Comparing `sts_lib-0.27.1/sts_lib.egg-info/PKG-INFO` & `sts_lib-0.27.2/sts_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-lib
-Version: 0.27.1
+Version: 0.27.2
 Summary: An open library for flexible simplified-traditional Chinese text conversion.
 Home-page: https://github.com/danny0838/sts-lib
 Author: Danny Lin
 Author-email: danny0838@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
```

### Comparing `sts_lib-0.27.1/sts_lib.egg-info/SOURCES.txt` & `sts_lib-0.27.2/sts_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

