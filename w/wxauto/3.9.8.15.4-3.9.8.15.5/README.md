# Comparing `tmp/wxauto-3.9.8.15.4.tar.gz` & `tmp/wxauto-3.9.8.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wxauto-3.9.8.15.4.tar", last modified: Mon Apr 22 02:32:57 2024, max compression
+gzip compressed data, was "dist\wxauto-3.9.8.15.5.tar", last modified: Tue Apr 23 06:26:23 2024, max compression
```

## Comparing `wxauto-3.9.8.15.4.tar` & `wxauto-3.9.8.15.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/
--rw-rw-rw-   0        0        0     3648 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/PKG-INFO
--rw-rw-rw-   0        0        0     3283 2024-04-16 07:34:36.000000 wxauto-3.9.8.15.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/setup.cfg
--rw-rw-rw-   0        0        0      736 2024-04-22 02:28:10.000000 wxauto-3.9.8.15.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/wxauto/
--rw-rw-rw-   0        0        0       52 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.4/wxauto/__init__.py
--rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.4/wxauto/color.py
--rw-rw-rw-   0        0        0    24356 2024-04-22 02:27:57.000000 wxauto-3.9.8.15.4/wxauto/elements.py
--rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.4/wxauto/errors.py
--rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.4/wxauto/languages.py
--rw-rw-rw-   0        0        0     8735 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.4/wxauto/utils.py
--rw-rw-rw-   0        0        0    26412 2024-04-22 02:27:46.000000 wxauto-3.9.8.15.4/wxauto/wxauto.py
-drwxrwxrwx   0        0        0        0 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/wxauto.egg-info/
--rw-rw-rw-   0        0        0     3648 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/wxauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/wxauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/wxauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/wxauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 02:32:57.000000 wxauto-3.9.8.15.4/wxauto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/
+-rw-rw-rw-   0        0        0     3648 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3283 2024-04-16 07:34:36.000000 wxauto-3.9.8.15.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/setup.cfg
+-rw-rw-rw-   0        0        0      736 2024-04-23 06:26:16.000000 wxauto-3.9.8.15.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/wxauto/
+-rw-rw-rw-   0        0        0       52 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/__init__.py
+-rw-rw-rw-   0        0        0     8728 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/color.py
+-rw-rw-rw-   0        0        0    24361 2024-04-23 06:25:46.000000 wxauto-3.9.8.15.5/wxauto/elements.py
+-rw-rw-rw-   0        0        0       49 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/errors.py
+-rw-rw-rw-   0        0        0     5449 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/languages.py
+-rw-rw-rw-   0        0        0     8735 2024-03-29 08:40:11.000000 wxauto-3.9.8.15.5/wxauto/utils.py
+-rw-rw-rw-   0        0        0    26412 2024-04-22 02:27:46.000000 wxauto-3.9.8.15.5/wxauto/wxauto.py
+drwxrwxrwx   0        0        0        0 2024-04-23 06:26:23.000000 wxauto-3.9.8.15.5/wxauto.egg-info/
+-rw-rw-rw-   0        0        0     3648 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 06:26:22.000000 wxauto-3.9.8.15.5/wxauto.egg-info/top_level.txt
```

### Comparing `wxauto-3.9.8.15.4/PKG-INFO` & `wxauto-3.9.8.15.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.4
+Version: 3.9.8.15.5
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

### Comparing `wxauto-3.9.8.15.4/README.md` & `wxauto-3.9.8.15.5/README.md`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.4/setup.py` & `wxauto-3.9.8.15.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wxauto',
-    version='3.9.8.15.4',
+    version='3.9.8.15.5',
     author='Cluic',
     author_email='tikic@qq.com',
     description='A simple wechat automation tool',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

### Comparing `wxauto-3.9.8.15.4/wxauto/color.py` & `wxauto-3.9.8.15.5/wxauto/color.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.4/wxauto/elements.py` & `wxauto-3.9.8.15.5/wxauto/elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
                 if atwnd.Exists(maxSearchSeconds=0.1):
                     atwnd.SendKeys('{ENTER}')
 
         t0 = time.time()
         while True:
             if time.time() - t0 > 10:
                 raise TimeoutError(f'发送消息超时 --> {self.who} - {msg}')
-            editbox.SetFocus()
+            self.editbox.SetFocus()
             time.sleep(0.1)
             SetClipboardText(msg)
             self.editbox.SendKeys('{Ctrl}v')
             if self.editbox.GetValuePattern().Value.strip('￼'):
                 break
         self.editbox.SendKeys('{Enter}')
```

### Comparing `wxauto-3.9.8.15.4/wxauto/languages.py` & `wxauto-3.9.8.15.5/wxauto/languages.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.4/wxauto/utils.py` & `wxauto-3.9.8.15.5/wxauto/utils.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.4/wxauto/wxauto.py` & `wxauto-3.9.8.15.5/wxauto/wxauto.py`

 * *Files identical despite different names*

### Comparing `wxauto-3.9.8.15.4/wxauto.egg-info/PKG-INFO` & `wxauto-3.9.8.15.5/wxauto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxauto
-Version: 3.9.8.15.4
+Version: 3.9.8.15.5
 Summary: A simple wechat automation tool
 Author: Cluic
 Author-email: tikic@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.6
```

