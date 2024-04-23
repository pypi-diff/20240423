# Comparing `tmp/jsonffi-1.0.3-py3-none-any.whl.zip` & `tmp/jsonffi-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1755 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat      865 b- defN 24-Apr-19 04:12 jsonffi/__init__.py
--rw-rw-rw-  2.0 fat      565 b- defN 24-Apr-19 04:13 jsonffi-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 04:13 jsonffi-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-19 04:13 jsonffi-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      371 b- defN 24-Apr-19 04:13 jsonffi-1.0.3.dist-info/RECORD
-5 files, 1901 bytes uncompressed, 1059 bytes compressed:  44.3%
+Zip file size: 1897 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     1468 b- defN 24-Apr-22 05:05 jsonffi/__init__.py
+-rw-rw-rw-  2.0 fat      565 b- defN 24-Apr-22 05:10 jsonffi-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 05:10 jsonffi-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 24-Apr-22 05:10 jsonffi-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      372 b- defN 24-Apr-22 05:10 jsonffi-1.0.4.dist-info/RECORD
+5 files, 2505 bytes uncompressed, 1201 bytes compressed:  52.1%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: jsonffi/__init__.py
 Comment: 
 
-Filename: jsonffi-1.0.3.dist-info/METADATA
+Filename: jsonffi-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: jsonffi-1.0.3.dist-info/WHEEL
+Filename: jsonffi-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: jsonffi-1.0.3.dist-info/top_level.txt
+Filename: jsonffi-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: jsonffi-1.0.3.dist-info/RECORD
+Filename: jsonffi-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonffi/__init__.py

```diff
@@ -1,22 +1,37 @@
 import json
 from cffi import FFI
 
 __copyright__    = 'Copyright (C) 2024 JavaCommons Technologies'
-__version__      = '1.0.3'
+__version__      = '1.0.4'
 __license__      = 'MIT'
 __author__       = 'JavaCommons Technologies'
 __author_email__ = 'javacommmons@gmail.com'
 __url__          = 'https://github.com/javacommons/py-jsonffi'
 __all__ = ['JsonFFI']
 
 class JsonFFI:
-    def __init__(self, dllSpec):
+    def __init__(self, dll):
         self.ffi = FFI()
         self.ffi.cdef("const char *Call(const char *, const char *);")
         self.ffi.cdef("const char *LastError();")
-        self.clib = self.ffi.dlopen(dllSpec)
+        self.clib = self.ffi.dlopen(dll)
     def call(self, name, args):
         answer = self.ffi.string(self.clib.Call(name.encode(), json.dumps(args).encode())).decode()
         error = self.ffi.string(self.clib.LastError()).decode()
         if error == "": return json.loads(answer)
         raise Exception(error)
+
+class MyJS:
+    def __init__(self, myjsDll, asmSpecList = []):
+        self.api = JsonFFI(myjsDll)
+        return self.api.call("Init", asmSpecList)
+    def SetValue(self, name, value):
+        return self.api.call("SetValue", [name, value])
+    def GetValue(self, name):
+        return self.api.call("GetValue", [name])
+    def Execute(self, script, *vars):
+        return self.api.call("Execute", [script, vars])
+    def Evaluate(self, script, *vars):
+        return self.api.call("Evaluate", [script, vars])
+    def Call(self, name, *vars):
+        return self.api.call("Call", [name, vars])
```

## Comparing `jsonffi-1.0.3.dist-info/METADATA` & `jsonffi-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonffi
-Version: 1.0.3
+Version: 1.0.4
 Summary: 一言で書けるパッケージ概要
 Home-page: https://github.com/javacommons/py-jsonffi
 Author: JavaCommons Technologies
 Author-email: javacommmons@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

