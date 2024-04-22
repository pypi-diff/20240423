# Comparing `tmp/ansi-string-1.0.2.tar.gz` & `tmp/ansi-string-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansi-string-1.0.2.tar", last modified: Mon Apr 22 02:46:44 2024, max compression
+gzip compressed data, was "ansi-string-1.0.3.tar", last modified: Mon Apr 22 23:32:26 2024, max compression
```

## Comparing `ansi-string-1.0.2.tar` & `ansi-string-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.853700 ansi-string-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 02:46:30.000000 ansi-string-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 02:46:30.000000 ansi-string-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-22 02:46:44.853700 ansi-string-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-22 02:46:30.000000 ansi-string-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 02:46:30.000000 ansi-string-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 02:46:44.853700 ansi-string-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 02:46:30.000000 ansi-string-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.849701 ansi-string-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.849701 ansi-string-1.0.2/src/ansi_string/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 02:46:30.000000 ansi-string-1.0.2/src/ansi_string/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73117 2024-04-22 02:46:30.000000 ansi-string-1.0.2/src/ansi_string/ansi_string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 02:46:44.853700 ansi-string-1.0.2/src/ansi_string.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 02:46:44.000000 ansi-string-1.0.2/src/ansi_string.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-22 23:32:19.000000 ansi-string-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 23:32:19.000000 ansi-string-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-22 23:32:26.836627 ansi-string-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-22 23:32:19.000000 ansi-string-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-22 23:32:19.000000 ansi-string-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 23:32:26.840627 ansi-string-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-22 23:32:19.000000 ansi-string-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/src/ansi_string/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 23:32:19.000000 ansi-string-1.0.3/src/ansi_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75795 2024-04-22 23:32:19.000000 ansi-string-1.0.3/src/ansi_string/ansi_string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:32:26.836627 ansi-string-1.0.3/src/ansi_string.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 23:32:26.000000 ansi-string-1.0.3/src/ansi_string.egg-info/top_level.txt
```

### Comparing `ansi-string-1.0.2/LICENSE` & `ansi-string-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.2/PKG-INFO` & `ansi-string-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.2
+Version: 1.0.3
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -31,30 +31,30 @@
 ANSI String Formatter in Python for CLI Color and Style Formatting
 
 ## Introduction
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
 
 The main goals for this project are:
-- To provide a simple way to construct an object with ANSI formatting without requiring the developer to know how ANSI formatting works
+- To provide a simple way to construct a string-like object with embedded ANSI formatting without requiring the developer to know how ANSI formatting works
 - Provide a way to further format the object using format string
 - Allow for concatenation of the object
 
 ## Contribution
 
 Feel free to open a bug report or make a merge request on [github](https://github.com/Tails86/ansi-string/issues).
 
 ## Installation
 This project is uploaded to PyPI at https://pypi.org/project/ansi-string
 
 To install, ensure you are connected to the internet and execute: `python3 -m pip install ansi-string --upgrade`
 
 ## Examples
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/0e2c943f25ccc219256204511fd308652a8075c0/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/36530493c87e282914d23d551ce427203fcd2719/docs/examples.jpg)
 
 Refer to the [test file](https://github.com/Tails86/ansi-string/blob/main/tests/test_ansi_string.py) for more examples on how to use the AnsiString class.
 
 ## Usage
 
 To begin, import AnsiString from the ansi_string module.
 
@@ -82,25 +82,30 @@
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
     def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]): ...
 ```
 
-The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting directives that can be applied to the entire string. These arguments can be in the form of any of the following:
-- A string color name for a formatting directive (i.e. any name of the AnsiFormat enum in lower or upper case)
-- An AnsiFormat directive (ex: `AnsiFormat.BOLD`)
+The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting setting directives that can be applied to the entire string. These arguments can be in the form of any of the following.
+- An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
+- A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
+- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, or `AnsiFormat.ul_rgb()`
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
     - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
+
+A formatting setting may also be any of the following, but it's not advised to specify settings these ways unless there is a specific reason to do so.
+- An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
-    - The string will normally be parsed into their individual values and verified unless the character "[" is the first character of the string (ex: `"[01;31"`)
+    - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
+    - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
```

### Comparing `ansi-string-1.0.2/README.md` & `ansi-string-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 ANSI String Formatter in Python for CLI Color and Style Formatting
 
 ## Introduction
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
 
 The main goals for this project are:
-- To provide a simple way to construct an object with ANSI formatting without requiring the developer to know how ANSI formatting works
+- To provide a simple way to construct a string-like object with embedded ANSI formatting without requiring the developer to know how ANSI formatting works
 - Provide a way to further format the object using format string
 - Allow for concatenation of the object
 
 ## Contribution
 
 Feel free to open a bug report or make a merge request on [github](https://github.com/Tails86/ansi-string/issues).
 
 ## Installation
 This project is uploaded to PyPI at https://pypi.org/project/ansi-string
 
 To install, ensure you are connected to the internet and execute: `python3 -m pip install ansi-string --upgrade`
 
 ## Examples
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/0e2c943f25ccc219256204511fd308652a8075c0/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/36530493c87e282914d23d551ce427203fcd2719/docs/examples.jpg)
 
 Refer to the [test file](https://github.com/Tails86/ansi-string/blob/main/tests/test_ansi_string.py) for more examples on how to use the AnsiString class.
 
 ## Usage
 
 To begin, import AnsiString from the ansi_string module.
 
@@ -54,25 +54,30 @@
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
     def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]): ...
 ```
 
-The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting directives that can be applied to the entire string. These arguments can be in the form of any of the following:
-- A string color name for a formatting directive (i.e. any name of the AnsiFormat enum in lower or upper case)
-- An AnsiFormat directive (ex: `AnsiFormat.BOLD`)
+The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting setting directives that can be applied to the entire string. These arguments can be in the form of any of the following.
+- An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
+- A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
+- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, or `AnsiFormat.ul_rgb()`
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
     - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
+
+A formatting setting may also be any of the following, but it's not advised to specify settings these ways unless there is a specific reason to do so.
+- An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
-    - The string will normally be parsed into their individual values and verified unless the character "[" is the first character of the string (ex: `"[01;31"`)
+    - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
+    - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
```

