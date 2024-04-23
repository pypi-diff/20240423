# Comparing `tmp/chemsource-1.0.0.tar.gz` & `tmp/chemsource-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemsource-1.0.0.tar", last modified: Tue Apr 23 20:30:16 2024, max compression
+gzip compressed data, was "chemsource-1.0.1.tar", last modified: Tue Apr 23 20:39:15 2024, max compression
```

## Comparing `chemsource-1.0.0.tar` & `chemsource-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:30:16.744066 chemsource-1.0.0/
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1072 2024-04-23 08:23:13.000000 chemsource-1.0.0/LICENSE
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      508 2024-04-23 20:30:16.743962 chemsource-1.0.0/PKG-INFO
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1474 2024-04-23 07:25:30.000000 chemsource-1.0.0/README.md
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      113 2024-04-23 20:30:16.744566 chemsource-1.0.0/setup.cfg
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      664 2024-04-23 20:22:21.000000 chemsource-1.0.0/setup.py
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:30:16.735887 chemsource-1.0.0/src/
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:30:16.740833 chemsource-1.0.0/src/chemsource/
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)       57 2024-04-23 20:27:26.000000 chemsource-1.0.0/src/chemsource/__init__.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1862 2024-04-23 20:07:41.000000 chemsource-1.0.0/src/chemsource/chemsource.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      602 2024-04-23 06:36:11.000000 chemsource-1.0.0/src/chemsource/classifier.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     2918 2024-04-23 20:03:10.000000 chemsource-1.0.0/src/chemsource/config.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      823 2024-04-10 21:23:32.000000 chemsource-1.0.0/src/chemsource/exceptions.py
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)     4019 2024-04-23 19:48:05.000000 chemsource-1.0.0/src/chemsource/retriever.py
-drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:30:16.743465 chemsource-1.0.0/src/chemsource.egg-info/
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      508 2024-04-23 20:30:16.000000 chemsource-1.0.0/src/chemsource.egg-info/PKG-INFO
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)      392 2024-04-23 20:30:16.000000 chemsource-1.0.0/src/chemsource.egg-info/SOURCES.txt
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)        1 2024-04-23 20:30:16.000000 chemsource-1.0.0/src/chemsource.egg-info/dependency_links.txt
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)       63 2024-04-23 20:30:16.000000 chemsource-1.0.0/src/chemsource.egg-info/requires.txt
--rw-r--r--   0 prajitrajkumar   (501) staff       (20)       11 2024-04-23 20:30:16.000000 chemsource-1.0.0/src/chemsource.egg-info/top_level.txt
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:39:15.707111 chemsource-1.0.1/
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1072 2024-04-23 08:23:13.000000 chemsource-1.0.1/LICENSE
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      508 2024-04-23 20:39:15.706986 chemsource-1.0.1/PKG-INFO
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1474 2024-04-23 07:25:30.000000 chemsource-1.0.1/README.md
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      113 2024-04-23 20:39:15.707485 chemsource-1.0.1/setup.cfg
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      664 2024-04-23 20:22:21.000000 chemsource-1.0.1/setup.py
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:39:15.702133 chemsource-1.0.1/src/
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:39:15.705031 chemsource-1.0.1/src/chemsource/
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)       57 2024-04-23 20:39:13.000000 chemsource-1.0.1/src/chemsource/__init__.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     1864 2024-04-23 20:37:25.000000 chemsource-1.0.1/src/chemsource/chemsource.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      602 2024-04-23 06:36:11.000000 chemsource-1.0.1/src/chemsource/classifier.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     2918 2024-04-23 20:35:54.000000 chemsource-1.0.1/src/chemsource/config.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      823 2024-04-10 21:23:32.000000 chemsource-1.0.1/src/chemsource/exceptions.py
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)     4019 2024-04-23 19:48:05.000000 chemsource-1.0.1/src/chemsource/retriever.py
+drwxr-xr-x   0 prajitrajkumar   (501) staff       (20)        0 2024-04-23 20:39:15.706544 chemsource-1.0.1/src/chemsource.egg-info/
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      508 2024-04-23 20:39:15.000000 chemsource-1.0.1/src/chemsource.egg-info/PKG-INFO
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)      392 2024-04-23 20:39:15.000000 chemsource-1.0.1/src/chemsource.egg-info/SOURCES.txt
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)        1 2024-04-23 20:39:15.000000 chemsource-1.0.1/src/chemsource.egg-info/dependency_links.txt
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)       63 2024-04-23 20:39:15.000000 chemsource-1.0.1/src/chemsource.egg-info/requires.txt
+-rw-r--r--   0 prajitrajkumar   (501) staff       (20)       11 2024-04-23 20:39:15.000000 chemsource-1.0.1/src/chemsource.egg-info/top_level.txt
```

### Comparing `chemsource-1.0.0/LICENSE` & `chemsource-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.0/README.md` & `chemsource-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.0/setup.py` & `chemsource-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.0/src/chemsource/chemsource.py` & `chemsource-1.0.1/src/chemsource/chemsource.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                          model=model, 
                          ncbi_key=ncbi_key,
                          prompt=prompt, 
                          max_tokens=max_tokens
                          )
     
     def chemsource(self, name, priority="WIKIPEDIA", single_source=False):
-        if self.openaikey is None:
+        if self.openai_key is None:
             raise ValueError("OpenAI API key must be provided")
 
         information = ret(name, 
                          priority,
                          single_source, 
                          ncbikey=self.ncbi_key
                          )
@@ -33,15 +33,15 @@
                                 information, 
                                 self.openai_key,
                                 self.prompt,
                                 self.model,
                                 self.max_tokens)
 
     def classify(self, name, information):
-        if self.openaikey is None:
+        if self.openai_key is None:
             raise ValueError("OpenAI API key must be provided")
         
         return cls(name, 
                    information,
                    self.openai_key,
                    self.prompt,
                    self.model,
```

### Comparing `chemsource-1.0.0/src/chemsource/classifier.py` & `chemsource-1.0.1/src/chemsource/classifier.py`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.0/src/chemsource/config.py` & `chemsource-1.0.1/src/chemsource/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,13 +58,13 @@
             openai_key_display = "*" * len(self.openai_key)
 
         if self.ncbi_key is None:
             ncbi_key_display = None
         else:
             ncbi_key_display =  "*" * len(self.ncbi_key)
         
-        return {"ncbi_key": openai_key_display,
-                "openai_key": ncbi_key_display, 
+        return {"openai_key": openai_key_display,
+                "ncbi_key": ncbi_key_display, 
                 "model": self.model,
                 "prompt": self.prompt,
                 "token_limit": self.max_tokens
                 }
```

### Comparing `chemsource-1.0.0/src/chemsource/exceptions.py` & `chemsource-1.0.1/src/chemsource/exceptions.py`

 * *Files identical despite different names*

### Comparing `chemsource-1.0.0/src/chemsource/retriever.py` & `chemsource-1.0.1/src/chemsource/retriever.py`

 * *Files identical despite different names*

