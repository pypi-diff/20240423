# Comparing `tmp/UtilityLib-2.8.20231123.tar.gz` & `tmp/UtilityLib-2.9.20240323.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UtilityLib-2.8.20231123.tar", last modified: Thu Nov 23 07:51:42 2023, max compression
+gzip compressed data, was "UtilityLib-2.9.20240323.tar", last modified: Sat Mar 23 11:24:42 2024, max compression
```

## Comparing `UtilityLib-2.8.20231123.tar` & `UtilityLib-2.9.20240323.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2023-11-23 07:51:42.379366 UtilityLib-2.8.20231123/
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       14 2023-08-29 10:01:21.000000 UtilityLib-2.8.20231123/MANIFEST.in
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     3044 2023-11-23 07:51:42.379366 UtilityLib-2.8.20231123/PKG-INFO
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     2842 2023-08-29 10:08:56.000000 UtilityLib-2.8.20231123/README.md
-drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2023-11-23 07:51:42.379366 UtilityLib-2.8.20231123/UtilityLib/
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     5791 2023-11-23 07:45:58.000000 UtilityLib-2.8.20231123/UtilityLib/BaseUtility.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     6038 2023-11-23 07:47:33.000000 UtilityLib-2.8.20231123/UtilityLib/CommandUtility.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)    14885 2023-11-23 07:43:00.000000 UtilityLib-2.8.20231123/UtilityLib/DataUtility.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     7740 2023-11-23 07:43:00.000000 UtilityLib-2.8.20231123/UtilityLib/DatabaseUtility.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)    31076 2023-11-23 07:43:00.000000 UtilityLib-2.8.20231123/UtilityLib/FileSystemUtility.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     4463 2023-11-23 07:43:00.000000 UtilityLib-2.8.20231123/UtilityLib/LoggingUtility.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     6670 2023-11-23 07:49:21.000000 UtilityLib-2.8.20231123/UtilityLib/ProjectManager.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     2158 2023-11-23 07:49:45.000000 UtilityLib-2.8.20231123/UtilityLib/TimeUtility.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      250 2023-11-23 07:43:00.000000 UtilityLib-2.8.20231123/UtilityLib/UtilityManager.py
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      677 2023-11-23 07:44:46.000000 UtilityLib-2.8.20231123/UtilityLib/__init__.py
-drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2023-11-23 07:51:42.379366 UtilityLib-2.8.20231123/UtilityLib.egg-info/
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     3044 2023-11-23 07:51:42.000000 UtilityLib-2.8.20231123/UtilityLib.egg-info/PKG-INFO
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      495 2023-11-23 07:51:42.000000 UtilityLib-2.8.20231123/UtilityLib.egg-info/SOURCES.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)        1 2023-11-23 07:51:42.000000 UtilityLib-2.8.20231123/UtilityLib.egg-info/dependency_links.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       28 2023-11-23 07:51:42.000000 UtilityLib-2.8.20231123/UtilityLib.egg-info/requires.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       11 2023-11-23 07:51:42.000000 UtilityLib-2.8.20231123/UtilityLib.egg-info/top_level.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       31 2023-08-30 15:48:59.000000 UtilityLib-2.8.20231123/requirements.txt
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       38 2023-11-23 07:51:42.379366 UtilityLib-2.8.20231123/setup.cfg
--rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      683 2023-08-30 15:23:50.000000 UtilityLib-2.8.20231123/setup.py
+drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-03-23 11:24:42.277245 UtilityLib-2.9.20240323/
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       14 2023-08-29 10:01:21.000000 UtilityLib-2.9.20240323/MANIFEST.in
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     3252 2024-03-23 11:24:42.277245 UtilityLib-2.9.20240323/PKG-INFO
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     2749 2024-03-23 08:24:21.000000 UtilityLib-2.9.20240323/README.md
+drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-03-23 11:24:42.273245 UtilityLib-2.9.20240323/UtilityLib/
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     5704 2024-03-23 11:19:39.000000 UtilityLib-2.9.20240323/UtilityLib/BaseUtility.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     6038 2024-03-15 07:46:55.000000 UtilityLib-2.9.20240323/UtilityLib/CommandUtility.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)    15922 2024-03-20 12:56:16.000000 UtilityLib-2.9.20240323/UtilityLib/DataUtility.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     7740 2024-03-15 07:46:55.000000 UtilityLib-2.9.20240323/UtilityLib/DatabaseUtility.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)    30965 2024-03-20 12:50:13.000000 UtilityLib-2.9.20240323/UtilityLib/FileSystemUtility.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     4463 2024-03-15 07:46:55.000000 UtilityLib-2.9.20240323/UtilityLib/LoggingUtility.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     6670 2024-03-15 07:46:55.000000 UtilityLib-2.9.20240323/UtilityLib/ProjectManager.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     2158 2024-03-15 07:46:55.000000 UtilityLib-2.9.20240323/UtilityLib/TimeUtility.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      896 2024-03-21 10:14:40.000000 UtilityLib-2.9.20240323/UtilityLib/UtilityManager.py
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      554 2024-03-23 08:14:06.000000 UtilityLib-2.9.20240323/UtilityLib/__init__.py
+drwxr-xr-x   0 vishalkumarsahu  (1000) root         (0)        0 2024-03-23 11:24:42.277245 UtilityLib-2.9.20240323/UtilityLib.egg-info/
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)     3252 2024-03-23 11:24:42.000000 UtilityLib-2.9.20240323/UtilityLib.egg-info/PKG-INFO
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      484 2024-03-23 11:24:42.000000 UtilityLib-2.9.20240323/UtilityLib.egg-info/SOURCES.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)        1 2024-03-23 11:24:42.000000 UtilityLib-2.9.20240323/UtilityLib.egg-info/dependency_links.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       43 2024-03-23 11:24:42.000000 UtilityLib-2.9.20240323/UtilityLib.egg-info/requires.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       11 2024-03-23 11:24:42.000000 UtilityLib-2.9.20240323/UtilityLib.egg-info/top_level.txt
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)      665 2024-03-23 11:23:16.000000 UtilityLib-2.9.20240323/pyproject.toml
+-rw-r--r--   0 vishalkumarsahu  (1000) root         (0)       38 2024-03-23 11:24:42.277245 UtilityLib-2.9.20240323/setup.cfg
```

### Comparing `UtilityLib-2.8.20231123/PKG-INFO` & `UtilityLib-2.9.20240323/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: UtilityLib
-Version: 2.8.20231123
-Summary: UtilityLib: Think, Explore, and Master
-Home-page: https://github.com/TheBiomics/UtilityLib
-Author: Vishal Kumar Sahu
-Author-email: mail@vishalkumarsahu.in
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 2.9.20240323
+Summary: Python Helper for Repetitive Tasks with File and Data Management
+Author-email: Vishal Kumar Sahu <mail@vishalkumarsahu.in>
+Project-URL: Homepage, https://github.com/TheBiomics/UtilityLib
+Project-URL: Issues, https://github.com/TheBiomics/UtilityLib/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: xmltodict
+Requires-Dist: sqlalchemy
+Requires-Dist: psutil
+Requires-Dist: pandas
+Requires-Dist: seaborn
 
 # About UtilityLib
 * Provided ready to use functions to process, read, write, list files and directories and more...
 
 # Installation
 
 * Install using source from github using python's pip module
