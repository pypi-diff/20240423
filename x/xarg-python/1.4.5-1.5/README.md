# Comparing `tmp/xarg-python-1.4.5.tar.gz` & `tmp/xarg-python-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarg-python-1.4.5.tar", last modified: Wed Apr 10 05:09:47 2024, max compression
+gzip compressed data, was "xarg-python-1.5.tar", last modified: Tue Apr 23 15:22:51 2024, max compression
```

## Comparing `xarg-python-1.4.5.tar` & `xarg-python-1.5.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 05:09:47.720985 xarg-python-1.4.5/
--rw-r--r--   0 root         (0) root         (0)     1114 2023-12-26 08:19:24.000000 xarg-python-1.4.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1424 2024-04-10 05:09:47.720985 xarg-python-1.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      656 2023-12-26 08:19:24.000000 xarg-python-1.4.5/README.md
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-10 05:09:47.720985 xarg-python-1.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      779 2024-03-28 12:58:33.000000 xarg-python-1.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 05:09:47.720985 xarg-python-1.4.5/xarg/
--rw-r--r--   0 root         (0) root         (0)      490 2024-04-07 12:41:34.000000 xarg-python-1.4.5/xarg/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22137 2024-04-09 12:36:04.000000 xarg-python-1.4.5/xarg/actuator.py
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-10 05:09:21.000000 xarg-python-1.4.5/xarg/attribute.py
--rw-r--r--   0 root         (0) root         (0)     9216 2024-04-07 12:41:34.000000 xarg-python-1.4.5/xarg/colorful.py
--rw-r--r--   0 root         (0) root         (0)     8184 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/complete.py
--rw-r--r--   0 root         (0) root         (0)     4359 2024-04-09 12:43:23.000000 xarg-python-1.4.5/xarg/logger.py
--rw-r--r--   0 root         (0) root         (0)     8479 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/parser.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/safefile.py
--rw-r--r--   0 root         (0) root         (0)     8482 2023-12-28 08:08:34.000000 xarg-python-1.4.5/xarg/scanner.py
--rw-r--r--   0 root         (0) root         (0)     1236 2024-04-01 02:36:04.000000 xarg-python-1.4.5/xarg/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 05:09:47.720985 xarg-python-1.4.5/xarg_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1424 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 05:09:47.000000 xarg-python-1.4.5/xarg_python.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:22:51.107725 xarg-python-1.5/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-08-28 15:46:08.000000 xarg-python-1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-04-23 15:22:51.107725 xarg-python-1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      656 2023-11-23 15:08:18.000000 xarg-python-1.5/README.md
+-rw-r--r--   0 root         (0) root         (0)      610 2024-04-23 15:22:51.107725 xarg-python-1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      779 2024-03-31 14:51:50.000000 xarg-python-1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:22:51.107725 xarg-python-1.5/xarg/
+-rw-r--r--   0 root         (0) root         (0)      649 2024-04-11 15:57:13.000000 xarg-python-1.5/xarg/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22587 2024-04-23 15:09:08.000000 xarg-python-1.5/xarg/actuator.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-04-23 15:22:42.000000 xarg-python-1.5/xarg/attribute.py
+-rw-r--r--   0 root         (0) root         (0)     8932 2024-04-23 15:09:08.000000 xarg-python-1.5/xarg/colorful.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2024-04-23 15:09:08.000000 xarg-python-1.5/xarg/complete.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-04-23 15:09:08.000000 xarg-python-1.5/xarg/logger.py
+-rw-r--r--   0 root         (0) root         (0)     8692 2024-04-23 15:09:08.000000 xarg-python-1.5/xarg/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-03-31 14:25:54.000000 xarg-python-1.5/xarg/safefile.py
+-rw-r--r--   0 root         (0) root         (0)     8554 2024-04-23 15:09:08.000000 xarg-python-1.5/xarg/scanner.py
+-rw-r--r--   0 root         (0) root         (0)    11227 2024-04-23 15:09:08.000000 xarg-python-1.5/xarg/sheet.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2024-03-31 15:00:43.000000 xarg-python-1.5/xarg/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 15:22:51.107725 xarg-python-1.5/xarg_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-04-23 15:22:51.000000 xarg-python-1.5/xarg_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2024-04-23 15:22:51.000000 xarg-python-1.5/xarg_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 15:22:51.000000 xarg-python-1.5/xarg_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-23 15:22:51.000000 xarg-python-1.5/xarg_python.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 15:22:51.000000 xarg-python-1.5/xarg_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-23 15:22:51.000000 xarg-python-1.5/xarg_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 15:22:51.000000 xarg-python-1.5/xarg_python.egg-info/zip-safe
```

### Comparing `xarg-python-1.4.5/LICENSE` & `xarg-python-1.5/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Mingzhe Zou <zoumingzhe@outlook.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Mingzhe Zou <zoumingzhe@outlook.com>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `xarg-python-1.4.5/README.md` & `xarg-python-1.5/README.md`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.5/setup.cfg` & `xarg-python-1.5/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 [options]
 zip_safe = True
 include_package_data = True
 install_requires = 
 	argcomplete >= 3.2.1
 	colorama
 	colorlog
