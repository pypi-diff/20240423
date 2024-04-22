# Comparing `tmp/ansi-string-1.0.1.tar.gz` & `tmp/ansi-string-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-1.0.1.tar", last modified: Sun Apr 21 22:02:49 2024, max compression
+gzip compressed data, was "ansi-string-1.0.2.tar", last modified: Mon Apr 22 02:46:44 2024, max compression
```

## Comparing `ansi-string-1.0.1.tar` & `ansi-string-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-21 22:02:42.000000 ansi-string-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 22:02:42.000000 ansi-string-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-21 22:02:49.074780 ansi-string-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-21 22:02:42.000000 ansi-string-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-21 22:02:42.000000 ansi-string-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 22:02:49.078780 ansi-string-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-21 22:02:42.000000 ansi-string-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-21 22:02:42.000000 ansi-string-1.0.1/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72102 2024-04-21 22:02:42.000000 ansi-string-1.0.1/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:02:49.074780 ansi-string-1.0.1/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 22:02:49.000000 ansi-string-1.0.1/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.853700 ansi-string-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 02:46:30.000000 ansi-string-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 02:46:30.000000 ansi-string-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-22 02:46:44.853700 ansi-string-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-22 02:46:30.000000 ansi-string-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 02:46:30.000000 ansi-string-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 02:46:44.853700 ansi-string-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 02:46:30.000000 ansi-string-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.849701 ansi-string-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.849701 ansi-string-1.0.2/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 02:46:30.000000 ansi-string-1.0.2/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73117 2024-04-22 02:46:30.000000 ansi-string-1.0.2/src/ansi_string/ansi_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.853700 ansi-string-1.0.2/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-1.0.1/LICENSE` & `ansi-string-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.1/PKG-INFO` & `ansi-string-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.1
+Version: 1.0.2
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -60,26 +60,26 @@
 
 ```py
 from ansi_string import en_tty_ansi, AnsiFormat, AnsiString
 ```
 
 ### Enabling ANSI Formatting
 
-Windows requires ANSI formatting to be enabled before it can be used. This can either be set in the environment or by simply calling the following before printing so that ANSI is enabled locally. This returns True when successful.
+Windows requires ANSI formatting to be enabled before it can be used. This can either be set in the environment or by simply calling the following before printing so that ANSI is enabled locally.
 ```py
 en_tty_ansi()
 ```
 
 If this also needs to be enabled for stderr, stderr may also be passed to this method.
 ```py
 import sys
 en_tty_ansi(sys.stderr)
 ```
 
-This function serves no purpose outside of Windows OS and will simply return True without action in those cases.
+For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY; no other action is taken.
 
 ### Construction
 
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
@@ -90,17 +90,17 @@
 - A string color name for a formatting directive (i.e. any name of the AnsiFormat enum in lower or upper case)
 - An AnsiFormat directive (ex: `AnsiFormat.BOLD`)
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
-    - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it will be treated as a decimal value
+    - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
-    - The string will normally be parsed and verified unless the character "[" is the first character of the string
+    - The string will normally be parsed into their individual values and verified unless the character "[" is the first character of the string (ex: `"[01;31"`)
 - A single ANSI directive as an integer
 
 Examples:
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
@@ -160,7 +160,11 @@
 Example:
 ```py
 s = AnsiString("Here is a strING that I will match formatting")
 # This will make the word "formatting" cyan with a pink background
 s.format_matching("[A-Za-z]+ing", "cyan", AnsiFormat.BG_PINK, regex=True, match_case=True)
 print(s)
 ```
+
+### Other String Manipulation Methods
+
+Many other methods that are found in the `str` class such as `replace()` are available in `AnsiString` which manipulate the string while applying formatting where necessary.
```

### Comparing `ansi-string-1.0.1/README.md` & `ansi-string-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,26 +32,26 @@
 
 ```py
 from ansi_string import en_tty_ansi, AnsiFormat, AnsiString
 ```
 
 ### Enabling ANSI Formatting
 
