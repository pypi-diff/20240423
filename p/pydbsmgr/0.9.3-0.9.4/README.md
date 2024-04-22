# Comparing `tmp/pydbsmgr-0.9.3.tar.gz` & `tmp/pydbsmgr-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbsmgr-0.9.3.tar", last modified: Wed Apr 10 03:13:26 2024, max compression
+gzip compressed data, was "pydbsmgr-0.9.4.tar", last modified: Mon Apr 22 21:47:15 2024, max compression
```

## Comparing `pydbsmgr-0.9.3.tar` & `pydbsmgr-0.9.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/pydbsmgr/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/fast_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/lightest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/pydbsmgr/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/utils/azure_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/utils/sql_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/pydbsmgr/utils/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/utils/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14049 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/pydbsmgr/utils/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/pydbsmgr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-10 03:13:26.000000 pydbsmgr-0.9.3/pydbsmgr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-10 03:13:26.000000 pydbsmgr-0.9.3/pydbsmgr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:13:26.000000 pydbsmgr-0.9.3/pydbsmgr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-10 03:13:26.000000 pydbsmgr-0.9.3/pydbsmgr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-10 03:13:26.000000 pydbsmgr-0.9.3/pydbsmgr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:13:26.917036 pydbsmgr-0.9.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-10 03:13:19.000000 pydbsmgr-0.9.3/test/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:47:15.449112 pydbsmgr-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-22 21:47:15.449112 pydbsmgr-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:47:15.445112 pydbsmgr-0.9.4/pydbsmgr/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/fast_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/lightest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14750 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:47:15.449112 pydbsmgr-0.9.4/pydbsmgr/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/utils/azure_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13970 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/utils/sql_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:47:15.449112 pydbsmgr-0.9.4/pydbsmgr/utils/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/utils/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/pydbsmgr/utils/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:47:15.449112 pydbsmgr-0.9.4/pydbsmgr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-22 21:47:15.000000 pydbsmgr-0.9.4/pydbsmgr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 21:47:15.000000 pydbsmgr-0.9.4/pydbsmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:47:15.000000 pydbsmgr-0.9.4/pydbsmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-22 21:47:15.000000 pydbsmgr-0.9.4/pydbsmgr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 21:47:15.000000 pydbsmgr-0.9.4/pydbsmgr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 21:47:15.449112 pydbsmgr-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:47:15.449112 pydbsmgr-0.9.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-22 21:47:10.000000 pydbsmgr-0.9.4/test/test_functions.py
```

### Comparing `pydbsmgr-0.9.3/LICENSE` & `pydbsmgr-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/PKG-INFO` & `pydbsmgr-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbsmgr
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python package for database control and DataFrame processing
 Home-page: https://github.com/jzsmoreno/pydbsmgr
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Maintainer: David Pedroza
 Maintainer-email: david.pedroza.segoviano@gmail.com
 License: MIT
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2.0.0
 Requires-Dist: pandas
-Requires-Dist: clean-text
 Requires-Dist: missingno
 Requires-Dist: pyodbc
 Requires-Dist: ipython
 Requires-Dist: SQLAlchemy
 Requires-Dist: pyyaml
 Requires-Dist: azure-storage-blob==12.16.0
 Requires-Dist: python-dotenv==1.0.0
```

### Comparing `pydbsmgr-0.9.3/README.md` & `pydbsmgr-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/pydbsmgr/fast_upload.py` & `pydbsmgr-0.9.4/pydbsmgr/fast_upload.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/pydbsmgr/health.py` & `pydbsmgr-0.9.4/pydbsmgr/health.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/pydbsmgr/lightest.py` & `pydbsmgr-0.9.4/pydbsmgr/lightest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import concurrent.futures
 from functools import partial
 
 from pydbsmgr.main import *
 from pydbsmgr.utils.tools import coerce_datetime, most_repeated_item
 
 
 def process_dates(x: str, format_type: str, auxiliary_type: str) -> str:
@@ -38,23 +37,27 @@
     x = x.replace("/", "")
     x = x.replace("-", "")
 
     if len(x) == 8:
         try:
             x = str(pd.to_datetime(x, format=format_type, errors="raise"))[:10]
         except:
-            if auxiliary_type != None:
+            if auxiliary_type is not None:
                 x = str(pd.to_datetime(x, format=auxiliary_type, errors="ignore"))[:10]
+            else:
+                raise ValueError("Date value does not match the expected format.")
     else:
         if str(x).find(":") != -1:
             try:
                 x = str(pd.to_datetime(x[:8], format=format_type, errors="raise"))[:10]
             except:
-                if auxiliary_type != None:
+                if auxiliary_type is not None:
                     x = str(pd.to_datetime(x[:8], format=auxiliary_type, errors="ignore"))[:10]
+                else:
+                    raise ValueError("Date value does not match the expected format.")
     return x
 
 
 class LightCleaner:
     """Performs a light cleaning on the table"""
 
     # Increase memory efficiency
@@ -69,39 +72,26 @@
         sample_frac: float = 0.1,
         fast_execution: bool = True,
         two_date_formats: bool = True,
         **kwargs,
     ) -> DataFrame:
         """`DataFrame` cleaning main function
 
+        Parameters
+        ----------
+        - sample_frac (`float`): The fraction of rows to use for date type inference. Default is 0.1 i.e., 10%.
+        - fast_execution (`bool`): If `False` use `applymap` pandas for extra text cleanup. Default is `True`.
+
         Keyword Arguments:
         ----------
-        - fix_unicode: (`bool`): By default it is set to `True`.
-        - to_ascii: (`bool`): By default it is set to `True`.
-        - lower: (`bool`): By default it is set to `True`.
-        - normalize_whitespace: (`bool`): By default it is set to `True`.
-        - no_line_breaks: (`bool`): By default it is set to `False`.
-        - strip_lines: (`bool`): By default it is set to `True`.
-        - keep_two_line_breaks: (`bool`): By default it is set to `False`.
-        - no_urls: (`bool`): By default it is set to `False`.
-        - no_emails: (`bool`): By default it is set to `False`.
-        - no_phone_numbers: (`bool`): By default it is set to `False`.
-        - no_numbers: (`bool`): By default it is set to `False`.
-        - no_digits: (`bool`): By default it is set to `False`.
-        - no_currency_symbols: (`bool`): By default it is set to `False`.
-        - no_punct: (`bool`): By default it is set to `False`.
         - no_emoji: (`bool`): By default it is set to `False`.
-        - replace_with_url: (`str`): For example, the following `<URL>`.
-        - replace_with_email: (`str`): For example, the following `<EMAIL>`.
-        - replace_with_phone_number: (`str`): For example, the following `<PHONE>`.
-        - replace_with_number: (`str`): For example, the following `<NUMBER>`.
-        - replace_with_digit: (`str`): For example, the following `0`.
-        - replace_with_currency_symbol: (`str`): For example, the following `<CUR>`.
-        - replace_with_punct: (`str`): = For example, the following `""`.
-        - lang: (`str`): = By default it is set to `en`.
+        If `True`, removes all emojis from text data. Works only when `fast_execution` = `False`.
+        - title_mode: (`bool`): By default it is set to `True`.
+        If `False`, converts the text to lowercase. Works only when `fast_execution` = `False`.
+        By default, converts everything to `title`.
         """
         table = (self.df).copy()
         cols = table.columns
         table_sample = table.sample(frac=sample_frac)
         for column_index, datatype in enumerate(table.dtypes):
             if datatype == "object":
                 datetype_column = (
@@ -116,58 +106,76 @@
                                 lambda item: item is not None,
                                 table_sample[cols[column_index]].apply(get_date_format),
                             )
                         ),
                         two_date_formats,
                     )
                     if auxiliary_type != None:
-                        format_type = auxiliary_type
+                        try:
+                            format_type = auxiliary_type
+                            partial_dates = partial(
+                                process_dates,
+                                format_type=format_type,
+                                auxiliary_type=None,
+                            )
+                            vpartial_dates = np.vectorize(partial_dates)
+                            table[cols[column_index]] = vpartial_dates(table[cols[column_index]])
+                        except:
+                            format_type = main_type
+                            partial_dates = partial(
+                                process_dates,
+                                format_type=format_type,
+                                auxiliary_type=None,
+                            )
+                            vpartial_dates = np.vectorize(partial_dates)
+                            table[cols[column_index]] = vpartial_dates(table[cols[column_index]])
                     else:
                         format_type = main_type
-                    with concurrent.futures.ThreadPoolExecutor() as executor:
                         partial_dates = partial(
                             process_dates,
                             format_type=format_type,
                             auxiliary_type=None,
                         )
-                        table[cols[column_index]] = list(
-                            executor.map(partial_dates, table[cols[column_index]])
-                        )
-                        table[cols[column_index]] = list(
-                            executor.map(coerce_datetime, table[cols[column_index]])
-                        )
+                        vpartial_dates = np.vectorize(partial_dates)
+                        table[cols[column_index]] = vpartial_dates(table[cols[column_index]])
+                    vcoerce_datetime = np.vectorize(coerce_datetime)
+                    table[cols[column_index]] = vcoerce_datetime(table[cols[column_index]])
                     table[cols[column_index]] = pd.to_datetime(
                         table[cols[column_index]], format="%Y%m%d", errors="coerce"
                     ).dt.normalize()
                 else:
-                    if fast_execution == False:
-                        partial_clean = partial(clean, **kwargs)
-                        with concurrent.futures.ThreadPoolExecutor() as executor:
-                            table[cols[column_index]] = list(
-                                executor.map(partial_clean, table[cols[column_index]])
-                            )
-                            table[cols[column_index]] = list(
-                                executor.map(remove_char, table[cols[column_index]])
-                            )
-                            try:
-                                table[cols[column_index]] = list(
-                                    executor.map(
-                                        lambda text: text.title() if text is not None else text,
-                                        table[cols[column_index]],
-                                    )
-                                )
-                            except AttributeError as e:
-                                warning_type = "UserWarning"
-                                msg = (
-                                    "It was not possible to perform the cleaning, the column {%s} is duplicated. "
-                                    % cols[column_index]
-                                )
-                                msg += "Error: {%s}" % e
-                                print(f"{warning_type}: {msg}")
-                                sys.exit("Perform correction manually")
+                    try:
+                        table[cols[column_index]] = (
+                            table[cols[column_index]]
+                            .replace(np.nan, "")
+                            .astype(str)
+                            .str.normalize("NFKD")
+                            .str.encode("ascii", errors="ignore")
+                            .str.decode("ascii")
+                            .str.title()
+                        )
+                    except AttributeError as e:
+                        warning_type = "UserWarning"
+                        msg = (
+                            "It was not possible to perform the cleaning, the column {%s} is duplicated. "
+                            % cols[column_index]
+                        )
+                        msg += "Error: {%s}" % e
+                        print(f"{warning_type}: {msg}")
+                        sys.exit("Perform correction manually")
+                    if not fast_execution:
+                        no_emoji = kwargs["no_emoji"] if "no_emoji" in kwargs else False
+                        title_mode = kwargs["title_mode"] if "title_mode" in kwargs else True
+                        partial_clean = partial(
+                            clean,
+                            no_emoji=no_emoji,
+                            title_mode=title_mode,
+                        )
+                        vpartial_clean = np.vectorize(partial_clean)
+                        table[cols[column_index]] = vpartial_clean(table[cols[column_index]])
 
         table = self._remove_duplicate_columns(table)
         self.df = table.copy()
         return self.df
 
     def _correct_float(self, value, datatype):
         """float correction function"""
