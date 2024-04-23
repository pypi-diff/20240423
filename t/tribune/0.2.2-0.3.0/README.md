# Comparing `tmp/tribune-0.2.2.tar.gz` & `tmp/tribune-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tribune-0.2.2.tar", last modified: Wed Feb  7 18:50:32 2018, max compression
+gzip compressed data, was "tribune-0.3.0.tar", last modified: Tue Apr 23 14:26:59 2024, max compression
```

## Comparing `tribune-0.2.2.tar` & `tribune-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-02-07 18:50:32.000000 tribune-0.2.2/
--rwxrwxrwx   0 root         (0) root         (0)      755 2018-02-07 18:46:28.000000 tribune-0.2.2/changelog.rst
--rwxrwxrwx   0 root         (0) root         (0)      205 2018-02-07 17:59:33.000000 tribune-0.2.2/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     2145 2018-02-07 18:50:32.000000 tribune-0.2.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      387 2016-02-07 02:17:32.000000 tribune-0.2.2/readme.rst
--rwxrwxrwx   0 root         (0) root         (0)      109 2018-02-07 18:50:32.000000 tribune-0.2.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1665 2018-02-07 18:49:44.000000 tribune-0.2.2/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-02-07 18:50:32.000000 tribune-0.2.2/tribune/
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-02-07 18:50:32.000000 tribune-0.2.2/tribune/sheet_import/
--rwxrwxrwx   0 root         (0) root         (0)     6418 2016-06-10 13:31:27.000000 tribune-0.2.2/tribune/sheet_import/parsers.py
--rwxrwxrwx   0 root         (0) root         (0)    10065 2018-02-07 17:59:33.000000 tribune-0.2.2/tribune/sheet_import/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-02-07 18:50:32.000000 tribune-0.2.2/tribune/tests/
--rwxrwxrwx   0 root         (0) root         (0)      670 2016-02-23 02:30:23.000000 tribune-0.2.2/tribune/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)      794 2016-02-23 02:30:23.000000 tribune-0.2.2/tribune/tests/entities.py
--rwxrwxrwx   0 root         (0) root         (0)     4566 2016-02-23 02:47:00.000000 tribune-0.2.2/tribune/tests/reports.py
--rwxrwxrwx   0 root         (0) root         (0)    13189 2018-02-07 17:59:42.000000 tribune-0.2.2/tribune/tests/test_objects.py
--rwxrwxrwx   0 root         (0) root         (0)     6219 2018-02-07 17:59:33.000000 tribune-0.2.2/tribune/tests/test_sheet_import.py
--rwxrwxrwx   0 root         (0) root         (0)     8823 2016-06-10 13:31:27.000000 tribune-0.2.2/tribune/tests/test_sheet_import_parsers.py
--rwxrwxrwx   0 root         (0) root         (0)     2837 2018-02-07 17:59:42.000000 tribune-0.2.2/tribune/tests/test_utils.py
--rwxrwxrwx   0 root         (0) root         (0)     4354 2016-02-23 02:47:00.000000 tribune-0.2.2/tribune/tests/utils.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2016-02-07 03:23:12.000000 tribune-0.2.2/tribune/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3210 2018-02-07 17:59:42.000000 tribune-0.2.2/tribune/utils.py
--rwxrwxrwx   0 root         (0) root         (0)       19 2018-02-07 18:48:25.000000 tribune-0.2.2/tribune/version.py
--rwxrwxrwx   0 root         (0) root         (0)    20860 2018-02-07 17:59:42.000000 tribune-0.2.2/tribune/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2018-02-07 18:50:32.000000 tribune-0.2.2/tribune.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)        1 2018-02-07 18:50:31.000000 tribune-0.2.2/tribune.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2016-02-23 02:54:01.000000 tribune-0.2.2/tribune.egg-info/not-zip-safe
--rwxrwxrwx   0 root         (0) root         (0)     2145 2018-02-07 18:50:31.000000 tribune-0.2.2/tribune.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      108 2018-02-07 18:50:31.000000 tribune-0.2.2/tribune.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)      622 2018-02-07 18:50:32.000000 tribune-0.2.2/tribune.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        8 2018-02-07 18:50:31.000000 tribune-0.2.2/tribune.egg-info/top_level.txt
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-23 14:26:59.378055 tribune-0.3.0/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      133 2024-04-12 12:49:30.000000 tribune-0.3.0/MANIFEST.in
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2617 2024-04-23 14:26:59.378055 tribune-0.3.0/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1661 2024-04-23 14:26:42.000000 tribune-0.3.0/changelog.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      387 2024-04-12 12:49:30.000000 tribune-0.3.0/readme.rst
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      109 2024-04-23 14:26:59.378055 tribune-0.3.0/setup.cfg
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     1544 2024-04-23 14:16:43.000000 tribune-0.3.0/setup.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-23 14:26:59.370056 tribune-0.3.0/tribune/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    20828 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/__init__.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-23 14:26:59.374055 tribune-0.3.0/tribune/sheet_import/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12911 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/sheet_import/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     6453 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/sheet_import/parsers.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-23 14:26:59.378055 tribune-0.3.0/tribune/tests/
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-12 12:49:30.000000 tribune-0.3.0/tribune/tests/__init__.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      676 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/tests/conftest.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      782 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/tests/entities.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4566 2024-04-12 12:49:30.000000 tribune-0.3.0/tribune/tests/reports.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    12446 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/tests/test_objects.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)    11851 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/tests/test_sheet_import.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     8860 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/tests/test_sheet_import_parsers.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     2900 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/tests/test_utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     4336 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/tests/utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)     3320 2024-04-23 14:16:43.000000 tribune-0.3.0/tribune/utils.py
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)       18 2024-04-23 14:20:17.000000 tribune-0.3.0/tribune/version.py
+drwxrwxr-x   0 mlewellyn  (1000) mlewellyn  (1000)        0 2024-04-23 14:26:59.374055 tribune-0.3.0/tribune.egg-info/
+-rw-r--r--   0 mlewellyn  (1000) mlewellyn  (1000)     2617 2024-04-23 14:26:58.000000 tribune-0.3.0/tribune.egg-info/PKG-INFO
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      622 2024-04-23 14:26:59.000000 tribune-0.3.0/tribune.egg-info/SOURCES.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2024-04-23 14:26:58.000000 tribune-0.3.0/tribune.egg-info/dependency_links.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        1 2024-04-22 17:43:47.000000 tribune-0.3.0/tribune.egg-info/not-zip-safe
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)      103 2024-04-23 14:26:59.000000 tribune-0.3.0/tribune.egg-info/requires.txt
+-rw-rw-r--   0 mlewellyn  (1000) mlewellyn  (1000)        8 2024-04-23 14:26:59.000000 tribune-0.3.0/tribune.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tribune-0.2.2/setup.py` & `tribune-0.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,19 @@
     from setuptools import setup
 
 # pip install -e .[develop]
 develop_requires = [
     'BlazeUtils',
     'SQLAlchemy',
     'XlsxWriter',
-    'mock',
+    'openpyxl',
     'pytest',
     'pytest-cov',
-    'six',
     'wrapt',
-    'xlrd',
+    'xlrd<2',
 ]
 
 cdir = osp.abspath(osp.dirname(__file__))
 README = open(osp.join(cdir, 'readme.rst')).read()
 CHANGELOG = open(osp.join(cdir, 'changelog.rst')).read()
 
 version_fpath = osp.join(cdir, 'tribune', 'version.py')
