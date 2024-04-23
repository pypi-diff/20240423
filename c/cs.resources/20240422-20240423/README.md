# Comparing `tmp/cs.resources-20240422.tar.gz` & `tmp/cs.resources-20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.resources-20240422.tar", last modified: Mon Apr 22 02:52:25 2024, max compression
+gzip compressed data, was "cs.resources-20240423.tar", last modified: Tue Apr 23 09:25:49 2024, max compression
```

## Comparing `cs.resources-20240422.tar` & `cs.resources-20240423.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.693492 cs.resources-20240422/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:51:51.000000 cs.resources-20240422/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    17383 2024-04-22 02:52:25.693095 cs.resources-20240422/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    16626 2024-04-22 02:52:01.000000 cs.resources-20240422/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.686981 cs.resources-20240422/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.687277 cs.resources-20240422/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.689590 cs.resources-20240422/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    27536 2024-04-22 02:51:38.000000 cs.resources-20240422/lib/python/cs/resources.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:52:25.692511 cs.resources-20240422/lib/python/cs.resources.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    17383 2024-04-22 02:52:24.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      210 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:52:25.000000 cs.resources-20240422/lib/python/cs.resources.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    17997 2024-04-22 02:52:23.000000 cs.resources-20240422/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:52:25.693602 cs.resources-20240422/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.160856 cs.resources-20240423/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-23 09:25:18.000000 cs.resources-20240423/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17501 2024-04-23 09:25:49.160427 cs.resources-20240423/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    16744 2024-04-23 09:25:28.000000 cs.resources-20240423/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.153738 cs.resources-20240423/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.154038 cs.resources-20240423/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.156806 cs.resources-20240423/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    27539 2024-04-23 09:25:03.000000 cs.resources-20240423/lib/python/cs/resources.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-23 09:25:49.159916 cs.resources-20240423/lib/python/cs.resources.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17501 2024-04-23 09:25:48.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-04-23 09:25:49.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-23 09:25:48.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      210 2024-04-23 09:25:48.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-23 09:25:49.000000 cs.resources-20240423/lib/python/cs.resources.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18115 2024-04-23 09:25:47.000000 cs.resources-20240423/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-23 09:25:49.160958 cs.resources-20240423/setup.cfg
```

### Comparing `cs.resources-20240422/PKG-INFO` & `cs.resources-20240423/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240422
+Version: 20240423
 Summary: Resource management classes and functions.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20240422*:
-dataclass backport for Python < 3.10.
+*Latest release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -345,15 +345,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -372,14 +372,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
+
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
```

### Comparing `cs.resources-20240422/README.md` & `cs.resources-20240423/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Resource management classes and functions.
 
-*Latest release 20240422*:
-dataclass backport for Python < 3.10.
+*Latest release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -327,15 +327,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -354,14 +354,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
+
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
```

### Comparing `cs.resources-20240422/lib/python/cs/resources.py` & `cs.resources-20240423/lib/python/cs/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from cs.pfx import pfx_call, pfx_method
 from cs.psutils import signal_handlers
 from cs.py.func import prop
 from cs.py.stack import caller, frames as stack_frames, stack_dump, StackSummary
 from cs.result import CancellationError
 from cs.threads import ThreadState, HasThreadState, NRLock
 
-__version__ = '20240422'
+__version__ = '20240423'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -855,15 +855,15 @@
   ''' Mixin to provide convenient access to a `RunState`.
 
       Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
   '''
 
   @uses_runstate
   @typechecked
-  def __init__(self, runstate: Union[RunState, str]):
+  def __init__(self, *, runstate: Union[RunState, str]):
     ''' Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
         Parameters:
         * `runstate`: optional `RunState` instance or name.
           If a `str`, a new `RunState` with that name is allocated.
           If omitted, the default `RunState` is used.
     '''
```

### Comparing `cs.resources-20240422/lib/python/cs.resources.egg-info/PKG-INFO` & `cs.resources-20240423/lib/python/cs.resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240422
+Version: 20240423
 Summary: Resource management classes and functions.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20240422*:
-dataclass backport for Python < 3.10.
+*Latest release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -345,15 +345,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -372,14 +372,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
+
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
```

### Comparing `cs.resources-20240422/pyproject.toml` & `cs.resources-20240423/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,28 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240422"
+version = "20240423"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Resource management classes and functions.
 
-*Latest release 20240422*:
-dataclass backport for Python < 3.10.
+*Latest release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -369,15 +369,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d3c5f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10d9e9f30>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -396,14 +396,17 @@
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
 # Release Log
 
 
 
+*Release 20240423*:
+RunStateMixin: make the optional runstate parameter keyword only.
+
 *Release 20240422*:
 dataclass backport for Python < 3.10.
 
 *Release 20240412*:
 * RunState: new optional thread_wide=False parameter - if true, set this RunState as the Thread-wide default - this mode used by @uses_runstate, unsure about this default.
 * RunState: new .iter(iterable) method which iterates while not RunState.cancelled.
 * MultiOpenMixin: replace __mo_getstate() method with MultiOpenMixin_state property.
```

