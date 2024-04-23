# Comparing `tmp/qualesim-quiets-1.0.8.tar.gz` & `tmp/qualesim-quiets-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quiets-1.0.8.tar", last modified: Mon Apr 22 11:28:41 2024, max compression
+gzip compressed data, was "qualesim-quiets-1.1.0.tar", last modified: Tue Apr 23 12:42:25 2024, max compression
```

## Comparing `qualesim-quiets-1.0.8.tar` & `qualesim-quiets-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 11:28:41.076100 qualesim-quiets-1.0.8/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.8/LICENSE
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-22 11:28:41.072100 qualesim-quiets-1.0.8/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      289 2024-04-19 07:49:03.000000 qualesim-quiets-1.0.8/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 11:28:41.064100 qualesim-quiets-1.0.8/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 11:28:41.064100 qualesim-quiets-1.0.8/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.8/data/bin/dqcsfeqi
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 11:28:41.068100 qualesim-quiets-1.0.8/qualesim_quiets/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.8/qualesim_quiets/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.8/qualesim_quiets/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    45676 2024-04-22 11:26:54.000000 qualesim-quiets-1.0.8/qualesim_quiets/frontend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-22 11:18:42.000000 qualesim-quiets-1.0.8/qualesim_quiets/utils.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 11:28:41.072100 qualesim-quiets-1.0.8/qualesim_quiets.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-22 11:28:41.000000 qualesim-quiets-1.0.8/qualesim_quiets.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      445 2024-04-22 11:28:41.000000 qualesim-quiets-1.0.8/qualesim_quiets.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-22 11:28:41.000000 qualesim-quiets-1.0.8/qualesim_quiets.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-22 11:28:41.000000 qualesim-quiets-1.0.8/qualesim_quiets.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-22 11:28:41.000000 qualesim-quiets-1.0.8/qualesim_quiets.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-22 11:28:41.076100 qualesim-quiets-1.0.8/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-22 11:27:15.000000 qualesim-quiets-1.0.8/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 11:28:41.072100 qualesim-quiets-1.0.8/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.8/tests/test_cls.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:57:47.000000 qualesim-quiets-1.0.8/tests/test_example_quiets_whitepaper.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.8/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.8/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 12:42:25.663794 qualesim-quiets-1.1.0/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.1.0/LICENSE
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-23 12:42:25.663794 qualesim-quiets-1.1.0/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      289 2024-04-19 07:49:03.000000 qualesim-quiets-1.1.0/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 12:42:25.659794 qualesim-quiets-1.1.0/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 12:42:25.659794 qualesim-quiets-1.1.0/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.1.0/data/bin/dqcsfeqi
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 12:42:25.659794 qualesim-quiets-1.1.0/qualesim_quiets/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.1.0/qualesim_quiets/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.1.0/qualesim_quiets/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    45508 2024-04-23 12:40:45.000000 qualesim-quiets-1.1.0/qualesim_quiets/frontend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11493 2024-04-23 11:44:15.000000 qualesim-quiets-1.1.0/qualesim_quiets/utils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 12:42:25.663794 qualesim-quiets-1.1.0/qualesim_quiets.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-23 12:42:25.000000 qualesim-quiets-1.1.0/qualesim_quiets.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      445 2024-04-23 12:42:25.000000 qualesim-quiets-1.1.0/qualesim_quiets.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-23 12:42:25.000000 qualesim-quiets-1.1.0/qualesim_quiets.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-23 12:42:25.000000 qualesim-quiets-1.1.0/qualesim_quiets.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-23 12:42:25.000000 qualesim-quiets-1.1.0/qualesim_quiets.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-23 12:42:25.663794 qualesim-quiets-1.1.0/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-23 12:41:10.000000 qualesim-quiets-1.1.0/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-23 12:42:25.663794 qualesim-quiets-1.1.0/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.1.0/tests/test_cls.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:57:47.000000 qualesim-quiets-1.1.0/tests/test_example_quiets_whitepaper.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.1.0/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.1.0/tests/test_qifile.py
```

### Comparing `qualesim-quiets-1.0.8/LICENSE` & `qualesim-quiets-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.8/PKG-INFO` & `qualesim-quiets-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.8
+Version: 1.1.0
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quiets-1.0.8/qualesim_quiets/frontend.py` & `qualesim-quiets-1.1.0/qualesim_quiets/frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,14 @@
         args_func_input: List[VariableDecl] = qi_function.get_input_args()
         args_func_output: List[VariableDecl] = qi_function.get_output_args()
         func_data: QiDataStack = func_initial(
             args_func_input, args_func_output, qi_input, qi_output
         )
         func_data.func_name = qi_function.func_name
         func_data.matrix_list[func_data.func_name] = []
