# Comparing `tmp/order_book-0.6.0.tar.gz` & `tmp/order_book-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "order_book-0.6.0.tar", last modified: Wed Oct 19 22:02:09 2022, max compression
+gzip compressed data, was "order_book-0.6.1.tar", last modified: Tue Apr 23 00:05:44 2024, max compression
```

## Comparing `order_book-0.6.0.tar` & `order_book-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-19 22:02:09.872817 order_book-0.6.0/
--rw-r--r--   0 bryant     (501) staff       (20)     3073 2022-10-19 21:58:42.000000 order_book-0.6.0/CHANGES.md
--rw-r--r--   0 bryant     (501) staff       (20)    35149 2021-03-05 00:18:28.000000 order_book-0.6.0/LICENSE
--rw-r--r--   0 bryant     (501) staff       (20)       36 2021-03-05 00:18:28.000000 order_book-0.6.0/MANIFEST.in
--rw-r--r--   0 bryant     (501) staff       (20)     8183 2022-10-19 22:02:09.872479 order_book-0.6.0/PKG-INFO
--rw-r--r--   0 bryant     (501) staff       (20)     4130 2022-09-04 17:08:39.000000 order_book-0.6.0/README.md
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-19 22:02:09.870178 order_book-0.6.0/order_book.egg-info/
--rw-r--r--   0 bryant     (501) staff       (20)     8183 2022-10-19 22:02:09.000000 order_book-0.6.0/order_book.egg-info/PKG-INFO
--rw-r--r--   0 bryant     (501) staff       (20)      311 2022-10-19 22:02:09.000000 order_book-0.6.0/order_book.egg-info/SOURCES.txt
--rw-r--r--   0 bryant     (501) staff       (20)        1 2022-10-19 22:02:09.000000 order_book-0.6.0/order_book.egg-info/dependency_links.txt
--rw-r--r--   0 bryant     (501) staff       (20)       11 2022-10-19 22:02:09.000000 order_book-0.6.0/order_book.egg-info/top_level.txt
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-19 22:02:09.872056 order_book-0.6.0/orderbook/
--rw-r--r--   0 bryant     (501) staff       (20)    16525 2022-08-23 23:08:25.000000 order_book-0.6.0/orderbook/orderbook.c
--rw-r--r--   0 bryant     (501) staff       (20)     3773 2022-05-29 18:06:28.000000 order_book-0.6.0/orderbook/orderbook.h
--rw-r--r--   0 bryant     (501) staff       (20)    13095 2022-10-19 21:58:42.000000 order_book-0.6.0/orderbook/sorteddict.c
--rw-r--r--   0 bryant     (501) staff       (20)     3769 2022-10-19 21:58:42.000000 order_book-0.6.0/orderbook/sorteddict.h
--rw-r--r--   0 bryant     (501) staff       (20)     1008 2022-05-29 18:06:28.000000 order_book-0.6.0/orderbook/utils.c
--rw-r--r--   0 bryant     (501) staff       (20)     3616 2022-05-29 18:06:28.000000 order_book-0.6.0/orderbook/utils.h
--rw-r--r--   0 bryant     (501) staff       (20)       38 2022-10-19 22:02:09.872960 order_book-0.6.0/setup.cfg
--rw-r--r--   0 bryant     (501) staff       (20)     2166 2022-08-23 23:15:02.000000 order_book-0.6.0/setup.py
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-04-23 00:05:44.370636 order_book-0.6.1/
+-rw-r--r--   0 bryant     (501) staff       (20)     3234 2024-04-23 00:05:10.000000 order_book-0.6.1/CHANGES.md
+-rw-r--r--   0 bryant     (501) staff       (20)    35149 2021-03-05 00:18:28.000000 order_book-0.6.1/LICENSE
+-rw-r--r--   0 bryant     (501) staff       (20)       36 2021-03-05 00:18:28.000000 order_book-0.6.1/MANIFEST.in
+-rw-r--r--   0 bryant     (501) staff       (20)     8578 2024-04-23 00:05:44.369926 order_book-0.6.1/PKG-INFO
+-rw-r--r--   0 bryant     (501) staff       (20)     4331 2023-01-27 01:28:13.000000 order_book-0.6.1/README.md
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-04-23 00:05:44.360609 order_book-0.6.1/order_book.egg-info/
+-rw-r--r--   0 bryant     (501) staff       (20)     8578 2024-04-23 00:05:44.000000 order_book-0.6.1/order_book.egg-info/PKG-INFO
+-rw-r--r--   0 bryant     (501) staff       (20)      384 2024-04-23 00:05:44.000000 order_book-0.6.1/order_book.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant     (501) staff       (20)        1 2024-04-23 00:05:44.000000 order_book-0.6.1/order_book.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant     (501) staff       (20)       11 2024-04-23 00:05:44.000000 order_book-0.6.1/order_book.egg-info/top_level.txt
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-04-23 00:05:44.365817 order_book-0.6.1/orderbook/
+-rw-r--r--   0 bryant     (501) staff       (20)    16551 2024-04-18 17:33:03.000000 order_book-0.6.1/orderbook/orderbook.c
+-rw-r--r--   0 bryant     (501) staff       (20)     3781 2024-04-18 17:33:03.000000 order_book-0.6.1/orderbook/orderbook.h
+-rw-r--r--   0 bryant     (501) staff       (20)    12846 2024-04-18 17:33:03.000000 order_book-0.6.1/orderbook/sorteddict.c
+-rw-r--r--   0 bryant     (501) staff       (20)     3591 2024-04-18 17:33:03.000000 order_book-0.6.1/orderbook/sorteddict.h
+-rw-r--r--   0 bryant     (501) staff       (20)     1008 2024-04-18 17:33:03.000000 order_book-0.6.1/orderbook/utils.c
+-rw-r--r--   0 bryant     (501) staff       (20)     3616 2024-04-18 17:33:03.000000 order_book-0.6.1/orderbook/utils.h
+-rw-r--r--   0 bryant     (501) staff       (20)       38 2024-04-23 00:05:44.370775 order_book-0.6.1/setup.cfg
+-rw-r--r--   0 bryant     (501) staff       (20)     2218 2024-04-18 17:33:03.000000 order_book-0.6.1/setup.py
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2024-04-23 00:05:44.368739 order_book-0.6.1/tests/
+-rw-r--r--   0 bryant     (501) staff       (20)    16766 2024-04-18 17:33:03.000000 order_book-0.6.1/tests/test_checksums.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6280 2024-04-18 17:33:03.000000 order_book-0.6.1/tests/test_orderbook.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7819 2024-04-18 17:33:03.000000 order_book-0.6.1/tests/test_sorteddict.py
```

### Comparing `order_book-0.6.0/CHANGES.md` & `order_book-0.6.1/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## Changelog
 
