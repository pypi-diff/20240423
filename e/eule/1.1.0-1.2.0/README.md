# Comparing `tmp/eule-1.1.0.tar.gz` & `tmp/eule-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eule-1.1.0.tar", max compression
+gzip compressed data, was "eule-1.2.0.tar", last modified: Mon Apr 22 22:25:25 2024, max compression
```

## Comparing `eule-1.1.0.tar` & `eule-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,30 @@
--rw-r--r--   0        0        0     1065 2023-02-27 21:15:10.623533 eule-1.1.0/LICENSE
--rw-r--r--   0        0        0     2949 2023-11-05 12:03:40.178468 eule-1.1.0/README.md
--rw-r--r--   0        0        0      238 2023-11-21 19:43:04.683984 eule-1.1.0/eule/__init__.py
--rw-r--r--   0        0        0     9443 2023-11-21 17:46:12.640153 eule-1.1.0/eule/core.py
--rw-r--r--   0        0        0      936 2023-11-21 17:15:28.702937 eule-1.1.0/eule/operations.py
--rw-r--r--   0        0        0     2124 2023-11-21 18:06:56.095669 eule-1.1.0/eule/utils.py
--rw-r--r--   0        0        0      663 2023-11-21 18:06:56.095669 eule-1.1.0/eule/validators.py
--rw-r--r--   0        0        0     1358 2023-11-21 19:43:26.728047 eule-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 eule-1.1.0/PKG-INFO
+drwxrwxr-x   0 brunolnetto  (1000) brunolnetto  (1000)        0 2024-04-22 22:25:25.114157 eule-1.2.0/
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     1065 2024-04-20 15:11:01.000000 eule-1.2.0/LICENSE
+-rw-r--r--   0 brunolnetto  (1000) brunolnetto  (1000)     3561 2024-04-22 22:25:25.114157 eule-1.2.0/PKG-INFO
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     3101 2024-04-20 15:11:01.000000 eule-1.2.0/README.md
+drwxrwxr-x   0 brunolnetto  (1000) brunolnetto  (1000)        0 2024-04-22 22:25:25.114157 eule-1.2.0/eule/
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)      238 2024-04-20 23:22:30.000000 eule-1.2.0/eule/__init__.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)    10173 2024-04-20 22:13:31.000000 eule-1.2.0/eule/core.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     1460 2024-04-20 23:22:13.000000 eule-1.2.0/eule/operations.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)      244 2024-04-20 22:10:54.000000 eule-1.2.0/eule/types.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     3878 2024-04-20 23:22:13.000000 eule-1.2.0/eule/utils.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)      946 2024-04-20 23:22:13.000000 eule-1.2.0/eule/validators.py
+drwxrwxr-x   0 brunolnetto  (1000) brunolnetto  (1000)        0 2024-04-22 22:25:25.114157 eule-1.2.0/eule.egg-info/
+-rw-r--r--   0 brunolnetto  (1000) brunolnetto  (1000)     3561 2024-04-22 22:25:25.000000 eule-1.2.0/eule.egg-info/PKG-INFO
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)      435 2024-04-22 22:25:25.000000 eule-1.2.0/eule.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)        1 2024-04-22 22:25:25.000000 eule-1.2.0/eule.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)      102 2024-04-22 22:25:25.000000 eule-1.2.0/eule.egg-info/requires.txt
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)       20 2024-04-22 22:25:25.000000 eule-1.2.0/eule.egg-info/top_level.txt
+drwxrwxr-x   0 brunolnetto  (1000) brunolnetto  (1000)        0 2024-04-22 22:25:25.114157 eule-1.2.0/examples/
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)        0 2024-04-20 15:11:01.000000 eule-1.2.0/examples/__init__.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)      335 2024-04-20 15:11:01.000000 eule-1.2.0/examples/example.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     1363 2024-04-20 22:24:31.000000 eule-1.2.0/pyproject.toml
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)       38 2024-04-22 22:25:25.114157 eule-1.2.0/setup.cfg
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     1187 2024-04-22 22:25:23.000000 eule-1.2.0/setup.py
+drwxrwxr-x   0 brunolnetto  (1000) brunolnetto  (1000)        0 2024-04-22 22:25:25.114157 eule-1.2.0/tests/
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)       70 2024-04-20 15:11:01.000000 eule-1.2.0/tests/__init__.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     2070 2024-04-20 21:41:56.000000 eule-1.2.0/tests/conftest.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     1830 2024-04-20 23:22:13.000000 eule-1.2.0/tests/fixtures.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     6013 2024-04-20 21:55:27.000000 eule-1.2.0/tests/test_core.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)      522 2024-04-20 20:21:01.000000 eule-1.2.0/tests/test_operations.py
+-rw-rw-r--   0 brunolnetto  (1000) brunolnetto  (1000)     1754 2024-04-20 23:22:13.000000 eule-1.2.0/tests/test_utils.py
```

### Comparing `eule-1.1.0/LICENSE` & `eule-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eule-1.1.0/README.md` & `eule-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,22 +51,22 @@
 
 euler_diagram = euler(sets)
 euler_keys = euler_keys(sets)
 euler_boundaries = euler_boundaries(sets)
 euler_instance=Euler(sets)
 
 # Euler dictionary:
