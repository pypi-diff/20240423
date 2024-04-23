# Comparing `tmp/smooth_logger-0.2.2.tar.gz` & `tmp/smooth_logger-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smooth_logger-0.2.2.tar", last modified: Tue Feb 27 19:02:23 2024, max compression
+gzip compressed data, was "smooth_logger-0.3.0.tar", last modified: Tue Apr 23 19:46:08 2024, max compression
```

## Comparing `smooth_logger-0.2.2.tar` & `smooth_logger-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-02-27 19:02:23.825469 smooth_logger-0.2.2/
--rw-r--r--   0 murdo      (502) murdo      (502)    34020 2022-08-16 10:25:55.000000 smooth_logger-0.2.2/LICENSE
--rw-r--r--   0 murdo      (502) murdo      (502)     4951 2024-02-27 19:02:23.824469 smooth_logger-0.2.2/PKG-INFO
--rw-r--r--   0 murdo      (502) murdo      (502)     3984 2024-02-27 00:58:27.000000 smooth_logger-0.2.2/README.md
--rw-r--r--   0 murdo      (502) murdo      (502)       38 2024-02-27 19:02:23.825469 smooth_logger-0.2.2/setup.cfg
--rw-r--r--   0 murdo      (502) murdo      (502)     1210 2024-02-27 19:02:01.000000 smooth_logger-0.2.2/setup.py
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-02-27 19:02:23.823469 smooth_logger-0.2.2/smooth_logger/
--rw-r--r--   0 murdo      (502) murdo      (502)      474 2024-02-27 11:04:48.000000 smooth_logger-0.2.2/smooth_logger/LogEntry.py
--rw-r--r--   0 murdo      (502) murdo      (502)    11860 2024-02-27 19:00:23.000000 smooth_logger-0.2.2/smooth_logger/Logger.py
--rw-r--r--   0 murdo      (502) murdo      (502)       57 2024-02-27 00:59:30.000000 smooth_logger-0.2.2/smooth_logger/__init__.py
-drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-02-27 19:02:23.824469 smooth_logger-0.2.2/smooth_logger.egg-info/
--rw-r--r--   0 murdo      (502) murdo      (502)     4951 2024-02-27 19:02:23.000000 smooth_logger-0.2.2/smooth_logger.egg-info/PKG-INFO
--rw-r--r--   0 murdo      (502) murdo      (502)      286 2024-02-27 19:02:23.000000 smooth_logger-0.2.2/smooth_logger.egg-info/SOURCES.txt
--rw-r--r--   0 murdo      (502) murdo      (502)        1 2024-02-27 19:02:23.000000 smooth_logger-0.2.2/smooth_logger.egg-info/dependency_links.txt
--rw-r--r--   0 murdo      (502) murdo      (502)       22 2024-02-27 19:02:23.000000 smooth_logger-0.2.2/smooth_logger.egg-info/requires.txt
--rw-r--r--   0 murdo      (502) murdo      (502)       14 2024-02-27 19:02:23.000000 smooth_logger-0.2.2/smooth_logger.egg-info/top_level.txt
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/
+-rw-r--r--   0 murdo      (502) murdo      (502)    34020 2022-08-16 10:25:55.000000 smooth_logger-0.3.0/LICENSE
+-rw-r--r--   0 murdo      (502) murdo      (502)     6638 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/PKG-INFO
+-rw-r--r--   0 murdo      (502) murdo      (502)     5671 2024-04-23 19:45:55.000000 smooth_logger-0.3.0/README.md
+-rw-r--r--   0 murdo      (502) murdo      (502)       38 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/setup.cfg
+-rw-r--r--   0 murdo      (502) murdo      (502)     1210 2024-04-23 19:36:03.000000 smooth_logger-0.3.0/setup.py
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-04-23 19:46:08.610517 smooth_logger-0.3.0/smooth_logger/
+-rw-r--r--   0 murdo      (502) murdo      (502)      474 2024-02-27 11:04:48.000000 smooth_logger-0.3.0/smooth_logger/LogEntry.py
+-rw-r--r--   0 murdo      (502) murdo      (502)    13305 2024-04-23 19:35:11.000000 smooth_logger-0.3.0/smooth_logger/Logger.py
+-rw-r--r--   0 murdo      (502) murdo      (502)       88 2024-04-23 18:45:53.000000 smooth_logger-0.3.0/smooth_logger/__init__.py
+-rw-r--r--   0 murdo      (502) murdo      (502)      233 2024-04-23 18:46:37.000000 smooth_logger-0.3.0/smooth_logger/enums.py
+drwxr-xr-x   0 murdo      (502) murdo      (502)        0 2024-04-23 19:46:08.611518 smooth_logger-0.3.0/smooth_logger.egg-info/
+-rw-r--r--   0 murdo      (502) murdo      (502)     6638 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/PKG-INFO
+-rw-r--r--   0 murdo      (502) murdo      (502)      309 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)        1 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)       22 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/requires.txt
+-rw-r--r--   0 murdo      (502) murdo      (502)       14 2024-04-23 19:46:08.000000 smooth_logger-0.3.0/smooth_logger.egg-info/top_level.txt
```

### Comparing `smooth_logger-0.2.2/LICENSE` & `smooth_logger-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smooth_logger-0.2.2/PKG-INFO` & `smooth_logger-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth_logger
-Version: 0.2.2
+Version: 0.3.0
 Summary: A simple logger made primarily for my own personal use. Made from a combination of necessity and so much sloth that it overflowed into productivity.
 Home-page: https://github.com/MurdoMaclachlan/smooth_logger
 Author: Murdo Maclachlan
 Author-email: murdomaclachlan@duck.com
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
@@ -22,81 +22,114 @@
 
 # smooth_logger
 
 A simple logger made primarily for my own personal use. Was made out of a combination of necessity and being so lazy that I overflowed into being productive and instead of searching for a library that suited my needs, I wrote my own.
 
 ## Installation
 
