# Comparing `tmp/aiomultiprocess-0.9.0.tar.gz` & `tmp/aiomultiprocess-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomultiprocess-0.9.0.tar", last modified: Mon Mar  1 01:18:59 2021, max compression
+gzip compressed data, was "aiomultiprocess-0.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiomultiprocess-0.9.0.tar` & `aiomultiprocess-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,36 @@
--rw-r--r--   0        0        0     1183 2020-11-18 18:50:10.608456 aiomultiprocess-0.9.0/.gitignore
--rw-r--r--   0        0        0    16637 2020-11-18 18:50:10.608632 aiomultiprocess-0.9.0/.pylint
--rw-r--r--   0        0        0       76 2020-11-18 18:50:10.608722 aiomultiprocess-0.9.0/.pyup.yml
--rw-r--r--   0        0        0      156 2020-11-18 18:50:10.608791 aiomultiprocess-0.9.0/.readthedocs.yml
--rw-r--r--   0        0        0     2557 2021-03-01 01:06:09.900939 aiomultiprocess-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     3212 2020-11-18 18:50:10.608986 aiomultiprocess-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      940 2020-11-18 18:50:10.609063 aiomultiprocess-0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1067 2020-11-18 18:50:10.609134 aiomultiprocess-0.9.0/LICENSE
--rw-r--r--   0        0        0       26 2020-11-18 18:50:10.609200 aiomultiprocess-0.9.0/MANIFEST.in
--rw-r--r--   0        0        0     3533 2020-11-18 18:50:10.609289 aiomultiprocess-0.9.0/README.md
--rw-r--r--   0        0        0      370 2021-02-28 23:34:32.436683 aiomultiprocess-0.9.0/aiomultiprocess/__init__.py
--rw-r--r--   0        0        0       22 2021-03-01 01:06:09.908857 aiomultiprocess-0.9.0/aiomultiprocess/__version__.py
--rw-r--r--   0        0        0     7835 2021-02-28 23:34:32.471127 aiomultiprocess-0.9.0/aiomultiprocess/core.py
--rw-r--r--   0        0        0    11688 2021-02-28 23:34:32.556459 aiomultiprocess-0.9.0/aiomultiprocess/pool.py
--rw-r--r--   0        0        0     2573 2021-02-28 23:34:32.489242 aiomultiprocess-0.9.0/aiomultiprocess/scheduler.py
--rw-r--r--   0        0        0      267 2021-02-28 23:34:32.572259 aiomultiprocess-0.9.0/aiomultiprocess/tests/__init__.py
--rw-r--r--   0        0        0      189 2021-02-28 23:34:32.662249 aiomultiprocess-0.9.0/aiomultiprocess/tests/__main__.py
--rw-r--r--   0        0        0     1245 2021-02-28 23:34:32.671175 aiomultiprocess-0.9.0/aiomultiprocess/tests/base.py
--rw-r--r--   0        0        0     6589 2021-02-28 23:34:32.613947 aiomultiprocess-0.9.0/aiomultiprocess/tests/core.py
--rw-r--r--   0        0        0     1611 2021-02-28 23:34:32.570457 aiomultiprocess-0.9.0/aiomultiprocess/tests/perf.py
--rw-r--r--   0        0        0     5957 2021-02-28 23:34:32.660887 aiomultiprocess-0.9.0/aiomultiprocess/tests/pool.py
--rw-r--r--   0        0        0      887 2021-02-28 23:34:32.620242 aiomultiprocess-0.9.0/aiomultiprocess/tests/scheduler.py
--rw-r--r--   0        0        0     1037 2021-02-28 23:34:32.478869 aiomultiprocess-0.9.0/aiomultiprocess/types.py
--rw-r--r--   0        0        0      320 2020-11-18 18:50:10.610587 aiomultiprocess-0.9.0/docs/_static/custom.css
--rw-r--r--   0        0        0      342 2020-11-18 18:50:10.610677 aiomultiprocess-0.9.0/docs/_templates/badges.html
--rw-r--r--   0        0        0      934 2020-11-18 18:50:10.610753 aiomultiprocess-0.9.0/docs/_templates/omnilib.html
--rw-r--r--   0        0        0      460 2020-11-18 18:50:10.610813 aiomultiprocess-0.9.0/docs/api.rst
--rw-r--r--   0        0        0       70 2020-11-18 18:50:10.610868 aiomultiprocess-0.9.0/docs/changelog.rst
--rw-r--r--   0        0        0     2810 2021-02-28 22:55:00.543307 aiomultiprocess-0.9.0/docs/conf.py
--rw-r--r--   0        0        0       79 2020-11-18 18:50:10.610997 aiomultiprocess-0.9.0/docs/contributing.rst
--rw-r--r--   0        0        0    10211 2021-02-28 23:30:20.742651 aiomultiprocess-0.9.0/docs/guide.rst
--rw-r--r--   0        0        0      221 2020-11-18 18:50:10.611201 aiomultiprocess-0.9.0/docs/index.rst
--rw-r--r--   0        0        0      922 2021-03-01 00:06:54.028360 aiomultiprocess-0.9.0/makefile
--rw-r--r--   0        0        0       37 2021-02-28 23:37:19.231601 aiomultiprocess-0.9.0/mypy.ini
--rw-r--r--   0        0        0     1059 2021-03-01 00:06:54.028740 aiomultiprocess-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      286 2021-02-28 23:41:11.955402 aiomultiprocess-0.9.0/requirements-dev.txt
--rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 aiomultiprocess-0.9.0/setup.py
--rw-r--r--   0        0        0      219 1970-01-01 00:00:00.000000 aiomultiprocess-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      171 2024-04-23 06:00:51.943004 aiomultiprocess-0.9.1/.flake8
+-rw-r--r--   0        0        0     1183 2024-04-23 06:00:51.943635 aiomultiprocess-0.9.1/.gitignore
+-rw-r--r--   0        0        0       50 2024-04-23 06:00:51.943722 aiomultiprocess-0.9.1/.mailmap
+-rw-r--r--   0        0        0      209 2024-04-23 07:42:45.273178 aiomultiprocess-0.9.1/.readthedocs.yml
+-rw-r--r--   0        0        0     3091 2024-04-23 08:16:28.980892 aiomultiprocess-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3216 2024-04-23 06:00:51.944046 aiomultiprocess-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      940 2024-04-23 06:00:51.944139 aiomultiprocess-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1066 2024-04-23 07:42:45.273458 aiomultiprocess-0.9.1/LICENSE
+-rw-r--r--   0        0        0       26 2024-04-23 06:00:51.944338 aiomultiprocess-0.9.1/MANIFEST.in
+-rw-r--r--   0        0        0     3543 2024-04-23 06:00:51.944443 aiomultiprocess-0.9.1/README.md
+-rw-r--r--   0        0        0      378 2024-04-23 06:00:51.944600 aiomultiprocess-0.9.1/aiomultiprocess/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-23 08:16:28.990043 aiomultiprocess-0.9.1/aiomultiprocess/__version__.py
+-rw-r--r--   0        0        0     8091 2024-04-23 08:08:01.535888 aiomultiprocess-0.9.1/aiomultiprocess/core.py
+-rw-r--r--   0        0        0    11756 2024-04-23 08:08:01.536217 aiomultiprocess-0.9.1/aiomultiprocess/pool.py
+-rw-r--r--   0        0        0     2577 2024-04-23 06:00:51.945096 aiomultiprocess-0.9.1/aiomultiprocess/scheduler.py
+-rw-r--r--   0        0        0      271 2024-04-23 06:00:51.945248 aiomultiprocess-0.9.1/aiomultiprocess/tests/__init__.py
+-rw-r--r--   0        0        0      193 2024-04-23 06:00:51.945354 aiomultiprocess-0.9.1/aiomultiprocess/tests/__main__.py
+-rw-r--r--   0        0        0     1241 2024-04-23 06:00:51.945468 aiomultiprocess-0.9.1/aiomultiprocess/tests/base.py
+-rw-r--r--   0        0        0     6550 2024-04-23 06:00:51.945595 aiomultiprocess-0.9.1/aiomultiprocess/tests/core.py
+-rw-r--r--   0        0        0     1615 2024-04-23 06:00:51.945709 aiomultiprocess-0.9.1/aiomultiprocess/tests/perf.py
+-rw-r--r--   0        0        0     5863 2024-04-23 06:00:51.945854 aiomultiprocess-0.9.1/aiomultiprocess/tests/pool.py
+-rw-r--r--   0        0        0      891 2024-04-23 06:00:51.945950 aiomultiprocess-0.9.1/aiomultiprocess/tests/scheduler.py
+-rw-r--r--   0        0        0     1041 2024-04-23 07:38:07.528582 aiomultiprocess-0.9.1/aiomultiprocess/types.py
+-rw-r--r--   0        0        0      320 2024-04-23 06:00:51.946254 aiomultiprocess-0.9.1/docs/_static/custom.css
+-rw-r--r--   0        0        0      342 2024-04-23 06:00:51.946402 aiomultiprocess-0.9.1/docs/_templates/badges.html
+-rw-r--r--   0        0        0      934 2024-04-23 06:00:51.946502 aiomultiprocess-0.9.1/docs/_templates/omnilib.html
+-rw-r--r--   0        0        0      460 2024-04-23 06:00:51.946593 aiomultiprocess-0.9.1/docs/api.rst
+-rw-r--r--   0        0        0       70 2024-04-23 06:00:51.946673 aiomultiprocess-0.9.1/docs/changelog.rst
+-rw-r--r--   0        0        0     2830 2024-04-23 06:00:51.946773 aiomultiprocess-0.9.1/docs/conf.py
+-rw-r--r--   0        0        0       79 2024-04-23 06:00:51.946854 aiomultiprocess-0.9.1/docs/contributing.rst
+-rw-r--r--   0        0        0    10215 2024-04-23 06:00:51.947001 aiomultiprocess-0.9.1/docs/guide.rst
+-rw-r--r--   0        0        0      221 2024-04-23 06:00:51.947095 aiomultiprocess-0.9.1/docs/index.rst
+-rw-r--r--   0        0        0      883 2024-04-23 07:42:45.274389 aiomultiprocess-0.9.1/makefile
+-rw-r--r--   0        0        0       37 2024-04-23 06:00:51.947294 aiomultiprocess-0.9.1/mypy.ini
+-rw-r--r--   0        0        0     1401 2024-04-23 08:10:12.885881 aiomultiprocess-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     4751 1970-01-01 00:00:00.000000 aiomultiprocess-0.9.1/PKG-INFO
```

### Comparing `aiomultiprocess-0.9.0/.gitignore` & `aiomultiprocess-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiomultiprocess-0.9.0/CHANGELOG.md` & `aiomultiprocess-0.9.1/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,61 @@
 aiomultiprocess
 ===============
 
