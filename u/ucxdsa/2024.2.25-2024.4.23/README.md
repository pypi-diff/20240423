# Comparing `tmp/ucxdsa-2024.2.25.tar.gz` & `tmp/ucxdsa-2024.4.23.tar.gz`

## Comparing `ucxdsa-2024.2.25.tar` & `ucxdsa-2024.4.23.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa.zip
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/test.ipynb
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/todo.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/__init__.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/array.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/doublylinkedlist.py
--rw-r--r--   0        0        0    18828 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/graph.py
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/hashtable.py
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/heap.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/huffman.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/pretty_print.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/queue.py
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/singlylinkedlist.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/sorttools.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/stack.py
--rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/tree.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa/trie.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa.egg-info/PKG-INFO
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/dsa.egg-info/top_level.txt
--rw-r--r--   0        0        0    35587 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/array.html
--rw-r--r--   0        0        0    22386 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/doublylinkedlist.html
--rw-r--r--   0        0        0    57112 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/graph.html
--rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/hashtable.html
--rw-r--r--   0        0        0    20103 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/heap.html
--rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/huffman.html
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/index.html
--rw-r--r--   0        0        0    12664 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/pretty_print.html
--rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/queue.html
--rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/singlylinkedlist.html
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/sorttools.html
--rw-r--r--   0        0        0    24822 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/stack.html
--rw-r--r--   0        0        0    18397 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/tree.html
--rw-r--r--   0        0        0    19308 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/html/dsa/trie.html
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/ucxdsa.egg-info/PKG-INFO
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/ucxdsa.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/ucxdsa.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/src/ucxdsa.egg-info/top_level.txt
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_array.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_doublylinkedlist.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_graph_list.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_graph_matrix.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_hash.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_heap.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_huffman.py
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_linkedlist.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_pretty_print.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_queue.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_stack.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_tree.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/tests/test_trie.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/LICENSE
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/README.md
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/pyproject.toml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ucxdsa-2024.2.25/PKG-INFO
+-rw-r--r--   0        0        0    26445 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.zip
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/test.ipynb
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/todo.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/__init__.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/array.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/doublylinkedlist.py
+-rw-r--r--   0        0        0    18828 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/graph.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/hashtable.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/heap.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/huffman.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/pretty_print.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/queue.py
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/singlylinkedlist.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/sorttools.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/stack.py
+-rw-r--r--   0        0        0     4155 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/tree.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa/trie.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/dsa.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35587 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/array.html
+-rw-r--r--   0        0        0    22386 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/doublylinkedlist.html
+-rw-r--r--   0        0        0    57112 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/graph.html
+-rw-r--r--   0        0        0    14870 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/hashtable.html
+-rw-r--r--   0        0        0    20103 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/heap.html
+-rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/huffman.html
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/index.html
+-rw-r--r--   0        0        0    12664 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/pretty_print.html
+-rw-r--r--   0        0        0    22281 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/queue.html
+-rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/singlylinkedlist.html
+-rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/sorttools.html
+-rw-r--r--   0        0        0    24822 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/stack.html
+-rw-r--r--   0        0        0    18397 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/tree.html
+-rw-r--r--   0        0        0    19308 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/html/dsa/trie.html
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/src/ucxdsa.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_array.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_doublylinkedlist.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_graph_list.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_graph_matrix.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_hash.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_heap.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_huffman.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_linkedlist.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_pretty_print.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_queue.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_stack.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_tree.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/tests/test_trie.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/LICENSE
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/README.md
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/pyproject.toml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ucxdsa-2024.4.23/PKG-INFO
```

### Comparing `ucxdsa-2024.2.25/src/dsa.zip` & `ucxdsa-2024.4.23/src/dsa.zip`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/test.ipynb` & `ucxdsa-2024.4.23/src/test.ipynb`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/array.py` & `ucxdsa-2024.4.23/src/dsa/array.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/doublylinkedlist.py` & `ucxdsa-2024.4.23/src/dsa/doublylinkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/graph.py` & `ucxdsa-2024.4.23/src/dsa/graph.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/hashtable.py` & `ucxdsa-2024.4.23/src/dsa/hashtable.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/heap.py` & `ucxdsa-2024.4.23/src/dsa/heap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 class Heap:
     """ 
-    A max heap implementation in Python
+    A heap implementation in Python
+
+    Args:
+        maxheap: return a max-heap if True  (default), otherwise return a min-heap
     """
