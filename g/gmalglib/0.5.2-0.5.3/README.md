# Comparing `tmp/gmalglib-0.5.2.tar.gz` & `tmp/gmalglib-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.5.2.tar", last modified: Sun Apr 14 11:50:49 2024, max compression
+gzip compressed data, was "gmalglib-0.5.3.tar", last modified: Tue Apr 23 13:15:57 2024, max compression
```

## Comparing `gmalglib-0.5.2.tar` & `gmalglib-0.5.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.051865 gmalglib-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 11:50:40.000000 gmalglib-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-14 11:50:49.047865 gmalglib-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-14 11:50:40.000000 gmalglib-0.5.2/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-14 11:50:40.000000 gmalglib-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.043865 gmalglib-0.5.2/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.043865 gmalglib-0.5.2/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-14 11:50:40.000000 gmalglib-0.5.2/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-14 11:50:40.000000 gmalglib-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:50:49.051865 gmalglib-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-14 11:50:40.000000 gmalglib-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.043865 gmalglib-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.047865 gmalglib-0.5.2/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.047865 gmalglib-0.5.2/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    36380 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 11:50:40.000000 gmalglib-0.5.2/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:50:49.047865 gmalglib-0.5.2/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 11:50:49.000000 gmalglib-0.5.2/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 13:15:51.000000 gmalglib-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-23 13:15:57.218980 gmalglib-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 13:15:51.000000 gmalglib-0.5.3/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-23 13:15:51.000000 gmalglib-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.214980 gmalglib-0.5.3/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.214980 gmalglib-0.5.3/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-23 13:15:51.000000 gmalglib-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:15:57.218980 gmalglib-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 13:15:51.000000 gmalglib-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.214980 gmalglib-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36380 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.5.2/LICENSE` & `gmalglib-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/PKG-INFO` & `gmalglib-0.5.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -23,32 +23,18 @@
 
 Python extension library for GM (GuoMi) cryptographic algorithms, providing a set of fundamental cryptographic algorithms.
 
 Implemented in C language, encapsulated based on the native CPython interface, without dependencies on any third-party libraries.
 
 ## Installation
 
-### Windows
-
-For `python3.8` and higher versions, you can directly install using `pip`.
-
 ```bash
 pip install gmalglib
 ```
 
-Alternatively, refer to the source code installation for other platforms.
-
-### Other Platforms
-
-Visit the PyPI project file list [Download files](https://pypi.org/project/gmalglib/#files) page to download the source distribution package `gmalglib-x.y.z.tar.gz`, then proceed with the source code installation.
-
-```bash
-pip install gmalglib-x.y.z.tar.gz
-```
-
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
```

### Comparing `gmalglib-0.5.2/README.en.md` & `gmalglib-0.5.3/README.en.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,18 @@
 
 Python extension library for GM (GuoMi) cryptographic algorithms, providing a set of fundamental cryptographic algorithms.
 
 Implemented in C language, encapsulated based on the native CPython interface, without dependencies on any third-party libraries.
 
 ## Installation
 
-### Windows
-
-For `python3.8` and higher versions, you can directly install using `pip`.
-
 ```bash
 pip install gmalglib
 ```
 
-Alternatively, refer to the source code installation for other platforms.
-
-### Other Platforms
-
-Visit the PyPI project file list [Download files](https://pypi.org/project/gmalglib/#files) page to download the source distribution package `gmalglib-x.y.z.tar.gz`, then proceed with the source code installation.
-
-```bash
-pip install gmalglib-x.y.z.tar.gz
-```
-
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
```

### Comparing `gmalglib-0.5.2/README.md` & `gmalglib-0.5.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,32 +6,18 @@
 
 国密算法的 Python 扩展库, 提供一些原始基础算法.
 
 使用 C 语言实现, 基于原生 CPython 接口进行封装, 不依赖其他任何第三方库.
 
 ## 安装
 
-### Windows
-
-对于 `python3.8` 及以上, 可以直接使用 `pip` 进行安装.
-
 ```bash
 pip install gmalglib
 ```
 
-或者参考其他平台使用源码安装.
-
-### 其他平台
-
-前往 PyPI 项目文件列表 [Download files](https://pypi.org/project/gmalglib/#files) 页面下载源码发布包 `gmalglib-x.y.z.tar.gz`, 之后使用源码安装.
-
-```bash
-pip install gmalglib-x.y.z.tar.gz
-```
-
 ## 已实现的核心算法
 
 - SM3 密码杂凑算法
     - 消息摘要
     - 密钥派生
     - 消息认证
 - SM4 分组密码算法
```

### Comparing `gmalglib-0.5.2/include/gmalglib/bignum.h` & `gmalglib-0.5.3/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/include/gmalglib/random.h` & `gmalglib-0.5.3/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/include/gmalglib/sm2.h` & `gmalglib-0.5.3/include/gmalglib/sm2.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/include/gmalglib/sm2curve.h` & `gmalglib-0.5.3/include/gmalglib/sm2curve.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/include/gmalglib/sm3.h` & `gmalglib-0.5.3/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/pyproject.toml` & `gmalglib-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/setup.py` & `gmalglib-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/core/bignum.c` & `gmalglib-0.5.3/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/core/random.c` & `gmalglib-0.5.3/src/gmalglib/core/random.c`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,16 @@
     while (bytes_len > 0)
     {
         chunk = (size_t)(bytes_len < SIZE_MAX ? bytes_len : SIZE_MAX);
         do {
             n = read(fd, bytes, chunk);
         } while (n < 0 && errno == EINTR);
 
-        if (n <= 0) {
+        if (n <= 0) 
+        {
             close(fd);
             return 0;
         }
 
         bytes += n;
         bytes_len -= n;
     }
```

### Comparing `gmalglib-0.5.2/src/gmalglib/core/sm2.c` & `gmalglib-0.5.3/src/gmalglib/core/sm2.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.3/src/gmalglib/core/sm2curve.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/core/sm3.c` & `gmalglib-0.5.3/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/core/sm4.c` & `gmalglib-0.5.3/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/core/zuc.c` & `gmalglib-0.5.3/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/coremodule.c` & `gmalglib-0.5.3/src/gmalglib/coremodule.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/sm2.pyi` & `gmalglib-0.5.3/src/gmalglib/sm2.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/sm3.pyi` & `gmalglib-0.5.3/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/wrapped.py` & `gmalglib-0.5.3/src/gmalglib/wrapped.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib/zuc.pyi` & `gmalglib-0.5.3/src/gmalglib/zuc.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.2/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.5.3/src/gmalglib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.2
+Version: 0.5.3
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -23,32 +23,18 @@
 
 Python extension library for GM (GuoMi) cryptographic algorithms, providing a set of fundamental cryptographic algorithms.
 
 Implemented in C language, encapsulated based on the native CPython interface, without dependencies on any third-party libraries.
 
 ## Installation
 
-### Windows
-
-For `python3.8` and higher versions, you can directly install using `pip`.
-
 ```bash
 pip install gmalglib
 ```
 
-Alternatively, refer to the source code installation for other platforms.
-
-### Other Platforms
-
-Visit the PyPI project file list [Download files](https://pypi.org/project/gmalglib/#files) page to download the source distribution package `gmalglib-x.y.z.tar.gz`, then proceed with the source code installation.
-
-```bash
-pip install gmalglib-x.y.z.tar.gz
-```
-
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
```

### Comparing `gmalglib-0.5.2/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.3/src/gmalglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