### Comparing `ansi-string-1.0.2/setup.py` & `ansi-string-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `ansi-string-1.0.2/src/ansi_string/ansi_string.py` & `ansi-string-1.0.3/src/ansi_string/ansi_string.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import sys
 import re
 import math
 from enum import Enum, auto as enum_auto
 import io
 from typing import Any, Union, List, Dict, Tuple
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 PACKAGE_NAME = 'ansi-string'
 
 WHITESPACE_CHARS = ' \t\n\r\v\f'
 
 IS_WINDOWS = sys.platform.lower().startswith('win')
 
 if IS_WINDOWS:
@@ -89,15 +89,17 @@
 
 ColourComponentType = ColorComponentType  # Alias for my British English friends
 
 class AnsiFormat(Enum):
     '''
     Formatting which may be supplied to AnsiString.
     '''
-    # Never use RESET
+
+    # RESET (0) is not defined here because it shouldn't be used with AnsiString
+
     BOLD='1'
     FAINT='2'
     ITALIC='3'
     ITALICS=ITALIC # Alias
     UNDERLINE='4'
     SLOW_BLINK='5'
     RAPID_BLINK='6'
@@ -740,17 +742,17 @@
 
     @staticmethod
     def rgb(
         r_or_rgb:int,
         g:Union[int,None]=None,
         b:Union[int,None]=None,
         component:ColorComponentType=ColorComponentType.FOREGROUND
-    ) -> str:
+    ) -> 'AnsiSetting':
         '''
-        Generates a FG or BG ANSI sequence for the given RGB values.
+        Generates a FG, BG, or UL ANSI sequence for the given RGB values.
         r_or_rgb: Either an 8-bit red component or the full 24-bit RGB value
         g: An 8-bit green component (b must also be specified when set)
         b: An 8-bit blue component (g must also be specified when set)
         component: The component to set color of (background, foreground, or underline)
         '''
         if r_or_rgb is None:
             raise ValueError('r_or_rgb must not be None')
@@ -762,221 +764,129 @@
             b = (r_or_rgb & 0x0000FF)
         else:
             r=min(255, max(0, r_or_rgb))
             g=min(255, max(0, g))
             b=min(255, max(0, b))
 
         if component == ColorComponentType.UNDERLINE:
-            return f'[{__class__.UNDERLINE.value};{__class__.SET_UNDERLINE_COLOR_RGB.value};{r};{g};{b}'
+            return AnsiSetting(f'{__class__.UNDERLINE.value};{__class__.SET_UNDERLINE_COLOR_RGB.value};{r};{g};{b}')
         elif component == ColorComponentType.BACKGROUND:
-            return f'[{__class__.BG_SET_RGB.value};{r};{g};{b}'
+            return AnsiSetting(f'{__class__.BG_SET_RGB.value};{r};{g};{b}')
         else:
-            return f'[{__class__.FG_SET_RGB.value};{r};{g};{b}'
+            return AnsiSetting(f'{__class__.FG_SET_RGB.value};{r};{g};{b}')
+
+    @staticmethod
+    def fg_rgb(r_or_rgb:int, g:Union[int,None]=None, b:Union[int,None]=None) -> 'AnsiSetting':
+        '''
+        Generates a foreground ANSI sequence for the given RGB values.
+        r_or_rgb: Either an 8-bit red component or the full 24-bit RGB value
+        g: An 8-bit green component (b must also be specified when set)
+        b: An 8-bit blue component (g must also be specified when set)
+        '''
+        return AnsiFormat.rgb(r_or_rgb, g, b)
+
+    @staticmethod
+    def bg_rgb(r_or_rgb:int, g:Union[int,None]=None, b:Union[int,None]=None) -> 'AnsiSetting':
+        '''
+        Generates a background ANSI sequence for the given RGB values.
+        r_or_rgb: Either an 8-bit red component or the full 24-bit RGB value
+        g: An 8-bit green component (b must also be specified when set)
+        b: An 8-bit blue component (g must also be specified when set)
+        '''
+        return AnsiFormat.rgb(r_or_rgb, g, b, ColorComponentType.BACKGROUND)
+
+    @staticmethod
+    def ul_rgb(r_or_rgb:int, g:Union[int,None]=None, b:Union[int,None]=None) -> 'AnsiSetting':
+        '''
+        Generates a underline ANSI sequence for the given RGB values.
+        r_or_rgb: Either an 8-bit red component or the full 24-bit RGB value
+        g: An 8-bit green component (b must also be specified when set)
+        b: An 8-bit blue component (g must also be specified when set)
+        '''
+        return AnsiFormat.rgb(r_or_rgb, g, b, ColorComponentType.UNDERLINE)
+
+class AnsiSetting:
+    '''
+    This class is used to wrap ANSI values which constitute as a single setting. Giving an AnsiSetting to the
+    constructor of AnsiString has a similar effect as providing a format string which starts with "[".
+    '''
+    def __init__(self, setting:Union[str, int, List[int], Tuple[int], AnsiFormat]):
+        if isinstance(setting, list) or isinstance(setting, tuple):
+            setting = ';'.join([str(s) for s in setting])
+        elif isinstance(setting, int):
+            setting = str(setting)
+        elif hasattr(setting, 'value') and isinstance(setting.value, str):
+            # Likely an enumeration - use the value
+            setting = setting.value
+        elif not isinstance(setting, str):
+            raise TypeError('Unsupported type for setting: {}'.format(type(setting)))
+
+        self._str = setting
+
+    def __eq__(self, value) -> bool:
+        if isinstance(value, str):
+            return self._str == value
+        elif isinstance(value, AnsiSetting):
+            return self._str == value._str
+        return False
+
+    def __str__(self) -> str:
+        return self._str
 
 class AnsiString:
     '''
     Represents an ANSI colorized/formatted string. All or part of the string may contain style and
     color formatting which may be used to print out to an ANSI-supported terminal such as those
     on Linux, Mac, and Windows 10+.
-
-    Example 1:
-    s = AnsiString('This string is red and bold string', [AnsiFormat.BOLD, AnsiFormat.FG_RED])
-    print(s)
-
-    Example 2:
-    s = AnsiString('This string contains custom formatting', '38;2;175;95;95')
-    print(s)
-
-    Example 3:
-    s = AnsiString('This string contains multiple color settings across different ranges')
-    s.apply_formatting(AnsiFormat.BOLD, 5, 11)
-    s.apply_formatting(AnsiFormat.BG_BLUE, 21, 29)
-    s.apply_formatting([AnsiFormat.FG_ORANGE, AnsiFormat.ITALIC], 21, 35)
-    print(s)
-
-    Example 4:
-    s = AnsiString('This string will be formatted bold and red')
-    print('{::01;31}'.format(s))
-
-    Example 5:
-    s = AnsiString('This string will be formatted bold and red')
-    # Use any name within AnsiFormat (can be lower or upper case representation of the name)
-    print('{::bold;fg_red}'.format(s))
-
-    Example 6:
-    s = AnsiString('This string will be formatted bold and red')
-    # The character '[' tells the format method to do no parsing/checking and use verbatim as codes
-    print('{::[01;31}'.format(s))
     '''
 
     # The escape sequence that needs to be formatted with command str
     ANSI_ESCAPE_FORMAT = '\x1b[{}m'
     # The escape sequence which will clear all previous formatting (empty command is same as 0)
     ANSI_ESCAPE_CLEAR = ANSI_ESCAPE_FORMAT.format('')
 
     # Change this to True for testing
     WITH_ASSERTIONS = False
 
     # This isn't in AnsiFormat because it shouldn't be used externally