-Windows requires ANSI formatting to be enabled before it can be used. This can either be set in the environment or by simply calling the following before printing so that ANSI is enabled locally. This returns True when successful.
+Windows requires ANSI formatting to be enabled before it can be used. This can either be set in the environment or by simply calling the following before printing so that ANSI is enabled locally.
 ```py
 en_tty_ansi()
 ```
 
 If this also needs to be enabled for stderr, stderr may also be passed to this method.
 ```py
 import sys
 en_tty_ansi(sys.stderr)
 ```
 
-This function serves no purpose outside of Windows OS and will simply return True without action in those cases.
+For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY; no other action is taken.
 
 ### Construction
 
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
@@ -62,17 +62,17 @@
 - A string color name for a formatting directive (i.e. any name of the AnsiFormat enum in lower or upper case)
 - An AnsiFormat directive (ex: `AnsiFormat.BOLD`)
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
-    - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it will be treated as a decimal value
+    - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
-    - The string will normally be parsed and verified unless the character "[" is the first character of the string
+    - The string will normally be parsed into their individual values and verified unless the character "[" is the first character of the string (ex: `"[01;31"`)
 - A single ANSI directive as an integer
 
 Examples:
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
@@ -131,8 +131,12 @@
 The method `AnsiString.format_matching()` is provided to apply formatting to an `AnsiString` based on a match specification.
 Example:
 ```py
 s = AnsiString("Here is a strING that I will match formatting")
 # This will make the word "formatting" cyan with a pink background
 s.format_matching("[A-Za-z]+ing", "cyan", AnsiFormat.BG_PINK, regex=True, match_case=True)
 print(s)
-```
+```
+
+### Other String Manipulation Methods
+
+Many other methods that are found in the `str` class such as `replace()` are available in `AnsiString` which manipulate the string while applying formatting where necessary.
```

### Comparing `ansi-string-1.0.1/setup.py` & `ansi-string-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.1/src/ansi_string/ansi_string.py` & `ansi-string-1.0.2/src/ansi_string/ansi_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import sys
 import re
 import math
 from enum import Enum, auto as enum_auto
 import io
 from typing import Any, Union, List, Dict, Tuple
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 PACKAGE_NAME = 'ansi-string'
 
 WHITESPACE_CHARS = ' \t\n\r\v\f'
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 if IS_WINDOWS:
@@ -762,19 +762,19 @@
             b = (r_or_rgb & 0x0000FF)
         else:
             r=min(255, max(0, r_or_rgb))
             g=min(255, max(0, g))
             b=min(255, max(0, b))
 
         if component == ColorComponentType.UNDERLINE:
-            return f'{__class__.UNDERLINE.value};{__class__.SET_UNDERLINE_COLOR_RGB.value};{r};{g};{b}'
+            return f'[{__class__.UNDERLINE.value};{__class__.SET_UNDERLINE_COLOR_RGB.value};{r};{g};{b}'
         elif component == ColorComponentType.BACKGROUND:
-            return f'{__class__.BG_SET_RGB.value};{r};{g};{b}'
+            return f'[{__class__.BG_SET_RGB.value};{r};{g};{b}'
         else:
-            return f'{__class__.FG_SET_RGB.value};{r};{g};{b}'
+            return f'[{__class__.FG_SET_RGB.value};{r};{g};{b}'
 
 class AnsiString:
     '''
     Represents an ANSI colorized/formatted string. All or part of the string may contain style and
     color formatting which may be used to print out to an ANSI-supported terminal such as those
     on Linux, Mac, and Windows 10+.
 
@@ -809,14 +809,17 @@
     '''
 
     # The escape sequence that needs to be formatted with command str
     ANSI_ESCAPE_FORMAT = '\x1b[{}m'
     # The escape sequence which will clear all previous formatting (empty command is same as 0)
     ANSI_ESCAPE_CLEAR = ANSI_ESCAPE_FORMAT.format('')
 
+    # Change this to True for testing
+    WITH_ASSERTIONS = False
+
     # This isn't in AnsiFormat because it shouldn't be used externally
     RESET = '0'
 
     class Setting:
         '''
         Internal use only - mainly used to create a unique objects which may contain same strings
         '''
