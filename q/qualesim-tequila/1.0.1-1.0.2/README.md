# Comparing `tmp/qualesim-tequila-1.0.1.tar.gz` & `tmp/qualesim-tequila-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-tequila-1.0.1.tar", last modified: Mon Apr 22 07:43:35 2024, max compression
+gzip compressed data, was "qualesim-tequila-1.0.2.tar", last modified: Tue Apr 23 03:15:09 2024, max compression
```

## Comparing `qualesim-tequila-1.0.1.tar` & `qualesim-tequila-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      660 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      143 2024-04-22 07:43:07.000000 qualesim-tequila-1.0.1/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      104 2024-03-15 09:02:38.000000 qualesim-tequila-1.0.1/data/bin/dqcsbetequila
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/qualesim_tequila/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-07-06 01:42:02.000000 qualesim-tequila-1.0.1/qualesim_tequila/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      102 2023-07-06 02:29:24.000000 qualesim-tequila-1.0.1/qualesim_tequila/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    16487 2024-04-22 07:41:26.000000 qualesim-tequila-1.0.1/qualesim_tequila/backend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2875 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.1/qualesim_tequila/test.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      660 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      352 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       17 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/setup.cfg
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1108 2024-04-22 07:42:08.000000 qualesim-tequila-1.0.1/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    25164 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.1/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2526 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.1/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:15:09.862422 qualesim-tequila-1.0.2/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      660 2024-04-23 03:15:09.862422 qualesim-tequila-1.0.2/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      143 2024-04-22 07:43:07.000000 qualesim-tequila-1.0.2/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:15:09.858422 qualesim-tequila-1.0.2/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:15:09.858422 qualesim-tequila-1.0.2/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      104 2024-03-15 09:02:38.000000 qualesim-tequila-1.0.2/data/bin/dqcsbetequila
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:15:09.858422 qualesim-tequila-1.0.2/qualesim_tequila/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-07-06 01:42:02.000000 qualesim-tequila-1.0.2/qualesim_tequila/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      102 2023-07-06 02:29:24.000000 qualesim-tequila-1.0.2/qualesim_tequila/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    16600 2024-04-23 02:36:32.000000 qualesim-tequila-1.0.2/qualesim_tequila/backend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2875 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.2/qualesim_tequila/test.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:15:09.862422 qualesim-tequila-1.0.2/qualesim_tequila.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      660 2024-04-23 03:15:09.000000 qualesim-tequila-1.0.2/qualesim_tequila.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      352 2024-04-23 03:15:09.000000 qualesim-tequila-1.0.2/qualesim_tequila.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-23 03:15:09.000000 qualesim-tequila-1.0.2/qualesim_tequila.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       17 2024-04-23 03:15:09.000000 qualesim-tequila-1.0.2/qualesim_tequila.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-23 03:15:09.862422 qualesim-tequila-1.0.2/setup.cfg
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1108 2024-04-23 02:46:43.000000 qualesim-tequila-1.0.2/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 03:15:09.862422 qualesim-tequila-1.0.2/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    25164 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.2/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2526 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.2/tests/test_qifile.py
```

### Comparing `qualesim-tequila-1.0.1/PKG-INFO` & `qualesim-tequila-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-tequila
-Version: 1.0.1
+Version: 1.0.2
 Summary: DQCsim backend for tequila.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-tequila.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim tequila
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-tequila-1.0.1/qualesim_tequila/backend.py` & `qualesim-tequila-1.0.2/qualesim_tequila/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,15 @@
             measurements.append(
                 Measurement(
                     qubit_refs[it],
                     cls_list[it],
                     struct.pack("<d", 1),
                     probability=1,
                     state_vector=state_res,
-                    state_vector_be=str([self.cls_dict, []]),
+                    state_vector_be=str([self.cls_dict, state_res_before]),
                     one_shot=msmts,
                 )
             )
         return measurements
 
     def handle_measurement_gate_quiets(self, qubit_refs, basis, arb):
         """handle_measurement_gate is to handle the measure gate and free opration.
@@ -354,26 +354,29 @@
                         list(i) for i in self.circuit.data[measure_targets[i]][0]
                     ]
                 else:
                     self.state_res[measure_targets[i]] = get_qubit_prob(
                         self.circuit.vec().tolist(), measure_targets[i], self.circuit.n
                     )
                 self.circuit.proj_site(measure_targets[i], cls_list[i])
-
         # form the Measurement and send it to upsteam plugins.
         for it in range(len(qubit_refs)):
-            state_res = str([self.cls_dict, self.state_res[qubit_refs[it]]])
+
+            if measure_mod == "free":
+                state_res = ""
+                p = 1
+            else:
+                state_res = str([self.cls_dict, self.state_res[measure_targets[it]]])
+                p = abs(self.state_res[measure_targets[it]][cls_list[it]][0] ** 2)
             measurements.append(
                 Measurement(
                     qubit_refs[it],
                     cls_list[it],
                     struct.pack("<d", 1),
-                    probability=abs(
-                        self.state_res[qubit_refs[it]][cls_list[it]][0] ** 2
-                    ),
+                    probability=p,
                     state_vector=state_res,
                     state_for_res=state_res_before,
                 )
             )
         return measurements
 
     def handle_prepare_gate(self, qubit_refs, basis, _arb):
```

### Comparing `qualesim-tequila-1.0.1/qualesim_tequila/test.py` & `qualesim-tequila-1.0.2/qualesim_tequila/test.py`

 * *Files identical despite different names*

### Comparing `qualesim-tequila-1.0.1/qualesim_tequila.egg-info/PKG-INFO` & `qualesim-tequila-1.0.2/qualesim_tequila.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-tequila
-Version: 1.0.1
+Version: 1.0.2
 Summary: DQCsim backend for tequila.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-tequila.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim tequila
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-tequila-1.0.1/setup.py` & `qualesim-tequila-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-tequila",
-    version="1.0.1",
+    version="1.0.2",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="DQCsim backend for tequila.",
     license="GPLv3",
     keywords="qualesim tequila",
     url="https://gitee.com/hpcl_quanta/dqcsim-tequila.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-tequila-1.0.1/tests/test_gate.py` & `qualesim-tequila-1.0.2/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-tequila-1.0.1/tests/test_qifile.py` & `qualesim-tequila-1.0.2/tests/test_qifile.py`

 * *Files identical despite different names*

