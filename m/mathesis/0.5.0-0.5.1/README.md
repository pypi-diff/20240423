# Comparing `tmp/mathesis-0.5.0.tar.gz` & `tmp/mathesis-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathesis-0.5.0.tar", max compression
+gzip compressed data, was "mathesis-0.5.1.tar", max compression
```

## Comparing `mathesis-0.5.0.tar` & `mathesis-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1070 2023-08-04 21:07:27.713958 mathesis-0.5.0/LICENSE.md
--rw-r--r--   0        0        0     2876 2023-11-09 17:38:29.832886 mathesis-0.5.0/README.md
--rw-r--r--   0        0        0      146 2022-05-12 17:46:19.512866 mathesis-0.5.0/mathesis/_utils.py
--rw-r--r--   0        0        0     2384 2023-09-29 06:35:16.972979 mathesis-0.5.0/mathesis/deduction/hilbert/axioms.py
--rw-r--r--   0        0        0     3480 2023-09-29 07:54:06.732725 mathesis-0.5.0/mathesis/deduction/hilbert/hilbert.py
--rw-r--r--   0        0        0      780 2023-09-29 07:53:26.486577 mathesis-0.5.0/mathesis/deduction/hilbert/rules.py
--rw-r--r--   0        0        0       74 2023-10-26 11:59:47.260570 mathesis-0.5.0/mathesis/deduction/natural_deduction/__init__.py
--rw-r--r--   0        0        0     2579 2023-11-09 17:26:42.303514 mathesis-0.5.0/mathesis/deduction/natural_deduction/natural_deduction.py
--rw-r--r--   0        0        0    13029 2023-11-09 17:13:17.278679 mathesis-0.5.0/mathesis/deduction/natural_deduction/rules.py
--rw-r--r--   0        0        0      113 2022-05-12 19:45:36.985648 mathesis-0.5.0/mathesis/deduction/sequent_calculus/__init__.py
--rw-r--r--   0        0        0     6777 2023-11-09 17:27:00.545224 mathesis-0.5.0/mathesis/deduction/sequent_calculus/rules.py
--rw-r--r--   0        0        0     4934 2023-11-09 17:27:04.490250 mathesis-0.5.0/mathesis/deduction/sequent_calculus/sequents.py
--rw-r--r--   0        0        0       49 2022-05-14 07:29:25.418347 mathesis-0.5.0/mathesis/deduction/tableau/__init__.py
--rw-r--r--   0        0        0     6371 2023-10-26 17:55:18.651296 mathesis-0.5.0/mathesis/deduction/tableau/rules.py
--rw-r--r--   0        0        0     6025 2023-10-26 11:15:21.360471 mathesis-0.5.0/mathesis/deduction/tableau/signed_rules.py
--rw-r--r--   0        0        0     5134 2023-11-09 08:53:56.188153 mathesis-0.5.0/mathesis/deduction/tableau/tableau.py
--rw-r--r--   0        0        0     6232 2023-10-31 06:47:08.032242 mathesis-0.5.0/mathesis/forms.py
--rw-r--r--   0        0        0     2921 2023-08-04 19:49:30.463359 mathesis-0.5.0/mathesis/grammars.py
--rw-r--r--   0        0        0     7580 2023-10-26 06:36:45.730363 mathesis-0.5.0/mathesis/semantics/model.py
--rw-r--r--   0        0        0      241 2023-10-26 06:22:19.672722 mathesis-0.5.0/mathesis/semantics/truth_table/__init__.py
--rw-r--r--   0        0        0     8070 2023-10-26 07:54:43.138198 mathesis-0.5.0/mathesis/semantics/truth_table/base.py
--rw-r--r--   0        0        0     1238 2023-10-26 05:46:33.904826 mathesis-0.5.0/mathesis/semantics/truth_table/classical.py
--rw-r--r--   0        0        0     1614 2023-10-26 06:25:40.945276 mathesis-0.5.0/mathesis/semantics/truth_table/k3.py
--rw-r--r--   0        0        0     1555 2023-10-26 05:47:55.982258 mathesis-0.5.0/mathesis/semantics/truth_table/lp.py
--rw-r--r--   0        0        0     2829 2023-08-04 19:49:30.463395 mathesis-0.5.0/mathesis/solvers.py
--rw-r--r--   0        0        0       50 2023-08-02 11:09:18.327468 mathesis-0.5.0/mathesis/system/classical/__init__.py
--rw-r--r--   0        0        0      171 2023-08-04 21:27:31.502226 mathesis-0.5.0/mathesis/system/classical/truth_table.py
--rw-r--r--   0        0        0       60 2023-10-26 16:56:11.949136 mathesis-0.5.0/mathesis/system/intuitionistic/__init__.py
--rw-r--r--   0        0        0       60 2023-10-26 16:57:49.711693 mathesis-0.5.0/mathesis/system/intuitionistic/sequent_calculus/__init__.py
--rw-r--r--   0        0        0     3291 2023-10-26 17:20:44.650963 mathesis-0.5.0/mathesis/system/intuitionistic/sequent_calculus/rules.py
--rw-r--r--   0        0        0      122 2023-09-29 04:56:47.125983 mathesis-0.5.0/mathesis/truth_values/__init__.py
--rw-r--r--   0        0        0       85 2023-09-29 04:50:01.846232 mathesis-0.5.0/mathesis/truth_values/boolean.py
--rw-r--r--   0        0        0      248 2023-09-29 04:55:54.872616 mathesis-0.5.0/mathesis/truth_values/numeric.py
--rw-r--r--   0        0        0      968 2023-11-09 18:00:34.465948 mathesis-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 mathesis-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-23 17:19:50.797509 mathesis-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     2876 2024-04-23 17:19:50.797837 mathesis-0.5.1/README.md
+-rw-r--r--   0        0        0      146 2024-04-23 17:19:50.803132 mathesis-0.5.1/mathesis/_utils.py
+-rw-r--r--   0        0        0     2384 2024-04-23 17:19:50.803524 mathesis-0.5.1/mathesis/deduction/hilbert/axioms.py
+-rw-r--r--   0        0        0     3480 2024-04-23 17:19:50.803931 mathesis-0.5.1/mathesis/deduction/hilbert/hilbert.py
+-rw-r--r--   0        0        0      780 2024-04-23 17:19:50.804252 mathesis-0.5.1/mathesis/deduction/hilbert/rules.py
+-rw-r--r--   0        0        0       82 2024-04-23 17:19:50.804520 mathesis-0.5.1/mathesis/deduction/natural_deduction/__init__.py
+-rw-r--r--   0        0        0     2579 2024-04-23 17:19:50.804824 mathesis-0.5.1/mathesis/deduction/natural_deduction/natural_deduction.py
+-rw-r--r--   0        0        0    13029 2024-04-23 17:19:50.805110 mathesis-0.5.1/mathesis/deduction/natural_deduction/rules.py
+-rw-r--r--   0        0        0      113 2024-04-23 17:19:50.805463 mathesis-0.5.1/mathesis/deduction/sequent_calculus/__init__.py
+-rw-r--r--   0        0        0     6777 2024-04-23 17:19:50.805834 mathesis-0.5.1/mathesis/deduction/sequent_calculus/rules.py
+-rw-r--r--   0        0        0     4998 2024-04-23 17:19:50.806269 mathesis-0.5.1/mathesis/deduction/sequent_calculus/sequents.py
+-rw-r--r--   0        0        0       49 2024-04-23 17:19:50.806555 mathesis-0.5.1/mathesis/deduction/tableau/__init__.py
+-rw-r--r--   0        0        0     6371 2024-04-23 17:19:50.806855 mathesis-0.5.1/mathesis/deduction/tableau/rules.py
+-rw-r--r--   0        0        0     6025 2024-04-23 17:19:50.807249 mathesis-0.5.1/mathesis/deduction/tableau/signed_rules.py
+-rw-r--r--   0        0        0     5134 2024-04-23 17:19:50.807536 mathesis-0.5.1/mathesis/deduction/tableau/tableau.py
+-rw-r--r--   0        0        0     6316 2024-04-23 17:19:50.807954 mathesis-0.5.1/mathesis/forms.py
+-rw-r--r--   0        0        0     3199 2024-04-23 17:19:50.808274 mathesis-0.5.1/mathesis/grammars.py
+-rw-r--r--   0        0        0     7637 2024-04-23 17:19:50.808817 mathesis-0.5.1/mathesis/semantics/model.py
+-rw-r--r--   0        0        0      241 2024-04-23 17:19:50.809165 mathesis-0.5.1/mathesis/semantics/truth_table/__init__.py
+-rw-r--r--   0        0        0     8080 2024-04-23 17:19:50.809524 mathesis-0.5.1/mathesis/semantics/truth_table/base.py
+-rw-r--r--   0        0        0     1238 2024-04-23 17:19:50.809832 mathesis-0.5.1/mathesis/semantics/truth_table/classical.py
+-rw-r--r--   0        0        0     1614 2024-04-23 17:19:50.810115 mathesis-0.5.1/mathesis/semantics/truth_table/k3.py
+-rw-r--r--   0        0        0     1555 2024-04-23 17:19:50.810363 mathesis-0.5.1/mathesis/semantics/truth_table/lp.py
+-rw-r--r--   0        0        0     2759 2024-04-23 17:19:50.810733 mathesis-0.5.1/mathesis/solvers.py
+-rw-r--r--   0        0        0       50 2024-04-23 17:19:50.811061 mathesis-0.5.1/mathesis/system/classical/__init__.py
+-rw-r--r--   0        0        0      171 2024-04-23 17:19:50.811363 mathesis-0.5.1/mathesis/system/classical/truth_table.py
+-rw-r--r--   0        0        0       60 2024-04-23 17:19:50.811672 mathesis-0.5.1/mathesis/system/intuitionistic/__init__.py
+-rw-r--r--   0        0        0       60 2024-04-23 17:19:50.811942 mathesis-0.5.1/mathesis/system/intuitionistic/sequent_calculus/__init__.py
+-rw-r--r--   0        0        0     3291 2024-04-23 17:19:50.812244 mathesis-0.5.1/mathesis/system/intuitionistic/sequent_calculus/rules.py
+-rw-r--r--   0        0        0      122 2024-04-23 17:19:50.812606 mathesis-0.5.1/mathesis/truth_values/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-23 17:19:50.812887 mathesis-0.5.1/mathesis/truth_values/boolean.py
+-rw-r--r--   0        0        0      248 2024-04-23 17:19:50.813227 mathesis-0.5.1/mathesis/truth_values/numeric.py
+-rw-r--r--   0        0        0      936 2024-04-23 17:24:17.016193 mathesis-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 mathesis-0.5.1/PKG-INFO
```

### Comparing `mathesis-0.5.0/LICENSE.md` & `mathesis-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/README.md` & `mathesis-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/hilbert/axioms.py` & `mathesis-0.5.1/mathesis/deduction/hilbert/axioms.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/hilbert/hilbert.py` & `mathesis-0.5.1/mathesis/deduction/hilbert/hilbert.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/hilbert/rules.py` & `mathesis-0.5.1/mathesis/deduction/hilbert/rules.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/natural_deduction/natural_deduction.py` & `mathesis-0.5.1/mathesis/deduction/natural_deduction/natural_deduction.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/natural_deduction/rules.py` & `mathesis-0.5.1/mathesis/deduction/natural_deduction/rules.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/sequent_calculus/rules.py` & `mathesis-0.5.1/mathesis/deduction/sequent_calculus/rules.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/sequent_calculus/sequents.py` & `mathesis-0.5.1/mathesis/deduction/sequent_calculus/sequents.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from copy import copy, deepcopy
 from itertools import count
 from operator import itemgetter
 from types import SimpleNamespace
 from typing import List
 
 from anytree import Node, NodeMixin, PostOrderIter, RenderTree