@@ -37,26 +36,23 @@
     author_email="matt.lewellyn@level12.io",
     url='https://github.com/level12/tribune',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
     ],
     license='BSD',
     packages=[
         'tribune',
         'tribune.sheet_import',
     ],
-    extras_require={'develop': develop_requires},
+    extras_require={'test': develop_requires},
     zip_safe=False,
     include_package_data=True,
     install_requires=[
         'BlazeUtils',
-        'six',
         'xlsxwriter',
     ],
 )
```

### Comparing `tribune-0.2.2/tribune/sheet_import/parsers.py` & `tribune-0.3.0/tribune/sheet_import/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-from six import text_type
-from six.moves import (
-    filter,
-    map,
-)
-
 from ..utils import (
     chain,
     raises,
 )
 from . import (
     SpreadsheetImportError,
     normalize_text,
@@ -22,15 +16,18 @@
 def filter_(func):
     """A strict (non-iterator), curried version of filter for convenience in parser chains."""
     return lambda values: list(filter(func, values))
 
 
 def parse_text(value):
     """Parses text as a unicode string and strips leading/trailing whitespace."""
-    return text_type(value).strip()
+    if value is None:
+        # we do not want to return 'None' as a string, and chained ops will expect str
+        return ''
+    return str(value).strip()
 
 
 def parse_yes_no(value):
     """Parses boolean values represented as 'yes' or 'no' (case insensitive)."""
     result = {
         normalize_text('yes'): True,
         normalize_text('no'):  False
@@ -50,15 +47,15 @@
         return as_int if as_int == as_float else raises(ValueError())
     except (ValueError, TypeError):
         raise SpreadsheetImportError([u'must be an integer'])
 
 
 def parse_int_as_text(value):
     """Parses integers but converts them to unicode strings in the result."""
-    return text_type(parse_int(value))
+    return str(parse_int(value))
 
 
 def parse_number(value):
     """Parses any floating point number."""
     try:
         return float(value)
     except (ValueError, TypeError):
@@ -72,15 +69,15 @@
         return parse_int_as_text(value)
     except SpreadsheetImportError:
         return parse_text(value)
 
 
 def default_to(default):
     """Returns a parser that gives the provided default if the value is empty."""
-    return lambda value: default if value is None or text_type(value).strip() == '' else value
+    return lambda value: default if value is None or str(value).strip() == '' else value
 
 
 def nullable(parser):
     """Returns a parser that wraps another parser and only applies it if the value is not empty.
     If the value is empty, this parser always converts it to `None`."""
     return lambda value: None if default_to(None)(value) is None else parser(value)
```

### Comparing `tribune-0.2.2/tribune/sheet_import/__init__.py` & `tribune-0.3.0/tribune/sheet_import/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,23 +19,34 @@
         ('Yuri Gagarin',   '34',  'Yes'),
         ('Alexei Leonov',  '81',  'Yes'),
         ('Amelia Earhart', '39',  'No'),
     ])
     records = MySheet().get_sheet_records(sheet)
 """
 import abc
+import warnings
 from collections import namedtuple
 from io import BytesIO
+from typing import BinaryIO, Union
+from zipfile import BadZipFile
 
-from blazeutils.spreadsheets import xlsx_to_reader
-from six import with_metaclass, text_type
-from six.moves import filter
-import xlrd
+from blazeutils.spreadsheets import xlsx_to_reader, xlsx_to_strio
 from xlsxwriter import Workbook
 
+try:
+    import openpyxl
+    from openpyxl.utils.exceptions import InvalidFileException
+except ImportError:
+    openpyxl = None
+
+try:
+    import xlrd
+except ImportError:
+    xlrd = None
+
 import tribune
 
 from ..utils import (
     column_letter,
     flatten,
     raises,
     split_every,
@@ -47,63 +58,128 @@
     def __init__(self, errors):
         self.errors = errors
 
     def __str__(self):
         return '<SpreadsheetImportError: {}>'.format(self.errors)
 
 
-def workbook_safe_open(file_handle):
+def xlrd_workbook_safe_open(file_handle):
+    warnings.warn(
+        "xlrd support is deprecated and will be removed in a future version",
+        DeprecationWarning
+    )
+
     try:
         return xlrd.open_workbook(file_contents=file_handle.read())
     except xlrd.biffh.XLRDError as e:
         msg = str(e)
         # we don't want to screen all xlrd load errors, but a few common ones need to be trapped
         #   for user-friendliness
         if 'unsupported format' in msg.lower() or 'not supported' in msg.lower() \
                 or 'not a known type of workbook' in str(e).lower():
-            raise SpreadsheetImportError([u'File format is not recognized. Please upload an Excel'
+            raise SpreadsheetImportError(['File format is not recognized. Please upload an Excel'
                                           ' file (.xlsx or .xls).'])
         elif 'file size is 0 bytes' in msg.lower():
-            raise SpreadsheetImportError([u'File is empty.'])
+            raise SpreadsheetImportError(['File is empty.'])
         else:
             raise SpreadsheetImportError([msg])
 
 
+def workbook_safe_open(filename_or_filelike: Union[str, BinaryIO]):
+    if not openpyxl:
+        return xlrd_workbook_safe_open(filename_or_filelike)
+
+    try:
+        return openpyxl.load_workbook(filename_or_filelike, data_only=True)
+    except (BadZipFile, InvalidFileException):
+        raise SpreadsheetImportError(['File format is not recognized. Please upload an Excel'
+                                      ' file (.xlsx).'])
+
+
 def normalize_text(x):
     """Normalizes a string by stripping whitespace and flattening case."""
-    return text_type(x).strip().lower()
+    return str(x).strip().lower()
 
 
 class Cell(object):
     """Represents a particular cell on a spreadsheet."""
+    is_zero_based = False
+
     def __init__(self, row, column):
         """
         :param row: is a 0-based row index.
         :param column: is a 0-based column index.
         """
         self.row = row
         self.column = column
 
     def __str__(self):
-        return column_letter(self.column) + str(self.row + 1)
+        # If we're using openpyxl, column indices are one-based
+        return (
+            column_letter(self.column, self.is_zero_based)
+            + str(self.row + (1 if self.is_zero_based else 0))
+        )
+
 
+class XlrdCell(Cell):
+    """Represents a single cell when reading sheets with xlrd, which uses
+    0-based indices."""
+    is_zero_based = True
 
-class SheetData(with_metaclass(abc.ABCMeta)):
+
+class SheetDataBase(metaclass=abc.ABCMeta):
     """An ABC that describes the minimum necessary API for importing a sheet."""
     @abc.abstractmethod
     def __len__(self):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def cell_value(self, cell):
         raise NotImplementedError()
 
 
-class XlrdSheetData(SheetData):
+class SheetData(SheetDataBase):
+    def __init__(self, sheet):
+        self.sheet = sheet
+
+    def __len__(self):
+        return self.sheet.max_row
+
+    def cell_value(self, cell: Cell):
+        try:
+            return self.sheet.cell(cell.row, cell.column).value
+        except IndexError:
+            return ''
+
+    @classmethod
+    def from_nested_iters(cls, data):
+        """Builds a SheetData from nested iterables.
+
+        param data: is nested iterables representing data for each cell.
+                    For example, `[('A1', 'B1'), ('A2', 'B2')]` represents two rows and two columns
+                    of data.
+        """
+        workbook = Workbook(BytesIO())
+        sheet = workbook.add_worksheet('test')
+
+        for row, row_data in enumerate(data):
+            for column, cell_data in enumerate(row_data):
+                sheet.write(row, column, cell_data)
+
+        workbook = openpyxl.load_workbook(xlsx_to_strio(workbook))
+        sheet = workbook[workbook.sheetnames[0]]
+        return SheetData(sheet)
+
+
+class XlrdSheetData(SheetDataBase):
     def __init__(self, sheet):
+        warnings.warn(
+            "xlrd support is deprecated and will be removed in a future version",
+            DeprecationWarning
+        )
         self.sheet = sheet
 
     def __len__(self):
         return self.sheet.nrows
 
     def cell_value(self, cell):
         try:
@@ -125,15 +201,15 @@
         for row, row_data in enumerate(data):
             for column, cell_data in enumerate(row_data):
                 sheet.write(row, column, cell_data)
 
         return XlrdSheetData(xlsx_to_reader(workbook).sheet_by_index(0))
 
 
-class NestedItersSheetData(SheetData):
+class NestedItersSheetData(SheetDataBase):
     """Wraps nested iterables to provide the SheetData API."""
 
     def __init__(self, data):
         """
         param data: is nested iterables representing data for each cell.
                     For example, `[('A1', 'B1'), ('A2', 'B2')]` represents two rows and two columns
                     of data.
