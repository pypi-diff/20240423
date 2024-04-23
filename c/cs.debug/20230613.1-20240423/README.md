# Comparing `tmp/cs.debug-20230613.1.tar.gz` & `tmp/cs.debug-20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.debug-20230613.1.tar", last modified: Tue Jun 13 01:11:26 2023, max compression
+gzip compressed data, was "cs.debug-20240423.tar", last modified: Tue Apr 23 07:58:49 2024, max compression
```

## Comparing `cs.debug-20230613.1.tar` & `cs.debug-20240423.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.058406 cs.debug-20230613.1/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-06-13 01:11:02.000000 cs.debug-20230613.1/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     6022 2023-06-13 01:11:26.058545 cs.debug-20230613.1/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     5455 2023-06-13 01:11:06.000000 cs.debug-20230613.1/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.053857 cs.debug-20230613.1/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.054307 cs.debug-20230613.1/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.056394 cs.debug-20230613.1/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    19453 2023-06-13 01:10:53.000000 cs.debug-20230613.1/lib/python/cs/debug.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-06-13 01:11:26.058138 cs.debug-20230613.1/lib/python/cs.debug.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     6022 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      292 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      199 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-06-13 01:11:26.000000 cs.debug-20230613.1/lib/python/cs.debug.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     6439 2023-06-13 01:11:17.000000 cs.debug-20230613.1/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1043 2023-06-13 01:11:26.059136 cs.debug-20230613.1/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-06-13 01:11:06.000000 cs.debug-20230613.1/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.129033 cs.debug-20240423/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-23 07:58:34.000000 cs.debug-20240423/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4591 2024-04-23 07:58:49.128766 cs.debug-20240423/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     3802 2024-04-23 07:58:38.000000 cs.debug-20240423/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.125067 cs.debug-20240423/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.125351 cs.debug-20240423/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.126602 cs.debug-20240423/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    20486 2024-04-23 07:58:20.000000 cs.debug-20240423/lib/python/cs/debug.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 07:58:49.128322 cs.debug-20240423/lib/python/cs.debug.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     4591 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      273 2024-04-23 07:58:49.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      216 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-23 07:58:48.000000 cs.debug-20240423/lib/python/cs.debug.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     5209 2024-04-23 07:58:47.000000 cs.debug-20240423/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-23 07:58:49.129152 cs.debug-20240423/setup.cfg
```

### Comparing `cs.debug-20230613.1/PKG-INFO` & `cs.debug-20240423/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,75 @@
-Metadata-Version: 2.1
-Name: cs.debug
-Version: 20230613.1
-Summary: Assorted debugging facilities.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
+[project]
+name = "cs.debug"
+description = "Assorted debugging facilities."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.deco>=20240412",
+    "cs.fs>=20240422",
+    "cs.lex>=20240316",
+    "cs.logutils>=20230212",
+    "cs.obj>=20220918",
+    "cs.pfx>=20240412",
+    "cs.py.func>=20230331",
+    "cs.py.stack>=20240412",
+    "cs.py3>=20220523",
+    "cs.seq>=20221118",
+    "cs.upd>=20240412",
+    "cs.x>=20240316",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 2",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240423"
 
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Assorted debugging facilities.
 
-*Latest release 20230613.1*:
-Bugfix builtins monkey patch.
+*Latest release 20240423*:
+* Support \"import *\" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
+* @trace: include the elapsed time on the return/exception log message.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
-The allowed names are the following:
+The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
+* `breakpoint`: `cs.upd.breakpoint`
 * `pformat`: `pprint.pformat`
 * `pprint`: `pprint.pprint`
+* `print`: `cs.upd.print`
 * `r`: `cs.lex.r`
+* `redirect_stdout`: `contextlib.redirect_stdout`
 * `s`: `cs.lex.s`