+	openpyxl
 	tabulate
+	wcwidth
+	xlrd
+	xlwt
 
 [options.entry_points]
 console_scripts = 
 	xargcomplete = xarg.complete:main
 
 [egg_info]
 tag_build =
```

### Comparing `xarg-python-1.4.5/setup.py` & `xarg-python-1.5/setup.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.5/xarg/actuator.py` & `xarg-python-1.5/xarg/actuator.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     For example:
 
     >>> from xarg import add_command\n
     >>> from xarg import argp\n
 
     >>> @add_command("example")\n
     >>> def cmd(_arg: argp):\n
-    >>>     argp.add_opt_on("-t", "--test")\n
+    >>>     _arg.add_opt_on("-t", "--test")\n
     '''
 
     def __init__(self, name: str, **kwargs):
         '''
         @param name: Node name
         @type name: str
 
@@ -56,21 +56,24 @@
             kwargs["help"] = kwargs["description"]
         self.__name: str = name
         self.__prev: add_command = self
         self.__cmds: commands = commands()
         self.__options: Dict[str, Any] = kwargs
         self.__bind: Optional[run_command] = None
         self.__subs: Optional[Tuple[add_command, ...]] = None
+        self.__func: Optional[Callable[[argp], None]] = None
 
     def __call__(self, cmd_func: Callable[[argp], None]):
-        self.__func: Callable[[argp], None] = cmd_func
+        self.__func = cmd_func
         return self
 
     @property
     def func(self) -> Callable[[argp], None]:
+        if self.__func is None:
+            raise ValueError("No function")
         return self.__func
 
     @property
     def name(self) -> str:
         return self.__name
 
     @property
@@ -162,21 +165,24 @@
         for sub in sub_cmds:
             sub.prev = cmd_bind
         commands().root = cmd_bind.root
         self.__skip: bool = skip
         self.__bind: add_command = cmd_bind
         self.__prep: Optional["pre_command"] = None
         self.__done: Optional["end_command"] = None
+        self.__func: Optional[Callable[["commands"], int]] = None
 
     def __call__(self, run_func: Callable[["commands"], int]):
-        self.__func: Callable[["commands"], int] = run_func
+        self.__func = run_func
         return self
 
     @property
     def func(self) -> Callable[["commands"], int]:
+        if self.__func is None:
+            raise ValueError("No function")
         return self.__func
 
     @property
     def bind(self) -> add_command:
         return self.__bind
 
     @property
@@ -224,21 +230,24 @@
         '''
         @param cmd_bind: Bind to a root command node
         @type name: add_command
         '''
         assert isinstance(run_bind, run_command)
         run_bind.prep = self
         self.__main: run_command = run_bind
