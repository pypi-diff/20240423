# Comparing `tmp/System_to_Matlab-0.0.4.tar.gz` & `tmp/system_to_matlab-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "System_to_Matlab-0.0.4.tar", last modified: Thu Aug 24 07:40:05 2023, max compression
+gzip compressed data, was "system_to_matlab-0.0.5.tar", last modified: Tue Apr 23 13:58:06 2024, max compression
```

## Comparing `System_to_Matlab-0.0.4.tar` & `system_to_matlab-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.707425 System_to_Matlab-0.0.4/
--rw-rw-rw-   0        0        0     4042 2023-08-11 16:31:21.000000 System_to_Matlab-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      264 2023-08-24 07:40:05.704432 System_to_Matlab-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.614674 System_to_Matlab-0.0.4/System_to_Matlab/
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.658591 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/
--rw-rw-rw-   0        0        0     3136 2023-08-10 08:45:01.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/FileGenerators.py
--rw-rw-rw-   0        0        0     1098 2023-08-08 15:57:47.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MFile.py
--rw-rw-rw-   0        0        0     4320 2023-08-10 06:18:27.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MFunction.py
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.668528 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MatlabElements/
--rw-rw-rw-   0        0        0     3524 2023-08-23 19:35:28.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MatlabElements/CodeElement.py
--rw-rw-rw-   0        0        0      382 2023-06-12 10:51:25.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MatlabElements/MatlabElement.py
--rw-rw-rw-   0        0        0      505 2023-08-23 19:43:37.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MatlabElements/StringElement.py
--rw-rw-rw-   0        0        0      124 2023-04-01 16:56:04.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MatlabElements/__init__.py
--rw-rw-rw-   0        0        0     6617 2023-04-04 08:53:16.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/SFunction.py
--rw-rw-rw-   0        0        0      141 2023-04-01 16:55:45.000000 System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.676507 System_to_Matlab-0.0.4/System_to_Matlab/HelperFunctions/
--rw-rw-rw-   0        0        0      867 2023-05-15 16:26:29.000000 System_to_Matlab-0.0.4/System_to_Matlab/HelperFunctions/GeneralHelperFuncitons.py
--rw-rw-rw-   0        0        0     1369 2023-04-03 13:09:38.000000 System_to_Matlab-0.0.4/System_to_Matlab/HelperFunctions/RobotikHelperFuncitons.py
--rw-rw-rw-   0        0        0      192 2023-05-15 16:23:00.000000 System_to_Matlab-0.0.4/System_to_Matlab/HelperFunctions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.685483 System_to_Matlab-0.0.4/System_to_Matlab/Symbols/
--rw-rw-rw-   0        0        0     8695 2023-08-23 18:59:41.000000 System_to_Matlab-0.0.4/System_to_Matlab/Symbols/DynamicSymbol.py
--rw-rw-rw-   0        0        0     3071 2023-08-23 19:05:24.000000 System_to_Matlab-0.0.4/System_to_Matlab/Symbols/StaticSymbol.py
--rw-rw-rw-   0        0        0     5319 2023-08-24 06:54:32.000000 System_to_Matlab-0.0.4/System_to_Matlab/Symbols/Symbol.py
--rw-rw-rw-   0        0        0      255 2023-05-25 17:08:02.000000 System_to_Matlab-0.0.4/System_to_Matlab/Symbols/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.693498 System_to_Matlab-0.0.4/System_to_Matlab/Systems/
--rw-rw-rw-   0        0        0    12723 2023-08-24 07:27:34.000000 System_to_Matlab-0.0.4/System_to_Matlab/Systems/DynamicSystem.py
--rw-rw-rw-   0        0        0     4564 2023-08-24 07:37:27.000000 System_to_Matlab-0.0.4/System_to_Matlab/Systems/StaticSystem.py
--rw-rw-rw-   0        0        0      509 2023-08-24 07:18:18.000000 System_to_Matlab-0.0.4/System_to_Matlab/Systems/System.py
--rw-rw-rw-   0        0        0      127 2023-04-01 06:50:42.000000 System_to_Matlab-0.0.4/System_to_Matlab/Systems/__init__.py
--rw-rw-rw-   0        0        0      323 2023-08-11 11:11:16.000000 System_to_Matlab-0.0.4/System_to_Matlab/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.702437 System_to_Matlab-0.0.4/System_to_Matlab/tests/
--rw-rw-rw-   0        0        0     1055 2023-08-23 19:40:14.000000 System_to_Matlab-0.0.4/System_to_Matlab/tests/test_CodeElement.py
--rw-rw-rw-   0        0        0     3598 2023-08-23 19:40:59.000000 System_to_Matlab-0.0.4/System_to_Matlab/tests/test_DynamicSymbol.py
--rw-rw-rw-   0        0        0      897 2023-08-23 19:49:58.000000 System_to_Matlab-0.0.4/System_to_Matlab/tests/test_StaticSymbol.py
--rw-rw-rw-   0        0        0      386 2023-08-23 19:43:19.000000 System_to_Matlab-0.0.4/System_to_Matlab/tests/test_StringElement.py
-drwxrwxrwx   0        0        0        0 2023-08-24 07:40:05.647584 System_to_Matlab-0.0.4/System_to_Matlab.egg-info/
--rw-rw-rw-   0        0        0      264 2023-08-24 07:40:05.000000 System_to_Matlab-0.0.4/System_to_Matlab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1374 2023-08-24 07:40:05.000000 System_to_Matlab-0.0.4/System_to_Matlab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-24 07:40:05.000000 System_to_Matlab-0.0.4/System_to_Matlab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-08-24 07:40:05.000000 System_to_Matlab-0.0.4/System_to_Matlab.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-24 07:40:05.000000 System_to_Matlab-0.0.4/System_to_Matlab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      534 2023-08-24 07:39:28.000000 System_to_Matlab-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-24 07:40:05.707425 System_to_Matlab-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.332899 system_to_matlab-0.0.5/
+-rw-rw-rw-   0        0        0     4042 2023-08-11 16:31:21.000000 system_to_matlab-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      320 2024-04-23 13:58:06.329907 system_to_matlab-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.198259 system_to_matlab-0.0.5/System_to_Matlab/
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.241148 system_to_matlab-0.0.5/System_to_Matlab/Calculation/
+-rw-rw-rw-   0        0        0     7114 2024-04-15 13:36:02.000000 system_to_matlab-0.0.5/System_to_Matlab/Calculation/Calculation.py
+-rw-rw-rw-   0        0        0       67 2024-01-03 10:33:31.000000 system_to_matlab-0.0.5/System_to_Matlab/Calculation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.259100 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/
+-rw-rw-rw-   0        0        0     3136 2024-01-17 15:50:06.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/FileGenerators.py
+-rw-rw-rw-   0        0        0     2408 2024-02-10 16:58:58.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MFile.py
+-rw-rw-rw-   0        0        0     7058 2024-04-11 13:44:10.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MFunction.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.272063 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MatlabElements/
+-rw-rw-rw-   0        0        0     4995 2024-04-11 13:29:30.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MatlabElements/CodeElement.py
+-rw-rw-rw-   0        0        0      382 2023-06-12 10:51:25.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MatlabElements/MatlabElement.py
+-rw-rw-rw-   0        0        0      505 2023-08-23 19:43:37.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MatlabElements/StringElement.py
+-rw-rw-rw-   0        0        0      124 2023-04-01 16:56:04.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MatlabElements/__init__.py
+-rw-rw-rw-   0        0        0    10360 2024-04-23 11:23:43.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/SFunction.py
+-rw-rw-rw-   0        0        0      141 2023-04-01 16:55:45.000000 system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.282036 system_to_matlab-0.0.5/System_to_Matlab/HelperFunctions/
+-rw-rw-rw-   0        0        0      823 2024-01-24 18:43:42.000000 system_to_matlab-0.0.5/System_to_Matlab/HelperFunctions/GeneralHelperFuncitons.py
+-rw-rw-rw-   0        0        0     1318 2024-01-24 18:43:25.000000 system_to_matlab-0.0.5/System_to_Matlab/HelperFunctions/RobotikHelperFuncitons.py
+-rw-rw-rw-   0        0        0      192 2023-05-15 16:23:00.000000 system_to_matlab-0.0.5/System_to_Matlab/HelperFunctions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.294003 system_to_matlab-0.0.5/System_to_Matlab/Symbols/
+-rw-rw-rw-   0        0        0     8641 2024-01-24 18:52:23.000000 system_to_matlab-0.0.5/System_to_Matlab/Symbols/DynamicSymbol.py
+-rw-rw-rw-   0        0        0     3107 2024-01-24 18:42:55.000000 system_to_matlab-0.0.5/System_to_Matlab/Symbols/StaticSymbol.py
+-rw-rw-rw-   0        0        0     5319 2023-08-24 06:54:32.000000 system_to_matlab-0.0.5/System_to_Matlab/Symbols/Symbol.py
+-rw-rw-rw-   0        0        0      255 2023-05-25 17:08:02.000000 system_to_matlab-0.0.5/System_to_Matlab/Symbols/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.303977 system_to_matlab-0.0.5/System_to_Matlab/Systems/
+-rw-rw-rw-   0        0        0    16820 2024-04-23 13:45:43.000000 system_to_matlab-0.0.5/System_to_Matlab/Systems/DynamicSystem.py
+-rw-rw-rw-   0        0        0     5656 2024-04-15 14:24:47.000000 system_to_matlab-0.0.5/System_to_Matlab/Systems/StaticSystem.py
+-rw-rw-rw-   0        0        0      536 2024-01-15 15:47:10.000000 system_to_matlab-0.0.5/System_to_Matlab/Systems/_System.py
+-rw-rw-rw-   0        0        0      127 2023-04-01 06:50:42.000000 system_to_matlab-0.0.5/System_to_Matlab/Systems/__init__.py
+-rw-rw-rw-   0        0        0      323 2023-08-11 11:11:16.000000 system_to_matlab-0.0.5/System_to_Matlab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.322925 system_to_matlab-0.0.5/System_to_Matlab/tests/
+-rw-rw-rw-   0        0        0     4759 2024-02-10 16:01:25.000000 system_to_matlab-0.0.5/System_to_Matlab/tests/test_Calculation.py
+-rw-rw-rw-   0        0        0     1363 2024-01-20 09:45:46.000000 system_to_matlab-0.0.5/System_to_Matlab/tests/test_CodeElement.py
+-rw-rw-rw-   0        0        0     3598 2023-08-23 19:40:59.000000 system_to_matlab-0.0.5/System_to_Matlab/tests/test_DynamicSymbol.py
+-rw-rw-rw-   0        0        0     5546 2024-04-23 13:49:44.000000 system_to_matlab-0.0.5/System_to_Matlab/tests/test_DynamicSystem.py
+-rw-rw-rw-   0        0        0      897 2023-08-23 19:49:58.000000 system_to_matlab-0.0.5/System_to_Matlab/tests/test_StaticSymbol.py
+-rw-rw-rw-   0        0        0     2666 2024-04-15 14:49:49.000000 system_to_matlab-0.0.5/System_to_Matlab/tests/test_StaticSystem.py
+-rw-rw-rw-   0        0        0      386 2023-08-23 19:43:19.000000 system_to_matlab-0.0.5/System_to_Matlab/tests/test_StringElement.py
+drwxrwxrwx   0        0        0        0 2024-04-23 13:58:06.326916 system_to_matlab-0.0.5/System_to_Matlab.egg-info/
+-rw-rw-rw-   0        0        0      320 2024-04-23 13:58:06.000000 system_to_matlab-0.0.5/System_to_Matlab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1592 2024-04-23 13:58:06.000000 system_to_matlab-0.0.5/System_to_Matlab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 13:58:06.000000 system_to_matlab-0.0.5/System_to_Matlab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 13:58:06.000000 system_to_matlab-0.0.5/System_to_Matlab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-23 13:58:06.000000 system_to_matlab-0.0.5/System_to_Matlab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      534 2024-04-23 13:57:21.000000 system_to_matlab-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 13:58:06.333898 system_to_matlab-0.0.5/setup.cfg
```

### Comparing `System_to_Matlab-0.0.4/LICENSE` & `system_to_matlab-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/FileGenerators.py` & `system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/FileGenerators.py`

 * *Files identical despite different names*

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/FileGenerators/MatlabElements/CodeElement.py` & `system_to_matlab-0.0.5/System_to_Matlab/FileGenerators/MatlabElements/CodeElement.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,123 @@
+from __future__ import annotations
 from .MatlabElement import MatlabElement
 from ...Symbols import DynamicSymbol
 from ...Symbols.Symbol import Symbol
-
+from ...Calculation.Calculation import Calculation
 
 import symengine as se
-from symengine.lib.symengine_wrapper import FunctionSymbol
 import sympy as sp
 
 from typing import Union, Any
 
 
 class CodeElement(MatlabElement):
-    def __init__(self, code, name: str, indent: int = 0,  use_cse: bool = True, clear: bool = True):
-        MatlabElement.__init__(self)
+    def __init__(self, code: Calculation, indent: int = 0,  use_cse: bool = True, clear: bool = True):
+        """ Code Element for the Matlab File Generator. Represents a chunk of code. Can also use cse to make the code more efficient.
 
-        if not isinstance(code, (list, se.Matrix)):
-            code = se.Matrix([code])
-        else:
-            code = se.Matrix(code)
+        Parameters
+        ----------
+        code : Calculation
+            code which should be generated
+        indent : int, optional
+            how much indents should be added at the front of every line, by default 0
+        use_cse : bool, optional
+            Sets if cse should be used on the code, by default True
+        clear : bool, optional
+            sets if the variables from cse should be cleared afterwards, by default True
+        """
+        MatlabElement.__init__(self)
 
-        if isinstance(name, str):
-            name = se.Symbol(name)
-            name = se.Matrix([name])
-        # elif isinstance(name, list):
-        #     if isinstance(name[0], str):
-        #         l = []
-        #         for na in name:  # type: ignore
-        #             l.append(se.Symbol(na))
-        #         name = se.Matrix(l)
-        # elif isinstance(name, (se.Matrix, sp.Matrix)):
-        #     name = se.sympify(name)
-        # elif isinstance(name, (FunctionSymbol, se.Symbol, sp.Function, sp.Symbol)):
-        #     name = se.Matrix([name])
+        # if not isinstance(code, (list, se.Matrix)):
+        #     code = se.Matrix([code])
         # else:
-        #     # display(type(name))
-        #     raise TypeError("name must be a string or a list of strings")
+        #     code = se.Matrix(code)
 
-        self._code = code.subs(Symbol._Symbol_to_printable_dict)
-        self._name = name.subs(
-            Symbol._Symbol_to_printable_dict)  # type: ignore
-        self._use_cse = use_cse
-        self._Indentation = indent
-        self._Clear = clear
+        # if isinstance(name, str):
+        #     name = se.Symbol(name)
+        #     name = se.Matrix([name])
+        # if isinstance(name, se.Symbol):
+        #     name = se.Matrix([name])
+            
+        if not isinstance(code, Calculation):
+            raise TypeError(f"code has to be a Calculation but {type(code)} was given")
+        self._code: Calculation = code
+        self._code.subs(Symbol._Symbol_to_printable_dict)
+        # self._name = name.subs(
+        #     Symbol._Symbol_to_printable_dict)  # type: ignore
+        self._use_cse: bool = use_cse
+        self._Indentation: int = indent
+        self._Clear: bool = clear
+        self._override: bool = False
+        self._lhs: se.Matrix = None
+
+    def override_lhs(self, lhs: se.Symbol) -> CodeElement:
+        if not isinstance(lhs, se.Symbol):
+            raise TypeError(f"lhs has to be a Symbol but {type(lhs)} was given")
+        self._override = True
+        self._lhs = se.Matrix([lhs])
+        return self
 
     def generateCode(self) -> str:
 
         s = ""
         if self._use_cse:
-            s += self._generate_cse(self._code, self._name)
+            s += self._generate_cse()
         else:
-            s += self._remove_curlyBreakets(sp.octave_code(self._name)) + " = " + self._remove_curlyBreakets(sp.octave_code(self._code)) + ";\n"
+            for i in range(len(self._code._calcs)):
+                if self._override:
+                    s += self._Indentation * "\t" + self._remove_curlyBreakets(sp.octave_code(self._lhs)) + " = " + self._remove_curlyBreakets(sp.octave_code(self._code._calcs[i])) + ";\n"
+                else:
+                    s += self._Indentation * "\t" + self._remove_curlyBreakets(sp.octave_code(self._code._vars[i])) + " = " + self._remove_curlyBreakets(sp.octave_code(self._code._calcs[i])) + ";\n"
+            # s += self._remove_curlyBreakets(sp.octave_code(self.vars)) + " = " + self._remove_curlyBreakets(sp.octave_code(self._code)) + ";\n"
         return s
 
-    def _generate_cse(self, code: se.Matrix, name: str) -> str:
-        # TODO allow cse for list of Matrices to maybe enhance the performance
-        # But this code in the File generator to make use cse on the whole code no only on each block individually
+    def _generate_cse(self) -> str:
         s = ""
 
-        shape = code.shape
-
-        f1, f2 = se.cse(code)
+        indizes_shapes, code_vector = self._code._generate_shape_index_list()
+        
+        f1, f2 = se.cse(code_vector)
         for temp in f1:
             s += self._Indentation * "\t" + \
                 self._remove_curlyBreakets(sp.octave_code(temp[0])) + " = " + \
                 self._remove_curlyBreakets(sp.octave_code(temp[1])) + ";\n"  # type: ignore
-        s += "\n"
+        if f1 != []:
+            s += "\n"
 
-        if shape == (1, 1):
-            s += self._Indentation * "\t" + \
-                self._remove_curlyBreakets(sp.octave_code(name[0, 0])) + " = " + \
-                self._remove_curlyBreakets(sp.octave_code(f2)) + ";\n"  # type: ignore
-        else:
-            s += self._Indentation * "\t" + self._remove_curlyBreakets(sp.octave_code(name)) + " = " + sp.octave_code(
-                se.Matrix(f2).reshape(shape[0], shape[1])) + ";\n"  # type: ignore
-        s += "\n"
-        if self._Clear:
-            s += self._Indentation * "\t" + "clear "
-            for temp in f1:
-                s += self._remove_curlyBreakets(sp.octave_code(temp[0])) + " "  # type: ignore
-            if s.endswith("clear "):
-                s = s[:-6]
+        ii = 0
+        for i in indizes_shapes:
+            index = i[0]
+            shape = i[1]
+            code = f2[index[0]:index[1]]
+            if self._override:
+                name = self._lhs
             else:
-                s = s[:-1]
-                s += ";"
-            s += "\n"
+                name = self._code._vars[ii]
+            ii += 1
+
+            if shape == (1, 1):
+                s += self._Indentation * "\t" + \
+                    self._remove_curlyBreakets(sp.octave_code(name[0])) + " = " + \
+                    self._remove_curlyBreakets(sp.octave_code(code)) + ";\n"  # type: ignore
+            else:
+                s += self._Indentation * "\t" + self._remove_curlyBreakets(sp.octave_code(name)) + " = " + sp.octave_code(
+                    se.Matrix(code).reshape(shape[0], shape[1])) + ";\n"  # type: ignore
+            # s += "\n"
+            if self._Clear:
+                s += self._Indentation * "\t" + "clear "
+                for temp in f1:
+                    s += self._remove_curlyBreakets(sp.octave_code(temp[0])) + " "  # type: ignore
+                if s.endswith("clear "):
+                    s = s[:-6]
+                else:
+                    s = s[:-1]
+                    s += ";"
+                s += "\n"
+            if s.endswith("\n\n\n"):
+                s = s[:-2]
         return s
 
     def _remove_curlyBreakets(self, code: str) -> str:
         if code.startswith("{") and code.endswith("}"):
             code = code[1:-1]
         return code
```

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/HelperFunctions/GeneralHelperFuncitons.py` & `system_to_matlab-0.0.5/System_to_Matlab/HelperFunctions/GeneralHelperFuncitons.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Union, Any, List, Tuple
 import symengine as se
 import sympy as sp
 
 def SymbolicMatrix(symbol:str, rows:int, cols:int) -> se.Matrix:
     """Creates a symbolic matrix with the given symbol.
 
     Args:
```

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/HelperFunctions/RobotikHelperFuncitons.py` & `system_to_matlab-0.0.5/System_to_Matlab/HelperFunctions/RobotikHelperFuncitons.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import Union, Any, List, Tuple
 import symengine as se
 
 
-def Drehmatrix(angle_vec: Union[se.Matrix , list]) -> se.Matrix:
+def Drehmatrix(angle_vec: se.Matrix | list) -> se.Matrix:
     """Computes the 3D rotation matrix for the given angle vector.
 
     The angle vector must be in the form [x, y, z], where x, y, and z
     represent the angles of rotation around the x, y, and z axes, respectively.
 
     Args:
         angle_vector: A 3x1 matrix or a list of three numbers representing the angles of rotation around the x, y, and z axes.