-* `trace`: `cs.debug.trace` (the `@trace` decorator)
-
-## Function `DEBUG(f, force=False)`
-
-Decorator to wrap functions in timing and value debuggers.
-
-## Function `debug_object_shell(o, prompt=None)`
-
-Interactive prompt for inspecting variables.
-
-## Class `DebuggingLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for `threading.Lock` to trace creation and use.
-
-`cs.threads.Lock()` returns one of these in debug mode or a raw
-`threading.Lock` otherwise.
-
-## Class `DebuggingRLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for threading.RLock to trace creation and use.
-
-`cs.threads.RLock()` returns on of these in debug mode or a raw
-`threading.RLock` otherwise.
-
-## Class `DebugShell(cmd.Cmd)`
-
-An interactive prompt for python statements, attached to `/dev/tty` by default.
-
-## Class `DebugWrapper(types.SimpleNamespace)`
-
-Base class for classes presenting debugging wrappers.
-
-## Function `DF(func, *a, **kw)`
-
-Wrapper for a function call to debug its use.
-
-This requires rewriting the call from `f(*a,*kw)` to `DF(f,*a,**kw)`.
-Alternatively one could rewrite as `DEBUG(f)(*a,**kw)`.
-
-## Class `Lock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for `threading.Lock` to trace creation and use.
-
-`cs.threads.Lock()` returns one of these in debug mode or a raw
-`threading.Lock` otherwise.
-
-## Function `openfiles(substr=None, pid=None)`
-
-Run lsof(8) against process `pid`
-returning paths of open files whose paths contain `substr`.
-
-Parameters:
-* `substr`: default substring to select by; default returns all paths.
-* `pid`: process to examine; default from `os.getpid()`.
-
-## Class `RLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for threading.RLock to trace creation and use.
-
-`cs.threads.RLock()` returns on of these in debug mode or a raw
-`threading.RLock` otherwise.
-
-## Function `selftest(module_name, defaultTest=None, argv=None)`
-
-Called by my unit tests.
+* `stack_dump`: dump current `Thread`'s call stack
+* `thread_dump` dump the active `Thread`s with their call stacks
+* `trace`: the `@trace` decorator
+`$CS_DEBUG_BUILTINS` can also be set to `\"1\"` to install all of
+`__all__` in the builtins.
 
 ## Function `stack_dump(stack=None, limit=None, logger=None, log_level=None)`
 
 Dump a stack trace to a logger.
 
 Parameters:
 * `stack`: a stack list as returned by `traceback.extract_stack`.
@@ -125,26 +93,22 @@
 
 A `Lock` replacement which times out, used for locating deadlock points.
 
 ## Function `trace(*da, **dkw)`
 
 Decorator to report the call and return of a function.
 
-## Function `trace_caller(func)`
-
-Decorator to report the caller of a function when called.
-
-## Class `TraceSuite`
-
-Context manager to trace start and end of a code suite.
-
 # Release Log
 
 
 
+*Release 20240423*:
+* Support \"import *\" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
+* @trace: include the elapsed time on the return/exception log message.
+
 *Release 20230613.1*:
 Bugfix builtins monkey patch.
 
 *Release 20230613*:
 Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
 
 *Release 20230610*:
@@ -171,17 +135,34 @@
 * Update imports for recentchanges.
 * New context manager TraceSuite to trace start and end of a code suite.
 
 *Release 20160918*:
 selftest(): fix parameter ordering to match unittest.
 
 *Release 20160828*:
-Update metadata with "install_requires" instead of "requires".
+Update metadata with \"install_requires\" instead of \"requires\".
 
 *Release 20160827*:
 * New openfiles() to return selected pathnames of open files via lsof(8).
 * New selftest() to invoke unittests with benefits.
 * DebugShell, a cmd.Cmd subclass for debugging - current use case calls this with self.__dict__ in a test case tearDwon.
 * debug_object_shell: convenience wrapper for DebugShell to call it on an object's attributes.
 
 *Release 20150116*:
-PyPI prep.
+PyPI prep."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.debug",
+]
+
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.debug-20230613.1/README.md` & `cs.debug-20240423/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,102 +1,31 @@
 Assorted debugging facilities.
 
-*Latest release 20230613.1*:
-Bugfix builtins monkey patch.
+*Latest release 20240423*:
+* Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
+* @trace: include the elapsed time on the return/exception log message.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
-The allowed names are the following:
+The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
+* `breakpoint`: `cs.upd.breakpoint`
 * `pformat`: `pprint.pformat`
 * `pprint`: `pprint.pprint`
+* `print`: `cs.upd.print`
 * `r`: `cs.lex.r`
+* `redirect_stdout`: `contextlib.redirect_stdout`
 * `s`: `cs.lex.s`