+        self.__func: Optional[Callable[["commands"], int]] = None
 
     def __call__(self, run_func: Callable[["commands"], int]):
-        self.__func: Callable[["commands"], int] = run_func
+        self.__func = run_func
         return self
 
     @property
     def func(self) -> Callable[["commands"], int]:
+        if self.__func is None:
+            raise ValueError("No function")
         return self.__func
 
     @property
     def main(self) -> run_command:
         return self.__main
 
 
@@ -264,21 +273,24 @@
         '''
         @param cmd_bind: Bind to a root command node
         @type name: add_command
         '''
         assert isinstance(run_bind, run_command)
         run_bind.done = self
         self.__main: run_command = run_bind
+        self.__func: Optional[Callable[["commands"], int]] = None
 
     def __call__(self, run_func: Callable[["commands"], int]):
-        self.__func: Callable[["commands"], int] = run_func
+        self.__func = run_func
         return self
 
     @property
     def func(self) -> Callable[["commands"], int]:
+        if self.__func is None:
+            raise ValueError("No function")
         return self.__func
 
     @property
     def main(self) -> run_command:
         return self.__main
 
 
@@ -298,15 +310,15 @@
     >>> from xarg import commands\n
     >>> from xarg import end_command\n
     >>> from xarg import pre_command\n
     >>> from xarg import run_command\n
 
     >>> @add_command("example")\n
     >>> def cmd(_arg: argp):\n
-    >>>     argp.add_opt_on("-t", "--test")\n
+    >>>     _arg.add_opt_on("-t", "--test")\n
 
     >>> @run_command(cmd, cmd_get, cmd_set)\n
     >>> def run(cmds: commands) -> int:\n
     >>>     return 0\n
 
     >>> @pre_command(run)\n
     >>> def pre(cmds: commands) -> int:\n
@@ -396,36 +408,36 @@
 
     def stderr(self, context: Any):
         '''Output string to sys.stderr.
         '''
         sys.stderr.write(f"{context}\n")
         sys.stderr.flush()
 
-    def __add_optional_version(self, argp: argp):
+    def __add_optional_version(self, _arg: argp):
         version = self.version
         if not isinstance(version, str):
             return
 
-        options = argp.filter_optional_name("-v", "--version")
+        options = _arg.filter_optional_name("-v", "--version")
         if len(options) > 0:
-            argp.add_argument(*options, action="version",
+            _arg.add_argument(*options, action="version",
                               version=f"%(prog)s {version.strip()}")
 
-    def __add_inner_parser_tail(self, argp: argp):
+    def __add_inner_parser_tail(self, _arg: argp):
 
         def filter_optional_name(*name: str) -> Optional[str]:
-            options = argp.filter_optional_name(*name)
+            options = _arg.filter_optional_name(*name)
             if len(options) > 0:
                 for i in name:
                     if i in options:
                         return i
             return None
 
         def add_optional_level():
-            group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
+            group = _arg.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group_level = group.add_mutually_exclusive_group()
 
             option_level = filter_optional_name("--level", "--log-level")
             if isinstance(option_level, str):
                 group_level.add_argument(
                     option_level,
                     type=str,
@@ -454,15 +466,15 @@
                                          help=f"Logger level set to {level}.")
 
         def add_optional_stream():
             option = filter_optional_name("--log", "--log-file")
             if not isinstance(option, str):
                 return
 
-            group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
+            group = _arg.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group.add_argument(option,
                                type=str,
                                nargs=1,
                                default=[],
                                metavar="FILE",
                                action="extend",
                                dest="_log_files_",
@@ -474,26 +486,26 @@
                 return
 
             DEFAULT_LOG_FMT = "%(log_color)s%(asctime)s"\
                 " %(process)d %(threadName)s %(levelname)s"\
                 " %(funcName)s %(filename)s:%(lineno)s"\
                 " %(message)s"
 
-            group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
+            group = _arg.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group.add_argument(option,
                                type=str,
                                nargs="?",
                                const=DEFAULT_LOG_FMT,
                                default=self.DEFAULT_LOG_FORMAT,
                                metavar="STRING",
                                dest="_log_format_",
                                help="Logger output format.")
 
         def add_optional_console():
-            group = argp.argument_group(self.LOGGER_ARGUMENT_GROUP)
+            group = _arg.argument_group(self.LOGGER_ARGUMENT_GROUP)
             group_std = group.add_mutually_exclusive_group()
 
             option = filter_optional_name("--stdout", "--log-stdout")
             if isinstance(option, str):
                 group_std.add_argument(option,
                                        const=sys.stdout,
                                        action="store_const",
@@ -564,15 +576,15 @@
               argv: Optional[Sequence[str]] = None, **kwargs) -> Namespace:
         '''Parse the command line.
         '''
         if root is None:
             root = self.root
         assert isinstance(root, add_command)
 
-        _map: Dict[add_command, argp] = dict()
+        _map: Dict[add_command, argp] = {}
         _arg = argp(argv=argv, **kwargs)
         self.__prog = _arg.prog
         self.__add_optional_version(_arg)
         # To support preparse_from_sys_argv(), all subparsers must be added
         # first. Otherwise, an error will occur during the help action.
         self.__add_parser(_map, _arg, root, **kwargs)
         self.__add_option(_map)
@@ -664,22 +676,22 @@
 
         if not isinstance(root, add_command):
             self.logger.debug("cannot find root")
             return ENOENT
 
         kwargs.pop("prog", None)  # Please do not specify prog
         args = self.parse(root, argv, **kwargs)
-        self.logger.debug(f"{args}")
+        self.logger.debug("%s", args)
 
         try:
             version = self.version
             if isinstance(version, str):
                 # Output version for the debug level. Internal log
                 # items are debug level only, except for errors.
-                self.logger.debug(f"version: {version}")
+                self.logger.debug("version: %s", version)
 
             ret = self.__pre(args, root)
             if ret != 0 and ret is not None:
                 return ret
             return self.__run(args, root)
         except KeyboardInterrupt:
             return EINTR
```

### Comparing `xarg-python-1.4.5/xarg/colorful.py` & `xarg-python-1.5/xarg/colorful.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 class color(str):
     '''Colorful terminal text
 
     Reference: https://en.wikipedia.org/wiki/ANSI_escape_code
     '''
 
-    def __init__(self, object: object):
+    def __init__(self, obj: object):
         self.__background: Optional[str] = None
         self.__foreground: Optional[str] = None
         self.__style: Set[str] = set()
         super().__init__()
 
     def __str__(self) -> str:
         message: str = super().__str__()
@@ -95,209 +95,209 @@
     def style(self, value: Set[StyleType]):
         assert isinstance(value, set), f"Unexpected type: {type(value)}"
         _value: Set[str] = {code_to_chars(v) if isinstance(v, int) else v
                             for v in value}
         self.__style = _value
 
     def add_style(self, value: StyleType) -> "color":
-        assert isinstance(value, StyleType), f"Unexpected type: {type(value)}"
+        assert isinstance(value, (str, int)), f"Unexpected type: {type(value)}"
         _value: str = code_to_chars(value) if isinstance(value, int) else value
         self.__style.add(_value)
         return self
 
     @classmethod
-    def new_background(cls, object: object, value: str) -> "color":
-        colour: color = color(object)
+    def new_background(cls, obj: object, value: str) -> "color":
+        colour: color = color(obj)
         colour.background = value
         return colour
 
     @classmethod
-    def new_foreground(cls, object: object, value: str) -> "color":
-        colour: color = color(object)
+    def new_foreground(cls, obj: object, value: str) -> "color":
+        colour: color = color(obj)
         colour.foreground = value
         return colour
 
     @classmethod
-    def new_style(cls, object: object, value: Set[StyleType]) -> "color":
-        colour: color = color(object)
+    def new_style(cls, obj: object, value: Set[StyleType]) -> "color":
+        colour: color = color(obj)
         colour.style = value
         return colour
 
     @classmethod
     def reset(cls) -> str:
         return Style.RESET_ALL
 
     @classmethod
-    def bold(cls, object: object) -> "color":
-        return color.new_style(object, {Style.BRIGHT})
+    def bold(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.BRIGHT})
 
     @classmethod
-    def dim(cls, object: object) -> "color":
-        return color.new_style(object, {Style.DIM})
+    def dim(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.DIM})
 
     @classmethod