@@ -58,24 +64,23 @@
 
 ```python
 _wos_files = EU.search(f"{path_scrapped_queries}/WOS-Downloads", "*.csv")
 EU.add_tgz_files(f"{path_scrapped_queries}/WOS-Downloads.tgz", _wos_files)
 EU.delete_path(f"{path_scrapped_queries}/WOS-Downloads")
 ```
 
-# ToDo
-- `require_from` GitHub
-- Saving file hashes to check if file has changed ever since last accessed
-
-# Requirements
-* xmltodict
-* sqlalchemy
+---
 
 # Version Updates
 
+## 2.8
+
+* Method aliases
+* Setup whl build system
+
 ## 2.6
 ### 20221103
 * Added `ProjectManager`
   - Dot notion to access or deep nested objected
   - Can hold data by pickling and unpickling (Could there be any data loss due to protocol version change?)
   - class to keep track of configuration
   - persistent storage
@@ -106,9 +111,7 @@
 * Minor changes (check commit)
 
 ## 2.5.20220818
 * Package reusability enhancement
 
 ## 2.4.20220129
 * Initial version
-
-
```

### Comparing `UtilityLib-2.8.20231123/README.md` & `UtilityLib-2.9.20240323/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,24 +47,23 @@
 
 ```python
 _wos_files = EU.search(f"{path_scrapped_queries}/WOS-Downloads", "*.csv")
 EU.add_tgz_files(f"{path_scrapped_queries}/WOS-Downloads.tgz", _wos_files)
 EU.delete_path(f"{path_scrapped_queries}/WOS-Downloads")
 ```
 