-* `trace`: `cs.debug.trace` (the `@trace` decorator)
-
-## Function `DEBUG(f, force=False)`
-
-Decorator to wrap functions in timing and value debuggers.
-
-## Function `debug_object_shell(o, prompt=None)`
-
-Interactive prompt for inspecting variables.
-
-## Class `DebuggingLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for `threading.Lock` to trace creation and use.
-
-`cs.threads.Lock()` returns one of these in debug mode or a raw
-`threading.Lock` otherwise.
-
-*Method `DebuggingLock.acquire(self, *a)`*:
-Acquire the lock.
-
-*Method `DebuggingLock.release(self)`*:
-Release the lock.
-
-## Class `DebuggingRLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for threading.RLock to trace creation and use.
-
-`cs.threads.RLock()` returns on of these in debug mode or a raw
-`threading.RLock` otherwise.
-
-## Class `DebugShell(cmd.Cmd)`
-
-An interactive prompt for python statements, attached to `/dev/tty` by default.
-
-*Method `DebugShell.default(self, line)`*:
-Default command action.
-
-## Class `DebugWrapper(types.SimpleNamespace)`
-
-Base class for classes presenting debugging wrappers.
-
-## Function `DF(func, *a, **kw)`
-
-Wrapper for a function call to debug its use.
-
-This requires rewriting the call from `f(*a,*kw)` to `DF(f,*a,**kw)`.
-Alternatively one could rewrite as `DEBUG(f)(*a,**kw)`.
-
-## Class `Lock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for `threading.Lock` to trace creation and use.
-
-`cs.threads.Lock()` returns one of these in debug mode or a raw
-`threading.Lock` otherwise.
-
-*Method `Lock.acquire(self, *a)`*:
-Acquire the lock.
-
-*Method `Lock.release(self)`*:
-Release the lock.
-
-## Function `openfiles(substr=None, pid=None)`
-
-Run lsof(8) against process `pid`
-returning paths of open files whose paths contain `substr`.
-
-Parameters:
-* `substr`: default substring to select by; default returns all paths.
-* `pid`: process to examine; default from `os.getpid()`.
-
-## Class `RLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for threading.RLock to trace creation and use.
-
-`cs.threads.RLock()` returns on of these in debug mode or a raw
-`threading.RLock` otherwise.
-
-## Function `selftest(module_name, defaultTest=None, argv=None)`
-
-Called by my unit tests.
+* `stack_dump`: dump current `Thread`'s call stack
+* `thread_dump` dump the active `Thread`s with their call stacks
+* `trace`: the `@trace` decorator
+`$CS_DEBUG_BUILTINS` can also be set to `"1"` to install all of
+`__all__` in the builtins.
 
 ## Function `stack_dump(stack=None, limit=None, logger=None, log_level=None)`
 
 Dump a stack trace to a logger.
 
 Parameters:
 * `stack`: a stack list as returned by `traceback.extract_stack`.
@@ -120,26 +49,22 @@
 
 A `Lock` replacement which times out, used for locating deadlock points.
 
 ## Function `trace(*da, **dkw)`
 
 Decorator to report the call and return of a function.
 
-## Function `trace_caller(func)`
-
-Decorator to report the caller of a function when called.
-
-## Class `TraceSuite`
-
-Context manager to trace start and end of a code suite.
-
 # Release Log
 
 
 
+*Release 20240423*:
+* Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
+* @trace: include the elapsed time on the return/exception log message.
+
 *Release 20230613.1*:
 Bugfix builtins monkey patch.
 
 *Release 20230613*:
 Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
 
 *Release 20230610*:
```

### Comparing `cs.debug-20230613.1/lib/python/cs/debug.py` & `cs.debug-20240423/lib/python/cs/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,33 @@
 r'''
 Assorted debugging facilities.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
-The allowed names are the following:
+The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
+* `breakpoint`: `cs.upd.breakpoint`
 * `pformat`: `pprint.pformat`
 * `pprint`: `pprint.pprint`
+* `print`: `cs.upd.print`
 * `r`: `cs.lex.r`
+* `redirect_stdout`: `contextlib.redirect_stdout`
 * `s`: `cs.lex.s`
-* `trace`: `cs.debug.trace` (the `@trace` decorator)
+* `stack_dump`: dump current `Thread`'s call stack
+* `thread_dump` dump the active `Thread`s with their call stacks
+* `trace`: the `@trace` decorator
+`$CS_DEBUG_BUILTINS` can also be set to `"1"` to install all of
+`__all__` in the builtins.
 '''
 
 from __future__ import print_function
 from cmd import Cmd
