# Comparing `tmp/freezegun-1.3.1.tar.gz` & `tmp/freezegun-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freezegun-1.3.1.tar", last modified: Mon Dec  4 19:43:43 2023, max compression
+gzip compressed data, was "freezegun-1.4.0.tar", last modified: Tue Dec 19 10:46:30 2023, max compression
```

## Comparing `freezegun-1.3.1.tar` & `freezegun-1.4.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 19:43:43.426289 freezegun-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-04 19:43:28.000000 freezegun-1.3.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-12-04 19:43:28.000000 freezegun-1.3.1/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2023-12-04 19:43:28.000000 freezegun-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-04 19:43:28.000000 freezegun-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-12-04 19:43:43.426289 freezegun-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10110 2023-12-04 19:43:28.000000 freezegun-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 19:43:43.422289 freezegun-1.3.1/freezegun/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-04 19:43:36.000000 freezegun-1.3.1/freezegun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-04 19:43:28.000000 freezegun-1.3.1/freezegun/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-04 19:43:28.000000 freezegun-1.3.1/freezegun/_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    29302 2023-12-04 19:43:28.000000 freezegun-1.3.1/freezegun/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2023-12-04 19:43:28.000000 freezegun-1.3.1/freezegun/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-04 19:43:28.000000 freezegun-1.3.1/freezegun/config.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 19:43:28.000000 freezegun-1.3.1/freezegun/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 19:43:43.426289 freezegun-1.3.1/freezegun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-12-04 19:43:43.000000 freezegun-1.3.1/freezegun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-04 19:43:43.000000 freezegun-1.3.1/freezegun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 19:43:43.000000 freezegun-1.3.1/freezegun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-04 19:43:43.000000 freezegun-1.3.1/freezegun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-04 19:43:43.000000 freezegun-1.3.1/freezegun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-04 19:43:28.000000 freezegun-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-04 19:43:28.000000 freezegun-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-12-04 19:43:43.426289 freezegun-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-04 19:43:28.000000 freezegun-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 19:43:43.426289 freezegun-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/another_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/fake_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_class_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)    27795 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_datetimes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_import_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_sqlite3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_ticking.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-04 19:43:28.000000 freezegun-1.3.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-04 19:43:28.000000 freezegun-1.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.612686 freezegun-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-19 10:46:15.000000 freezegun-1.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-12-19 10:46:15.000000 freezegun-1.4.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2023-12-19 10:46:15.000000 freezegun-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-19 10:46:15.000000 freezegun-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-12-19 10:46:30.612686 freezegun-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10110 2023-12-19 10:46:15.000000 freezegun-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.608686 freezegun-1.4.0/freezegun/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2023-12-19 10:46:24.000000 freezegun-1.4.0/freezegun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29579 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:15.000000 freezegun-1.4.0/freezegun/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.612686 freezegun-1.4.0/freezegun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-19 10:46:30.000000 freezegun-1.4.0/freezegun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-19 10:46:15.000000 freezegun-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-19 10:46:15.000000 freezegun-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-12-19 10:46:30.616685 freezegun-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-19 10:46:15.000000 freezegun-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:30.612686 freezegun-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/another_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/fake_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_class_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27795 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_import_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_sqlite3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_ticking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-19 10:46:15.000000 freezegun-1.4.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-12-19 10:46:15.000000 freezegun-1.4.0/tox.ini
```

### Comparing `freezegun-1.3.1/AUTHORS.rst` & `freezegun-1.4.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/CHANGELOG` & `freezegun-1.4.0/CHANGELOG`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Freezegun Changelog
 ===================
 
+1.4.0
+-----
+ * `asyncio`-support from 1.3.x introduced quite a few  bugs, so that functionality is now hidden behind a flag:
+   `with freeze_time('1970-01-02', real_asyncio=True):`
+
+1.3.1
+-----
+ * Fixed the release number in the build
+
 1.3.0
 -----
 
 * Fixed `asyncio` support to avoid `await asyncio.sleep(1)` hanging forever.
 
 * Added support for Python 3.12
```

