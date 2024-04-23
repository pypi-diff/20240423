# Comparing `tmp/IISRapi-1.0.1.tar.gz` & `tmp/IISRapi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IISRapi-1.0.1.tar", last modified: Mon Apr 22 09:08:24 2024, max compression
+gzip compressed data, was "IISRapi-1.1.tar", last modified: Tue Apr 23 07:12:48 2024, max compression
```

## Comparing `IISRapi-1.0.1.tar` & `IISRapi-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.522702 IISRapi-1.0.1/
-drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.482783 IISRapi-1.0.1/IISRapi/
--rw-rw-rw-   0        0        0        0 2024-04-22 07:53:31.000000 IISRapi-1.0.1/IISRapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.516897 IISRapi-1.0.1/IISRapi/model/
--rw-rw-rw-   0        0        0       26 2024-04-22 06:07:16.000000 IISRapi-1.0.1/IISRapi/model/__init__.py
--rw-rw-rw-   0        0        0      202 2024-04-22 08:37:02.000000 IISRapi-1.0.1/IISRapi/model/data.py
--rw-rw-rw-   0        0        0     6161 2024-04-22 09:07:33.000000 IISRapi-1.0.1/IISRapi/model/ner.py
--rw-rw-rw-   0        0        0     5374 2024-04-22 09:07:48.000000 IISRapi-1.0.1/IISRapi/model/pun.py
-drwxrwxrwx   0        0        0        0 2024-04-22 09:08:24.509168 IISRapi-1.0.1/IISRapi.egg-info/
--rw-rw-rw-   0        0        0      140 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-22 09:08:24.000000 IISRapi-1.0.1/IISRapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      140 2024-04-22 09:08:24.520708 IISRapi-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-22 09:08:24.522702 IISRapi-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      242 2024-04-22 09:08:07.000000 IISRapi-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:12:48.484487 IISRapi-1.1/
+drwxrwxrwx   0        0        0        0 2024-04-23 07:12:48.449903 IISRapi-1.1/IISRapi/
+-rw-rw-rw-   0        0        0        0 2024-04-22 07:53:31.000000 IISRapi-1.1/IISRapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:12:48.481504 IISRapi-1.1/IISRapi/model/
+-rw-rw-rw-   0        0        0       26 2024-04-22 06:07:16.000000 IISRapi-1.1/IISRapi/model/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-04-22 08:37:02.000000 IISRapi-1.1/IISRapi/model/data.py
+-rw-rw-rw-   0        0        0     5839 2024-04-23 05:54:06.000000 IISRapi-1.1/IISRapi/model/ner.py
+-rw-rw-rw-   0        0        0     3529 2024-04-23 05:53:57.000000 IISRapi-1.1/IISRapi/model/pun.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:12:48.473515 IISRapi-1.1/IISRapi.egg-info/
+-rw-rw-rw-   0        0        0      138 2024-04-23 07:12:48.000000 IISRapi-1.1/IISRapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-23 07:12:48.000000 IISRapi-1.1/IISRapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 07:12:48.000000 IISRapi-1.1/IISRapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 07:12:48.000000 IISRapi-1.1/IISRapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 07:12:48.000000 IISRapi-1.1/IISRapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      138 2024-04-23 07:12:48.483490 IISRapi-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-23 07:12:48.485484 IISRapi-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      240 2024-04-23 05:54:59.000000 IISRapi-1.1/setup.py
```

### Comparing `IISRapi-1.0.1/IISRapi/model/ner.py` & `IISRapi-1.1/IISRapi/model/ner.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,35 +11,29 @@
     def __init__(self,dev):
         self.pos=[]
         self.model_path=self.get_path()
         if(dev>=0 and torch.cuda.is_available()):
              flair.device = torch.device('cuda:' + str(dev))
         else:
             flair.device = torch.device('cpu')
-           
-        if not os.path.exists(self.model_path):
-            print(f"Model file not found. Downloading model...")
-            model_url="https://github.com/DH-code-space/punctuation-and-named-entity-recognition-for-Ming-Shilu/releases/download/IISRmodel/IISRner-1.0-py3-none-any.whl"
-            subprocess.call(["pip", "install", model_url])
-        elif self.model_path==self.wrong_path():
-            print("You loaded wrong model, changing to the ner model...")
-            self.model_path=self.get_path()
-        else:
-            print("Model found at "+self.model_path)
-            
+       
         self.model = self.load_model()
         
     def get_path(self):
-        path=os.path.abspath(os.path.join(os.path.dirname( __file__ ), '..','..', "IISRner\\best-model-ner.pt"))
-        return path
-    
-    def wrong_path(self):
-        path=os.path.abspath(os.path.join(os.path.dirname( __file__ ), '..','..', "IISRpunctuation\\best-model-pun.pt"))
+        try:
+            import IISRner
+            path=os.path.join(os.path.dirname(IISRner.__file__),"best-model-ner.pt")
+        except ModuleNotFoundError:
+            print("Model file not found. Downloading model...")
+            model_url="https://github.com/DH-code-space/punctuation-and-named-entity-recognition-for-Ming-Shilu/releases/download/IISRmodel/IISRner-1.0-py3-none-any.whl"
+            subprocess.call(["pip", "install", model_url])
+            import IISRner
+            path=os.path.join(os.path.dirname(IISRner.__file__),"best-model-ner.pt")
         return path
-    
+
     def load_model(self):
         return SequenceTagger.load(self.model_path)
         
     def __call__(self,texts):
         if isinstance(texts,str):
             result=Data(ori_txt=texts, ret_txt=self.ner(texts),ner_tags=self.pos)
             return result
```

