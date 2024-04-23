# Comparing `tmp/dicomselect-0.9.0.tar.gz` & `tmp/dicomselect-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomselect-0.9.0.tar", last modified: Fri Nov 17 16:16:33 2023, max compression
+gzip compressed data, was "dicomselect-0.9.1.tar", last modified: Wed Dec 13 08:54:55 2023, max compression
```

## Comparing `dicomselect-0.9.0.tar` & `dicomselect-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-11-17 16:16:33.826476 dicomselect-0.9.0/
--rw-rw-rw-   0        0        0     1082 2023-04-18 16:33:48.000000 dicomselect-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     5686 2023-11-17 16:16:33.825977 dicomselect-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4967 2023-11-17 16:13:14.000000 dicomselect-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-11-17 16:16:33.815977 dicomselect-0.9.0/dicomselect/
--rw-rw-rw-   0        0        0      245 2023-11-17 16:13:14.000000 dicomselect-0.9.0/dicomselect/__init__.py
--rw-rw-rw-   0        0        0       23 2023-11-17 16:15:15.000000 dicomselect-0.9.0/dicomselect/__version__.py
--rw-rw-rw-   0        0        0     1358 2023-05-04 13:16:46.000000 dicomselect-0.9.0/dicomselect/constants.py
--rw-rw-rw-   0        0        0    10315 2023-11-17 16:15:28.000000 dicomselect-0.9.0/dicomselect/convert.py
--rw-rw-rw-   0        0        0    17357 2023-11-17 16:13:14.000000 dicomselect-0.9.0/dicomselect/database.py
--rw-rw-rw-   0        0        0     2468 2023-11-17 16:13:14.000000 dicomselect-0.9.0/dicomselect/dicom.py
--rw-rw-rw-   0        0        0     2569 2023-11-17 16:13:14.000000 dicomselect-0.9.0/dicomselect/info.py
--rw-rw-rw-   0        0        0     1839 2023-11-17 16:13:14.000000 dicomselect-0.9.0/dicomselect/logging.py
--rw-rw-rw-   0        0        0     6609 2023-11-17 16:13:14.000000 dicomselect-0.9.0/dicomselect/query.py
--rw-rw-rw-   0        0        0     2759 2023-05-08 11:24:09.000000 dicomselect-0.9.0/dicomselect/queryfactory.py
--rw-rw-rw-   0        0        0    17081 2023-11-17 16:13:14.000000 dicomselect-0.9.0/dicomselect/reader.py
--rw-rw-rw-   0        0        0   203115 2023-05-04 13:16:46.000000 dicomselect-0.9.0/dicomselect/tags_generated.py
-drwxrwxrwx   0        0        0        0 2023-11-17 16:16:33.821476 dicomselect-0.9.0/dicomselect.egg-info/
--rw-rw-rw-   0        0        0     5686 2023-11-17 16:16:33.000000 dicomselect-0.9.0/dicomselect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-11-17 16:16:33.000000 dicomselect-0.9.0/dicomselect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-17 16:16:33.000000 dicomselect-0.9.0/dicomselect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      181 2023-11-17 16:16:33.000000 dicomselect-0.9.0/dicomselect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-11-17 16:16:33.000000 dicomselect-0.9.0/dicomselect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-17 16:16:33.826476 dicomselect-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-11-17 16:15:15.000000 dicomselect-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-17 16:16:33.824478 dicomselect-0.9.0/tests/
--rw-rw-rw-   0        0        0     5256 2023-11-17 16:13:16.000000 dicomselect-0.9.0/tests/test_convert.py
--rw-rw-rw-   0        0        0     2578 2023-11-17 16:13:16.000000 dicomselect-0.9.0/tests/test_create.py
--rw-rw-rw-   0        0        0     1603 2023-11-17 16:13:16.000000 dicomselect-0.9.0/tests/test_example.py
--rw-rw-rw-   0        0        0     3663 2023-11-17 16:13:16.000000 dicomselect-0.9.0/tests/test_select.py
--rw-rw-rw-   0        0        0      168 2023-11-17 16:13:16.000000 dicomselect-0.9.0/tests/test_version.py
+drwxrwxrwx   0        0        0        0 2023-12-13 08:54:55.042673 dicomselect-0.9.1/
+-rw-rw-rw-   0        0        0     1082 2023-04-18 16:33:48.000000 dicomselect-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     5614 2023-12-13 08:54:55.041173 dicomselect-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4895 2023-12-13 08:38:29.000000 dicomselect-0.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-12-13 08:54:55.032172 dicomselect-0.9.1/dicomselect/
+-rw-rw-rw-   0        0        0      245 2023-11-17 16:13:14.000000 dicomselect-0.9.1/dicomselect/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-12-13 08:54:20.000000 dicomselect-0.9.1/dicomselect/__version__.py
+-rw-rw-rw-   0        0        0     1358 2023-05-04 13:16:46.000000 dicomselect-0.9.1/dicomselect/constants.py
+-rw-rw-rw-   0        0        0    10610 2023-12-13 08:38:08.000000 dicomselect-0.9.1/dicomselect/convert.py
+-rw-rw-rw-   0        0        0    17358 2023-12-13 08:38:29.000000 dicomselect-0.9.1/dicomselect/database.py
+-rw-rw-rw-   0        0        0     2468 2023-11-17 16:13:14.000000 dicomselect-0.9.1/dicomselect/dicom.py
+-rw-rw-rw-   0        0        0     3028 2023-12-13 08:38:29.000000 dicomselect-0.9.1/dicomselect/info.py
+-rw-rw-rw-   0        0        0     1839 2023-12-13 08:54:08.000000 dicomselect-0.9.1/dicomselect/logging.py
+-rw-rw-rw-   0        0        0     6609 2023-11-17 16:13:14.000000 dicomselect-0.9.1/dicomselect/query.py
+-rw-rw-rw-   0        0        0     2759 2023-05-08 11:24:09.000000 dicomselect-0.9.1/dicomselect/queryfactory.py
+-rw-rw-rw-   0        0        0    17081 2023-11-17 16:13:14.000000 dicomselect-0.9.1/dicomselect/reader.py
+-rw-rw-rw-   0        0        0   203115 2023-05-04 13:16:46.000000 dicomselect-0.9.1/dicomselect/tags_generated.py
+drwxrwxrwx   0        0        0        0 2023-12-13 08:54:55.040173 dicomselect-0.9.1/dicomselect.egg-info/
+-rw-rw-rw-   0        0        0     5614 2023-12-13 08:54:55.000000 dicomselect-0.9.1/dicomselect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-12-13 08:54:55.000000 dicomselect-0.9.1/dicomselect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-13 08:54:55.000000 dicomselect-0.9.1/dicomselect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      181 2023-12-13 08:54:55.000000 dicomselect-0.9.1/dicomselect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-12-13 08:54:55.000000 dicomselect-0.9.1/dicomselect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-13 08:54:55.042673 dicomselect-0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-11-28 11:51:34.000000 dicomselect-0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-13 08:54:55.039173 dicomselect-0.9.1/tests/
+-rw-rw-rw-   0        0        0     5256 2023-11-17 16:13:16.000000 dicomselect-0.9.1/tests/test_convert.py
+-rw-rw-rw-   0        0        0     2578 2023-11-17 16:13:16.000000 dicomselect-0.9.1/tests/test_create.py
+-rw-rw-rw-   0        0        0     1603 2023-11-17 16:13:16.000000 dicomselect-0.9.1/tests/test_example.py
+-rw-rw-rw-   0        0        0     3663 2023-11-17 16:13:16.000000 dicomselect-0.9.1/tests/test_select.py
+-rw-rw-rw-   0        0        0      168 2023-11-17 16:13:16.000000 dicomselect-0.9.1/tests/test_version.py
```

### Comparing `dicomselect-0.9.0/LICENSE` & `dicomselect-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/PKG-INFO` & `dicomselect-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicomselect
-Version: 0.9.0
+Version: 0.9.1
 Home-page: https://github.com/DIAGNijmegen/dicomselect
 Author-email: Stan.Noordman@radboudumc.nl
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dicomselect
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom~=2.3.1
@@ -71,15 +71,15 @@
 
 plan.execute()
 ```
 
 Check out the results in `tests/output/example`
 
 
-===========================================================================
+---
 
 # Create a new database
 ```python
 from pathlib import Path
 from dicomselect.database import Database
 
 db_path = Path("/path/to/dicomselect_archive.db")
