# Comparing `tmp/la_coding_theory-0.0.3.tar.gz` & `tmp/la_coding_theory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "la_coding_theory-0.0.3.tar", last modified: Sat Apr 20 14:37:54 2024, max compression
+gzip compressed data, was "la_coding_theory-0.0.4.tar", last modified: Tue Apr 23 12:13:18 2024, max compression
```

## Comparing `la_coding_theory-0.0.3.tar` & `la_coding_theory-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-20 14:37:54.697345 la_coding_theory-0.0.3/
--rw-r--r--   0 maxondevelop   (501) staff       (20)     1073 2024-04-15 13:57:55.000000 la_coding_theory-0.0.3/LICENCE
--rw-r--r--   0 maxondevelop   (501) staff       (20)      812 2024-04-20 14:37:54.697118 la_coding_theory-0.0.3/PKG-INFO
--rw-r--r--   0 maxondevelop   (501) staff       (20)      171 2024-04-15 13:58:05.000000 la_coding_theory-0.0.3/README.md
--rw-r--r--   0 maxondevelop   (501) staff       (20)      661 2024-04-20 14:36:12.000000 la_coding_theory-0.0.3/pyproject.toml
--rw-r--r--   0 maxondevelop   (501) staff       (20)       38 2024-04-20 14:37:54.697392 la_coding_theory-0.0.3/setup.cfg
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-20 14:37:54.695236 la_coding_theory-0.0.3/src/
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-20 14:37:54.696217 la_coding_theory-0.0.3/src/la_coding_theory/
--rw-------   0 maxondevelop   (501) staff       (20)     9790 2024-04-20 14:24:41.000000 la_coding_theory-0.0.3/src/la_coding_theory/__convolutional.py
--rw-r--r--   0 maxondevelop   (501) staff       (20)     3282 2024-04-17 11:28:08.000000 la_coding_theory-0.0.3/src/la_coding_theory/__crc.py
--rw-r--r--   0 maxondevelop   (501) staff       (20)        0 2024-04-15 14:00:47.000000 la_coding_theory-0.0.3/src/la_coding_theory/__init__.py
--rw-r--r--   0 maxondevelop   (501) staff       (20)     3279 2024-04-20 14:35:06.000000 la_coding_theory-0.0.3/src/la_coding_theory/_lrc.py
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-20 14:37:54.696905 la_coding_theory-0.0.3/src/la_coding_theory.egg-info/
--rw-r--r--   0 maxondevelop   (501) staff       (20)      812 2024-04-20 14:37:54.000000 la_coding_theory-0.0.3/src/la_coding_theory.egg-info/PKG-INFO
--rw-r--r--   0 maxondevelop   (501) staff       (20)      340 2024-04-20 14:37:54.000000 la_coding_theory-0.0.3/src/la_coding_theory.egg-info/SOURCES.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)        1 2024-04-20 14:37:54.000000 la_coding_theory-0.0.3/src/la_coding_theory.egg-info/dependency_links.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)       17 2024-04-20 14:37:54.000000 la_coding_theory-0.0.3/src/la_coding_theory.egg-info/top_level.txt
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-23 12:13:18.114036 la_coding_theory-0.0.4/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)     1073 2024-04-15 13:57:55.000000 la_coding_theory-0.0.4/LICENCE
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      812 2024-04-23 12:13:18.113868 la_coding_theory-0.0.4/PKG-INFO
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      171 2024-04-15 13:58:05.000000 la_coding_theory-0.0.4/README.md
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      661 2024-04-23 12:11:37.000000 la_coding_theory-0.0.4/pyproject.toml
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       38 2024-04-23 12:13:18.114077 la_coding_theory-0.0.4/setup.cfg
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-23 12:13:18.110862 la_coding_theory-0.0.4/src/
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-23 12:13:18.113108 la_coding_theory-0.0.4/src/la_coding_theory/
+-rw-------   0 maxondevelop   (501) staff       (20)     9790 2024-04-20 14:24:41.000000 la_coding_theory-0.0.4/src/la_coding_theory/__convolutional.py
+-rw-r--r--   0 maxondevelop   (501) staff       (20)     2605 2024-04-22 19:15:12.000000 la_coding_theory-0.0.4/src/la_coding_theory/__crc.py
+-rw-r--r--   0 maxondevelop   (501) staff       (20)        0 2024-04-15 14:00:47.000000 la_coding_theory-0.0.4/src/la_coding_theory/__init__.py
+-rw-r--r--   0 maxondevelop   (501) staff       (20)     3279 2024-04-20 14:35:06.000000 la_coding_theory-0.0.4/src/la_coding_theory/__lrc.py
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      133 2024-04-22 19:44:37.000000 la_coding_theory-0.0.4/src/la_coding_theory/__vrc.py
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-23 12:13:18.113703 la_coding_theory-0.0.4/src/la_coding_theory.egg-info/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      812 2024-04-23 12:13:18.000000 la_coding_theory-0.0.4/src/la_coding_theory.egg-info/PKG-INFO
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      371 2024-04-23 12:13:18.000000 la_coding_theory-0.0.4/src/la_coding_theory.egg-info/SOURCES.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)        1 2024-04-23 12:13:18.000000 la_coding_theory-0.0.4/src/la_coding_theory.egg-info/dependency_links.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       17 2024-04-23 12:13:18.000000 la_coding_theory-0.0.4/src/la_coding_theory.egg-info/top_level.txt
```

### Comparing `la_coding_theory-0.0.3/LICENCE` & `la_coding_theory-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `la_coding_theory-0.0.3/PKG-INFO` & `la_coding_theory-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: la_coding_theory
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small library, where we implemented  some coding algorithms with LA proving
 Author-email: Max Kutsenko <kutsenko.pn@ucu.edu.ua>, Katja Kovalchuk <kovalchuk.pn@ucu.edu.ua>, Roman Zaletskyy <rzaletskyy@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `la_coding_theory-0.0.3/pyproject.toml` & `la_coding_theory-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "la_coding_theory"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Max Kutsenko", email="kutsenko.pn@ucu.edu.ua" },
 	{ name="Katja Kovalchuk", email="kovalchuk.pn@ucu.edu.ua" },
 	{ name="Roman Zaletskyy", email="rzaletskyy@gmail.com" },
 ]
 description = "A small library, where we implemented  some coding algorithms with LA proving"
 readme = "README.md"