+### 0.6.1 (2024-04-22)
+ * Update: to_list's behavior matches that of to_dict (respects max_depth, if set).
+ * Update: resolve build warnings on some compilers.
+
 ### 0.6.0 (2022-10-19)
  * Update: Drop support for python 3.7
  * Feature: to_list method
  * Bugfix: Initialize iterator correctly
 
 ### 0.5.0 (2022-08-23)
  * Bugfix: fix segmentation fault when calculating checksum on empty orderbook
```

### Comparing `order_book-0.6.0/LICENSE` & `order_book-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `order_book-0.6.0/PKG-INFO` & `order_book-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: order_book
-Version: 0.6.0
+Version: 0.6.1
 Summary: A fast orderbook implementation, in C, for Python
 Home-page: https://github.com/bmoscon/orderbook
 Author: Bryant Moscon
 Author-email: bmoscon@gmail.com
 License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Keywords: market data,trading
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -83,14 +83,22 @@
 
 # Data can be exported to a sorted dictionary
 # In Python3.7+ dictionaries remain in insertion ordering. The
 # dict returned by .to_dict() has had its keys inserted in sorted order
 print("\n\nRaw asks dictionary")
 print(ob.asks.to_dict())
 
+
+# Data can also be exported as an ordered list
+# .to_list() returns a list of (price, size) tuples
+print("Top 5 Asks")
+print(ob.asks.to_list()[:5])
+print("\nTop 5 Bids")
+print(ob.bids.to_list()[:5])
+
 ```
 
 ### Main Features
 
 * Sides maintained in correct order
 * Can perform orderbook checksums
 * Supports max depth and depth truncation
@@ -140,14 +148,18 @@
 For other performance metrics, run `performance_test.py` as well as the other performance tests in [`perf/`](perf/)
 
 
 ----
 
 ## Changelog
 
