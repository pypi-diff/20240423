# Comparing `tmp/bytecore-1.1.0.tar.gz` & `tmp/bytecore-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytecore-1.1.0.tar", last modified: Sun Oct  8 19:26:13 2023, max compression
+gzip compressed data, was "bytecore-1.1.1.tar", last modified: Tue Apr 23 21:40:24 2024, max compression
```

## Comparing `bytecore-1.1.0.tar` & `bytecore-1.1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-10-08 19:26:13.656720 bytecore-1.1.0/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1074 2023-10-08 19:25:20.000000 bytecore-1.1.0/LICENSE
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14737 2023-10-08 19:26:13.656720 bytecore-1.1.0/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14160 2023-10-08 19:25:20.000000 bytecore-1.1.0/README.md
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      756 2023-10-08 19:25:20.000000 bytecore-1.1.0/pyproject.toml
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2023-10-08 19:26:13.656720 bytecore-1.1.0/setup.cfg
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-10-08 19:26:13.648720 bytecore-1.1.0/src/
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-10-08 19:26:13.652720 bytecore-1.1.0/src/bytecore/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/__init__.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4662 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/accumulator.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      799 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/bit.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2162 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/byte.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1769 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/byte_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      294 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/constant_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11455 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/control_unit.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      276 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/control_unit_state.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2620 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/cpu.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1024 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/emulator.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2737 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/memory.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1552 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/memory_bytes_builder.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      178 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/opcode.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1009 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/proxy_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/py.typed
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1974 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/replay_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1146 2023-10-08 19:25:20.000000 bytecore-1.1.0/src/bytecore/state.py
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-10-08 19:26:13.656720 bytecore-1.1.0/src/bytecore.egg-info/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14737 2023-10-08 19:26:13.000000 bytecore-1.1.0/src/bytecore.egg-info/PKG-INFO
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)      820 2023-10-08 19:26:13.000000 bytecore-1.1.0/src/bytecore.egg-info/SOURCES.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2023-10-08 19:26:13.000000 bytecore-1.1.0/src/bytecore.egg-info/dependency_links.txt
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)        9 2023-10-08 19:26:13.000000 bytecore-1.1.0/src/bytecore.egg-info/top_level.txt
-drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2023-10-08 19:26:13.656720 bytecore-1.1.0/tests/
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1085 2023-10-08 19:25:20.000000 bytecore-1.1.0/tests/test_bit.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2959 2023-10-08 19:25:20.000000 bytecore-1.1.0/tests/test_byte.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1707 2023-10-08 19:25:20.000000 bytecore-1.1.0/tests/test_byte_register.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15238 2023-10-08 19:25:20.000000 bytecore-1.1.0/tests/test_cpu.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     8575 2023-10-08 19:25:20.000000 bytecore-1.1.0/tests/test_emulator.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3238 2023-10-08 19:25:20.000000 bytecore-1.1.0/tests/test_memory.py
--rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10452 2023-10-08 19:25:20.000000 bytecore-1.1.0/tests/test_memory_bytes_builder.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:40:24.442379 bytecore-1.1.1/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1074 2024-04-23 20:32:09.000000 bytecore-1.1.1/LICENSE
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14737 2024-04-23 21:40:24.438379 bytecore-1.1.1/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14160 2024-04-23 20:32:09.000000 bytecore-1.1.1/README.md
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      756 2024-04-23 21:35:58.000000 bytecore-1.1.1/pyproject.toml
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)       38 2024-04-23 21:40:24.442379 bytecore-1.1.1/setup.cfg
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:40:24.434379 bytecore-1.1.1/src/
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:40:24.438379 bytecore-1.1.1/src/bytecore/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/__init__.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     4584 2024-04-23 21:07:29.000000 bytecore-1.1.1/src/bytecore/accumulator.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      799 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/bit.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2162 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/byte.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1769 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/byte_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      294 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/constant_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    11455 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/control_unit.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      276 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/control_unit_state.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2620 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/cpu.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1024 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/emulator.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2737 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/memory.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1552 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/memory_bytes_builder.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      178 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/opcode.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1009 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/proxy_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/py.typed
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      439 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1974 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/replay_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1146 2024-04-23 20:32:09.000000 bytecore-1.1.1/src/bytecore/state.py
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:40:24.438379 bytecore-1.1.1/src/bytecore.egg-info/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    14737 2024-04-23 21:40:24.000000 bytecore-1.1.1/src/bytecore.egg-info/PKG-INFO
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)      820 2024-04-23 21:40:24.000000 bytecore-1.1.1/src/bytecore.egg-info/SOURCES.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        1 2024-04-23 21:40:24.000000 bytecore-1.1.1/src/bytecore.egg-info/dependency_links.txt
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)        9 2024-04-23 21:40:24.000000 bytecore-1.1.1/src/bytecore.egg-info/top_level.txt
+drwxr-xr-x   0 gitpod   (33333) gitpod   (33333)        0 2024-04-23 21:40:24.438379 bytecore-1.1.1/tests/
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1085 2024-04-23 20:32:09.000000 bytecore-1.1.1/tests/test_bit.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     2959 2024-04-23 20:32:09.000000 bytecore-1.1.1/tests/test_byte.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     1707 2024-04-23 20:32:09.000000 bytecore-1.1.1/tests/test_byte_register.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    15238 2024-04-23 20:32:09.000000 bytecore-1.1.1/tests/test_cpu.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10983 2024-04-23 21:30:28.000000 bytecore-1.1.1/tests/test_emulator.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)     3238 2024-04-23 20:32:09.000000 bytecore-1.1.1/tests/test_memory.py
+-rw-r--r--   0 gitpod   (33333) gitpod   (33333)    10452 2024-04-23 20:32:09.000000 bytecore-1.1.1/tests/test_memory_bytes_builder.py
```

### Comparing `bytecore-1.1.0/LICENSE` & `bytecore-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/PKG-INFO` & `bytecore-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecore
-Version: 1.1.0
+Version: 1.1.1
 Summary: A minimal, 8-bit CPU emulator designed to help developers explore low-level computing concepts.
 Author-email: Joakim Winum Lien <joakim@winum.xyz>
 Project-URL: Homepage, https://github.com/joakimwinum/bytecore
 Project-URL: Bug Tracker, https://github.com/joakimwinum/bytecore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bytecore-1.1.0/README.md` & `bytecore-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/pyproject.toml` & `bytecore-1.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bytecore"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Joakim Winum Lien", email="joakim@winum.xyz" },
 ]
 description = "A minimal, 8-bit CPU emulator designed to help developers explore low-level computing concepts."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `bytecore-1.1.0/src/bytecore/accumulator.py` & `bytecore-1.1.1/src/bytecore/accumulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,32 +60,32 @@
 
         self._memory.read_high()
         memory = self._memory.get_bus()
         self._memory.read_low()
 
         result = self._byte_adder_helper(temp, memory)
 
-        self._accumulator.write_high()
-        self._accumulator.set_bus(result)
-        self._accumulator.write_low()
+        self.write_high()
+        self.set_bus(result)
+        self.write_low()
 
     def sub_memory_from_accumulator(self) -> None:
         self._temp_register.read_high()
         temp = self._temp_register.get_bus()
         self._temp_register.read_low()
 
         self._memory.read_high()
         memory = self._memory.get_bus()
         self._memory.read_low()
 
         result = self._byte_subtractor_helper(temp, memory)
 
-        self._accumulator.write_high()
-        self._accumulator.set_bus(result)
-        self._accumulator.write_low()
+        self.write_high()
+        self.set_bus(result)
+        self.write_low()
 
     def write_high(self) -> None:
         self._accumulator.write_high()
 
     def write_low(self) -> None:
         self._accumulator.write_low()
```