-# ToDo
-- `require_from` GitHub
-- Saving file hashes to check if file has changed ever since last accessed
-
-# Requirements
-* xmltodict
-* sqlalchemy
+---
 
 # Version Updates
 
+## 2.8
+
+* Method aliases
+* Setup whl build system
+
 ## 2.6
 ### 20221103
 * Added `ProjectManager`
   - Dot notion to access or deep nested objected
   - Can hold data by pickling and unpickling (Could there be any data loss due to protocol version change?)
   - class to keep track of configuration
   - persistent storage
```

### Comparing `UtilityLib-2.8.20231123/UtilityLib/BaseUtility.py` & `UtilityLib-2.9.20240323/UtilityLib/BaseUtility.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,30 @@
       "_imported_modules": [],
     }
     self.__defaults.update(kwargs)
     self.set_system_type(**self.__defaults)
     self.update_attributes(self, self.__defaults)
 
   def is_running(self, *args, **kwargs):
-    _file = args[0] if len(args) > 0 else kwargs.get("file", "process-v2.txt")
+    _file = args[0] if len(args) > 0 else kwargs.get("file", "UtilityLib-Processes-v2.txt")
     _dir = args[1] if len(args) > 1 else kwargs.get("dir", 'Documents/PyProcessConfig')
 
-    _path_user_settings = OS.path.join(OS.path.expanduser('~'), _dir)
+    self.OS = OS
+
+    _path_user_settings = self.OS.path.join(self.OS.path.expanduser('~'), _dir)
     _path_file_pid = f"{_path_user_settings}/{_file}"
 
-    if not OS.path.exists(_path_user_settings):
-      OS.makedirs(_path_user_settings)
+    if not self.OS.path.exists(_path_user_settings):
+      self.OS.makedirs(_path_user_settings)
 
     _current_pid = getpid()
 
     from psutil import pid_exists, Process
 
-    if OS.path.exists(_path_file_pid):
+    if self.OS.path.exists(_path_file_pid):
       with open(_path_file_pid) as f:
         pid = f.read()
         pid = int(pid) if pid.isnumeric() else None
       if pid is not None and pid_exists(pid) and Process(pid).cmdline() == Process(_current_pid).cmdline():
         return True
 
     with open(_path_file_pid, 'w') as f:
@@ -50,49 +52,43 @@
   def update_attributes(self, object=None, kw=dict(), defaults=dict()):
     """
       Sets attribute (dict) values and defaults
     """
     if object is None:
       object = self
 
+    if hasattr(self, 'path_base') and not self.path_base:
+      self.path_base = self.OS.getcwd()
+
     if isinstance(kw.get('path_bases'), (list, tuple)):
       self.set_directories(**kw)
 
     [setattr(object, _k, defaults[_k]) for _k in defaults.keys() if not hasattr(object, _k)]
     [setattr(object, _k, kw[_k]) for _k in kw.keys()]
 
   def set_directories(self, *args, **kwargs):
-    _path_bases = args[0] if len(args) > 0 else kwargs.get("path_bases", self.OS.getcwd())
+    _path_bases = args[0] if len(args) > 0 else kwargs.get("path_bases", self.path_base)
     # Consider first path is for Linux and second path is for Windows
     if isinstance(_path_bases, (str)):
       self.path_base = _path_bases
     elif isinstance(_path_bases, (list, tuple)):
       _path_bases = _path_bases * 2
       self.path_base = _path_bases[1] if self.is_windows else _path_bases[0]
     elif isinstance(_path_bases, (dict)):
       # ToDo: first linux, then windows
       self.path_base = self.set_directories(path_bases=_path_bases.values())
 
   def __call__(self, *args, **kwargs):
     self.update_attributes(self, kwargs)
     return self
 
-  def __str__(self):
-    return "@ToDo: implement str magic."
-
-  def preprocess_output(self, *args, **kwargs):
-    """
-      @ToDo: Test and QA
-    """
-    _value = args[0] if len(args) > 0 else kwargs.get("value")
-    _callback = args[1] if len(args) > 1 else kwargs.get("callback")
-    if _callback and _value:
-      return _callback(_value)
+  def __repr__(self):
+    return f"{self.name}: Use help() function to see the list of all methods."
 