+### 0.6.1 (2024-04-22)
+ * Update: to_list's behavior matches that of to_dict (respects max_depth, if set).
+ * Update: resolve build warnings on some compilers.
+
 ### 0.6.0 (2022-10-19)
  * Update: Drop support for python 3.7
  * Feature: to_list method
  * Bugfix: Initialize iterator correctly
 
 ### 0.5.0 (2022-08-23)
  * Bugfix: fix segmentation fault when calculating checksum on empty orderbook
@@ -213,9 +225,7 @@
   * Feature: New unit tests to improve SortedDict coverage
   * Feature: Modularize files
   * Feature: Add ability to set bids/asks to dictionaries via attributes or \[ \]
   * Docs: Update README with simple usage example
 
 ### 0.0.1 (2020-12-26)
   * Initial Release
-
-
```

### Comparing `order_book-0.6.0/README.md` & `order_book-0.6.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -58,14 +58,22 @@
 
 # Data can be exported to a sorted dictionary
 # In Python3.7+ dictionaries remain in insertion ordering. The
 # dict returned by .to_dict() has had its keys inserted in sorted order
 print("\n\nRaw asks dictionary")
 print(ob.asks.to_dict())
 
+
+# Data can also be exported as an ordered list
+# .to_list() returns a list of (price, size) tuples
+print("Top 5 Asks")
+print(ob.asks.to_list()[:5])
+print("\nTop 5 Bids")
+print(ob.bids.to_list()[:5])
+
 ```
 
 ### Main Features
 
 * Sides maintained in correct order
 * Can perform orderbook checksums
 * Supports max depth and depth truncation
```

### Comparing `order_book-0.6.0/order_book.egg-info/PKG-INFO` & `order_book-0.6.1/order_book.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: order-book
-Version: 0.6.0
+Version: 0.6.1
 Summary: A fast orderbook implementation, in C, for Python
 Home-page: https://github.com/bmoscon/orderbook
 Author: Bryant Moscon
 Author-email: bmoscon@gmail.com
 License: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Keywords: market data,trading
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -83,14 +83,22 @@
 
 # Data can be exported to a sorted dictionary
 # In Python3.7+ dictionaries remain in insertion ordering. The
 # dict returned by .to_dict() has had its keys inserted in sorted order
 print("\n\nRaw asks dictionary")
 print(ob.asks.to_dict())
 
+
+# Data can also be exported as an ordered list
+# .to_list() returns a list of (price, size) tuples
+print("Top 5 Asks")
+print(ob.asks.to_list()[:5])
+print("\nTop 5 Bids")
+print(ob.bids.to_list()[:5])
+
 ```
 
 ### Main Features
 
 * Sides maintained in correct order
 * Can perform orderbook checksums
 * Supports max depth and depth truncation
@@ -140,14 +148,18 @@
 For other performance metrics, run `performance_test.py` as well as the other performance tests in [`perf/`](perf/)
 
 
 ----
 
 ## Changelog
 
+### 0.6.1 (2024-04-22)
+ * Update: to_list's behavior matches that of to_dict (respects max_depth, if set).
+ * Update: resolve build warnings on some compilers.
+
 ### 0.6.0 (2022-10-19)
  * Update: Drop support for python 3.7
  * Feature: to_list method
  * Bugfix: Initialize iterator correctly
 
 ### 0.5.0 (2022-08-23)
  * Bugfix: fix segmentation fault when calculating checksum on empty orderbook
@@ -213,9 +225,7 @@
   * Feature: New unit tests to improve SortedDict coverage
   * Feature: Modularize files
   * Feature: Add ability to set bids/asks to dictionaries via attributes or \[ \]
   * Docs: Update README with simple usage example
 
 ### 0.0.1 (2020-12-26)
   * Initial Release
-
-
```

### Comparing `order_book-0.6.0/orderbook/orderbook.c` & `order_book-0.6.1/orderbook/orderbook.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-Copyright (C) 2020-2022  Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2020-2024  Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 */
 #include "orderbook.h"
 #include "utils.h"
 