@@ -863,32 +866,34 @@
             component_dict = {
                 'ul_': ColorComponentType.UNDERLINE,
                 'bg_': ColorComponentType.BACKGROUND,
                 'fg_': ColorComponentType.FOREGROUND
             }
 
             # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 3 distinct values as decimal or hex
-            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\(\[?\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*\]?\)$', s)
+            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\([\[\()]?\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*[\)\]]?\)$', s)
             if match:
                 try:
                     r = int(match.group(3), 16 if match.group(2) else 10)
                     g = int(match.group(5), 16 if match.group(4) else 10)
                     b = int(match.group(7), 16 if match.group(6) else 10)
                 except ValueError:
                     raise ValueError('Invalid rgb value(s)')
-                return AnsiFormat.rgb(r, g, b, component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
+                # Get RGB format and remove the leading '['
+                return AnsiFormat.rgb(r, g, b, component_dict.get(match.group(1), ColorComponentType.FOREGROUND))[1:]
 
             # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 1 value as decimal or hex
-            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\(\[?\s*(0x)?([0-9a-fA-F]+)\s*\]?\)$', s)
+            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\([\[\()]?\s*(0x)?([0-9a-fA-F]+)\s*[\)\]]?\)$', s)
             if match:
                 try:
                     rgb = int(match.group(3), 16 if match.group(2) else 10)
                 except ValueError:
                     raise ValueError('Invalid rgb value')
-                return AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND))
+                # Get RGB format and remove the leading '['
+                return AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND))[1:]
             return None
 
         @staticmethod
         def _scrub_ansi_format_string(ansi_format:str) -> List[str]:
             if ansi_format.startswith("["):
                 # Use the rest of the string as-is for settings
                 return [ansi_format[1:]]
@@ -908,16 +913,16 @@
                     if ansi_fmt_enum is None:
                         rgb_format = __class__._parse_rgb_string(format)
                         if not rgb_format:
                             try:
                                 int_value = int(format)
                                 # 0 should never be used because it will mess with internal assumptions
                                 # Negative values are invalid
-                                if int_value <= 0:
-                                    raise ValueError(f'Invalid value [{int_value}]; must be greater than 0')
+                                if int_value < 0:
+                                    raise ValueError(f'Invalid value [{int_value}]; must be greater than or equal to 0')
                             except ValueError:
                                 raise ValueError(
                                     'AnsiString.__format__ failed to parse format ({}); invalid name: {}'
                                     .format(ansi_format, format)
                                 )
                             else:
                                 # Value is an integer - use the format verbatim
@@ -1122,15 +1127,16 @@
             for setting in settings.rem:
                 # setting object will only be matched and removed if it is the same reference to one
                 # previously added - will raise exception otherwise which should not happen if the
                 # settings dictionary and this method were setup correctly.
                 remove_idx = AnsiString._find_setting_reference(setting, self.current_settings)
                 if remove_idx >= 0:
                     del self.current_settings[remove_idx]
-                else:
+                elif AnsiString.WITH_ASSERTIONS:
+                    # This exception is really only useful in testing
                     raise ValueError('could not remove setting: not in list')
             # Apply settings that it is time to add
             self.current_settings += settings.add
             return (idx, settings, self.current_settings)
 
     class CharIterator:
         def __init__(self, s:'AnsiString'):
@@ -1319,23 +1325,29 @@
             out_str += __class__.ANSI_ESCAPE_CLEAR
 
         return out_str
 
     def __iter__(self):
         return iter(__class__.CharIterator(self))
 
-    def capitalize(self) -> 'AnsiString':
-        cpy = self.copy()
-        cpy._s = cpy._s.capitalize()
-        return cpy
+    def capitalize(self, inplace:bool=False) -> 'AnsiString':
+        if inplace:
+            obj = self
+        else:
+            obj = self.copy()
+        obj._s = obj._s.capitalize()
+        return obj
 