-# {'a,b': [2], 'b,c': [4], 'a,b,c,d': [3], 'c,d': [5], 'd': [6], 'a': [1]}
+# {('a', 'b'): [2], ('b', 'c'): [4], ('a', 'b', 'c', 'd'): [3], ('c', 'd'): [5], ('d', ): [6], ('a', ): [1]}
 print(euler_diagram)
 print(euler_instance.as_dict())
 
 print('\n')
 
 # Euler keys list:
-# ['a,b', 'b,c', 'a,b,c,d', 'c,d', 'd', 'a']
+# [('a', 'b'), ('b', 'c'), ('a', 'b', 'c', d'), ('c', 'd'), ('d', ), ('a', )]
 print(euler_keys)
 print(euler_instance.euler_keys())
 
 print('\n')
 
 # Euler boundaries dictionary:
 # {
@@ -100,12 +100,13 @@
 print(euler_instance[('a', )])
 print(euler_instance[('a', 'b', )])
 print(euler_instance[('a', 'b', 'c',)])
 
 print('\n')
 
 # Euler instance remove_key:
+# {('b', 'c'): [4], ('c', 'd'): [5], ('b', 'c', 'd'): [3], ('d',): [6], ('b',): [2]}
 euler_instance.remove_key('a')
 print(euler_instance.as_dict())
 ```
 
 </details>
```

### Comparing `eule-1.1.0/eule/core.py` & `eule-1.2.0/eule/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,89 @@
 """Main module."""
+from typing import List, Dict, Union
 
 from copy import deepcopy
 from warnings import warn
 from reprlib import repr
 
-from .utils import update_tuple, clear, tuplify
-from .operations import union, difference, intersection
-from .validators import validate_euler_generator_input
-
-def euler_generator(sets):
+from .utils import \
+    ordered_tuplify, \
+    update_ordered_tuple, \
+    cleared_set_keys
+from .operations import \
+    union, \
+    difference, \
+    intersection
+from .validators import \
+    validate_euler_generator_input
+from .types import SetsType, KeyType
+
+def euler_generator(
+    sets: SetsType
+):
     """This generator function returns each tuple (key, elems) of the
     Euler diagram in a generator-wise fashion systematic:
 
     1. Begin with the available `sets` and their exclusive elements;
-    2. Compute complementary elements to current key-set;
-    3. In case complementary set-keys AND current set content are not empty,
-    continue; Otherwise, go to next key-set;
-    4. Find the euler diagram on complementary sets;
-    5. Compute exclusive combination elements;
-    6. In case there are exclusive elements to combination: yield exclusive
-    scombination elements; Remove exclusive combination elements from current key-set.
+    2. Compute complementary elements to the current key-set;
+    3. In case complementary set-keys AND current set content are not empty, continue; 
+    4. Otherwise, go to the next key-set;
+    5. Find the euler diagram on complementary sets;
+    6. Compute exclusive combination elements;
+    7. In case there are exclusive elements to the combination: yield exclusive
+       combination elements; Remove exclusive combination elements from the current key-set.
 
     :param dict sets: array/dict of arrays
     :returns: (key, euler_set) tuple of given sets
     :rtype: tuple
     """
