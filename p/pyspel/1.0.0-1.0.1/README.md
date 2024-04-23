# Comparing `tmp/pyspel-1.0.0.tar.gz` & `tmp/pyspel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyspel-1.0.0.tar", last modified: Thu Jan 13 17:09:21 2022, max compression
+gzip compressed data, was "pyspel-1.0.1.tar", last modified: Tue Apr 23 20:05:49 2024, max compression
```

## Comparing `pyspel-1.0.0.tar` & `pyspel-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2022-01-13 17:09:21.000000 pyspel-1.0.0/
--rw-r--r--   0 carmine    (501) staff       (20)      974 2022-01-13 17:09:21.000000 pyspel-1.0.0/PKG-INFO
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2022-01-13 17:09:21.000000 pyspel-1.0.0/pyspel.egg-info/
--rw-r--r--   0 carmine    (501) staff       (20)      974 2022-01-13 17:09:21.000000 pyspel-1.0.0/pyspel.egg-info/PKG-INFO
--rw-r--r--   0 carmine    (501) staff       (20)      203 2022-01-13 17:09:21.000000 pyspel-1.0.0/pyspel.egg-info/SOURCES.txt
--rw-r--r--   0 carmine    (501) staff       (20)       10 2022-01-13 17:09:21.000000 pyspel-1.0.0/pyspel.egg-info/requires.txt
--rw-r--r--   0 carmine    (501) staff       (20)        7 2022-01-13 17:09:21.000000 pyspel-1.0.0/pyspel.egg-info/top_level.txt
--rw-r--r--   0 carmine    (501) staff       (20)        1 2022-01-13 17:09:21.000000 pyspel-1.0.0/pyspel.egg-info/dependency_links.txt
-drwxr-xr-x   0 carmine    (501) staff       (20)        0 2022-01-13 17:09:21.000000 pyspel-1.0.0/pyspel/
--rw-r--r--   0 carmine    (501) staff       (20)        0 2022-01-13 15:05:31.000000 pyspel-1.0.0/pyspel/__init__.py
--rw-r--r--   0 carmine    (501) staff       (20)    31003 2022-01-13 14:31:44.000000 pyspel-1.0.0/pyspel/pyspel.py
--rw-r--r--   0 carmine    (501) staff       (20)        8 2020-10-30 09:13:34.000000 pyspel-1.0.0/README.md
--rw-r--r--   0 carmine    (501) staff       (20)     1170 2022-01-13 17:09:17.000000 pyspel-1.0.0/setup.py
--rw-r--r--   0 carmine    (501) staff       (20)       38 2022-01-13 17:09:21.000000 pyspel-1.0.0/setup.cfg
+drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-23 20:05:49.578458 pyspel-1.0.1/
+-rw-r--r--   0 carmine    (501) staff       (20)    11357 2020-10-30 09:13:34.000000 pyspel-1.0.1/LICENSE
+-rw-r--r--   0 carmine    (501) staff       (20)     1068 2024-04-23 20:05:49.578280 pyspel-1.0.1/PKG-INFO
+-rw-r--r--   0 carmine    (501) staff       (20)        8 2020-10-30 09:13:34.000000 pyspel-1.0.1/README.md
+drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-23 20:05:49.577106 pyspel-1.0.1/pyspel/
+-rw-r--r--   0 carmine    (501) staff       (20)        0 2022-01-13 15:05:31.000000 pyspel-1.0.1/pyspel/__init__.py
+-rw-r--r--   0 carmine    (501) staff       (20)    31445 2024-04-23 20:00:56.000000 pyspel-1.0.1/pyspel/pyspel.py
+drwxr-xr-x   0 carmine    (501) staff       (20)        0 2024-04-23 20:05:49.578113 pyspel-1.0.1/pyspel.egg-info/
+-rw-r--r--   0 carmine    (501) staff       (20)     1068 2024-04-23 20:05:49.000000 pyspel-1.0.1/pyspel.egg-info/PKG-INFO
+-rw-r--r--   0 carmine    (501) staff       (20)      182 2024-04-23 20:05:49.000000 pyspel-1.0.1/pyspel.egg-info/SOURCES.txt
+-rw-r--r--   0 carmine    (501) staff       (20)        1 2024-04-23 20:05:49.000000 pyspel-1.0.1/pyspel.egg-info/dependency_links.txt
+-rw-r--r--   0 carmine    (501) staff       (20)        7 2024-04-23 20:05:49.000000 pyspel-1.0.1/pyspel.egg-info/top_level.txt
+-rw-r--r--   0 carmine    (501) staff       (20)       38 2024-04-23 20:05:49.578496 pyspel-1.0.1/setup.cfg
+-rw-r--r--   0 carmine    (501) staff       (20)     1228 2024-04-23 20:03:52.000000 pyspel-1.0.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyspel-1.0.0/PKG-INFO` & `pyspel-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyspel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Specification Language (Pyspel)
 Home-page: https://github.com/dodaro/pyspel
+Download-URL: https://github.com/dodaro/pyspel/archive/refs/tags/v1.0.1.tar.gz
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 License: Apache 2.0
-Download-URL: https://github.com/dodaro/pyspel/archive/refs/tags/v1.0.0.tar.gz
-Description: Pyspel is a python-based specification language that combines python programs with Answer Set Programming
 Keywords: answer set programming,specification language,combinatorial problems
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+Pyspel is a python-based specification language that combines python programs with Answer Set Programming
```

### Comparing `pyspel-1.0.0/pyspel.egg-info/PKG-INFO` & `pyspel-1.0.1/pyspel.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyspel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python Specification Language (Pyspel)
 Home-page: https://github.com/dodaro/pyspel