+from contextlib import redirect_stdout
 import inspect
 import logging
 import os
 from pprint import pformat, pprint  # pylint: disable=unused-import
 from subprocess import Popen, PIPE
 import sys
 from threading import (
@@ -34,28 +42,29 @@
     RLock as threading_RLock,
     Thread as threading_Thread,
 )
 import time
 import traceback
 from types import SimpleNamespace as NS
 
-from cs.deco import decorator
+from cs.deco import ALL, decorator
 from cs.fs import shortpath
 from cs.lex import s, r, is_identifier  # pylint: disable=unused-import
 import cs.logutils
 from cs.logutils import debug, error, warning, D, ifdebug, loginfo
 from cs.obj import Proxy
 from cs.pfx import Pfx
 from cs.py.func import funccite, func_a_kw_fmt
 from cs.py.stack import caller
 from cs.py3 import Queue, Queue_Empty, exec_code
 from cs.seq import seq
+from cs.upd import breakpoint, print  # pylint: disable=redefined-builtin
 from cs.x import X
 
-__version__ = '20230613.1'
+__version__ = '20240423'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
@@ -67,28 +76,35 @@
         'cs.logutils',
         'cs.obj',
         'cs.pfx',
         'cs.py.func',
         'cs.py.stack',
         'cs.py3',
         'cs.seq',
+        'cs.upd',
         'cs.x',
     ],
 }
 
+__all__ = [
+    'X', 'breakpoint', 'pformat', 'pprint', 'print', 'r', 'redirect_stdout',
+    's'
+]
+
 # environment variable specifying names to become built in
 CS_DEBUG_BUILTINS_ENVVAR = 'CS_DEBUG_BUILTINS'
 
 # white list of allowed builtin names
 CS_DEBUG_BUILTINS_NAMES = ('X', 'pformat', 'pprint', 's', 'r', 'trace')
 
 # @DEBUG dispatches a thread to monitor function elapsed time.
 # This is how often it polls for function completion.
 DEBUG_POLL_RATE = 0.25
 
+@ALL
 class TimingOutLock(object):
   ''' A `Lock` replacement which times out, used for locating deadlock points.
   '''
 
   def __init__(self, deadlock_timeout=20.0, recursive=False):
     self._lock = threading_RLock() if recursive else threading_Lock()
     self._deadlock_timeout = deadlock_timeout
@@ -139,14 +155,15 @@
 
 def Thread(*a, **kw):
   if not ifdebug():
     return threading_Thread(*a, **kw)
   filename, lineno = inspect.stack()[1][1:3]
   return DebuggingThread({'filename': filename, 'lineno': lineno}, *a, **kw)
 
+@ALL
 def thread_dump(Ts=None, fp=None):
   ''' Write thread identifiers and stack traces to the file `fp`.
 
       Parameters:
       * `Ts`: the `Thread`s to dump; if unspecified use `threading.enumerate()`.
       * `fp`: the file to which to write; if unspecified use `sys.stderr`.
   '''
@@ -162,14 +179,15 @@
       except KeyError:
         warning("no frame for Thread.ident=%s", T.ident)
         continue
       print("Thread", T.ident, T.name, file=fp)
       traceback.print_stack(frame, None, fp)
       print(file=fp)
 
