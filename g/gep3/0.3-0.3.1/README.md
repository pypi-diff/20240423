# Comparing `tmp/gep3-0.3.tar.gz` & `tmp/gep3-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gep3-0.3.tar", last modified: Tue Apr 23 19:59:48 2024, max compression
+gzip compressed data, was "gep3-0.3.1.tar", last modified: Tue Apr 23 20:35:32 2024, max compression
```

## Comparing `gep3-0.3.tar` & `gep3-0.3.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 19:59:45.000000 gep3-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-23 19:59:48.195155 gep3-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 19:59:45.000000 gep3-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 19:59:45.000000 gep3-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 19:59:48.195155 gep3-0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.187155 gep3-0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/ccid/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/bulk_in_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/bulk_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/bulk_out_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-23 19:59:45.000000 gep3-0.3/src/ccid/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-23 19:59:45.000000 gep3-0.3/src/common/ber.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-23 19:59:45.000000 gep3-0.3/src/common/binary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-23 19:59:45.000000 gep3-0.3/src/common/bitstr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-23 19:59:45.000000 gep3-0.3/src/common/hstr.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 19:59:45.000000 gep3-0.3/src/common/intlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-23 19:59:45.000000 gep3-0.3/src/common/parserc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 19:59:45.000000 gep3-0.3/src/common/str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-04-23 19:59:45.000000 gep3-0.3/src/crypto/des.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-23 19:59:45.000000 gep3-0.3/src/crypto/modes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/emv/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/dsc.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/key_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 19:59:45.000000 gep3-0.3/src/emv/records.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/emv_key_derivation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/evc_cvc3.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-23 19:59:45.000000 gep3-0.3/src/examples/evc_dcvv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/gep3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 19:59:48.000000 gep3-0.3/src/gep3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.191155 gep3-0.3/src/globalplatform/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 19:59:45.000000 gep3-0.3/src/globalplatform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-23 19:59:45.000000 gep3-0.3/src/globalplatform/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-23 19:59:45.000000 gep3-0.3/src/globalplatform/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/iso7816/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20583 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/apdu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-23 19:59:45.000000 gep3-0.3/src/iso7816/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/multos/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 19:59:45.000000 gep3-0.3/src/multos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 19:59:45.000000 gep3-0.3/src/multos/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-23 19:59:45.000000 gep3-0.3/src/multos/encodings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:48.195155 gep3-0.3/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:59:45.000000 gep3-0.3/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-23 19:59:45.000000 gep3-0.3/src/tests/test_common_ber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 19:59:45.000000 gep3-0.3/src/tests/test_crypto_des.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-23 20:35:28.000000 gep3-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 20:35:32.613160 gep3-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 20:35:28.000000 gep3-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-23 20:35:28.000000 gep3-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-23 20:35:32.617159 gep3-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.609159 gep3-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.609159 gep3-0.3.1/src/ccid/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-23 20:35:28.000000 gep3-0.3.1/src/ccid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-04-23 20:35:28.000000 gep3-0.3.1/src/ccid/bulk_in_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-23 20:35:28.000000 gep3-0.3.1/src/ccid/bulk_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 20:35:28.000000 gep3-0.3.1/src/ccid/bulk_out_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-23 20:35:28.000000 gep3-0.3.1/src/ccid/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.609159 gep3-0.3.1/src/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/binary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/bitstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/hstr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/intlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/parserc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-23 20:35:28.000000 gep3-0.3.1/src/common/str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.609159 gep3-0.3.1/src/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:28.000000 gep3-0.3.1/src/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-04-23 20:35:28.000000 gep3-0.3.1/src/crypto/des.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-23 20:35:28.000000 gep3-0.3.1/src/crypto/modes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/src/emv/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 20:35:28.000000 gep3-0.3.1/src/emv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-23 20:35:28.000000 gep3-0.3.1/src/emv/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12423 2024-04-23 20:35:28.000000 gep3-0.3.1/src/emv/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-23 20:35:28.000000 gep3-0.3.1/src/emv/dsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-23 20:35:28.000000 gep3-0.3.1/src/emv/key_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 20:35:28.000000 gep3-0.3.1/src/emv/records.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/src/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:28.000000 gep3-0.3.1/src/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-23 20:35:28.000000 gep3-0.3.1/src/examples/emv_key_derivation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-23 20:35:28.000000 gep3-0.3.1/src/examples/evc_cvc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-23 20:35:28.000000 gep3-0.3.1/src/examples/evc_dcvv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/src/gep3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-23 20:35:32.000000 gep3-0.3.1/src/gep3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-23 20:35:32.000000 gep3-0.3.1/src/gep3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:35:32.000000 gep3-0.3.1/src/gep3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 20:35:32.000000 gep3-0.3.1/src/gep3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 20:35:32.000000 gep3-0.3.1/src/gep3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/src/globalplatform/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-23 20:35:28.000000 gep3-0.3.1/src/globalplatform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-23 20:35:28.000000 gep3-0.3.1/src/globalplatform/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-23 20:35:28.000000 gep3-0.3.1/src/globalplatform/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/src/iso7816/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 20:35:28.000000 gep3-0.3.1/src/iso7816/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20583 2024-04-23 20:35:28.000000 gep3-0.3.1/src/iso7816/apdu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 20:35:28.000000 gep3-0.3.1/src/iso7816/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-23 20:35:28.000000 gep3-0.3.1/src/iso7816/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/src/multos/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-23 20:35:28.000000 gep3-0.3.1/src/multos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-23 20:35:28.000000 gep3-0.3.1/src/multos/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-23 20:35:28.000000 gep3-0.3.1/src/multos/encodings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:32.613160 gep3-0.3.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:35:28.000000 gep3-0.3.1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-23 20:35:28.000000 gep3-0.3.1/src/tests/test_common_ber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 20:35:28.000000 gep3-0.3.1/src/tests/test_crypto_des.py
```

### Comparing `gep3-0.3/LICENSE` & `gep3-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gep3-0.3/PKG-INFO` & `gep3-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.3
+Version: 0.3.1
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
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: parsec==3
+Requires-Dist: parsec
 
 # gep3
 Generic Encryption Peripheral: various utilities related to cryptography and smart cards