-    def italic(cls, object: object) -> "color":
-        return color.new_style(object, {Style.ITALIC})
+    def italic(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.ITALIC})
 
     @classmethod
-    def underline(cls, object: object) -> "color":
-        return color.new_style(object, {Style.UNDERLINE})
+    def underline(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.UNDERLINE})
 
     @classmethod
-    def slow_blink(cls, object: object) -> "color":
-        return color.new_style(object, {Style.SLOWBLINK})
+    def slow_blink(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.SLOWBLINK})
 
     @classmethod
-    def rapid_blink(cls, object: object) -> "color":
-        return color.new_style(object, {Style.RAPIDBLINK})
+    def rapid_blink(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.RAPIDBLINK})
 
     @classmethod
-    def invert(cls, object: object) -> "color":
-        return color.new_style(object, {Style.INVERT})
+    def invert(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.INVERT})
 
     @classmethod
-    def hide(cls, object: object) -> "color":
-        return color.new_style(object, {Style.HIDE})
+    def hide(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.HIDE})
 
     @classmethod
-    def strikethrough(cls, object: object) -> "color":
-        return color.new_style(object, {Style.STRIKETHROUGH})
+    def strikethrough(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.STRIKETHROUGH})
 
     @classmethod
-    def doubly_underlined(cls, object: object) -> "color":
-        return color.new_style(object, {Style.DOUBLYUNDERLINED})
+    def doubly_underlined(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.DOUBLYUNDERLINED})
 
     @classmethod
-    def normal(cls, object: object) -> "color":
-        return color.new_style(object, {Style.NORMAL})
+    def normal(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.NORMAL})
 
     @classmethod
-    def reveal(cls, object: object) -> "color":
-        return color.new_style(object, {Style.REVEAL})
+    def reveal(cls, obj: object) -> "color":
+        return color.new_style(obj, {Style.REVEAL})
 
     @classmethod
-    def black(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.BLACK)
+    def black(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.BLACK)
 
     @classmethod
-    def red(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.RED)
+    def red(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.RED)
 
     @classmethod
-    def green(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.GREEN)
+    def green(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.GREEN)
 
     @classmethod
-    def yellow(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.YELLOW)
+    def yellow(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.YELLOW)
 
     @classmethod
-    def blue(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.BLUE)
+    def blue(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.BLUE)
 
     @classmethod
-    def magenta(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.MAGENTA)
+    def magenta(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.MAGENTA)
 
     @classmethod
-    def cyan(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.CYAN)
+    def cyan(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.CYAN)
 
     @classmethod
-    def white(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.WHITE)
+    def white(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.WHITE)
 
     @classmethod
-    def lightblack(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTBLACK_EX)
+    def lightblack(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTBLACK_EX)
 
     @classmethod
-    def lightred(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTRED_EX)
+    def lightred(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTRED_EX)
 
     @classmethod
-    def lightgreen(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTGREEN_EX)
+    def lightgreen(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTGREEN_EX)
 
     @classmethod
-    def lightyellow(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTYELLOW_EX)
+    def lightyellow(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTYELLOW_EX)
 
     @classmethod
-    def lightblue(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTBLUE_EX)
+    def lightblue(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTBLUE_EX)
 
     @classmethod
-    def lightmagenta(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTMAGENTA_EX)
+    def lightmagenta(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTMAGENTA_EX)
 
     @classmethod
-    def lightcyan(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTCYAN_EX)
+    def lightcyan(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTCYAN_EX)
 
     @classmethod