-        measure_flag = 0
         # bind the index for formal parameters and arguments.
         output_index = dict()
         for i in range(len(qi_output)):
             if isinstance(qi_output[i], QiVariable):
                 index, name = QiVar_index_name(qi_output[i], func_data)
             else:
                 name = qi_output[i].name
@@ -213,15 +212,14 @@
             # variable declaration
             if isinstance(instr, VariableDecl):
                 self.function_var_decl(instr, func_data)
 
             # function call, and measure is a special form of function call instructions.
             elif isinstance(instr, FunctionCall):
                 if instr.name == "measure":
-                    measure_flag = 1
                     self.function_measure_res(
                         func_body, func_data, measure_mod, get_prob
                     )
                 else:
                     func_data.matrix_list[func_data.func_name].append(
                         "call func " + str(instr)
                     )
@@ -339,38 +337,36 @@
                             func_data.res_qubit.append(ii)
                             tar.append(func_data.func_qubit[ii][0])
                         else:
                             tar.append(func_data.func_qubit[ii][jj])
                             func_data.res_qubit.append(str(ii) + "[" + str(jj) + "]")
             res_state_vector["classical"] = res_cls
             if measure_mod == "state_vector":
-                if measure_flag == 1:
-                    if len(tar) == 0:
-                        res_state_vector["quantum"] = (
-                            [],
-                            [],
-                        )
-                    else:
-                        self.measure(
-                            tar,
-                            arb=ArbData(measure_mod=measure_mod),
-                        )
-                        res_state_vector["quantum"] = (func_data.res_qubit,eval(self.get_measurement(tar[0])["state_for_res"])[1])
+                if len(tar) == 0:
+                    res_state_vector["quantum"] = (
+                        [],
+                        [],
+                    )
+                elif len(func_data.free_list) == 0:
+                    res_state_vector["quantum"] = [1]
+                elif len(func_data.qubit_measure.keys())!= 0:
+                    self.measure(
+                        tar,
+                        arb=ArbData(measure_mod=measure_mod),
+                    )
+                    res_state_vector["quantum"] = (func_data.res_qubit,eval(self.get_measurement(tar[0])["state_for_res"])[1])
                 else:
-                    if len(func_data.free_list) == 0:
-                        res_state_vector["quantum"] = [1]
-                    else:
-                        self.measure(
-                            tar,
-                            arb=ArbData(measure_mod="measureforres"),
-                        )
-                        res_state_vector["quantum"] = (
-                            func_data.res_qubit,
-                            eval(self.get_measurement(tar[0])["state_for_res"])[1],
-                        )
+                    self.measure(
+                        tar,
+                        arb=ArbData(measure_mod="measureforres"),
+                    )
+                    res_state_vector["quantum"] = (
+                        func_data.res_qubit,
+                        eval(self.get_measurement(tar[0])["state_for_res"])[1],
+                    )
             func_data.state_vector = str(res_state_vector)
             for i in func_data.free_list:
                 self.free(func_data.func_qubit[i])
             return func_data, ret
 
         for i in func_data.free_list:
             self.free(func_data.func_qubit[i])
```

### Comparing `qualesim-quiets-1.0.8/qualesim_quiets/utils.py` & `qualesim-quiets-1.1.0/qualesim_quiets/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,14 +304,15 @@
 ):
     func_data: QiDataStack = QiDataStack()
     for i in range(len(args_in)):
         name = args_in[i].var.name
         i_type = check_var_type(args_in[i].type)
         if i_type == 1:
             func_data.func_qubit[name] = qi_input[i]
+            func_data.qubit_list[name] = [-1] * (len(qi_input[i]))
         elif i_type == 2:
             func_data.func_int[name] = qi_input[i]
             if isinstance(args_in[i].var, QiList) and args_in[i].var.size == 0:
                 func_data.changeable_list[name] = str(args_in[i].type)
         elif i_type == 3:
             func_data.func_double[name] = qi_input[i]
             if isinstance(args_in[i].var, QiList) and args_in[i].var.size == 0:
```

### Comparing `qualesim-quiets-1.0.8/qualesim_quiets.egg-info/PKG-INFO` & `qualesim-quiets-1.1.0/qualesim_quiets.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.8
+Version: 1.1.0
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `qualesim-quiets-1.0.8/setup.py` & `qualesim-quiets-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quiets",
-    version="1.0.8",
+    version="1.1.0",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim frontend for QUIET-S.",
     license="GPLv3",
     keywords="qualesim quiets",
     url="https://gitee.com/hpcl_quanta/dqcsim-quiets.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-quiets-1.0.8/tests/test_cls.py` & `qualesim-quiets-1.1.0/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.8/tests/test_gate.py` & `qualesim-quiets-1.1.0/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.8/tests/test_qifile.py` & `qualesim-quiets-1.1.0/tests/test_qifile.py`

 * *Files identical despite different names*