```

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/Symbols/DynamicSymbol.py` & `system_to_matlab-0.0.5/System_to_Matlab/Symbols/DynamicSymbol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .Symbol import Symbol
 import symengine as se
-from typing import Union, List, Any
+from typing import Union, Any
 
 
 class DynamicSymbol(Symbol):
     """generates an instance of the DynamicSymbol class
 
         Parameters
         ----------
@@ -49,20 +49,20 @@
         self._number_of_variables = number_of_variables
         self._number_of_derivatives = number_of_derivatives
         self._gen_numbered_state_variables()
         if number_of_derivatives > 0:
             self._gen_differentiation_dict()
 
     @property
-    def vars(self) -> Union[se.MutableDenseMatrix, List[se.MutableDenseMatrix]]:
+    def vars(self) -> Union[se.Matrix, list[se.Matrix]]:
         """returns a Matrix of the generated Symbols
 
         Returns
         -------
-        Union[se.MutableDenseMatrix, List[se.MutableDenseMatrix]]
+        Union[se.Matrix, list[se.Matrix]]
             Matrix of the generated Symbols
         """
         if self._number_of_derivatives == 0:
             return se.Matrix(self._Symbols)
         else:
             v = []
             for i in range(self._number_of_derivatives + 1):
@@ -152,32 +152,32 @@
     #         for ii in range(self._number_of_variables):
     #             self._dict_of_steady_state_substitutions.update({self.vars[i][ii]: self.vars[0][ii]})
 
     def _repr_latex_(self):
         return se.Matrix(self._Symbols).reshape(self._number_of_variables, self._number_of_derivatives + 1)._repr_latex_()
 
 
-def DynamicSymbols(names: List[str], number_of_variables: int = 1, number_of_derivatives: int = 0, as_matrix_list = False) -> Any:
+def DynamicSymbols(names: list[str], number_of_variables: int = 1, number_of_derivatives: int = 0, as_matrix_list = False) -> Any:
     """ Method to generate a list of DynamicSymbols
 
     Parameters
     ----------
-    names : List[str]
-        List of names for the DynamicSymbols
+    names : list[str]
+        list of names for the DynamicSymbols
     number_of_variables : int, optional
         Number of variables to create per name, by default 1
     number_of_derivatives : int, optional
         Number of derivatives to create per name and number, by default 0
     as_matrix_list : bool, optional
         Spezifies if the variables should be returned as a single Matrix or a list of vectors, by default False
 
     Returns
     -------
     Any
-        List of DynamicSymbols or Matrix of DynamicSymbols
+        list of DynamicSymbols or Matrix of DynamicSymbols
     """
     l = []
     
     if as_matrix_list:  
         for s in names:
             l.append(DynamicSymbol(s, number_of_variables,
                     number_of_derivatives).var_as_vec())
```

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/Symbols/StaticSymbol.py` & `system_to_matlab-0.0.5/System_to_Matlab/Symbols/StaticSymbol.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from .Symbol import Symbol
 import symengine as se
 