-    def lightwhite(cls, object: object) -> "color":
-        return color.new_foreground(object, Fore.LIGHTWHITE_EX)
+    def lightwhite(cls, obj: object) -> "color":
+        return color.new_foreground(obj, Fore.LIGHTWHITE_EX)
 
     @classmethod
-    def black_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.BLACK)
+    def black_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.BLACK)
 
     @classmethod
-    def red_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.RED)
+    def red_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.RED)
 
     @classmethod
-    def green_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.GREEN)
+    def green_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.GREEN)
 
     @classmethod
-    def yellow_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.YELLOW)
+    def yellow_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.YELLOW)
 
     @classmethod
-    def blue_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.BLUE)
+    def blue_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.BLUE)
 
     @classmethod
-    def magenta_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.MAGENTA)
+    def magenta_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.MAGENTA)
 
     @classmethod
-    def cyan_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.CYAN)
+    def cyan_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.CYAN)
 
     @classmethod
-    def white_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.WHITE)
+    def white_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.WHITE)
 
     @classmethod
-    def lightblack_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTBLACK_EX)
+    def lightblack_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTBLACK_EX)
 
     @classmethod
-    def lightred_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTRED_EX)
+    def lightred_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTRED_EX)
 
     @classmethod
-    def lightgreen_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTGREEN_EX)
+    def lightgreen_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTGREEN_EX)
 
     @classmethod
-    def lightyellow_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTYELLOW_EX)
+    def lightyellow_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTYELLOW_EX)
 
     @classmethod
-    def lightblue_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTBLUE_EX)
+    def lightblue_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTBLUE_EX)
 
     @classmethod
-    def lightmagenta_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTMAGENTA_EX)
+    def lightmagenta_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTMAGENTA_EX)
 
     @classmethod
-    def lightcyan_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTCYAN_EX)
+    def lightcyan_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTCYAN_EX)
 
     @classmethod
-    def lightwhite_back(cls, object: object) -> "color":
-        return color.new_background(object, Back.LIGHTWHITE_EX)
+    def lightwhite_back(cls, obj: object) -> "color":
+        return color.new_background(obj, Back.LIGHTWHITE_EX)
```

### Comparing `xarg-python-1.4.5/xarg/complete.py` & `xarg-python-1.5/xarg/complete.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,18 +42,18 @@
         bash_completion_code = """
 for bcfile in ~/.bash_completion.d/* ; do
   source ${bcfile}
 done
 """
         if not os.path.exists(bash_completion_hook):
             os.makedirs(bash_completion_hook)
-        with open(bash_completion_path, "r") as fh:
+        with open(bash_completion_path, "r", encoding="utf-8") as fh:
             if bash_completion_code in fh.read():
                 return
-        with open(bash_completion_path, "a") as fh:
+        with open(bash_completion_path, "a", encoding="utf-8") as fh:
             fh.write(f"\n{bash_completion_code}\n")
 
     update_code()
     update_bash(__prog_complete__)
 
 
 def update_bash(cmd: str) -> int:
@@ -87,30 +87,30 @@
 
 
 @singleton
 class collections:
 
     def __init__(self):
         self.__cmds: Set[str] = set()
-        for _pkg in {"argcomplete", __project__}:
-            for _req in {i for i in self.get_package_info(_pkg).required_by}:
+        for _pkg in tuple({"argcomplete", __project__}):
+            for _req in set(self.get_package_info(_pkg).required_by):
                 config = ConfigParser()
                 package_info = self.get_package_info(_req)
                 config.read_string(os.linesep.join(package_info.entry_points))
                 if config.has_section("console_scripts"):
                     for _cmd in config["console_scripts"]:
                         self.__cmds.add(_cmd)
 
     @property
     def cmds(self) -> Iterable[str]:
         return iter(self.__cmds)
 
     @classmethod
     def get_package_info(cls, package_name: str) -> _PackageInfo:
-        return [i for i in search_packages_info([package_name])][0]
+        return list(search_packages_info([package_name]))[0]
 
 
 @add_command("enable", help="Enable completion.")
 def add_cmd_enable(_arg: argp):
     pass
```

### Comparing `xarg-python-1.4.5/xarg/logger.py` & `xarg-python-1.5/xarg/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,16 @@
     def get_logger(self, name: Optional[str] = None) -> logging.Logger:
         return logging.getLogger(name if isinstance(name, str) else prog)
 
     def initiate_logger(self, logger: logging.Logger,
                         level: Optional[str] = None,
                         handlers: Optional[Iterable[logging.Handler]] = None,
                         filters: Optional[Iterable[logging.Filter]] = None):
-        assert not self.logger_initiated(logger.name)
+        if self.logger_initiated(logger.name):
+            logger.warning(F"logger {logger.name} is already initiated")
 
         if isinstance(level, str):
             logger.setLevel(logging._nameToLevel[level.upper()])
 
         if filters is None:
             filters = [once_filter()]
```

### Comparing `xarg-python-1.4.5/xarg/parser.py` & `xarg-python-1.5/xarg/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,29 +87,38 @@
                  **kwargs):
         kwargs.setdefault("prog", prog)
         kwargs.setdefault("usage", usage)
         kwargs.setdefault("description", description)
         kwargs.setdefault("epilog", epilog)
         ArgumentParser.__init__(self, **kwargs)
         self.__argv: Optional[Sequence[str]] = argv
-        self.__help_option: Dict[str, _HelpAction] = dict()
+        self.__help_option: Dict[str, _HelpAction] = {}
         self.__prev_parser: argp = prev_parser or self
-        self.__next_parser: List[argp] = list()
+        self.__next_parser: List[argp] = []
         if prev_parser is not None:
-            prev_parser.__next_parser.append(self)
+            prev_parser.next_parser.append(self)
 
     @property
     def argv(self) -> Optional[Sequence[str]]:
-        return self.root_parser.__argv
+        root = self.root_parser
+        return root.argv if root is not self else self.__argv
+
+    @property
+    def prev_parser(self) -> "argp":
+        return self.__prev_parser
+
+    @property
+    def next_parser(self) -> List["argp"]:
+        return self.__next_parser
 
     @property
     def root_parser(self) -> "argp":
-        root = self.__prev_parser
-        while root.__prev_parser != root:
-            root = root.__prev_parser
+        root = self.prev_parser
+        while root.prev_parser != root:
+            root = root.prev_parser
         return root
 
     def argument_group(self,
                        title: Optional[str] = None,
                        description: Optional[str] = None,
                        **kwargs) -> _ArgumentGroup:
         '''Find the created argument group by title, create if not exist.
@@ -212,20 +221,20 @@
 
         So, disable the help action before calling parse_known_args().
         The help option will be stored, and restored after the call ends.
         '''
 
         def __dfs_enable_help_action(root: argp):
             root.__enable_help_action()
-            for _sub in root.__next_parser:
+            for _sub in root.next_parser:
                 __dfs_enable_help_action(_sub)
 
         def __dfs_disable_help_action(root: argp):
             root.__disable_help_action()
-            for _sub in root.__next_parser:
+            for _sub in root.next_parser:
                 __dfs_disable_help_action(_sub)
 
         try:
             __dfs_disable_help_action(self.root_parser)
             namespace, _ = self.root_parser.parse_known_args(self.argv)
             return namespace
         finally:
```

### Comparing `xarg-python-1.4.5/xarg/safefile.py` & `xarg-python-1.5/xarg/safefile.py`

 * *Files identical despite different names*

### Comparing `xarg-python-1.4.5/xarg/scanner.py` & `xarg-python-1.5/xarg/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         @property
         def sha256(self) -> str:
             code, = self.hash(sha256())
             return code
 
     def __init__(self):