-    def __init__(self):
+    def __init__(self, maxheap=True):
         self._array = []
+
+        # comparator determines the order of the insertion by flipping its sign if min-heap 
+        if maxheap:
+            self.comparator = lambda x: x
+        else:
+            self.comparator = lambda x: -x
     
     def root(self):
         """
         Get the root value.
 
         Returns:
         The root node's value. None if count is 0.
         """
         if self.count() == 0:
             return None
 
         return self._array[0]
     
+    def peek(self):
+        """
+        Get the max value if max-heap and min value if min-heap.
+
+        Returns:
+        Get the max value if max-heap and min value if min-heap.
+        """
+        return self.root()
+
     def last(self):
         """
         Get the last node of the heap.
 
         Returns:
         The last node's value. None if count is 0.
         """
@@ -117,15 +135,15 @@
         """
         Perform heapify up starting at a given index.
 
         Args:
             index: starting index  
         """
         parent_index = self.parent_index(index)
-        while self.has_parent(index) and self._array[index] > self._array[parent_index]:
+        while self.has_parent(index) and self.comparator(self._array[index]) > self.comparator(self._array[parent_index]):
             self._array[index], self._array[parent_index] = self._array[parent_index], self._array[index]
             index = parent_index
             parent_index = self.parent_index(index)
 
     def pop(self):
         """
         Get the value of the root node and remove it from the heap.
@@ -150,20 +168,19 @@
         Perform heapify down starting at a given index.
 
         Args:
             index: starting index  
         """
         while self.has_left(index):
             higher_index = self.left_index(index)
-
             right_index = self.right_index(index)
-            if self.has_right(index) and self._array[right_index] > self._array[higher_index]:
+            if self.has_right(index) and self.comparator(self._array[right_index]) > self.comparator(self._array[higher_index]):
                 higher_index = right_index
             
-            if self._array[index] > self._array[higher_index]:
+            if self.comparator(self._array[index]) > self.comparator(self._array[higher_index]):
                 break
             else:
                 self._array[index], self._array[higher_index] = self._array[higher_index], self._array[index]
                 
             index = higher_index
     
     def enumerate(self):