@@ -164,15 +240,18 @@
 
 
 Field = namedtuple('Field', ['label', 'field', 'parser'])
 
 
 class SheetImporter(object):
     """A base class for defining how to parse a single spreadsheet."""
-    data_start_row = 1  # 0-based index where first row of data begins
+    data_start_row = 2  # openpyxl indices are 1-based
+    data_start_col = 1
+    is_zero_based = False
+    cell_cls = Cell
     fields = ()         # Ordered iterable of Field tuples
 
     def __init__(self, fields=None, data_start_row=None):
         """
         :param fields: is an ordered iterable of Field tuples. If not provided, the class-level
                        value will be used.
         :param data_start_row: is the 0-based index where the first row of data begins. If not
@@ -184,17 +263,18 @@
     def _get_header_errors(self, sheet):
         """Builds a list of errors regarding the sheet header. The list will be empty if there are
         no errors."""
         header = self.data_start_row - 1
         return [
             'Expected "{header}" in header cell {cell}.'.format(
                 header=field.label,
-                cell=Cell(header, col)
-            ) for col, field in enumerate(self.fields)
-            if normalize_text(sheet.cell_value(Cell(header, col))) != normalize_text(field.label)
+                cell=self.cell_cls(header, col)
+            ) for col, field in enumerate(self.fields, self.data_start_col)
+            if normalize_text(sheet.cell_value(self.cell_cls(header, col)))
+            != normalize_text(field.label)
         ]
 
     @staticmethod
     def _parse_cell(field, cell, value):
         """Parses a cell using the given field definition. The result is an ErrorOrValue tuple.
 
         :param field: is a Field tuple which defines the field.