-smooth-logger can be installed through pip. Either download the latest release from Codeberg/GitHub, or do `pip install smooth-logger` to install from PyPi. For the latest commits, check the `dev` branches on the repositories.
+smooth_logger can be installed through pip. Either download the latest release from Codeberg/GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branches on the repositories.
 
-smooth-logger was written in Python 3.9, but should work with Python 3.5 and up. A minimum of 3.5 is required due to the project's use of type hinting, which was introduced in that version.
+smooth_logger is currently devloped using Python 3.11, but should work with Python 3.5 and up. A minimum of 3.5 is required due to the project's use of type hinting, which was introduced in that version.
 
-smooth-logger supports Linux, macOS and Windows.
+smooth_logger supports Linux, macOS and Windows.
 
 ## Usage
 
 Usage of smooth-logger is, as it should be, quite simple.
 
 The `Logger` model provides a number of methods for your use:
 
+- `Logger.add_scope()` adds a new scope.
 - `Logger.clean()` erases all log entries currently in memory.
+- `Logger.edit_scope()` modifies the category of an existing scope.
 - `Logger.get()` allows you to retrieve either the most recent log entry or all log entries, optionally filtered by scope.
 - `Logger.get_time()` returns the full date & time, or optionally just the date, in ISO-8601 formatting.
 - `Logger.init_bar()` initialises the `ProgressBar` model imported from the `smooth_progress` dependency.
 - `Logger.notify()` sends a desktop notification using the `plyer` dependency.
 - `Logger.new()` creates and, depending on scope, prints a new log entry.
 - `Logger.output()` saves all log entries of appropriate scope to the log file and cleans the log array for the next group of log entries. A new log file is created for each new day. This method only attempts to create or update the log file if there are entries of an appropriate scope to be written to it; if there are none, it just executes `Logger.clean()`.
+- `Logger.remove_scope()` removes an existing scope.
 
-When initialising the Logger, you can optionally provide values to associate with each scope:
-
-- 0: disabled, do not print to console or save to log file
-- 1: enabled, print to console but do not save to log file
-- 2: maximum, print to console and save to log file
-
-The scopes available, along with their default values and suggested use cases, are:
-
-- DEBUG (0): Information for debugging the program.
-- ERROR (2): Errors that the program can recover from but impact functionality or performance.
-- FATAL (2): Errors that mean the program must continue; handled crashes.
-- INFO (1): General information for the user.
-- WARNING (2): Things that have no immediate impact to functionality but could cause errors later on.
+### Initialisation
 
 Here is a simple example showing the initialisation of the logger:
 
 ```py
 import smooth_logger
 
-Log = smooth_logger.Logger("Example", "~/.config/example")
+Log = smooth_logger.Logger("Example")
 Log.new("This is a log message!", "INFO")
 ```
 