-    return _value
+  __str__ = __repr__
 
   def set_system_type(self, *args, **kwargs):
     self.is_windows = False
     self.is_linux = False
     self.OS = OS
     if self.OS.name == "nt":
       self.is_windows = True
```

### Comparing `UtilityLib-2.8.20231123/UtilityLib/CommandUtility.py` & `UtilityLib-2.9.20240323/UtilityLib/CommandUtility.py`

 * *Files identical despite different names*

### Comparing `UtilityLib-2.8.20231123/UtilityLib/DataUtility.py` & `UtilityLib-2.9.20240323/UtilityLib/DataUtility.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 
 class DataUtility(TimeUtility):
   def __init__(self, *args, **kwargs):
     self.__defaults = {}
     self.__defaults.update(kwargs)
     super(DataUtility, self).__init__(**self.__defaults)
 
-  def digit_only(self, *args, **kwargs):
-    """See self.parse_digits"""
-    return self.parse_digits(*args, **kwargs)
-
-  def parse_digits(self, *args, **kwargs):
+  # DataFrame Functions
+  ## Pandas
+  def df_reset_columns(self, *args, **kwargs):
     """
-      @return digit parts of a given _data
+      @return reset column multiindex additionally set group index as a column
 
       @params
-      0|data: String type
+      0|df: DataFrame
+      1|key: DataFrame.groupby().key
 
       # Considering data is str
       # Float, int list etc are not tested or handled
     """
-    _data = args[0] if len(args) > 0 else kwargs.get("data")
-    return "".join([_s for _s in _data if _s.isdigit()])
+
+    _df = args[0] if len(args) > 0 else kwargs.get("df")
+    _key = args[1] if len(args) > 1 else kwargs.get("key")
+
+    _joined_cols = ["__".join(_idx) for _idx in _df.columns if isinstance(_idx, tuple)]
+    _df.columns = _joined_cols if len(_joined_cols) == len(_df.columns) else _df.columns
+    if _key and (not _key in _df.columns) and (not 'index' in _df.columns):
+        _df = _df.reset_index()
+    return _df
 
   def pd_categorical(self, df, col_name, sort=True):
       """
       Arguments:
         0|df: pandas DataFrame
         1|col_name: Column Name
         2|sort: boolean
@@ -139,14 +145,42 @@
     return self.read_csv(*args, **kwargs)
 
   def read_csv(self, *args, **kwargs):
     _file = args[0] if len(args) > 0 else kwargs.get("file")
     if self.require("pandas", "PD"):
       return self.PD.read_csv(_file, **kwargs)
 
+  # Helpers
+
+  def preprocess_output(self, *args, **kwargs):
+    """
+      @ToDo: Test and QA
+    """
+    _value = args[0] if len(args) > 0 else kwargs.get("value")
+    _callback = args[1] if len(args) > 1 else kwargs.get("callback")
+    if _callback and _value:
+      return _callback(_value)
+
+    return _value
+
+  def parse_digits(self, *args, **kwargs):
+    """Digit parts of a given data
+
+      @params
+      0|data: String type
+
+      # Considering data is str
+      # Float, int list etc are not tested or handled
+    """
+    _data = args[0] if len(args) > 0 else kwargs.get("data")
+    return "".join([_s for _s in str(_data) if _s.isdigit()])
+
+  digits = parse_digits
+  digit_only = parse_digits
+
   def re_compile(self, *args, **kwargs):
     _pattern = args[0] if len(args) > 0 else kwargs.get("pattern")
     _ignore_case = args[1] if len(args) > 1 else kwargs.get("ignore_case", True)
     _escape = args[1] if len(args) > 1 else kwargs.get("escape", False)
 
     if self.require("re", "REGEX"):
       _pattern = self.REGEX.escape(_pattern) if _escape else _pattern
@@ -244,29 +278,31 @@
 
     """
     _obj = args[0] if len(args) > 0 else kwargs.get("obj")
     _size = args[1] if len(args) > 1 else kwargs.get("size", 10)
     for _n in range(0, len(_obj), _size):
       yield _obj[_n:_n+_size]
 