@@ -209,24 +289,36 @@
                 for msg in e.errors
             ]
             return ErrorOrValue(contextualized_errors, None)
 
     def _parse_row(self, sheet, row):
         """Parses all the columns in a sheet at a given row index and returns aggregated errors or
         values (for every column) as an ErrorOrValue tuple."""
-        col_data = [self._parse_cell(field, Cell(row, col), sheet.cell_value(Cell(row, col)))
-                    for col, field in enumerate(self.fields)]
+        col_data = [
+            self._parse_cell(
+                field,
+                self.cell_cls(row, col),
+                sheet.cell_value(self.cell_cls(row, col)),
+            )
+            for col, field in enumerate(self.fields, self.data_start_col)
+        ]
         errors, values = aggregate_error_or_value(col_data)
         return ErrorOrValue(errors, None) if errors \
             else ErrorOrValue([], self.row_to_record(values))
 
     def _parse_sheet_data(self, sheet):
         """Parses only the data rows from a sheet and returns aggregated errors or valuse as an
         ErrorOrValue tuple."""
-        return [self._parse_row(sheet, row) for row in range(self.data_start_row, len(sheet))]
+        return [
+            self._parse_row(sheet, row)
+            for row in range(
+                self.data_start_row,
+                len(sheet) + (1 if not self.is_zero_based else 0),
+            )
+        ]
 
     def _parse_sheet(self, sheet):
         """Parses a sheet (including the headers) and returns aggregated errors or values as an
         ErrorOrValue tuple."""
         header_errors = self._get_header_errors(sheet)
         if header_errors:
             return [ErrorOrValue(header_errors, None)]