-## Roadmap
+In the case above, the logger will automatically create a folder called `Example` under `~.config` on Linux and macOS, or `APPDATA\Roaming` on Windows, which will contain a subfolder called `logs`, where the log files will be saved.
+
+You can use the format below to provide a custom location:
+
+```py
+Log = smooth_logger.Logger("Example", config_path="~/this/is/an/example")
+```
+
+In this case, logs would be stored under, `~/this/is/an/example/logs`.
+
+### Scopes
+
+Every log message is associated with a scope. This is an all-caps prefix to the message that should, in a single word, communicate what the message is about. The default scopes available, along with their suggested use cases, are:
 
-A roadmap of planned future improvements and features:
+- DEBUG: Information for debugging the program.
+- ERROR: Errors that the program can recover from but impact functionality or performance.
+- FATAL: Errors that mean the program must continue; handled crashes.
+- INFO: General information for the user.
+- WARNING: Things that have no immediate impact to functionality but could cause errors later on.
 
-- Allow the creation of custom scopes. These would be instance-specific and not hard saved in any way. Suggested format and example:
+You can also use the value "NOSCOPE" to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
+
+### Categories
+
+When initialising the Logger, you can optionally provide categories to associate with each scope:
+
+- DISABLED (will not print to console or save to log file)
+- ENABLED (will print to console but not save to log file)
+- MAXIMUM (will print to console and save to log file)
+
+By default, the DEBUG scope is disabled, the INFO scope is enabled, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
+
+Categories are accessed like so:
+
+```py
+from smooth_logger.enums import Categories
+
+Categories.ENABLED
+```
 
-  ```
-  Log.add_scope(name: str, description: str, default_value: int)
-  
-  Log.add_scope("NEWSCOPE", "A new scope of mine!", 1)
-  ```
-  
-  Potentially also allow removal of scopes. In this situation, default scopes should be removable, but doing so should log a warning.
-  
-
-- Allow editing of the values of existing scopes post-initialisation. For example:
-
-  ```
-  Log.edit_scope(name: str, new_value: int)
-  
-  Log.edit_scope("DEBUG", 1)
-  ```
-  
-  to temporarily enable debug statements. This feature would probably see the most use from custom scopes.
-  
+### Customising scopes
 
-- Add an optional argument `notify: bool` to `Logger.new()` to allow log entries to be created and notified in one statement, rather than the two currently required.
+You can create custom scopes using the `Logger.add_scope()` method. These are currently instance-specific and not hard saved in any way. A simple usage of this is as follows:
+
+```py
+Log.add_scope("NEWSCOPE", Categories.ENABLED)
+```
+
+Similarly, you can use `Logger.edit_scope()` to modify the category of an existing scope (for the specific instance only), like so:
+
+```py
+Log.edit_scope("DEBUG", Categories.ENABLED)
+```
+
+The above statement could, for example, be used to temporarily enable debug statements if an error is detected.
+
+Only the categories defined in the `Categories` enum will be recognised; attempting to pass anything else as a category will prompt a warning, and the scope will not be added/edited.
+
+Finally, you can remove any scope with the following method:
+
+```py
+Log.remove_scope("DEBUG")
+```
+
+It is recommended to be careful with this method. Removing scopes, like adding or editing them, is ephemeral and won't be hard-saved anywhere, but removing a scope during run-time will produce warnings if you attempt to use that scope anywhere in your program.
+
+## Roadmap
 
 - Rework `Logger.get()` to allow passing of a specific number of log values to be fetched. If these values exceed the number in the log, all matching log values should be returned, and a warning should be issued (but not returned).
 
 - Possibly replace some internal warnings with Exceptions so they can be more easily-handled by end-user programs.