-from typing import Union, List
-
 class StaticSymbol(Symbol):
     """generates an instance of the StaticSymbol class
 
         Parameters
         ----------
         Notation : str
             Name of the Symbol
@@ -20,20 +18,21 @@
         ----------
         Notation : str
             Name of the Symbol
         number_of_variables : int, optional
             Number of variables which should be created, by default 1
         """
         if not isinstance(Notation, str) or Notation == "" :
-            raise ValueError("Notation must be a non empty string")
+            raise ValueError(f"Notation must be a non empty string but {type(Notation)} was given")
         
         super().__init__(Notation)
+        self._Outputs: list = []
         self._number_of_variables = number_of_variables
         self._gen_numbered_state_variables()
-    
+        
     @property
     def vars(self) -> se.Matrix:
         """returns a Matrix of the generated Symbols
 
         Returns
         -------
         se.Matrix
@@ -58,28 +57,28 @@
                 #self._Symbols.append(se.Symbol(self._Notation + f"_{i}"))
                 super()._Symbol_to_printable_dict.update({self._Symbols[i-1]: se.Symbol(s_sub)})
         
     def _repr_latex_(self) -> str:
         return self.vars._repr_latex_()
     
 
-def StaticSymbols(names: List[str], number_of_variables: int = 1) -> List[se.Symbol]:
+def StaticSymbols(names: list[str], number_of_variables: int = 1) -> list[se.Symbol]:
     """Method to generate a list of StaticSymbols
 
     Parameters
     ----------