-    RESET = '0'
+    RESET_VALUE = '0'
 
-    class Setting:
+    def __init__(
+        self,
+        s:str='',
+        *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting']
+    ):
         '''
-        Internal use only - mainly used to create a unique objects which may contain same strings
+        Creates an AnsiString
+        s: The underlying string
+        setting_or_settings: setting(s) in any of the listed formats below
+            - An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
+            - A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
+            - The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, or
+              `AnsiFormat.ul_rgb()`
+            - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
+                - `rgb(...)` or `fg_rgb(...)` to adjust text color
+                - `bg_rgb(...)` to adjust background color
+                - `ul_rgb(...)` to enable underline and set the underline color
+                - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
+                - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x",
+                  otherwise it is treated as a decimal value
+
+        A setting may also be any of the following, but it's not advised to specify settings these ways unless there is
+        a specific reason to do so.
+            - An AnsiSetting object
+            - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
+                - The string will normally be parsed into separate settings unless the character "[" is the first
+                  character of the string (ex: `"[38;5;214"`)
+                - Never specify the reset directive (0) because this is implicitly handled internally
+            - A single ANSI directive as an integer
         '''
-        def __init__(self, setting:Union[str, int, AnsiFormat]):
-            if isinstance(setting, int):
-                setting = str(setting)
-            elif hasattr(setting, 'value') and isinstance(setting.value, str):
-                # Likely an enumeration - use the value
-                setting = setting.value
-            elif not isinstance(setting, str):
-                raise TypeError('Unsupported type for setting_or_settings: {}'.format(type(setting)))
-
-            self._str = setting
-
-        def __eq__(self, value) -> bool:
-            if isinstance(value, str):
-                return self._str == value
-            elif isinstance(value, AnsiString.Setting):
-                return self._str == value._str
-            return False
-
-        def __str__(self) -> str:
-            return self._str
-
-    class SettingPoint:
-        def __init__(
-            self,
-            add:Union[List['AnsiString.Setting'],None]=None,
-            rem:Union[List['AnsiString.Setting'],None]=None
-        ):
-            self.add:List[AnsiString.Setting] = add or []
-            self.rem:List[AnsiString.Setting] = rem or []
-
-        def __eq__(self, value) -> bool:
-            if isinstance(value, AnsiString.SettingPoint):
-                return value.add == self.add and value.rem == self.rem
-            return False
-
-        def __bool__(self) -> bool:
-            return bool(self.add) or bool(self.rem)
-
-        @staticmethod
-        def _parse_rgb_string(s:str) -> str:
-            component_dict = {
-                'ul_': ColorComponentType.UNDERLINE,
-                'bg_': ColorComponentType.BACKGROUND,
-                'fg_': ColorComponentType.FOREGROUND
-            }
-
-            # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 3 distinct values as decimal or hex
-            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\([\[\()]?\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*[\)\]]?\)$', s)
-            if match:
-                try:
-                    r = int(match.group(3), 16 if match.group(2) else 10)
-                    g = int(match.group(5), 16 if match.group(4) else 10)
-                    b = int(match.group(7), 16 if match.group(6) else 10)
-                except ValueError:
-                    raise ValueError('Invalid rgb value(s)')
-                # Get RGB format and remove the leading '['
-                return AnsiFormat.rgb(r, g, b, component_dict.get(match.group(1), ColorComponentType.FOREGROUND))[1:]
-
-            # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 1 value as decimal or hex
-            match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\([\[\()]?\s*(0x)?([0-9a-fA-F]+)\s*[\)\]]?\)$', s)
-            if match:
-                try:
-                    rgb = int(match.group(3), 16 if match.group(2) else 10)
-                except ValueError:
-                    raise ValueError('Invalid rgb value')
-                # Get RGB format and remove the leading '['
-                return AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND))[1:]
-            return None
-
-        @staticmethod
-        def _scrub_ansi_format_string(ansi_format:str) -> List[str]:
-            if ansi_format.startswith("["):
-                # Use the rest of the string as-is for settings
-                return [ansi_format[1:]]
-            else:
-                # The format string contains names within AnsiFormat or integers, separated by semicolon
-                formats = ansi_format.split(';')
-                format_settings_strs = []
-                for format in formats:
-                    ansi_fmt_enum = None
-                    try:
-                        ansi_fmt_enum = AnsiFormat[format.upper()]
-                    except KeyError:
-                        pass
-                    else:
-                        format_settings_strs.append(ansi_fmt_enum.value)
-
-                    if ansi_fmt_enum is None:
-                        rgb_format = __class__._parse_rgb_string(format)
-                        if not rgb_format:
-                            try:
-                                int_value = int(format)
-                                # 0 should never be used because it will mess with internal assumptions
-                                # Negative values are invalid
-                                if int_value < 0:
-                                    raise ValueError(f'Invalid value [{int_value}]; must be greater than or equal to 0')
-                            except ValueError:
-                                raise ValueError(
-                                    'AnsiString.__format__ failed to parse format ({}); invalid name: {}'
-                                    .format(ansi_format, format)
-                                )
-                            else:
-                                # Value is an integer - use the format verbatim
-                                format_settings_strs.append(format)
-                        else:
-                            format_settings_strs.append(rgb_format)
-                return format_settings_strs
-
-        def insert_setting(self, apply:bool, setting:'AnsiString.Setting', topmost:bool=True):
-            lst = self.add if apply else self.rem
-            if topmost:
-                lst.append(setting)
-            else:
-                lst.insert(0, setting)
-
-        def insert_settings(
-            self,
-            apply:bool,
-            settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiString.Setting'], 'AnsiString.Setting'],
-            topmost:bool=True
-        ) -> List['AnsiString.Setting']:
-            if not isinstance(settings, list) and not isinstance(settings, tuple):
-                settings = [settings]
-
-            settings_to_insert = []
-            for setting in settings:
-                if isinstance(setting, AnsiString.Setting):
-                    settings_to_insert.append(setting)
-                elif isinstance(setting, str) or isinstance(setting, int):
-                    settings_to_insert.extend([AnsiString.Setting(s) for s in __class__._scrub_ansi_format_string(str(setting))])
-                elif hasattr(setting, "value") and isinstance(setting.value, str):
-                    settings_to_insert.append(AnsiString.Setting(setting.value))
-
-            lst = self.add if apply else self.rem
-            if topmost:
-                lst.extend(settings_to_insert)
-            else:
-                lst[:0] = settings_to_insert
-
-            return settings_to_insert
-
-    def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]):
         self._s = s
         # Key is the string index to make a color change at