+@ALL
 def stack_dump(stack=None, limit=None, logger=None, log_level=None):
   ''' Dump a stack trace to a logger.
 
       Parameters:
       * `stack`: a stack list as returned by `traceback.extract_stack`.
         If missing or `None`, use the result of `traceback.extract_stack()`.
       * `limit`: a limit to the number of stack entries to dump.
@@ -583,14 +601,15 @@
     intro += '\n  %s = %r' % (k, v[k])
   intro += '\n'
   C.prompt = prompt
   C.cmdloop(intro)
 
 _trace_indent = ""
 
+@ALL
 @decorator
 # pylint: disable=too-many-arguments
 def trace(
     func,
     call=True,
     retval=False,
     exception=True,
@@ -620,32 +639,48 @@
     if with_caller:
       log_cite = log_cite + "from[%s]" % (caller(),)
     if call:
       fmt, av = func_a_kw_fmt(log_cite, *a, **kw)
       xlog("%sCALL " + fmt, _trace_indent, *av)
     old_indent = _trace_indent
     _trace_indent += '  '
+    start_time = time.time()
     try:
       result = func(*a, **kw)
     except Exception as e:
+      end_time = time.time()
       if exception:
-        xlog("%sCALL %s RAISE %r", _trace_indent, log_cite, e)
+        xlog(
+            "%sCALL %s %gs RAISE %r",
+            _trace_indent,
+            log_cite,
+            end_time - start_time,
+            e,
+        )
       _trace_indent = old_indent
       raise
     else:
+      end_time = time.time()
       if retval:
         xlog(
-            "%sCALL %s RETURN %s",
+            "%sCALL %s %gs RETURN %s",
             _trace_indent,
             log_cite,
+            end_time - start_time,
             (pformat if use_pformat else repr)(result),
         )
       else:
         ##xlog("%sRETURN %s <= %s", _trace_indent, type(result), log_cite)
-        xlog("%sRETURN %s <= %s", _trace_indent, s(result), log_cite)
+        xlog(
+            "%sRETURN %gs %s <= %s",
+            _trace_indent,
+            end_time - start_time,
+            s(result),
+            log_cite,
+        )
       _trace_indent = old_indent
       return result
 
   traced_function_wrapper.__name__ = "@trace(%s)" % (citation,)
   traced_function_wrapper.__doc__ = "@trace(%s)\n\n" + (func.__doc__ or '')
   return traced_function_wrapper
 
@@ -669,24 +704,28 @@
     import builtins  # pylint: disable=unused-import
   except ImportError:
     warning(
         "$%s=%r but connot import builtins for monkey patching",
         CS_DEBUG_BUILTINS_ENVVAR, builtin_names_s
     )
   else:
-    for builtin_name in builtin_names_s.split(','):
+    vs = vars()
+    for builtin_name in (__all__ if builtin_names_s == "1" else
+                         builtin_names_s.split(',')):
       if not builtin_name:
         continue
-      if builtin_name not in CS_DEBUG_BUILTINS_NAMES:
+      if builtin_name in ('breakpoint',):
+        # breakpoint doesn't work right if wrapped, gets the wrong frame
+        continue
+      if builtin_name not in __all__:
         warning(
-            "$%s: ignoring %r, not in CS_DEBUG_BUILTINS_NAMES:%r",
-            CS_DEBUG_BUILTINS_ENVVAR, builtin_name, CS_DEBUG_BUILTINS_NAMES
+            "$%s: ignoring %r, not in cs.debug.__all__:%r",
+            CS_DEBUG_BUILTINS_ENVVAR, builtin_name, __all__
         )
         continue
       if not is_identifier(builtin_name):
         warning(
             "$%s: ignoring %r, not an identifier", CS_DEBUG_BUILTINS_ENVVAR,
             builtin_name
         )
         continue
-      # pylint: disable=eval-used
-      eval('setattr(builtins,builtin_name,%s)' % (builtin_name,))
+      setattr(builtins, builtin_name, vs[builtin_name])
```

### Comparing `cs.debug-20230613.1/lib/python/cs.debug.egg-info/PKG-INFO` & `cs.debug-20240423/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,50 @@
 Metadata-Version: 2.1
 Name: cs.debug
-Version: 20230613.1
+Version: 20240423
 Summary: Assorted debugging facilities.
-Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
-Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted debugging facilities.
 
-*Latest release 20230613.1*:
-Bugfix builtins monkey patch.
+*Latest release 20240423*:
+* Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
+* @trace: include the elapsed time on the return/exception log message.
 
 If the environment variable $CS_DEBUG_BUILTINS is set to a comma
 separated list of names then the `builtins` module will be monkey
 patched with those names, enabling trite debug use of those names
 anywhere in the code provided this module has been imported somewhere.
-The allowed names are the following:
+The allowed names are the list `cs.debug.__all__` and include:
 * `X`: `cs.x.X`
+* `breakpoint`: `cs.upd.breakpoint`
 * `pformat`: `pprint.pformat`
 * `pprint`: `pprint.pprint`
+* `print`: `cs.upd.print`
 * `r`: `cs.lex.r`
+* `redirect_stdout`: `contextlib.redirect_stdout`
 * `s`: `cs.lex.s`
-* `trace`: `cs.debug.trace` (the `@trace` decorator)
-
-## Function `DEBUG(f, force=False)`
-
-Decorator to wrap functions in timing and value debuggers.
-
-## Function `debug_object_shell(o, prompt=None)`
-
-Interactive prompt for inspecting variables.
-
-## Class `DebuggingLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for `threading.Lock` to trace creation and use.
-
-`cs.threads.Lock()` returns one of these in debug mode or a raw
-`threading.Lock` otherwise.
-
-## Class `DebuggingRLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for threading.RLock to trace creation and use.
-
-`cs.threads.RLock()` returns on of these in debug mode or a raw
-`threading.RLock` otherwise.
-
-## Class `DebugShell(cmd.Cmd)`
-
-An interactive prompt for python statements, attached to `/dev/tty` by default.
-
-## Class `DebugWrapper(types.SimpleNamespace)`
-
-Base class for classes presenting debugging wrappers.
-
-## Function `DF(func, *a, **kw)`
-
-Wrapper for a function call to debug its use.
-
-This requires rewriting the call from `f(*a,*kw)` to `DF(f,*a,**kw)`.
-Alternatively one could rewrite as `DEBUG(f)(*a,**kw)`.
-
-## Class `Lock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for `threading.Lock` to trace creation and use.
-
-`cs.threads.Lock()` returns one of these in debug mode or a raw
-`threading.Lock` otherwise.
-
-## Function `openfiles(substr=None, pid=None)`
-
-Run lsof(8) against process `pid`
-returning paths of open files whose paths contain `substr`.
-
-Parameters:
-* `substr`: default substring to select by; default returns all paths.
-* `pid`: process to examine; default from `os.getpid()`.
-
-## Class `RLock(DebugWrapper, types.SimpleNamespace)`
-
-Wrapper class for threading.RLock to trace creation and use.
-
-`cs.threads.RLock()` returns on of these in debug mode or a raw
-`threading.RLock` otherwise.
-
-## Function `selftest(module_name, defaultTest=None, argv=None)`
-
-Called by my unit tests.
+* `stack_dump`: dump current `Thread`'s call stack
+* `thread_dump` dump the active `Thread`s with their call stacks
+* `trace`: the `@trace` decorator
+`$CS_DEBUG_BUILTINS` can also be set to `"1"` to install all of
+`__all__` in the builtins.
 
 ## Function `stack_dump(stack=None, limit=None, logger=None, log_level=None)`
 
 Dump a stack trace to a logger.
 
 Parameters:
 * `stack`: a stack list as returned by `traceback.extract_stack`.
@@ -125,26 +68,22 @@
 
 A `Lock` replacement which times out, used for locating deadlock points.
 
 ## Function `trace(*da, **dkw)`
 
 Decorator to report the call and return of a function.
 
-## Function `trace_caller(func)`
-
-Decorator to report the caller of a function when called.
-
-## Class `TraceSuite`
-
-Context manager to trace start and end of a code suite.
-
 # Release Log
 
 
 
+*Release 20240423*:
+* Support "import *" by populating __all__ with X, r, s, TimingOutLock, thread_dump, stack_dump, trace.
+* @trace: include the elapsed time on the return/exception log message.
+
 *Release 20230613.1*:
 Bugfix builtins monkey patch.
 
 *Release 20230613*:
 Honour $CS_DEBUG_BUILTINS envvar to monkey patch the builtins module, constraints via a white list.
 
 *Release 20230610*:
@@ -181,7 +120,8 @@
 * New openfiles() to return selected pathnames of open files via lsof(8).
 * New selftest() to invoke unittests with benefits.
 * DebugShell, a cmd.Cmd subclass for debugging - current use case calls this with self.__dict__ in a test case tearDwon.
 * debug_object_shell: convenience wrapper for DebugShell to call it on an object's attributes.
 
 *Release 20150116*:
 PyPI prep.
+
```