+
+- Add a category that saves to the log file but doesn't print to the console.
```

### Comparing `smooth_logger-0.2.2/setup.py` & `smooth_logger-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     return open('README.md', 'r').read()
 
 
 setup(
     name="smooth_logger",
-    version="0.2.2",
+    version="0.3.0",
     author="Murdo Maclachlan",
     author_email="murdomaclachlan@duck.com",
     description=(
         "A simple logger made primarily for my own personal use. Made from a combination of"
         + " necessity and so much sloth that it overflowed into productivity."
     ),
     long_description=readme(),
```

### Comparing `smooth_logger-0.2.2/smooth_logger/Logger.py` & `smooth_logger-0.3.0/smooth_logger/Logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 from datetime import datetime
 from os import environ, makedirs
 from os.path import expanduser, isdir
 from plyer import notification
+from plyer.facades import Notification
 from smooth_progress import ProgressBar
 from time import time
-from .LogEntry import LogEntry
+from typing_extensions import Union
 
-from plyer.facades import Notification
-from typing import Dict, List, Union
+from .enums import Categories
+from .LogEntry import LogEntry
 
 
 class Logger:
     """
     Class for controlling the entirety of logging. The logging works on a scope-based system where
     (almost) every message has a defined scope, and the scopes are each associated with a specific
-    value between 0 and 2 inclusive. The meanings of the values are as follows:
+    category between 0 and 2 inclusive. The meanings of the categories are as follows:
 
     0: disabled, do not print to console or save to log file
     1: enabled, print to console but do not save to log file
     2: maximum, print to console and save to log file
     """
     def __init__(self,
                  program_name: str,
                  config_path: str = None,
-                 debug: int = 0,
-                 error: int = 2,
-                 fatal: int = 2,
-                 info: int = 1,
-                 warning: int = 2) -> None:
+                 debug: int = Categories.DISABLED,
+                 error: int = Categories.MAXIMUM,
+                 fatal: int = Categories.MAXIMUM,
+                 info: int = Categories.ENABLED,
+                 warning: int = Categories.MAXIMUM) -> None:
         self.bar: ProgressBar = ProgressBar()
         self.__is_empty: bool = True
-        self.__log: List[LogEntry] = []
+        self.__log: list[LogEntry] = []
         self.__notifier: Notification = notification
         self.__program_name: str = program_name
