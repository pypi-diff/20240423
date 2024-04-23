# Comparing `tmp/titanoboa-0.1.8.tar.gz` & `tmp/titanoboa-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titanoboa-0.1.8.tar", last modified: Thu Oct 12 16:48:13 2023, max compression
+gzip compressed data, was "titanoboa-0.1.9.tar", last modified: Thu Mar  7 02:32:22 2024, max compression
```

## Comparing `titanoboa-0.1.8.tar` & `titanoboa-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,67 @@
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.579211 titanoboa-0.1.8/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1256 2022-06-27 13:46:21.000000 titanoboa-0.1.8/LICENSE
--rw-r--r--   0 charles   (1000) charles   (1000)     9352 2023-10-12 16:48:13.579211 titanoboa-0.1.8/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)     7434 2023-09-25 17:15:35.000000 titanoboa-0.1.8/README.md
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.575211 titanoboa-0.1.8/boa/
--rw-rw-r--   0 charles   (1000) charles   (1000)     1225 2023-10-12 00:58:40.000000 titanoboa-0.1.8/boa/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     5971 2023-09-22 15:12:58.000000 titanoboa-0.1.8/boa/coverage.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      797 2023-07-30 17:33:51.000000 titanoboa-0.1.8/boa/debugger.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    20487 2023-10-10 16:33:42.000000 titanoboa-0.1.8/boa/environment.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.575211 titanoboa-0.1.8/boa/integrations/
--rw-rw-r--   0 charles   (1000) charles   (1000)     9507 2023-09-22 15:12:58.000000 titanoboa-0.1.8/boa/integrations/jupyter.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     3312 2023-09-25 17:15:35.000000 titanoboa-0.1.8/boa/interpret.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1371 2023-04-07 20:31:03.000000 titanoboa-0.1.8/boa/ipython.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    13075 2023-09-22 15:12:58.000000 titanoboa-0.1.8/boa/network.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     3940 2023-09-25 17:15:35.000000 titanoboa-0.1.8/boa/precompile.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    13031 2023-07-30 17:33:51.000000 titanoboa-0.1.8/boa/profiling.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     2538 2023-09-22 15:12:58.000000 titanoboa-0.1.8/boa/rpc.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.575211 titanoboa-0.1.8/boa/test/
--rw-rw-r--   0 charles   (1000) charles   (1000)       97 2023-07-30 17:33:51.000000 titanoboa-0.1.8/boa/test/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     2618 2023-09-22 15:12:58.000000 titanoboa-0.1.8/boa/test/plugin.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     7631 2023-09-22 15:12:58.000000 titanoboa-0.1.8/boa/test/strategies.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.579211 titanoboa-0.1.8/boa/util/
--rw-rw-r--   0 charles   (1000) charles   (1000)     2055 2023-07-30 17:33:51.000000 titanoboa-0.1.8/boa/util/disk_cache.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      428 2023-09-22 15:12:58.000000 titanoboa-0.1.8/boa/util/eip1167.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     2132 2023-09-22 15:14:09.000000 titanoboa-0.1.8/boa/util/eip5202.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      625 2023-04-07 20:31:03.000000 titanoboa-0.1.8/boa/util/exceptions.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      973 2023-10-12 01:02:23.000000 titanoboa-0.1.8/boa/util/leveldb.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      587 2023-09-25 17:15:35.000000 titanoboa-0.1.8/boa/util/lrudict.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.579211 titanoboa-0.1.8/boa/vm/
--rw-rw-r--   0 charles   (1000) charles   (1000)     6602 2023-10-12 01:02:23.000000 titanoboa-0.1.8/boa/vm/fork.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1739 2023-04-07 20:31:03.000000 titanoboa-0.1.8/boa/vm/gas_meters.py
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.579211 titanoboa-0.1.8/boa/vyper/
--rw-rw-r--   0 charles   (1000) charles   (1000)       79 2023-07-30 17:33:51.000000 titanoboa-0.1.8/boa/vyper/__init__.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     2006 2023-07-30 17:33:51.000000 titanoboa-0.1.8/boa/vyper/ast_utils.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     3992 2023-10-10 15:47:48.000000 titanoboa-0.1.8/boa/vyper/compiler_utils.py
--rw-rw-r--   0 charles   (1000) charles   (1000)    39690 2023-10-10 15:47:48.000000 titanoboa-0.1.8/boa/vyper/contract.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     3302 2023-09-25 17:15:35.000000 titanoboa-0.1.8/boa/vyper/decoder_utils.py
--rw-rw-r--   0 charles   (1000) charles   (1000)      999 2023-07-30 17:33:51.000000 titanoboa-0.1.8/boa/vyper/event.py
--rw-rw-r--   0 charles   (1000) charles   (1000)     1006 2023-10-12 01:06:00.000000 titanoboa-0.1.8/pyproject.toml
--rw-rw-r--   0 charles   (1000) charles   (1000)      398 2023-10-12 16:48:13.579211 titanoboa-0.1.8/setup.cfg
-drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2023-10-12 16:48:13.579211 titanoboa-0.1.8/titanoboa.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)     9352 2023-10-12 16:48:13.000000 titanoboa-0.1.8/titanoboa.egg-info/PKG-INFO
--rw-rw-r--   0 charles   (1000) charles   (1000)      796 2023-10-12 16:48:13.000000 titanoboa-0.1.8/titanoboa.egg-info/SOURCES.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        1 2023-10-12 16:48:13.000000 titanoboa-0.1.8/titanoboa.egg-info/dependency_links.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)       38 2023-10-12 16:48:13.000000 titanoboa-0.1.8/titanoboa.egg-info/entry_points.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)      133 2023-10-12 16:48:13.000000 titanoboa-0.1.8/titanoboa.egg-info/requires.txt
--rw-rw-r--   0 charles   (1000) charles   (1000)        4 2023-10-12 16:48:13.000000 titanoboa-0.1.8/titanoboa.egg-info/top_level.txt
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.800861 titanoboa-0.1.9/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1256 2022-06-27 13:46:21.000000 titanoboa-0.1.9/LICENSE
+-rw-r--r--   0 charles   (1000) charles   (1000)     9425 2024-03-07 02:32:22.800861 titanoboa-0.1.9/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7434 2023-10-20 18:38:00.000000 titanoboa-0.1.9/README.md
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1981 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/__init__.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/contracts/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/contracts/__init__.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/contracts/abi/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/contracts/abi/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    12584 2024-03-04 17:25:24.000000 titanoboa-0.1.9/boa/contracts/abi/abi_contract.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2828 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/contracts/base_evm_contract.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/contracts/vyper/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/contracts/vyper/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1999 2024-02-28 01:14:37.000000 titanoboa-0.1.9/boa/contracts/vyper/ast_utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4851 2024-03-07 02:18:19.000000 titanoboa-0.1.9/boa/contracts/vyper/compiler_utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     3647 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/contracts/vyper/decoder_utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      993 2024-02-28 01:14:37.000000 titanoboa-0.1.9/boa/contracts/vyper/event.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    30387 2024-03-07 02:18:19.000000 titanoboa-0.1.9/boa/contracts/vyper/ir_executor.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    37146 2024-03-07 02:18:19.000000 titanoboa-0.1.9/boa/contracts/vyper/vyper_contract.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     5986 2024-03-07 02:18:19.000000 titanoboa-0.1.9/boa/coverage.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      797 2023-07-30 17:33:51.000000 titanoboa-0.1.9/boa/debugger.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    24686 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/environment.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1426 2024-02-16 13:29:32.000000 titanoboa-0.1.9/boa/explorer.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/integrations/
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-01-17 15:43:25.000000 titanoboa-0.1.9/boa/integrations/__init__.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/integrations/jupyter/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      815 2024-02-16 13:29:32.000000 titanoboa-0.1.9/boa/integrations/jupyter/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7916 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/integrations/jupyter/browser.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      565 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/integrations/jupyter/constants.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2944 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/integrations/jupyter/handlers.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4698 2024-03-04 17:25:24.000000 titanoboa-0.1.9/boa/integrations/jupyter/jupyter.js
+-rw-rw-r--   0 charles   (1000) charles   (1000)      737 2024-03-07 02:18:20.000000 titanoboa-0.1.9/boa/integrations/jupyter/utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4875 2024-03-07 02:18:20.000000 titanoboa-0.1.9/boa/interpret.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1371 2023-04-07 20:31:03.000000 titanoboa-0.1.9/boa/ipython.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    15138 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/network.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4028 2024-03-07 02:18:20.000000 titanoboa-0.1.9/boa/precompile.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    13041 2024-03-07 02:18:20.000000 titanoboa-0.1.9/boa/profiling.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     4108 2024-02-28 01:14:37.000000 titanoboa-0.1.9/boa/rpc.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/test/
+-rw-rw-r--   0 charles   (1000) charles   (1000)       97 2023-07-30 17:33:51.000000 titanoboa-0.1.9/boa/test/__init__.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2618 2023-09-22 15:12:58.000000 titanoboa-0.1.9/boa/test/plugin.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     7636 2024-02-28 01:14:37.000000 titanoboa-0.1.9/boa/test/strategies.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/util/
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2706 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/util/abi.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2055 2023-07-30 17:33:51.000000 titanoboa-0.1.9/boa/util/disk_cache.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      428 2023-09-22 15:12:58.000000 titanoboa-0.1.9/boa/util/eip1167.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2132 2023-10-20 18:38:00.000000 titanoboa-0.1.9/boa/util/eip5202.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)        0 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/util/evm.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      655 2024-02-16 12:46:12.000000 titanoboa-0.1.9/boa/util/exceptions.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      973 2023-10-20 18:38:00.000000 titanoboa-0.1.9/boa/util/leveldb.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      640 2023-10-20 18:38:00.000000 titanoboa-0.1.9/boa/util/lrudict.py
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.796861 titanoboa-0.1.9/boa/vm/
+-rw-rw-r--   0 charles   (1000) charles   (1000)      852 2023-10-26 22:36:11.000000 titanoboa-0.1.9/boa/vm/fast_accountdb.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     2797 2023-10-20 18:38:00.000000 titanoboa-0.1.9/boa/vm/fast_mem.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)    10879 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/vm/fork.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1756 2024-03-04 17:25:21.000000 titanoboa-0.1.9/boa/vm/gas_meters.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)      381 2023-10-20 18:38:00.000000 titanoboa-0.1.9/boa/vm/utils.py
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1314 2024-03-07 02:18:30.000000 titanoboa-0.1.9/pyproject.toml
+-rw-rw-r--   0 charles   (1000) charles   (1000)      398 2024-03-07 02:32:22.800861 titanoboa-0.1.9/setup.cfg
+drwxrwxr-x   0 charles   (1000) charles   (1000)        0 2024-03-07 02:32:22.800861 titanoboa-0.1.9/titanoboa.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)     9425 2024-03-07 02:32:22.000000 titanoboa-0.1.9/titanoboa.egg-info/PKG-INFO
+-rw-rw-r--   0 charles   (1000) charles   (1000)     1349 2024-03-07 02:32:22.000000 titanoboa-0.1.9/titanoboa.egg-info/SOURCES.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        1 2024-03-07 02:32:22.000000 titanoboa-0.1.9/titanoboa.egg-info/dependency_links.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)       38 2024-03-07 02:32:22.000000 titanoboa-0.1.9/titanoboa.egg-info/entry_points.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)      176 2024-03-07 02:32:22.000000 titanoboa-0.1.9/titanoboa.egg-info/requires.txt
+-rw-rw-r--   0 charles   (1000) charles   (1000)        4 2024-03-07 02:32:22.000000 titanoboa-0.1.9/titanoboa.egg-info/top_level.txt
```

### Comparing `titanoboa-0.1.8/LICENSE` & `titanoboa-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/PKG-INFO` & `titanoboa-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanoboa
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Vyper interpreter
 License: Copyright 2022 Charles Cooper
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -13,20 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Keywords: ethereum,evm,smart contract,development
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vyper>=0.3.10
-Requires-Dist: eth-stdlib
+Requires-Dist: eth-stdlib<0.3.0,>=0.2.7
 Requires-Dist: eth-abi
 Requires-Dist: py-evm>=0.7.0a4
 Requires-Dist: eth-typing
 Requires-Dist: hypothesis
 Requires-Dist: pytest
+Requires-Dist: pytest-cov
+Requires-Dist: typing-extensions
 Requires-Dist: rich
 Requires-Dist: requests
 Requires-Dist: eth-account
 Provides-Extra: forking-recommended
 Requires-Dist: ujson; extra == "forking-recommended"
 
 # Titanoboa
```

### Comparing `titanoboa-0.1.8/README.md` & `titanoboa-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/boa/coverage.py` & `titanoboa-0.1.9/boa/coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import cached_property
 
 import coverage.plugin
 import vyper.ast as vy_ast
 from vyper.ir import compile_ir
 
 import boa.interpret
+from boa.contracts.vyper.ast_utils import get_fn_ancestor_from_node
 from boa.environment import Env
-from boa.vyper.ast_utils import get_fn_ancestor_from_node
 
 
 def coverage_init(registry, options):
     plugin = TitanoboaPlugin(options)
     registry.add_file_tracer(plugin)
     registry.add_configurer(plugin)
 
@@ -64,15 +64,15 @@
         return frame.f_locals["contract"]
 
     def dynamic_source_filename(self, filename, frame):
         contract = self._contract_for_frame(frame)
         if contract is None:
             return None
 
-        return contract.filename
+        return str(contract.filename)
 
     def has_dynamic_source_filename(self):
         return True
 
     # https://coverage.rtfd.io/en/stable/api_plugin.html#coverage.FileTracer.line_number_range
     def line_number_range(self, frame):
         contract = self._contract_for_frame(frame)
```

### Comparing `titanoboa-0.1.8/boa/debugger.py` & `titanoboa-0.1.9/boa/debugger.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/boa/environment.py` & `titanoboa-0.1.9/boa/environment.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,33 +2,39 @@
 # handles low level details around state and py-evm tracing.
 
 import contextlib
 import logging
 import random
 import sys
 import warnings
-from typing import Any, Iterator, Optional, Union
+from typing import Any, Iterator, Optional, TypeAlias
 
 import eth.constants as constants
 import eth.tools.builder.chain as chain
 import eth.vm.forks.spurious_dragon.computation as spurious_dragon
 from eth._utils.address import generate_contract_address
 from eth.chains.mainnet import MainnetChain
-from eth.codecs import abi
+from eth.db.account import AccountDB
 from eth.db.atomic import AtomicDB
+from eth.exceptions import Halt
 from eth.vm.code_stream import CodeStream
+from eth.vm.gas_meter import allow_negative_refund_strategy
 from eth.vm.message import Message
 from eth.vm.opcode_values import STOP
 from eth.vm.transaction_context import BaseTransactionContext
-from eth_typing import Address
-from eth_utils import setup_DEBUG2_logging, to_canonical_address, to_checksum_address
+from eth_typing import Address as PYEVM_Address  # it's just bytes.
+from eth_utils import setup_DEBUG2_logging
 
+from boa.rpc import RPC, EthereumRPC
+from boa.util.abi import Address, abi_decode
 from boa.util.eip1167 import extract_eip1167_address, is_eip1167_contract
+from boa.vm.fast_accountdb import patch_pyevm_state_object, unpatch_pyevm_state_object
 from boa.vm.fork import AccountDBFork
 from boa.vm.gas_meters import GasMeter, NoGasMeter, ProfilingGasMeter
+from boa.vm.utils import to_bytes, to_int
 
 
 def enable_pyevm_verbose_logging():
     logging.basicConfig()
     logger = logging.getLogger("eth.vm.computation.Computation")
     setup_DEBUG2_logging()
     logger.setLevel("DEBUG2")