-        # Each value element is a list of 2 lists
-        #   index 0: the settings to apply at this string index
-        #   index 1: the settings to remove at this string index
-        # TODO: it likely makes sense to create a separate class to maintain setting lists. This map of lists gets
-        #       really difficult to read!
-        self._fmts:Dict[int,'AnsiString.SettingPoint'] = {}
+        self._fmts:Dict[int,'_AnsiSettingPoint'] = {}
 
         # Unpack settings
         settings = []
         for sos in setting_or_settings:
             if not isinstance(sos, list) and not isinstance(sos, tuple):
                 settings.append(sos)
             else:
@@ -1004,75 +914,88 @@
         '''
         return self._s
 
     def copy(self) -> 'AnsiString':
         return self[:]
 
     @staticmethod
-    def _shift_settings_idx(settings_dict:Dict[int,'AnsiString.SettingPoint'], num:int, keep_origin:bool):
+    def _shift_settings_idx(settings_dict:Dict[int,'_AnsiSettingPoint'], num:int, keep_origin:bool):
         '''
         Not fully supported for when num is negative
         '''
         for key in sorted(settings_dict.keys(), reverse=(num > 0)):
             if not keep_origin or key != 0:
                 new_key = max(key + num, 0)
                 # new_key could be negative when num is negative - TODO: either handle or raise exception
                 settings_dict[new_key] = settings_dict.pop(key)
 
     def _insert_settings(
         self,
         idx:int,
         apply:bool,
-        settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiString.Setting'], 'AnsiString.Setting'],
+        settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting'],
         topmost:bool=True
-    ) -> List['AnsiString.Setting']:
+    ) -> List['AnsiSetting']:
         if idx not in self._fmts:
-            self._fmts[idx] = __class__.SettingPoint()
+            self._fmts[idx] = _AnsiSettingPoint()
         return self._fmts[idx].insert_settings(apply, settings, topmost)
 
     def apply_formatting(
             self,
-            setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiString.Setting'], 'AnsiString.Setting'],
+            setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting'],
             start:int=0,
             end:Union[int,None]=None,
             topmost:bool=True
     ):
         '''
         Sets the formatting for a given range of characters.
-        Inputs: setting_or_settings - Can either be a single item or list of items;
-                                      each item can either be a string or AnsiFormat type
+        Inputs: setting_or_settings - setting or list of settings to apply
                 start - The string start index where setting(s) are to be applied
                 end - The string index where the setting(s) should be removed
                 topmost - When true, this setting is placed at the end of the set for the given