+[![Generated by attribution][attribution-badge]][attribution-url]
+
+
+v0.9.1
+------
+
+Maintenance release
+
+- Tested up to Python 3.12 (#195)
+- Dropped support for Python 3.7 and 3.6 (#195)
+- Updated project metadata (#93, #195)
+- Updated type hints
+
+```text
+$ git shortlog -s v0.9.0...v0.9.1
+    16	Amethyst Reese
+    33	dependabot[bot]
+     5	pyup.io bot
+```
+
+
 v0.9.0
 ------
 
 Feature release
 
 * Added uncaught exception handler for pool workers (#80, #82)
 * Fixed testing on Windows/Python 3.8 (#73)
 * Support for Python 3.9 (#83, #85)
 
-```
+```text
 $ git shortlog -s v0.8.0...v0.9.0
+    15	Amethyst Reese
      5	Dmitriy Ferens
-    15	John Reese
      1	Pranab
      4	pyup.io bot
 ```
 
 
 v0.8.0
 ------
 
 Feature release
 
 - Pool.map/starmap can now be used in `async for` loops (#48)
 - Added support for alternate event loops and uvloop (#50)
 - Updated documentation, with a new user guide
 
-```
+```text
 $ git shortlog -s v0.7.0...v0.8.0
-    14	John Reese
+    14	Amethyst Reese
      1	Thomas Grainger
 ```
 
 
 v0.7.0
 ------
 
@@ -44,106 +65,109 @@
 - Use sharded work/result queues for Pools, using round robin
   by default, with option to provide a custom scheduler
 - Initializers now run after creating the event loop
 - Full support for Python 3.8 and Windows
 - Major refactoring and splitting of internals
 - 100% test coverage
 
-```
+```text
 $ git shortlog -s v0.6.1...v0.7.0
+    17	Amethyst Reese
     12	Daniel Ip
      1	HJK
-    17	John Reese
 ```
 
 
 v0.6.1
 ------
 
 Minor release v0.6.1
 
 - Better exception handling/proxying from child process (#27)
 - Improved test coverage (#29)
 
-```
+```text
 $ git shortlog -s v0.6.0...v0.6.1
+     6	Amethyst Reese
      9	Daniel Ip
-     6	John Reese
 ```
 
 
 v0.6.0
 ------
 
 Feature release v0.6.0
 
 - Enable passing initializer functions/args to process pools (#23)
 - `kill()` and `close()` are only available on Python 3.7+
 - Added correct Python version requirements to package metadata
 - Bundled unit tests inside module for distrtibution
 
-```
+```text
 $ git shortlog -s v0.5.0...v0.6.0
+    18	Amethyst Reese
      1	Daniel Ip
-    18	John Reese
 ```
 
 
 v0.5.0
 ------
 
 Feature release v0.5.0:
 
 - Support Windows
 - Support "spawn" contexts on all platforms
 - Allow changing the multiprocessing context at runtime
 - Better support for features in Python 3.7
 
-```
+```text
 $ git shortlog -s v0.4.0...v0.5.0
-    15	John Reese
+    15	Amethyst Reese
      1	smheidrich
      1	x1ah
 ```
 
 
 v0.4.0
 ------
 
 Feature release v0.4.0:
 
 - Allow awaiting Process objects directly to start/join child process
 - Worker objects return final result from await/join
 - Better unit testing, types, and documentation
 
-```
+```text
 $ git shortlog -s v0.3.0...v0.4.0
-    12	John Reese
+    12	Amethyst Reese
 ```
 
 
 v0.3.0
 ------
 
 Feature release:
 
 - enable multiple coroutines per child process
 - perf testing
 
-```
+```text
 $ git shortlog -s v0.2.0...v0.3.0
-    10	John Reese
+    10	Amethyst Reese
 ```
 
 
 v0.2.0
 ------
 
 Feature release:
 
 - Run coroutines on child process or process pool
 
-```
-$ git shortlog -s d58104b244a984f37d2f672431b4a2fc7e74931b...v0.2.0
-     1	John Reese
+```text
+$ git shortlog -s v0.2.0
+    12	Amethyst Reese
 ```
 
+[attribution-badge]:
+    https://img.shields.io/badge/generated%20by-attribution-informational
+[attribution-url]: https://attribution.omnilib.dev
```

### Comparing `aiomultiprocess-0.9.0/CODE_OF_CONDUCT.md` & `aiomultiprocess-0.9.1/CODE_OF_CONDUCT.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 ## Scope
 
 This Code of Conduct applies both within project spaces and in public spaces when an individual is representing the project or its community. Examples of representing a project or community include using an official project e-mail address, posting via an official social media account, or acting as an appointed representative at an online or offline event. Representation of a project may be further defined and clarified by project maintainers.
 
 ## Enforcement
 
-Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at john@noswap.com. The project team will review and investigate all complaints, and will respond in a way that it deems appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the reporter of an incident. Further details of specific enforcement policies may be posted separately.
+Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at contact@omnilib.dev. The project team will review and investigate all complaints, and will respond in a way that it deems appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the reporter of an incident. Further details of specific enforcement policies may be posted separately.
 
 Project maintainers who do not follow or enforce the Code of Conduct in good faith may face temporary or permanent repercussions as determined by other members of the project's leadership.
 
 ## Attribution
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4, available at [http://contributor-covenant.org/version/1/4][version]
```

### Comparing `aiomultiprocess-0.9.0/CONTRIBUTING.md` & `aiomultiprocess-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiomultiprocess-0.9.0/README.md` & `aiomultiprocess-0.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 from aiomultiprocess import Pool
 
 async def get(url):
     async with request("GET", url) as response:
         return await response.text("utf-8")
 
 async def main():
-    urls = ["https://jreese.sh", ...]
+    urls = ["https://noswap.com", ...]
     async with Pool() as pool:
         async for result in pool.map(get, urls):
             ...  # process result
             
 if __name__ == '__main__':
     # Python 3.7
     asyncio.run(main())
@@ -71,23 +71,23 @@
 ```
 
 Take a look at the [User Guide][] for more details and examples.
 
 For further context, watch the PyCon US 2018 talk about aiomultiprocess,
 ["Thinking Outside the GIL"][pycon-2018]:
 
-> [![IMAGE ALT TEXT](http://img.youtube.com/vi/0kXaLh8Fz3k/0.jpg)](http://www.youtube.com/watch?v=0kXaLh8Fz3k "PyCon 2018 - John Reese - Thinking Outside the GIL with AsyncIO and Multiprocessing")
+> [![IMAGE ALT TEXT](http://img.youtube.com/vi/0kXaLh8Fz3k/0.jpg)](http://www.youtube.com/watch?v=0kXaLh8Fz3k "PyCon 2018 - Amethyst Reese - Thinking Outside the GIL with AsyncIO and Multiprocessing")
 
 Slides available at [Speaker Deck](https://speakerdeck.com/jreese/thinking-outside-the-gil-2).
 
 
 License
 -------
 
-aiomultiprocess is copyright [John Reese](https://jreese.sh), and licensed under
+aiomultiprocess is copyright [Amethyst Reese](https://noswap.com), and licensed under
 the MIT license.  I am providing code in this repository to you under an open
 source license.  This is my personal repository; the license you receive to
 my code is from me and not from my employer. See the `LICENSE` file for details.
 
 
 [User Guide]: https://aiomultiprocess.omnilib.dev/en/latest/guide.html
 [pycon-2018]: https://www.youtube.com/watch?v=0kXaLh8Fz3k
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/core.py` & `aiomultiprocess-0.9.1/aiomultiprocess/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-# Copyright 2018 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import asyncio
 import logging
 import multiprocessing
+import multiprocessing.context
 import multiprocessing.managers
 import os
 import sys
 from typing import Any, Callable, Dict, Optional, Sequence
 
 from .types import Context, R, Unit
 
 DEFAULT_START_METHOD = "spawn"
 
 # shared context for all multiprocessing primitives, for platform compatibility
 # "spawn" is default/required on windows and mac, but can't execute non-global functions
 # see https://docs.python.org/3/library/multiprocessing.html#contexts-and-start-methods
-context = multiprocessing.get_context(DEFAULT_START_METHOD)
+context: multiprocessing.context.BaseContext = multiprocessing.get_context(
+    DEFAULT_START_METHOD
+)
 _manager = None
 
 log = logging.getLogger(__name__)
 
 
 def get_manager() -> multiprocessing.managers.SyncManager:
     """Return a singleton shared manager."""
@@ -76,20 +79,20 @@
 
 class Process:
     """Execute a coroutine on a separate process."""
 
     def __init__(
         self,
         group: None = None,
-        target: Callable = None,
-        name: str = None,
-        args: Sequence[Any] = None,
-        kwargs: Dict[str, Any] = None,
+        target: Optional[Callable] = None,
+        name: Optional[str] = None,
+        args: Optional[Sequence[Any]] = None,
+        kwargs: Optional[Dict[str, Any]] = None,
         *,
-        daemon: bool = None,
+        daemon: Optional[bool] = None,
         initializer: Optional[Callable] = None,
         initargs: Sequence[Any] = (),
         loop_initializer: Optional[Callable] = None,
         process_target: Optional[Callable] = None,
     ) -> None:
         if target is not None and not asyncio.iscoroutinefunction(target):
             raise ValueError("target must be coroutine function")
@@ -107,15 +110,15 @@
             args=args or (),
             kwargs=kwargs or {},
             namespace=get_manager().Namespace(),
             initializer=initializer,
             initargs=initargs,
             loop_initializer=loop_initializer,
         )
-        self.aio_process = context.Process(
+        self.aio_process = context.Process(  # type: ignore[attr-defined]
             group=group,
             target=process_target or Process.run_async,
             args=(self.unit,),
             name=name,
             daemon=daemon,
         )
 
@@ -123,15 +126,15 @@
         """Enable awaiting of the process result by chaining to `start()` & `join()`."""
         if not self.is_alive() and self.exitcode is None:
             self.start()
 
         return self.join().__await__()
 
     @staticmethod
-    def run_async(unit: Unit) -> R:
+    def run_async(unit: Unit) -> R:  # type: ignore[type-var]
         """Initialize the child process and event loop, then execute the coroutine."""
         try:
             if unit.loop_initializer is None:
                 loop = asyncio.new_event_loop()
             else:
                 loop = unit.loop_initializer()
 
@@ -148,15 +151,15 @@
             log.exception(f"aio process {os.getpid()} failed")
             raise
 
     def start(self) -> None:
         """Start the child process."""
         return self.aio_process.start()
 
-    async def join(self, timeout: int = None) -> None:
+    async def join(self, timeout: Optional[int] = None) -> None:
         """Wait for the process to finish execution without blocking the main thread."""
         if not self.is_alive() and self.exitcode is None:
             raise ValueError("must start process before joining it")
 
         if timeout is not None:
             return await asyncio.wait_for(self.join(), timeout)
 
@@ -212,30 +215,30 @@
     """Execute a coroutine on a separate process and return the result."""
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, process_target=Worker.run_async, **kwargs)
         self.unit.namespace.result = None
 
     @staticmethod
-    def run_async(unit: Unit) -> R:
+    def run_async(unit: Unit) -> R:  # type: ignore[type-var]
         """Initialize the child process and event loop, then execute the coroutine."""
         try:
             result: R = Process.run_async(unit)
             unit.namespace.result = result
             return result
 
         except BaseException as e:
             unit.namespace.result = e
             raise
 
-    async def join(self, timeout: int = None) -> Any:
+    async def join(self, timeout: Optional[int] = None) -> Any:
         """Wait for the worker to finish, and return the final result."""
         await super().join(timeout)
         return self.result
 
     @property
-    def result(self) -> R:
+    def result(self) -> R:  # type: ignore[type-var]
         """Easy access to the resulting value from the coroutine."""
         if self.exitcode is None:
             raise ValueError("coroutine not completed")
 
         return self.unit.namespace.result
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/pool.py` & `aiomultiprocess-0.9.1/aiomultiprocess/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import asyncio
 import logging
 import os
 import queue
 import traceback
@@ -16,15 +16,15 @@
     Generator,
     Optional,
     Sequence,
     Tuple,
     TypeVar,
 )
 
-from .core import Process, get_context
+from .core import get_context, Process
 from .scheduler import RoundRobin, Scheduler
 from .types import (
     LoopInitializer,
     PoolTask,
     ProxyException,
     Queue,
     QueueID,
@@ -104,15 +104,15 @@
             for future in done:
                 tid = pending.pop(future)
 
                 result = None
                 tb = None
                 try:
                     result = future.result()
-                except BaseException as e:
+                except BaseException as e:  # noqa: B036
                     if self.exception_handler is not None:
                         self.exception_handler(e)
 
                     tb = traceback.format_exc()
 
                 self.rx.put_nowait((tid, result, tb))
                 completed += 1
@@ -146,21 +146,21 @@
 
 
 class Pool:
     """Execute coroutines on a pool of child processes."""
 
     def __init__(
         self,
-        processes: int = None,
-        initializer: Callable[..., None] = None,
+        processes: Optional[int] = None,
+        initializer: Optional[Callable[..., None]] = None,
         initargs: Sequence[Any] = (),
         maxtasksperchild: int = MAX_TASKS_PER_CHILD,
         childconcurrency: int = CHILD_CONCURRENCY,
         queuecount: Optional[int] = None,
-        scheduler: Scheduler = None,
+        scheduler: Optional[Scheduler] = None,
         loop_initializer: Optional[LoopInitializer] = None,
         exception_handler: Optional[Callable[[BaseException], None]] = None,
     ) -> None:
         self.context = get_context()
 
         self.scheduler = scheduler or RoundRobin()
         self.process_count = max(1, processes or os.cpu_count() or 2)
@@ -312,16 +312,16 @@
             await asyncio.sleep(0.005)
 
         return [ready[tid] for tid in tids]
 
     async def apply(
         self,
         func: Callable[..., Awaitable[R]],
-        args: Sequence[Any] = None,
-        kwds: Dict[str, Any] = None,
+        args: Optional[Sequence[Any]] = None,
+        kwds: Optional[Dict[str, Any]] = None,
     ) -> R:
         """Run a single coroutine on the pool."""
         if not self.running:
             raise RuntimeError("pool is closed")
 
         args = args or ()
         kwds = kwds or {}
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/scheduler.py` & `aiomultiprocess-0.9.1/aiomultiprocess/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2019 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import itertools
 from abc import ABC, abstractmethod
 from typing import Any, Awaitable, Callable, Dict, Iterator, List, Sequence
 
 from .types import Queue, QueueID, R, TaskID
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/tests/base.py` & `aiomultiprocess-0.9.1/aiomultiprocess/tests/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import asyncio
 import os
 from functools import wraps
 from unittest import skipUnless
 
@@ -33,15 +33,15 @@
 DUMMY_CONSTANT = None
 
 
 def initializer(value):
     global DUMMY_CONSTANT
 
     DUMMY_CONSTANT = value
-    _loop = asyncio.get_event_loop()
+    asyncio.get_event_loop()
 
 
 async def get_dummy_constant():
     return DUMMY_CONSTANT
 
 
 async def raise_fn():
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/tests/core.py` & `aiomultiprocess-0.9.1/aiomultiprocess/tests/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import asyncio
 import sys
 import time
 from unittest import TestCase
 from unittest.mock import patch
@@ -15,15 +15,15 @@
     initializer,
     raise_fn,
     sleepy,
     two,
 )
 
 
-class CoreTest(TestCase):  # pylint: disable=too-many-public-methods
+class CoreTest(TestCase):
     def setUp(self):
         # reset to default context before each test
         amp.set_start_method()
 
     @async_test
     async def test_process(self):
         p = amp.Process(target=sleepy, name="test_process")
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/tests/perf.py` & `aiomultiprocess-0.9.1/aiomultiprocess/tests/perf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import asyncio
 import time
 from unittest import TestCase
 
 import aiomultiprocess as amp
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/tests/pool.py` & `aiomultiprocess-0.9.1/aiomultiprocess/tests/pool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# Copyright 2018 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
-# pylint: disable=import-error,import-outside-toplevel
 
 import asyncio
 from unittest import TestCase
 
 import aiomultiprocess as amp
 from aiomultiprocess.core import get_context
 from aiomultiprocess.pool import PoolWorker, ProxyException
@@ -15,15 +14,15 @@
 async def check_uvloop():
     import uvloop
 
     loop = asyncio.get_event_loop()
     return isinstance(loop, uvloop.Loop)
 
 
-class PoolTest(TestCase):  # pylint: disable=too-many-public-methods
+class PoolTest(TestCase):
     @async_test
     async def test_pool_worker_max_tasks(self):
         tx = get_context().Queue()
         rx = get_context().Queue()
         worker = PoolWorker(tx, rx, 1)
         worker.start()
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/tests/scheduler.py` & `aiomultiprocess-0.9.1/aiomultiprocess/tests/scheduler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 from unittest import TestCase
 
 import aiomultiprocess as amp
```

### Comparing `aiomultiprocess-0.9.0/aiomultiprocess/types.py` & `aiomultiprocess-0.9.1/aiomultiprocess/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 John Reese
+# Copyright 2022 Amethyst Reese
 # Licensed under the MIT license
 
 import multiprocessing
 from asyncio import BaseEventLoop
 from typing import (
     Any,
     Callable,
```

### Comparing `aiomultiprocess-0.9.0/docs/_templates/omnilib.html` & `aiomultiprocess-0.9.1/docs/_templates/omnilib.html`

 * *Files identical despite different names*

### Comparing `aiomultiprocess-0.9.0/docs/conf.py` & `aiomultiprocess-0.9.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 
 
 # -- Project information -----------------------------------------------------
 
 import datetime
 
 project = "aiomultiprocess"
-copyright = f"{datetime.date.today().year}, John Reese"
-author = "John Reese"
+copyright = f"{datetime.date.today().year}, Amethyst Reese"
+author = "Amethyst Reese"
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["m2r", "sphinx.ext.autodoc", "sphinx.ext.intersphinx"]
+extensions = ["sphinx_mdinclude", "sphinx.ext.autodoc", "sphinx.ext.intersphinx"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -41,15 +41,16 @@
 
 autodoc_default_options = {
     "show-inheritance": True,
     "members": True,
     "inherited-members": True,
 }
 autodoc_member_order = "bysource"
-# autodoc_typehints = "description"
+autodoc_typehints = "description"
+
 highlight_language = "python3"
 intersphinx_mapping = {"python": ("https://docs.python.org/3", None)}
 master_doc = "index"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
```

### Comparing `aiomultiprocess-0.9.0/docs/guide.rst` & `aiomultiprocess-0.9.1/docs/guide.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     from aiomultiprocess import Pool
 
     async def get(url):
         async with request("GET", url) as response:
             return await response.text("utf-8")
 
     async def main():
-        urls = ["https://jreese.sh", ...]
+        urls = ["https://noswap.com", ...]
         async with Pool() as pool:
             async for result in pool.map(get, urls):
                 ...  # process result
 
 
 Workers
 -------
@@ -34,26 +34,26 @@
     async def get(url, method="GET"):
         async with request(method, url) as response:
             return await response.text("utf-8")
 
     async def main():
         result = await Worker(
             target=get,
-            args=("https://jreese.sh",),
+            args=("https://noswap.com",),
             kwargs={"method": "GET"}
         )
 
 The worker process can also be started by manually calling the ``start()``
 method, and the results can then be retrieved by awaiting the ``join()``
 method::
 
     async def main():
         worker = Worker(
             target=get,
-            args=("https://jreese.sh",),
+            args=("https://noswap.com",),
             kwargs={"method": "GET"}
         )
         worker.start()
         result = await worker.join()
 
 
 Process Pools
@@ -70,15 +70,15 @@
 
     async def get(url):
         async with request("GET", url) as response:
             return await response.text("utf-8")
 
     async with Pool() as pool:
         a, b, c = gather(
-            pool.apply(get, "https://jreese.sh"),
+            pool.apply(get, "https://github.com"),
             pool.apply(get, "https://noswap.com"),
             pool.apply(get, "https://omnilib.dev"),
         )
 
 Multiple jobs sharing the same coroutine can be queued using the ``map()``
 and ``starmap()`` methods, which will automatically queue one job for each
 element in the iterable passed to it. The method can be awaited to get all
```

### Comparing `aiomultiprocess-0.9.0/makefile` & `aiomultiprocess-0.9.1/makefile`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-SRCS:=aiomultiprocess
-build:
-	python -m flit build
-
-dev:
-	python -m flit install --symlink
-
-setup:
-	python -m pip install -Ur requirements-dev.txt
+PKG:=aiomultiprocess
+EXTRAS:=dev,docs
 
 .venv:
 	python -m venv .venv
-	source .venv/bin/activate && make setup dev
+	source .venv/bin/activate && make install
 	echo 'run `source .venv/bin/activate` to use virtualenv'
-
+ 
 venv: .venv
 
+install:
+	python -m pip install -U pip
+	python -m pip install -Ue .[$(EXTRAS)]
+
 release: lint test clean
 	python -m flit publish
 
 format:
-	python -m usort format $(SRCS)
-	python -m black $(SRCS)
+	python -m usort format $(PKG)
+	python -m black $(PKG)
 
 lint:
-	python -m mypy $(SRCS)
-	python -m pylint --rcfile .pylint $(SRCS)
-	python -m usort check $(SRCS)
-	python -m black --check $(SRCS)
+	python -m flake8 $(PKG)
+	python -m usort check $(PKG)
+	python -m black --check $(PKG)
 
 test:
 	python -m coverage run -m aiomultiprocess.tests
 	python -m coverage combine
 	python -m coverage report
+	python -m mypy $(PKG)
 
 perf:
 	export PERF_TESTS=1 && make test
 
+.PHONY: html
 html: .venv README.md docs/* docs/*/* aiomultiprocess/*
-	source .venv/bin/activate && sphinx-build -b html docs html
+	source .venv/bin/activate && sphinx-build -ab html docs html
 
 clean:
 	rm -rf build dist html README MANIFEST aiomultiprocess.egg-info
 
 distclean: clean
 	rm -rf .venv
```