@@ -86,19 +92,16 @@
 
         finally:
             for s, _ in self._patchables:
                 for attr in s:
                     setattr(self, attr, snap[attr])
 
 
-AddressType = Union[Address, bytes, str]  # make mypy happy
-
-
-def _addr(addr: AddressType) -> Address:
-    return Address(to_canonical_address(addr))
+# make mypy happy
+_AddressType: TypeAlias = Address | str | bytes | PYEVM_Address
 
 
 _opcode_overrides = {}
 
 
 def patch_opcode(opcode_value, fn):
     global _opcode_overrides
@@ -117,31 +120,31 @@
     warnings.warn(
         "register_recompile has been renamed to register_raw_precompile!", stacklevel=2
     )
 
 
 def register_raw_precompile(address, fn, force=False):
     global _precompiles
-    address = _addr(address)
+    address = Address(address)
     if address in _precompiles and not force:
         raise ValueError(f"Already registered: {address}")
-    _precompiles[address] = fn
+    _precompiles[address.canonical_address] = fn
 
 
 def deregister_raw_precompile(address, force=True):
-    address = _addr(address)
+    address = Address(address).canonical_address
     if address not in _precompiles and not force:
         raise ValueError("Not registered: {address}")
     _precompiles.pop(address, None)
 
 
 def console_log(computation):
     msgdata = computation.msg.data_as_bytes
-    schema, payload = abi.decode("(string,bytes)", msgdata[4:])
-    data = abi.decode(schema, payload)
+    schema, payload = abi_decode("(string,bytes)", msgdata[4:])
+    data = abi_decode(schema, payload)
     print(*data, file=sys.stderr)
     return computation
 
 
 CONSOLE_ADDRESS = bytes.fromhex("000000000000000000636F6E736F6C652E6C6F67")
 
 
@@ -180,91 +183,201 @@
     def __len__(self):
         if self._fake_codesize is not None:
             return self._fake_codesize
         return self._length_cache
 
 
 # ### section: sha3 preimage tracing
-# (TODO: move to dedicated module)
-def to_int(value):
+def _stackitem_to_int(value):
     if isinstance(value, tuple):
-        return to_int(value[1])  # how py-evm stores stuff on stack
-    if isinstance(value, int):
-        return value
-    if isinstance(value, bytes):
-        return int.from_bytes(value, "big")
+        return to_int(value[1])  # how py-evm<=0.8.0b1 stores stuff on stack
+    else:
+        return to_int(value)
 
-    raise ValueError("invalid type %s", type(value))
 
-
-def to_bytes(value):
+def _stackitem_to_bytes(value):
     if isinstance(value, tuple):
-        return to_bytes(value[1])  # how py-evm stores stuff on stack
-    if isinstance(value, bytes):
-        return value
-    if isinstance(value, int):
-        return value.to_bytes(32, "big")
-
-    raise ValueError("invalid type %s", type(value))
+        return to_bytes(value[1])  # how py-evm<=0.8.0b1 stores stuff on stack
+    else:
+        return to_bytes(value)
 
 
 class Sha3PreimageTracer:
     mnemonic = "SHA3"
 
     # trace preimages of sha3
 
-    def __init__(self, sha3_op, preimage_map):
-        self.preimages = preimage_map
+    def __init__(self, sha3_op, env):
+        self.env = env
         self.sha3 = sha3_op
 
     def __call__(self, computation):
-        size, offset = [to_int(x) for x in computation._stack.values[-2:]]
+        size, offset = [_stackitem_to_int(x) for x in computation._stack.values[-2:]]
 
         # dispatch into py-evm
         self.sha3(computation)
 
         if size != 64:
             return
 
         preimage = computation._memory.read_bytes(offset, size)
 
-        image = to_bytes(computation._stack.values[-1])
+        image = _stackitem_to_bytes(computation._stack.values[-1])
 
-        self.preimages[image] = preimage
+        self.env._trace_sha3_preimage(preimage, image)
 
 
 class SstoreTracer:
     mnemonic = "SSTORE"
 
-    def __init__(self, sstore_op, trace_db):
-        self.trace_db = trace_db
+    def __init__(self, sstore_op, env):
+        self.env = env
         self.sstore = sstore_op
 
     def __call__(self, computation):
-        value, slot = [to_bytes(t) for t in computation._stack.values[-2:]]
-        account = to_checksum_address(computation.msg.storage_address)
+        value, slot = [_stackitem_to_int(t) for t in computation._stack.values[-2:]]
+        account = computation.msg.storage_address
 
-        self.trace_db.setdefault(account, set())
-        # we don't want to deal with snapshots/commits/reverts, so just
-        # register that the slot was touched and downstream can filter
-        # zero entries.
-        self.trace_db[account].add(slot)
+        self.env._trace_sstore(account, slot)
 
         # dispatch into py-evm
         self.sstore(computation)
 
 
 # ### End section: sha3 tracing
 
 
+# py-evm uses class instantiaters which need to be classes
+# instead of like factories or other easier to use architectures -
+# `titanoboa_computation` is a class which can be constructed dynamically
+class titanoboa_computation:
+    _gas_meter_class = GasMeter
+
+    def __init__(self, *args, **kwargs):
+        # super() hardcodes CodeStream into the ctor
+        # so we have to override it here
+        super().__init__(*args, **kwargs)
+
+        self.code = TracingCodeStream(
+            self.code._raw_code_bytes,
+            fake_codesize=getattr(self.msg, "_fake_codesize", None),
+            start_pc=getattr(self.msg, "_start_pc", 0),
+        )
+        global _precompiles
+        # copy so as not to mess with class state
+        self._precompiles = self._precompiles.copy()
+        self._precompiles.update(_precompiles)
+
+        global _opcode_overrides
+        # copy so as not to mess with class state
+        self.opcodes = self.opcodes.copy()
+        self.opcodes.update(_opcode_overrides)
+
+        self._gas_meter = self._gas_meter_class(
+            self.msg.gas, refund_strategy=allow_negative_refund_strategy
+        )
+        if hasattr(self._gas_meter, "_set_code"):
+            self._gas_meter._set_code(self.code)
+
+        self._child_pcs = []
+        self._contract_repr_before_revert = None
+
+    @property
+    def net_gas_used(self):
+        return max(0, self.get_gas_used() - self.get_gas_refund())
+
+    def add_child_computation(self, child_computation):
+        super().add_child_computation(child_computation)
+        # track PCs of child calls for profiling purposes
+        self._child_pcs.append(self.code.program_counter)
+
+    # hijack creations to automatically generate blueprints
+    @classmethod
+    def apply_create_message(cls, state, msg, tx_ctx):
+        computation = super().apply_create_message(state, msg, tx_ctx)
+
+        bytecode = msg.code
+        # cf. eth/vm/logic/system/Create* opcodes
+        contract_address = msg.storage_address
+
+        if is_eip1167_contract(bytecode):
+            contract_address = extract_eip1167_address(bytecode)
+            bytecode = cls.env.vm.state.get_code(contract_address)
+
+        if bytecode in cls.env._code_registry:
+            target = cls.env._code_registry[bytecode].deployer.at(contract_address)
+            target.created_from = Address(msg.sender)
+            cls.env.register_contract(contract_address, target)
+
+        return computation
+
+    @classmethod
+    def apply_computation(cls, state, msg, tx_ctx):
+        addr = msg.code_address
+        contract = cls.env._lookup_contract_fast(addr) if addr else None
+
+        def finalize(c):
+            if c.is_error:
+                # After the computation is applied with an error the state is
+                # reverted. Before the revert, save the contract repr for the
+                # error message
+                c._contract_repr_before_revert = repr(contract)
+            return c
+
+        if contract is None or not cls.env._fast_mode_enabled:
+            # print("SLOW MODE")
+            computation = super().apply_computation(state, msg, tx_ctx)
+            return finalize(computation)
+
+        with cls(state, msg, tx_ctx) as computation:
+            try:
+                if getattr(msg, "_ir_executor", None) is not None:
+                    # print("MSG HAS IR EXECUTOR")
+                    # this happens when bytecode is overridden, e.g.
+                    # for injected functions. note ir_executor is (correctly)
+                    # used for the outer computation only because on subcalls
+                    # a clean message is constructed for the child computation
+                    msg._ir_executor.exec(computation)
+                else:
+                    # print("REGULAR FAST MODE")
+                    contract.ir_executor.exec(computation)
+            except Halt:
+                pass
+
+        # return computation outside of with block; computation.__exit__
+        # swallows exceptions (including Revert).
+        return finalize(computation)
+
+
+# Message object with extra attrs we can use to thread things through
+# the execution context.
+class FakeMessage(Message):
+    def __init__(
+        self,
+        *args,
+        ir_executor=None,
+        fake_codesize=None,
+        start_pc=0,
+        contract=None,
+        **kwargs,
+    ):
+        super().__init__(*args, **kwargs)
+        self._ir_executor = ir_executor
+        self._fake_codesize = fake_codesize
+        self._start_pc = start_pc
+        self._contract = contract
+
+
 # wrapper class around py-evm which provides a "contract-centric" API
 class Env:
     _singleton = None
     _random = random.Random("titanoboa")  # something reproducible
     _coverage_enabled = False
+    _fast_mode_enabled = False
+    _fork_try_prefetch_state = False
 
     def __init__(self):
         self.chain = _make_chain()
 
         self._gas_price = None
 
         self._aliases = {}
@@ -276,110 +389,93 @@
         self._code_registry = {}
 
         self._profiled_contracts = {}
         self._cached_call_profiles = {}
         self._cached_line_profiles = {}
         self._coverage_data = {}
 
+        self._gas_tracker = 0
+
         self.sha3_trace = {}
         self.sstore_trace = {}
 
         self._init_vm()
 
     def set_random_seed(self, seed=None):
         self._random = random.Random(seed)
 
     def get_gas_price(self):
         return self._gas_price or 0
 
-    def _init_vm(self, reset_traces=True):
+    def _init_vm(self, reset_traces=True, account_db_class=AccountDB):
         self.vm = self.chain.get_vm()
+        self.vm.__class__._state_class.account_db_class = account_db_class
         self.vm.patch = VMPatcher(self.vm)
 
-        env = self
-
-        class OpcodeTracingComputation(self.vm.state.computation_class):
-            _gas_meter_class = GasMeter
-
-            def __init__(self, *args, **kwargs):
-                # super() hardcodes CodeStream into the ctor
-                # so we have to override it here
-                super().__init__(*args, **kwargs)
-                self.code = TracingCodeStream(
-                    self.code._raw_code_bytes,
-                    fake_codesize=getattr(self.msg, "_fake_codesize", None),
-                    start_pc=getattr(self.msg, "_start_pc", 0),
-                )
-                global _precompiles
-                # copy so as not to mess with class state
-                self._precompiles = self._precompiles.copy()
-                self._precompiles.update(_precompiles)
-
-                global _opcode_overrides
-                # copy so as not to mess with class state
-                self.opcodes = self.opcodes.copy()
-                self.opcodes.update(_opcode_overrides)
-
-                self._gas_meter = self._gas_meter_class(self.msg.gas)
-                if hasattr(self._gas_meter, "_set_code"):
-                    self._gas_meter._set_code(self.code)
-
-                self._child_pcs = []
-
-            def add_child_computation(self, child_computation):
-                super().add_child_computation(child_computation)
-                # track PCs of child calls for profiling purposes
-                self._child_pcs.append(self.code.program_counter)
-
-            # hijack creations to automatically generate blueprints
-            @classmethod
-            def apply_create_message(cls, state, msg, tx_ctx):
-                computation = super().apply_create_message(state, msg, tx_ctx)
-
-                bytecode = msg.code
-                # cf. eth/vm/logic/system/Create* opcodes
-                contract_address = msg.storage_address
-
-                if is_eip1167_contract(bytecode):
-                    contract_address = extract_eip1167_address(bytecode)
-                    bytecode = self.vm.state.get_code(contract_address)
-
-                if bytecode in self._code_registry:
-                    target = self._code_registry[bytecode].deployer.at(contract_address)
-                    target.created_from = to_checksum_address(msg.sender)
-                    env.register_contract(contract_address, target)
-
-                return computation
+        c = type(
+            "TitanoboaComputation",
+            (titanoboa_computation, self.vm.state.computation_class),
+            {"env": self},
+        )
 
-        # TODO make metering toggle-able
-        c = OpcodeTracingComputation
+        if self._fast_mode_enabled:
+            patch_pyevm_state_object(self.vm.state)
 
         self.vm.state.computation_class = c
 
         # we usually want to reset the trace data structures
         # but sometimes don't, give caller the option.
         if reset_traces:
             self.sha3_trace = {}
             self.sstore_trace = {}
 
         # patch in tracing opcodes
-        c.opcodes[0x20] = Sha3PreimageTracer(c.opcodes[0x20], self.sha3_trace)
-        c.opcodes[0x55] = SstoreTracer(c.opcodes[0x55], self.sstore_trace)
+        c.opcodes[0x20] = Sha3PreimageTracer(c.opcodes[0x20], self)
+        c.opcodes[0x55] = SstoreTracer(c.opcodes[0x55], self)
+
+    def _trace_sha3_preimage(self, preimage, image):
+        self.sha3_trace[image] = preimage
 
-    def fork(self, url, reset_traces=True, **kwargs):
-        kwargs["url"] = url
-        AccountDBFork._rpc_init_kwargs = kwargs
-        self.vm.__class__._state_class.account_db_class = AccountDBFork
-        self._init_vm(reset_traces=reset_traces)
+    def _trace_sstore(self, account, slot):
+        self.sstore_trace.setdefault(account, set())
+        # we don't want to deal with snapshots/commits/reverts, so just
+        # register that the slot was touched and downstream can filter
+        # zero entries.
+        self.sstore_trace[account].add(slot)
+
+    def enable_fast_mode(self, flag: bool = True):
+        self._fast_mode_enabled = flag
+        if flag:
+            patch_pyevm_state_object(self.vm.state)
+        else:
+            unpatch_pyevm_state_object(self.vm.state)
+
+    def fork(self, url: str, reset_traces=True, block_identifier="safe", **kwargs):
+        return self.fork_rpc(EthereumRPC(url), reset_traces, block_identifier, **kwargs)
+
+    def fork_rpc(self, rpc: RPC, reset_traces=True, block_identifier="safe", **kwargs):
+        """
+        Fork the environment to a local chain.
+        :param rpc: RPC to fork from
+        :param reset_traces: Reset the traces
+        :param block_identifier: Block identifier to fork from
+        :param kwargs: Additional arguments for the RPC
+        """
+        account_db_class = AccountDBFork.class_from_rpc(rpc, block_identifier, **kwargs)
+        self._init_vm(reset_traces, account_db_class)
         block_info = self.vm.state._account_db._block_info
 
         self.vm.patch.timestamp = int(block_info["timestamp"], 16)
         self.vm.patch.block_number = int(block_info["number"], 16)
         # TODO patch the other stuff
 
+    @property
+    def _fork_mode(self):
+        return self.vm.__class__._state_class.account_db_class == AccountDBFork
+
     def set_gas_meter_class(self, cls: type) -> None:
         self.vm.state.computation_class._gas_meter_class = cls
 
     @contextlib.contextmanager
     def gas_meter_class(self, cls):
         tmp = self.vm.state.computation_class._gas_meter_class
         try:
@@ -396,137 +492,157 @@
 
     def reset_gas_metering_behavior(self) -> None:
         # Reset gas metering to the default behavior
         self.set_gas_meter_class(GasMeter)
 
     # set balance of address in py-evm
     def set_balance(self, addr, value):