@@ -88,15 +90,17 @@
         )
 
 
 class SequentItem:
     n = None
     sequent = None
 
-    def __init__(self, fml: Formula, sign, n: int = None, sequent: Sequent = None):
+    def __init__(
+        self, fml: Formula, sign, n: int | None = None, sequent: Sequent | None = None
+    ):
         self.fml = fml
         self.sign = sign
         self.n = n
         self.sequent = sequent
 
     def clone(self):
         clone = deepcopy(self)
```

### Comparing `mathesis-0.5.0/mathesis/deduction/tableau/rules.py` & `mathesis-0.5.1/mathesis/deduction/tableau/rules.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/tableau/signed_rules.py` & `mathesis-0.5.1/mathesis/deduction/tableau/signed_rules.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/deduction/tableau/tableau.py` & `mathesis-0.5.1/mathesis/deduction/tableau/tableau.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/forms.py` & `mathesis-0.5.1/mathesis/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def transform(self, transformer):
         return transformer(self)
 
 
 class Atom(Formula):
     def __init__(self, constant_or_nonzero: str | list):
-        if type(constant_or_nonzero) is list:
+        if isinstance(constant_or_nonzero, list):
             self.predicate, self.terms = (
                 str(constant_or_nonzero[0]),
                 tuple(map(str, constant_or_nonzero[1:])),
             )
         else:
             constant = constant_or_nonzero
             self.predicate = str(constant)