-    def casefold(self) -> 'AnsiString':
-        cpy = self.copy()
-        cpy._s = cpy._s.casefold()
-        return cpy
+    def casefold(self, inplace:bool=False) -> 'AnsiString':
+        if inplace:
+            obj = self
+        else:
+            obj = self.copy()
+        obj._s = obj._s.casefold()
+        return obj
 
     def center(self, width:int, fillchar:str=' ', inplace:bool=False) -> 'AnsiString':
         '''
         Center justification.
         inplace: True to execute in-place; False to return a copy
         '''
         if inplace:
@@ -1392,15 +1404,15 @@
         if num > 0:
             obj._s = fillchar * num + obj._s
             # Shift all indices except for the origin (formats the left fillchars with same as first char)
             __class__._shift_settings_idx(obj._fmts, num, True)
 
         return obj
 
-    def count(self, sub:str, start:int, end:int) -> int:
+    def count(self, sub:str, start:int=None, end:int=None) -> int:
         return self._s.count(sub, start, end)
 
     def encode(self, encoding:str="utf-8", errors:str="strict") -> bytes:
         return str(self).encode(encoding, errors)
 
     def endswith(self, suffix:str, start:int=None, end:int=None) -> bool:
         return self._s.endswith(suffix, start, end)
@@ -1417,14 +1429,17 @@
     def isalnum(self) -> bool:
         return self._s.isalnum()
 
     def isalpha(self) -> bool:
         return self._s.isalpha()
 
     def isascii(self) -> bool:
+        '''
+        This is only available for Python >=3.7
+        '''
         return self._s.isascii()
 
     def isdecimal(self) -> bool:
         return self._s.isdecimal()
 
     def isdigit(self) -> bool:
         return self._s.isdigit()
@@ -1493,15 +1508,15 @@
                         for find_idx, add_idx in reversed(finds):
                             self._fmts[key].rem[add_idx] = replace_settings[find_idx]
                             # Note: find_idx will always be sorted in ascending order and this is iterating in reverse
                             del find_settings[find_idx]
                             del replace_settings[find_idx]
 
         else:
-            raise ValueError(f'value is invalid type: {type(value)}')
+            raise TypeError(f'value is invalid type: {type(value)}')
         return self
 
     def __eq__(self, value:'AnsiString') -> bool:
         if not isinstance(value, AnsiString):
             return False
         return self._s == value._s and self._fmts == value._fmts
 
@@ -1522,15 +1537,15 @@
         args = list(args)
         first_arg = args[0]
         if isinstance(first_arg, str):
             joint = AnsiString(first_arg)
         elif isinstance(first_arg, AnsiString):
             joint = first_arg.copy()
         else:
-            raise ValueError(f'value is invalid type: {type(first_arg)}')
+            raise TypeError(f'value is invalid type: {type(first_arg)}')
         for arg in args[1:]:
             joint += arg
         return joint
 
     def lower(self, inplace:bool=False) -> 'AnsiString':
         '''
         Convert to lowercase.
@@ -1548,15 +1563,15 @@
         Convert to uppercase.
         inplace: True to execute in-place; False to return a copy
         '''
         if inplace:
             obj = self
         else:
             obj = self.copy()
