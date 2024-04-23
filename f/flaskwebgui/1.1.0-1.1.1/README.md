# Comparing `tmp/flaskwebgui-1.1.0.tar.gz` & `tmp/flaskwebgui-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaskwebgui-1.1.0.tar", last modified: Sat Mar 23 13:56:10 2024, max compression
+gzip compressed data, was "flaskwebgui-1.1.1.tar", last modified: Tue Apr 23 04:51:35 2024, max compression
```

## Comparing `flaskwebgui-1.1.0.tar` & `flaskwebgui-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-03-23 13:56:10.009316 flaskwebgui-1.1.0/
--rw-rw-r--   0 climentea  (1000) climentea  (1000)     1064 2024-02-07 06:46:59.000000 flaskwebgui-1.1.0/LICENSE
--rw-r--r--   0 climentea  (1000) climentea  (1000)     9826 2024-03-23 13:56:10.009316 flaskwebgui-1.1.0/PKG-INFO
--rw-rw-r--   0 climentea  (1000) climentea  (1000)     9492 2024-03-23 10:13:17.000000 flaskwebgui-1.1.0/README.md
--rw-rw-r--   0 climentea  (1000) climentea  (1000)       38 2024-03-23 13:56:10.009316 flaskwebgui-1.1.0/setup.cfg
--rw-rw-r--   0 climentea  (1000) climentea  (1000)      851 2024-03-23 13:54:56.000000 flaskwebgui-1.1.0/setup.py
-drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-03-23 13:56:10.005316 flaskwebgui-1.1.0/src/
-drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-03-23 13:56:10.009316 flaskwebgui-1.1.0/src/flaskwebgui.egg-info/
--rw-r--r--   0 climentea  (1000) climentea  (1000)     9826 2024-03-23 13:56:09.000000 flaskwebgui-1.1.0/src/flaskwebgui.egg-info/PKG-INFO
--rw-rw-r--   0 climentea  (1000) climentea  (1000)      239 2024-03-23 13:56:09.000000 flaskwebgui-1.1.0/src/flaskwebgui.egg-info/SOURCES.txt
--rw-rw-r--   0 climentea  (1000) climentea  (1000)        1 2024-03-23 13:56:09.000000 flaskwebgui-1.1.0/src/flaskwebgui.egg-info/dependency_links.txt
--rw-rw-r--   0 climentea  (1000) climentea  (1000)       12 2024-03-23 13:56:09.000000 flaskwebgui-1.1.0/src/flaskwebgui.egg-info/requires.txt
--rw-rw-r--   0 climentea  (1000) climentea  (1000)       12 2024-03-23 13:56:09.000000 flaskwebgui-1.1.0/src/flaskwebgui.egg-info/top_level.txt
--rw-rw-r--   0 climentea  (1000) climentea  (1000)     8231 2024-03-23 13:48:50.000000 flaskwebgui-1.1.0/src/flaskwebgui.py
+drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-04-23 04:51:35.314486 flaskwebgui-1.1.1/
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)     1064 2024-02-07 06:46:59.000000 flaskwebgui-1.1.1/LICENSE
+-rw-r--r--   0 climentea  (1000) climentea  (1000)     9911 2024-04-23 04:51:35.314486 flaskwebgui-1.1.1/PKG-INFO
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)     9577 2024-04-23 04:49:37.000000 flaskwebgui-1.1.1/README.md
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)       38 2024-04-23 04:51:35.314486 flaskwebgui-1.1.1/setup.cfg
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)      851 2024-04-23 04:49:37.000000 flaskwebgui-1.1.1/setup.py
+drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-04-23 04:51:35.310486 flaskwebgui-1.1.1/src/
+drwxrwxr-x   0 climentea  (1000) climentea  (1000)        0 2024-04-23 04:51:35.310486 flaskwebgui-1.1.1/src/flaskwebgui.egg-info/
+-rw-r--r--   0 climentea  (1000) climentea  (1000)     9911 2024-04-23 04:51:35.000000 flaskwebgui-1.1.1/src/flaskwebgui.egg-info/PKG-INFO
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)      239 2024-04-23 04:51:35.000000 flaskwebgui-1.1.1/src/flaskwebgui.egg-info/SOURCES.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)        1 2024-04-23 04:51:35.000000 flaskwebgui-1.1.1/src/flaskwebgui.egg-info/dependency_links.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)       12 2024-04-23 04:51:35.000000 flaskwebgui-1.1.1/src/flaskwebgui.egg-info/requires.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)       12 2024-04-23 04:51:35.000000 flaskwebgui-1.1.1/src/flaskwebgui.egg-info/top_level.txt
+-rw-rw-r--   0 climentea  (1000) climentea  (1000)     8373 2024-04-23 04:49:37.000000 flaskwebgui-1.1.1/src/flaskwebgui.py
```

### Comparing `flaskwebgui-1.1.0/LICENSE` & `flaskwebgui-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flaskwebgui-1.1.0/PKG-INFO` & `flaskwebgui-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskwebgui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Create desktop applications with Flask/Django/FastAPI!
 Home-page: https://github.com/ClimenteA/flaskwebgui
 Author: Climente Alin
 Author-email: climente.alin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -253,14 +253,15 @@
 - `app: Any = None`: `wsgi` or `asgi` app;
 - `port: int = None`: specify port if not a free port will set;
 - `width: int = None`: width of the window;
 - `height: int = None`: height of the window;
 - `fullscreen: bool = True`: start app in fullscreen (maximized);
 - `on_startup: Callable = None`: function to before starting the browser and webserver;
 - `on_shutdown: Callable = None`: function to after the browser and webserver shutdown;