@@ -102,14 +102,16 @@
 class Negation(Unary):
     signature = "Neg"
     connective = "¬"
     connective_latex = r"\neg"
 
 
 class Binary(Formula):
+    subs: tuple[Formula, Formula]
+
     def __init__(self):
         pass
 
     def clone(self):
         clones = [sub.clone() for sub in self.subs]
         for clone in clones:
             clone.__dict__ = deepcopy(clone.__dict__)
@@ -164,34 +166,34 @@
 
 
 class Conjunction(Binary):
     signature = "Conj"
     connective = "∧"
     connective_latex = r"\land"
 
-    def __init__(self, *subs: tuple[Formula]):
-        self.subs = subs
+    def __init__(self, sub1: Formula, sub2: Formula):
+        self.subs = (sub1, sub2)
 
 
 class Disjunction(Binary):
     signature = "Disj"
     connective = "∨"
     connective_latex = r"\lor"
 
-    def __init__(self, *subs: tuple[Formula]):
-        self.subs = subs
+    def __init__(self, sub1: Formula, sub2: Formula):
+        self.subs = (sub1, sub2)
 
 
 class Conditional(Binary):
     signature = "Cond"
     connective = "→"
     connective_latex = r"\to"
 
-    def __init__(self, *subs: tuple[Formula]):
-        self.subs = subs
+    def __init__(self, sub1: Formula, sub2: Formula):
+        self.subs = (sub1, sub2)
 
 
 class Quantifier(Formula):
     def __init__(self, term, sub: Formula):
         self.variable = term
         self.sub = sub
