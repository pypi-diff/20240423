# Comparing `tmp/gep3-0.2.tar.gz` & `tmp/gep3-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gep3-0.2.tar", last modified: Fri Aug 18 00:55:27 2023, max compression
+gzip compressed data, was "gep3-0.3.tar", last modified: Tue Apr 23 19:59:48 2024, max compression
```

## Comparing `gep3-0.2.tar` & `gep3-0.3.tar`

### file list

```diff
@@ -1,49 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.812388 gep3-0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-08-18 00:55:17.000000 gep3-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-08-18 00:55:27.812388 gep3-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-08-18 00:55:17.000000 gep3-0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-08-18 00:55:17.000000 gep3-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-08-18 00:55:27.816388 gep3-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.804387 gep3-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.808388 gep3-0.2/src/ccid/
--rw-r--r--   0 runner    (1001) docker     (122)      490 2023-08-18 00:55:17.000000 gep3-0.2/src/ccid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2300 2023-08-18 00:55:17.000000 gep3-0.2/src/ccid/bulk_in_messages.py
--rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-08-18 00:55:17.000000 gep3-0.2/src/ccid/bulk_message.py
--rw-r--r--   0 runner    (1001) docker     (122)     2410 2023-08-18 00:55:17.000000 gep3-0.2/src/ccid/bulk_out_messages.py
--rw-r--r--   0 runner    (1001) docker     (122)     8379 2023-08-18 00:55:17.000000 gep3-0.2/src/ccid/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.808388 gep3-0.2/src/common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:17.000000 gep3-0.2/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6724 2023-08-18 00:55:17.000000 gep3-0.2/src/common/ber.py
--rw-r--r--   0 runner    (1001) docker     (122)     1327 2023-08-18 00:55:17.000000 gep3-0.2/src/common/bitstr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3954 2023-08-18 00:55:17.000000 gep3-0.2/src/common/hstr.py
--rw-r--r--   0 runner    (1001) docker     (122)      755 2023-08-18 00:55:17.000000 gep3-0.2/src/common/intlist.py
--rw-r--r--   0 runner    (1001) docker     (122)     1168 2023-08-18 00:55:17.000000 gep3-0.2/src/common/str.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.808388 gep3-0.2/src/crypto/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:17.000000 gep3-0.2/src/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21863 2023-08-18 00:55:17.000000 gep3-0.2/src/crypto/des.py
--rw-r--r--   0 runner    (1001) docker     (122)     1193 2023-08-18 00:55:17.000000 gep3-0.2/src/crypto/modes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.808388 gep3-0.2/src/emv/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-08-18 00:55:17.000000 gep3-0.2/src/emv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2909 2023-08-18 00:55:17.000000 gep3-0.2/src/emv/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    12423 2023-08-18 00:55:17.000000 gep3-0.2/src/emv/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1149 2023-08-18 00:55:17.000000 gep3-0.2/src/emv/dsc.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-08-18 00:55:17.000000 gep3-0.2/src/emv/key_management.py
--rw-r--r--   0 runner    (1001) docker     (122)     1614 2023-08-18 00:55:17.000000 gep3-0.2/src/emv/records.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.812388 gep3-0.2/src/gep3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-08-18 00:55:27.000000 gep3-0.2/src/gep3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-08-18 00:55:27.000000 gep3-0.2/src/gep3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-18 00:55:27.000000 gep3-0.2/src/gep3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-08-18 00:55:27.000000 gep3-0.2/src/gep3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.812388 gep3-0.2/src/globalplatform/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-08-18 00:55:17.000000 gep3-0.2/src/globalplatform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3335 2023-08-18 00:55:17.000000 gep3-0.2/src/globalplatform/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     6323 2023-08-18 00:55:17.000000 gep3-0.2/src/globalplatform/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.812388 gep3-0.2/src/iso7816/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-08-18 00:55:17.000000 gep3-0.2/src/iso7816/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20583 2023-08-18 00:55:17.000000 gep3-0.2/src/iso7816/apdu.py
--rw-r--r--   0 runner    (1001) docker     (122)     2120 2023-08-18 00:55:17.000000 gep3-0.2/src/iso7816/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     3734 2023-08-18 00:55:17.000000 gep3-0.2/src/iso7816/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-18 00:55:27.812388 gep3-0.2/src/multos/
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-08-18 00:55:17.000000 gep3-0.2/src/multos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2023-08-18 00:55:17.000000 gep3-0.2/src/multos/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-08-18 00:55:17.000000 gep3-0.2/src/multos/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 19:59:45.000000 gep3-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-23 19:59:48.195155 gep3-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 19:59:45.000000 gep3-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 19:59:45.000000 gep3-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 19:59:48.195155 gep3-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.187155 gep3-0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/ccid/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/bulk_in_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/bulk_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/bulk_out_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-23 19:59:45.000000 gep3-0.3/src/common/ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-23 19:59:45.000000 gep3-0.3/src/common/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-23 19:59:45.000000 gep3-0.3/src/common/bitstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-23 19:59:45.000000 gep3-0.3/src/common/hstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 19:59:45.000000 gep3-0.3/src/common/intlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-23 19:59:45.000000 gep3-0.3/src/common/parserc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 19:59:45.000000 gep3-0.3/src/common/str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-04-23 19:59:45.000000 gep3-0.3/src/crypto/des.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-23 19:59:45.000000 gep3-0.3/src/crypto/modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/emv/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/key_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/emv_key_derivation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/evc_cvc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/evc_dcvv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/gep3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/globalplatform/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 19:59:45.000000 gep3-0.3/src/globalplatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-23 19:59:45.000000 gep3-0.3/src/globalplatform/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-23 19:59:45.000000 gep3-0.3/src/globalplatform/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/iso7816/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20583 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/apdu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/multos/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 19:59:45.000000 gep3-0.3/src/multos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 19:59:45.000000 gep3-0.3/src/multos/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-23 19:59:45.000000 gep3-0.3/src/multos/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-23 19:59:45.000000 gep3-0.3/src/tests/test_common_ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 19:59:45.000000 gep3-0.3/src/tests/test_crypto_des.py
```

### Comparing `gep3-0.2/LICENSE` & `gep3-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gep3-0.2/PKG-INFO` & `gep3-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.2
+Version: 0.3
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Smart Card
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: parsec==3
 
 # gep3
 Generic Encryption Peripheral: various utilities related to cryptography and smart cards