```

### Comparing `dicomselect-0.9.0/README.md` & `dicomselect-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 plan.execute()
 ```
 
 Check out the results in `tests/output/example`
 
 
-===========================================================================
+---
 
 # Create a new database
 ```python
 from pathlib import Path
 from dicomselect.database import Database
 
 db_path = Path("/path/to/dicomselect_archive.db")
```

### Comparing `dicomselect-0.9.0/dicomselect/constants.py` & `dicomselect-0.9.1/dicomselect/constants.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/dicomselect/convert.py` & `dicomselect-0.9.1/dicomselect/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 import SimpleITK as sitk
 from tqdm import tqdm
 from treelib import Tree
 
+from dicomselect.logging import LOG_FILENAME, Logger
 from dicomselect.reader import DICOMImageReader
-from dicomselect.logging import Logger, LOG_FILENAME
 
 CustomPostprocessFunction = Callable[[DICOMImageReader], Union[sitk.Image, Dict[str, sitk.Image]]]
 
 
 class Convert:
     def __init__(self, uid: str, source: str, target: str, columns: List[str], values: List[str]):
         if len(columns) != len(values):
@@ -41,15 +41,16 @@
             return text.replace(placeholder, f'empty_{col}')
         return text.replace(placeholder, value)
 
     def __str__(self):
         return f'{self.source} -> {self.target}'
 
     def convert(self, extension: str, source_dir: Path, target_dir: Path,
-                postprocess_func: Optional[CustomPostprocessFunction] = None) -> str:
+                postprocess_func: Optional[CustomPostprocessFunction] = None,
+                exist_ok: bool = False) -> str:
         reader = DICOMImageReader(source_dir / self.source)
 
         if postprocess_func:
             try:
                 return_value = postprocess_func(reader)
                 msg = f'PostProcessFunction did not return an Image or a Dict[str, Image] ({str(self)})'
 