@@ -266,7 +358,15 @@
             for ___field in self.fields:  # This iteration variable gets left behind on the class!
                 tribune.LabeledColumn(___field.label)
 
             def fetch_records(self):
                 return []
 
         return NewReportSheet
+
+
+class XlrdSheetImporter(SheetImporter):
+    """A base class for defining how to parse a single spreadsheet."""
+    data_start_row = 1  # xlrd rows are 0-based
+    data_start_col = 0
+    cell_cls = XlrdCell
+    is_zero_based = True
```

### Comparing `tribune-0.2.2/tribune/tests/conftest.py` & `tribune-0.3.0/tribune/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     from sqlalchemy import engine_from_config
     from sqlalchemy.orm import sessionmaker, scoped_session
     engine = engine_from_config({'url': 'sqlite:///'}, prefix='')
     session = scoped_session(sessionmaker(bind=engine))
 
     from tribune.tests import entities
     entities.meta.bind = engine
-    entities.meta.create_all()
+    entities.meta.create_all(engine)
     entities.session = session
     for x in range(1, 50):
         p = entities.Person()
         p.firstname = 'fn%03d' % x
         p.lastname = 'ln%03d' % x
         p.sortorder = x
         p.numericcol = D('29.26') * x / D('.9')
```

### Comparing `tribune-0.2.2/tribune/tests/entities.py` & `tribune-0.3.0/tribune/tests/entities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from blazeutils.strings import randchars
 import sqlalchemy as sa
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 
 from .utils import DefaultMixin
 
 meta = sa.MetaData()
 session = None
 Base = declarative_base(metadata=meta)
```

### Comparing `tribune-0.2.2/tribune/tests/reports.py` & `tribune-0.3.0/tribune/tests/reports.py`

 * *Files identical despite different names*

### Comparing `tribune-0.2.2/tribune/tests/test_objects.py` & `tribune-0.3.0/tribune/tests/test_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import operator
 from io import BytesIO
+from unittest import mock
 
 from blazeutils.datastructures import BlankObject
 from blazeutils.spreadsheets import xlsx_to_reader
