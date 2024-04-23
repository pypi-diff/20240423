# Comparing `tmp/pynumstim-0.2.7.tar.gz` & `tmp/pynumstim-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumstim-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynumstim-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynumstim-0.2.7.tar` & `pynumstim-0.2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.7/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.7/LICENSE
--rw-r--r--   0        0        0      675 2024-04-15 14:25:22.348690 pynumstim-0.2.7/README.md
--rw-r--r--   0        0        0      362 2024-04-20 11:24:43.126941 pynumstim-0.2.7/pynumstim/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-18 16:18:12.229886 pynumstim-0.2.7/pynumstim/_data_sets.py
--rw-r--r--   0        0        0    12942 2024-04-20 11:24:17.654382 pynumstim-0.2.7/pynumstim/_mplist.py
--rw-r--r--   0        0        0     3344 2024-04-18 14:51:30.308979 pynumstim-0.2.7/pynumstim/_number.py
--rw-r--r--   0        0        0     9720 2024-04-18 17:53:40.832655 pynumstim-0.2.7/pynumstim/_problem.py
--rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.7/pynumstim/datasets/Ahren_Jackson_79.toml
--rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.7/pynumstim/datasets/Lindemann_Tira_10.toml
--rw-r--r--   0        0        0     4513 2024-04-18 16:18:12.229886 pynumstim-0.2.7/pynumstim/image.py
--rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.7/pyproject.toml
--rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.7/trial_list.txt
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 pynumstim-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.8/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.8/LICENSE
+-rw-r--r--   0        0        0      675 2024-04-15 14:25:22.348690 pynumstim-0.2.8/README.md
+-rw-r--r--   0        0        0      362 2024-04-23 12:41:46.894010 pynumstim-0.2.8/pynumstim/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-18 16:18:12.229886 pynumstim-0.2.8/pynumstim/_data_sets.py
+-rw-r--r--   0        0        0    13077 2024-04-23 12:41:46.894010 pynumstim-0.2.8/pynumstim/_mplist.py
+-rw-r--r--   0        0        0     3344 2024-04-18 14:51:30.308979 pynumstim-0.2.8/pynumstim/_number.py
+-rw-r--r--   0        0        0     9720 2024-04-20 15:57:27.525304 pynumstim-0.2.8/pynumstim/_problem.py
+-rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.8/pynumstim/datasets/Ahren_Jackson_79.toml
+-rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.8/pynumstim/datasets/Lindemann_Tira_10.toml
+-rw-r--r--   0        0        0     4513 2024-04-18 16:18:12.229886 pynumstim-0.2.8/pynumstim/image.py
+-rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.8/trial_list.txt
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 pynumstim-0.2.8/PKG-INFO
```

### Comparing `pynumstim-0.2.7/.gitignore` & `pynumstim-0.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/LICENSE` & `pynumstim-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/README.md` & `pynumstim-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/pynumstim/_data_sets.py` & `pynumstim-0.2.8/pynumstim/_data_sets.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/pynumstim/_mplist.py` & `pynumstim-0.2.8/pynumstim/_mplist.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 from ._problem import MathProblem, TProperties
 
 
 class MathProblemList(object):
 
     def __init__(self):
         self._list: List[MathProblem] = []
-        self.number_types: Set[type] = set() # involved number types
+        self.number_types: Set[type] = set()  # involved number types
 
     def __str__(self):
         rtn = ""
         for x in self._list:
             rtn += str(x) + "\n"
         return rtn
 
     @property
     def list(self) -> List[MathProblem]:
         return self._list
 
     @list.setter
-    def list(self, val:List[MathProblem]):
+    def list(self, val: List[MathProblem]):
         self._list = val
         self.number_types: Set[type] = set()
         for x in self._list:
             self.number_types = self.number_types | x.number_types
 
     def append(self, problem: Union[MathProblem, MathProblemList]):
         if isinstance(problem, MathProblem):