-        self.vm.state.set_balance(to_canonical_address(addr), value)
+        self.vm.state.set_balance(Address(addr).canonical_address, value)
 
     # get balance of address in py-evm
     def get_balance(self, addr):
-        return self.vm.state.get_balance(to_canonical_address(addr))
+        return self.vm.state.get_balance(Address(addr).canonical_address)
 
     def register_contract(self, address, obj):
-        self._contracts[to_checksum_address(address)] = obj
+        addr = Address(address).canonical_address
+        self._contracts[addr] = obj
 
         # also register it in the registry for
         # create_minimal_proxy_to and create_copy_of
-        bytecode = self.vm.state.get_code(to_canonical_address(address))
+        bytecode = self.vm.state.get_code(addr)
         self._code_registry[bytecode] = obj
 
     def register_blueprint(self, bytecode, obj):
         self._code_registry[bytecode] = obj
 
-    def lookup_contract(self, address):
+    def _lookup_contract_fast(self, address: PYEVM_Address):
+        return self._contracts.get(address)
+
+    def lookup_contract(self, address: _AddressType):
         if address == b"":
             return None
-        return self._contracts.get(to_checksum_address(address))
+        return self._contracts.get(Address(address).canonical_address)
 
     def alias(self, address, name):
-        self._aliases[to_checksum_address(address)] = name
+        self._aliases[Address(address).canonical_address] = name
 
     def lookup_alias(self, address):
-        return self._aliases[to_checksum_address(address)]
+        return self._aliases[Address(address).canonical_address]
 
     # advanced: reset warm/cold counters for addresses and storage
     def _reset_access_counters(self):
         self.vm.state._account_db._reset_access_counters()
 
+    def get_gas_used(self):
+        return self._gas_tracker
+
+    def reset_gas_used(self):
+        self._gas_tracker = 0
+        self._reset_access_counters()
+
     # context manager which snapshots the state and reverts
     # to the snapshot on exiting the with statement
     @contextlib.contextmanager
     def anchor(self):
         snapshot_id = self.vm.state.snapshot()
         try:
             with self.vm.patch.anchor():
                 yield
         finally:
             self.vm.state.revert(snapshot_id)
 
     @contextlib.contextmanager
     def sender(self, address):
         tmp = self.eoa
-        self.eoa = to_checksum_address(address)
+        self.eoa = Address(address)
         try:
             yield
         finally:
             self.eoa = tmp
 
     def prank(self, *args, **kwargs):
         return self.sender(*args, **kwargs)
 
     @classmethod
     def get_singleton(cls):
         if cls._singleton is None:
             cls._singleton = cls()
         return cls._singleton
 
-    def generate_address(self, alias: Optional[str] = None) -> AddressType:
-        t = self._random.randbytes(20)
-        # checksum addr easier for humans to debug
-        ret = to_checksum_address(t)
+    def generate_address(self, alias: Optional[str] = None) -> _AddressType:
+        t = Address(self._random.randbytes(20))
         if alias is not None:
-            self.alias(ret, alias)
+            self.alias(t, alias)
 
-        return ret
+        return t
 
     # helper fn
-    def _get_sender(self, sender=None) -> Address:
+    def _get_sender(self, sender=None) -> PYEVM_Address:
         if sender is None:
             sender = self.eoa
         if self.eoa is None:
             raise ValueError(f"{self}.eoa not defined!")
-        return _addr(sender)
+        return Address(sender).canonical_address
+
+    def _update_gas_used(self, gas_used: int):
+        self._gas_tracker += gas_used
 
     def deploy_code(
         self,
-        sender: Optional[AddressType] = None,
+        sender: Optional[_AddressType] = None,
         gas: Optional[int] = None,
         value: int = 0,
         bytecode: bytes = b"",
         start_pc: int = 0,
         # override the target address:
-        override_address: Optional[AddressType] = None,
-    ) -> tuple[AddressType, bytes]:
+        override_address: Optional[_AddressType] = None,
+    ) -> tuple[Address, bytes]:
         if gas is None:
             gas = self.vm.state.gas_limit
+
         sender = self._get_sender(sender)
 
         if override_address is not None:
-            target_address = _addr(override_address)
+            target_address = Address(override_address)
         else:
             nonce = self.vm.state.get_nonce(sender)
             self.vm.state.increment_nonce(sender)
-            target_address = generate_contract_address(sender, nonce)
+            target_address = Address(generate_contract_address(sender, nonce))
 
         msg = Message(
             to=constants.CREATE_CONTRACT_ADDRESS,  # i.e., b""
             sender=sender,
             gas=gas,
             value=value,
             code=bytecode,
-            create_address=target_address,
+            create_address=target_address.canonical_address,
             data=b"",
         )
+
+        if self._fork_mode and self._fork_try_prefetch_state:
+            self.vm.state._account_db.try_prefetch_state(msg)
+
         origin = sender  # XXX: consider making this parametrizable
         tx_ctx = BaseTransactionContext(origin=origin, gas_price=self.get_gas_price())
         c = self.vm.state.computation_class.apply_create_message(
             self.vm.state, msg, tx_ctx
         )
 
+        if c._gas_meter_class != NoGasMeter:
+            self._update_gas_used(c.get_gas_used())
+
         if c.is_error:
             raise c.error
 
         return target_address, c.output
 
     def raw_call(
         self,
         to_address,
-        sender: Optional[AddressType] = None,
+        sender: Optional[_AddressType] = None,
         gas: Optional[int] = None,
         value: int = 0,
         data: bytes = b"",
     ):
         # simple wrapper around `execute_code` to help simulate calling
         # a contract from an EOA.
         ret = self.execute_code(
@@ -539,33 +655,32 @@
             # like a regular contract call.
             raise ret.error
 
         return ret
 
     def execute_code(
         self,
-        to_address: AddressType = constants.ZERO_ADDRESS,
-        sender: Optional[AddressType] = None,
+        to_address: _AddressType = constants.ZERO_ADDRESS,
+        sender: Optional[_AddressType] = None,
         gas: Optional[int] = None,
         value: int = 0,
         data: bytes = b"",
         override_bytecode: Optional[bytes] = None,
+        ir_executor: Any = None,
         is_modifying: bool = True,
         start_pc: int = 0,
         fake_codesize: Optional[int] = None,
         contract: Any = None,  # the calling VyperContract
     ) -> Any:
         if gas is None:
             gas = self.vm.state.gas_limit
-        sender = self._get_sender(sender)
 
-        class FakeMessage(Message):  # Message object with settable attrs
-            __dict__: dict = {}
+        sender = self._get_sender(sender)
 
-        to = _addr(to_address)
+        to = Address(to_address).canonical_address
 
         bytecode = override_bytecode
         if override_bytecode is None:
             bytecode = self.vm.state.get_code(to)
 
         is_static = not is_modifying
 
@@ -573,37 +688,46 @@
             sender=sender,
             to=to,
             gas=gas,
             value=value,
             code=bytecode,  # type: ignore
             data=data,
             is_static=is_static,
+            fake_codesize=fake_codesize,
+            start_pc=start_pc,
+            ir_executor=ir_executor,
+            contract=contract,
         )
+        if self._fork_mode and self._fork_try_prefetch_state:
+            self.vm.state._account_db.try_prefetch_state(msg)
 
-        msg._fake_codesize = fake_codesize  # type: ignore
-        msg._start_pc = start_pc  # type: ignore
-        msg._contract = contract  # type: ignore
         origin = sender  # XXX: consider making this parametrizable
         tx_ctx = BaseTransactionContext(origin=origin, gas_price=self.get_gas_price())
+
         ret = self.vm.state.computation_class.apply_message(self.vm.state, msg, tx_ctx)
 
         if self._coverage_enabled:
             self._hook_trace_computation(ret, contract)
 
+        if ret._gas_meter_class != NoGasMeter:
+            self._update_gas_used(ret.get_gas_used())
+
         return ret
 
     def _hook_trace_computation(self, computation, contract=None):
         # XXX perf: don't trace if contract is None
         for _pc in computation.code._trace:
             # loop over pc so that it is available when coverage hooks into it
             pass
+
         for child in computation.children:
-            if child.msg.code_address != b"":
-                child_contract = self.lookup_contract(child.msg.code_address)
-                self._hook_trace_computation(child, child_contract)
+            if child.msg.code_address == b"":
+                continue
+            child_contract = self._lookup_contract_fast(child.msg.code_address)
+            self._hook_trace_computation(child, child_contract)
 
     # function to time travel
     def time_travel(
         self,
         seconds: Optional[int] = None,
         blocks: Optional[int] = None,
         block_delta: int = 12,
```

### Comparing `titanoboa-0.1.8/boa/ipython.py` & `titanoboa-0.1.9/boa/ipython.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/boa/network.py` & `titanoboa-0.1.9/boa/network.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 # an Environment which interacts with a real (prod or test) chain
 import contextlib
-import time
 import warnings
+from dataclasses import dataclass
 from functools import cached_property
 from math import ceil
 
 from eth_account import Account
-from eth_utils import to_canonical_address, to_checksum_address
+from requests.exceptions import HTTPError
 
 from boa.environment import Env
-from boa.rpc import EthereumRPC, RPCError, to_bytes, to_hex, to_int
+from boa.rpc import (
+    RPC,
+    EthereumRPC,
+    RPCError,
+    fixup_dict,
+    to_bytes,
+    to_hex,
+    to_int,
+    trim_dict,
+)
+from boa.util.abi import Address
 
 
 class TraceObject:
     def __init__(self, raw_trace):
         self.raw_trace = raw_trace
 
     @cached_property
@@ -33,46 +43,79 @@
     def is_error(self):
         if "structLogs" in self.raw_trace:
             return self.raw_trace["failed"]
         else:
             return "error" in self.raw_trace
 
 
-def trim_dict(kv):
-    return {k: v for (k, v) in kv.items() if bool(v)}
-
-
-def _fixup_dict(kv):
-    return {k: to_hex(v) for (k, v) in trim_dict(kv).items()}
-
-
 class _EstimateGasFailed(Exception):
     pass
 
 
+@dataclass
+class TransactionSettings:
+    # when calculating the base fee, the number of blocks N ahead
+    # to compute a cap for the Nth block.
+    # defaults to 4 (4 blocks ahead, pending block's baseFee * ~1.6)
+    # but can be tweaked. if you get errors like
+    # `boa.rpc.RPCError: -32000: err: max fee per gas less than block base fee`
+    # try increasing the constant.
+    # do not recommend setting below 0.
+    base_fee_estimator_constant: int = 4
+
+    # amount of time to wait, in seconds before giving up on a transaction
+    poll_timeout: float = 240.0
+
+
+@dataclass
+class ExternalAccount:
+    address: Address
+    _rpc: EthereumRPC
+
+    def __post_init__(self):
+        self.address = Address(self.address)
+
+    def send_transaction(self, tx_data):
+        txhash = self._rpc.fetch("eth_sendTransaction", [tx_data])
+        # format to be the same as what BrowserSigner returns
+        return {"hash": txhash}
+
+
 class NetworkEnv(Env):
     """
     An Env object which can be swapped in via `boa.set_env()`.
     It runs non-mutable (view or pure) functions via eth_call,
     mutable functions and contract creation via eth_sendRawTransaction.
     """
 
-    def __init__(self, rpc_url, accounts=None):
+    # always prefetch state in network mode
+    _fork_try_prefetch_state = True
+
+    def __init__(self, rpc: str | RPC, accounts: dict[str, Account] = None):
         super().__init__()
 
-        self._rpc = EthereumRPC(rpc_url)
+        if isinstance(rpc, str):
+            warnings.warn(
+                "NetworkEnv(url) is deprecated. Use boa.set_network_env(url) instead.",
+                stacklevel=2,
+            )
+            rpc = EthereumRPC(rpc)
+
+        self._rpc = rpc
 
         self._reset_fork()
 
-        self._accounts: dict[str, Account] = accounts or {}
+        self._accounts = accounts or {}
 
         self.eoa = None
 
         self._gas_price = None
 
+        self.tx_settings = TransactionSettings()
+
     @cached_property
     def _rpc_has_snapshot(self):
         try:
             snapshot_id = self._rpc.fetch("evm_snapshot", [])
             self._rpc.fetch("evm_revert", [snapshot_id])
             return True
         except RPCError:
@@ -90,91 +133,108 @@
             # note we cannot call super.anchor() because vm/accountdb fork
             # state is reset after every txn.
         finally:
             self._rpc.fetch("evm_revert", [snapshot_id])
             # wipe forked state
             self._reset_fork(blkid)
 
+    # add account, or "Account-like" object. MUST expose
+    # `sign_transaction` or `send_transaction` method!
     def add_account(self, account: Account, force_eoa=False):
         self._accounts[account.address] = account  # type: ignore
         if self.eoa is None or force_eoa:
             self.eoa = account.address  # type: ignore
 
+    def add_accounts_from_rpc(self, rpc: str | EthereumRPC) -> None:
+        if isinstance(rpc, str):
+            rpc = EthereumRPC(rpc)
+
+        # address strings, ex. ["0x0e5437b1b3448d22c07caed31e5bcdc4ec5284a9"]
+        addresses = rpc.fetch("eth_accounts", [])
+        if not addresses:
+            # strip out content in the URL which might not want to get into logs
+            warnings.warn(f"No accounts fetched from <{rpc.name}>!", stacklevel=2)
+        for address in addresses:
+            self.add_account(ExternalAccount(_rpc=rpc, address=address))  # type: ignore
+
     def set_eoa(self, eoa: Account) -> None:
         self.add_account(eoa, force_eoa=True)
 
+    @classmethod
+    def from_url(cls, url: str) -> "NetworkEnv":
+        return cls(EthereumRPC(url))
+
     # overrides
     def get_gas_price(self) -> int:
         if self._gas_price is not None:
             return self._gas_price
         return to_int(self._rpc.fetch("eth_gasPrice", []))
 
-    # when calculating the base fee, the number of blocks N ahead
-    # to compute a cap for the Nth block.
-    # defaults to 0 (no blocks ahead, just use pending block's baseFee)
-    # but can be tweaked if you get errors like
-    # `boa.rpc.RPCError: -32000: err: max fee per gas less than block base fee`
-
-    BASE_FEE_ESTIMATOR_CONSTANT = 0
-
-    def get_fee_info(self) -> tuple[str, str, str, str]:
+    def get_eip1559_fee(self) -> tuple[str, str, str, str]:
         # returns: base_fee, max_fee, max_priority_fee
         reqs = [
             ("eth_getBlockByNumber", ["pending", False]),
             ("eth_maxPriorityFeePerGas", []),
             ("eth_chainId", []),
         ]
         block_info, max_priority_fee, chain_id = self._rpc.fetch_multi(reqs)
         base_fee = block_info["baseFeePerGas"]
 
         # Each block increases the base fee by 1/8 at most.
         # here we have the next block's base fee, compute a cap for the
         # next N blocks here.
-        blocks_ahead = self.BASE_FEE_ESTIMATOR_CONSTANT
+        blocks_ahead = self.tx_settings.base_fee_estimator_constant
         base_fee_estimate = ceil(to_int(base_fee) * (9 / 8) ** blocks_ahead)
 
         max_fee = to_hex(base_fee_estimate + to_int(max_priority_fee))
         return to_hex(base_fee_estimate), max_priority_fee, max_fee, chain_id
 
+    def get_static_fee(self) -> tuple[str, str]:
+        # non eip-1559 transaction
+        return tuple(self._rpc.fetch_multi([("eth_gasPrice", []), ("eth_chainId", [])]))
+
     def _check_sender(self, address):
         if address is None:
             raise ValueError("No sender!")
-        return to_checksum_address(address)
+        return Address(address)
 
     # OVERRIDES
     def execute_code(
         self,
         to_address,
         sender=None,
         gas=None,
         value=0,
         data=b"",
         override_bytecode=None,
         contract=None,
         is_modifying=True,
+        ir_executor=None,  # maybe just have **kwargs to collect extra kwargs
     ):
         # call execute_code for tracing side effects
+        # note: we could get a perf improvement if we ran this in
+        # the background while waiting on RPC network calls
         computation = super().execute_code(
             to_address=to_address,
             sender=sender,
             gas=gas,
             value=value,
             data=data,
             is_modifying=is_modifying,
             contract=contract,
         )
 
         sender = self._check_sender(self._get_sender(sender))
 
-        data = to_hex(data)
+        hexdata = to_hex(data)
 
         if is_modifying:
             try:
                 receipt, trace = self._send_txn(
-                    from_=sender, to=to_address, value=value, gas=gas, data=data
+                    from_=sender, to=to_address, value=value, gas=gas, data=hexdata
                 )
             except _EstimateGasFailed:
                 # no need to actually run the txn.
                 # caller will decide what to do with the error - probably revert
 
                 # if not computation.is_error, either a bug in boa
                 # or out of sync with node.
@@ -190,21 +250,21 @@
                 # unrecoverable error and bail out
                 if trace.is_error and not computation.is_error:
                     raise RuntimeError(
                         f"panic: local computation succeeded but node didnt: {trace}"
                     )
 
         else:
-            args = _fixup_dict(
+            args = fixup_dict(
                 {
                     "from": sender,
                     "to": to_address,
                     "gas": gas,
                     "value": value,
-                    "data": data,
+                    "data": hexdata,
                 }
             )
             returnvalue = self._rpc.fetch("eth_call", [args, "latest"])
             output = to_bytes(returnvalue)
             # we don't need to do the check for computation.is_error
             # because if the eth_call failed it would have just raised
             # an actual RPC error
@@ -235,116 +295,118 @@
         bytecode = to_hex(bytecode)
         sender = self._check_sender(self._get_sender(sender))
 
         receipt, trace = self._send_txn(
             from_=sender, value=value, gas=gas, data=bytecode
         )
 
-        create_address = to_canonical_address(receipt["contractAddress"])
+        create_address = Address(receipt["contractAddress"])
 
         deployed_bytecode = local_bytecode
 
         if trace is not None and local_bytecode != trace.returndata_bytes:
             # not sure what to do about this, for now just complain
             warnings.warn(
                 "local fork did not match node! this indicates state got out "
                 "of sync with the network or a bug in titanoboa!",
                 stacklevel=2,
             )
-            # return what the node returned anyways.
+            # return what the node returned anyway
             deployed_bytecode = trace.returndata_bytes
 
         if local_address != create_address:
             raise RuntimeError(f"uh oh! {local_address} != {create_address}")
 
         # TODO get contract info in here
-        print(f"contract deployed at {to_checksum_address(create_address)}")
+        print(f"contract deployed at {create_address}")
 
         return create_address, deployed_bytecode
 
-    def _wait_for_tx_trace(self, tx_hash, timeout=60, poll_latency=0.25):
-        start = time.time()
-        while True:
-            receipt = self._rpc.fetch("eth_getTransactionReceipt", [tx_hash])
-            if receipt is not None:
-                break
-            if time.time() + poll_latency > start + timeout:
-                raise ValueError(f"Timed out waiting for ({tx_hash})")
-            time.sleep(poll_latency)
-
-        trace = None
-        if self._tracer is not None:
-            trace = self._rpc.fetch("debug_traceTransaction", [tx_hash, self._tracer])
-        return receipt, trace
-
     @cached_property
     def _tracer(self):
+        def _warn_no_tracer():
+            warnings.warn(
+                "debug_traceTransaction not available! "
+                "titanoboa will try hard to interact with the network, but "
+                "this means that titanoboa is not able to do certain "
+                "safety checks at runtime. it is recommended to switch "
+                "to a node or provider with debug_traceTransaction.",
+                stacklevel=3,
+            )
+
         try:
             txn_hash = "0x" + "00" * 32
             # alchemy only can do callTracer, plus it has lowest
             # overhead.
             call_tracer = {"tracer": "callTracer", "onlyTopCall": True}
             self._rpc.fetch("debug_traceTransaction", [txn_hash, call_tracer])
+
         except RPCError as e:
-            if e.code == -32601:
-                warnings.warn(
-                    "debug_traceTransaction not available! "
-                    "titanoboa will try hard to interact with the network, but "
-                    "this means that titanoboa is not able to do certain "
-                    "safety checks at runtime. it is recommended to switch "
-                    "to a node or provider with debug_traceTransaction.",
-                    stacklevel=2,
-                )
-                return None
             # can't handle callTracer, use default (i.e. structLogs)
             if e.code == -32602:
                 return {}
+
+            # catchall - just don't have a tracer
+            # note on error codes:
+            # -32600 is alchemy unpaid tier error message
+            # -32601 is infura error message (if i recall correctly)
+            _warn_no_tracer()
+            return None
+
+        except HTTPError:
+            _warn_no_tracer()
+            return None
+
         return call_tracer
 
     def _get_nonce(self, addr):
         return self._rpc.fetch("eth_getTransactionCount", [addr, "latest"])
 
     def _reset_fork(self, block_identifier="latest"):
         # use "latest" to make sure we are forking with up-to-date state
         # but use reset_traces=False to help with storage dumps
-        super().fork(
-            self._rpc._rpc_url,
+        self.fork_rpc(
+            self._rpc,
             reset_traces=False,
             block_identifier=block_identifier,
             cache_file=None,
         )
         self.vm.state._account_db._rpc._init_mem_db()
 
     def _send_txn(self, from_, to=None, gas=None, value=None, data=None):
-        tx_data = _fixup_dict(
+        tx_data = fixup_dict(
             {"from": from_, "to": to, "gas": gas, "value": value, "data": data}
         )
 
-        base_fee, max_priority_fee, max_fee, chain_id = self.get_fee_info()
         try:
             # eip-1559 txn
+            (base_fee, max_priority_fee, max_fee, chain_id) = self.get_eip1559_fee()
             tx_data["maxPriorityFeePerGas"] = max_priority_fee
             tx_data["maxFeePerGas"] = max_fee
             tx_data["chainId"] = chain_id
-        except RPCError:
-            tx_data["gasPrice"] = to_hex(self.get_gas_price())
+        except (RPCError, KeyError):
+            gas_price, chain_id = self.get_static_fee()
+            tx_data["gasPrice"] = gas_price
+            tx_data["chainId"] = chain_id
 
         tx_data["nonce"] = self._get_nonce(from_)
 
-        try:
-            tx_data["gas"] = self._rpc.fetch("eth_estimateGas", [tx_data])
-        except RPCError as e:
-            if e.code == 3:
-                # execution failed at estimateGas, probably the txn reverted
-                raise _EstimateGasFailed()
-            raise e from e
+        if gas is None:
+            try:
+                tx_data["gas"] = self._rpc.fetch("eth_estimateGas", [tx_data])
+            except RPCError as e:
+                if e.code == 3:
+                    # execution failed at estimateGas, probably the txn reverted
+                    raise _EstimateGasFailed()
+                raise e from e
 
         if from_ not in self._accounts:
             raise ValueError(f"Account not available: {from_}")
         account = self._accounts[from_]
+
         if hasattr(account, "sign_transaction"):
             signed = account.sign_transaction(tx_data)
 
             # note: signed.rawTransaction has type HexBytes
             tx_hash = self._rpc.fetch(
                 "eth_sendRawTransaction", [to_hex(bytes(signed.rawTransaction))]
             )
@@ -352,15 +414,21 @@
             # some providers (i.e. metamask) don't have sign_transaction
             # we just have to call send_transaction and pray for the best
             tx_hash = account.send_transaction(tx_data)["hash"]
 
         # TODO real logging
         print(f"tx broadcasted: {tx_hash}")
 
-        receipt, trace = self._wait_for_tx_trace(tx_hash)
+        receipt = self._rpc.wait_for_tx_receipt(tx_hash, self.tx_settings.poll_timeout)
+
+        trace = None
+        if self._tracer is not None:
+            trace = self._rpc.fetch_uncached(
+                "debug_traceTransaction", [tx_hash, self._tracer]
+            )
 
         print(f"{tx_hash} mined in block {receipt['blockHash']}!")
 
         # the block was mined, reset state
         self._reset_fork(block_identifier=receipt["blockNumber"])
 
         t_obj = TraceObject(trace) if trace is not None else None
```

### Comparing `titanoboa-0.1.8/boa/precompile.py` & `titanoboa-0.1.9/boa/precompile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from typing import Any
 
-from eth.codecs import abi
 from vyper.ast import parse_to_ast
 from vyper.builtins._signatures import BuiltinFunction
-from vyper.builtins.functions import (
-    DISPATCH_TABLE,
-    STMT_DISPATCH_TABLE,
-    abi_encode,
-    ir_tuple_from_args,
-    process_inputs,
-)
+from vyper.builtins.functions import DISPATCH_TABLE, STMT_DISPATCH_TABLE
+from vyper.builtins.functions import abi_encode as abi_encode_ir
+from vyper.builtins.functions import ir_tuple_from_args, process_inputs
 from vyper.codegen.core import IRnode, needs_external_call_wrap
 from vyper.evm.address_space import MEMORY
 from vyper.semantics.analysis.base import VarInfo
 from vyper.semantics.namespace import get_namespace
 from vyper.semantics.types import TupleT
 from vyper.semantics.types.function import ContractFunctionT
 from vyper.utils import keccak256
 
 from boa.environment import register_raw_precompile
+from boa.util.abi import abi_decode, abi_encode
 
 
 class PrecompileBuiltin(BuiltinFunction):
     def __init__(self, name, args, return_type, address):
         # override BuiltinFunction attributes
         self._id = name
         self._inputs = args  # list[tuple[str, VyperType]]
@@ -40,15 +36,15 @@
         args_as_tuple = ir_tuple_from_args(args)
         args_abi_t = args_as_tuple.typ.abi_type
         args_buf = context.new_internal_variable(args_as_tuple.typ)
 
         ret = ["seq"]
 
         # store abi-encoded argument at buf
-        args_len = abi_encode(
+        args_len = abi_encode_ir(
             args_buf, args_as_tuple, context, args_abi_t.size_bound(), returns_len=True
         )
         ret_len = self._return_type.abi_type.size_bound()
 
         addr = int.from_bytes(self._address, "big")
 
         # call precompile
@@ -67,29 +63,29 @@
         func_t = ContractFunctionT.from_FunctionDef(vy_ast, is_interface=True)
 
         args_t = TupleT(tuple(func_t.argument_types))
 
         def wrapper(computation):
             # Decode input arguments from message data
             msg_data = computation.msg.data_as_bytes
-            arg_values = abi.decode(args_t.abi_type.selector_name(), msg_data)
+            arg_values = abi_decode(args_t.abi_type.selector_name(), msg_data)
 
             # Call the original function with decoded input arguments
             res = func(*arg_values)
 
             return_t = func_t.return_type
             if return_t is not None:
                 # Encode the result to be ABI-compatible
                 # wrap to make it a tuple if necessary
                 if needs_external_call_wrap(return_t):
                     res = (res,)
                     return_t = TupleT((return_t,))
 
                 ret_abi_t = return_t.abi_type.selector_name()
-                computation.output = abi.encode(ret_abi_t, res)
+                computation.output = abi_encode(ret_abi_t, res)
 
                 return computation
 
         address = keccak256(user_signature.encode("utf-8"))[:20]
         register_raw_precompile(address, wrapper, force=force)
 
         args = [(arg.name, arg.typ) for arg in func_t.arguments]
```

### Comparing `titanoboa-0.1.8/boa/profiling.py` & `titanoboa-0.1.9/boa/profiling.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from dataclasses import dataclass
 from functools import cached_property
 from textwrap import dedent
 
 from eth_utils import to_checksum_address
 from rich.table import Table
 
+from boa.contracts.vyper.ast_utils import get_fn_name_from_lineno, get_line
 from boa.environment import Env
-from boa.vyper.ast_utils import get_fn_name_from_lineno, get_line
 
 
 @dataclass(unsafe_hash=True)
 class LineInfo:
     address: str
     contract_name: str
     lineno: int
```

### Comparing `titanoboa-0.1.8/boa/test/plugin.py` & `titanoboa-0.1.9/boa/test/plugin.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/boa/test/strategies.py` & `titanoboa-0.1.9/boa/test/strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import random
 import string
-from typing import Any, Callable, Iterable, Optional, Tuple, Union
+from typing import Any, Callable, Iterable, Optional, Union
 
 from eth_abi.grammar import BasicType, TupleType, parse
 from eth_utils import to_checksum_address
 from hypothesis import given
 from hypothesis import strategies as st
 from hypothesis.strategies import SearchStrategy
 from hypothesis.strategies._internal.deferred import DeferredStrategy
 
-from boa.vyper.contract import VyperFunction
+from boa.contracts.vyper.vyper_contract import VyperFunction
 
 # hypothesis fuzzing strategies, adapted from brownie 0.19.2 (86258c7bd)
 # in the future these may be superseded by eth-stdlib.
 
 TYPE_STR_TRANSLATIONS = {"byte": "bytes1", "decimal": "fixed168x10"}
 
 ArrayLengthType = Union[int, list, None]
 NumberType = Union[float, int, None]
 
 
 # note: there are also utils in the vyper codebase we could use for
 # this. also, in the future we may want to replace these with strategies
 # that use vyper types instead of abi types.
-def get_int_bounds(type_str: str) -> Tuple[int, int]:
+def get_int_bounds(type_str: str) -> tuple[int, int]:
     """Returns the lower and upper bound for an integer type."""
     size = int(type_str.strip("uint") or 256)
     if size < 8 or size > 256 or size % 8:
         raise ValueError(f"Invalid type: {type_str}")
     if type_str.startswith("u"):
         return 0, 2**size - 1
     return -(2 ** (size - 1)), 2 ** (size - 1) - 1
@@ -39,15 +39,15 @@
         self._repr_target = repr_target
 
     def __repr__(self):
         return f"sampled_from({self._repr_target})"
 
 
 def _exclude_filter(fn: Callable) -> Callable:
-    def wrapper(*args: Tuple, exclude: Any = None, **kwargs: int) -> SearchStrategy:
+    def wrapper(*args: tuple, exclude: Any = None, **kwargs: int) -> SearchStrategy:
         strat = fn(*args, **kwargs)
         if exclude is None:
             return strat
         if callable(exclude):
             return strat.filter(exclude)
         if not isinstance(exclude, Iterable) or isinstance(exclude, str):
             exclude = (exclude,)
@@ -58,29 +58,29 @@
         return strat
 
     return wrapper
 
 
 def _check_numeric_bounds(
     type_str: str, min_value: NumberType, max_value: NumberType
-) -> Tuple:
+) -> tuple[NumberType, NumberType]:
     lower, upper = get_int_bounds(type_str)
     min_final = lower if min_value is None else min_value
     max_final = upper if max_value is None else max_value
     if min_final < lower or max_final > upper or min_final > max_final:
         raise ValueError
     return min_final, max_final
 
 
 @_exclude_filter
 def _integer_strategy(
     type_str: str, min_value: Optional[int] = None, max_value: Optional[int] = None
 ) -> SearchStrategy:
-    min_value, max_value = _check_numeric_bounds(type_str, min_value, max_value)
-    return st.integers(min_value=min_value, max_value=max_value)
+    min_val, max_val = _check_numeric_bounds(type_str, min_value, max_value)
+    return st.integers(min_val, max_val)
 
 
 @_exclude_filter
 def _decimal_strategy(
     min_value: NumberType = None, max_value: NumberType = None, places: int = 10
 ) -> SearchStrategy:
     min_value, max_value = _check_numeric_bounds("int128", min_value, max_value)
```

### Comparing `titanoboa-0.1.8/boa/util/disk_cache.py` & `titanoboa-0.1.9/boa/util/disk_cache.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/boa/util/eip5202.py` & `titanoboa-0.1.9/boa/util/eip5202.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/boa/util/exceptions.py` & `titanoboa-0.1.9/boa/util/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 import types
 
 
 # take an exception instance, and strip frames in the target module
 # from the traceback
 def strip_internal_frames(exc, module_name=None):
-    ei = sys.exc_info()
-    frame = ei[2].tb_frame
+    error_type, error, traceback = sys.exc_info()
+    frame = traceback.tb_frame
 
     if module_name is None:
         module_name = frame.f_globals["__name__"]
 
     while frame.f_globals.get("__name__", None) == module_name:
         frame = frame.f_back
 
     # kwargs incompatible with pypy here
     # tb_next=None, tb_frame=frame, tb_lasti=frame.f_lasti, tb_lineno=frame.f_lineno
     tb = types.TracebackType(None, frame, frame.f_lasti, frame.f_lineno)
-    return ei[1].with_traceback(tb)
+    return error.with_traceback(tb)
```

### Comparing `titanoboa-0.1.8/boa/util/leveldb.py` & `titanoboa-0.1.9/boa/util/leveldb.py`

 * *Files identical despite different names*

### Comparing `titanoboa-0.1.8/boa/util/lrudict.py` & `titanoboa-0.1.9/boa/util/lrudict.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,10 +12,12 @@
     def __setitem__(self, k, val):
         if len(self) == self.n:
             del self[next(iter(self))]
         super().__setitem__(k, val)
 
     # set based on a lambda
     def setdefault_lambda(self, k, fn):
-        if k in self:
+        try:
             return self[k]
-        self[k] = fn()
+        except KeyError:
+            self[k] = (ret := fn(k))
+            return ret
```

### Comparing `titanoboa-0.1.8/boa/vm/fork.py` & `titanoboa-0.1.9/boa/vm/fork.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,53 @@
 import os
-from typing import Any
+import sys
+from typing import Any, Type
+
+from requests import HTTPError
 
 try:
     import ujson as json
 except ImportError:
     import json  # type: ignore
 
 import rlp
 from eth.db.account import AccountDB, keccak
 from eth.db.backends.memory import MemoryDB
 from eth.db.cache import CacheDB
+from eth.db.journal import JournalDB
 from eth.rlp.accounts import Account
 from eth.vm.interrupt import MissingBytecode
-from eth_utils import int_to_big_endian, to_checksum_address
+from eth.vm.message import Message
+from eth_utils import int_to_big_endian, to_canonical_address, to_checksum_address
 
-from boa.rpc import EthereumRPC, to_bytes, to_hex, to_int
+from boa.rpc import RPC, RPCError, fixup_dict, to_bytes, to_hex, to_int
 from boa.util.lrudict import lrudict
 
 TIMEOUT = 60  # default timeout for http requests in seconds
 
 
 DEFAULT_CACHE_DIR = "~/.cache/titanoboa/fork.db"
+_PREDEFINED_BLOCKS = {"safe", "latest", "finalized", "pending", "earliest"}
 
 
 _EMPTY = b""  # empty rlp stuff
+_HAS_KEY = b"\x01"  # could be anything
 
 
-class CachingRPC(EthereumRPC):
-    def __init__(self, url: str, cache_file: str = DEFAULT_CACHE_DIR):
-        super().__init__(url)
-
+class CachingRPC(RPC):
+    def __init__(self, rpc: RPC, cache_file: str = DEFAULT_CACHE_DIR):
         # (default to memory db plyvel not found or cache_file is None)
+        self._rpc = rpc
         self._init_mem_db()
         if cache_file is not None:
             try:
                 from boa.util.leveldb import LevelDB
 
+                print("(using leveldb)", file=sys.stderr)
+
                 cache_file = os.path.expanduser(cache_file)
                 # use CacheDB as an additional layer over disk
                 # (ideally would use leveldb lru cache but it's not configurable
                 # via LevelDB API).
                 self._db = CacheDB(LevelDB(cache_file), cache_size=1024 * 1024)  # type: ignore
             except ImportError:
                 # plyvel not found
@@ -49,104 +57,131 @@
     # reduces fork time after the first fork.
     _loaded: dict[tuple[str, str], "CachingRPC"] = {}
     _pid: int = os.getpid()  # so we can detect if our fds are bad
 
     def _init_mem_db(self):
         self._db = MemoryDB(lrudict(1024 * 1024))
 
-    @classmethod
-    def get_rpc(cls, url, cache_file=DEFAULT_CACHE_DIR):
+    @property
+    def identifier(self) -> str:
+        return self._rpc.identifier
+
+    @property
+    def name(self):
+        return self._rpc.name
+
+    def __new__(cls, rpc, cache_file=DEFAULT_CACHE_DIR):
+        if isinstance(rpc, cls):
+            return rpc
+
         if os.getpid() != cls._pid:
             # we are in a fork. reload everything so that fds are not corrupted
             cls._loaded = {}
             cls._pid = os.getpid()
 
-        if (url, cache_file) in cls._loaded:
-            return cls._loaded[(url, cache_file)]
+        if (rpc.identifier, cache_file) in cls._loaded:
+            return cls._loaded[(rpc.identifier, cache_file)]
 
-        ret = cls(url, cache_file)
-        cls._loaded[(url, cache_file)] = ret
+        ret = super().__new__(cls)
+        ret.__init__(rpc, cache_file)
+        cls._loaded[(rpc.identifier, cache_file)] = ret
         return ret
 
     # a stupid key for the kv store
     def _mk_key(self, method: str, params: Any) -> Any:
         return json.dumps({"method": method, "params": params}).encode("utf-8")
 
     def fetch(self, method, params):
         # dispatch into fetch_multi for caching behavior.
         (res,) = self.fetch_multi([(method, params)])
         return res
 
+    def fetch_uncached(self, method, params):
+        return self._rpc.fetch_uncached(method, params)
+
     # caching fetch of multiple payloads
-    # note: overrides super().fetch_multi!
     def fetch_multi(self, payload):
         ret = {}
-        ks = []
+        keys = []
         batch = []
-        for i, (method, params) in enumerate(payload):
-            k = self._mk_key(method, params)
+        for item_ix, (method, params) in enumerate(payload):
+            key = self._mk_key(method, params)
             try:
-                ret[i] = json.loads(self._db[k])
+                ret[item_ix] = json.loads(self._db[key])
             except KeyError:
-                ks.append(k)
-                batch.append((i, method, params))
+                keys.append((key, item_ix))
+                batch.append((method, params))
 
         if len(batch) > 0:
-            res = self._raw_fetch_multi(batch)
-            for i, s in res.items():
-                k = ks[i]
-                ret[i] = s
-                self._db[k] = json.dumps(s).encode("utf-8")
+            # fetch_multi is called only with the missing payloads
+            # map the results back to the original indices
+            for result_ix, rpc_result in enumerate(self._rpc.fetch_multi(batch)):
+                key, item_ix = keys[result_ix]
+                ret[item_ix] = rpc_result
+                self._db[key] = json.dumps(rpc_result).encode("utf-8")
 
         return [ret[i] for i in range(len(ret))]
 
 
 # AccountDB which dispatches to an RPC when we don't have the
 # data locally
 class AccountDBFork(AccountDB):
-    _rpc_init_kwargs: dict[str, Any] = {}
+    @classmethod
+    def class_from_rpc(
+        cls, rpc: RPC, block_identifier: str, **kwargs
+    ) -> Type["AccountDBFork"]:
+        class _ConfiguredAccountDB(AccountDBFork):
+            def __init__(self, *args, **kwargs2):
+                caching_rpc = CachingRPC(rpc, **kwargs)
+                super().__init__(caching_rpc, block_identifier, *args, **kwargs2)
+
+        return _ConfiguredAccountDB
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, rpc: CachingRPC, block_identifier: str, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
-        rpc_kwargs = self._rpc_init_kwargs.copy()
+        self._dontfetch = JournalDB(MemoryDB())
 
-        block_identifier = rpc_kwargs.pop("block_identifier", "safe")
-        self._rpc = CachingRPC.get_rpc(**rpc_kwargs)
+        self._rpc = rpc
 
-        if block_identifier not in ("safe", "latest", "finalized"):
+        if block_identifier not in _PREDEFINED_BLOCKS:
             block_identifier = to_hex(block_identifier)
 
-        # do not cache - use raw_fetch
-        self._block_info = self._rpc._raw_fetch_multi(
-            [(0, "eth_getBlockByNumber", [block_identifier, False])]
-        )[0]
+        self._block_info = self._rpc.fetch_uncached(
+            "eth_getBlockByNumber", [block_identifier, False]
+        )
         self._block_number = to_int(self._block_info["number"])
 
     @property
     def _block_id(self):
         return to_hex(self._block_number)
 
     def _has_account(self, address, from_journal=True):
         return super()._get_encoded_account(address, from_journal) != _EMPTY
 
-    def _get_account(self, address, from_journal=True):
+    def _get_account_helper(self, address, from_journal=True):
         # cf. super impl of _get_account
-        # we need to override this in order so that internal uses of
-        # _set_account() work correctly
-
         if from_journal and address in self._account_cache:
             return self._account_cache[address]
 
         rlp_account = self._get_encoded_account(address, from_journal)
 
         if rlp_account:
-            account = rlp.decode(rlp_account, sedes=Account)
+            return rlp.decode(rlp_account, sedes=Account)
         else:
+            return None
+
+    def _get_account(self, address, from_journal=True):
+        # we need to override this in order so that internal uses of
+        # _set_account() work correctly
+        account = self._get_account_helper(address, from_journal)
+
+        if account is None:
             account = self._get_account_rpc(address)
+
         if from_journal:
             self._account_cache[address] = account
 
         return account
 
     def _get_account_rpc(self, address):
         addr = to_checksum_address(address)
@@ -159,40 +194,118 @@
         balance = to_int(res[0])
         nonce = to_int(res[1])
         code = to_bytes(res[2])
         code_hash = keccak(code)
 
         return Account(nonce=nonce, balance=balance, code_hash=code_hash)
 
+    # try call debug_traceCall to get the ostensible prestate for this call
+    def try_prefetch_state(self, msg: Message):
+        args = fixup_dict(
+            {
+                "from": msg.sender,
+                "to": msg.to,
+                "gas": msg.gas,
+                "value": msg.value,
+                "data": msg.data,
+            }
+        )
+        # TODO: skip debug_traceCall if we have seen these specific
+        # arguments with this specific block before
+        try:
+            tracer = {"tracer": "prestateTracer"}
+            res = self._rpc.fetch_uncached(
+                "debug_traceCall", [args, self._block_id, tracer]
+            )
+        except (RPCError, HTTPError):
+            return
+
+        snapshot = self.record()
+
+        # everything is returned in hex
+        for address, v in res.items():
+            try:
+                address = to_canonical_address(address)
+            except ValueError:
+                # the trace we have been given is invalid, roll back changes
+                self.discard(snapshot)
+                return
+
+            # set account if we don't already have it
+            if self._get_account_helper(address) is None:
+                balance = to_int(v.get("balance", "0x"))
+                code = to_bytes(v.get("code", "0x"))
+                nonce = v.get("nonce", 0)  # already an int
+                self._set_account(address, Account(nonce=nonce, balance=balance))
+                self.set_code(address, code)
+
+            storage = v.get("storage", dict())
+
+            account_store = super()._get_address_store(address)
+            for hexslot, hexvalue in storage.items():
+                slot = to_int(hexslot)
+                value = to_int(hexvalue)
+                # set storage if we don't already have it.
+                # see AccountStorageDB.get()
+                # note we explicitly write 0s, so that they appear
+                # in the journal later when called by get_storage
+                key = int_to_big_endian(slot)
+                if not self._helper_have_storage(address, slot):
+                    account_store._journal_storage[key] = rlp.encode(value)  # type: ignore
+        self.lock_changes()
+
     def get_code(self, address):
         try:
             return super().get_code(address)
         except MissingBytecode:  # will get thrown if code_hash != hash(empty)
             ret = self._rpc.fetch(
                 "eth_getCode", [to_checksum_address(address), self._block_id]
             )
             return to_bytes(ret)
 
-    def get_storage(self, address, slot, from_journal=True):
-        # call super to get address warming semantics
-        s = super().get_storage(address, slot, from_journal)
+    def discard(self, checkpoint):
+        super().discard(checkpoint)
+        self._dontfetch.discard(checkpoint)
+
+    def commit(self, checkpoint):
+        super().commit(checkpoint)
+        self._dontfetch.commit(checkpoint)
+
+    def record(self):
+        checkpoint = super().record()
+        self._dontfetch.record(checkpoint)
+        return checkpoint
+
+    # helper to determine if something is in the storage db
+    # or we need to get from RPC
+    def _helper_have_storage(self, address, slot, from_journal=True):
+        if not from_journal:
+            db = super()._get_address_store(address)._locked_changes
+            key = int_to_big_endian(slot)
+            return db.get(key, _EMPTY) != _EMPTY
 
-        # cf. AccountStorageDB.get()
-        store = super()._get_address_store(address)
-        key = int_to_big_endian(slot)
-        db = store._journal_storage if from_journal else store._locked_changes
-        try:
-            if db[key] != _EMPTY:
-                return s
-        except KeyError:
-            # (it was deleted in the journal.)
-            return s
+        key = self._get_storage_tracker_key(address, slot)
+        return self._dontfetch.get(key) == _HAS_KEY
+
+    def get_storage(self, address, slot, from_journal=True):
+        # call super for address warming semantics
+        val = super().get_storage(address, slot, from_journal)
+        if self._helper_have_storage(address, slot, from_journal=from_journal):
+            return val
 
         addr = to_checksum_address(address)
-        ret = self._rpc.fetch("eth_getStorageAt", [addr, to_hex(slot), self._block_id])
-        return to_int(ret)
+        raw_val = self._rpc.fetch(
+            "eth_getStorageAt", [addr, to_hex(slot), self._block_id]
+        )
+        return to_int(raw_val)
+
+    def set_storage(self, address, slot, value):
+        super().set_storage(address, slot, value)
+        # mark don't fetch
+        key = self._get_storage_tracker_key(address, slot)
+        self._dontfetch[key] = _HAS_KEY
 
     def account_exists(self, address):
         if super().account_exists(address):
             return True
 
         return self.get_balance(address) > 0 or self.get_nonce(address) > 0
```

### Comparing `titanoboa-0.1.8/boa/vm/gas_meters.py` & `titanoboa-0.1.9/boa/vm/gas_meters.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     """
     A trivial gas meter, which does not meter gas usage.
     Improves EVM runtime performance by about 10%.
     Useful if you don't care about gas usage but want a
     performance boost.
     """
 
-    def __init__(self, start_gas):
+    def __init__(self, start_gas, *args, **kwargs):
         pass
 
     def consume_gas(self, amount, reason):
         pass
 
     def refund_gas(self, amount):
         pass
```

### Comparing `titanoboa-0.1.8/boa/vyper/ast_utils.py` & `titanoboa-0.1.9/boa/contracts/vyper/ast_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import re
 import tokenize
-from typing import Any, Optional, Tuple
+from typing import Any, Optional
 
 import vyper.ast as vy_ast
 from vyper.codegen.core import getpos
 
 
 def get_block(source_code: str, lineno: int, end_lineno: int) -> str:
     source_lines = source_code.splitlines(keepends=True)
@@ -32,15 +32,15 @@
     return None
 
 
 # extract the dev revert reason at a given line.
 # somewhat heuristic.
 def reason_at(
     source_code: str, lineno: int, end_lineno: int
-) -> Optional[Tuple[str, str]]:
+) -> Optional[tuple[str, str]]:
     block = get_block(source_code, lineno, end_lineno)
     c = _get_comment(block)
     if c is not None:
         return _extract_reason(c)
     return None
```

### Comparing `titanoboa-0.1.8/boa/vyper/contract.py` & `titanoboa-0.1.9/boa/contracts/vyper/vyper_contract.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,48 +10,63 @@
 from typing import Any, Optional
 
 import vyper
 import vyper.ast as vy_ast
 import vyper.ir.compile_ir as compile_ir
 import vyper.semantics.analysis as analysis
 import vyper.semantics.namespace as vy_ns
-from eth.codecs import abi
 from eth.exceptions import VMError
-from eth_typing import Address
-from eth_utils import to_canonical_address, to_checksum_address
 from vyper.ast.utils import parse_to_ast
-from vyper.codegen.core import calculate_type_for_external_return
+from vyper.codegen.core import anchor_opt_level, calculate_type_for_external_return
 from vyper.codegen.function_definitions import generate_ir_for_function
 from vyper.codegen.function_definitions.common import ExternalFuncIR, InternalFuncIR
 from vyper.codegen.global_context import GlobalContext
 from vyper.codegen.ir_node import IRnode
 from vyper.codegen.module import generate_ir_for_module
+from vyper.compiler import CompilerData
 from vyper.compiler import output as compiler_output
+from vyper.compiler.output import build_abi_output
 from vyper.compiler.settings import OptimizationLevel
+from vyper.evm.opcodes import anchor_evm_version
 from vyper.exceptions import VyperException
 from vyper.ir.optimizer import optimize
 from vyper.semantics.analysis.data_positions import set_data_positions
-from vyper.semantics.types import AddressT, EventT, HashMapT, TupleT
-from vyper.semantics.types.function import ContractFunctionT
+from vyper.semantics.types import AddressT, HashMapT, TupleT
 from vyper.utils import method_id
 
-from boa.environment import AddressType, Env, to_int
-from boa.profiling import LineProfile, cache_gas_used_for_computation
-from boa.util.exceptions import strip_internal_frames
-from boa.util.lrudict import lrudict
-from boa.vm.gas_meters import ProfilingGasMeter
-from boa.vyper import _METHOD_ID_VAR
-from boa.vyper.ast_utils import ast_map_of, get_fn_ancestor_from_node, reason_at
-from boa.vyper.compiler_utils import (
-    _compile_vyper_function,
+from boa import BoaError
+from boa.contracts.base_evm_contract import (
+    StackTrace,
+    _BaseEVMContract,
+    _handle_child_trace,
+)
+from boa.contracts.vyper.ast_utils import (
+    ast_map_of,
+    get_fn_ancestor_from_node,
+    reason_at,
+)
+from boa.contracts.vyper.compiler_utils import (
+    _METHOD_ID_VAR,
+    anchor_compiler_settings,
+    compile_vyper_function,
     generate_bytecode_for_arbitrary_stmt,
     generate_bytecode_for_internal_fn,
 )
-from boa.vyper.decoder_utils import ByteAddressableStorage, decode_vyper_object
-from boa.vyper.event import Event, RawEvent
+from boa.contracts.vyper.decoder_utils import (
+    ByteAddressableStorage,
+    decode_vyper_object,
+)
+from boa.contracts.vyper.event import Event, RawEvent
+from boa.contracts.vyper.ir_executor import executor_from_ir
+from boa.environment import Env
+from boa.profiling import LineProfile, cache_gas_used_for_computation
+from boa.util.abi import Address, abi_decode, abi_encode
+from boa.util.lrudict import lrudict
+from boa.vm.gas_meters import ProfilingGasMeter
+from boa.vm.utils import to_bytes, to_int
 
 # error messages for external calls
 EXTERNAL_CALL_ERRORS = ("external call failed", "returndatasize too small")
 
 CREATE_ERRORS = ("create failed", "create2 failed")
 
 # error detail where user possibly provided dev revert reason
@@ -60,15 +75,16 @@
 
 class VyperDeployer:
     def __init__(self, compiler_data, filename=None):
         self.compiler_data = compiler_data
 
         # force compilation so that if there are any errors in the contract,
         # we fail at load rather than at deploy time.
-        _ = compiler_data.bytecode
+        with anchor_compiler_settings(self.compiler_data):
+            _ = compiler_data.bytecode, compiler_data.bytecode_runtime
 
         self.filename = filename
 
     def __call__(self, *args, **kwargs):
         return self.deploy(*args, **kwargs)
 
     def deploy(self, *args, **kwargs):
@@ -77,50 +93,70 @@
         )
 
     def deploy_as_blueprint(self, *args, **kwargs):
         return VyperBlueprint(
             self.compiler_data, *args, filename=self.filename, **kwargs
         )
 
+    def stomp(self, address: Any, data_section=None) -> "VyperContract":
+        address = Address(address)
+
+        ret = self.deploy(override_address=address, skip_initcode=True)
+        vm = ret.env.vm
+        old_bytecode = vm.state.get_code(address.canonical_address)
+        new_bytecode = self.compiler_data.bytecode_runtime
+
+        immutables_size = self.compiler_data.global_ctx.immutable_section_bytes
+        if immutables_size > 0:
+            data_section = old_bytecode[-immutables_size:]
+            new_bytecode += data_section
+
+        vm.state.set_code(address.canonical_address, new_bytecode)
+        ret.env.register_contract(address, ret)
+        ret._set_bytecode(new_bytecode)
+        return ret
+
     # TODO: allow `env=` kwargs and so on
-    def at(self, address: AddressType) -> "VyperContract":
-        address = to_checksum_address(address)
-        ret = VyperContract(
-            self.compiler_data,
-            override_address=address,
-            skip_initcode=True,
-            filename=self.filename,
-        )
+    def at(self, address: Any) -> "VyperContract":
+        address = Address(address)
+
+        ret = self.deploy(override_address=address, skip_initcode=True)
         vm = ret.env.vm
-        bytecode = vm.state.get_code(to_canonical_address(address))
+        bytecode = vm.state.get_code(address.canonical_address)
 
         ret._set_bytecode(bytecode)
 
         ret.env.register_contract(address, ret)
 
         return ret
 
 
 # a few lines of shared code between VyperBlueprint and VyperContract
-class _BaseContract:
-    def __init__(self, compiler_data, env=None, filename=None):
+class _BaseVyperContract(_BaseEVMContract):
+    def __init__(
+        self,
+        compiler_data: CompilerData,
+        env: Optional[Env] = None,
+        filename: Optional[str] = None,
+    ):
+        super().__init__(env, filename)
         self.compiler_data = compiler_data
 
-        if env is None:
-            env = Env.get_singleton()
-
-        self.env = env
+        with anchor_compiler_settings(self.compiler_data):
+            _ = compiler_data.bytecode, compiler_data.bytecode_runtime
 
-        self.filename = filename
+    @cached_property
+    def abi(self):
+        return build_abi_output(self.compiler_data)
 
 
 # create a blueprint for use with `create_from_blueprint`.
 # uses a ERC5202 preamble, when calling `create_from_blueprint` will
 # need to use `code_offset=3`
-class VyperBlueprint(_BaseContract):
+class VyperBlueprint(_BaseVyperContract):
     def __init__(
         self,
         compiler_data,
         env=None,
         override_address=None,
         blueprint_preamble=b"\xFE\x71\x00",
         filename=None,
@@ -140,15 +176,15 @@
 
         deploy_bytecode += blueprint_bytecode
 
         addr, self.bytecode = self.env.deploy_code(
             bytecode=deploy_bytecode, override_address=override_address
         )
 
-        self.address = to_checksum_address(addr)
+        self._address = Address(addr)
 
         self.env.register_blueprint(compiler_data.bytecode, self)
 
     @cached_property
     def deployer(self):
         return VyperDeployer(self.compiler_data, filename=self.filename)
 
@@ -181,108 +217,71 @@
     def __str__(self):
         return f"<{self.reason_type}: {self.reason_str}>"
 
 
 @dataclass
 class ErrorDetail:
     vm_error: VMError
-    contract: "VyperContract"
+    contract_repr: str  # string representation of the contract for the error
     error_detail: str  # compiler provided error detail
     dev_reason: DevReason
     frame_detail: FrameDetail
-    storage_detail: Optional[FrameDetail]
     ast_source: vy_ast.VyperNode
 
     @classmethod
     def from_computation(cls, contract, computation):
-        error_detail = contract.find_error_meta(computation.code)
-        ast_source = contract.find_source_of(computation.code)
+        error_detail = contract.find_error_meta(computation)
+        ast_source = contract.find_source_of(computation)
         reason = None
         if ast_source is not None:
             reason = DevReason.at_source_location(
                 contract.compiler_data.source_code,
                 ast_source.lineno,
                 ast_source.end_lineno,
             )
         frame_detail = contract.debug_frame(computation)
-        storage_detail = contract._storage.dump()
 
+        contract_repr = computation._contract_repr_before_revert or repr(contract)
         return cls(
             vm_error=computation.error,
-            contract=contract,
+            contract_repr=contract_repr,
             error_detail=error_detail,
             dev_reason=reason,
             frame_detail=frame_detail,
-            storage_detail=storage_detail,
             ast_source=ast_source,
         )
 
     @property
     def pretty_vm_reason(self):
         err = self.vm_error
         # decode error msg if it's "Error(string)"
         # b"\x08\xc3y\xa0" == method_id("Error(string)")
         if isinstance(err.args[0], bytes) and err.args[0][:4] == b"\x08\xc3y\xa0":
-            return abi.decode("(string)", err.args[0][4:])[0]
+            return abi_decode("(string)", err.args[0][4:])[0]
 
         return repr(err)
 
     def __str__(self):
-        msg = f"{self.contract}\n"
+        msg = f"{self.contract_repr}\n"
 
         if self.error_detail is not None:
             msg += f" <compiler: {self.error_detail}>"
 
         if self.ast_source is not None:
             # VyperException.__str__ does a lot of formatting for us
             msg = str(VyperException(msg, self.ast_source))
 
         if self.frame_detail is not None:
             self.frame_detail.fn_name = "locals"  # override the displayed name
             if len(self.frame_detail) > 0:
                 msg += f" {self.frame_detail}"
 
-        if self.storage_detail is not None:
-            self.storage_detail.fn_name = "storage"  # override displayed name
-            if len(self.storage_detail) > 0:
-                msg += f"\n {self.storage_detail}"
-
         return msg
 
 
-class StackTrace(list):
-    def __str__(self):
-        return "\n\n".join(str(x) for x in self)
-
-    @property
-    def last_frame(self):
-        return self[-1]
-
-
-def trace_for_unknown_contract(computation, env):
-    ret = StackTrace(
-        [f"<Unknown location in unknown contract {computation.msg.code_address.hex()}>"]
-    )
-    return _handle_child_trace(computation, env, ret)
-
-
-def _handle_child_trace(computation, env, return_trace):
-    if len(computation.children) == 0:
-        return return_trace
-    if not computation.children[-1].is_error:
-        return return_trace
-    child = computation.children[-1]
-    child_obj = env.lookup_contract(child.msg.code_address)
-    if child_obj is None:
-        child_trace = trace_for_unknown_contract(child, env)
-    else:
-        child_trace = child_obj.stack_trace(child)
-    return StackTrace(child_trace + return_trace)
-
-
 # "pattern match" a BoaError. tries to match fields of the error
 # to the args/kwargs provided. raises if no match
 def check_boa_error_matches(error, *args, **kwargs):
     assert isinstance(error, BoaError)
 
     def _check(cond, msg=""):
         if not cond:
@@ -293,16 +292,16 @@
         assert len(args) == 1, "multiple args!"
         assert len(kwargs) == 0, "can't mix args and kwargs!"
         err = args[0]
         # try to match anything
         _check(
             err == frame.pretty_vm_reason
             or err == frame.error_detail
-            or err == frame.dev_reason.reason_str,
-            "does not match {args}",
+            or (frame.dev_reason and err == frame.dev_reason.reason_str),
+            f"does not match {args}",
         )
         return
 
     # try to match a specific kwarg
     assert len(kwargs) == 1 and len(args) == 0
 
     # don't accept magic
@@ -312,15 +311,15 @@
     k, v = next(iter(kwargs.items()))
     if k == "compiler":
         _check(v == frame.error_detail, f"{frame.error_detail} != {v}")
     elif k == "vm_error":
         _check(
             frame.error_detail == "user revert with reason"
             and v == frame.pretty_vm_reason,
-            f"{frame.vm_error} != {v}",
+            f"{frame.pretty_vm_reason} != {v}",
         )
     # assume it is a dev reason string
     else:
         assert_ast_types = (vy_ast.Assert, vy_ast.Raise)
         if frame.ast_source.get_ancestor(assert_ast_types) is not None:
             # if it's a dev reason on an assert statement, check that
             # we are actually handling the user assertion and not some other
@@ -339,16 +338,17 @@
 
 # using sha3 preimages, take a storage key and undo
 # hashes to get the sequence of hashes ("path") that gave us this image.
 def unwrap_storage_key(sha3_db, k):
     path = []
 
     def unwrap(k):
-        if k in sha3_db:
-            preimage = sha3_db[k]
+        k_bytes = to_bytes(k)
+        if k_bytes in sha3_db:
+            preimage = sha3_db[k_bytes]
             slot, k = preimage[:32], preimage[32:]
 
             unwrap(slot)
 
         path.append(k)
 
     unwrap(k)
@@ -362,15 +362,15 @@
         else:
             lens = lens.setdefault(k, {})
 
 
 class StorageVar:
     def __init__(self, contract, slot, typ):
         self.contract = contract
-        self.addr = to_canonical_address(self.contract.address)
+        self.addr = self.contract._address.canonical_address
         self.accountdb = contract.env.vm.state._account_db
         self.slot = slot
         self.typ = typ
 
     def _decode(self, slot, typ, truncate_limit=None):
         n = typ.memory_bytes_required
         if truncate_limit is not None and n > truncate_limit:
@@ -384,29 +384,29 @@
             return self.contract.env.lookup_alias(maybe_address)
         except KeyError:  # not found, return the input
             return maybe_address
 
     def get(self, truncate_limit=None):
         if isinstance(self.typ, HashMapT):
             ret = {}
-            for k in self.contract.env.sstore_trace.get(self.contract.address, {}):
+            for k in self.contract.env.sstore_trace.get(self.addr, {}):
                 path = unwrap_storage_key(self.contract.env.sha3_trace, k)
                 if to_int(path[0]) != self.slot:
                     continue
 
                 path = path[1:]  # drop the slot
                 path_t = []
 
                 ty = self.typ
                 for i, p in enumerate(path):
                     path[i] = decode_vyper_object(memoryview(p), ty.key_type)
                     path_t.append(ty.key_type)
                     ty = ty.value_type
 
-                val = self._decode(to_int(k), ty, truncate_limit)
+                val = self._decode(k, ty, truncate_limit)
 
                 # set val only if value is nonzero
                 if val:
                     # decode aliases as needed/possible
                     dealiased_path = []
                     for p, t in zip(path, path_t):
                         if isinstance(t, AddressT):
@@ -457,25 +457,25 @@
     def dump(self):
         return FrameDetail("immutables", vars(self))
 
     def __repr__(self):
         return repr(self.dump())
 
 
-class VyperContract(_BaseContract):
+class VyperContract(_BaseVyperContract):
     def __init__(
         self,
-        compiler_data,
+        compiler_data: CompilerData,
         *args,
-        env=None,
-        override_address=None,
-        # whether or not to skip constructor
+        env: Env = None,
+        override_address: Address = None,
+        # whether to skip constructor
         skip_initcode=False,
-        created_from=None,
-        filename=None,
+        created_from: Address = None,
+        filename: str = None,
     ):
         super().__init__(compiler_data, env, filename)
 
         self.created_from = created_from
 
         # add all exposed functions from the interface to the contract
         external_fns = {
@@ -486,17 +486,18 @@
 
         # set external methods as class attributes:
         self._ctor = None
         if "__init__" in external_fns:
             self._ctor = VyperFunction(external_fns.pop("__init__"), self)
 
         if skip_initcode:
-            self.address = to_checksum_address(override_address)
+            addr = Address(override_address)
         else:
-            self.address = self._run_init(*args, override_address=override_address)
+            addr = self._run_init(*args, override_address=override_address)
+        self._address = addr
 
         for fn_name, fn in external_fns.items():
             setattr(self, fn_name, VyperFunction(fn, self))
 
         # set internal methods as class.internal attributes:
         self.internal = lambda: None
         for fn in self.global_ctx.functions:
@@ -506,26 +507,26 @@
 
         self._storage = StorageModel(self)
 
         self._eval_cache = lrudict(0x1000)
         self._source_map = None
         self._computation = None
 
-        self.env.register_contract(self.address, self)
+        self.env.register_contract(self._address, self)
 
     def _run_init(self, *args, override_address=None):
         encoded_args = b""
         if self._ctor:
             encoded_args = self._ctor.prepare_calldata(*args)
 
         initcode = self.compiler_data.bytecode + encoded_args
         addr, self.bytecode = self.env.deploy_code(
             bytecode=initcode, override_address=override_address
         )
-        return to_checksum_address(addr)
+        return Address(addr)
 
     # manually set the runtime bytecode, instead of using deploy
     def _set_bytecode(self, bytecode: bytes) -> None:
         to_check = bytecode
         if self.data_section_size != 0:
             to_check = bytecode[: -self.data_section_size]
         if to_check != self.compiler_data.bytecode_runtime:
@@ -533,15 +534,15 @@
                 f"casted bytecode does not match compiled bytecode at {self}",
                 stacklevel=2,
             )
         self.bytecode = bytecode
 
     def __repr__(self):
         ret = (
-            f"<{self.compiler_data.contract_name} at {to_checksum_address(self.address)}, "
+            f"<{self.compiler_data.contract_name} at {self.address}, "
             f"compiled with vyper-{vyper.__version__}+{vyper.__commit__}>"
         )
 
         if self.created_from is not None:
             ret += f" (created by {self.created_from})"
 
         dump_storage = True  # maybe make this configurable in the future
@@ -565,15 +566,15 @@
         return self.deployer.at(address)
 
     @cached_property
     def ast_map(self):
         return ast_map_of(self.compiler_data.vyper_module)
 
     def _get_fn_from_computation(self, computation):
-        node = self.find_source_of(computation.code)
+        node = self.find_source_of(computation)
         return get_fn_ancestor_from_node(node)
 
     def debug_frame(self, computation=None):
         if computation is None:
             computation = self._computation
 
         fn = self._get_fn_from_computation(computation)
@@ -600,27 +601,38 @@
     @property
     def global_ctx(self):
         return self.compiler_data.global_ctx
 
     @property
     def source_map(self):
         if self._source_map is None:
-            _, self._source_map = compile_ir.assembly_to_evm(
-                self.compiler_data.assembly_runtime
-            )
+            with anchor_compiler_settings(self.compiler_data):
+                _, self._source_map = compile_ir.assembly_to_evm(
+                    self.compiler_data.assembly_runtime
+                )
         return self._source_map
 
-    def find_error_meta(self, code_stream):
+    def find_error_meta(self, computation):
+        if hasattr(computation, "vyper_error_msg"):
+            # this is set by ir executor currently.
+            return computation.vyper_error_msg
+
+        code_stream = computation.code
         error_map = self.source_map.get("error_map", {})
         for pc in reversed(code_stream._trace):
             if pc in error_map:
                 return error_map[pc]
         return None
 
-    def find_source_of(self, code_stream, is_initcode=False):
+    def find_source_of(self, computation, is_initcode=False):
+        if hasattr(computation, "vyper_source_pos"):
+            # this is set by ir executor currently.
+            return self.ast_map.get(computation.vyper_source_pos)
+
+        code_stream = computation.code
         pc_map = self.source_map["pc_pos_map"]
         for pc in reversed(code_stream._trace):
             if pc in pc_map and pc_map[pc] in self.ast_map:
                 return self.ast_map[pc_map[pc]]
         return None
 
     # ## handling events
@@ -657,15 +669,15 @@
     @cached_property
     def event_for(self):
         m = self.compiler_data.vyper_module_folded._metadata["type"]
         return {e.event_id: e for e in m.events.values()}
 
     def decode_log(self, e):
         log_id, address, topics, data = e
-        assert to_canonical_address(self.address) == address
+        assert self._address.canonical_address == address
         event_hash = topics[0]
         event_t = self.event_for[event_hash]
 
         topic_typs = []
         arg_typs = []
         for is_topic, typ in zip(event_t.indexed, event_t.arguments.values()):
             if not is_topic:
@@ -674,22 +686,22 @@
                 topic_typs.append(typ)
 
         decoded_topics = []
         for typ, t in zip(topic_typs, topics[1:]):
             # convert to bytes for abi decoder
             encoded_topic = t.to_bytes(32, "big")
             decoded_topics.append(
-                abi.decode(typ.abi_type.selector_name(), encoded_topic)
+                abi_decode(typ.abi_type.selector_name(), encoded_topic)
             )
 
         tuple_typ = TupleT(arg_typs)
 
-        args = abi.decode(tuple_typ.abi_type.selector_name(), data)
+        args = abi_decode(tuple_typ.abi_type.selector_name(), data)
 
-        return Event(log_id, self.address, event_t, decoded_topics, args)
+        return Event(log_id, self._address, event_t, decoded_topics, args)
 
     def marshal_to_python(self, computation, vyper_typ):
         self._computation = computation  # for further inspection
 
         if computation.is_error:
             self.handle_error(computation)
 
@@ -698,34 +710,26 @@
         if gas_meter == ProfilingGasMeter:
             cache_gas_used_for_computation(self, computation)
 
         if vyper_typ is None:
             return None
 
         return_typ = calculate_type_for_external_return(vyper_typ)
-        ret = abi.decode(return_typ.abi_type.selector_name(), computation.output)
+        ret = abi_decode(return_typ.abi_type.selector_name(), computation.output)
 
         # unwrap the tuple if needed
         if not isinstance(vyper_typ, TupleT):
             (ret,) = ret
 
         return vyper_object(ret, vyper_typ)
 
-    def handle_error(self, computation):
-        try:
-            raise BoaError(self.stack_trace(computation))
-        except BoaError as b:
-            # modify the error so the traceback starts in userland.
-            # inspired by answers in https://stackoverflow.com/q/1603940/
-            raise strip_internal_frames(b) from None
-
     def stack_trace(self, computation=None):
         computation = computation or self._computation
         ret = StackTrace([ErrorDetail.from_computation(self, computation)])
-        error_detail = self.find_error_meta(computation.code)
+        error_detail = self.find_error_meta(computation)
         if error_detail not in EXTERNAL_CALL_ERRORS + CREATE_ERRORS:
             return ret
         return _handle_child_trace(computation, self.env, ret)
 
     def line_profile(self, computation=None):
         computation = computation or self._computation
         ret = LineProfile.from_single(self, computation)
@@ -737,32 +741,35 @@
         return ret
 
     @cached_property
     def _ast_module(self):
         module = copy.deepcopy(self.compiler_data.vyper_module)
 
         # do the same thing as vyper_module_folded but skip getter expansion
-        vy_ast.folding.fold(module)
-        with vy_ns.get_namespace().enter_scope():
-            analysis.add_module_namespace(module, self.compiler_data.interface_codes)
-            analysis.validate_functions(module)
-            # we need to cache the namespace right here(!).
-            # set_data_positions will modify the type definitions in place.
-            self._cache_namespace(vy_ns.get_namespace())
-
-        vy_ast.expansion.remove_unused_statements(module)
-        # calculate slots for all storage variables, tagging
-        # the types in the namespace.
-        set_data_positions(module, storage_layout_overrides=None)
-
-        # ensure _ir_info is generated for all functions in this copied/shadow
-        # namespace
-        _ = generate_ir_for_module(GlobalContext(module))
+        with anchor_compiler_settings(self.compiler_data):
+            vy_ast.folding.fold(module)
+            with vy_ns.get_namespace().enter_scope():
+                analysis.add_module_namespace(
+                    module, self.compiler_data.interface_codes
+                )
+                analysis.validate_functions(module)
+                # we need to cache the namespace right here(!).
+                # set_data_positions will modify the type definitions in place.
+                self._cache_namespace(vy_ns.get_namespace())
+
+            vy_ast.expansion.remove_unused_statements(module)
+            # calculate slots for all storage variables, tagging
+            # the types in the namespace.
+            set_data_positions(module, storage_layout_overrides=None)
+
+            # ensure _ir_info is generated for all functions in this copied/shadow
+            # namespace
+            _ = generate_ir_for_module(GlobalContext(module))
 
-        return module
+            return module
 
     # the global namespace is expensive to compute, so cache it
     def _cache_namespace(self, namespace):
         # copy.copy doesn't really work on Namespace objects, copy by hand
         ret = vy_ns.Namespace()
         ret._scopes = copy.deepcopy(namespace._scopes)
         for s in namespace._scopes:
@@ -770,26 +777,35 @@
                 ret[n] = namespace[n]
         self._vyper_namespace = ret
 
     @contextlib.contextmanager
     def override_vyper_namespace(self):
         # ensure self._vyper_namespace is computed
         m = self._ast_module  # noqa: F841
+        contract_members = self._vyper_namespace["self"].typ.members
         try:
+            to_keep = set(contract_members.keys())
             with vy_ns.override_global_namespace(self._vyper_namespace):
                 yield
         finally:
-            self._vyper_namespace["self"].typ.members.pop("__boa_debug__", None)
+            # drop all keys which were added while yielding
+            keys = list(contract_members.keys())
+            for k in keys:
+                if k not in to_keep:
+                    contract_members.pop(k)
 
     # for eval(), we need unoptimized assembly, since the dead code
     # eliminator might prune a dead function (which we want to eval)
     @cached_property
     def unoptimized_assembly(self):
-        runtime = self.compiler_data.ir_runtime
-        return compile_ir.compile_to_assembly(runtime, optimize=OptimizationLevel.NONE)
+        with anchor_evm_version(self.compiler_data.settings.evm_version):
+            runtime = self.unoptimized_ir[1]
+            return compile_ir.compile_to_assembly(
+                runtime, optimize=OptimizationLevel.NONE
+            )
 
     @cached_property
     def data_section_size(self):
         return self.global_ctx.immutable_section_bytes
 
     @cached_property
     def data_section(self):
@@ -797,18 +813,32 @@
         if self.data_section_size:
             return self.bytecode[-self.data_section_size :]
         else:
             return b""
 
     @cached_property
     def unoptimized_bytecode(self):
-        s, _ = compile_ir.assembly_to_evm(
-            self.unoptimized_assembly, insert_vyper_signature=True
-        )
-        return s + self.data_section
+        with anchor_evm_version(self.compiler_data.settings.evm_version):
+            s, _ = compile_ir.assembly_to_evm(
+                self.unoptimized_assembly, insert_vyper_signature=True
+            )
+            return s + self.data_section
+
+    @cached_property
+    def unoptimized_ir(self):
+        with anchor_opt_level(OptimizationLevel.NONE), anchor_evm_version(
+            self.compiler_data.settings.evm_version
+        ):
+            return generate_ir_for_module(self.compiler_data.global_ctx)
+
+    @cached_property
+    def ir_executor(self):
+        _, ir_runtime = self.unoptimized_ir
+        with anchor_evm_version(self.compiler_data.settings.evm_version):
+            return executor_from_ir(ir_runtime, self.compiler_data)
 
     @contextlib.contextmanager
     def _anchor_source_map(self, source_map):
         tmp = self._source_map
         try:
             self._source_map = source_map
             yield
@@ -821,35 +851,32 @@
         value: int = 0,
         gas: Optional[int] = None,
         sender: Optional[Address] = None,
     ) -> Any:
         """eval vyper code in the context of this contract"""
 
         # this method is super slow so we cache compilation results
-        if stmt in self._eval_cache:
-            bytecode, source_map, typ = self._eval_cache[stmt]
-        else:
-            bytecode, source_map, typ = generate_bytecode_for_arbitrary_stmt(stmt, self)
-            self._eval_cache[stmt] = (bytecode, source_map, typ)
+        if stmt not in self._eval_cache:
+            self._eval_cache[stmt] = generate_bytecode_for_arbitrary_stmt(stmt, self)
+        _, ir_executor, bytecode, source_map, typ = self._eval_cache[stmt]
 
         with self._anchor_source_map(source_map):
             method_id = b"dbug"  # note dummy method id, doesn't get validated
             c = self.env.execute_code(
-                to_address=self.address,
+                to_address=self._address,
                 sender=sender,
                 data=method_id,
                 value=value,
                 gas=gas,
                 contract=self,
                 override_bytecode=bytecode,
+                ir_executor=ir_executor,
             )
 
-            ret = self.marshal_to_python(c, typ)
-
-            return ret
+            return self.marshal_to_python(c, typ)
 
     # inject a function into this VyperContract without affecting the
     # contract's source code. useful for testing private functionality
     def inject_function(self, fn_source_code, force=False):
         if not hasattr(self, "inject"):
             self.inject = lambda: None
 
@@ -864,32 +891,40 @@
         self._vyper_namespace["self"].typ.members.pop(fn_ast.name, None)
         f = _InjectVyperFunction(self, fn_source_code)
         setattr(self.inject, fn_ast.name, f)
 
 
 class VyperFunction:
     def __init__(self, fn_ast, contract):
+        super().__init__()
         self.fn_ast = fn_ast
         self.contract = contract
         self.env = contract.env
 
+        self.__doc__ = (
+            fn_ast.doc_string.value if hasattr(fn_ast, "doc_string") else None
+        )
+        self.__module__ = self.contract.compiler_data.contract_name
+
     def __repr__(self):
         return f"{self.contract.compiler_data.contract_name}.{self.fn_ast.name}"
 
+    def __str__(self):
+        return repr(self.func_t)
+
     @cached_property
     def _source_map(self):
         return self.contract.source_map
 
     @property
     def func_t(self):
         return self.fn_ast._metadata["type"]
 
     @cached_property
     def ir(self):
-        # patch compiler_data to have IR for every function
         global_ctx = self.contract.global_ctx
 
         res = generate_ir_for_function(self.fn_ast, global_ctx, False)
         if isinstance(res, InternalFuncIR):
             ir = res.func_ir
         elif isinstance(res, ExternalFuncIR):
             ir = res.common_ir
@@ -912,24 +947,26 @@
         bytecode, _ = compile_ir.assembly_to_evm(self.assembly)
         return bytecode
 
     # hotspot, cache the signature computation
     def args_abi_type(self, num_kwargs):
         if not hasattr(self, "_signature_cache"):
             self._signature_cache = {}
+
         if num_kwargs in self._signature_cache:
             return self._signature_cache[num_kwargs]
 
         # align the kwargs with the signature
         sig_kwargs = self.func_t.keyword_args[:num_kwargs]
         sig_args = self.func_t.positional_args + sig_kwargs
         args_abi_type = (
             "(" + ",".join(arg.typ.abi_type.selector_name() for arg in sig_args) + ")"
         )
         abi_sig = self.func_t.name + args_abi_type
+
         _method_id = method_id(abi_sig)
         self._signature_cache[num_kwargs] = (_method_id, args_abi_type)
 
         return _method_id, args_abi_type
 
     def prepare_calldata(self, *args, **kwargs):
         n_total_args = self.func_t.n_total_args
@@ -944,40 +981,47 @@
                 f"({expectation_str}, got {len(args)})"
             )
 
         # align the kwargs with the signature
         # sig_kwargs = self.func_t.default_args[: len(kwargs)]
 
         total_non_base_args = len(kwargs) + len(args) - n_pos_args
-        # allow things with `.address` to be encode-able
+
         args = [getattr(arg, "address", arg) for arg in args]
 
         method_id, args_abi_type = self.args_abi_type(total_non_base_args)
-        encoded_args = abi.encode(args_abi_type, args)
+        encoded_args = abi_encode(args_abi_type, args)
 
         if self.func_t.is_constructor or self.func_t.is_fallback:
             return encoded_args
 
         return method_id + encoded_args
 
     def __call__(self, *args, value=0, gas=None, sender=None, **kwargs):
         calldata_bytes = self.prepare_calldata(*args, **kwargs)
+
         # getattr(x, attr, None) swallows exceptions. use explicit hasattr+getattr
+        ir_executor = None
+        if hasattr(self, "_ir_executor"):
+            ir_executor = self._ir_executor
+
         override_bytecode = None
-        if hasattr(self, "override_bytecode"):
-            override_bytecode = self.override_bytecode
+        if hasattr(self, "_override_bytecode"):
+            override_bytecode = self._override_bytecode
+
         with self.contract._anchor_source_map(self._source_map):
             computation = self.env.execute_code(
-                to_address=self.contract.address,
+                to_address=self.contract._address,
                 sender=sender,
                 data=calldata_bytes,
                 value=value,
                 gas=gas,
                 is_modifying=self.func_t.is_mutable,
                 override_bytecode=override_bytecode,
+                ir_executor=ir_executor,
                 contract=self.contract,
             )
 
             typ = self.func_t.return_type
             return self.contract.marshal_to_python(computation, typ)
 
 
@@ -990,187 +1034,52 @@
 
     @cached_property
     def _compiled(self):
         return generate_bytecode_for_internal_fn(self)
 
     # OVERRIDE so that __call__ uses the specially crafted bytecode
     @cached_property
-    def override_bytecode(self):
-        bytecode, _, _ = self._compiled
+    def _override_bytecode(self):
+        _, _, bytecode, _, _ = self._compiled
         return bytecode
 
-    # OVERRIDE so that __call__ uses corresponding source map
-    @cached_property
-    def _source_map(self):
-        _, source_map, _ = self._compiled
-        return source_map
-
-
-# a contract which we only have the ABI for.
-# TODO refactor:
-# right now inherits functionality from VyperContract
-# but would be better to put this in like BaseContract
-# and have both BaseContract => InterfaceContract
-# and separately BaseContract => VyperContract
-class ABIContract(VyperContract):
-    def __init__(self, name, functions, events, address, created_from=None, env=None):
-        if env is None:
-            env = Env.get_singleton()
-        self.env = env
-
-        self._name = name
-        self._events = events
-        self._functions = functions
-
-        for func_t in self._functions:
-            setattr(self, func_t.name, ABIFunction(func_t, self))
-
-        self.address = to_checksum_address(address)
-        self.created_from = created_from
-
-        self._source_map = {"pc_pos_map": {}}  # override
-
-    @cached_property
-    def method_id_map(self):
-        ret = {}
-        for func_t in self._functions:
-            for abi_sig, method_id_int in func_t.method_ids.items():
-                method_id_bytes = method_id_int.to_bytes(4, "big")
-                assert method_id_bytes not in ret  # vyper guarantees unique method ids
-                ret[method_id_bytes] = abi_sig
-        return ret
-
-    def stack_trace(self, computation=None):
-        computation = computation or self._computation
-        calldata_method_id = bytes(computation.msg.data[:4])
-        abi_sig = self.method_id_map[calldata_method_id]
-        ret = StackTrace([f"  (unknown location in {self}.{abi_sig})"])
-        return _handle_child_trace(computation, self.env, ret)
-
-    @property
-    def deployer(self):
-        return ABIContractFactory(self._name, self._functions, self._events)
-
-    def __repr__(self):
-        ret = f"<{self._name} interface at {to_checksum_address(self.address)}>"
-
-        if self.created_from is not None:
-            ret += f" (created by {self.created_from})"
-
-        return ret
-
-    # OVERRIDE
     @cached_property
-    def event_for(self):
-        return {e.event_id: e for e in self._events}
-
-
-# name Factory instead of Deployer because it doesn't actually do any
-# contract deployment.
-class ABIContractFactory:
-    def __init__(self, name, functions, events):
-        self._name = name
-        self._functions = functions
-        self._events = events
-
-    @classmethod
-    def from_abi_dict(cls, abi, name=None):
-        if name is None:
-            name = "<anonymous contract>"
-
-        functions = [
-            ContractFunctionT.from_abi(i) for i in abi if i.get("type") == "function"
-        ]
-
-        # warn on functions with same name
-        _tmp = set()
-        for f in functions:
-            if f.name in _tmp:
-                warnings.warn(
-                    f"{name} overloads {f.name}! overloaded methods "
-                    "might not work correctly at this time",
-                    stacklevel=1,
-                )
-            _tmp.add(f.name)
-
-        events = [EventT.from_abi(i) for i in abi if i.get("type") == "event"]
-
-        return cls(name, functions, events)
-
-    def at(self, address) -> ABIContract:
-        address = to_checksum_address(address)
-
-        ret = ABIContract(self._name, self._functions, self._events, address)
-
-        bytecode = ret.env.vm.state.get_code(to_canonical_address(address))
-        if bytecode == b"":
-            warnings.warn(
-                "requested {ret} but there is no bytecode at that address!",
-                stacklevel=2,
-            )
-
-        ret.env.register_contract(address, ret)
-
-        return ret
-
-
-class ABIFunction(VyperFunction):
-    def __init__(self, func_t, contract):
-        self.contract = contract
-        self.env = contract.env
-        self._func_t = func_t
-
-    def __repr__(self):
-        return f"{self.contract._name}.{self._func_t.name}"
+    def _ir_executor(self):
+        _, ir_executor, _, _, _ = self._compiled
+        return ir_executor
 
-    # OVERRIDE
-    @property
-    def func_t(self):
-        return self._func_t
-
-    # OVERRIDE
+    # OVERRIDE so that __call__ uses corresponding source map
     @cached_property
     def _source_map(self):
-        return {"pc_pos_map": {}}
+        _, _, _, source_map, _ = self._compiled
+        return source_map
 
 
 class _InjectVyperFunction(VyperFunction):
     def __init__(self, contract, fn_source):
-        ast, bytecode, source_map, _ = _compile_vyper_function(fn_source, contract)
+        ast, ir_executor, bytecode, source_map, _ = compile_vyper_function(
+            fn_source, contract
+        )
         super().__init__(ast, contract)
 
-        self.override_bytecode = bytecode
-
-        # OVERRIDE so that __call__ uses special source map
+        # OVERRIDES so that __call__ does the right thing
+        self._override_bytecode = bytecode
+        self._ir_executor = ir_executor
         self._source_map = source_map
 
 
-@dataclass
-class BoaError(Exception):
-    stack_trace: StackTrace
-
-    # perf TODO: don't materialize the stack trace until we need it,
-    # i.e. BoaError ctor only takes what is necessary to construct the
-    # stack trace but does not require the actual stack trace itself.
-    def __str__(self):
-        frame = self.stack_trace.last_frame
-        err = frame.vm_error
-        err.args = (frame.pretty_vm_reason, *err.args[1:])
-        return f"{err}\n\n{self.stack_trace}"
-
-
 _typ_cache = {}
 
 
 def vyper_object(val, vyper_type):
     # make a thin wrapper around whatever type val is,
     # and tag it with _vyper_type metadata
 
     vt = type(val)
-    if vt is bool:
+    if vt is bool or vt is Address:
         # https://stackoverflow.com/q/2172189
         # bool is not ambiguous wrt vyper type anyways.
         return val
 
     if vt not in _typ_cache:
         # ex. class int_wrapper(int): pass
         _typ_cache[vt] = type(f"{vt.__name__}_wrapper", (vt,), {})
```

### Comparing `titanoboa-0.1.8/boa/vyper/decoder_utils.py` & `titanoboa-0.1.9/boa/contracts/vyper/decoder_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,21 +10,15 @@
     SArrayT,
     StringT,
     StructT,
     TupleT,
 )
 from vyper.utils import unsigned_to_signed
 
-
-def ceil32(n):
-    return floor32(n + 31)
-
-
-def floor32(n):
-    return n & ~31
+from boa.vm.utils import ceil32, floor32
 
 
 # wrap storage in something which looks like memory
 class ByteAddressableStorage:
     def __init__(self, db, address, key):
         self.db = db
         self.address = address
@@ -36,58 +30,69 @@
             start = subscript.start or 0
             stop = subscript.stop
             i = self.key + start // 32
             while i < self.key + ceil32(stop) // 32:
                 ret += self.db.get_storage(self.address, i).to_bytes(32, "big")
                 i += 1
 
-            start -= floor32(start)
-            stop -= floor32(start)
+            start_ofst = floor32(start)
+            start -= start_ofst
+            stop -= start_ofst
             return memoryview(ret[start:stop])
         else:
             raise Exception("Must slice {self}")
 
 
 class _Struct(dict):
     def __init__(self, name, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.struct_name = name
 
     def __repr__(self):
         return f"{self.struct_name}({super().__repr__()})"
 
 
+def _get_length(mem, bound):
+    ret = int.from_bytes(mem[:32], "big")
+    if ret > bound:
+        # perf -- this is an uninitialized variable; length and data are
+        # both garbage. truncate length to the bound of the container of
+        # this type. the data will still be garbage, but we avoid OOM.
+        return bound
+    return ret
+
+
 def decode_vyper_object(mem, typ):
     if isinstance(typ, BytesM_T):
         # TODO tag return value like `vyper_object` does
         return mem[: typ.m_bits].tobytes()
     if isinstance(typ, (AddressT, InterfaceT)):
         return to_checksum_address(mem[12:32].tobytes())
     if isinstance(typ, BoolT):
         return bool.from_bytes(mem[31:32], "big")
     if isinstance(typ, IntegerT):
         ret = int.from_bytes(mem[:32], "big")
         if typ.is_signed:
             return unsigned_to_signed(ret, 256)
         return ret
     if isinstance(typ, BytesT):
-        length = int.from_bytes(mem[:32], "big")
+        length = _get_length(mem[:32], typ.length)
         return mem[32 : 32 + length].tobytes()
     if isinstance(typ, StringT):
-        length = int.from_bytes(mem[:32], "big")
+        length = _get_length(mem[:32], typ.length)
         return mem[32 : 32 + length].tobytes().decode("utf-8")
     if isinstance(typ, SArrayT):
         length = typ.count
         n = typ.subtype.memory_bytes_required
         return [
             decode_vyper_object(mem[i * n : i * n + n], typ.subtype)
             for i in range(length)
         ]
     if isinstance(typ, DArrayT):
-        length = int.from_bytes(mem[:32], "big")
+        length = _get_length(mem[:32], typ.length)
         n = typ.subtype.memory_bytes_required
         ofst = 32
         ret = []
         for _ in range(length):
             ret.append(decode_vyper_object(mem[ofst : ofst + n], typ.subtype))
             ofst += n
         return ret
```

### Comparing `titanoboa-0.1.8/boa/vyper/event.py` & `titanoboa-0.1.9/boa/contracts/vyper/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass
-from typing import Any, List
+from typing import Any
 
 
 @dataclass
 class Event:
     log_id: int  # internal py-evm log id, for ordering purposes
     address: str  # checksum address
     event_type: Any  # vyper.semantics.types.user.EventT
-    topics: List[Any]  # list of decoded topics
-    args: List[Any]  # list of decoded args
+    topics: list[Any]  # list of decoded topics
+    args: list[Any]  # list of decoded args
 
     def __repr__(self):
         t_i = 0
         a_i = 0
         b = []
         # align the evm topic + args lists with the way they appear in the source
         # ex. Transfer(indexed address, address, indexed address)
```

### Comparing `titanoboa-0.1.8/pyproject.toml` & `titanoboa-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "titanoboa"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Vyper interpreter"
 #authors = []
 license = { file = "LICENSE" }
 readme = "README.md"
 #homepage = "https://github.com/vyperlang/titanoboa"
 #repository = "https://github.com/vyperlang/titanoboa"
 #documentation =
@@ -12,20 +12,26 @@
 keywords = ["ethereum", "evm", "smart contract", "development"]
 
 classifiers = ["Topic :: Software Development"]
 
 # Requirements
 dependencies = [
     "vyper >= 0.3.10",
-    "eth-stdlib",
+    "eth-stdlib>=0.2.7,<0.3.0",
     "eth-abi",
     "py-evm>=0.7.0a4",
     "eth-typing",
     "hypothesis",
     "pytest",
+    "pytest-cov",
+
+    # eth-rlp requirement, not installed by default with 3.12
+    "typing-extensions",
+
+    # gas profiling tables
     "rich",
 
     # required for forking:
     "requests",
 
     # required for networked accounts
     "eth-account",
@@ -37,11 +43,18 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [tool.setuptools.packages.find]
 include = ["boa*"]
 
 [tool.pytest.ini_options]
-markers = ["ignore_isolation: Do not preserve state during tests"]
+markers = [
+    "ignore_isolation: Do not preserve state during tests",
+    "gas_profile: Enable gas profiling.",
+    "ignore_profiling: Disable gas profiling.",
+]
+
+[tool.setuptools.package-data]
+boa = ["integrations/**/*.js"]
 
 #[dev-dependencies]
 #black = { version = "^18.3-alpha.0", python = "^3.6" }
```

### Comparing `titanoboa-0.1.8/titanoboa.egg-info/PKG-INFO` & `titanoboa-0.1.9/titanoboa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titanoboa
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Vyper interpreter
 License: Copyright 2022 Charles Cooper
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
@@ -13,20 +13,22 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Keywords: ethereum,evm,smart contract,development
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vyper>=0.3.10
-Requires-Dist: eth-stdlib
+Requires-Dist: eth-stdlib<0.3.0,>=0.2.7
 Requires-Dist: eth-abi
 Requires-Dist: py-evm>=0.7.0a4
 Requires-Dist: eth-typing
 Requires-Dist: hypothesis
 Requires-Dist: pytest
+Requires-Dist: pytest-cov
+Requires-Dist: typing-extensions
 Requires-Dist: rich
 Requires-Dist: requests
 Requires-Dist: eth-account
 Provides-Extra: forking-recommended
 Requires-Dist: ujson; extra == "forking-recommended"
 
 # Titanoboa
```