```

### Comparing `gep3-0.3/setup.cfg` & `gep3-0.3.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gep3
-version = 0.3
+version = 0.3.1
 author = Sebastien Pochic
 author_email = spochic@gmail.com
 description = Generic Encryption Peripheral: various utilities related to cryptography and smart cards
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/spochic/gep3
 project_urls = 
@@ -18,15 +18,15 @@
 	Topic :: System :: Hardware :: Universal Serial Bus (USB) :: Smart Card
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.11
-install_requires = parsec==3
+install_requires = parsec
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gep3-0.3/src/ccid/bulk_in_messages.py` & `gep3-0.3.1/src/ccid/bulk_in_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/ccid/bulk_message.py` & `gep3-0.3.1/src/ccid/bulk_message.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/ccid/bulk_out_messages.py` & `gep3-0.3.1/src/ccid/bulk_out_messages.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/ccid/descriptors.py` & `gep3-0.3.1/src/ccid/descriptors.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/common/ber.py` & `gep3-0.3.1/src/common/ber.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/common/binary.py` & `gep3-0.3.1/src/common/binary.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/common/bitstr.py` & `gep3-0.3.1/src/common/bitstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/common/hstr.py` & `gep3-0.3.1/src/common/hstr.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/common/intlist.py` & `gep3-0.3.1/src/common/intlist.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/common/parserc.py` & `gep3-0.3.1/src/common/parserc.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/common/str.py` & `gep3-0.3.1/src/common/str.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/crypto/des.py` & `gep3-0.3.1/src/crypto/des.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/crypto/modes.py` & `gep3-0.3.1/src/crypto/modes.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/emv/commands.py` & `gep3-0.3.1/src/emv/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/emv/data.py` & `gep3-0.3.1/src/emv/data.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/emv/dsc.py` & `gep3-0.3.1/src/emv/dsc.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/emv/key_management.py` & `gep3-0.3.1/src/emv/key_management.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/emv/records.py` & `gep3-0.3.1/src/emv/records.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/examples/emv_key_derivation.py` & `gep3-0.3.1/src/examples/emv_key_derivation.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/examples/evc_cvc3.py` & `gep3-0.3.1/src/examples/evc_cvc3.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/examples/evc_dcvv.py` & `gep3-0.3.1/src/examples/evc_dcvv.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/gep3.egg-info/PKG-INFO` & `gep3-0.3.1/src/gep3.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gep3
-Version: 0.3
+Version: 0.3.1
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
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: parsec==3
+Requires-Dist: parsec
 
 # gep3
 Generic Encryption Peripheral: various utilities related to cryptography and smart cards
```

### Comparing `gep3-0.3/src/gep3.egg-info/SOURCES.txt` & `gep3-0.3.1/src/gep3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/globalplatform/commands.py` & `gep3-0.3.1/src/globalplatform/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/globalplatform/encodings.py` & `gep3-0.3.1/src/globalplatform/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/iso7816/apdu.py` & `gep3-0.3.1/src/iso7816/apdu.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/iso7816/commands.py` & `gep3-0.3.1/src/iso7816/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/iso7816/encodings.py` & `gep3-0.3.1/src/iso7816/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/multos/commands.py` & `gep3-0.3.1/src/multos/commands.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/multos/encodings.py` & `gep3-0.3.1/src/multos/encodings.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/tests/test_common_ber.py` & `gep3-0.3.1/src/tests/test_common_ber.py`

 * *Files identical despite different names*

### Comparing `gep3-0.3/src/tests/test_crypto_des.py` & `gep3-0.3.1/src/tests/test_crypto_des.py`

 * *Files identical despite different names*