-        obj._s = obj._s.lower()
+        obj._s = obj._s.upper()
         return obj
 
     def lstrip(self, chars:str=None, inplace:bool=False) -> 'AnsiString':
         '''
         Remove leading whitespace
         chars: If not None, remove characters in chars instead
         inplace: True to execute in-place; False to return a copy
@@ -1656,27 +1671,30 @@
         if idx >= 0:
             sep_len = len(sep)
             idx_end = idx + sep_len
             return (self[0:idx], self[idx:idx_end], self[idx_end:])
         else:
             return (self.copy(), AnsiString(), AnsiString())
 
-    def settings_at(self, idx:int) -> str:
-        '''
-        Returns a string which represents the settings being used at the given index
-        '''
+    def _settings_at(self, idx:int) -> List[Setting]:
         if idx >= 0 and idx < len(self._s):
             previous_settings = []
             for sidx, _, current_settings in __class__.SettingsIterator(self._fmts):
                 if sidx > idx:
                     break
                 previous_settings = list(current_settings)
-            return ';'.join(str(s) for s in previous_settings)
+            return previous_settings
         else:
-            return ''
+            return []
+
+    def settings_at(self, idx:int) -> str:
+        '''
+        Returns a string which represents the settings being used at the given index
+        '''
+        return ';'.join(str(s) for s in self._settings_at(idx))
 
     def removeprefix(self, prefix:str, inplace:bool=False) -> 'AnsiString':
         if not self._s.startswith(prefix):
             if inplace:
                 return self
             else:
                 return self.copy()
@@ -1689,21 +1707,29 @@
                 return self
             else:
                 return self.copy()
         else:
             return self.clip(end=-len(suffix), inplace=inplace)
 
     def replace(self, old:str, new:Union[str,'AnsiString'], count:int=-1, inplace:bool=False) -> 'AnsiString':
+        '''
+        Does a find-and-replace - if new is a str, the string the is applied will take on the format settings of the
+        first character of the old string in each replaced item.
+        '''
         obj = self
-        idx = self._s.find(old)
+        idx = obj._s.find(old)
         while (count < 0 or count > 0) and idx >= 0:
-            obj = self[:idx] + new + self[idx+len(new):]
+            if isinstance(new, str):
+                replace = AnsiString(new, obj._settings_at(idx))
+            else:
+                replace = new
+            obj = obj[:idx] + replace + obj[idx+len(old):]
             if count > 0:
                 count -= 1
-            idx = self._s.find(old, idx + len(old))
+            idx = obj._s.find(old, idx + len(new))
 
         if inplace:
             self._s = obj._s
             self._fmts = obj._fmts
             return self
         else:
             return obj
```

### Comparing `ansi-string-1.0.1/src/ansi_string.egg-info/PKG-INFO` & `ansi-string-1.0.2/src/ansi_string.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.1
+Version: 1.0.2
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -60,26 +60,26 @@
 
 ```py
 from ansi_string import en_tty_ansi, AnsiFormat, AnsiString
 ```
 
 ### Enabling ANSI Formatting
 
-Windows requires ANSI formatting to be enabled before it can be used. This can either be set in the environment or by simply calling the following before printing so that ANSI is enabled locally. This returns True when successful.
+Windows requires ANSI formatting to be enabled before it can be used. This can either be set in the environment or by simply calling the following before printing so that ANSI is enabled locally.
 ```py
 en_tty_ansi()
 ```
 
 If this also needs to be enabled for stderr, stderr may also be passed to this method.
 ```py
 import sys
 en_tty_ansi(sys.stderr)
 ```
 
-This function serves no purpose outside of Windows OS and will simply return True without action in those cases.
+For Windows, this returns True if the given IO is a TTY (i.e. not piped to a file) and enabling ANSI was successful. For all other operating systems, this will return True if and only if the given IO is a TTY; no other action is taken.
 
 ### Construction
 
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
@@ -90,17 +90,17 @@
 - A string color name for a formatting directive (i.e. any name of the AnsiFormat enum in lower or upper case)
 - An AnsiFormat directive (ex: `AnsiFormat.BOLD`)
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
-    - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it will be treated as a decimal value
+    - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
-    - The string will normally be parsed and verified unless the character "[" is the first character of the string
+    - The string will normally be parsed into their individual values and verified unless the character "[" is the first character of the string (ex: `"[01;31"`)
 - A single ANSI directive as an integer
 
 Examples:
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
@@ -160,7 +160,11 @@
 Example:
 ```py
 s = AnsiString("Here is a strING that I will match formatting")
 # This will make the word "formatting" cyan with a pink background
 s.format_matching("[A-Za-z]+ing", "cyan", AnsiFormat.BG_PINK, regex=True, match_case=True)
 print(s)
 ```
+
+### Other String Manipulation Methods
+
+Many other methods that are found in the `str` class such as `replace()` are available in `AnsiString` which manipulate the string while applying formatting where necessary.
```