### Comparing `freezegun-1.3.1/LICENSE` & `freezegun-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/PKG-INFO` & `freezegun-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freezegun
-Version: 1.3.1
+Version: 1.4.0
 Summary: Let your Python tests travel through time
 Home-page: https://github.com/spulec/freezegun
 Author: Steve Pulec
 Author-email: spulec@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/spulec/freezegun/issues
 Project-URL: Changes, https://github.com/spulec/freezegun/blob/master/CHANGELOG
```

### Comparing `freezegun-1.3.1/README.rst` & `freezegun-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/freezegun/_async.py` & `freezegun-1.4.0/freezegun/_async.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/freezegun/api.py` & `freezegun-1.4.0/freezegun/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,24 +540,25 @@
         target_datetime = _parse_time_to_freeze(target_datetime)
         delta = target_datetime - self.time_to_freeze
         self.tick(delta=delta)
 
 
 class _freeze_time:
 
-    def __init__(self, time_to_freeze_str, tz_offset, ignore, tick, as_arg, as_kwarg, auto_tick_seconds):
+    def __init__(self, time_to_freeze_str, tz_offset, ignore, tick, as_arg, as_kwarg, auto_tick_seconds, real_asyncio):
         self.time_to_freeze = _parse_time_to_freeze(time_to_freeze_str)
         self.tz_offset = _parse_tz_offset(tz_offset)
         self.ignore = tuple(ignore)
         self.tick = tick
         self.auto_tick_seconds = auto_tick_seconds
         self.undo_changes = []
         self.modules_at_start = set()
         self.as_arg = as_arg
         self.as_kwarg = as_kwarg
+        self.real_asyncio = real_asyncio
 
     def __call__(self, func):
         if inspect.isclass(func):
             return self.decorate_class(func)
         elif inspect.iscoroutinefunction(func):
             return self.decorate_coroutine(func)
         return self.decorate_callable(func)
@@ -723,28 +724,29 @@
                 module_attrs = _get_cached_module_attributes(module)
                 for attribute_name, attribute_value in module_attrs:
                     fake = fakes.get(id(attribute_value))
                     if fake:
                         setattr(module, attribute_name, fake)
                         add_change((module, attribute_name, attribute_value))
 
-        # To avoid breaking `asyncio.sleep()`, let asyncio event loops see real
-        # monotonic time even though we've just frozen `time.monotonic()` which
-        # is normally used there. If we didn't do this, `await asyncio.sleep()`
-        # would be hanging forever breaking many tests that use `freeze_time`.
-        #
-        # Note that we cannot statically tell the class of asyncio event loops
-        # because it is not officially documented and can actually be changed
-        # at run time using `asyncio.set_event_loop_policy`. That's why we check
-        # the type by creating a loop here and destroying it immediately.
-        event_loop = asyncio.new_event_loop()
-        event_loop.close()
-        EventLoopClass = type(event_loop)
-        add_change((EventLoopClass, "time", EventLoopClass.time))
-        EventLoopClass.time = lambda self: real_monotonic()
+        if self.real_asyncio:
+            # To avoid breaking `asyncio.sleep()`, let asyncio event loops see real
+            # monotonic time even though we've just frozen `time.monotonic()` which
+            # is normally used there. If we didn't do this, `await asyncio.sleep()`
+            # would be hanging forever breaking many tests that use `freeze_time`.
+            #
+            # Note that we cannot statically tell the class of asyncio event loops
+            # because it is not officially documented and can actually be changed
+            # at run time using `asyncio.set_event_loop_policy`. That's why we check
+            # the type by creating a loop here and destroying it immediately.
+            event_loop = asyncio.new_event_loop()
+            event_loop.close()
+            EventLoopClass = type(event_loop)
+            add_change((EventLoopClass, "time", EventLoopClass.time))
+            EventLoopClass.time = lambda self: real_monotonic()
 
         return freeze_factory
 
     def stop(self):
         freeze_factories.pop()
         ignore_lists.pop()
         tick_flags.pop()