-                        start_index meaning it is applied last; when false, setting is applied first
-
-        Note: The desired effect may not be achieved if the same setting is applied over an
-              overlapping range of characters.
+                          start_index meaning it takes precedent over others; when false, setting is
+                          applied first
         '''
         start = self._slice_val_to_idx(start, 0)
         end = self._slice_val_to_idx(end, len(self._s))
 
         if not setting_or_settings or start >= len(self._s) or end <= start:
             # Ignore - nothing to apply
             return
 
+        if not isinstance(setting_or_settings, list) and not isinstance(setting_or_settings, tuple):
+            settings = [setting_or_settings]
+        else:
+            settings = list(setting_or_settings)
+
+        # Settings are removed by reference (using "is" instead of "==") because this is easier than generating unique
+        # IDs, so it is necessary to ensure the incoming settings have distinct references. It would be possible to do
+        # so only if the setting is not already in self._fmts[*].add, but it doesn't add much more overhead to just make
+        # a copy for every incoming AnsiSetting.
+        for i in range(len(settings)):
+            if isinstance(settings[i], AnsiSetting):
+                settings[i] = AnsiSetting(str(settings[i]))
+
         # Apply settings
-        inserted_settings = self._insert_settings(start, True, setting_or_settings, topmost)
+        inserted_settings = self._insert_settings(start, True, settings, topmost)
 
         # Remove settings
         self._insert_settings(end, False, inserted_settings, topmost)
 
     def apply_formatting_for_match(
             self,
             setting_or_settings:Union[List[str], str, List[AnsiFormat], AnsiFormat],
             match_object,
             group:int=0
     ):
         '''
         Apply formatting using a match object generated from re
+        setting_or_settings - setting or list of settings to apply to matching strings
+        match_object - the match object to use (result of re.search() or re.finditer())
+        group - match the group to set
         '''
         s = match_object.start(group)
         e = match_object.end(group)
         self.apply_formatting(setting_or_settings, s, e)
 
     def format_matching(self, matchspec:str, *format, regex:bool=False, match_case=False):
         '''
@@ -1091,71 +1014,29 @@
     def clear_formatting(self):
         '''
         Clears all internal formatting.
         '''
         self._fmts = {}
 
     @staticmethod
-    def _find_setting_reference(find:Setting, in_list:List[Setting]) -> int:
+    def _find_setting_reference(find:AnsiSetting, in_list:List[AnsiSetting]) -> int:
         for i, s in enumerate(in_list):
             if s is find:
                 return i
         return -1
 
     @staticmethod
-    def _find_settings_references(find_list:List[Setting], in_list:List[Setting]) -> List[Tuple]:
+    def _find_settings_references(find_list:List[AnsiSetting], in_list:List[AnsiSetting]) -> List[Tuple]:
         matches = []
         for i, s in enumerate(find_list):
             for i2, s2 in enumerate(in_list):
                 if s is s2:
                     matches.append((i, i2))
         return matches
 
-    class SettingsIterator:
-        def __init__(self, settings_dict:Dict[int,'AnsiString.SettingPoint']):
-            self.settings_dict:Dict[int,AnsiString.SettingPoint] = settings_dict
-            self.current_settings:List[AnsiString.Setting] = []
-            self.dict_iter = iter(sorted(self.settings_dict))
-
-        def __iter__(self):
-            return self
-
-        def __next__(self) -> Tuple[int,'AnsiString.SettingPoint',List['AnsiString.Setting']]:
-            # Will raise StopIteration when complete
-            idx = next(self.dict_iter)
-            settings = self.settings_dict[idx]
-            # Remove settings that it is time to remove
-            for setting in settings.rem:
-                # setting object will only be matched and removed if it is the same reference to one
-                # previously added - will raise exception otherwise which should not happen if the
-                # settings dictionary and this method were setup correctly.
-                remove_idx = AnsiString._find_setting_reference(setting, self.current_settings)
-                if remove_idx >= 0:
-                    del self.current_settings[remove_idx]
-                elif AnsiString.WITH_ASSERTIONS:
-                    # This exception is really only useful in testing
-                    raise ValueError('could not remove setting: not in list')
-            # Apply settings that it is time to add
-            self.current_settings += settings.add
-            return (idx, settings, self.current_settings)
-
-    class CharIterator:
-        def __init__(self, s:'AnsiString'):
-            self.current_idx:int = -1
-            self.s:AnsiString = s
-
-        def __iter__(self):
-            return self
-
-        def __next__(self) -> 'AnsiString':
-            self.current_idx += 1
-            if self.current_idx >= len(self.s):
-                raise StopIteration
-            return self.s[self.current_idx]
-
     def _slice_val_to_idx(self, val:int, default:int) -> int:
         if val is None:
             return default
         elif val < 0:
             ret_val = len(self._s) + val
             if ret_val < 0:
                 ret_val = 0
@@ -1186,53 +1067,53 @@
             # Special case - string is now empty
             return new_s
 
         # String cannot be empty from this point on, so that will be assumed going forward
 
         previous_settings = None
         settings_initialized = False
-        for idx, settings, current_settings in __class__.SettingsIterator(self._fmts):
+        for idx, settings, current_settings in _AnsiSettingsIterator(self._fmts):
             if idx > len(self._s) or idx > en:
                 # Complete
                 break
             elif idx == en:
                 if settings.rem:
-                    new_s._fmts[idx - st] = __class__.SettingPoint(rem=list(settings.rem))
+                    new_s._fmts[idx - st] = _AnsiSettingPoint(rem=list(settings.rem))
                 # Complete
                 break
             elif idx == st:
                 if current_settings:
-                    new_s._fmts[0] = __class__.SettingPoint(add=list(current_settings))
+                    new_s._fmts[0] = _AnsiSettingPoint(add=list(current_settings))
                 settings_initialized = True
             elif idx > st:
                 if not settings_initialized and previous_settings:
-                    new_s._fmts[0] = __class__.SettingPoint(add=previous_settings)
+                    new_s._fmts[0] = _AnsiSettingPoint(add=previous_settings)
                 settings_initialized = True
-                new_s._fmts[idx - st] = __class__.SettingPoint(settings.add, settings.rem)
+                new_s._fmts[idx - st] = _AnsiSettingPoint(settings.add, settings.rem)
 
             # It's necessary to copy (i.e. call list()) since current_settings ref will change on next loop
             previous_settings = list(current_settings)
 
         if not settings_initialized and previous_settings:
             # Substring was between settings
-            new_s._fmts[0] = __class__.SettingPoint(add=previous_settings)
+            new_s._fmts[0] = _AnsiSettingPoint(add=previous_settings)
 
         # Because this class supports concatenation, it's necessary to remove all settings before ending
         if previous_settings:
             new_len = len(new_s._s)
             if new_len not in new_s._fmts:
-                new_s._fmts[new_len] = __class__.SettingPoint()
+                new_s._fmts[new_len] = _AnsiSettingPoint()
             settings_to_remove = [s for s in previous_settings if s not in new_s._fmts[new_len].rem]
             new_s._fmts[new_len].rem.extend(settings_to_remove)
 
         return new_s
 
     def __str__(self) -> str:
         '''
-        Returns an ANSI format string with only internal formatting set.
+        Returns a string with ANSI-formatting applied
         '''
         return self.__format__(None)
 
     def _apply_string_format(self, string_format:str):
         match = re.search(r'^(.?)<([0-9]*)$', string_format)
         if match:
             # Left justify
@@ -1296,42 +1177,43 @@
         else:
             # No changes - just copy the reference
             obj = self
 
         out_str = ''
         last_idx = 0
         clear_needed = False
-        for idx, settings, current_settings in __class__.SettingsIterator(obj._fmts):
+        for idx, settings, current_settings in _AnsiSettingsIterator(obj._fmts):
             if idx >= len(obj):
                 # Invalid
                 break
             # Catch up output to current index
             out_str += obj._s[last_idx:idx]
             last_idx = idx
 
             settings_to_apply = [str(s) for s in current_settings]
             if settings.rem and settings_to_apply:
                 # Settings were removed and there are settings to be applied -
                 # need to reset before applying current settings
-                settings_to_apply = [__class__.RESET] + settings_to_apply
+                settings_to_apply = [__class__.RESET_VALUE] + settings_to_apply
             # Apply these settings
             out_str += __class__.ANSI_ESCAPE_FORMAT.format(';'.join(settings_to_apply))
             # Save this flag in case this is the last loop
             clear_needed = bool(current_settings)
 
         # Final catch up
         out_str += obj._s[last_idx:]
         if clear_needed:
             # Clear settings
             out_str += __class__.ANSI_ESCAPE_CLEAR
 
         return out_str
 
-    def __iter__(self):
-        return iter(__class__.CharIterator(self))
+    def __iter__(self) -> 'AnsiString':
+        ''' Iterates over each character '''
+        return iter(_AnsiCharIterator(self))
 
     def capitalize(self, inplace:bool=False) -> 'AnsiString':
         if inplace:
             obj = self
         else:
             obj = self.copy()
         obj._s = obj._s.capitalize()
@@ -1430,15 +1312,15 @@
         return self._s.isalnum()
 
     def isalpha(self) -> bool:
         return self._s.isalpha()
 
     def isascii(self) -> bool:
         '''
-        This is only available for Python >=3.7
+        This is only available for Python >=3.7; exception will be raised in Python 3.6
         '''
         return self._s.isascii()
 
     def isdecimal(self) -> bool:
         return self._s.isdecimal()
 
     def isdigit(self) -> bool:
@@ -1467,22 +1349,23 @@
 
     def __add__(self, value:Union[str,'AnsiString']) -> 'AnsiString':
         cpy = self.copy()
         cpy += value
         return cpy
 
     def __iadd__(self, value:Union[str,'AnsiString']) -> 'AnsiString':
+        ''' Appends a string or AnsiString to this AnsiString '''
         if isinstance(value, str):
             self._s += value
         elif isinstance(value, AnsiString):
             shift = len(self._s)
             self._s += value._s
             find_settings = []
             replace_settings = []
-            for key, settings in value._fmts.items():
+            for key, settings in sorted(value._fmts.items()):
                 key += shift
                 if key in self._fmts:
                     if (
                         key == shift
                         and settings.add
                         and self._fmts[key].rem[:len(settings.add)] == settings.add
                     ):
@@ -1497,29 +1380,30 @@
                             del self._fmts[key]
                             continue
 
                     self._fmts[key].add.extend(settings.add)
                     self._fmts[key].rem.extend(settings.rem)
 
                 else:
-                    self._fmts[key] = __class__.SettingPoint(list(settings.add), list(settings.rem))
+                    self._fmts[key] = _AnsiSettingPoint(list(settings.add), list(settings.rem))
 
                     finds = __class__._find_settings_references(find_settings, settings.rem)
                     if finds:
                         for find_idx, add_idx in reversed(finds):
                             self._fmts[key].rem[add_idx] = replace_settings[find_idx]
                             # Note: find_idx will always be sorted in ascending order and this is iterating in reverse
                             del find_settings[find_idx]
                             del replace_settings[find_idx]
 
         else:
             raise TypeError(f'value is invalid type: {type(value)}')
         return self
 
     def __eq__(self, value:'AnsiString') -> bool:
+        ''' == operator - returns True if exactly equal '''
         if not isinstance(value, AnsiString):
             return False
         return self._s == value._s and self._fmts == value._fmts
 
     def __contains__(self, value:Union[str,'AnsiString',Any]) -> bool:
         if isinstance(value, str):
             return value in self._s
@@ -1528,14 +1412,15 @@
         return False
 
     def __len__(self) -> int:
         return len(self._s)
 
     @staticmethod
     def join(*args:Union[str,'AnsiString']) -> 'AnsiString':
+        ''' Joins strings and AnsiStrings into a single AnsiString object '''
         if not args:
             return AnsiString()
         args = list(args)
         first_arg = args[0]
         if isinstance(first_arg, str):
             joint = AnsiString(first_arg)
         elif isinstance(first_arg, AnsiString):
@@ -1671,18 +1556,18 @@
         if idx >= 0:
             sep_len = len(sep)
             idx_end = idx + sep_len
             return (self[0:idx], self[idx:idx_end], self[idx_end:])
         else:
             return (self.copy(), AnsiString(), AnsiString())
 
-    def _settings_at(self, idx:int) -> List[Setting]:
+    def _settings_at(self, idx:int) -> List[AnsiSetting]:
         if idx >= 0 and idx < len(self._s):
             previous_settings = []