-import mock
 import pytest
 from xlsxwriter import Workbook
 import wrapt
 
 from tribune import (
     LabeledColumn,
     PortraitRow,
@@ -239,48 +239,43 @@
         book = xlsx_to_reader(wb)
         return book.sheet_by_name('Car Info')
 
     def test_header(self):
         ws = self.generate_report()
         assert ws.cell_value(0, 0) == 'Cars'
 
-    def test_column_headings(self):
-        def checkit(ws, row, column, value):
-            assert ws.cell_value(row, column) == value
-
+    @pytest.mark.parametrize('row,column,value', [
+        (2, 0, ''),
+        (2, 1, 'Year'),
+        (2, 2, 'Make'),
+        (2, 3, 'Model'),
+        (2, 4, 'Style'),
+        (2, 5, 'Color'),
+        (2, 6, 'Blue'),
+        (3, 6, 'Book'),
+    ])
+    def test_column_headings(self, row, column, value):
         ws = self.generate_report()
-        for row, column, value in [
-            (2, 0, ''),
-            (2, 1, 'Year'),
-            (2, 2, 'Make'),
-            (2, 3, 'Model'),
-            (2, 4, 'Style'),
-            (2, 5, 'Color'),
-            (2, 6, 'Blue'),
-            (3, 6, 'Book'),
-        ]:
-            yield checkit, ws, row, column, value
-
-    def test_column_data(self):
-        def checkit(ws, row, column, value):
-            assert ws.cell_value(row, column) == value
+        assert ws.cell_value(row, column) == value
 
+    @pytest.mark.parametrize('data_row, data', enumerate(car_data(None)))
+    @pytest.mark.parametrize('header,key', [
+        ('Year', 'year'),
+        ('Make', 'make'),
+        ('Model', 'model'),
+        ('Style', 'style'),
+        ('Color', 'color'),
+        ('Blue', 'book_value'),
+    ])
+    def test_column_data(self, header, key, data_row, data):
         ws = self.generate_report()
-        for data_row, data in enumerate(car_data(None)):
-            row = data_row + 4
-            for column, value in [
-                (0, ''),
-                (find_sheet_col(ws, 'Year', 2), data['year']),
-                (find_sheet_col(ws, 'Make', 2), data['make']),
-                (find_sheet_col(ws, 'Model', 2), data['model']),
-                (find_sheet_col(ws, 'Style', 2), data['style']),
-                (find_sheet_col(ws, 'Color', 2), data['color']),
-                (find_sheet_col(ws, 'Blue', 2), data['book_value']),
-            ]:
-                yield checkit, ws, row, column, value
+        row = data_row + 4
+        col = header if isinstance(header, int) else find_sheet_col(ws, header, 2)
+        assert ws.cell_value(row, 0) == ''
+        assert ws.cell_value(row, col) == data[key]
 
     def test_merged_section_heading(self):
         class TestSheet(ReportSheet):
             class CarMergedHeaderSection(SheetSection):
                 LabeledColumn('Style', 'style')
                 LabeledColumn('Color', 'color')
 
@@ -327,58 +322,37 @@
         book = xlsx_to_reader(wb)
         return book.sheet_by_name('Dealership Summary')
 
     def test_header(self):
         ws = self.generate_report()
         assert ws.cell_value(0, 0) == 'Dealership'
 
-    def test_column_headings(self):
-        def checkit(ws, row, column, value):
-            assert ws.cell_value(row, column) == value
-
+    @pytest.mark.parametrize('row,column,value', [
+        (3, 0, ''),
+        (3, 1, 'Count'),
+        (3, 2, 'Income'),
+        (3, 3, 'Expense'),
+        (3, 4, 'Net'),
+    ])
+    def test_column_headings(self, row, column, value):
         ws = self.generate_report()
-        for row, column, value in [
-            (3, 0, ''),
-            (3, 1, 'Count'),
-            (3, 2, 'Income'),
-            (3, 3, 'Expense'),
-            (3, 4, 'Net'),
-        ]:
-            yield checkit, ws, row, column, value
-
-    def test_row_data(self):
-        def checkit(ws, row, column, value):
-            assert ws.cell_value(row, column) == value
+        assert ws.cell_value(row, column) == value
 
+    @pytest.mark.parametrize('row_header,column,value', [
+        ('Sales', 1, 5),
+        ('Sales', 2, 75000),
+        ('Sales', 3, 25000),
+        ('Sales', 4, 50000),
+        ('Rentals', 1, 46),
+        ('Rentals', 2, 8600),
+        ('Rentals', 3, 2900),
+        ('Rentals', 4, 5700),
+        ('Leases', 1, 27),
+        ('Leases', 2, 10548),
+        ('Leases', 3, 3680),
+        ('Leases', 4, 6868),
+        ('Totals', 4, 100000),
+    ])
+    def test_row_data(self, row_header, column, value):
         ws = self.generate_report()
-        row = find_sheet_row(ws, 'Sales', 0)
-        for column, value in [
-            (1, 5),
-            (2, 75000),
-            (3, 25000),
-            (4, 50000),
-        ]:
-            yield checkit, ws, row, column, value
-
-        row = find_sheet_row(ws, 'Rentals', 0)
-        for column, value in [
-            (1, 46),
-            (2, 8600),
-            (3, 2900),
-            (4, 5700),
-        ]:
-            yield checkit, ws, row, column, value
-
-        row = find_sheet_row(ws, 'Leases', 0)
-        for column, value in [
-            (1, 27),
-            (2, 10548),
-            (3, 3680),
-            (4, 6868),
-        ]:
-            yield checkit, ws, row, column, value
-
-        row = find_sheet_row(ws, 'Totals', 0)
-        for column, value in [
-            (4, 100000),
-        ]:
-            yield checkit, ws, row, column, value
+        row = find_sheet_row(ws, row_header, 0)
+        assert ws.cell_value(row, column) == value
```

### Comparing `tribune-0.2.2/tribune/tests/test_sheet_import_parsers.py` & `tribune-0.3.0/tribune/tests/test_sheet_import_parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 import pytest
 import tribune.sheet_import.parsers as p
 from .utils import assert_import_errors
 
 
 def assert_really_equal(left, right):
-    assert type(left) == type(right)
+    assert type(left) is type(right)
     assert left == right
 
 
 def test_chain():
     assert p.chain(lambda _: 'Python')(0.99) == 'Python'
     assert p.chain(lambda x: x + 1, lambda x: x - 1)(0) == 0
     assert p.chain(lambda x: x * 2, lambda x: x - 1)(1) == 1
     assert p.chain(lambda x: x - 1, lambda x: x * 2)(1) == 0
 
 
 def test_parse_text():
+    assert p.parse_text(None) == u''
     assert p.parse_text('') == u''
     assert p.parse_text('  ') == u''
     assert p.parse_text(' A ') == u'A'
 
 
 def test_parse_yes_no():
     assert p.parse_yes_no('yes') is True
```

### Comparing `tribune-0.2.2/tribune/tests/test_utils.py` & `tribune-0.3.0/tribune/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,23 +4,24 @@
     column_letter,
     deepcopy_tuple_except,
     split_every,
 )
 
 
 def test_column_letter():