### Comparing `bytecore-1.1.0/src/bytecore/bit.py` & `bytecore-1.1.1/src/bytecore/bit.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/byte.py` & `bytecore-1.1.1/src/bytecore/byte.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/byte_register.py` & `bytecore-1.1.1/src/bytecore/byte_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/control_unit.py` & `bytecore-1.1.1/src/bytecore/control_unit.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/cpu.py` & `bytecore-1.1.1/src/bytecore/cpu.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/emulator.py` & `bytecore-1.1.1/src/bytecore/emulator.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/memory.py` & `bytecore-1.1.1/src/bytecore/memory.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/memory_bytes_builder.py` & `bytecore-1.1.1/src/bytecore/memory_bytes_builder.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/proxy_register.py` & `bytecore-1.1.1/src/bytecore/proxy_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/replay_register.py` & `bytecore-1.1.1/src/bytecore/replay_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore/state.py` & `bytecore-1.1.1/src/bytecore/state.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/src/bytecore.egg-info/PKG-INFO` & `bytecore-1.1.1/src/bytecore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytecore
-Version: 1.1.0
+Version: 1.1.1
 Summary: A minimal, 8-bit CPU emulator designed to help developers explore low-level computing concepts.
 Author-email: Joakim Winum Lien <joakim@winum.xyz>
 Project-URL: Homepage, https://github.com/joakimwinum/bytecore
 Project-URL: Bug Tracker, https://github.com/joakimwinum/bytecore/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bytecore-1.1.0/src/bytecore.egg-info/SOURCES.txt` & `bytecore-1.1.1/src/bytecore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/tests/test_bit.py` & `bytecore-1.1.1/tests/test_bit.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/tests/test_byte.py` & `bytecore-1.1.1/tests/test_byte.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/tests/test_byte_register.py` & `bytecore-1.1.1/tests/test_byte_register.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/tests/test_cpu.py` & `bytecore-1.1.1/tests/test_cpu.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/tests/test_emulator.py` & `bytecore-1.1.1/tests/test_emulator.py`

 * *Files 18% similar despite different names*