@@ -826,37 +828,37 @@
             return result
         functools.update_wrapper(wrapper, func)
 
         return wrapper
 
 
 def freeze_time(time_to_freeze=None, tz_offset=0, ignore=None, tick=False, as_arg=False, as_kwarg='',
-                auto_tick_seconds=0):
+                auto_tick_seconds=0, real_asyncio=False):
     acceptable_times = (type(None), str, datetime.date, datetime.timedelta,
              types.FunctionType, types.GeneratorType)
 
     if MayaDT is not None:
         acceptable_times += MayaDT,
 
     if not isinstance(time_to_freeze, acceptable_times):
         raise TypeError(('freeze_time() expected None, a string, date instance, datetime '
                          'instance, MayaDT, timedelta instance, function or a generator, but got '
                          'type {}.').format(type(time_to_freeze)))
     if tick and not _is_cpython:
         raise SystemError('Calling freeze_time with tick=True is only compatible with CPython')
 
     if isinstance(time_to_freeze, types.FunctionType):
-        return freeze_time(time_to_freeze(), tz_offset, ignore, tick, as_arg, as_kwarg, auto_tick_seconds)
+        return freeze_time(time_to_freeze(), tz_offset, ignore, tick, as_arg, as_kwarg, auto_tick_seconds, real_asyncio=real_asyncio)
 
     if isinstance(time_to_freeze, types.GeneratorType):
-        return freeze_time(next(time_to_freeze), tz_offset, ignore, tick, as_arg, as_kwarg, auto_tick_seconds)
+        return freeze_time(next(time_to_freeze), tz_offset, ignore, tick, as_arg, as_kwarg, auto_tick_seconds, real_asyncio=real_asyncio)
 
     if MayaDT is not None and isinstance(time_to_freeze, MayaDT):
         return freeze_time(time_to_freeze.datetime(), tz_offset, ignore,
-                           tick, as_arg, as_kwarg, auto_tick_seconds)
+                           tick, as_arg, as_kwarg, auto_tick_seconds, real_asyncio=real_asyncio)
 
     if ignore is None:
         ignore = []
     ignore = ignore[:]
     if config.settings.default_ignore_list:
         ignore.extend(config.settings.default_ignore_list)
 
@@ -864,14 +866,15 @@
         time_to_freeze_str=time_to_freeze,
         tz_offset=tz_offset,
         ignore=ignore,
         tick=tick,
         as_arg=as_arg,
         as_kwarg=as_kwarg,
         auto_tick_seconds=auto_tick_seconds,
+        real_asyncio=real_asyncio,
     )
 
 
 # Setup adapters for sqlite
 try:
     # noinspection PyUnresolvedReferences
     import sqlite3
```

### Comparing `freezegun-1.3.1/freezegun/api.pyi` & `freezegun-1.4.0/freezegun/api.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         time_to_freeze_str: _Freezable | None,
         tz_offset: int | timedelta,
         ignore: Sequence[str],
         tick: bool,
         as_arg: bool,
         as_kwarg: str,
         auto_tick_seconds: float,
+        real_asyncio: bool,
     ) -> None: ...
     @overload
     def __call__(self, func: type[_T]) -> type[_T]: ...
     @overload
     def __call__(self, func: Callable[..., Awaitable[_T]]) -> Callable[..., Awaitable[_T]]: ...
     @overload
     def __call__(self, func: Callable[..., _T]) -> Callable[..., _T]: ...
@@ -53,8 +54,9 @@
     time_to_freeze: _Freezable | Callable[..., _Freezable] | Iterator[_Freezable] | None = ...,
     tz_offset: int | timedelta | None = ...,
     ignore: Sequence[str] | None = ...,
     tick: bool | None = ...,
     as_arg: bool | None = ...,
     as_kwarg: str | None = ...,
     auto_tick_seconds: float | None = ...,