-    names : List[str]
-        List of names for the StaticSymbols
+    names : list[str]
+        list of names for the StaticSymbols
     number_of_variables : int, optional
         Number of variables to create per name given, by default 1
 
     Returns
     -------
-    List[se.Symbol]
-        List of the generated StaticSymbols
+    list[se.Symbol]
+        list of the generated StaticSymbols
     """
     l = []
     if number_of_variables == 1:
         for s in names:
             l.append(StaticSymbol(s,number_of_variables).vars[0])
     else:    
         for s in names:
```

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/Symbols/Symbol.py` & `system_to_matlab-0.0.5/System_to_Matlab/Symbols/Symbol.py`

 * *Files identical despite different names*

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/Systems/DynamicSystem.py` & `system_to_matlab-0.0.5/System_to_Matlab/Systems/DynamicSystem.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from .System import System
+#from .System import System
 from ..Symbols import DynamicSymbol, StaticSymbol
 from ..Symbols.Symbol import Symbol
 from ..FileGenerators import MFile, MFunction, SFunction
+from ..Calculation.Calculation import Calculation
 
 import symengine as se
 import sympy as sp
 
 from typing import Any, Union
 
-class DynamicSystem(System):
+class DynamicSystem():
     """Generates a class for a dynamic system with the following structure:
 
         Args:
             x (se.Matrix): Vector of the state variables
             u (se.Matrix): Vector of the input variables
 
         Raises:
@@ -26,23 +27,31 @@
             x (se.Matrix): Vector of the state variables
             u (se.Matrix): Vector of the input variables
 
         Raises:
             ValueError: state vector is no column vector
             ValueError: input vector is no column vector
         """
-        super().__init__()
         self._is_linearized = False
         if x.shape[1] != 1:
             raise ValueError("State vector has to be a column vector")
         if u.shape[1] != 1:
             raise ValueError("Input vector has to be a column vector")
         self._x = se.sympify(x)
         self._u = se.sympify(u)
-        self._Equations = [None, None]
+        self._State_Equations: Calculation = Calculation()
+        # self._Calcs: Calculation = Calculation()
+        self._Outputs: list[se.Symbols | se.Function] = []
+        self._Outputs_Calcs: Calculation = Calculation()
+        self._Inputs: list[se.Symbols | se.Function] = [se.Symbol("u")]
+        # self._Input_Calcs: Calculation = Calculation()
+
+        # self._Input_Calcs.addCalculation(self._u, se.Symbol('u'),is_matrix_input=True)
+        
+        self._Parameters: list[tuple[se.Symbol | se.Function, float]] = []
     
     @property
     def A(self) -> se.Matrix:
         if self._is_linearized:
             return self._A
         else:
             raise ValueError("System has to be linearized before accessing the A matrix")
@@ -88,72 +97,76 @@
         se.Matrix
             vector of the input variables
         """
         return self._u
     
     @property
     def x_dot(self) -> se.Matrix:
+        """vector of the derivatives of the state variables
+
+        Returns
+        -------
+        se.Matrix
+            vector of the derivatives of the state variables
+        """
         return se.Matrix([se.diff(x, DynamicSymbol._derivation_variable).subs(DynamicSymbol._dict_of_derivation_for_substitutions) for x in self.x])
     
     @property
     def y(self) -> se.Matrix:
         """ vector of the output functions
 
         Returns
         -------
         se.Matrix
             vector of the output functions
         """
-        l = None
-        for i in self._Outputs:
-            if l is None:
-                l = i[1]
-            else:
-                l = l.col_join(i[1])
-        return l
+        _ , vec = self._Outputs_Calcs._generate_shape_index_list()
+        return vec
     
     def linearize(self, steady_state_state_vec: se.Matrix = None, steady_state_input_vec: se.Matrix = None) -> list[se.Matrix]:
         """ linearizes the system around a given steady state
 
         Parameters
         ----------
         steady_state_state_vec : se.Matrix, optional
             vector of variables which should be used in the steady state, by default None
+            Can be omitted if the steady state is 0
         steady_state_input_vec : se.Matrix, optional
             vector of input variables which should be used in the strady state , by default None
+            Can be omitted if the steady state is 0
 
         Returns
         -------
         list[se.Matrix]
             returns the linearized Matrizes [A,B,C,D]
 
         Raises
         ------
         ValueError
             Raised if the dimensions of the given steady state vector does not match the dimensions of the state vector 
         """
         
         
-        if self._Equations[0] is None or self._Equations[1] is None:
+        if len(self._State_Equations.calcs) == 0 or len(self._Outputs_Calcs.calcs) == 0:
             raise ValueError("State and output equations have to be set before linearization")
         
         if steady_state_state_vec is None:
             steady_state_state_vec = self._create_symbolic_steady_state_state_vector()
             
         if steady_state_input_vec is None:
             steady_state_input_vec = self._create_symbolic_steady_state_input_vector()
         
         if steady_state_state_vec.shape != self.x.shape or steady_state_input_vec.shape != self.u.shape:
             raise ValueError(
                 "Size of steady_state hast to be equal to the size of the state vector x")
 