@@ -68,15 +69,15 @@
                 raise e
         else:
             convert_dict: Dict[str, sitk.Image] = {'': reader.image}
 
         for suffix, image in convert_dict.items():
             name = str(self.target) + suffix + extension
             target = target_dir / name
-            target.parent.mkdir(parents=True, exist_ok=True)
+            target.parent.mkdir(parents=True, exist_ok=exist_ok)
             target_tmp = target.parent / ('tmp_' + target.name)
             sitk.WriteImage(image, target_tmp.as_posix(), useCompression=True)
             os.replace(target_tmp, target)
 
 
 class Plan(Logger):
     def __init__(self, default_source_dir: Path, converts: List[Convert]):
@@ -118,15 +119,16 @@
     @target_dir.setter
     def target_dir(self, value: os.PathLike):
         assert value is not None, ValueError('target_dir is not set.')
         value = Path(value).absolute()
         assert not value.exists() or value.is_dir(), NotADirectoryError(f'{value} is not a directory.')
         if value.exists():
             files = [file.name for file in value.iterdir()]
-            assert len(files) == 0 or files == [LOG_FILENAME], ValueError(f'{value} is not empty.')
+            if len(files) > 0 and files != [LOG_FILENAME]:
+                print(f'Warning: {value} is not empty. Set exist_ok=True to overwrite existing files.')
         self._invalidate('target_dir', value)
         self._target_dir = value
 
     @property
     def extension(self) -> str:
         """
         The extension defines the converted filetype. See https://simpleitk.readthedocs.io/en/master/IO.html#images
@@ -195,44 +197,50 @@
 
         tree = self._tree()
         text = 'dicomselect conversion plan\n'
         for param in ['source_dir', 'target_dir', 'extension']:
             text += '\n' + f'{param:<20}{getattr(self, param)}'
         return text + '\n\n' + tree.show(stdout=False)
 
-    def execute(self, max_workers: int = 4, postprocess_func: Optional[CustomPostprocessFunction] = None, exists_ok=False):
+    def execute(self, max_workers: int = 4, postprocess_func: Optional[CustomPostprocessFunction] = None, exist_ok=False):
         """
         Execute the conversion plan.
 
         Parameters
         ----------
         max_workers
             Max number of workers for parallel execution of this conversion.
         postprocess_func:
             Postprocess function, providing a DICOMImageReader. If it returns False, the conversion is skipped. If it
             returns a SimpleITK.Image, the conversion is executed using the returned image. If it returns a dict of
             [str, SimpleITK.Image], it converts each entry, where key is attached to the end of the name template.
             Note that multiple converted files from one image will not be cached and will be marked for deletion in future
             plans due to the anonymous nature of this function.
