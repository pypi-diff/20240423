# Comparing `tmp/pynumstim-0.2.8.tar.gz` & `tmp/pynumstim-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumstim-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynumstim-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynumstim-0.2.8.tar` & `pynumstim-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.8/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.8/LICENSE
--rw-r--r--   0        0        0      675 2024-04-15 14:25:22.348690 pynumstim-0.2.8/README.md
--rw-r--r--   0        0        0      362 2024-04-23 12:41:46.894010 pynumstim-0.2.8/pynumstim/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-18 16:18:12.229886 pynumstim-0.2.8/pynumstim/_data_sets.py
--rw-r--r--   0        0        0    13077 2024-04-23 12:41:46.894010 pynumstim-0.2.8/pynumstim/_mplist.py
--rw-r--r--   0        0        0     3344 2024-04-18 14:51:30.308979 pynumstim-0.2.8/pynumstim/_number.py
--rw-r--r--   0        0        0     9720 2024-04-20 15:57:27.525304 pynumstim-0.2.8/pynumstim/_problem.py
--rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.8/pynumstim/datasets/Ahren_Jackson_79.toml
--rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.8/pynumstim/datasets/Lindemann_Tira_10.toml
--rw-r--r--   0        0        0     4513 2024-04-18 16:18:12.229886 pynumstim-0.2.8/pynumstim/image.py
--rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.8/pyproject.toml
--rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.8/trial_list.txt
--rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 pynumstim-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.9/LICENSE
+-rw-r--r--   0        0        0      675 2024-04-15 14:25:22.348690 pynumstim-0.2.9/README.md
+-rw-r--r--   0        0        0      362 2024-04-23 12:46:56.918945 pynumstim-0.2.9/pynumstim/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-18 16:18:12.229886 pynumstim-0.2.9/pynumstim/_data_sets.py
+-rw-r--r--   0        0        0    13080 2024-04-23 12:46:25.974453 pynumstim-0.2.9/pynumstim/_mplist.py
+-rw-r--r--   0        0        0     3344 2024-04-18 14:51:30.308979 pynumstim-0.2.9/pynumstim/_number.py
+-rw-r--r--   0        0        0     9720 2024-04-20 15:57:27.525304 pynumstim-0.2.9/pynumstim/_problem.py
+-rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.9/pynumstim/datasets/Ahren_Jackson_79.toml
+-rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.9/pynumstim/datasets/Lindemann_Tira_10.toml
+-rw-r--r--   0        0        0      852 2024-04-23 12:46:25.974453 pynumstim-0.2.9/pynumstim/eprime.py
+-rw-r--r--   0        0        0     4513 2024-04-18 16:18:12.229886 pynumstim-0.2.9/pynumstim/image.py
+-rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.9/trial_list.txt
+-rw-r--r--   0        0        0     1377 1970-01-01 00:00:00.000000 pynumstim-0.2.9/PKG-INFO
```

### Comparing `pynumstim-0.2.8/.gitignore` & `pynumstim-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/LICENSE` & `pynumstim-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/README.md` & `pynumstim-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/pynumstim/_data_sets.py` & `pynumstim-0.2.9/pynumstim/_data_sets.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/pynumstim/_mplist.py` & `pynumstim-0.2.9/pynumstim/_mplist.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
         ----
         Setting results does not work (yet) for fractions
         """  # TODO
 
         for x in range(len(self._list)):
             self._list[x].result = self._list[x].calc() + dev_corr
 
+
     def find(self,
              first_operand: Optional[TNum] = None,
              operation: Optional[str] = None,
              second_operand: Optional[TNum] = None,
              correct: Optional[bool] = None,
              result: Optional[TNum] = None,
              deviation: Optional[TNum] = None,
@@ -184,17 +185,18 @@
                n_carry=False,
                rounding_digits: int = 2,
                sep: str = '\t') -> pd.DataFrame:
         """pandas data frame, includes problem ids, if first_id is defined"""
         df = self.data_frame(
             first_id=first_id, problem_size=problem_size, n_carry=n_carry)
         df = df.round(rounding_digits)
-        df.to_csv(filename, sep=sep, index=False, lineterminator="\n")
+        df.to_csv(filename, sep="\t", index=False, lineterminator="\n")
         return df
 
+
     def import_toml(self, filename: Union[Path, str]):
         """imports toml
 
         the following methods exist (illustrated by toml representation):
         method a:
 
             [category]
```

### Comparing `pynumstim-0.2.8/pynumstim/_number.py` & `pynumstim-0.2.9/pynumstim/_number.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/pynumstim/_problem.py` & `pynumstim-0.2.9/pynumstim/_problem.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/pynumstim/datasets/Lindemann_Tira_10.toml` & `pynumstim-0.2.9/pynumstim/datasets/Lindemann_Tira_10.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/pynumstim/image.py` & `pynumstim-0.2.9/pynumstim/image.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/pyproject.toml` & `pynumstim-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/trial_list.txt` & `pynumstim-0.2.9/trial_list.txt`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.8/PKG-INFO` & `pynumstim-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumstim
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python library to create symbolic number and arithmetic stimuli for psychological experiments
 Keywords: experiment control,open science,experimental psychology
 Author-email: Oliver Lindemann <lindemann@essb.eur.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