+
+    # Deep copy of sets and validates for List case
     sets_ = deepcopy(sets)
     sets_ = validate_euler_generator_input(sets_)
-
+    
     # Only a set
     if len(sets_.keys()) == 1:
         comb_key = list(sets_.keys())[0]
         comb_elements = list(sets_.values())[0]
-        yield ((comb_key), comb_elements)
+        yield ((comb_key, ), comb_elements)
 
     else:
         # Sets with non-empty elements
-        set_keys = clear(sets_)
+        set_keys = cleared_set_keys(sets_)
 
         # Traverse the combination lattice
         for set_key in set_keys:
-            compl_sets_keys = difference(set_keys, [set_key])
+            other_keys = difference(set_keys, [set_key])
 
             # There are still sets to analyze
-            if len(compl_sets_keys) != 0 and len(sets[set_key]) != 0:
+            this_key_set = sets_[set_key]
+            
+            are_sets_still = len(other_keys) != 0 and \
+                             len(this_key_set) != 0
+            
+            if are_sets_still:
                 # Complementary sets
-                csets = {cset_key: sets_[cset_key] for cset_key in compl_sets_keys}
+                csets = {
+                    cset_key: sets_[cset_key] 
+                    for cset_key in other_keys
+                }
 
                 # Instrospective recursion: Exclusive combination elements
                 for euler_tuple, celements in euler_generator(csets):
-
+                    
                     # Remove current set_key elements
-                    comb_elems = difference(celements, sets_[set_key])
+                    this_key_set = sets_[set_key]
+                    
+                    comb_elems = difference(celements, this_key_set)
 
                     # Non-empty combination exclusivity case
                     if len(comb_elems) != 0:
                         # Sort keys to assure deterministic behavior
-                        sorted_comb_key = tuplify(sorted(tuplify(euler_tuple)))
+                        sorted_comb_key = ordered_tuplify(euler_tuple)
 
                         # 1. Exclusive elements respective complementary keys
                         yield (sorted_comb_key, comb_elems)
 
                         # Remove comb_elems elements from its original sets
                         for euler_set_key in sorted_comb_key:
                             sets_[euler_set_key] = difference(sets_[euler_set_key], comb_elems)
@@ -69,29 +92,29 @@
 
                     # Retrieve intersection elements
                     comb_elems = intersection(celements, sets[set_key])
 
                     # Non-empty intersection set
                     if len(comb_elems) != 0:
                         # Sort keys to assure deterministic behavior
-                        comb_key = tuplify(sorted(update_tuple(euler_tuple, set_key)))
+                        comb_key = update_ordered_tuple(euler_tuple, set_key)
 
                         # 2. Intersection of analysis element and exclusive group:
                         yield (comb_key, comb_elems)
 
                         # Remove intersection elements from current key-set and complementary sets
                         for euler_set_key in comb_key:
                             sets_[euler_set_key] = difference(sets_[euler_set_key], comb_elems)
 
                         sets_[set_key] = difference(sets_[set_key], comb_elems)
 
                     else:
                         pass
 
-                    set_keys = clear(sets_)
+                    set_keys = cleared_set_keys(sets_)
 
                 if len(sets_[set_key]) != 0:
                     # Load combination key
                     comb_key = (set_key, )
                     comb_elems = sets_[set_key]
 
                     # 3. Remaining exclusive elements
@@ -99,27 +122,31 @@
 
                     # Remove remaining set elements
                     sets_[set_key] = []
 
                 else:
                     pass
 
-                set_keys = clear(sets_)
+                set_keys = cleared_set_keys(sets_)
 
 
-def euler(sets):
+def euler(
+    sets: SetsType
+):
     """Euler diagram dictionary of set-dictionary of non-repetitive elements
 
     :param dict sets: array/dict of arrays
     :returns: euler sets
     :rtype: dict
     """
     return dict(euler_generator(sets))
 
-def euler_keys(sets):
+def euler_keys(
+    sets: SetsType
+):
     """Euler diagram keys
 
     :param dict sets: array/dict of arrays
     :returns: euler sets keys
     :rtype: list
     """
     return list(euler(sets).keys())