```

### Comparing `ucxdsa-2024.2.25/src/dsa/huffman.py` & `ucxdsa-2024.4.23/src/dsa/huffman.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/pretty_print.py` & `ucxdsa-2024.4.23/src/dsa/pretty_print.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/queue.py` & `ucxdsa-2024.4.23/src/dsa/queue.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/singlylinkedlist.py` & `ucxdsa-2024.4.23/src/dsa/singlylinkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/sorttools.py` & `ucxdsa-2024.4.23/src/dsa/sorttools.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/stack.py` & `ucxdsa-2024.4.23/src/dsa/stack.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/tree.py` & `ucxdsa-2024.4.23/src/dsa/tree.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa/trie.py` & `ucxdsa-2024.4.23/src/dsa/trie.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/dsa.egg-info/PKG-INFO` & `ucxdsa-2024.4.23/src/dsa.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/array.html` & `ucxdsa-2024.4.23/src/html/dsa/array.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/doublylinkedlist.html` & `ucxdsa-2024.4.23/src/html/dsa/doublylinkedlist.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/graph.html` & `ucxdsa-2024.4.23/src/html/dsa/graph.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/hashtable.html` & `ucxdsa-2024.4.23/src/html/dsa/hashtable.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/heap.html` & `ucxdsa-2024.4.23/src/html/dsa/heap.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/huffman.html` & `ucxdsa-2024.4.23/src/html/dsa/huffman.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/index.html` & `ucxdsa-2024.4.23/src/html/dsa/index.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/pretty_print.html` & `ucxdsa-2024.4.23/src/html/dsa/pretty_print.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/queue.html` & `ucxdsa-2024.4.23/src/html/dsa/queue.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/singlylinkedlist.html` & `ucxdsa-2024.4.23/src/html/dsa/singlylinkedlist.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/sorttools.html` & `ucxdsa-2024.4.23/src/html/dsa/sorttools.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/stack.html` & `ucxdsa-2024.4.23/src/html/dsa/stack.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/tree.html` & `ucxdsa-2024.4.23/src/html/dsa/tree.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/html/dsa/trie.html` & `ucxdsa-2024.4.23/src/html/dsa/trie.html`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/src/ucxdsa.egg-info/PKG-INFO` & `ucxdsa-2024.4.23/src/ucxdsa.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_array.py` & `ucxdsa-2024.4.23/tests/test_array.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_doublylinkedlist.py` & `ucxdsa-2024.4.23/tests/test_doublylinkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_graph_list.py` & `ucxdsa-2024.4.23/tests/test_graph_list.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_graph_matrix.py` & `ucxdsa-2024.4.23/tests/test_graph_matrix.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_hash.py` & `ucxdsa-2024.4.23/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_heap.py` & `ucxdsa-2024.4.23/tests/test_heap.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,45 @@
 import unittest
 
 from dsa.heap import Heap
 
 class TestHeap(unittest.TestCase):
     def test_create(self):
-        h = Heap()
-        self.assertEqual(h.count(), 0)
+        mxh = Heap()
+        mnh = Heap(maxheap=False)
+        self.assertEqual(mxh.count(), 0)
+        self.assertEqual(mnh.count(), 0)
     
     def test_add(self):
-        h = Heap()
+        mxh = Heap()
+        mnh = Heap(maxheap=False)
 
         for _ in range(20):
-            h.insert(_)
-        self.assertEqual(h.count(), 20)
+            mxh.insert(_)
+            mnh.insert(_)
+
+        self.assertEqual(mxh.count(), 20)
+        self.assertEqual(mxh.peek(), 19)
+        self.assertEqual(mnh.count(), 20)
+        self.assertEqual(mnh.peek(), 0)
 
     def test_delete(self):
-        h = Heap()
+        mxh = Heap()
+        mnh = Heap(maxheap=False)
 
         for _ in range(20):
-            h.insert(_)
+            mxh.insert(_)
+            mnh.insert(_)
 
         i = 19
-        while not h.is_empty():
-            v = h.pop()
+        while not mxh.is_empty():
+            v = mxh.pop()
             self.assertEqual(v, i)
             i = i - 1
+        self.assertTrue(mxh.is_empty())
 
-        self.assertTrue(h.is_empty())
+        i = 0
+        while not mnh.is_empty():
+            v = mnh.pop()
+            self.assertEqual(v, i)
+            i += 1
+        self.assertTrue(mnh.is_empty())
```

### Comparing `ucxdsa-2024.2.25/tests/test_huffman.py` & `ucxdsa-2024.4.23/tests/test_huffman.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_linkedlist.py` & `ucxdsa-2024.4.23/tests/test_linkedlist.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_pretty_print.py` & `ucxdsa-2024.4.23/tests/test_pretty_print.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_queue.py` & `ucxdsa-2024.4.23/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_stack.py` & `ucxdsa-2024.4.23/tests/test_stack.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_tree.py` & `ucxdsa-2024.4.23/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/tests/test_trie.py` & `ucxdsa-2024.4.23/tests/test_trie.py`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/LICENSE` & `ucxdsa-2024.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `ucxdsa-2024.2.25/pyproject.toml` & `ucxdsa-2024.4.23/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ucxdsa"
-version = "2024.02.25"
+version = "2024.04.23"
 authors = [
   { name="Carl Limsico", email="limsico@berkeley.edu" },
 ]
 description = "Data Structures and Algorithms Source Code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ucxdsa-2024.2.25/PKG-INFO` & `ucxdsa-2024.4.23/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ucxdsa
-Version: 2024.2.25
+Version: 2024.4.23
 Summary: Data Structures and Algorithms Source Code
 Author-email: Carl Limsico <limsico@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