-            for sidx, _, current_settings in __class__.SettingsIterator(self._fmts):
+            for sidx, _, current_settings in _AnsiSettingsIterator(self._fmts):
                 if sidx > idx:
                     break
                 previous_settings = list(current_settings)
             return previous_settings
         else:
             return []
 
@@ -1797,7 +1682,180 @@
 
         obj._s = obj._s.title()
 
         return obj
 
     def zfill(self, width:int, inplace:bool=False) -> 'AnsiString':
         return self.rjust(width, "0", inplace)
+
+
+class _AnsiSettingPoint:
+    '''
+    This class is used internally to keep track of ANSI settings at a specific string index
+    '''
+
+    def __init__(
+        self,
+        add:Union[List['AnsiSetting'],None]=None,
+        rem:Union[List['AnsiSetting'],None]=None
+    ):
+        self.add:List[AnsiSetting] = add or []
+        self.rem:List[AnsiSetting] = rem or []
+
+    def __eq__(self, value) -> bool:
+        if isinstance(value, _AnsiSettingPoint):
+            return value.add == self.add and value.rem == self.rem
+        return False
+
+    def __bool__(self) -> bool:
+        return bool(self.add) or bool(self.rem)
+
+    @staticmethod
+    def _parse_rgb_string(s:str) -> str:
+        component_dict = {
+            'ul_': ColorComponentType.UNDERLINE,
+            'bg_': ColorComponentType.BACKGROUND,
+            'fg_': ColorComponentType.FOREGROUND
+        }
+
+        # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 3 distinct values as decimal or hex
+        match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\([\[\()]?\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*,\s*(0x)?([0-9a-fA-F]+)\s*[\)\]]?\)$', s)
+        if match:
+            try:
+                r = int(match.group(3), 16 if match.group(2) else 10)
+                g = int(match.group(5), 16 if match.group(4) else 10)
+                b = int(match.group(7), 16 if match.group(6) else 10)
+            except ValueError:
+                raise ValueError('Invalid rgb value(s)')
+            # Get RGB format and remove the leading '['
+            return str(AnsiFormat.rgb(r, g, b, component_dict.get(match.group(1), ColorComponentType.FOREGROUND)))
+
+        # rgb(), fg_rgb(), bg_rgb(), or ul_rgb() with 1 value as decimal or hex
+        match = re.search(r'^((?:fg_)?|(?:bg_)|(?:ul_))rgb\([\[\()]?\s*(0x)?([0-9a-fA-F]+)\s*[\)\]]?\)$', s)
+        if match:
+            try:
+                rgb = int(match.group(3), 16 if match.group(2) else 10)
+            except ValueError:
+                raise ValueError('Invalid rgb value')
+            # Get RGB format and remove the leading '['
+            return str(AnsiFormat.rgb(rgb, component=component_dict.get(match.group(1), ColorComponentType.FOREGROUND)))
+        return None
+
+    @staticmethod
+    def _scrub_ansi_format_string(ansi_format:str) -> List[str]:
+        if ansi_format.startswith("["):
+            # Use the rest of the string as-is for settings
+            return [ansi_format[1:]]
+        else:
+            # The format string contains names within AnsiFormat or integers, separated by semicolon
+            formats = ansi_format.split(';')
+            format_settings_strs = []
+            for format in formats:
+                ansi_fmt_enum = None
+                try:
+                    ansi_fmt_enum = AnsiFormat[format.upper()]
+                except KeyError:
+                    pass
+                else:
+                    format_settings_strs.append(ansi_fmt_enum.value)
+
+                if ansi_fmt_enum is None:
+                    rgb_format = __class__._parse_rgb_string(format)
+                    if not rgb_format:
+                        try:
+                            int_value = int(format)
+                            # 0 should never be used because it will mess with internal assumptions
+                            # Negative values are invalid
+                            if int_value < 0:
+                                raise ValueError(f'Invalid value [{int_value}]; must be greater than or equal to 0')
+                        except ValueError:
+                            raise ValueError(
+                                'AnsiString.__format__ failed to parse format ({}); invalid name: {}'
+                                .format(ansi_format, format)
+                            )
+                        else:
+                            # Value is an integer - use the format verbatim
+                            format_settings_strs.append(format)
+                    else:
+                        format_settings_strs.append(rgb_format)
+            return format_settings_strs
+
+    def insert_setting(self, apply:bool, setting:'AnsiSetting', topmost:bool=True):
+        lst = self.add if apply else self.rem
+        if topmost:
+            lst.append(setting)
+        else:
+            lst.insert(0, setting)
+
+    def insert_settings(
+        self,
+        apply:bool,
+        settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat, List['AnsiSetting'], 'AnsiSetting'],
+        topmost:bool=True
+    ) -> List['AnsiSetting']:
+        if not isinstance(settings, list) and not isinstance(settings, tuple):
+            settings = [settings]
+
+        settings_to_insert = []
+        for setting in settings:
+            if isinstance(setting, AnsiSetting):
+                settings_to_insert.append(setting)
+            elif isinstance(setting, str) or isinstance(setting, int):
+                settings_to_insert.extend([AnsiSetting(s) for s in __class__._scrub_ansi_format_string(str(setting))])
+            elif hasattr(setting, "value") and isinstance(setting.value, str):
+                settings_to_insert.append(AnsiSetting(setting.value))
+
+        lst = self.add if apply else self.rem
+        if topmost:
+            lst.extend(settings_to_insert)
+        else:
+            lst[:0] = settings_to_insert
+
+        return settings_to_insert
+
+class _AnsiSettingsIterator:
+    '''
+    Internally-used class which helps iterate over settings
+    '''
+    def __init__(self, settings_dict:Dict[int,'_AnsiSettingPoint']):
+        self.settings_dict:Dict[int,_AnsiSettingPoint] = settings_dict
+        self.current_settings:List[AnsiSetting] = []
+        self.dict_iter = iter(sorted(self.settings_dict))
+
+    def __iter__(self):
+        return self
+
+    def __next__(self) -> Tuple[int,'_AnsiSettingPoint',List['AnsiSetting']]:
+        # Will raise StopIteration when complete
+        idx = next(self.dict_iter)
+        settings = self.settings_dict[idx]
+        # Remove settings that it is time to remove
+        for setting in settings.rem:
+            # setting object will only be matched and removed if it is the same reference to one
+            # previously added - will raise exception otherwise which should not happen if the
+            # settings dictionary and this method were setup correctly.
+            remove_idx = AnsiString._find_setting_reference(setting, self.current_settings)
+            if remove_idx >= 0:
+                del self.current_settings[remove_idx]
+            elif AnsiString.WITH_ASSERTIONS:
+                # This exception is really only useful in testing
+                raise ValueError('could not remove setting: not in list')
+        # Apply settings that it is time to add
+        self.current_settings += settings.add
+        return (idx, settings, self.current_settings)
+
+class _AnsiCharIterator:
+    '''
+    Internally-used class which helps iterate over characters
+    '''
+    def __init__(self, s:'AnsiString'):
+        self.current_idx:int = -1
+        self.s:AnsiString = s
+
+    def __iter__(self):
+        return self
+
+    def __next__(self) -> 'AnsiString':
+        self.current_idx += 1
+        if self.current_idx >= len(self.s):
+            raise StopIteration
+        return self.s[self.current_idx]
```

### Comparing `ansi-string-1.0.2/src/ansi_string.egg-info/PKG-INFO` & `ansi-string-1.0.3/src/ansi_string.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansi-string
-Version: 1.0.2
+Version: 1.0.3
 Summary: ANSI String Formatter in Python for CLI Color and Style Formatting
 Home-page: https://github.com/Tails86/ansi-string
 Author: James Smith
 Author-email: jmsmith86@gmail.com
 Project-URL: Documentation, https://github.com/Tails86/ansi-string
 Project-URL: Bug Reports, https://github.com/Tails86/ansi-string/issues
 Project-URL: Source Code, https://github.com/Tails86/ansi-string