+  slices = chunks
+  sliced = chunks
+
   @staticmethod
   def is_iterable(*args, **kwargs):
     """
       Checks for iterables except str
 
       @usage
       .flatten(list|tuple, 2)
     """
     _obj = args[0] if len(args) > 0 else kwargs.get("obj")
     return hasattr(_obj, '__iter__') and not isinstance(_obj, str)
 
   @staticmethod
   def flatten(_nested, _level=99, _depth=0):
-    """
-      Flattens nested iterables except str
+    """Flattens nested iterables except str
 
       @usage
       .flatten(list|tuple, 2)
     """
     _collector = []
     _depth += 1
     if all([DataUtility.is_iterable(_nested), not _level <= _depth]):
@@ -274,17 +310,15 @@
         _val = DataUtility.flatten(_item, _level, _depth)
         _collector.extend(_val) if DataUtility.is_iterable(_val) else _collector.append(_val)
     else:
       _collector = _nested
     return _collector
 
   def product(self, *args, **kwargs):
-    """
-      @generator
-      Provides combinations of the given items
+    """@generator Provides combinations of the given items
       NOTE: Single string will be converted to one item list
       "AUGC" will behave like ["A", "U", ...]
       ["AUGC"] will be treated as it is
 
       @params
       0|items (list): Object(s) to unpack using *
       1|repeat (1|int)
@@ -363,16 +397,15 @@
 
     """
     _results = self.common_substrings(*args, **kwargs)
     _result = max(_results, key=len) if len(_results) > 0 else ""
     return _result
 
   def get_deep_key(self, *args, **kwargs):
-    """
-      Get method to access nested key
+    """Get method to access nested key
 
       @params
       0|obj: dictionary
       1|keys: string, pipe separated string, list, tuple, set
       2|default -> optional:
 
       @example
```

### Comparing `UtilityLib-2.8.20231123/UtilityLib/DatabaseUtility.py` & `UtilityLib-2.9.20240323/UtilityLib/DatabaseUtility.py`

 * *Files identical despite different names*

### Comparing `UtilityLib-2.8.20231123/UtilityLib/FileSystemUtility.py` & `UtilityLib-2.9.20240323/UtilityLib/FileSystemUtility.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 
 class FileSystemUtility(LoggingUtility):
   def __init__(self, *args, **kwargs):
     self.__defaults = {}
     self.__defaults.update(kwargs)
     super(FileSystemUtility, self).__init__(**self.__defaults)
 
+  def backup(self, *args, **kwargs):
+    _file = args[0] if len(args) > 0 else kwargs.get("file")
+    _ext = self.ext(_file)
+    _copy_name = self.change_ext(self.time_stamp() + f".{_ext}")
+    return self.copy(_file, _copy_name)
+
   def rename(self, *args, **kwargs):
     _old_name = args[0] if len(args) > 0 else kwargs.get("from")
     _new_name = args[1] if len(args) > 1 else kwargs.get("to")
     return OS.rename(_old_name, _new_name)
 
   def compress_gz(self, *args, **kwargs):
     """Compress a file to gz
@@ -225,20 +231,14 @@
     self.update_attributes(self, kwargs)
     _text = args[0] if len(args) > 0 else kwargs.get("text")
 
     from bs4 import BeautifulSoup
     _html = BeautifulSoup(_text, "html.parser")
     return _html
 
-  def unpickle(self, *args, **kwargs):
-    """
-      @alias read_pickle
-    """
-    return self.read_pickle(*args, **kwargs)
-
   def read_pickle(self, *args, **kwargs):
     """
       @function
       reads pickle file
 
       @params
       0|source (str|path): File path
@@ -262,23 +262,30 @@
         with open(_source, 'rb+') as _fp:
           _default = self.PICKLE.load(_fp)
     else:
       self.log_error("Required module or pickle path is not found!")
 
     return _default
 
+  unpickle = read_pickle
+  get_pickle = read_pickle
+
   def read_html(self, *args, **kwargs):
     self.update_attributes(self, kwargs)
     _source = args[0] if len(args) > 0 else kwargs.get("source")
     _read = self.read_text(_source)
     _file_content = None
     if isinstance(_read, (list, tuple, set)):
       _file_content = "".join(_read)
     return self.parse_html(_file_content, **kwargs)
 