```

### Comparing `mathesis-0.5.0/mathesis/grammars.py` & `mathesis-0.5.1/mathesis/grammars.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 from __future__ import annotations
 
-from abc import ABC, abstractmethod
+from abc import ABC
 
 from lark import Lark, Transformer
 
-from mathesis.forms import *
+from mathesis.forms import (
+    Atom,
+    Conditional,
+    Conjunction,
+    Disjunction,
+    Negation,
+    Particular,
+    Universal,
+)
 
 
 class ToFml(Transformer):
     def atom(self, v):
         if len(v) == 1:
             return Atom(*v)
         else:
@@ -30,27 +38,31 @@
         return Disjunction(*v)
 
     def conditional(self, v):
         return Conditional(*v)
 
 
 class Grammar(ABC):
+    """Abstract class for grammars."""
+
+    grammar_rules: str
+
     def __repr__(self):
         return self.grammar_rules
 
-    @abstractmethod
-    def parse(self, text_or_list: str | list):
-        raise NotImplementedError()
+    # @abstractmethod
+    # def parse(self, text_or_list: str | list):
+    #     raise NotImplementedError()
 
     def __init__(self):
         self.grammar = Lark(self.grammar_rules, start="fml")
 
     def parse(self, text_or_list: str | list):
         # print(fml_strings)