@@ -536,15 +536,15 @@
 {
     int startpos = *pos;
     if (EXPECT(str_string_builder(pydata, data, pos), 0)) {
         return -1;
     }
 
     // default 'str' formatting is wrong when the value is in scientific notation
-    if (EXPECT(memchr(&data[startpos], (char) 'E', *pos - startpos), 0)) {
+    if (EXPECT((long)memchr(&data[startpos], (char) 'E', *pos - startpos), (long)0)) {
         *pos = startpos;
         if (EXPECT(formatf_string_builder(pydata, data, pos), 0)) {
             return -1;
         }
     }
 
     return 0;
@@ -555,15 +555,15 @@
 {
     int startpos = *pos;
     if (EXPECT(str_string_builder(pydata, data, pos), 0)) {
         return -1;
     }
 
     // default 'str' formatting is wrong when the value is less than 0.0001 or in scientific notation
-    if (EXPECT(!strncmp(&data[startpos], "0.0000", 6) || memchr(&data[startpos], (char) 'E', *pos - startpos), 0)) {
+    if (EXPECT(!strncmp((const char *)&data[startpos], "0.0000", 6) || memchr(&data[startpos], (char) 'E', *pos - startpos), 0)) {
         *pos = startpos;
         if (EXPECT(floatstr_string_builder(pydata, data, pos), 0)) {
             return -1;
         }
     }
 
     return 0;
```

### Comparing `order_book-0.6.0/orderbook/orderbook.h` & `order_book-0.6.1/orderbook/orderbook.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-Copyright (C) 2020-2022  Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2020-2024  Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 */
 #ifndef __ORDERBOOK__
 #define __ORDERBOOK__
 
@@ -117,15 +117,15 @@
     .m_name = "order_book",
     .m_doc = "Orderbook data structure",
     .m_size = sizeof(OrderBookModuleState),
     .m_methods = NULL,
     .m_slots = NULL,
     .m_traverse = order_book_traverse,
     .m_clear = order_book_clear,
-    .m_free = order_book_free,
+    .m_free = (void *)order_book_free,
 };
 
 
 // Checksum Definitions
 static PyObject* calculate_checksum(const Orderbook *ob);
```

### Comparing `order_book-0.6.0/orderbook/sorteddict.c` & `order_book-0.6.1/orderbook/sorteddict.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-Copyright (C) 2020-2022  Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2020-2024  Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 */
 #include "sorteddict.h"
 #include "utils.h"
 
@@ -30,15 +30,15 @@
     if (self != NULL) {
         self->data = PyDict_New();
         if (!self->data) {
             Py_DECREF(self);
             return NULL;
         }
 
-	self->ordering = INVALID_ORDERING;
+        self->ordering = INVALID_ORDERING;
         // -1 means uninitalized
         self->iterator_index = -1;
         self->keys = NULL;
         self->dirty = false;
         self->depth = 0;
         self->truncate = false;
     }
@@ -335,43 +335,36 @@
         }
     }
 
     return ret;
 }
 
 