+  # added v2.8
+  html = read_html
+  from_html = read_html
+
   def read_xml(self, *args, **kwargs):
     self.update_attributes(self, kwargs)
     _source = args[0] if len(args) > 0 else kwargs.get("source")
     _content = ""
 
     from lxml import etree as XMLTree
     if self.check_path(_source):
@@ -325,14 +332,18 @@
       _content = _return_type(_content)
 
     if _callback is not None:
       _content = _callback(_content)
 
     return _content
 
+  # added v2.8
+  text = read_text
+  from_text = read_text
+
   def read_json(self, *args, **kwargs):
     self.update_attributes(self, kwargs)
     _file_path = args[0] if len(args) > 0 else kwargs.get("file_path")
     _res_dict = {}
 
     if self.check_path(_file_path):
       _content = self.read_text(_file_path, str)
@@ -340,14 +351,18 @@
       try:
         _res_dict = JSON.loads(_content)
       except:
         _res_dict = self.AbsSynTree.literal_eval(_content)
 
     return _res_dict
 
+  # added v2.8
+  from_json = read_json
+  from_JSON = read_json
+
   def write(self, *args, **kwargs):
     """
       @params
         0|destination:
         1|content
         2|append (boolean)
         3|encoding
@@ -392,26 +407,14 @@
       if isinstance(_content, (bytes, bytearray, str)):
         _fh.write(_content)
       elif isinstance(_content, (list, tuple, set)):
         _fh.write("\n".join(_content))
 
     return self.check_path(_destination)
 
-  def save_pickle(self, *args, **kwargs):
-    """
-      @alias write_pickle
-    """
-    return self.write_pickle(*args, **kwargs)
-
-  def pickle(self, *args, **kwargs):
-    """
-      @alias write_pickle
-    """
-    return self.write_pickle(*args, **kwargs)
-
   def write_pickle(self, *args, **kwargs):
     """
       @function
       Writes python object as pickle file
 
       @params
       0|destination (str|path)
@@ -432,14 +435,17 @@
 
       with self.GZip.open(_destination,'wb') as _fh:
         self.PICKLE.dump(_content, _fh)
     else:
       self.log_error("Either pickle/gzip module was not loaded or some other error occurred.")
     return self.exists(_destination)
 
+  save_pickle = write_pickle
+  pickle = write_pickle
+
   def write_json(self, *args, **kwargs):
     """
       @function
       Writes dict content as JSON
 
       @returns
       True|False if file path exists
@@ -462,24 +468,16 @@
     """
     self.update_attributes(self, kwargs)
     _destination = args[0] if len(args) > 0 else kwargs.get("destination")
     _content = args[1] if len(args) > 1 else kwargs.get("content")
     self.write(_destination, _content, **kwargs)
     return self.check_path(_destination)
 
-  def conv_xml_to_dict(self, *args, **kwargs):
-    """
-      @alias xml_to_dict
-    """
-    return self.xml_to_dict(*args, **kwargs)
-
   def xml_to_dict(self, *args, **kwargs):