```

### Comparing `pydbsmgr-0.9.3/pydbsmgr/logs.py` & `pydbsmgr-0.9.4/pydbsmgr/logs.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/pydbsmgr/main.py` & `pydbsmgr-0.9.4/pydbsmgr/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import re
 import sys
 import warnings
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
-from cleantext import clean
 from IPython.display import clear_output
 from pandas.core.frame import DataFrame
 from pandas.core.indexes.base import Index
 from pandas.core.series import Series
 
 warnings.filterwarnings("ignore")
 
@@ -28,14 +27,16 @@
         r"[0-1]+[0-9](-|/)[0-3]+[0-9](-|/)\d{4}",
         r"([1-9]|[12][0-9]|3[01])(-|/)([1-9]|1[0-2])(-|/)\d{4}",
         r"([1-9]|1[0-2])(-|/)([1-9]|[12][0-9]|3[01])(-|/)\d{4}",
     ]
     formats = ["%Y%m%d", "%Y%d%m", "%d%m%Y", "%m%d%Y", "dayfirst", "monthfirst"]
     for format, regex in enumerate(regex_formats):
         if re.search(regex, str(input_string)):
+            if formats[format] == formats[2] and int((input_string[3:5]).replace("0", "")) > 12:
+                return formats[3]
             return formats[format]
 
     return ""
 
 
 def check_if_contains_dates(input_string: str) -> bool:
     """Check if a string contains date."""
@@ -59,15 +60,20 @@
 
     Returns:
         `str`: clean character string
     """
     return re.sub(r"\d", "", input_string)
 
 
-def clean_names(dirty_string: str, pattern: str = r"[a-zA-Zñáéíóú_]+\b") -> str:
+def clean(
+    dirty_string: str,
+    pattern: str = r"[a-zA-Zñáéíóú_@.0-9]+\b",
+    no_emoji: bool = False,
+    title_mode: bool = False,
+) -> str:
     """
     Receive a string and clean it of special characters
 
     Parameters
     ----------
     dirty_string : `str`
         string of characters
@@ -75,22 +81,35 @@
         regular expression string
 
     Returns
     -------
     result : `str`
         clean character string
     """
-    result = re.findall(pattern, str(dirty_string).replace("_", ""))
-    if len(result) > 0:
-        result = "_".join(result)
+    if no_emoji:
+        emoji_pattern = re.compile(
+            "["
+            "\U0001F600-\U0001F64F"
+            "\U0001F300-\U0001F5FF"
+            "\U0001F680-\U0001F6FF"
+            "\U0001F1E0-\U0001F1FF"
+            "]+",
+            flags=re.UNICODE,
+        )
+        dirty_string = emoji_pattern.sub(r"", dirty_string)
+    dirty_string = dirty_string.lower()
+    words = dirty_string.split()
+    processed_words = ["".join(re.findall(pattern, word)) for word in words]
+    result = " ".join(processed_words)
+    # Remove any extra spaces that were introduced by
+    result = result.strip()
+    if title_mode:
+        return result.title()
     else:
-        pattern = r"[a-zA-Z]+"
-        result = re.findall(pattern, str(dirty_string).replace("_", ""))
-        result = "_".join(result)
-    return result
+        return result
 
 
 def clean_transform_helper(
     col: str, mode: bool = True, remove_numeric: bool = True, remove_spaces: bool = True
 ) -> str:
     """
     Transforms a column name by cleaning the column name and if needed makes it capital.
```

### Comparing `pydbsmgr-0.9.3/pydbsmgr/utils/azure_sdk.py` & `pydbsmgr-0.9.4/pydbsmgr/utils/azure_sdk.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/pydbsmgr/utils/config.py` & `pydbsmgr-0.9.4/pydbsmgr/utils/config.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/pydbsmgr/utils/sql_functions.py` & `pydbsmgr-0.9.4/pydbsmgr/utils/sql_functions.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/pydbsmgr/utils/tools/tools.py` & `pydbsmgr-0.9.4/pydbsmgr/utils/tools/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,16 +93,16 @@
     def get_frame(self, **kwargs) -> DataFrame:
         self.df = self._process_columns(**kwargs)
         return self.df
 
     def _process_columns(self, surrounding: bool = True) -> DataFrame:
         df = (self.df).copy()
         df.columns = df.columns.str.lower()