-        if type(text_or_list) is list:
+        if isinstance(text_or_list, list):
             fml_strings = text_or_list
             fmls = []
             for fml_string in fml_strings:
                 tree = self.grammar.parse(fml_string)
                 fml = ToFml().transform(tree)
                 fmls.append(fml)
             return fmls
@@ -58,14 +70,16 @@
             fml_string = text_or_list
             tree = self.grammar.parse(fml_string)
             fml = ToFml().transform(tree)
             return fml
 
 
 class BasicPropositionalGrammar(Grammar):
+    """Basic grammar for the propositional language."""
+
     grammar_rules = r"""
 ?fml: conjunction
     | disjunction
     | conditional
     | negation
     | atom
     | _subfml
@@ -91,14 +105,16 @@
         self.grammar_rules = self.grammar_rules.format(
             conditional_symbol=symbols["conditional"]
         )
         super().__init__()
 
 
 class BasicGrammar(BasicPropositionalGrammar):
+    """Basic grammar for the first-order language."""
+
     grammar_rules = r"""
 ?fml: conjunction
     | disjunction
     | conditional
     | negation
     | universal
     | particular
```

### Comparing `mathesis-0.5.0/mathesis/semantics/model.py` & `mathesis-0.5.1/mathesis/semantics/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+from __future__ import annotations
+
 from itertools import permutations
-from typing import Any, Callable, Dict, List, Set, Tuple
+from typing import Any, Callable, Set
 
 from mathesis import forms
 from mathesis.semantics.truth_table import classical as truth_table
 
 
 def normalize_predicates(predicates):
     return dict(
         map(
-            lambda x: (x[0], tuple((v,) for v in x[1]))
-            if (len(x[1]) > 0 and type(list(x[1])[0]) is not tuple)
-            else x,
+            lambda x: (
+                (x[0], tuple((v,) for v in x[1]))
+                if (len(x[1]) > 0 and type(list(x[1])[0]) is not tuple)
+                else x
+            ),
             predicates.items(),
         )
     )
 
 
 class Model:
     def __init__(
         self,
         domain: Set[Any] = set(),
-        predicates: Dict[str, Set[Any]] = dict(),
-        constants: Dict[str, Any] = dict(),
-        functions: Dict[str, Callable] = dict(),
+        predicates: dict[str, Set[Any]] = dict(),
+        constants: dict[str, Any] = dict(),
+        functions: dict[str, Callable] = dict(),
     ):
         """
         Args:
             domain (Set): a set of objects
-            predicates (Dict): a dictionary with predicate symbols as keys and sets of tuples of objects as values,
+            predicates (dict): a dictionary with predicate symbols as keys and sets of tuples of objects as values,
                 or a function that assigns sets of tuples of objects to predicate symbols
-            constants (Dict): a dictionary with constant symbols as keys and objects as values,
+            constants (dict): a dictionary with constant symbols as keys and objects as values,
                 or a function that assigns objects to constants
-            functions (Dict): a dictionary with function symbols as keys and functions over domain as values
+            functions (dict): a dictionary with function symbols as keys and functions over domain as values
         """
         self.domain = domain
         # Make sure that the value of a predicate is a list of tuples
         predicates = normalize_predicates(predicates)
         self.predicates = predicates
         self.constants = constants
         self.functions = functions
@@ -44,21 +48,21 @@
 
     # def assign_term_denotation(self, term):
     #     if term in self.variables:
     #         pass
     #     elif term in self.constants:
     #         return self.denotations.get(term, term)
 
-    def valuate(self, fml: forms.Formula, variable_assignment: Dict[str, Any] = dict()):
+    def valuate(self, fml: forms.Formula, variable_assignment: dict[str, Any] = dict()):
         """
         Valuates a formula in a model.
 
         Args:
             fml (Formula): a formula
-            variable_assignment (Dict): a dictionary with variable symbols as keys and assigned objects as values
+            variable_assignment (dict): a dictionary with variable symbols as keys and assigned objects as values
         """
         if isinstance(fml, forms.Atom):
             # Denotations of the terms, a list to be converted to a tuple
             term_denotations = []
 
             # Iterate over all terms in the formula
             for term in fml.terms:
```

### Comparing `mathesis-0.5.0/mathesis/semantics/truth_table/base.py` & `mathesis-0.5.1/mathesis/semantics/truth_table/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from __future__ import annotations
+
 import logging
 from itertools import permutations, product
-from typing import List, Set
 
 from anytree import Node, NodeMixin, PostOrderIter, RenderTree
-from prettytable import PrettyTable, PLAIN_COLUMNS
+from prettytable import PLAIN_COLUMNS, PrettyTable
 
 from mathesis import forms
 
-logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
+_logger = logging.getLogger(__name__)
+_logger.addHandler(logging.NullHandler())
 
 
 class ConnectiveClause:
-    column_names: List[str]
+    column_names: list[str]
     table: dict
     truth_value_symbols: None
 
     def __init__(self, truth_value_symbols=None) -> None:
         self.truth_value_symbols = truth_value_symbols
 
     def apply(self, *values):
@@ -93,67 +94,67 @@
     def __str__(self):
         return f"{str(self.fml)} = {self.truth_value}"
 
 
 class TruthTable:
     """The truth table class."""
 
-    truth_values: Set = (set(),)
-    designated_values: Set = (set(),)
+    truth_values: set = set()
+    designated_values: set = set()
     clauses = {}
 
     def __init__(
         self,
-        formula_or_premises: List[forms.Formula],
-        conclusions: List[forms.Formula] = [],
+        formula_or_premises: list[forms.Formula],
+        conclusions: list[forms.Formula] = [],
     ):
-        if type(formula_or_premises) is list:
+        if isinstance(formula_or_premises, list):
             raise NotImplementedError()
         else:
             self.premises = [formula_or_premises]
 
         self.conclusions = conclusions
 
     def __str__(self):
         return self.to_string()
 
     def compute_truth_value(self, assigned_node):
         if isinstance(assigned_node.fml, forms.Atom):
             # assigned_node.truth_value = assigned_node._truth_value
             pass
         elif isinstance(assigned_node.fml, forms.Negation):
-            if not forms.Negation in self.clauses:
+            if forms.Negation not in self.clauses:
                 raise NotImplementedError("Negation clause not implemented")
             assigned_node.truth_value = self.clauses[forms.Negation].apply(
                 assigned_node.children[0].truth_value
             )
         elif isinstance(assigned_node.fml, forms.Conjunction):
-            if not forms.Conjunction in self.clauses:
+            if forms.Conjunction not in self.clauses:
                 raise NotImplementedError("Conjunction clause not implemented")
             assigned_node.truth_value = self.clauses[forms.Conjunction].apply(
                 *tuple(child.truth_value for child in assigned_node.children)
             )
         elif isinstance(assigned_node.fml, forms.Disjunction):
-            if not forms.Disjunction in self.clauses:
+            if forms.Disjunction not in self.clauses:
                 raise NotImplementedError("Disjunction clause not implemented")
             assigned_node.truth_value = self.clauses[forms.Disjunction].apply(
                 *tuple(child.truth_value for child in assigned_node.children)
             )
         elif isinstance(assigned_node.fml, forms.Conditional):
-            if not forms.Conditional in self.clauses:
+            if forms.Conditional not in self.clauses:
                 raise NotImplementedError("Conditional clause not implemented")
             assigned_node.truth_value = self.clauses[forms.Conditional].apply(
                 *tuple(child.truth_value for child in assigned_node.children)
             )
         else:
             raise NotImplementedError(
                 f"Clause for {type(assigned_node.fml)} not implemented"
             )
 
-    def wrap_fml(self, fml):
+    def _wrap_fml(self, fml):
         def transformer(fml):
             node = AssignedNode(str(fml), fml=fml)
             if isinstance(fml, forms.Binary):
                 node.children = [transformer(subfml) for subfml in fml.subs]
             elif isinstance(fml, forms.Unary):
                 node.children = [transformer(fml.sub)]
             # NOTE: No truth table for quantifiers