-    """
-      @function
-      Converts XML to dict
+    """Converts XML to dict
 
       @returns
       dict of the converted xml
     """
     self.update_attributes(self, kwargs)
     _data = args[0] if len(args) > 0 else kwargs.get("data")
     _res = {}
@@ -491,14 +489,16 @@
       if not isinstance(_data, (str)):
         _data = XMLTree.tostring(_data, encoding='utf8', method='xml')
       _res = JSON.loads(JSON.dumps(self.XMLTODICT.parse(_data)))
     except:
       self.log_info(f"Failed to convert XML to DICT. Some error occurred.")
     return _res
 
+  conv_xml_to_dict = xml_to_dict
+
   def dict_to_csv(self, *args, **kwargs):
     _destination = args[0] if len(args) > 0 else kwargs.get("destination")
     _data = args[1] if len(args) > 1 else kwargs.get("data")
 
     if isinstance(_data, list) and isinstance(_data[0], dict):
       _keys = _data[0].keys()
       self.require("csv", "CSV")
@@ -659,49 +659,59 @@
         return _response.text
     except:
       self.log_warning(f"Normal procedure failed. Trying alternate method 'urlretrieve'.")
       self.download_content(_url, _destination)
 
     return self.check_path(_destination)
 
-  def find_dirs(self, *args, **kwargs):
-    """@alias search_dirs"""
-    return self.search_dirs(*args, **kwargs)
-
   def search_dirs(self, *args, **kwargs):
+    """Search directories using pattern
+
+    """
     self.update_attributes(self, kwargs)
     _source = args[0] if len(args) > 0 else kwargs.get("dir", getattr(self, "dir"))
     _pattern = args[1] if len(args) > 1 else kwargs.get("pattern", "/*/")
-    return self.search(_source, _pattern)
+    return self._search_path_pattern(_source, _pattern)
 
-  def find_files(self, *args, **kwargs):
-    """@alias search_files"""
-    return self.search_files(*args, **kwargs)
+  find_dirs = search_dirs
 
   def search_files(self, *args, **kwargs):
+    """Search files using pattern
+
+    """
     _source = args[0] if len(args) > 0 else kwargs.get("dir", getattr(self, "dir"))
     _pattern = args[1] if len(args) > 1 else kwargs.get("pattern", ["*"])
 
-    return self.search(_source, _pattern)
+    return self._search_path_pattern(_source, _pattern)
+
+  # added v2.8
+  find_files = search_files
+  search = search_files
 
   def get_file_types(self, *args, **kwargs):
+    """Search files using extension
+
+    """
     _source = args[0] if len(args) > 0 else kwargs.get("source", getattr(self, "source", OS.getcwd()))
     _ext = args[1] if len(args) > 1 else kwargs.get("ext", getattr(self, "ext", ()))
     _matches = []
 
     if not all((_source, len(_ext) > 0)):
       return _matches
 
     for _root, _dir_names, _file_names in OS.walk(_source):
       for filename in _file_names:
         if filename.endswith(_ext):
           _matches.append(OS.path.join(_root, filename))
     return _matches
 
-  def search(self, *args, **kwargs):
+  def _search_path_pattern(self, *args, **kwargs):
+    """Internal Function to Search Paths based on pattern
+
+    """
     self.update_attributes(self, kwargs)
     _results = []
     _source = args[0] if len(args) > 0 else kwargs.get("source", getattr(self, "source"))
     _pattern = args[1] if len(args) > 1 else kwargs.get("pattern", "*")
 
     if not _source or not _pattern:
       return _results
@@ -734,23 +744,16 @@
         _res = OS.makedirs(_d)
         _dir_created[_d] = _res
       else:
         self.log_warning(f"Either {_d} already exists or some other error occurred while creating the file.")
 
     return _dir_created
 
-  def exists(self, *args, **kwargs):
-    """
-      @alias check_path
-    """
-    return self.check_path(*args, **kwargs)
-
   def get_existing(self, *args, **kwargs):
-    """
-      Returns first existing path from the given list
+    """Returns first existing path from the given list
 
       @extends check_path
     """
     _path = args[0] if len(args) > 0 else kwargs.get("path")
     if isinstance(_path, (str)):
       _path = [_path]
 
@@ -778,20 +781,22 @@
         _r = _p if self.check_path(_p) else False
         _result.append(_r)
     else:
       _result = OS.path.exists(_path) if _path else _result
 
     return _result
 
+  exists = check_path
+
   def validate_subdir(self, *args, **kwargs):
     _base = args[0] if len(args) > 0 else kwargs.get("base")
     _sub = args[0] if len(args) > 0 else kwargs.get("sub")
-    r = self.re_compile(r"[/\\]")
+    _rgx = self.re_compile(r"[/\\]")
     # Check if sub_dir contains any slash so that it is not directory name, append it's parent path
-    if r.search(str(_sub)) == None:
+    if _rgx.search(str(_sub)) == None:
       return self.validate_dir(f"{_base}{OS.sep}{_sub}")
     else:
       return self.validate_dir(_sub)
 
   def validate_dir(self, *args, **kwargs):
     self.update_attributes(self, kwargs)
     _dir = args[0] if len(args) > 0 else kwargs.get("dir")
@@ -832,20 +837,14 @@
       _fpath = OS.path.dirname(_fpath)
 
     if _validate and not OS.path.isdir(_fpath):
       return None
 
     return _fpath
 