-        df.columns = df.columns.str.replace(".", "")
-        df.columns = df.columns.str.replace(",", "")
+        df.columns = df.columns.str.replace(".", "", regex=False)
+        df.columns = df.columns.str.replace(",", "", regex=False)
         df.columns = df.columns.str.replace(r"[^a-zA-Z0-9ñáéíóú_]", "_", regex=True)
 
         df.columns = df.columns.str.replace("_+", "_", regex=True)
         df.columns = df.columns.str.strip()
         df.columns = df.columns.str.strip("_")
         if surrounding:
             df.columns = [f"[{col}]" for col in df.columns]
```

### Comparing `pydbsmgr-0.9.3/pydbsmgr.egg-info/PKG-INFO` & `pydbsmgr-0.9.4/pydbsmgr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbsmgr
-Version: 0.9.3
+Version: 0.9.4
 Summary: Python package for database control and DataFrame processing
 Home-page: https://github.com/jzsmoreno/pydbsmgr
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Maintainer: David Pedroza
 Maintainer-email: david.pedroza.segoviano@gmail.com
 License: MIT
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy<2.0.0
 Requires-Dist: pandas
-Requires-Dist: clean-text
 Requires-Dist: missingno
 Requires-Dist: pyodbc
 Requires-Dist: ipython
 Requires-Dist: SQLAlchemy
 Requires-Dist: pyyaml
 Requires-Dist: azure-storage-blob==12.16.0
 Requires-Dist: python-dotenv==1.0.0
```

### Comparing `pydbsmgr-0.9.3/pydbsmgr.egg-info/SOURCES.txt` & `pydbsmgr-0.9.4/pydbsmgr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/setup.py` & `pydbsmgr-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `pydbsmgr-0.9.3/test/conftest.py` & `pydbsmgr-0.9.4/test/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 @pytest.fixture()
 def _get_extraction_date() -> Callable:
     return get_extraction_date
 
 
 @pytest.fixture()
-def _clean_names() -> Callable:
-    return clean_names
+def _clean() -> Callable:
+    return clean
 
 
 @pytest.fixture()
 def _clean_transform() -> Callable:
     return clean_transform
```

### Comparing `pydbsmgr-0.9.3/test/test_functions.py` & `pydbsmgr-0.9.4/test/test_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import re
 import sys
 from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 import pytest
-from cleantext import clean
 from pandas.core.frame import DataFrame
 from pandas.core.indexes.base import Index
 from pandas.core.series import Series
 
 
-def test_clean_names(_clean_names):
-    assert _clean_names("#tes$ting") == "tes_ting"
+def test_clean(_clean):
+    assert _clean("#Tes$ting method*") == "testing method"
 
 
 def test_clean_transform(_clean_transform):
     assert _clean_transform(["TesTing", "PyTest"]) == ["Testing", "Pytest"]
     assert _clean_transform(["1 TesTing", "(PyTest)"]) == ["Testing", "Pytest"]
 
 
@@ -45,17 +44,14 @@
 
 def test_columns_dtypes(columns_dtypes_with_data):
     df = columns_dtypes_with_data.correct(sample_frac=0.33)
     data_types = df.dtypes
     assert data_types[1] == "datetime64[ns]"
 
 
-@pytest.mark.xfail(
-    reason="Due to the use of 'concurrent.futures' you have this error. Try to run it again."
-)
 def test_lightest(lightest_with_data):
     fecha, first_date, anther_date, third_date = lightest_with_data
     comparison = ["1974-09-10", "1973-01-06", "1975-01-18", "2020-08-25"]
     assert fecha == comparison
     assert first_date == comparison
     assert anther_date == comparison
     assert third_date == comparison
```