```

### Comparing `gep3-0.2/setup.cfg` & `gep3-0.3/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gep3
-version = 0.2
+version = 0.3
 author = Sebastien Pochic
 author_email = spochic@gmail.com
 description = Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spochic/gep3
 project_urls = 
@@ -17,15 +17,16 @@
 	Topic :: Security :: Cryptography
 	Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Smart Card
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.10
+python_requires = >=3.11
+install_requires = parsec==3
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gep3-0.2/src/ccid/bulk_in_messages.py` & `gep3-0.3/src/ccid/bulk_in_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/ccid/bulk_message.py` & `gep3-0.3/src/ccid/bulk_message.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/ccid/bulk_out_messages.py` & `gep3-0.3/src/ccid/bulk_out_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/ccid/descriptors.py` & `gep3-0.3/src/ccid/descriptors.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/common/bitstr.py` & `gep3-0.3/src/common/bitstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/common/hstr.py` & `gep3-0.3/src/common/hstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/common/intlist.py` & `gep3-0.3/src/common/intlist.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/common/str.py` & `gep3-0.3/src/common/str.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,41 +5,43 @@
 
 # Standard library imports
 
 # Third party imports
 
 # Local application imports
 
-def perm(str_in, permutation):
+
+def perm(str_in: str, permutation: list[int]) -> str:
     """perm():
     """
     str_out = ''
 
     for i in permutation:
         str_out += str_in[i-1]
 
     return str_out
 
 
-def exp(str_in, expansion):
+def exp(str_in: str, expansion: list[int]) -> str:
     """exp():
     """
     return perm(str_in, expansion)
 
 
