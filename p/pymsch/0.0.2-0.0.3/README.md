# Comparing `tmp/pymsch-0.0.2.tar.gz` & `tmp/pymsch-0.0.3.tar.gz`

## Comparing `pymsch-0.0.2.tar` & `pymsch-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    36727 2020-02-02 00:00:00.000000 pymsch-0.0.2/src/pymsch/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pymsch-0.0.2/LICENSE
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymsch-0.0.2/README.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 pymsch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pymsch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    36890 2020-02-02 00:00:00.000000 pymsch-0.0.3/src/pymsch/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pymsch-0.0.3/LICENSE
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 pymsch-0.0.3/README.md
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 pymsch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pymsch-0.0.3/PKG-INFO
```

### Comparing `pymsch-0.0.2/src/pymsch/__init__.py` & `pymsch-0.0.3/src/pymsch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
- 
- 
 import struct, zlib, os, base64, pyperclip, math
 from enum import Enum
 
 class Block:
     def __init__(self, block, x, y, config, rotation):
         self.block = block
         self.x = x 
@@ -21,66 +19,68 @@
 
     def __init__(self):
         self.tiles = []
         self.tags = {}
         self.types_list = []
 
     def add_block(self, tile: Block):
-        self.tiles.append(tile)
-        if(tile.get_block_name() not in self.types_list):
-            self.types_list.append(tile.get_block_name())
+        if(len(self.types_list) >= 127 and tile.get_block_name() not in self.types_list):
+            raise Exception("Failed to add block (total block types can't exceed 127)")
+        else:
+            self.tiles.append(tile)
+            if(tile.get_block_name() not in self.types_list):
+                self.types_list.append(tile.get_block_name())
 
     def add_schem(self, schem: Schematic, x: int, y: int):
         offset_x = 1000000
         offset_y = 1000000
 
         for block in self.tiles:
             offset_x = min(offset_x, block.x + (block.block.value.size // 2))
             offset_y = min(offset_y, block.y + (block.block.value.size // 2))
         offset_x *= -1
         offset_y *= -1
 
         for block in self.tiles:
-            block.x = block.x + offset_x + 1
-            block.y = block.y + offset_y + 1
+            block.x = block.x + offset_x
+            block.y = block.y + offset_y
 
         for tile in list(schem.tiles):
             self.add_block(Block(tile.block, tile.x + x, tile.y + y, tile.config, tile.rotation))
 
     def write(self):
         
         width = -1000000
         height = -1000000
         offset_x = 1000000
         offset_y = 1000000
 
         for block in self.tiles:
-            offset_x = min(offset_x, block.x + (block.block.value.size // 2))
-            offset_y = min(offset_y, block.y + (block.block.value.size // 2))
+            offset_x = min(offset_x, block.x - (block.block.value.size // 2))
+            offset_y = min(offset_y, block.y - (block.block.value.size // 2))
             width = max(width, block.x + (block.block.value.size // 2) + 1)
             height = max(height, block.y + (block.block.value.size // 2) + 1)
         offset_x *= -1
         offset_y *= -1
-        width += offset_x + 1
-        height += offset_y + 1
+        width += offset_x
+        height += offset_y
 
         for block in self.tiles:
-            block.x = block.x + offset_x + 1
-            block.y = block.y + offset_y + 1
+            block.x = block.x + offset_x
+            block.y = block.y + offset_y
 
         buffer = ByteBuffer()
 
         buffer.writeShort(width)
         buffer.writeShort(height)
 
         buffer.writeByte(len(self.tags))
         for k, v in self.tags.items():
             buffer.writeUTF(k)
             buffer.writeUTF(v)
-            
         buffer.writeByte(len(self.types_list)) #dictionary
         for t in self.types_list:
             buffer.writeUTF(t)
         
         buffer.writeInt(len(self.tiles))
         for t in self.tiles:
             buffer.writeByte(self.types_list.index(t.get_block_name())) #dictionary index
```

### Comparing `pymsch-0.0.2/LICENSE` & `pymsch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymsch-0.0.2/PKG-INFO` & `pymsch-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pymsch
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for creating mindustry schematic files
 Author: skyethefoxyfox
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