@@ -52,30 +52,30 @@
             properties: Optional[Optional[TProperties]] = None):
 
         self.append(MathProblem(operand1=first_operand, operation=operation,
                                 operand2=second_operand, result=result,
                                 properties=properties))
 
     def get_random(self, n: int = 1,
-                   dev_corr:Optional[int|float]=None) -> MathProblemList:
+                   dev_corr: Optional[int | float] = None) -> MathProblemList:
         """Get x random problems
 
         Optionally set results via `dev_cor`, which defined the deviation from
         correct (see `set_results`)
         """
         lst = deepcopy(self._list)
         shuffle(lst)
         rtn = MathProblemList()
         rtn.list = lst[0:n]
         if dev_corr is not None:
             rtn.set_results(dev_corr=dev_corr)
         return rtn
 
     def pop_random(self, n: int = 1,
-                   dev_corr:Optional[int|float]=None) -> MathProblemList:
+                   dev_corr: Optional[int | float] = None) -> MathProblemList:
         """Pop x random problems
 
         Optionally set results via `dev_cor`, which defined the deviation from
         correct (see `set_results`)
         """
 
         rtn = MathProblemList()
@@ -83,27 +83,26 @@
             index = randint(0, len(self._list)-1)
             p = self._list.pop(index)
             if dev_corr is not None:
                 p.result = p.calc() + dev_corr
             rtn.append(p)
         return rtn
 
-    def set_results(self, dev_corr:int|float):
+    def set_results(self, dev_corr: int | float):
         """Sets results of all problem to a value that deviation from
         correct result by `dev_corr`. Thus, `dev_corr=0` returns correct problems.
 
         Note
         ----
         Setting results does not work (yet) for fractions
-        """ # TODO
+        """  # TODO
 
         for x in range(len(self._list)):
             self._list[x].result = self._list[x].calc() + dev_corr
 
-
     def find(self,
              first_operand: Optional[TNum] = None,
              operation: Optional[str] = None,
              second_operand: Optional[TNum] = None,
              correct: Optional[bool] = None,
              result: Optional[TNum] = None,
              deviation: Optional[TNum] = None,
@@ -149,15 +148,15 @@
         rtn = MathProblemList()
         rtn.list = lst
         return rtn
 
     def shuffel(self):
         shuffle(self._list)
 
-    def update_properties(self, properties:TProperties):
+    def update_properties(self, properties: TProperties):
         """updates the properties of all problems"""
         for x in self._list:
             x.update_properties(properties)
 
     def data_frame(self,
                    first_id: Optional[int] = None,
                    problem_size=False,
@@ -172,30 +171,30 @@
         if Fraction not in self.number_types:
             if float in self.number_types:
                 t = float
             else:
                 t = int
             for x in ['op1', 'op2', 'result']:
                 rtn[x] = rtn[x].astype(t, errors='ignore', copy=False)
-        self.number_types
+
         return rtn
 
     def to_csv(self, filename: Union[Path, str],
                first_id: Optional[int] = None,
                problem_size=False,
                n_carry=False,
-               rounding_digits:int=2) -> pd.DataFrame:
+               rounding_digits: int = 2,
+               sep: str = '\t') -> pd.DataFrame:
         """pandas data frame, includes problem ids, if first_id is defined"""
         df = self.data_frame(
             first_id=first_id, problem_size=problem_size, n_carry=n_carry)
         df = df.round(rounding_digits)
-        df.to_csv(filename, sep="\t", index=False, lineterminator="\n")
+        df.to_csv(filename, sep=sep, index=False, lineterminator="\n")
         return df
 
-
     def import_toml(self, filename: Union[Path, str]):
         """imports toml
 
         the following methods exist (illustrated by toml representation):
         method a:
 
             [category]