-        self.__objdict: Dict[str, scanner.object] = dict()
+        self.__objdict: Dict[str, scanner.object] = {}
         self.__objects: Set[scanner.object] = set()
         self.__objsyms: Set[scanner.object] = set()
         self.__objregs: Set[scanner.object] = set()
         self.__objdirs: Set[scanner.object] = set()
 
     def __iter__(self):
         return iter(self.__objects)
@@ -180,18 +180,21 @@
                 self.__objdirs.add(obj)
             elif obj.isreg:
                 self.__objregs.add(obj)
 
     @classmethod
     def load(cls,
              paths: Sequence[str],
-             exclude: Sequence[str] = [],
+             exclude: Optional[Sequence[str]] = None,
              linkdir: bool = True,
              threads: int = THDNUM_DEFAULT,
              handler: Optional[Callable[[object], bool]] = None):
+        if exclude is None:
+            exclude = []
+
         assert isinstance(paths, Sequence)
         assert isinstance(exclude, Sequence)
         assert isinstance(linkdir, bool)
         assert isinstance(threads, int)
 
         cmds = commands()
         thds = min(max(THDNUM_MINIMUM, threads), THDNUM_MAXIMUM)
@@ -212,34 +215,34 @@
         class task_stat:
 
             def __init__(self):
                 self.exit = False
                 self.handler = handler
                 self.scanner = scanner()
                 self.filter: Set[str] = filter()
-                self.q_path: Queue[str] = Queue()
-                self.q_task: Queue[scanner.object] = Queue(maxsize=thds * 2)
+                self.q_path: "Queue[str]" = Queue()
+                self.q_task: "Queue[scanner.object]" = Queue(maxsize=thds * 2)
 
         scan_stat = task_stat()
 
         def task_scan_path():
             scanned_dirs = set()
             name = current_thread().name
-            cmds.logger.debug(f"task thread[{name}] start")
+            cmds.logger.debug("task thread[%s] start", name)
             while not scan_stat.exit or not scan_stat.q_path.empty():
                 try:
                     path = scan_stat.q_path.get(timeout=0.01)
                 except Empty:
                     continue
 
                 path = rpath(path)
                 assert isinstance(path, str)
 
                 if path in scan_stat.filter or not os.path.exists(path):
-                    cmds.logger.debug(f"scan filter {path}")
+                    cmds.logger.debug("scan filter %s", path)
                     scan_stat.q_path.task_done()
                     continue
 
                 if os.path.isdir(path) and path not in scanned_dirs:
                     scanned_dirs.add(path)
                     # scan symbolic link dirs?
                     if not os.path.islink(path) or linkdir:
@@ -253,29 +256,29 @@
                 if isinstance(scan_stat.handler, Callable):
                     result = scan_stat.handler(object)
                     assert isinstance(result, bool)
 
                 if result is True:
                     scan_stat.q_task.put(object)
                 scan_stat.q_path.task_done()
-            cmds.logger.debug(f"task thread[{name}] exit")
+            cmds.logger.debug("task thread[%s] exit", name)
 
         def task_scan():
             name = current_thread().name
-            cmds.logger.debug(f"task thread[{name}] start")
+            cmds.logger.debug("task thread[%s] start", name)
             while not scan_stat.exit or not scan_stat.q_task.empty():
                 try:
                     obj = scan_stat.q_task.get(timeout=0.01)
                 except Empty:
                     continue
 
-                cmds.logger.debug(f"scan {obj.path}")
+                cmds.logger.debug("scan %s", obj.path)
                 scan_stat.scanner.add(obj=obj)
                 scan_stat.q_task.task_done()
-            cmds.logger.debug(f"task thread[{name}] exit")
+            cmds.logger.debug("task thread[%s] exit", name)
 
         task_threads: List[Thread] = []
         task_threads.append(Thread(target=task_scan, name="xarg-scan"))
         task_threads.extend([
             Thread(target=task_scan_path, name=f"xarg-scan{i}")
             for i in range(thds)
         ])
```

### Comparing `xarg-python-1.4.5/xarg/util.py` & `xarg-python-1.5/xarg/util.py`

 * *Files identical despite different names*