-        self.__scopes: Dict[str, int] = {
+        self.__scopes: dict[str, int] = {
             "DEBUG":   debug,   # information for debugging the program
             "ERROR":   error,   # errors the program can recover from
             "FATAL":   fatal,   # errors that mean the program cannot continue
             "INFO":    info,    # general information for the user
             "WARNING": warning  # things that could cause errors later on
         }
         self.__write_logs = False
@@ -116,15 +117,15 @@
 
         :param entry: the entry to display
         :param scope: the scope of the entry
         :param notify: whether to show a desktop notification for the entry
         :param is_bar: whether the progress bar is active
         :param console: whether the message should be printed to the console
         """
-        if scope == "NOSCOPE" or (self.__scopes[scope] > 0 and print_to_console):
+        if scope == "NOSCOPE" or (self.__scopes[scope] != Categories.DISABLED and print_to_console):
             print(entry.rendered)
         if is_bar:
             print(self.bar.state, end="\r", flush=True)
         if notify:
             self.notify(entry.message)
 
     def __get_time(self, method: str = "time") -> str:
@@ -140,97 +141,112 @@
             return datetime.fromtimestamp(time()).strftime(
                 ("%Y-%m-%d", "%Y-%m-%d %H:%M:%S")[method == "time"]
             )
         else:
             self.new("Bad method passed to Logger.get_time().", "ERROR")
             return ""
 
-    def add_scope(self, name: str, value: int) -> bool:
+    def add_scope(self, name: str, category: int) -> bool:
         """
         Adds a new logging scope for use with log entries. Users should be careful when doing this;
         custom scopes would be best added immediately following initialisation. If a 'Logger.new()'
         call is made before the scope it uses is added, it will generate a warning.
 
         The recommended format for scope names is all uppercase, with no spaces or underscores.
         Custom scopes are instance specific and not hard saved.
 
         :param name: the name of the new scope
-        :param value: the default value of the new scope (0-2)
+        :param category: the default category of the new scope (0-2)
 
         :return: a boolean sucess status
         """
         if name in self.__scopes.keys():
             self.new(
                 f"Attempt was made to add new scope with name {name}, but scope with this name "
                 + "already exists.",
                 "WARNING"
             )
         else:
-            self.__scopes[name] = value
-            return True
+            if category in set(item for item in Categories):
+                self.__scopes[name] = category
+                return True
+            else:
+                self.new(
+                    f"Attempt was made to add new scope with category {category}, but this is not "
+                    + "a valid category.",
+                    "WARNING"
+                )
         return False
 
     def clean(self) -> None:
         """
         Empties log array. Any log entries not saved to the output file will be lost.
         """
         del self.__log[:]
         self.__is_empty = True
         self.__write_logs = False
 
-    def edit_scope(self, name: str, value: int) -> bool:
+    def edit_scope(self, name: str, category: int) -> bool:
         """
-        Edits an existing scope's value. Edited values are instance specific and not hard saved.
+        Edits an existing scope's category, if the scope exists. Edited categories are instance
+        specific and not hard saved.
 
         :param name: the name of the scope to edit
-        :param value: the new value of the scope (0-2)
+        :param category: the new category of the scope (0-2)
 
         :returns: a boolean success status
         """
         if name in self.__scopes.keys():
-            self.__scopes[name] = value
-            return True
+            if category in set(item for item in Categories):
+                self.__scopes[name] = category
+                return True
+            else:
+                self.new(
+                    f"Attempt was made to change category of scope {name} to {category}, but this "
+                    + "is not a valid category.",
+                    "WARNING"
+                )
         else:
             self.new(
-                f"Attempt was made to edit a scope with name {name}, but no scope with "
-                + "this name exists.",
+                f"Attempt was made to edit a scope with name {name}, but no scope with this name "
+                + "exists.",
                 "WARNING"
             )
         return False
 
-    def get(self, mode: str = "all", scope: str = None) -> Union[List[LogEntry], LogEntry]:
+    def get(self, mode: str = "all", scope: str = None) -> Union[list[LogEntry], LogEntry, None]:
         """
         Returns item(s) in the log. The entries returned can be controlled by passing optional
         arguments.
 
         If no entries match the query, nothing will be returned.
 
         :param mode: optional; 'all' for all log entries or 'recent' for only the most recent one
-        :param scope: optional; if passed, only entries matching its value will be returned
+        :param scope: optional; if passed, only entries matching its category will be returned
 
         :returns: a single log entry or list of log entries, or nothing
         """
         if self.__is_empty:
             pass
         elif scope is None:
             return (self.__log, self.__log[-1])[mode == "recent"]
         else:
             # return all log entries matching the query
             if mode == "all":
                 data: list[LogEntry] = []
-                for i in self.__log:
-                    if scope is None or i.scope == scope:
-                        data.append(i)
+                for entry in self.__log:
+                    if scope is None or entry.scope == scope:
+                        data.append(entry)
                 if data:
                     return data
             # iterate through the log in reverse to find the most recent entry matching the query
             elif mode == "recent":
-                for i in range(len(self.__log)-1, 0):
-                    if scope is None or self.__log[i].scope == scope:
-                        return self.__log[i]
+                for entry in reversed(self.__log):
+                    if scope is None or entry.scope == scope:
+                        return entry
             else:
                 self.new("Unknown mode passed to Logger.get().", "WARNING")
 
     def init_bar(self, limit: int) -> None:
         """
         Initiate and open the progress bar.
 
@@ -255,15 +271,19 @@
                                  the console
         :param notify: optional, default False; whether the message should be displayed as a
                        desktop notification
 
         :returns: a boolean success status
         """
         if scope in self.__scopes or scope == "NOSCOPE":
-            output: bool = (self.__scopes[scope] == 2) if scope != "NOSCOPE" else False
+            output: bool = (
+                (self.__scopes[scope] == Categories.MAXIMUM)
+                if scope != "NOSCOPE" else
+                False
+            )
             is_bar: bool = (self.bar is not None) and self.bar.opened
 
             # if the progress bar is enabled, append any necessary empty characters to the message
             # to completely overwrite it upon output
             if is_bar and len(message) < len(self.bar.state):
                 message += " " * (len(self.bar.state) - len(message))
             
@@ -296,7 +316,26 @@
         if self.__write_logs:
             with open(f"{self.__output_path}/log-{self.__get_time(method='date')}.txt",
                       "at+") as log_file:
                 for line in self.__log:
                     if line.output:
                         log_file.write(line.rendered + "\n")
         self.clean()
+
+    def remove_scope(self, name: str) -> bool:
+        """
+        Removes an existing scope if it exists.
+
+        :param name: the name of the scope to remove
+
+        :returns: a boolean success status
+        """
+        if name in self.__scopes.keys():
+            del self.__scopes[name]
+            return True
+        else:
+            self.new(
+                f"Attempt was made to remove a scope with name {name}, but no scope with this "
+                + "name exists.",
+                "WARNING"
+            )
+        return False
```

### Comparing `smooth_logger-0.2.2/smooth_logger.egg-info/PKG-INFO` & `smooth_logger-0.3.0/smooth_logger.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smooth_logger
-Version: 0.2.2
+Version: 0.3.0
 Summary: A simple logger made primarily for my own personal use. Made from a combination of necessity and so much sloth that it overflowed into productivity.
 Home-page: https://github.com/MurdoMaclachlan/smooth_logger
 Author: Murdo Maclachlan
 Author-email: murdomaclachlan@duck.com
 License: AGPLv3+
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.7
@@ -22,81 +22,114 @@
 
 # smooth_logger
 
 A simple logger made primarily for my own personal use. Was made out of a combination of necessity and being so lazy that I overflowed into being productive and instead of searching for a library that suited my needs, I wrote my own.
 
 ## Installation
 
-smooth-logger can be installed through pip. Either download the latest release from Codeberg/GitHub, or do `pip install smooth-logger` to install from PyPi. For the latest commits, check the `dev` branches on the repositories.
+smooth_logger can be installed through pip. Either download the latest release from Codeberg/GitHub, or do `pip install smooth_logger` to install from PyPi. For the latest commits, check the `dev` branches on the repositories.
 
-smooth-logger was written in Python 3.9, but should work with Python 3.5 and up. A minimum of 3.5 is required due to the project's use of type hinting, which was introduced in that version.
+smooth_logger is currently devloped using Python 3.11, but should work with Python 3.5 and up. A minimum of 3.5 is required due to the project's use of type hinting, which was introduced in that version.
 
-smooth-logger supports Linux, macOS and Windows.
+smooth_logger supports Linux, macOS and Windows.
 
 ## Usage
 
 Usage of smooth-logger is, as it should be, quite simple.
 
 The `Logger` model provides a number of methods for your use:
 
+- `Logger.add_scope()` adds a new scope.
 - `Logger.clean()` erases all log entries currently in memory.
+- `Logger.edit_scope()` modifies the category of an existing scope.
 - `Logger.get()` allows you to retrieve either the most recent log entry or all log entries, optionally filtered by scope.
 - `Logger.get_time()` returns the full date & time, or optionally just the date, in ISO-8601 formatting.
 - `Logger.init_bar()` initialises the `ProgressBar` model imported from the `smooth_progress` dependency.
 - `Logger.notify()` sends a desktop notification using the `plyer` dependency.
 - `Logger.new()` creates and, depending on scope, prints a new log entry.
 - `Logger.output()` saves all log entries of appropriate scope to the log file and cleans the log array for the next group of log entries. A new log file is created for each new day. This method only attempts to create or update the log file if there are entries of an appropriate scope to be written to it; if there are none, it just executes `Logger.clean()`.
+- `Logger.remove_scope()` removes an existing scope.
 
-When initialising the Logger, you can optionally provide values to associate with each scope:
-
-- 0: disabled, do not print to console or save to log file
-- 1: enabled, print to console but do not save to log file
-- 2: maximum, print to console and save to log file
-
-The scopes available, along with their default values and suggested use cases, are:
-
-- DEBUG (0): Information for debugging the program.
-- ERROR (2): Errors that the program can recover from but impact functionality or performance.
-- FATAL (2): Errors that mean the program must continue; handled crashes.
-- INFO (1): General information for the user.
-- WARNING (2): Things that have no immediate impact to functionality but could cause errors later on.
+### Initialisation
 
 Here is a simple example showing the initialisation of the logger:
 
 ```py
 import smooth_logger
 
-Log = smooth_logger.Logger("Example", "~/.config/example")
+Log = smooth_logger.Logger("Example")
 Log.new("This is a log message!", "INFO")
 ```
 
-## Roadmap
+In the case above, the logger will automatically create a folder called `Example` under `~.config` on Linux and macOS, or `APPDATA\Roaming` on Windows, which will contain a subfolder called `logs`, where the log files will be saved.
+
+You can use the format below to provide a custom location:
+
+```py
+Log = smooth_logger.Logger("Example", config_path="~/this/is/an/example")
+```
+
+In this case, logs would be stored under, `~/this/is/an/example/logs`.
+
+### Scopes
+
+Every log message is associated with a scope. This is an all-caps prefix to the message that should, in a single word, communicate what the message is about. The default scopes available, along with their suggested use cases, are:
 
-A roadmap of planned future improvements and features:
+- DEBUG: Information for debugging the program.
+- ERROR: Errors that the program can recover from but impact functionality or performance.
+- FATAL: Errors that mean the program must continue; handled crashes.
+- INFO: General information for the user.
+- WARNING: Things that have no immediate impact to functionality but could cause errors later on.
 
-- Allow the creation of custom scopes. These would be instance-specific and not hard saved in any way. Suggested format and example:
+You can also use the value "NOSCOPE" to indicate that a message should be printed without a prefixed scope. Messages with no scope are printed to the console, not saved to the output file, and are not accompanied by a timestamp.
+
+### Categories
+
+When initialising the Logger, you can optionally provide categories to associate with each scope:
+
+- DISABLED (will not print to console or save to log file)
+- ENABLED (will print to console but not save to log file)
+- MAXIMUM (will print to console and save to log file)
+
+By default, the DEBUG scope is disabled, the INFO scope is enabled, and the ERROR, FATAL and WARNING scopes are all set to maximum. Scopes set to maximum are not *automatically* saved to the log file; calling `Logger.output()` will save them and then clean the in-memory log to avoid duplication.
+
+Categories are accessed like so:
+
+```py
+from smooth_logger.enums import Categories
+
+Categories.ENABLED
+```
 
-  ```
-  Log.add_scope(name: str, description: str, default_value: int)
-  
-  Log.add_scope("NEWSCOPE", "A new scope of mine!", 1)
-  ```
-  
-  Potentially also allow removal of scopes. In this situation, default scopes should be removable, but doing so should log a warning.
-  
-
-- Allow editing of the values of existing scopes post-initialisation. For example:
-
-  ```
-  Log.edit_scope(name: str, new_value: int)
-  
-  Log.edit_scope("DEBUG", 1)
-  ```
-  
-  to temporarily enable debug statements. This feature would probably see the most use from custom scopes.
-  
+### Customising scopes
 
-- Add an optional argument `notify: bool` to `Logger.new()` to allow log entries to be created and notified in one statement, rather than the two currently required.
+You can create custom scopes using the `Logger.add_scope()` method. These are currently instance-specific and not hard saved in any way. A simple usage of this is as follows:
+
+```py
+Log.add_scope("NEWSCOPE", Categories.ENABLED)
+```
+
+Similarly, you can use `Logger.edit_scope()` to modify the category of an existing scope (for the specific instance only), like so:
+
+```py
+Log.edit_scope("DEBUG", Categories.ENABLED)
+```
+
+The above statement could, for example, be used to temporarily enable debug statements if an error is detected.
+
+Only the categories defined in the `Categories` enum will be recognised; attempting to pass anything else as a category will prompt a warning, and the scope will not be added/edited.
+
+Finally, you can remove any scope with the following method:
+
+```py
+Log.remove_scope("DEBUG")
+```
+
+It is recommended to be careful with this method. Removing scopes, like adding or editing them, is ephemeral and won't be hard-saved anywhere, but removing a scope during run-time will produce warnings if you attempt to use that scope anywhere in your program.
+
+## Roadmap
 
 - Rework `Logger.get()` to allow passing of a specific number of log values to be fetched. If these values exceed the number in the log, all matching log values should be returned, and a warning should be issued (but not returned).
 
 - Possibly replace some internal warnings with Exceptions so they can be more easily-handled by end-user programs.
+
+- Add a category that saves to the log file but doesn't print to the console.
```