@@ -218,15 +217,15 @@
 
         Args:
             problem_dict: _description_
             sections: _description_. Defaults to None.
         """
         return self.import_dict(toml.load(filename))
 
-    def import_markdown_text(self, text:str):
+    def import_markdown_text(self, text: str):
         """important markdown text.
 
         see also
         --------
         `import_markdown`
         """
         curr_cat = None
@@ -286,31 +285,31 @@
             if 'op1' in d and 'op2' in d and 'operation' in d:
                 for op1 in d['op1']:
                     for op2 in d['op2']:
                         p = MathProblem(op1, d['operation'], op2,
                                         properties=prop)
                         self.append(p)
 
-    def import_data_frame(self, df:pd.DataFrame):
+    def import_data_frame(self, df: pd.DataFrame):
         for _, row in df.iterrows():
             self.add(first_operand=row['op1'],
                      operation=row['operation'],
                      second_operand=row['op2'],
                      result=row['result'])
 
     def rand_selection(self,
-            n_correct: int,
-            n_smaller: int,
-            n_larger: int,
-            dev_corr: int | float = 1,
-            dev_mean_operand: Optional[float] = None,
-            min_result:Optional[int|float] = None,
-            max_result:Optional[int|float] = None,
-            max_iterations:int = 10000
-            ) -> MathProblemList:
+                       n_correct: int,
+                       n_smaller: int,
+                       n_larger: int,
+                       dev_corr: int | float = 1,
+                       dev_mean_operand: Optional[float] = None,
+                       min_result: Optional[int | float] = None,
+                       max_result: Optional[int | float] = None,
+                       max_iterations: int = 10000
+                       ) -> MathProblemList:
         """select problems with correct and incorrect results and with a maximum
         deviation of mean operands between correct and incorrect problems
 
         min_result and max_result: the minimum and maximum value of the
         correct and incorrect results
 
         returns a new MathProblemList with a copies of the selected problems
@@ -332,38 +331,38 @@
         while True:
             if n > max_iterations:
                 raise RuntimeError("Can't find a solution")
             n = n + 1
             # smaller
             df_smaller = df.sample(n=n_smaller, replace=False)
             df_smaller['result'] = df_smaller['result'] - dev_corr
-            if min_result  and (df_smaller['result'] < min_result).any():
+            if min_result and (df_smaller['result'] < min_result).any():
                 continue
             # larger
             df_larger = df.sample(n=n_larger, replace=False)
             df_larger['result'] = df_larger['result'] + dev_corr
             if max_result and (df_larger['result'] > max_result).any():
                 continue
             # correct
             df_c = df.sample(n=n_correct, replace=False)
 
             if dev_mean_operand is not None:
                 # calc means
                 m_op = df_c['op1'].mean()
                 m_op_s = df_smaller['op1'].mean()
                 m_op_l = df_larger['op1'].mean()
-                if (abs(m_op - m_op_s) > dev_mean_operand or \
-                    abs(m_op - m_op_l) > dev_mean_operand):
+                if (abs(m_op - m_op_s) > dev_mean_operand or
+                        abs(m_op - m_op_l) > dev_mean_operand):
                     continue
 
                 m_op = df_c['op2'].mean()
                 m_op_s = df_smaller['op2'].mean()
                 m_op_l = df_larger['op2'].mean()
-                if (abs(m_op - m_op_s) > dev_mean_operand or \
-                    abs(m_op - m_op_l) > dev_mean_operand):
+                if (abs(m_op - m_op_s) > dev_mean_operand or
+                        abs(m_op - m_op_l) > dev_mean_operand):
                     continue
 
             break
 
         rtn = MathProblemList()
         rtn.import_data_frame(df_c)
         rtn.import_data_frame(df_smaller)
```

### Comparing `pynumstim-0.2.7/pynumstim/_number.py` & `pynumstim-0.2.8/pynumstim/_number.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/pynumstim/_problem.py` & `pynumstim-0.2.8/pynumstim/_problem.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/pynumstim/datasets/Lindemann_Tira_10.toml` & `pynumstim-0.2.8/pynumstim/datasets/Lindemann_Tira_10.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/pynumstim/image.py` & `pynumstim-0.2.8/pynumstim/image.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/pyproject.toml` & `pynumstim-0.2.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/trial_list.txt` & `pynumstim-0.2.8/trial_list.txt`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.7/PKG-INFO` & `pynumstim-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumstim
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python library to create symbolic number and arithmetic stimuli for psychological experiments
 Keywords: experiment control,open science,experimental psychology
 Author-email: Oliver Lindemann <lindemann@essb.eur.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