```

### Comparing `la_coding_theory-0.0.3/src/la_coding_theory/__convolutional.py` & `la_coding_theory-0.0.4/src/la_coding_theory/__convolutional.py`

 * *Files identical despite different names*

### Comparing `la_coding_theory-0.0.3/src/la_coding_theory/__crc.py` & `la_coding_theory-0.0.4/src/la_coding_theory/__crc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,69 @@
 """
-Cyclic Redundancy Check implementation
+     implementation
 """
 
 import typing as _typing
-import matplotlib.pyplot as plt
+import random as _random
 
 
 class CRC:
     """
     Cyclic Redundancy Check class
     """
     def __init__(self, message: str, key: str) -> None:
         """
         __init__ method
         """
         self.message = message
         self.key = key
-
-    def _message_to_bits(self) -> str:
-        """
-        Convert inner message to bits
-        """
-        return ''.join(format(ord(x), '08b') for x in self.message)
-    
-    def _key_to_bits(self) -> str:
-        """
-        Convert key value to bits
-        """
-        return ''.join(format(ord(x), '08b') for x in self.key)
-    
-    def _bits_message_to_string(self) -> str:
-        """
-        convert bits message to string
-        """
-        bits_message = self._message_to_bits()
-        return ''.join([chr(int(bits_message[i:i + 8], 2)) for i in range(0, len(bits_message), 8)])
     
     def _xor(self, data_1: str, data_2: str) -> str:
         """
         Find XOR between two massages
         """
         return ''.join(['0' if data_1[i] == data_2[i] else '1' for i in range(1, len(data_2))])
 
     def _mod_2_div(self, dividend: str) -> str:
         """
         Find mod 2
         """
-        pick = len(self._key_to_bits())
+        pick = len(self.key)
         tmp = dividend[0:pick]
 
         while pick < len(dividend):
             if tmp[0] == '1':
-                tmp = self._xor(self._key_to_bits(), tmp) + dividend[pick]
+                tmp = self._xor(self.key, tmp) + dividend[pick]
             else:
                 tmp = self._xor('0' * pick, tmp) + dividend[pick]
             pick += 1
         if tmp[0] == '1':
-            tmp = self._xor(self._key_to_bits(), tmp)
+            tmp = self._xor(self.key, tmp)
         else:
             tmp = self._xor('0' * pick, tmp)
         checkword = tmp
         return checkword
 
     def _encode_data(self) -> _typing.Tuple[str, str]:
         """
         Encode process
         """
-        l_key = len(self._key_to_bits())
+        l_key = len(self.key)
 
-        appended_data = self._message_to_bits() + '0' * (l_key - 1)
+        appended_data = self.message + '0' * (l_key - 1)
         remainder = self._mod_2_div(appended_data)
 
-        codeword = self._message_to_bits() + remainder
+        codeword = self.message + remainder
         return (codeword, remainder)
 
     def _decode_data(self, encoded_data: str) -> _typing.Tuple[str, str]:
         """
         Decode process
         """
-        l_key = len(self._key_to_bits())
+        l_key = len(self.key)
 
         remainder = self._mod_2_div(encoded_data)
         return (encoded_data[:(len(encoded_data) - len(remainder))], remainder)
     
     def _display(self) -> None:
         """
         Display results
@@ -91,15 +72,15 @@
         encoded_data, encoded_reminder = encoded_data_items[0], encoded_data_items[1]
 
         decoded_data_items = self._decode_data(encoded_data)
         decoded_data, decoded_reminder = decoded_data_items[0], decoded_data_items[1]
         print(f'Inner data = {self.message}\nKey = {self.key}\nEncoded data = {encoded_data}\nEncode reminder = {encoded_reminder}\nDecoded data = {decoded_data}\nDecoded reminder = {decoded_reminder}\n{"Data transmitted correctly" if all(i == '0' for i in decoded_reminder) else "Data transmitted corrupt"}')
         return encoded_data
 
-
 if __name__ == "__main__":
-    text_messgae = "hello"
-    key = "s"
-    crc = CRC(text_messgae, key)
-    encoded_data = crc._display()
-    print()
-    print(crc._bits_message_to_string())
+    # text_messgae = "hello"
+    # key = "s"
+    # crc = CRC(text_messgae, key)
+    # encoded_data = crc._display()
+    # print()
+    # print(crc._bits_message_to_string())
+    pass
```

### Comparing `la_coding_theory-0.0.3/src/la_coding_theory/_lrc.py` & `la_coding_theory-0.0.4/src/la_coding_theory/__lrc.py`

 * *Files identical despite different names*

### Comparing `la_coding_theory-0.0.3/src/la_coding_theory.egg-info/PKG-INFO` & `la_coding_theory-0.0.4/src/la_coding_theory.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: la_coding_theory
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small library, where we implemented  some coding algorithms with LA proving
 Author-email: Max Kutsenko <kutsenko.pn@ucu.edu.ua>, Katja Kovalchuk <kovalchuk.pn@ucu.edu.ua>, Roman Zaletskyy <rzaletskyy@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