```diff
@@ -250,7 +250,73 @@
         #                         # 2
         accumulator = a           # LOAD
         output = accumulator      # STORE
         #                         # HALT
 
         # Assert
         assert output == expected
+
+    def test__cycle__jz_works_as_expected_after_add__accumulator_and_pc_contains_expected_values(self) -> None:
+        # Arrange
+        expected_accumulator = Byte(1)
+        expected_msb_register = Byte(0)
+        expected_lsb_register = Byte(9)
+        memory_bytes = MemoryBytesBuilder()\
+            .msb('00').lsb('00').load()\
+            .msb('00').lsb('01').data('01')\
+            .msb('00').lsb('02').data('00')\
+            .msb('00').lsb('03').add()\
+            .msb('00').lsb('04').data('01')\
+            .msb('00').lsb('05').data('01')\
+            .msb('00').lsb('06').jz()\
+            .msb('00').lsb('07').data('FF')\
+            .msb('00').lsb('08').data('FF')\
+            \
+            .msb('01').lsb('00').data('00').comment(' 0')\
+            .msb('01').lsb('01').data('01').comment(' 1')\
+            .build()
+
+        byte_core = ByteCore(memory_bytes)
+
+        # Act
+        byte_core.cycle()
+        byte_core.cycle()
+        byte_core.cycle()
+        dump = byte_core.dump()
+
+        # Assert
+        assert dump.accumulator == expected_accumulator
+        assert dump.pc_msb_register == expected_msb_register
+        assert dump.pc_lsb_register == expected_lsb_register
+
+    def test__cycle__jz_works_as_expected_after_sub__accumulator_and_pc_contains_expected_values(self) -> None:
+        # Arrange
+        expected_accumulator = Byte(255)
+        expected_msb_register = Byte(0)
+        expected_lsb_register = Byte(9)
+        memory_bytes = MemoryBytesBuilder()\
+            .msb('00').lsb('00').load()\
+            .msb('00').lsb('01').data('01')\
+            .msb('00').lsb('02').data('00')\
+            .msb('00').lsb('03').sub()\
+            .msb('00').lsb('04').data('01')\
+            .msb('00').lsb('05').data('01')\
+            .msb('00').lsb('06').jz()\
+            .msb('00').lsb('07').data('FF')\
+            .msb('00').lsb('08').data('FF')\
+            \
+            .msb('01').lsb('00').data('00').comment(' 0')\
+            .msb('01').lsb('01').data('01').comment(' 1')\
+            .build()
+
+        byte_core = ByteCore(memory_bytes)
+
+        # Act
+        byte_core.cycle()
+        byte_core.cycle()
+        byte_core.cycle()
+        dump = byte_core.dump()
+
+        # Assert
+        assert dump.accumulator == expected_accumulator
+        assert dump.pc_msb_register == expected_msb_register
+        assert dump.pc_lsb_register == expected_lsb_register
```

### Comparing `bytecore-1.1.0/tests/test_memory.py` & `bytecore-1.1.1/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `bytecore-1.1.0/tests/test_memory_bytes_builder.py` & `bytecore-1.1.1/tests/test_memory_bytes_builder.py`

 * *Files identical despite different names*