+Download-URL: https://github.com/dodaro/pyspel/archive/refs/tags/v1.0.1.tar.gz
 Author: Carmine Dodaro
 Author-email: carmine.dodaro@unical.it
 License: Apache 2.0
-Download-URL: https://github.com/dodaro/pyspel/archive/refs/tags/v1.0.0.tar.gz
-Description: Pyspel is a python-based specification language that combines python programs with Answer Set Programming
 Keywords: answer set programming,specification language,combinatorial problems
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+License-File: LICENSE
+
+Pyspel is a python-based specification language that combines python programs with Answer Set Programming
```

### Comparing `pyspel-1.0.0/pyspel/pyspel.py` & `pyspel-1.0.1/pyspel/pyspel.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import field
 import os
 import json
 from time import sleep
 from types import FunctionType, CodeType
 from typing import Any, ClassVar
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 invalid_exit_codes = {1, 65}
 
 
 def domain(min, max):
     return Term(ObjectVariable(f'{min}..{max}'))
 
@@ -141,29 +141,45 @@
         return Term._op(self, other, ">=")
 
     def __add__(self, other):
         if not isinstance(other, Term):
             other = Term(other)
         return Term._arithmetic(self.value, other.value, "+")
 
+    def __radd__(self, other):
+        return self.__add__(other)
+
     def __sub__(self, other):
         if not isinstance(other, Term):
             other = Term(other)
         return Term._arithmetic(self.value, other.value, "-")
 
+    def __rsub__(self, other):
+        if not isinstance(other, Term):
+            other = Term(other)
+        return Term._arithmetic(other.value, self.value, "-")
+
     def __mul__(self, other):
         if not isinstance(other, Term):
             other = Term(other)
         return Term._arithmetic(self.value, other.value, "*")
 
+    def __rmul__(self, other):
+        return self.__mul__(other)
+
     def __truediv__(self, other):
         if not isinstance(other, Term):
             other = Term(other)
         return Term._arithmetic(self.value, other.value, "/")
 
+    def __rtruediv__(self, other):
+        if not isinstance(other, Term):
+            other = Term(other)
+        return Term._arithmetic(other.value, self.value, "/")
+
     def __mod__(self, other):
         if not isinstance(other, Term):
             other = Term(other)
         return Term._arithmetic(self.value, other.value, "\\")
 
     def __pow__(self, power, modulo=None):
         if not isinstance(power, Term):
@@ -220,22 +236,23 @@
                 terms.append(t.value)
             elif isinstance(t, Atom):
                 terms.append(t.to_python_class())
             elif not isinstance(t, Predicate):
                 terms.append(t.name)
         name = self.predicate.name[0].upper() + self.predicate.name[1:]
         cls = globals()[name]
+        obj = cls()
         args = getattr(cls, '__annotations__', {})
         new_args = {}
         count = 0
         for i in args:
             new_args[i] = terms[count]
-            setattr(cls, f'{i}', terms[count])
+            setattr(obj, f'{i}', terms[count])
             count += 1
-        return cls
+        return obj
 
     def __str__(self):
         terms = []
         for term in self.__dict__:
             if isinstance(self.__dict__[term], Term):
                 terms.append(f"{self.__dict__[term]}")
             elif isinstance(self.__dict__[term], Atom):
@@ -687,20 +704,19 @@
                 raise ValueError(f"Expected list of atoms as parameter, got {type(atom_)}")
 
         instance = open(filename, "r")
         (stdout, stderr, exit_code, killed) = _run_solver(rules='\n'.join(instance.readlines()), solver_path=solver_path, options=["--outf=2"], timeout=None)
         res = json.loads(stdout)
         if res['Result'] == 'SATISFIABLE':
             costs = []
-            r = Result(Result.HAS_SOLUTION)
             assert len(res['Call'][0]['Witnesses']) == 1
             answer_set = res['Call'][0]['Witnesses'][0]
+            output = []
             if 'Value' in answer_set:
                 answer = Answer(answer_set['Value'], costs, False)
-                output = []
                 for atom_name in atoms:
                     output.extend(answer.get_atom_occurrences(atom_name=atom_name))
             return output
 
 
 class Result:
     NO_SOLUTION = 1
```

### Comparing `pyspel-1.0.0/setup.py` & `pyspel-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 NAME = 'pyspel'
 DESCRIPTION = 'Python Specification Language (Pyspel)'
 LONG_DESCRIPTION = 'Pyspel is a python-based specification language that combines python programs with Answer Set Programming'
 
 setup(
   name=NAME,
   packages=find_packages(),
-  version='1.0.0',
+  version='1.0.1',
   license='Apache 2.0',
   description=DESCRIPTION,
   long_description=LONG_DESCRIPTION,
   author='Carmine Dodaro',
   author_email='carmine.dodaro@unical.it',
   url='https://github.com/dodaro/pyspel',
-  download_url='https://github.com/dodaro/pyspel/archive/refs/tags/v1.0.0.tar.gz',
+  download_url='https://github.com/dodaro/pyspel/archive/refs/tags/v1.0.1.tar.gz',
   keywords=['answer set programming', 'specification language', 'combinatorial problems'],
-  install_requires=['decorator'],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
   ],
 )
```

