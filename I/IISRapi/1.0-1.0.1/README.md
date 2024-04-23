# Comparing `tmp/IISRapi-1.0.tar.gz` & `tmp/IISRapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IISRapi-1.0.tar", last modified: Mon Apr 22 08:57:56 2024, max compression
+gzip compressed data, was "IISRapi-1.0.1.tar", last modified: Mon Apr 22 09:08:24 2024, max compression
```

## Comparing `IISRapi-1.0.tar` & `IISRapi-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:56.363568 IISRapi-1.0/
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:56.329857 IISRapi-1.0/IISRapi/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:53:31.000000 IISRapi-1.0/IISRapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:56.361474 IISRapi-1.0/IISRapi/model/
--rw-rw-rw-   0        0        0       26 2024-04-22 06:07:16.000000 IISRapi-1.0/IISRapi/model/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-22 08:37:02.000000 IISRapi-1.0/IISRapi/model/data.py
--rw-rw-rw-   0        0        0     6182 2024-04-22 08:23:34.000000 IISRapi-1.0/IISRapi/model/ner.py
--rw-rw-rw-   0        0        0     5377 2024-04-22 08:23:26.000000 IISRapi-1.0/IISRapi/model/pun.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:57:56.351807 IISRapi-1.0/IISRapi.egg-info/
--rw-rw-rw-   0        0        0      138 2024-04-22 08:57:56.000000 IISRapi-1.0/IISRapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-22 08:57:56.000000 IISRapi-1.0/IISRapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 08:57:56.000000 IISRapi-1.0/IISRapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-22 08:57:56.000000 IISRapi-1.0/IISRapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 08:57:56.000000 IISRapi-1.0/IISRapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      138 2024-04-22 08:57:56.363568 IISRapi-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-22 08:57:56.363568 IISRapi-1.0/setup.cfg
--rw-rw-rw-   0        0        0      240 2024-04-22 08:42:50.000000 IISRapi-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.522702 IISRapi-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.482783 IISRapi-1.0.1/IISRapi/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:53:31.000000 IISRapi-1.0.1/IISRapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.516897 IISRapi-1.0.1/IISRapi/model/
+-rw-rw-rw-   0        0        0       26 2024-04-22 06:07:16.000000 IISRapi-1.0.1/IISRapi/model/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-22 08:37:02.000000 IISRapi-1.0.1/IISRapi/model/data.py
+-rw-rw-rw-   0        0        0     6161 2024-04-22 09:07:33.000000 IISRapi-1.0.1/IISRapi/model/ner.py
+-rw-rw-rw-   0        0        0     5374 2024-04-22 09:07:48.000000 IISRapi-1.0.1/IISRapi/model/pun.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.509168 IISRapi-1.0.1/IISRapi.egg-info/
+-rw-rw-rw-   0        0        0      140 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      140 2024-04-22 09:08:24.520708 IISRapi-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-22 09:08:24.522702 IISRapi-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      242 2024-04-22 09:08:07.000000 IISRapi-1.0.1/setup.py
```

### Comparing `IISRapi-1.0/IISRapi/model/ner.py` & `IISRapi-1.0.1/IISRapi/model/ner.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.model_path=self.get_path()
         if(dev>=0 and torch.cuda.is_available()):
              flair.device = torch.device('cuda:' + str(dev))
         else:
             flair.device = torch.device('cpu')
            
         if not os.path.exists(self.model_path):
-            print(f"Model file not found at {self.model_path}. Downloading model...")
+            print(f"Model file not found. Downloading model...")
             model_url="https://github.com/DH-code-space/punctuation-and-named-entity-recognition-for-Ming-Shilu/releases/download/IISRmodel/IISRner-1.0-py3-none-any.whl"
             subprocess.call(["pip", "install", model_url])
         elif self.model_path==self.wrong_path():
             print("You loaded wrong model, changing to the ner model...")
             self.model_path=self.get_path()
         else:
             print("Model found at "+self.model_path)
```

### Comparing `IISRapi-1.0/IISRapi/model/pun.py` & `IISRapi-1.0.1/IISRapi/model/pun.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self.result=Data(ori_txt="",ret_txt="")
         if(dev>=0 and torch.cuda.is_available()):
              flair.device = torch.device('cuda:' + str(dev))
         else:
             flair.device = torch.device('cpu')
             
         if not os.path.exists(self.model_path):
-            print("Model file not found at. Downloading model...")
+            print("Model file not found. Downloading model...")
             model_url="https://github.com/DH-code-space/punctuation-and-named-entity-recognition-for-Ming-Shilu/releases/download/IISRmodel/IISRpunctuation-1.0-py3-none-any.whl"
             subprocess.call(["pip", "install", model_url])
         elif self.model_path==self.wrong_path():
             print("You loaded wrong model, changing to the punctuation model...")
             self.model_path=self.get_path()
         else:
             print("Model found at "+self.model_path)
```