-        exists_ok:
+        exist_ok:
             If exist_ok is true, FileExistsError exceptions will be ignored.
         """
         self._validate()
         self.init_logger(self.target_dir / LOG_FILENAME)
 
         converts_len = len(self._converts)
 
         try:
-            convert_args = (self.extension, self.source_dir, self.target_dir, postprocess_func)
+            convert_kwargs = {
+                "extension": self.extension,
+                "source_dir": self.source_dir,
+                "target_dir": self.target_dir,
+                "postprocess_func": postprocess_func,
+                "exist_ok": exist_ok,
+            }
 
             if not self.target_dir.exists():
-                self.target_dir.mkdir(parents=True, exist_ok=exists_ok)
+                self.target_dir.mkdir(parents=True, exist_ok=exist_ok)
 
             def _execute(convert: Convert) -> Optional[str]:
-                return convert.convert(*convert_args)
+                return convert.convert(**convert_kwargs)
 
             print(f"Converting {converts_len} DICOM series from {self.source_dir} to {self.target_dir}")
             with tqdm(total=converts_len, desc=f"Converting to {self.extension}") as pbar, ThreadPoolExecutor(max_workers=max_workers) as pool:
                 chunk_size = 5000
                 for i in range(0, converts_len, chunk_size):
                     futures = {pool.submit(_execute, convert): convert for convert in self._converts[i:i+chunk_size]}
                     for future in as_completed(futures):
```

### Comparing `dicomselect-0.9.0/dicomselect/database.py` & `dicomselect-0.9.1/dicomselect/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             raise IsADirectoryError('Provide a file path with as extension, .db')
         self._conn: sqlite3.Connection = None
         self._query_factory: QueryFactory = None
         self._db_dir: Path = None
         self._is_warned_outdated_db = False
 
         self._prefer_mode = PreferMode.PreferZipFile
-        self._verify_dcm_filenames = True
+        self._verify_dcm_filenames = False
 
         self._headers: List[str] = None
         self._custom_header_func: CustomHeaderFunction = None
         self._custom_headers: Dict[str, type] = None
         self._additional_dicom_tags: List[str] = None
 
     @property
```

### Comparing `dicomselect-0.9.0/dicomselect/dicom.py` & `dicomselect-0.9.1/dicomselect/dicom.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/dicomselect/info.py` & `dicomselect-0.9.1/dicomselect/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import TYPE_CHECKING, Dict, List
 
+import pandas as pd
+
 if TYPE_CHECKING:
     from dicomselect.query import Query
 
 
 class Info:
     def __init__(self, parent: 'Query', rows: List[tuple], cols: Dict[str, Dict[str, int]]):
         self._query_parent = parent
@@ -40,14 +42,28 @@
             items = sorted(self._cols[key].items(), key=lambda a: a[1], reverse=True)
             for value, count in items:
                 count: str = f'({count})'.ljust(len(str(len(self._rows))) + 2)
                 contents.append(f'\t{count} {value}')
 
         return '\n'.join(contents)
 
+    def to_df(self, sort_by_homogeneous: bool = True) -> pd.DataFrame:
+        # untested
+        df = pd.DataFrame(columns=self._cols)
+        sort_by_similarity = sorted(
+            sorted(self._cols.keys()),
+            key=lambda k: len(self._cols[k]),
+            reverse=not sort_by_homogeneous
+        )
+
+        for c, row in enumerate(self._rows):
+            df.loc[c] = row[1:]
+            
+        return df
+
     def include(self, *columns) -> 'Info':
         included_cols = {key: value for key, value in self._cols.items() if key in columns}
         return Info(self._query_parent, self._rows, included_cols)
 
     def exclude(self, *columns, recommended: bool = True, exclude_all_distinct: bool = False, exclude_none_distinct: bool = False) -> 'Info':
         r = [k for k in self._cols.keys() if 'uid' in k] + \
             ['path', 'dicomselect_uid', 'image_position_patient', 'patient_position']
```

### Comparing `dicomselect-0.9.0/dicomselect/logging.py` & `dicomselect-0.9.1/dicomselect/logging.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/dicomselect/query.py` & `dicomselect-0.9.1/dicomselect/query.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/dicomselect/queryfactory.py` & `dicomselect-0.9.1/dicomselect/queryfactory.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/dicomselect/reader.py` & `dicomselect-0.9.1/dicomselect/reader.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/dicomselect/tags_generated.py` & `dicomselect-0.9.1/dicomselect/tags_generated.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/dicomselect.egg-info/PKG-INFO` & `dicomselect-0.9.1/dicomselect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicomselect
-Version: 0.9.0
+Version: 0.9.1
 Home-page: https://github.com/DIAGNijmegen/dicomselect
 Author-email: Stan.Noordman@radboudumc.nl
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/dicomselect
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydicom~=2.3.1
@@ -71,15 +71,15 @@
 
 plan.execute()
 ```
 
 Check out the results in `tests/output/example`
 
 
-===========================================================================
+---
 
 # Create a new database
 ```python
 from pathlib import Path
 from dicomselect.database import Database
 
 db_path = Path("/path/to/dicomselect_archive.db")
```

### Comparing `dicomselect-0.9.0/dicomselect.egg-info/SOURCES.txt` & `dicomselect-0.9.1/dicomselect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/setup.py` & `dicomselect-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-version = '0.9.0'
+version = '0.9.1'
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
         name='dicomselect',
```

### Comparing `dicomselect-0.9.0/tests/test_convert.py` & `dicomselect-0.9.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/tests/test_create.py` & `dicomselect-0.9.1/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/tests/test_example.py` & `dicomselect-0.9.1/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `dicomselect-0.9.0/tests/test_select.py` & `dicomselect-0.9.1/tests/test_select.py`

 * *Files identical despite different names*