-        self._A: se.Matrix = self._Equations[0].jacobian(self.x)
-        self._B: se.Matrix = self._Equations[0].jacobian(self.u)
-        self._C: se.Matrix = self._Equations[1].jacobian(self.x)
-        self._D: se.Matrix = self._Equations[1].jacobian(self.u)
+        self._A: se.Matrix = self._State_Equations._generate_shape_index_list()[1].jacobian(self.x)
+        self._B: se.Matrix = self._State_Equations._generate_shape_index_list()[1].jacobian(self.u)
+        self._C: se.Matrix = self._Outputs_Calcs._generate_shape_index_list()[1].jacobian(self.x)
+        self._D: se.Matrix = self._Outputs_Calcs._generate_shape_index_list()[1].jacobian(self.u)
 
         for i in range(len(self.x)):
             self._A = self._A.subs(self.x[i], steady_state_state_vec[i])
             self._B = self._B.subs(self.x[i], steady_state_state_vec[i])
             self._C = self._C.subs(self.x[i], steady_state_state_vec[i])
             self._D = self._D.subs(self.x[i], steady_state_state_vec[i])
         
@@ -164,60 +177,106 @@
             self._D = self._D.subs(self.u[i], steady_state_input_vec[i])
 
         self._is_linearized = True
 
         
         return [self._A, self._B, self._C, self._D]
 
-    def addStateEquations(self, equations: se.Matrix) -> None:
+    def addStateEquations(self, equations: se.Matrix , add_as_Output = True) -> None:
         """adding the equations for the states of the system x_dot = f(x, u)
 
         Args:
             equation (se.Matrix): Matrix of the expressions corresponding to the system states
+            add_as_Output (bool, optional): If true the equations will be added as outputs. Defaults to True.
         """
-        if equations.shape[1] != 1:
-            raise ValueError("Equations have to be a column vector")
-        if equations.shape[0] != self.x.shape[0]:
-            raise ValueError("Number of equations has to be equal to the number of states")
+        if isinstance(equations, se.Matrix):
+            if equations.shape[1] != 1:
+                raise ValueError("Equations have to be a column vector")
+            if equations.shape[0] != self.x.shape[0]:
+                raise ValueError("Number of equations has to be equal to the number of states")
+        else:
+            raise TypeError("Equations have to be a Matrix")
         
-        # maybe add warning if equations are already set
-        self._Equations[0] = equations
+        if len(self._State_Equations.calcs) != 0:
+            raise ValueError("State equations are already set")
+        self._State_Equations.addCalculation(self.x_dot, equations)
+        self._number_of_states = equations.shape[0]
+        
+        if add_as_Output:
+            for state in self.x:
+                self.addOutput(state)
   
-    def addInput(self, input: Any, name: str) -> None:
-        """Adds an input to the system
-
-        Args:
-            input (Any): input which should be added to the system, has to be an expressions or a Matrix of expressions
+    # def addInput(self, input: se.Symbol | se.Function | se.Matrix, name: str | se.Symbol = "") -> None:
+    #     """Adds an aditional input to the System.
+    #     Not needed normally, standard inputs should be given when initializing the System.
+    #     (Inputs which do not change should be included via the parameters)
+    #     When a name is given the given Symbol/Matrix will be outputed with the given name.
+    #     Names are not used in the S-Function 
+    #         --(order of the input vector must be the same as here)
+    #         --(if you input multiple inputs the order is also the same)
+    #     ----------
+    #     input : se.Symbol | se.Function | se.Matrix
+    #         The input to be added.
+    #     name : str, optional
+    #         The name of the input. If non is given the name of the Symbol itself is used. Defaults to "".
+    #     """
+        
+    #     if isinstance(input, se.Matrix):
+    #         if name == "":
+    #             raise ValueError("Matrix inputs have to have a name")
+    #         is_input_matrix = True
+    #     else:
+    #         is_input_matrix = False
+        
+    #     if name == "":
+    #         self._Inputs.append(input)
+    #     else:
+    #         self._Inputs.append(se.Symbol(name))
+    #         self._Input_Calcs.addCalculation(input, se.Symbol(name),is_matrix_input=is_input_matrix)
+        
+    
+    def addCalculation(self, name: Union[str, se.Symbol, list[str], Calculation], rhs: se.Expr = None) -> None:
+        """Adding an Calculation to the System. Should be used if you want to add some Output equations in the form y = f(x) 
+        Has to have the form name = rhs.
+            name hast to be a Symbol or a string which can be converted to a Symbol
+        Parameters
+        ----------
+        name : Union[str, se.Symbol, list[str]]
+            Can be an Calculation object or,
+            the name of the variable calculated in the equation. Must be a Symbol or a string that can be converted to a Symbol. 
+        rhs : se.Expr, optional
+            The calculation to be added to the system. Defaults to None.
         """
-        self._Inputs.append(input)  
-    
-    def addOutput(self, output: Union[se.Expr, se.Matrix], name: str) -> None:
-        """Adds an output to the system y = h(x,u)
 
-        Args:
-            output (Union[se.Expr, se.Matrix]): output which should be added to the system, has to be an expressions or a Matrix of expressions
-            name (str): name of the output
-        """
-        output = se.sympify(output)
-        
-        if self._Equations[1] is None:
-            if type(output) == se.Matrix:
-                self._Equations[1] = output
-            else:
-                self._Equations[1] = se.Matrix([output])
+        if isinstance(name, Calculation):
+            self._Outputs_Calcs.append_Calculation(name)
         else:
-            if type(output) == se.Matrix:
-                self._Equations[1] = self._Equations[1].col_join(output)
-            else:
-                self._Equations[1] = self._Equations[1].col_join(se.Matrix([output]))
-        
-        self._Outputs.append((output, StaticSymbol(name, len(output)).vars))
+            calc = Calculation()
+            calc.addCalculation(name, rhs)
+            self._Outputs_Calcs.addCalculation(name, rhs)
+
+    def addOutput(self, output: se.Symbol | se.Function, name: str = "") -> None:
+        """Adds an output to the System.
+        When a name is given the given Symbol will be outputed with the given name (only when using M-Functions, an S-function has only one combined output).
+        ----------
+        output : se.Symbol | se.Function
+            The output to be added.
+        name : str, optional
+            The name of the output. Defaults to "".
+        """
+        if not isinstance(output, (se.Symbol, se.Function)):
+            raise TypeError("Output has to be a Symbol or a Function")
+        if name == "":
+            self._Outputs.append(output)
+        else:
+            self._Outputs.append(se.Symbol(name))
+            self._Outputs_Calcs.addCalculation(se.Symbol(name), output)
     