-    assert column_letter(0) == 'A'
-    assert column_letter(2) == 'C'
-    assert column_letter(25) == 'Z'
-    assert column_letter(26) == 'AA'
-    assert column_letter(27) == 'AB'
-    assert column_letter(26*2) == 'BA'
-    assert column_letter(26*3) == 'CA'
-    assert column_letter(26**2+25) == 'ZZ'
-    assert column_letter(26**2+26) == 'AAA'
+    assert column_letter(1) == 'A'
+    assert column_letter(3) == 'C'
+    assert column_letter(26) == 'Z'
+    assert column_letter(27) == 'AA'
+    assert column_letter(28) == 'AB'
+    assert column_letter(26*2 + 1) == 'BA'
+    assert column_letter(26*3 + 1) == 'CA'
+    assert column_letter(26**2+26) == 'ZZ'
+    assert column_letter(26**2+27) == 'AAA'
+    assert column_letter(1, is_zero_based=True) == 'B'
 
 
 class TestDeepCopyTupleExcept(object):
     class DoDeepCopy:
         def __init__(self, value):
             self.value = value
```

### Comparing `tribune-0.2.2/tribune/tests/utils.py` & `tribune-0.3.0/tribune/tests/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import datetime as dt
 
-import six
 import sqlalchemy as sa
 import sqlalchemy.orm as saorm
 import sqlalchemy.sql as sasql
 import wrapt
 
 from tribune.sheet_import import SpreadsheetImportError
 
