# Comparing `tmp/octoflatbuffers-2.0.8.tar.gz` & `tmp/octoflatbuffers-24.3.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoflatbuffers-2.0.8.tar", last modified: Thu Jan  4 19:24:21 2024, max compression
+gzip compressed data, was "octoflatbuffers-24.3.25.tar", last modified: Mon Apr 22 22:57:53 2024, max compression
```

## Comparing `octoflatbuffers-2.0.8.tar` & `octoflatbuffers-24.3.25.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 19:24:21.382284 octoflatbuffers-2.0.8/
--rw-rw-rw-   0        0        0     1484 2024-01-04 19:24:21.381280 octoflatbuffers-2.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-01-04 19:24:21.363720 octoflatbuffers-2.0.8/octoflatbuffers/
--rw-rw-rw-   0        0        0      770 2022-12-05 05:05:56.000000 octoflatbuffers-2.0.8/octoflatbuffers/__init__.py
--rw-rw-rw-   0        0        0      711 2024-01-04 19:24:21.000000 octoflatbuffers-2.0.8/octoflatbuffers/_version.py
--rw-rw-rw-   0        0        0    26740 2022-12-05 05:51:57.000000 octoflatbuffers-2.0.8/octoflatbuffers/builder.py
--rw-rw-rw-   0        0        0     2195 2022-12-05 05:39:21.000000 octoflatbuffers-2.0.8/octoflatbuffers/compat.py
--rw-rw-rw-   0        0        0     1548 2022-12-05 05:25:31.000000 octoflatbuffers-2.0.8/octoflatbuffers/encode.py
--rw-rw-rw-   0        0        0    45554 2022-12-05 05:05:56.000000 octoflatbuffers-2.0.8/octoflatbuffers/flexbuffers.py
--rw-rw-rw-   0        0        0     4061 2022-12-05 05:26:31.000000 octoflatbuffers-2.0.8/octoflatbuffers/number_types.py
--rw-rw-rw-   0        0        0     1207 2022-12-05 05:05:56.000000 octoflatbuffers-2.0.8/octoflatbuffers/packer.py
--rw-rw-rw-   0        0        0     5189 2022-12-05 05:05:56.000000 octoflatbuffers-2.0.8/octoflatbuffers/table.py
--rw-rw-rw-   0        0        0     1712 2022-12-05 05:05:56.000000 octoflatbuffers-2.0.8/octoflatbuffers/util.py
-drwxrwxrwx   0        0        0        0 2024-01-04 19:24:21.380282 octoflatbuffers-2.0.8/octoflatbuffers.egg-info/
--rw-rw-rw-   0        0        0     1484 2024-01-04 19:24:21.000000 octoflatbuffers-2.0.8/octoflatbuffers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2024-01-04 19:24:21.000000 octoflatbuffers-2.0.8/octoflatbuffers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 19:24:21.000000 octoflatbuffers-2.0.8/octoflatbuffers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-01-04 19:24:21.000000 octoflatbuffers-2.0.8/octoflatbuffers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2024-01-04 19:24:21.384284 octoflatbuffers-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2935 2024-01-04 19:24:04.000000 octoflatbuffers-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:57:53.680150 octoflatbuffers-24.3.25/
+-rw-rw-rw-   0        0        0     1512 2024-04-22 22:57:53.679151 octoflatbuffers-24.3.25/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-22 22:57:53.661115 octoflatbuffers-24.3.25/octoflatbuffers/
+-rw-rw-rw-   0        0        0      770 2024-04-22 22:31:27.000000 octoflatbuffers-24.3.25/octoflatbuffers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-22 22:57:53.000000 octoflatbuffers-24.3.25/octoflatbuffers/_version.py
+-rw-rw-rw-   0        0        0    28330 2024-04-22 22:31:42.000000 octoflatbuffers-24.3.25/octoflatbuffers/builder.py
+-rw-rw-rw-   0        0        0     2976 2024-04-22 22:31:42.000000 octoflatbuffers-24.3.25/octoflatbuffers/compat.py
+-rw-rw-rw-   0        0        0     1634 2024-04-22 22:31:42.000000 octoflatbuffers-24.3.25/octoflatbuffers/encode.py
+-rw-rw-rw-   0        0        0    45811 2024-04-22 22:31:42.000000 octoflatbuffers-24.3.25/octoflatbuffers/flexbuffers.py
+-rw-rw-rw-   0        0        0     4147 2024-04-22 22:31:42.000000 octoflatbuffers-24.3.25/octoflatbuffers/number_types.py
+-rw-rw-rw-   0        0        0     1207 2024-04-22 22:31:27.000000 octoflatbuffers-24.3.25/octoflatbuffers/packer.py
+-rw-rw-rw-   0        0        0     5660 2024-04-22 22:31:42.000000 octoflatbuffers-24.3.25/octoflatbuffers/table.py
+-rw-rw-rw-   0        0        0     1712 2024-04-22 22:31:27.000000 octoflatbuffers-24.3.25/octoflatbuffers/util.py
+drwxrwxrwx   0        0        0        0 2024-04-22 22:57:53.678149 octoflatbuffers-24.3.25/octoflatbuffers.egg-info/
+-rw-rw-rw-   0        0        0     1512 2024-04-22 22:57:53.000000 octoflatbuffers-24.3.25/octoflatbuffers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2024-04-22 22:57:53.000000 octoflatbuffers-24.3.25/octoflatbuffers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 22:57:53.000000 octoflatbuffers-24.3.25/octoflatbuffers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-22 22:57:53.000000 octoflatbuffers-24.3.25/octoflatbuffers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      119 2024-04-22 22:57:53.686670 octoflatbuffers-24.3.25/setup.cfg
+-rw-rw-rw-   0        0        0     2895 2024-04-22 22:57:46.000000 octoflatbuffers-24.3.25/setup.py
```

### Comparing `octoflatbuffers-2.0.8/PKG-INFO` & `octoflatbuffers-24.3.25/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoflatbuffers
-Version: 2.0.8
+Version: 24.3.25
 Summary: A fork of flatbuffers used for OctoEverywhere and Homeway
 Home-page: https://github.com/QuinnDamerell/octoflatbuffers
 Author: Quinn Damerell
 Author-email: support@octoeverywhere.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/QuinnDamerell/octoflatbuffers
 Project-URL: Source, https://github.com/QuinnDamerell/octoflatbuffers
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: ../license
 
 
 # OctoFlatBuffers
 A fork of [flatbuffers](https://flatbuffers.dev/) with some special modifications. Used as the core protocol for:
 - [OctoEverywhere](https://octoeverywhere.com/?source=pypi) - Free, private, and secure remote access for OctoPrint and Klipper 3D printer.
 - [Homeway](https://homeway.io/?source=pypi) - Free, private, and secure remote access for Home Assistant.
```

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/__init__.py` & `octoflatbuffers-24.3.25/octoflatbuffers/__init__.py`

 * *Files identical despite different names*

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/builder.py` & `octoflatbuffers-24.3.25/octoflatbuffers/builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,21 @@
 
 from . import encode
 from . import packer
 
 from . import compat
 from .compat import range_func
 from .compat import memoryview_type
+#from .compat import import_numpy, NumpyRequiredForThisFeature
+#np = import_numpy()
 np = None
 
+import warnings
+
+np = import_numpy()
 ## @file
 ## @addtogroup flatbuffers_python_api
 ## @{
 
 ## @cond FLATBUFFERS_INTERNAL
 class OffsetArithmeticError(RuntimeError):
     """
@@ -70,14 +75,21 @@
 
 class BuilderNotFinishedError(RuntimeError):
     """
     Error caused by not calling `Finish` before calling `Output`.
     """
     pass
 
+class EndVectorLengthMismatched(RuntimeError):
+    """
+    The number of elements passed to EndVector does not match the number 
+    specified in StartVector.
+    """
+    pass
+
 
 # VtableMetadataFields is the count of metadata fields in each vtable.
 VtableMetadataFields = 2
 ## @endcond
 
 class Builder(object):
     """ A Builder is used to construct one or more FlatBuffers.
@@ -98,15 +110,16 @@
     Attributes:
       Bytes: The internal `bytearray` for the Builder.
       finished: A boolean determining if the Builder has been finalized.
     """
 
     ## @cond FLATBUFFERS_INTENRAL
     __slots__ = ("Bytes", "current_vtable", "head", "minalign", "objectEnd",
-                 "vtables", "nested", "forceDefaults", "finished", "vectorNumElems")
+                 "vtables", "nested", "forceDefaults", "finished", "vectorNumElems",
+                 "sharedStrings")
 
     """Maximum buffer size constant, in bytes.
 
     Builder will never allow it's buffer grow over this size.
     Currently equals 2Gb.
     """
     MAX_BUFFER_SIZE = 2**31
@@ -127,14 +140,29 @@
         self.current_vtable = None
         self.head = UOffsetTFlags.py_type(initialSize)
         self.minalign = 1
         self.objectEnd = None
         self.vtables = {}
         self.nested = False
         self.forceDefaults = False
+        self.sharedStrings = {}
+        ## @endcond
+        self.finished = False
+
+    def Clear(self) -> None:
+        ## @cond FLATBUFFERS_INTERNAL
+        self.current_vtable = None
+        self.head = UOffsetTFlags.py_type(len(self.Bytes))
+        self.minalign = 1
+        self.objectEnd = None
+        self.vtables = {}
+        self.nested = False
+        self.forceDefaults = False
+        self.sharedStrings = {}
+        self.vectorNumElems = None
         ## @endcond
         self.finished = False
 
     def Output(self):
         """Return the portion of the buffer that has been used for writing data.
 
         This is the typical way to access the FlatBuffer data inside the
@@ -372,26 +400,47 @@
         self.nested = True
         self.vectorNumElems = numElems
         self.Prep(N.Uint32Flags.bytewidth, elemSize*numElems)
         self.Prep(alignment, elemSize*numElems)  # In case alignment > int.
         return self.Offset()
     ## @endcond
 
-    def EndVector(self):
+    def EndVector(self, numElems = None):
         """EndVector writes data necessary to finish vector construction."""
 
         self.assertNested()
         ## @cond FLATBUFFERS_INTERNAL
         self.nested = False
         ## @endcond
+               
+        if numElems:
+            warnings.warn("numElems is deprecated.", 
+                          DeprecationWarning, stacklevel=2)
+            if numElems != self.vectorNumElems:
+                raise EndVectorLengthMismatched();
+
         # we already made space for this, so write without PrependUint32
         self.PlaceUOffsetT(self.vectorNumElems)
         self.vectorNumElems = None
         return self.Offset()
 
+    def CreateSharedString(self, s, encoding='utf-8', errors='strict'):
+        """
+        CreateSharedString checks if the string is already written to the buffer
+        before calling CreateString.
+        """
+
+        if s in self.sharedStrings:
+            return self.sharedStrings[s]
+
+        off = self.CreateString(s, encoding, errors)
+        self.sharedStrings[s] = off
+
+        return off
+
     def CreateString(self, s, encoding='utf-8', errors='strict'):
         """CreateString writes a null-terminated byte string as a vector."""
 
         self.assertNotNested()
         ## @cond FLATBUFFERS_INTERNAL
         self.nested = True
         ## @endcond
@@ -557,17 +606,19 @@
 
     ## @cond FLATBUFFERS_INTERNAL
     def Prepend(self, flags, off):
         self.Prep(flags.bytewidth, 0)
         self.Place(off, flags)
 
     def PrependSlot(self, flags, o, x, d):
-        N.enforce_number(x, flags)
-        N.enforce_number(d, flags)
-        if x != d or self.forceDefaults:
+        if x is not None:
+            N.enforce_number(x, flags)
+        if d is not None:
+            N.enforce_number(d, flags)
+        if x != d or (self.forceDefaults and d is not None):
             self.Prepend(flags, x)
             self.Slot(o)
 
     def PrependBoolSlot(self, *args): self.PrependSlot(N.BoolFlags, *args)
 
     def PrependByteSlot(self, *args): self.PrependSlot(N.Uint8Flags, *args)
```

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/compat.py` & `octoflatbuffers-24.3.25/octoflatbuffers/compat.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ A tiny version of `six` to help with backwards compability. Also includes
  compatibility helpers for numpy. """
 
 import sys
-import imp
 
 PY2 = sys.version_info[0] == 2
 PY26 = sys.version_info[0:2] == (2, 6)
 PY27 = sys.version_info[0:2] == (2, 7)
 PY275 = sys.version_info[0:3] >= (2, 7, 5)
 PY3 = sys.version_info[0] == 3
 PY34 = sys.version_info[0:2] >= (3, 4)
 
 if PY3:
+    import importlib.machinery
     string_types = (str,)
     binary_types = (bytes,bytearray)
     range_func = range
     memoryview_type = memoryview
     struct_bool_decl = "?"
 else:
+    import imp
     string_types = (unicode,)
     if PY26 or PY27:
         binary_types = (str,bytearray)
     else:
         binary_types = (str,)
     range_func = xrange
     if PY26 or (PY27 and not PY275):
@@ -44,14 +45,38 @@
     else:
         memoryview_type = memoryview
         struct_bool_decl = "?"
 
 # Helper functions to facilitate making numpy optional instead of required
 
 def import_numpy():
+    """
+    Returns the numpy module if it exists on the system,
+    otherwise returns None.
+    """
+    # if PY3:
+    #     numpy_exists = (
+    #         importlib.machinery.PathFinder.find_spec('numpy') is not None)
+    # else:
+    #     try:
+    #         imp.find_module('numpy')
+    #         numpy_exists = True
+    #     except ImportError:
+    #         numpy_exists = False
+
+    # if numpy_exists:
+    #     # We do this outside of try/except block in case numpy exists
+    #     # but is not installed correctly. We do not want to catch an
+    #     # incorrect installation which would manifest as an
+    #     # ImportError.
+    #     import numpy as np
+    # else:
+    #     np = None
+    #
+    # return np
     # OctoEverywhere change! - Disable any type of numpy loading.
     # We found a few of our users had other plugins attempt to load numpy and it didn't fully install.
     # Thus, when numpy attempts to load, it discovers it's broken, and throws and fails, and messes up our plugin.
     numpy_exists = False
     return None
```

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/encode.py` & `octoflatbuffers-24.3.25/octoflatbuffers/encode.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import number_types as N
 from . import packer
 from .compat import memoryview_type
+#from .compat import import_numpy, NumpyRequiredForThisFeature
+#np = import_numpy()
 np = None
 
 FILE_IDENTIFIER_LENGTH=4
 
 def Get(packer_type, buf, head):
     """ Get decodes a value at buf[head] using `packer_type`. """
     return packer_type.unpack_from(memoryview_type(buf), head)[0]
```

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/flexbuffers.py` & `octoflatbuffers-24.3.25/octoflatbuffers/flexbuffers.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     #   return BitWidth.U(2 * (-value) - 1)  # ~x = -x - 1
     value *= 2
     return BitWidth.U(value if value >= 0 else ~value)
 
   @staticmethod
   def F(value):
     """Returns the `BitWidth` to encode floating point value."""
-    if struct.unpack('f', struct.pack('f', value))[0] == value:
+    if struct.unpack('<f', struct.pack('<f', value))[0] == value:
       return BitWidth.W32
     return BitWidth.W64
 
   @staticmethod
   def B(byte_width):
     return {
         1: BitWidth.W8,
@@ -91,28 +91,28 @@
 
 I = {1: 'b', 2: 'h', 4: 'i', 8: 'q'}  # Integer formats
 U = {1: 'B', 2: 'H', 4: 'I', 8: 'Q'}  # Unsigned integer formats
 F = {4: 'f', 8: 'd'}  # Floating point formats
 
 
 def _Unpack(fmt, buf):
-  return struct.unpack(fmt[len(buf)], buf)[0]
+  return struct.unpack('<%s' % fmt[len(buf)], buf)[0]
 
 
 def _UnpackVector(fmt, buf, length):
   byte_width = len(buf) // length
-  return struct.unpack('%d%s' % (length, fmt[byte_width]), buf)
+  return struct.unpack('<%d%s' % (length, fmt[byte_width]), buf)
 
 
 def _Pack(fmt, value, byte_width):
-  return struct.pack(fmt[byte_width], value)
+  return struct.pack('<%s' % fmt[byte_width], value)
 
 
 def _PackVector(fmt, values, byte_width):
-  return struct.pack('%d%s' % (len(values), fmt[byte_width]), *values)
+  return struct.pack('<%d%s' % (len(values), fmt[byte_width]), *values)
 
 
 def _Mutate(fmt, buf, value, byte_width, value_bit_width):
   if (1 << value_bit_width) <= byte_width:
     buf[:byte_width] = _Pack(fmt, value, byte_width)
     return True
   return False
@@ -724,14 +724,23 @@
       raise self._ConvertError(Type.KEY)
 
   @property
   def IsString(self):
     return self._type is Type.STRING
 
   @property
+  def AsStringBytes(self):
+    if self.IsString:
+      return String(self._Indirect(), self._byte_width).Bytes
+    elif self.IsKey:
+      return self.AsKeyBytes
+    else:
+      raise self._ConvertError(Type.STRING)
+
+  @property
   def AsString(self):
     if self.IsString:
       return str(String(self._Indirect(), self._byte_width))
     elif self.IsKey:
       return self.AsKey
     else:
       raise self._ConvertError(Type.STRING)
```

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/number_types.py` & `octoflatbuffers-24.3.25/octoflatbuffers/number_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import collections
 import struct
 
 from . import packer
+#from .compat import import_numpy, NumpyRequiredForThisFeature
+#np = import_numpy()
 np = None
 
 # For reference, see:
 # https://docs.python.org/2/library/ctypes.html#ctypes-fundamental-data-types-2
 
 # These classes could be collections.namedtuple instances, but those are new
 # in 2.6 and we want to work towards 2.5 compatability.
```

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/packer.py` & `octoflatbuffers-24.3.25/octoflatbuffers/packer.py`

 * *Files identical despite different names*

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/table.py` & `octoflatbuffers-24.3.25/octoflatbuffers/table.py`

 * *Files 13% similar despite different names*

```diff
@@ -118,21 +118,30 @@
         GetVectorAsByteArray returns a view into the byte array.
         (copied from GetVectorAsNumpy)
         """
         offset = self.Vector(off)
         length = self.VectorLen(off) # TODO: length accounts for bytewidth, right?
         return self.Bytes[offset:offset+length]
 
+    def GetArrayAsNumpy(self, flags, off, length):
+        """
+        GetArrayAsNumpy returns the array with fixed width that starts at `Vector(offset)`
+        with length `length` as a numpy array with the type specified by `flags`. The
+        array is a `view` into Bytes so modifying the returned will modify Bytes in place.
+        """
+        numpy_dtype = N.to_numpy_type(flags)
+        return encode.GetVectorAsNumpy(numpy_dtype, self.Bytes, length, off)
+
     def GetVOffsetTSlot(self, slot, d):
         """
         GetVOffsetTSlot retrieves the VOffsetT that the given vtable location
         points to. If the vtable value is zero, the default value `d`
         will be returned.
         """
 
         N.enforce_number(slot, N.VOffsetTFlags)
         N.enforce_number(d, N.VOffsetTFlags)
 
         off = self.Offset(slot)
         if off == 0:
-                return d
+            return d
         return off
```

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers/util.py` & `octoflatbuffers-24.3.25/octoflatbuffers/util.py`

 * *Files identical despite different names*

### Comparing `octoflatbuffers-2.0.8/octoflatbuffers.egg-info/PKG-INFO` & `octoflatbuffers-24.3.25/octoflatbuffers.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoflatbuffers
-Version: 2.0.8
+Version: 24.3.25
 Summary: A fork of flatbuffers used for OctoEverywhere and Homeway
 Home-page: https://github.com/QuinnDamerell/octoflatbuffers
 Author: Quinn Damerell
 Author-email: support@octoeverywhere.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/QuinnDamerell/octoflatbuffers
 Project-URL: Source, https://github.com/QuinnDamerell/octoflatbuffers
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: ../license
 
 
 # OctoFlatBuffers
 A fork of [flatbuffers](https://flatbuffers.dev/) with some special modifications. Used as the core protocol for:
 - [OctoEverywhere](https://octoeverywhere.com/?source=pypi) - Free, private, and secure remote access for OctoPrint and Klipper 3D printer.
 - [Homeway](https://homeway.io/?source=pypi) - Free, private, and secure remote access for Home Assistant.
```

### Comparing `octoflatbuffers-2.0.8/setup.py` & `octoflatbuffers-24.3.25/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,33 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import fileinput
-import os
 import re
 import sys
-from datetime import datetime
+import fileinput
 from setuptools import setup
 
-
 def _update_version_attr(new_version):
     for line in fileinput.input('octoflatbuffers/_version.py', inplace=True):
         if line.startswith('__version__'):
             line = re.sub(r'".*"', '"{}"'.format(new_version), line)
         sys.stdout.write(line)
 
 
 def version():
     # We will manually set the version to track the flatbuffer version for the most part.
     # The exception being for revision bumps we make ourselves.
-    version = "2.0.8"
+    version = "24.3.25"
     _update_version_attr(version)
     return version
 
 
 setup(
     name='octoflatbuffers',
     version=version(),
@@ -65,8 +62,8 @@
     ],
     project_urls={
         'Documentation': 'https://github.com/QuinnDamerell/octoflatbuffers',
         'Source': 'https://github.com/QuinnDamerell/octoflatbuffers',
         'OctoEverywhere': 'https://octoeverywhere.com/?source=pypi',
         'Homeway': 'https://homeway.io/?source=pypi',
     },
-)
+)
```