@@ -136,33 +163,38 @@
     eulerSetsKeys = euler_keys(sets)
 
     boundaries = dict(map(lambda key: (key, []), setsKeys))
 
     for setKey in setsKeys:
         for eulerSetKeys in eulerSetsKeys:
             if setKey in eulerSetKeys:
-                boundaries[setKey] = union(boundaries[setKey], difference(eulerSetKeys, [setKey]))
-
-    return {setKey: sorted(neighborsKeys) for setKey, neighborsKeys in boundaries.items()}
+                this_boundaries = boundaries[setKey]
+                ekeys_not_this = difference(eulerSetKeys, [setKey])
+                boundaries[setKey] = union(this_boundaries, ekeys_not_this)
+
+    return {\
+        setKey: sorted(neighborsKeys) \
+        for setKey, neighborsKeys in boundaries.items()\
+    }
 
 class Euler:
-    def __init__(self, sets):
+    def __init__(self, sets: Union[List, Dict]):
         """
         Initialize an Euler object.
 
         Parameters:
         sets (dict): A dictionary containing sets indexed by keys.
 
         This constructor makes a deep copy of the input sets and computes
         the Euler set representation.
         """
         self.sets=deepcopy(sets)
         self.esets=euler(sets)
 
-    def __getitem__(self, keys):
+    def __getitem__(self, keys: KeyType):
         """
         Get the elements from the sets associated with the specified keys.
 
         Parameters:
         keys (tuple or str): The key or keys for accessing the sets.
 
         Returns:
@@ -181,15 +213,15 @@
                 raise KeyError(keys)
 
         else:
             elements=[]
             try:
                 for key in keys:
                     elements=union(self.sets[key], elements)
-
+                
                 return elements
             except KeyError:
                 keys=str(keys)
                 header=f'The keys must be among keys: ({keys}).'
 
                 msg=f'{header}'
```

### Comparing `eule-1.1.0/eule/validators.py` & `eule-1.2.0/eule/validators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,37 @@
-from .utils import uniq, reduc
 from warnings import warn
 
-def validate_euler_generator_input(sets_):
+from .utils import reduc, uniq, sequence_to_set
+from .types import SetsType
+
+def validate_euler_generator_input(
+    sets_: SetsType
+):  
+    """This function validates the input for euler_generator
+
+    :param dict sets_: dictionary with sets
+    :returns: validated sets
+    :rtype: dict
+    """
+    
     # There are no sets
     if not isinstance(sets_, (list, dict)):
         msg_1 = 'Ill-conditioned input.'
         msg_2 = 'It must be either a dict or array of arrays object!'
         raise TypeError(msg_1 + msg_2)
 
     is_unique_set_arr = [
-        len(uniq(values)) == len(values) for values in sets_.values()
+        len(sequence_to_set(values)) == len(values) 
+        for values in sets_.values()
     ]
 
     def and_map(a, b):
         return (a and b)
 
     if not reduc(and_map, is_unique_set_arr, True):
         warn('Each array MUST NOT have duplicates')
-        sets_ = {key: uniq(values) for key, values in sets_.items()}
+        sets_ = {
+            key: uniq(values)
+            for key, values in sets_.items()
+        }
 
     return sets_
```

### Comparing `eule-1.1.0/pyproject.toml` & `eule-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eule"
-version = "1.1.0"
+version = "1.2.0"
 description = "Euler diagrams in python"
 authors = ["Bruno Peixoto <brunolnetto@gmail.com>"]
 license = "MIT license"
 readme = "README.md"
 packages = [{include = "eule"}]
 homepage = "https://pypi.org/project/eule/"
 repository = "https://github.com/trouchet/eule"
@@ -28,15 +28,15 @@
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^6.0.0"
 sphinxcontrib-websupport = "^1.2.4"
 sphinxcontrib-serializinghtml = "^1.1.5"
 ruff = "^0.0.217"
 pre-commit = "^2.20.0"
-black = "^22.12.0"
+black = ">=22.12,<25.0"
 coverage = "^7.0"
 tox = "^4.0.19"
 flake8 = "^6.0.0"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-watch = "^4.2.0"
 pylint = "^2.15.9"
```