-  def file_name(self, *args, **kwargs):
-    """
-      @alias filename
-    """
-    return self.filename(*args, **kwargs)
-
   def filename(self, *args, **kwargs):
     """
       @function
       Returns file_name from path <path>/<file_name>.<extn>.<ext2>.<ext1>
 
       @params
       0|file_path
@@ -873,35 +872,34 @@
     _file_path = _file_path.rsplit(".", _num_ext)
 
     if len(_file_path):
       return _file_path[0]
 
     return None
 
-  def file_ext(self, *args, **kwargs):
-    """
-      @alias ext
-    """
-    return self.ext(*args, **kwargs)
+  file_name = filename
 
-  def ext(self, *args, **kwargs):
-    """
-      @function
-      Returns file fxtension
+  def file_ext(self, *args, **kwargs):
+    """Returns file fxtension
 
       @params
       0|file_path
       1|num_ext=1: Number of extension with a dot
     """
     _file_path = args[0] if len(args) > 0 else kwargs.get("file_path")
     _num_ext = args[1] if len(args) > 1 else kwargs.get("num_ext", 1)
     _delimiter = args[2] if len(args) > 2 else kwargs.get("delimiter", ".")
 
     _file_path = OS.path.basename(_file_path)
     _file_path = _file_path.rsplit(_delimiter, _num_ext) # str.removesuffix
     _file_path = f"{_delimiter}".join(_file_path[-_num_ext:])
     return _file_path
 
+  get_extension = file_ext
+  get_ext = file_ext
+  file_extension = file_ext
+  ext = file_ext
+
   def split_file(self, *args, **kwargs):
     # TODO
     _file_path = args[0] if len(args) > 0 else kwargs.get("file_path")
     _sdf_id_delimiter = args[2] if len(args) > 2 else kwargs.get("id_delimiter")
```

### Comparing `UtilityLib-2.8.20231123/UtilityLib/LoggingUtility.py` & `UtilityLib-2.9.20240323/UtilityLib/LoggingUtility.py`

 * *Files identical despite different names*

### Comparing `UtilityLib-2.8.20231123/UtilityLib/ProjectManager.py` & `UtilityLib-2.9.20240323/UtilityLib/ProjectManager.py`

 * *Files identical despite different names*

### Comparing `UtilityLib-2.8.20231123/UtilityLib/TimeUtility.py` & `UtilityLib-2.9.20240323/UtilityLib/TimeUtility.py`

 * *Files identical despite different names*

### Comparing `UtilityLib-2.8.20231123/UtilityLib.egg-info/PKG-INFO` & `UtilityLib-2.9.20240323/UtilityLib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: UtilityLib
-Version: 2.8.20231123
-Summary: UtilityLib: Think, Explore, and Master
-Home-page: https://github.com/TheBiomics/UtilityLib
-Author: Vishal Kumar Sahu
-Author-email: mail@vishalkumarsahu.in
-License: UNKNOWN
-Platform: UNKNOWN
+Version: 2.9.20240323
+Summary: Python Helper for Repetitive Tasks with File and Data Management
+Author-email: Vishal Kumar Sahu <mail@vishalkumarsahu.in>
+Project-URL: Homepage, https://github.com/TheBiomics/UtilityLib
+Project-URL: Issues, https://github.com/TheBiomics/UtilityLib/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: xmltodict
+Requires-Dist: sqlalchemy
+Requires-Dist: psutil
+Requires-Dist: pandas
+Requires-Dist: seaborn
 
 # About UtilityLib
 * Provided ready to use functions to process, read, write, list files and directories and more...
 
 # Installation
 
 * Install using source from github using python's pip module
@@ -58,24 +64,23 @@
 
 ```python
 _wos_files = EU.search(f"{path_scrapped_queries}/WOS-Downloads", "*.csv")
 EU.add_tgz_files(f"{path_scrapped_queries}/WOS-Downloads.tgz", _wos_files)
 EU.delete_path(f"{path_scrapped_queries}/WOS-Downloads")
 ```
 
-# ToDo
-- `require_from` GitHub
-- Saving file hashes to check if file has changed ever since last accessed
-
-# Requirements
-* xmltodict
-* sqlalchemy
+---
 
 # Version Updates
 
+## 2.8
+
+* Method aliases
+* Setup whl build system
+
 ## 2.6
 ### 20221103
 * Added `ProjectManager`
   - Dot notion to access or deep nested objected
   - Can hold data by pickling and unpickling (Could there be any data loss due to protocol version change?)
   - class to keep track of configuration
   - persistent storage
@@ -106,9 +111,7 @@
 * Minor changes (check commit)
 
 ## 2.5.20220818
 * Package reusability enhancement
 
 ## 2.4.20220129
 * Initial version
-
-
```

