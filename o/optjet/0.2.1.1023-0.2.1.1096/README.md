# Comparing `tmp/optjet-0.2.1.1023-cp39-cp39-win_amd64.whl.zip` & `tmp/optjet-0.2.1.1096-cp311-cp311-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3857363 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      188 b- defN 24-Apr-01 15:29 optjet/__init__.py
--rw-rw-rw-  2.0 fat  1256448 b- defN 24-Apr-02 06:57 optjet/md_encoder.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  8504320 b- defN 24-Apr-02 06:42 optjet/quant_engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1481 b- defN 24-Apr-02 06:59 optjet-0.2.1.1023.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3225 b- defN 24-Apr-02 06:59 optjet-0.2.1.1023.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-02 06:59 optjet-0.2.1.1023.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-02 06:59 optjet-0.2.1.1023.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      674 b- defN 24-Apr-02 06:59 optjet-0.2.1.1023.dist-info/RECORD
-8 files, 9766443 bytes uncompressed, 3856191 bytes compressed:  60.5%
+Zip file size: 4535301 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      188 b- defN 24-Apr-23 16:36 optjet/__init__.py
+-rw-r--r--  2.0 unx  1650848 b- defN 24-Apr-23 16:36 optjet/md_encoder.cpython-311-darwin.so
+-rwxr-xr-x  2.0 unx 13187312 b- defN 24-Apr-23 16:36 optjet/quant_engine.cpython-311-darwin.so
+-rw-r--r--  2.0 unx     1481 b- defN 24-Apr-23 16:36 optjet-0.2.1.1096.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3175 b- defN 24-Apr-23 16:36 optjet-0.2.1.1096.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-23 16:36 optjet-0.2.1.1096.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-23 16:36 optjet-0.2.1.1096.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      681 b- defN 24-Apr-23 16:36 optjet-0.2.1.1096.dist-info/RECORD
+8 files, 14843802 bytes uncompressed, 4534117 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: optjet/__init__.py
 Comment: 
 
-Filename: optjet/md_encoder.cp39-win_amd64.pyd
+Filename: optjet/md_encoder.cpython-311-darwin.so
 Comment: 
 
-Filename: optjet/quant_engine.cp39-win_amd64.pyd
+Filename: optjet/quant_engine.cpython-311-darwin.so
 Comment: 
 
-Filename: optjet-0.2.1.1023.dist-info/LICENSE
+Filename: optjet-0.2.1.1096.dist-info/LICENSE
 Comment: 
 
-Filename: optjet-0.2.1.1023.dist-info/METADATA
+Filename: optjet-0.2.1.1096.dist-info/METADATA
 Comment: 
 
-Filename: optjet-0.2.1.1023.dist-info/WHEEL
+Filename: optjet-0.2.1.1096.dist-info/WHEEL
 Comment: 
 
-Filename: optjet-0.2.1.1023.dist-info/top_level.txt
+Filename: optjet-0.2.1.1096.dist-info/top_level.txt
 Comment: 
 
-Filename: optjet-0.2.1.1023.dist-info/RECORD
+Filename: optjet-0.2.1.1096.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `optjet-0.2.1.1023.dist-info/LICENSE` & `optjet-0.2.1.1096.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `optjet-0.2.1.1023.dist-info/METADATA` & `optjet-0.2.1.1096.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,77 @@
-Metadata-Version: 2.1
-Name: optjet
-Version: 0.2.1.1023
-Summary: optjet - package of Solvers and Transformers from 'Quantum Systems'
-Author-email: sea <es@qusolve.ru>
-License: Copyright (c) 2022-2024 Quantum Systems
-        
-        Redistribution and use in source and binary forms, with or without modification,
-        are permitted provided that the following conditions are met:
-        1. Redistributions of source code must retain the above copyright notice,
-           this list of conditions and the following disclaimer.
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        3. Neither the name of the copyright holder nor the names of its contributors
-           may be used to endorse or promote products derived from this software
-           without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
-        IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
-        INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-        BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-        DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
-        LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
-        OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
-        ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://en.qusolve.ru/
-Project-URL: Issues, https://en.qusolve.ru/
-Keywords: QuSolve,optjet,quant,SAT solver,linear solver,CNF,WCNF,CNF encoder,maxsat,pseudo-boolean constraint
-Platform: win-amd64
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: C++
-Classifier: License :: Free for non-commercial use
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: <3.12,>=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
- ----------------------------------------------------------------------------- 
-optjet - package of Solvers and Transformers from 'Quantum Systems'
-
-"pip install optjet"
- ----------------------------------------------------------------------------- 
-
-1)
-python package for python-3.x (3.8, 3.9, 3.10, 3.11).
-
-Use in Python
-"
-import optjet
-"
-or
-"
-import optjet.quant_engine as qe
-import optjet.md_encoder as enc
-"
-
-
-2)
-to use in python-3.x on OS Windows and on Linux (Ubuntu 18.04, Ubuntu 22.04, Rocky 9.2) need call:
-"pip install numpy"
- ------------------------------------------------------------------------------ 
+Metadata-Version: 2.1
+Name: optjet
+Version: 0.2.1.1096
+Summary: optjet - package of Solvers and Transformers from 'Quantum Systems'
+Author-email: sea <es@qusolve.ru>
+License: Copyright (c) 2022-2024 Quantum Systems
+        
+        Redistribution and use in source and binary forms, with or without modification,
+        are permitted provided that the following conditions are met:
+        1. Redistributions of source code must retain the above copyright notice,
+           this list of conditions and the following disclaimer.
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        3. Neither the name of the copyright holder nor the names of its contributors
+           may be used to endorse or promote products derived from this software
+           without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+        WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED.
+        IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
+        INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+        BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+        DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
+        LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
+        OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
+        ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://en.qusolve.ru/
+Project-URL: Issues, https://en.qusolve.ru/
+Keywords: QuSolve,optjet,quant,SAT solver,linear solver,CNF,WCNF,CNF encoder,maxsat,pseudo-boolean constraint
+Platform: macosx_11_0_arm64
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: C++
+Classifier: License :: Free for non-commercial use
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: <3.12,>=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# optjet
+
+**optjet** - package of Solvers and Transformers from **'Quantum Systems'**
+
+## Python requirements
+You must have one of the following Python versions installed: 3.8, 3.9, 3.10, 3.11.
+
+You must have "pip" installer.
+
+And you must have one of version NumPy: "pip install numpy"
+
+## Getting started
+``` bash
+pip install optjet
+```
+or for update
+``` bash
+pip install -U optjet
+```
+
+## Use in Python
+``` python
+import optjet
+```
+or
+``` python
+import optjet.quant_engine as qe
+import optjet.md_encoder as enc
+```
+
+## For test
+This package was tested on OS Windows (10, 11) and Linux (Ubuntu 18.04, Ubuntu 22.04, Rocky 9.2).
```