@@ -167,15 +168,15 @@
     def is_valid(self):
         for fml in self.premises + self.conclusions:
             atom_symbols = fml.atoms.keys()
             atom_symbols = sorted(atom_symbols)
             values = []
             for tv in product(self.truth_values, repeat=len(atom_symbols)):
                 assignments = dict(zip(atom_symbols, tv))
-                tv_fml = self.wrap_fml(fml)
+                tv_fml = self._wrap_fml(fml)
                 tv_fml.assign_atom_values(assignments)
                 for node in PostOrderIter(tv_fml):
                     self.compute_truth_value(node)
                 values.append(tv_fml.truth_value)
             if all([value in self.designated_values for value in values]):
                 return True
             else:
@@ -190,15 +191,15 @@
         table.format = True
 
         for fml in self.premises + self.conclusions:
             atom_symbols = fml.atoms.keys()
             atom_symbols = sorted(atom_symbols)
             for tv in product(self.truth_values, repeat=len(atom_symbols)):
                 assignments = dict(zip(atom_symbols, tv))
-                tree = self.wrap_fml(fml)
+                tree = self._wrap_fml(fml)
                 # print(RenderTree(tree))
                 tree.assign_atom_values(assignments)
                 # print(tree.truth_value)
                 # print(RenderTree(tree))
                 field_names = []
                 row = []
                 for node in PostOrderIter(tree):
```

### Comparing `mathesis-0.5.0/mathesis/semantics/truth_table/classical.py` & `mathesis-0.5.1/mathesis/semantics/truth_table/classical.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/semantics/truth_table/k3.py` & `mathesis-0.5.1/mathesis/semantics/truth_table/k3.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/semantics/truth_table/lp.py` & `mathesis-0.5.1/mathesis/semantics/truth_table/lp.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/mathesis/solvers.py` & `mathesis-0.5.1/mathesis/solvers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import logging
 from collections import namedtuple
-from operator import itemgetter
 from typing import List
 
-from anytree import Node, RenderTree
-
 from mathesis import forms
 from mathesis.deduction.tableau import Tableau, rules
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
```

### Comparing `mathesis-0.5.0/mathesis/system/intuitionistic/sequent_calculus/rules.py` & `mathesis-0.5.1/mathesis/system/intuitionistic/sequent_calculus/rules.py`

 * *Files identical despite different names*

### Comparing `mathesis-0.5.0/pyproject.toml` & `mathesis-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mathesis"
-version = "0.5.0"
+version = "0.5.1"
 description = "Formal logic library in Python for humans"
 authors = ["Kentaro Ozeki <32771324+ozekik@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://mathesis.readthedocs.io/"
 repository = "https://github.com/ozekik/mathesis"
 keywords = ['logic', 'semantics', 'proof', 'philosophy']
 license = "MIT"
@@ -20,15 +20,14 @@
 ipykernel = "^6.13.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.1"
 mkdocs-material = "^9.1.21"
 mkdocstrings-python = "^1.2.1"
 mkdocs-exclude = "^1.0.2"
-markdown-exec = { extras = ["ansi"], version = "^1.6.0" }
+markdown-exec = { extras = ["ansi"], version = "^1.8.1" }
 mkdocs-jupyter = "^0.24.5"
-notebook = "^6.5.6"
-jupyter-contrib-nbextensions = "^0.7.0"
+griffe-typingdoc = "^0.2.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mathesis-0.5.0/PKG-INFO` & `mathesis-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: mathesis
-Version: 0.5.0
+Version: 0.5.1
 Summary: Formal logic library in Python for humans
 Home-page: https://mathesis.readthedocs.io/
 License: MIT
 Keywords: logic,semantics,proof,philosophy
 Author: Kentaro Ozeki
 Author-email: 32771324+ozekik@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: anytree (>=2.8.0,<3.0.0)
 Requires-Dist: lark (>=1.1.2,<2.0.0)
 Requires-Dist: prettytable (>=3.3.0,<4.0.0)
 Project-URL: Repository, https://github.com/ozekik/mathesis
 Description-Content-Type: text/markdown
 
 # Mathesis
```