+- `extra_flags: List[str] = None`: list of additional flags for the browser command;
 - `browser_path: str = None`: set path to chrome executable or let the defaults do that;
 - `browser_command: List[str] = None`: command line with starts chrome in `app` mode;
 - `socketio: Any = None`: socketio instance in case of flask_socketio;
 
 Develop your app as you would normally do, add flaskwebgui at the end or for tests.
 **flaskwebgui doesn't interfere with your way of doing an application** it just helps converting it into a desktop app more easily with pyinstaller or [pyvan](https://github.com/ClimenteA/pyvan).
```

### Comparing `flaskwebgui-1.1.0/README.md` & `flaskwebgui-1.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
 - `app: Any = None`: `wsgi` or `asgi` app;
 - `port: int = None`: specify port if not a free port will set;
 - `width: int = None`: width of the window;
 - `height: int = None`: height of the window;
 - `fullscreen: bool = True`: start app in fullscreen (maximized);
 - `on_startup: Callable = None`: function to before starting the browser and webserver;
 - `on_shutdown: Callable = None`: function to after the browser and webserver shutdown;
+- `extra_flags: List[str] = None`: list of additional flags for the browser command;
 - `browser_path: str = None`: set path to chrome executable or let the defaults do that;
 - `browser_command: List[str] = None`: command line with starts chrome in `app` mode;
 - `socketio: Any = None`: socketio instance in case of flask_socketio;
 
 Develop your app as you would normally do, add flaskwebgui at the end or for tests.
 **flaskwebgui doesn't interfere with your way of doing an application** it just helps converting it into a desktop app more easily with pyinstaller or [pyvan](https://github.com/ClimenteA/pyvan).
```

### Comparing `flaskwebgui-1.1.0/setup.py` & `flaskwebgui-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 with open("requirements.txt", "r") as r:
     install_requires = r.readlines()
 
 
 setup(
     name="flaskwebgui",
-    version="1.1.0",
+    version="1.1.1",
     description="Create desktop applications with Flask/Django/FastAPI!",
     url="https://github.com/ClimenteA/flaskwebgui",
     author="Climente Alin",
     author_email="climente.alin@gmail.com",
     license="MIT",
     py_modules=["flaskwebgui"],
     install_requires=install_requires,
```

### Comparing `flaskwebgui-1.1.0/src/flaskwebgui.egg-info/PKG-INFO` & `flaskwebgui-1.1.1/src/flaskwebgui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaskwebgui
-Version: 1.1.0
+Version: 1.1.1
 Summary: Create desktop applications with Flask/Django/FastAPI!
 Home-page: https://github.com/ClimenteA/flaskwebgui
 Author: Climente Alin
 Author-email: climente.alin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -253,14 +253,15 @@
 - `app: Any = None`: `wsgi` or `asgi` app;
 - `port: int = None`: specify port if not a free port will set;
 - `width: int = None`: width of the window;
 - `height: int = None`: height of the window;
 - `fullscreen: bool = True`: start app in fullscreen (maximized);
 - `on_startup: Callable = None`: function to before starting the browser and webserver;
 - `on_shutdown: Callable = None`: function to after the browser and webserver shutdown;
+- `extra_flags: List[str] = None`: list of additional flags for the browser command;
 - `browser_path: str = None`: set path to chrome executable or let the defaults do that;
 - `browser_command: List[str] = None`: command line with starts chrome in `app` mode;
 - `socketio: Any = None`: socketio instance in case of flask_socketio;
 
 Develop your app as you would normally do, add flaskwebgui at the end or for tests.
 **flaskwebgui doesn't interfere with your way of doing an application** it just helps converting it into a desktop app more easily with pyinstaller or [pyvan](https://github.com/ClimenteA/pyvan).
```

### Comparing `flaskwebgui-1.1.0/src/flaskwebgui.py` & `flaskwebgui-1.1.1/src/flaskwebgui.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 
 def find_browser_on_windows():
     paths = [
         r"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe",
         r"C:\Program Files\Microsoft\Edge\Application\msedge.exe",
         r"C:\Program Files\Google\Chrome\Application\chrome.exe",
-        r"C:\Program Files\BraveSoftware\Brave-Browser\Application\\brave.exe",
+        r"C:\Program Files\BraveSoftware\Brave-Browser\Application\brave.exe",
     ]
     for path in paths:
         if os.path.exists(path):
             return path
     return None
 
 
@@ -186,14 +186,15 @@
     app: Any = None
     port: int = None
     width: int = None
     height: int = None
     fullscreen: bool = True
     on_startup: Callable = None
     on_shutdown: Callable = None
+    extra_flags: List[str] = None
     browser_path: str = None
     browser_command: List[str] = None
     socketio: Any = None
     profile_dir_prefix: str = "flaskwebgui"
 
     def __post_init__(self):
         self.__keyboard_interrupt = False
@@ -238,14 +239,18 @@
         ]
 
         if self.width and self.height:
             flags.extend([f"--window-size={self.width},{self.height}"])
         elif self.fullscreen:
             flags.extend(["--start-maximized"])
 
+        if self.extra_flags:
+            for flag in self.extra_flags:
+                flags.extend([flag])
+
         flags.extend([f"--app={self.url}"])
 
         return flags
 
     def start_browser(self, server_process: Union[Thread, Process]):
         print("Command:", " ".join(self.browser_command))
         global FLASKWEBGUI_BROWSER_PROCESS
```