@@ -97,15 +96,15 @@
         structure.
         """
         # surrogate can be guessed from autoincrement/sequence but I guess
         # that's not 100% reliable, so we'll need an override
 
         mapper = saorm.object_mapper(self)
 
-        for key, value in six.iteritems(data):
+        for key, value in data.items():
             if isinstance(value, dict):
                 dbvalue = getattr(self, key)
                 rel_class = mapper.get_property(key).mapper.class_
                 pk_props = rel_class._descriptor.primary_key_properties
 
                 # If the data doesn't contain any pk, and the relationship
                 # already has a value, update that record.
```

### Comparing `tribune-0.2.2/tribune/utils.py` & `tribune-0.3.0/tribune/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,14 @@
     chain as _itertools_chain,
     count,
     islice,
     takewhile,
 )
 from functools import reduce
 
-from six.moves import map
-
 
 def raises(e):
     """A functional form of `raise`."""
     raise e
 
 
 def compose(*functions):
@@ -84,25 +82,27 @@
     than n elements.
 
     See http://stackoverflow.com/a/22919323/503377."""
     items = iter(iterable)
     return takewhile(bool, (list(islice(items, n)) for _ in count(0)))
 
 
-def column_letter(n):
+def column_letter(n, is_zero_based=False):
     """Returns the spreadsheet column name for a given 0-based column index.
 
     Adapted from http://stackoverflow.com/a/4532562/503377. Spreadsheet column names are a strange
     base-26 number (for 26 letters in the alphabet) where each place value is 1-based instead of
     0-based.
 
-    :param n: is a 0-based column index.
+    :param n: is an integer column index
+    :param is_zero_based: some libs zero-base int indices, so allow this to be controlled
     """
     alphabet = string.ascii_uppercase
 
-    n = n + 1  # Turn our 0-based number into a 1-based number.
+    if is_zero_based:
+        n = n + 1  # Turn our 0-based number into a 1-based number.
     name = ''  # initial column name
     while n > 0:
         n = n - 1  # Turn this place value into a 0-based number.
         name = alphabet[n % len(alphabet)] + name
         n //= len(alphabet)
     return name
```

### Comparing `tribune-0.2.2/tribune/__init__.py` & `tribune-0.3.0/tribune/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import copy
 from decimal import Decimal
 import sys
 from types import FunctionType
 
 from blazeutils.spreadsheets import WriterX
-import six
 from xlsxwriter.format import Format
 
 from .utils import (
     column_letter,
     deepcopy_tuple_except
 )
 
@@ -160,24 +159,24 @@
         self.sheet = sheet
         self.write_header = write_header_func or self.write_header
         self.write_data = write_data_func or self.write_data
         self.write_total = write_total_func or self.write_total
 
         # look for header values in kwargs, construct a header dict
         self._init_header = dict()
-        for k, v in six.iteritems(kwargs):
+        for k, v in kwargs.items():
             if k.startswith('header_'):
                 try:
                     self._init_header[int(k[7:])] = v
                 except ValueError:
                     pass
 
     def _construct_header_data(self, init_header):
         d = ['' for i in range(self.sheet.pre_data_rows)]
-        for k, v in six.iteritems(init_header):
+        for k, v in init_header.items():
             try:
                 d[k] = v
             except IndexError:
                 raise ProgrammingError('not enough pre-data rows on sheet')
         self.header_data = d
 
     def xls_width_calc(self, value):
@@ -389,15 +388,15 @@
         if not worksheet:
             worksheet = parent_book.add_worksheet(self.sheet_name)
         super(ReportSheet, self).__init__(ws=worksheet)
         self.set_base_style_dicts()
 
         # fetch records first, as units may need some data for initialization
         filter_args = dict([
-            (k[7:], v) for k, v in six.iteritems(kwargs) if k[:7] == 'filter_'
+            (k[7:], v) for k, v in kwargs.items() if k[:7] == 'filter_'
         ])
         self.records = self.fetch_records(**filter_args)
 
         # list of (row,col) tuples to guard when writing. Idea here is to have
         #   as short a list as possible, for performance (i.e. don't check
         #   xlwt's complete sheet or row list)
         self.locked_cells = []
```

### Comparing `tribune-0.2.2/tribune.egg-info/SOURCES.txt` & `tribune-0.3.0/tribune.egg-info/SOURCES.txt`

 * *Files identical despite different names*