-def lcs(str_in, shift):
+def lcs(str_in: str, shift: int) -> str:
     """lcs():
     """
     return str_in[shift:] + str_in[:shift]
 
 
-def to_ascii(str_in):
+def to_ascii(str_in: str) -> str:
     return ''.join([F"{ord(c):02X}" for c in str_in])
 
-def clean (str_in: str, keep_char = '', remove_char = '', command_name='()', str_name='') -> str:
+
+def clean(str_in: str, keep_char='', remove_char='', command_name='()', str_name='') -> str:
     """clean(str)
 
     - Removes '_' characters
     - Raises exceptions on illegal characters
     """
     str_out = ''
     for nibble in str_in:
@@ -50,8 +52,8 @@
         else:
             if str_name == '':
                 raise TypeError(F"{command_name}: Unknown nibble: {nibble}")
             else:
                 raise TypeError(
                     F"{command_name}: Unknown nibble in {str_name}: {nibble}")
 
-    return str_out
+    return str_out
```

### Comparing `gep3-0.2/src/emv/commands.py` & `gep3-0.3/src/emv/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/emv/data.py` & `gep3-0.3/src/emv/data.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/emv/records.py` & `gep3-0.3/src/emv/records.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/gep3.egg-info/PKG-INFO` & `gep3-0.3/src/gep3.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.2
+Version: 0.3
 Summary: Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 Home-page: https://github.com/spochic/gep3
 Author: Sebastien Pochic
 Author-email: spochic@gmail.com
 Project-URL: Bug Tracker, https://github.com/spochic/gep3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Smart Card
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: parsec==3
 
 # gep3
 Generic Encryption Peripheral: various utilities related to cryptography and smart cards
```

### Comparing `gep3-0.2/src/gep3.egg-info/SOURCES.txt` & `gep3-0.3/src/gep3.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -5,34 +5,44 @@
 src/ccid/__init__.py
 src/ccid/bulk_in_messages.py
 src/ccid/bulk_message.py
 src/ccid/bulk_out_messages.py
 src/ccid/descriptors.py
 src/common/__init__.py
 src/common/ber.py
+src/common/binary.py
 src/common/bitstr.py
 src/common/hstr.py
 src/common/intlist.py
+src/common/parserc.py
 src/common/str.py
 src/crypto/__init__.py
 src/crypto/des.py
 src/crypto/modes.py
 src/emv/__init__.py
 src/emv/commands.py
 src/emv/data.py
 src/emv/dsc.py
 src/emv/key_management.py
 src/emv/records.py
+src/examples/__init__.py
+src/examples/emv_key_derivation.py
+src/examples/evc_cvc3.py
+src/examples/evc_dcvv.py
 src/gep3.egg-info/PKG-INFO
 src/gep3.egg-info/SOURCES.txt
 src/gep3.egg-info/dependency_links.txt
+src/gep3.egg-info/requires.txt
 src/gep3.egg-info/top_level.txt
 src/globalplatform/__init__.py
 src/globalplatform/commands.py
 src/globalplatform/encodings.py
 src/iso7816/__init__.py
 src/iso7816/apdu.py
 src/iso7816/commands.py
 src/iso7816/encodings.py
 src/multos/__init__.py
 src/multos/commands.py
-src/multos/encodings.py
+src/multos/encodings.py
+src/tests/__init__.py
+src/tests/test_common_ber.py
+src/tests/test_crypto_des.py
```

### Comparing `gep3-0.2/src/globalplatform/commands.py` & `gep3-0.3/src/globalplatform/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/globalplatform/encodings.py` & `gep3-0.3/src/globalplatform/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/iso7816/apdu.py` & `gep3-0.3/src/iso7816/apdu.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/iso7816/commands.py` & `gep3-0.3/src/iso7816/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/iso7816/encodings.py` & `gep3-0.3/src/iso7816/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/multos/commands.py` & `gep3-0.3/src/multos/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.2/src/multos/encodings.py` & `gep3-0.3/src/multos/encodings.py`

 * *Files identical despite different names*