-PyObject* SortedDict_tolist(SortedDict *self, PyObject *args, PyObject *kwargs)
+PyObject* SortedDict_tolist(SortedDict *self, PyObject *Py_UNUSED(ignored))
 {
-    static char* keywords[] = {"n_levels", NULL};
-    
-    int n_levels = -1;
-    if (!PyArg_ParseTupleAndKeywords(args, kwargs, "|i", keywords, &n_levels)) {
-        return NULL;
-    }
 
-    int data_len = PyDict_Size(self->data);
-    // Set n_levels to data_len if n_levels is the default value
-    if (n_levels == -1 | n_levels > data_len) {
-        n_levels = data_len;
+    int len = PyDict_Size(self->data);
+    if ((self->depth > 0) && (self->depth < len)) {
+        len = self->depth;
     }
 
     if (EXPECT(PyErr_Occurred() != NULL, 0)) {
         return NULL;
     }
 
     if (EXPECT(update_keys(self), 0)) {
         return NULL;
     }
 
-    PyObject *ret = PyList_New(n_levels);
+    PyObject *ret = PyList_New(len);
     if (EXPECT(!ret, 0)) {
         return NULL;
     }
 
-    for (int i = 0; i < n_levels; ++i) {
+    for (int i = 0; i < len; ++i) {
         // new reference
         PyObject *key = PySequence_GetItem(self->keys, i);
         if (EXPECT(!key, 0)) {
             return NULL;
         }
 
         // borrowed reference
@@ -494,15 +487,15 @@
 }
 
 /* iterator methods */
 PyObject *SortedDict_getiter(SortedDict *self)
 {
     Py_INCREF(self);
     self->iterator_index = -1;
-    return self;
+    return (PyObject *)self;
 }
 
 PyObject *SortedDict_next(SortedDict *self)
 {
     if (self->iterator_index == -1) {
         self->iterator_index = 0;
```

### Comparing `order_book-0.6.0/orderbook/sorteddict.h` & `order_book-0.6.1/orderbook/sorteddict.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-Copyright (C) 2020-2022  Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2020-2024  Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 */
 #ifndef __SORTEDDICT__
 #define __SORTEDDICT__
 
@@ -38,15 +38,15 @@
 PyObject *SortedDict_new(PyTypeObject *type, PyObject *args, PyObject *kwds);
 int SortedDict_init(SortedDict *self, PyObject *args, PyObject *kwds);
 
 
 PyObject* SortedDict_keys(SortedDict *self, PyObject *Py_UNUSED(ignored));
 PyObject* SortedDict_index(SortedDict *self, PyObject *index);
 PyObject* SortedDict_todict(SortedDict *self, PyObject *unused, PyObject *kwargs);
-PyObject* SortedDict_tolist(SortedDict *self, PyObject *args, PyObject *kwargs);
+PyObject* SortedDict_tolist(SortedDict *self, PyObject *Py_UNUSED(ignored));
 PyObject* SortedDict_truncate(SortedDict *self, PyObject *Py_UNUSED(ignored));
 
 Py_ssize_t SortedDict_len(const SortedDict *self);
 PyObject *SortedDict_getitem(SortedDict *self, PyObject *key);
 int SortedDict_setitem(SortedDict *self, PyObject *key, PyObject *value);
 
 int SortedDict_contains(const SortedDict *self, PyObject *value);
@@ -66,15 +66,15 @@
 
 // SortedDict methods
 static PyMethodDef SortedDict_methods[] = {
     {"keys", (PyCFunction) SortedDict_keys, METH_NOARGS, "return a list of keys in the sorted dictionary"},
     {"index", (PyCFunction) SortedDict_index, METH_O, "return a key, value tuple at index N"},
     {"truncate", (PyCFunction) SortedDict_truncate, METH_NOARGS, "truncate to length max_depth"},
     {"to_dict", (PyCFunction) SortedDict_todict, METH_VARARGS | METH_KEYWORDS, "return a python dictionary, sorted by keys"},
-    {"to_list", (PyCFunction) SortedDict_tolist, METH_VARARGS | METH_KEYWORDS, "return a list of key, value tuple with length specified in input argument. if no argument is passed or the argument is larger than length of self->data, return items with length of self->data."},
+    {"to_list", (PyCFunction) SortedDict_tolist, METH_NOARGS, "return a list of key, value tuples."},
     {NULL}
 };
 
 
 // Sorted Dictionary Type Setup
 static PyMappingMethods SortedDict_mapping = {
 	(lenfunc)SortedDict_len,
```

### Comparing `order_book-0.6.0/orderbook/utils.c` & `order_book-0.6.1/orderbook/utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-Copyright (C) 2020-2022  Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2020-2024  Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 */
 #include <string.h>
 #include <stdint.h>
 #include "utils.h"
```

### Comparing `order_book-0.6.0/orderbook/utils.h` & `order_book-0.6.1/orderbook/utils.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /*
-Copyright (C) 2020-2022  Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2020-2024  Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 */
 #ifndef __UTILS__
 #define __UTILS__
```

### Comparing `order_book-0.6.0/setup.py` & `order_book-0.6.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2020-2022  Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2020-2024  Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import glob
 import os
 from os import path
@@ -31,15 +31,15 @@
         import pytest
         errno = pytest.main(['tests/'])
         sys.exit(errno)
 
 
 setup(
     name='order_book',
-    version='0.6.0',
+    version='0.6.1',
     author="Bryant Moscon",
     author_email="bmoscon@gmail.com",
     description="A fast orderbook implementation, in C, for Python",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     keywords=["market data", "trading"],
     url="https://github.com/bmoscon/orderbook",
@@ -49,17 +49,18 @@
     tests_require=["pytest", "requests", "sortedcontainers"],
     cmdclass={'test': Test},
     classifiers=[
         "Intended Audience :: Developers",
         "Development Status :: 3 - Alpha",
         "Programming Language :: C",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Operating System :: MacOS",
         "Operating System :: POSIX :: Linux",
         "Operating System :: POSIX"
     ],
 )
```