-    def addParameter(self, parameter: Any, values = 0) -> None:
-        """adds a parameter to the system
+    def addParameter(self, parameter: Any, values:list|int = 0) -> None:
+        """adds a parameter to the System. If values are provided then the init file will include them if not they will be set to 0.
 
         Args:
             parameter (Any): parameter which should be added to the system, has to be a symbol or a Matrix of symbols
             
             values (Union[None, Any], optional): values for the parameter. Either a list or a column Matrix.
             Defaults to None.
         """
@@ -225,108 +284,118 @@
         if values == 0:
             values = list(0 for i in range(len(parameter)))
         if len(parameter) != len(values):
             raise ValueError("Number of parameters and values does not match")
         
         self._Parameters.extend(list(zip(parameter, values)))
     
-    def write_ABCD_to_File(self, name:str, path:str = "", override:bool = True):
+    def write_ABCD_to_File(self, name:str, path:str = "", overwrite:bool = True):
         """writes the ABCD Matrizes of the linearized system to a matlab file
 
         Parameters
         ----------
         name : str
             Name of the file
         path : str, optional
             Path in which the file should be saved, by default ""
-        override : bool, optional
+        overwrite : bool, optional
             If true, the file will be overwritten if it already exists, by default True
         """
         File = MFile(name, path)
-        File.addMathExpression(self._A, "A")
-        File.addMathExpression(self._B, "B")
-        File.addMathExpression(self._C, "C")
-        File.addMathExpression(self._D, "D")
-        File.generateFile(override)
-        pass
+        ABCD_calc = Calculation()
+        ABCD_calc.addCalculation(se.Symbol("A"), self._A)
+        ABCD_calc.addCalculation(se.Symbol("B"), self._B)
+        ABCD_calc.addCalculation(se.Symbol("C"), self._C)
+        ABCD_calc.addCalculation(se.Symbol("D"), self._D)
+        File.addCalculation(ABCD_calc)
+        File.generateFile(overwrite)
     
-    def write_init_File(self, name:str, path:str = "", override:bool = True):
+    def write_init_File(self, name:str, path:str = "", overwrite:bool = True):
         """writes an init file for the Parameters and the initial conditions of the system
 
         Parameters
         ----------
         name : str
             Name of the file
         path : str, optional
             Path where the file should be saved, by default ""
-        override : bool, optional
+        overwrite : bool, optional
             If true, the file will be overwritten if it already exists, by default True
         """
         File = MFile(name, path)
         File.addText(r"%% System parameters")
         File.addText("\n")
         for para in self._Parameters:
             File.addText(str(sp.octave_code(para[0].subs(Symbol._Symbol_to_printable_dict))) + " = " + str(para[1]) + ";\n")
             
             
         File.addText(r"params = [" + ", ".join([sp.octave_code(para[0].subs(Symbol._Symbol_to_printable_dict)) for para in self._Parameters]) + "]; \n \n") # type: ignore
         File.addText(r"%% Initial conditions" + "\n")
         File.addText("x_ic = " + str(sp.octave_code(self._x * 0)) + ";\n")
-        File.generateFile(override)
+        File.generateFile(overwrite)
     
-    def write_SFunction(self, name:str, path:str = "", override:bool = True):
+    def write_SFunction(self, name:str, path:str = "", overwrite:bool = True):
         """writes the nonlinear system as a SFunction to a matlab file
 
         Parameters
         ----------
         name : str
             Name of the file
         path : str, optional
             Path where the file should be stored, by default ""
-        override : bool, optional
+        overwrite : bool, optional
             If true, the file will be overwritten if it already exists, by default True
         """
         File = SFunction(name, path)
-        File.addState(self._x, self._Equations[0])
-        File.addOutput(self._Equations[1])
-        for inp in self._Inputs:
-            File.addInput(inp)
+        File.addState(self._x, self._State_Equations)
+        File.addOutput_equations(self._Outputs_Calcs)
+        for o in self._Outputs:
+            File.addOutput(o)
+        
+        #for i in self._Input_Calcs.outputs:
+        #    File.addInput(i)
+        File.addInput(self._u, se.Symbol('u'))
+            
         File.addParameter(self._Parameters) 
-        File.generateFile(override)
+        File.generateFile(overwrite)
     
-    def write_MFunctions(self, name:str, path:str = "", override:bool = True):
+    def write_MFunctions(self, name:str, path:str = "", overwrite:bool = True):
         """write the nonlinear system as two MFunctions to a matlab file
 
         Parameters
         ----------
         name : str
             Name of the files
         path : str, optional
             Path where the files should be saved, by default ""