+    real_asyncio: bool | None = ...
 ) -> _freeze_time: ...
```

### Comparing `freezegun-1.3.1/freezegun/config.py` & `freezegun-1.4.0/freezegun/config.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/freezegun.egg-info/PKG-INFO` & `freezegun-1.4.0/freezegun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freezegun
-Version: 1.3.1
+Version: 1.4.0
 Summary: Let your Python tests travel through time
 Home-page: https://github.com/spulec/freezegun
 Author: Steve Pulec
 Author-email: spulec@gmail.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/spulec/freezegun/issues
 Project-URL: Changes, https://github.com/spulec/freezegun/blob/master/CHANGELOG
```

### Comparing `freezegun-1.3.1/freezegun.egg-info/SOURCES.txt` & `freezegun-1.4.0/freezegun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/setup.cfg` & `freezegun-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/another_module.py` & `freezegun-1.4.0/tests/another_module.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/fake_module.py` & `freezegun-1.4.0/tests/fake_module.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_asyncio.py` & `freezegun-1.4.0/tests/test_asyncio.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     the asyncio event loop can see real monotonic time, which is required
     to make things like `asyncio.sleep()` work.
     """
 
     async def coroutine():
         # Sleeping with time frozen should sleep the expected duration.
         before_sleep = time.time()
-        with freeze_time('1970-01-02'):
+        with freeze_time('1970-01-02', real_asyncio=True):
             await asyncio.sleep(0.05)
         assert 0.02 <= time.time() - before_sleep < 0.3
 
         # Exiting `freeze_time` the time should not break asyncio sleeping.
         before_sleep = time.time()
         await asyncio.sleep(0.05)
         assert 0.02 <= time.time() - before_sleep < 0.3
@@ -72,9 +72,9 @@
         assert timestamps == []
 
         # But sleeping more (150 ms in this case) should call `to_call_later`
         # and we should see `timestamps` updated.
         await asyncio.sleep(0.15)
         assert timestamps == [86400]
 
-    with freeze_time('1970-01-02'):
+    with freeze_time('1970-01-02', real_asyncio=True):
         asyncio.run(coroutine())
```

### Comparing `freezegun-1.3.1/tests/test_class_import.py` & `freezegun-1.4.0/tests/test_class_import.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_configure.py` & `freezegun-1.4.0/tests/test_configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             time_to_freeze_str="2020-10-06",
             tz_offset=0,
             ignore=expected_ignore_list,
             tick=False,
             as_arg=False,
             as_kwarg='',
             auto_tick_seconds=0,
+            real_asyncio=False,
         )
 
 def test_extend_default_ignore_list():
     freezegun.configure(extend_ignore_list=['tensorflow'])
 
     with mock.patch("freezegun.api._freeze_time.__init__", return_value=None) as _freeze_time_init_mock:
 
@@ -60,8 +61,9 @@
             time_to_freeze_str="2020-10-06",
             tz_offset=0,
             ignore=expected_ignore_list,
             tick=False,
             as_arg=False,
             as_kwarg='',
             auto_tick_seconds=0,
+            real_asyncio=False,
         )
```

### Comparing `freezegun-1.3.1/tests/test_datetimes.py` & `freezegun-1.4.0/tests/test_datetimes.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_errors.py` & `freezegun-1.4.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_import_alias.py` & `freezegun-1.4.0/tests/test_import_alias.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_operations.py` & `freezegun-1.4.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_pickle.py` & `freezegun-1.4.0/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_ticking.py` & `freezegun-1.4.0/tests/test_ticking.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_utils.py` & `freezegun-1.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_uuid.py` & `freezegun-1.4.0/tests/test_uuid.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/test_warnings.py` & `freezegun-1.4.0/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `freezegun-1.3.1/tests/utils.py` & `freezegun-1.4.0/tests/utils.py`

 * *Files identical despite different names*