@@ -31,30 +31,30 @@
 ANSI String Formatter in Python for CLI Color and Style Formatting
 
 ## Introduction
 
 This code was originally written for [greplica](https://pypi.org/project/greplica/), but I felt it deserved its own, separate library.
 
 The main goals for this project are:
-- To provide a simple way to construct an object with ANSI formatting without requiring the developer to know how ANSI formatting works
+- To provide a simple way to construct a string-like object with embedded ANSI formatting without requiring the developer to know how ANSI formatting works
 - Provide a way to further format the object using format string
 - Allow for concatenation of the object
 
 ## Contribution
 
 Feel free to open a bug report or make a merge request on [github](https://github.com/Tails86/ansi-string/issues).
 
 ## Installation
 This project is uploaded to PyPI at https://pypi.org/project/ansi-string
 
 To install, ensure you are connected to the internet and execute: `python3 -m pip install ansi-string --upgrade`
 
 ## Examples
 
-![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/0e2c943f25ccc219256204511fd308652a8075c0/docs/examples.jpg)
+![Examples](https://raw.githubusercontent.com/Tails86/ansi-string/36530493c87e282914d23d551ce427203fcd2719/docs/examples.jpg)
 
 Refer to the [test file](https://github.com/Tails86/ansi-string/blob/main/tests/test_ansi_string.py) for more examples on how to use the AnsiString class.
 
 ## Usage
 
 To begin, import AnsiString from the ansi_string module.
 
@@ -82,25 +82,30 @@
 The AnsiString class contains the following `__init__` method.
 
 ```py
 class AnsiString:
     def __init__(self, s:str='', *setting_or_settings:Union[List[str], str, List[int], int, List[AnsiFormat], AnsiFormat]): ...
 ```
 
-The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting directives that can be applied to the entire string. These arguments can be in the form of any of the following:
-- A string color name for a formatting directive (i.e. any name of the AnsiFormat enum in lower or upper case)
-- An AnsiFormat directive (ex: `AnsiFormat.BOLD`)
+The first argument, `s`, is a string to be formatted. The next 0 to N arguments are formatting setting directives that can be applied to the entire string. These arguments can be in the form of any of the following.
+- An AnsiFormat enum (ex: `AnsiFormat.BOLD`)
+- A string color or formatting name (i.e. any name of the AnsiFormat enum in lower or upper case)
+- The result of calling `AnsiFormat.rgb()`, `AnsiFormat.fg_rgb()`, `AnsiFormat.bg_rgb()`, or `AnsiFormat.ul_rgb()`
 - An `rgb(...)` function directive as a string (ex: `"rgb(255, 255, 255)"`)
     - `rgb(...)` or `fg_rgb(...)` to adjust text color
     - `bg_rgb(...)` to adjust background color
     - `ul_rgb(...)` to enable underline and set the underline color
     - Value given may be either a 24-bit integer or 3 x 8-bit integers, separated by commas
     - Each given value within the parenthesis is treated as hexadecimal if the value starts with "0x", otherwise it is treated as a decimal value
+
+A formatting setting may also be any of the following, but it's not advised to specify settings these ways unless there is a specific reason to do so.
+- An AnsiSetting object
 - A string containing known ANSI directives (ex: `"01;31"` for BOLD and FG_RED)
-    - The string will normally be parsed into their individual values and verified unless the character "[" is the first character of the string (ex: `"[01;31"`)
+    - The string will normally be parsed into separate settings unless the character "[" is the first character of the string (ex: `"[38;5;214"`)
+    - Never specify the reset directive (0) because this is implicitly handled internally
 - A single ANSI directive as an integer
 
 Examples:
 ```py
 # Set foreground to light_sea_green using string directive
 # Set background to chocolate using AnsiFormat directive
 # Underline in gray using ul_rgb() directive
```