-        override : bool, optional
+        overwrite : bool, optional
             If true, the files will be overwritten if they already exist, by default True
         """
         Fdyn = MFunction(name + "_dyn", path)
+        
         Fdyn.addInput(self.x, "x")
         Fdyn.addInput(self.u, "u")
-        pars = []
-        for i in self._Parameters:
-            pars.append(i[0])
-        Fdyn.addInput(pars, "params")
-        Fdyn.addOutput(self.x_dot, "xdot")
-        Fdyn.addEquations(self._Equations[0], self.x_dot)
+        # pars = []
+        # for i in self._Parameters:
+        #     pars.append(i[0])
+        Fdyn.addInput(se.Matrix([i[0] for i in self._Parameters ]), "params")
+        #Fdyn.addOutput(self.x_dot, "xdot")
+        temp = Calculation()
+        temp.addCalculation(se.Symbol("xdot"),self._State_Equations.calcs[0] )
+        Fdyn.addCalculation(Calculation.append_Calculations([temp]))
+        Fdyn.addOutput(se.Symbol("xdot"))
         
-        Fdyn.generateFile(override)
+        Fdyn.generateFile(overwrite)
         
         Fout = MFunction(name + "_out", path)
         Fout.addInput(self.x, "x")
-        Fout.addInput(pars, "params")
+        Fout.addInput(se.Matrix([i[0] for i in self._Parameters ]), "params")
         Fout.addOutput(self.y, "y")
-        Fout.addEquations(self._Equations[1], self.y)
-        Fout.generateFile(override)
+        Fout.addCalculation(Calculation.append_Calculations([self._Outputs_Calcs]))
+        Fout.generateFile(overwrite)
     
     def _create_symbolic_steady_state_state_vector(self) -> se.Matrix:
         return se.Matrix([se.Symbol("x_{" + str(i) + "ss}") for i in range(len(self.x))])
     
     def _create_symbolic_steady_state_input_vector(self) -> se.Matrix:
         return se.Matrix([se.Symbol("u_{" + str(i) + "ss}") for i in range(len(self.u))])
```

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/tests/test_CodeElement.py` & `system_to_matlab-0.0.5/System_to_Matlab/tests/test_CodeElement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 from System_to_Matlab.FileGenerators.MatlabElements import CodeElement
+from System_to_Matlab.Calculation import Calculation
 import pytest
 import symengine as se
 
 q1 = se.Symbol("q1")
 q2 = se.Symbol("q2")
-R = se.Matrix([[se.cos(q1+q2), -se.sin(q1+q2), 0],[se.sin(q1+q2), se.cos(q1+q2), 0],[0, 0, 1]])
+R_m = se.Matrix([[se.cos(q1+q2), -se.sin(q1+q2), 0],[se.sin(q1+q2), se.cos(q1+q2), 0],[0, 0, 1]])
+R = Calculation()
+R.addCalculation(se.Symbol("R"), R_m)
+simple = Calculation()
+simple.addCalculation(se.Symbol("x"), q1+q2)
+
+def test_CodeElement_single_line():
+    ce =  CodeElement(simple)
+    assert ce.generateCode() =="x = q1 + q2;\n\n"
 
 def test_CodeElement_standard():
-    ce =  CodeElement(R, "R")
-    assert ce.generateCode() =="x0 = q1 + q2;\nx1 = cos(x0);\nx2 = sin(x0);\n\nR = [x1 -x2 0; x2 x1 0; 0 0 1];\n\nclear x0 x1 x2;\n"
+    ce =  CodeElement(R)
+    assert ce.generateCode() =="x0 = q1 + q2;\nx1 = cos(x0);\nx2 = sin(x0);\n\nR = [x1 -x2 0; x2 x1 0; 0 0 1];\nclear x0 x1 x2;\n"
+
 
 def test_CodeElement_indents():
-    ce =  CodeElement(R, "R", indent=1)
-    assert ce.generateCode() =="\tx0 = q1 + q2;\n\tx1 = cos(x0);\n\tx2 = sin(x0);\n\n\tR = [x1 -x2 0; x2 x1 0; 0 0 1];\n\n\tclear x0 x1 x2;\n"
+    ce =  CodeElement(R, indent=1)
+    assert ce.generateCode() =="\tx0 = q1 + q2;\n\tx1 = cos(x0);\n\tx2 = sin(x0);\n\n\tR = [x1 -x2 0; x2 x1 0; 0 0 1];\n\tclear x0 x1 x2;\n"
 
 def test_CodeElement_no_cse():
-    ce =  CodeElement(R, "R", use_cse=False)
+    ce =  CodeElement(R, use_cse=False)
     assert ce.generateCode() =="R = [cos(q1 + q2) -sin(q1 + q2) 0; sin(q1 + q2) cos(q1 + q2) 0; 0 0 1];\n"
 
 def test_CodeElement_clear():
-    ce = CodeElement(R, "R",  clear=False)
-    assert ce.generateCode() =="x0 = q1 + q2;\nx1 = cos(x0);\nx2 = sin(x0);\n\nR = [x1 -x2 0; x2 x1 0; 0 0 1];\n\n"
+    ce = CodeElement(R,  clear=False)
+    s = ce.generateCode()
+    assert ce.generateCode() =="x0 = q1 + q2;\nx1 = cos(x0);\nx2 = sin(x0);\n\nR = [x1 -x2 0; x2 x1 0; 0 0 1];\n"
```

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/tests/test_DynamicSymbol.py` & `system_to_matlab-0.0.5/System_to_Matlab/tests/test_DynamicSymbol.py`

 * *Files identical despite different names*

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab/tests/test_StaticSymbol.py` & `system_to_matlab-0.0.5/System_to_Matlab/tests/test_StaticSymbol.py`

 * *Files identical despite different names*

### Comparing `System_to_Matlab-0.0.4/System_to_Matlab.egg-info/SOURCES.txt` & `system_to_matlab-0.0.5/System_to_Matlab.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 pyproject.toml
 System_to_Matlab/__init__.py
 System_to_Matlab.egg-info/PKG-INFO
 System_to_Matlab.egg-info/SOURCES.txt
 System_to_Matlab.egg-info/dependency_links.txt
 System_to_Matlab.egg-info/requires.txt
 System_to_Matlab.egg-info/top_level.txt
+System_to_Matlab/Calculation/Calculation.py
+System_to_Matlab/Calculation/__init__.py
 System_to_Matlab/FileGenerators/FileGenerators.py
 System_to_Matlab/FileGenerators/MFile.py
 System_to_Matlab/FileGenerators/MFunction.py
 System_to_Matlab/FileGenerators/SFunction.py
 System_to_Matlab/FileGenerators/__init__.py
 System_to_Matlab/FileGenerators/MatlabElements/CodeElement.py
 System_to_Matlab/FileGenerators/MatlabElements/MatlabElement.py
@@ -20,13 +22,16 @@
 System_to_Matlab/HelperFunctions/__init__.py
 System_to_Matlab/Symbols/DynamicSymbol.py
 System_to_Matlab/Symbols/StaticSymbol.py
 System_to_Matlab/Symbols/Symbol.py
 System_to_Matlab/Symbols/__init__.py
 System_to_Matlab/Systems/DynamicSystem.py
 System_to_Matlab/Systems/StaticSystem.py
-System_to_Matlab/Systems/System.py
+System_to_Matlab/Systems/_System.py
 System_to_Matlab/Systems/__init__.py
+System_to_Matlab/tests/test_Calculation.py
 System_to_Matlab/tests/test_CodeElement.py
 System_to_Matlab/tests/test_DynamicSymbol.py
+System_to_Matlab/tests/test_DynamicSystem.py
 System_to_Matlab/tests/test_StaticSymbol.py
+System_to_Matlab/tests/test_StaticSystem.py
 System_to_Matlab/tests/test_StringElement.py
```

