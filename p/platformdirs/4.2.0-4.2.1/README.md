# Comparing `tmp/platformdirs-4.2.0.tar.gz` & `tmp/platformdirs-4.2.1.tar.gz`

## Comparing `platformdirs-4.2.0.tar` & `platformdirs-4.2.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tox.ini
--rw-r--r--   0        0        0    22134 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     8940 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/version.py
--rw-r--r--   0        0        0    10008 2020-02-02 00:00:00.000000 platformdirs-4.2.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tests/conftest.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tests/test_android.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tests/test_api.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tests/test_main.py
--rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 platformdirs-4.2.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-4.2.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-4.2.0/LICENSE
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 platformdirs-4.2.0/README.rst
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 platformdirs-4.2.0/pyproject.toml
--rw-r--r--   0        0        0    11366 2020-02-02 00:00:00.000000 platformdirs-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0    22225 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7681 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/android.py
+-rw-r--r--   0        0        0     8996 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/api.py
+-rw-r--r--   0        0        0     5580 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/py.typed
+-rw-r--r--   0        0        0    10643 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/version.py
+-rw-r--r--   0        0        0    10125 2020-02-02 00:00:00.000000 platformdirs-4.2.1/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 platformdirs-4.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 platformdirs-4.2.1/tests/test_android.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 platformdirs-4.2.1/tests/test_api.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 platformdirs-4.2.1/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 platformdirs-4.2.1/tests/test_macos.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 platformdirs-4.2.1/tests/test_main.py
+-rw-r--r--   0        0        0     6974 2020-02-02 00:00:00.000000 platformdirs-4.2.1/tests/test_unix.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 platformdirs-4.2.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-4.2.1/LICENSE
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 platformdirs-4.2.1/README.rst
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 platformdirs-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11429 2020-02-02 00:00:00.000000 platformdirs-4.2.1/PKG-INFO
```

### Comparing `platformdirs-4.2.0/src/platformdirs/__init__.py` & `platformdirs-4.2.1/src/platformdirs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
-Utilities for determining application-specific dirs. See <https://github.com/platformdirs/platformdirs> for details and
-usage.
+Utilities for determining application-specific dirs.
+
+See <https://github.com/platformdirs/platformdirs> for details and usage.
+
 """
 
 from __future__ import annotations
 
 import os
 import sys
 from typing import TYPE_CHECKING
@@ -16,30 +18,30 @@
 if TYPE_CHECKING:
     from pathlib import Path
     from typing import Literal
 
 
 def _set_platform_dir_class() -> type[PlatformDirsABC]:
     if sys.platform == "win32":
-        from platformdirs.windows import Windows as Result
+        from platformdirs.windows import Windows as Result  # noqa: PLC0415
     elif sys.platform == "darwin":
-        from platformdirs.macos import MacOS as Result
+        from platformdirs.macos import MacOS as Result  # noqa: PLC0415
     else:
-        from platformdirs.unix import Unix as Result
+        from platformdirs.unix import Unix as Result  # noqa: PLC0415
 
     if os.getenv("ANDROID_DATA") == "/data" and os.getenv("ANDROID_ROOT") == "/system":
         if os.getenv("SHELL") or os.getenv("PREFIX"):
             return Result
 
-        from platformdirs.android import _android_folder
+        from platformdirs.android import _android_folder  # noqa: PLC0415
 
         if _android_folder() is not None:
-            from platformdirs.android import Android
+            from platformdirs.android import Android  # noqa: PLC0415
 
-            return Android  # return to avoid redefinition of result
+            return Android  # return to avoid redefinition of a result
 
     return Result
 
 
 PlatformDirs = _set_platform_dir_class()  #: Currently active platform
 AppDirs = PlatformDirs  #: Backwards compatibility with appdirs
 
@@ -503,15 +505,15 @@
         version=version,
         opinion=opinion,
         ensure_exists=ensure_exists,
     ).user_log_path
 
 
 def user_documents_path() -> Path:
-    """:returns: documents path tied to the user"""
+    """:returns: documents a path tied to the user"""
     return PlatformDirs().user_documents_path
 
 
 def user_downloads_path() -> Path:
     """:returns: downloads path tied to the user"""
     return PlatformDirs().user_downloads_path
 
@@ -581,45 +583,45 @@
         version=version,
         opinion=opinion,
         ensure_exists=ensure_exists,
     ).site_runtime_path
 
 
 __all__ = [
-    "__version__",
-    "__version_info__",
-    "PlatformDirs",
     "AppDirs",
+    "PlatformDirs",
     "PlatformDirsABC",
-    "user_data_dir",
-    "user_config_dir",
-    "user_cache_dir",
-    "user_state_dir",
-    "user_log_dir",
-    "user_documents_dir",
-    "user_downloads_dir",
-    "user_pictures_dir",
-    "user_videos_dir",
-    "user_music_dir",
-    "user_desktop_dir",
-    "user_runtime_dir",
-    "site_data_dir",
-    "site_config_dir",
+    "__version__",
+    "__version_info__",
     "site_cache_dir",
+    "site_cache_path",
+    "site_config_dir",
+    "site_config_path",
+    "site_data_dir",
+    "site_data_path",
     "site_runtime_dir",
-    "user_data_path",
-    "user_config_path",
+    "site_runtime_path",
+    "user_cache_dir",
     "user_cache_path",
-    "user_state_path",
-    "user_log_path",
+    "user_config_dir",
+    "user_config_path",
+    "user_data_dir",
+    "user_data_path",
+    "user_desktop_dir",
+    "user_desktop_path",
+    "user_documents_dir",
     "user_documents_path",
+    "user_downloads_dir",
     "user_downloads_path",
-    "user_pictures_path",
-    "user_videos_path",
+    "user_log_dir",
+    "user_log_path",
+    "user_music_dir",
     "user_music_path",
-    "user_desktop_path",
+    "user_pictures_dir",
+    "user_pictures_path",
+    "user_runtime_dir",
     "user_runtime_path",
-    "site_data_path",
-    "site_config_path",
-    "site_cache_path",
-    "site_runtime_path",
+    "user_state_dir",
+    "user_state_path",
+    "user_videos_dir",
+    "user_videos_path",
 ]
```

### Comparing `platformdirs-4.2.0/src/platformdirs/__main__.py` & `platformdirs-4.2.1/src/platformdirs/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "site_config_dir",
     "site_cache_dir",
     "site_runtime_dir",
 )
 
 
 def main() -> None:
-    """Run main entry point."""
+    """Run the main entry point."""
     app_name = "MyApp"
     app_author = "MyCompany"
 
     print(f"-- platformdirs {__version__} --")  # noqa: T201
 
     print("-- app dirs (with optional 'version')")  # noqa: T201
     dirs = PlatformDirs(app_name, app_author, version="1.0")
```

### Comparing `platformdirs-4.2.0/src/platformdirs/android.py` & `platformdirs-4.2.1/src/platformdirs/android.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 from typing import cast
 
 from .api import PlatformDirsABC
 
 
 class Android(PlatformDirsABC):
     """
-    Follows the guidance `from here <https://android.stackexchange.com/a/216132>`_. Makes use of the
-    `appname <platformdirs.api.PlatformDirsABC.appname>`,
-    `version <platformdirs.api.PlatformDirsABC.version>`,
-    `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
+    Follows the guidance `from here <https://android.stackexchange.com/a/216132>`_.
+
+    Makes use of the `appname <platformdirs.api.PlatformDirsABC.appname>`, `version
+    <platformdirs.api.PlatformDirsABC.version>`, `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
+
     """
 
     @property
     def user_data_dir(self) -> str:
         """:return: data directory tied to the user, e.g. ``/data/user/<userid>/<packagename>/files/<AppName>``"""
         return self._append_app_name_and_version(cast(str, _android_folder()), "files")
 
@@ -40,15 +41,15 @@
     @property
     def site_config_dir(self) -> str:
         """:return: config directory shared by the users, same as `user_config_dir`"""
         return self.user_config_dir
 
     @property
     def user_cache_dir(self) -> str:
-        """:return: cache directory tied to the user, e.g. e.g. ``/data/user/<userid>/<packagename>/cache/<AppName>``"""
+        """:return: cache directory tied to the user, e.g.,``/data/user/<userid>/<packagename>/cache/<AppName>``"""
         return self._append_app_name_and_version(cast(str, _android_folder()), "cache")
 
     @property
     def site_cache_dir(self) -> str:
         """:return: cache directory shared by users, same as `user_cache_dir`"""
         return self.user_cache_dir
 
@@ -115,21 +116,21 @@
         return self.user_runtime_dir
 
 
 @lru_cache(maxsize=1)
 def _android_folder() -> str | None:
     """:return: base folder for the Android OS or None if it cannot be found"""
     try:
-        # First try to get path to android app via pyjnius
-        from jnius import autoclass
+        # First try to get a path to android app via pyjnius
+        from jnius import autoclass  # noqa: PLC0415
 
         context = autoclass("android.content.Context")
         result: str | None = context.getFilesDir().getParentFile().getAbsolutePath()
     except Exception:  # noqa: BLE001
-        # if fails find an android folder looking path on the sys.path
+        # if fails find an android folder looking a path on the sys.path
         pattern = re.compile(r"/data/(data|user/\d+)/(.+)/files")
         for path in sys.path:
             if pattern.match(path):
                 result = path.split("/files")[0]
                 break
         else:
             result = None
@@ -137,15 +138,15 @@
 
 
 @lru_cache(maxsize=1)
 def _android_documents_folder() -> str:
     """:return: documents folder for the Android OS"""
     # Get directories with pyjnius
     try:
-        from jnius import autoclass
+        from jnius import autoclass  # noqa: PLC0415
 
         context = autoclass("android.content.Context")
         environment = autoclass("android.os.Environment")
         documents_dir: str = context.getExternalFilesDir(environment.DIRECTORY_DOCUMENTS).getAbsolutePath()
     except Exception:  # noqa: BLE001
         documents_dir = "/storage/emulated/0/Documents"
 
@@ -153,15 +154,15 @@
 
 
 @lru_cache(maxsize=1)
 def _android_downloads_folder() -> str:
     """:return: downloads folder for the Android OS"""
     # Get directories with pyjnius
     try:
-        from jnius import autoclass
+        from jnius import autoclass  # noqa: PLC0415
 
         context = autoclass("android.content.Context")
         environment = autoclass("android.os.Environment")
         downloads_dir: str = context.getExternalFilesDir(environment.DIRECTORY_DOWNLOADS).getAbsolutePath()
     except Exception:  # noqa: BLE001
         downloads_dir = "/storage/emulated/0/Downloads"
 
@@ -169,15 +170,15 @@
 
 
 @lru_cache(maxsize=1)
 def _android_pictures_folder() -> str:
     """:return: pictures folder for the Android OS"""
     # Get directories with pyjnius
     try:
-        from jnius import autoclass
+        from jnius import autoclass  # noqa: PLC0415
 
         context = autoclass("android.content.Context")
         environment = autoclass("android.os.Environment")
         pictures_dir: str = context.getExternalFilesDir(environment.DIRECTORY_PICTURES).getAbsolutePath()
     except Exception:  # noqa: BLE001
         pictures_dir = "/storage/emulated/0/Pictures"
 
@@ -185,15 +186,15 @@
 
 
 @lru_cache(maxsize=1)
 def _android_videos_folder() -> str:
     """:return: videos folder for the Android OS"""
     # Get directories with pyjnius
     try:
-        from jnius import autoclass
+        from jnius import autoclass  # noqa: PLC0415
 
         context = autoclass("android.content.Context")
         environment = autoclass("android.os.Environment")
         videos_dir: str = context.getExternalFilesDir(environment.DIRECTORY_DCIM).getAbsolutePath()
     except Exception:  # noqa: BLE001
         videos_dir = "/storage/emulated/0/DCIM/Camera"
 
@@ -201,15 +202,15 @@
 
 
 @lru_cache(maxsize=1)
 def _android_music_folder() -> str:
     """:return: music folder for the Android OS"""
     # Get directories with pyjnius
     try:
-        from jnius import autoclass
+        from jnius import autoclass  # noqa: PLC0415
 
         context = autoclass("android.content.Context")
         environment = autoclass("android.os.Environment")
         music_dir: str = context.getExternalFilesDir(environment.DIRECTORY_MUSIC).getAbsolutePath()
     except Exception:  # noqa: BLE001
         music_dir = "/storage/emulated/0/Music"
```

### Comparing `platformdirs-4.2.0/src/platformdirs/api.py` & `platformdirs-4.2.1/src/platformdirs/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Iterator, Literal
 
 
-class PlatformDirsABC(ABC):
+class PlatformDirsABC(ABC):  # noqa: PLR0904
     """Abstract base class for platform directories."""
 
-    def __init__(  # noqa: PLR0913
+    def __init__(  # noqa: PLR0913, PLR0917
         self,
         appname: str | None = None,
         appauthor: str | None | Literal[False] = None,
         version: str | None = None,
         roaming: bool = False,  # noqa: FBT001, FBT002
         multipath: bool = False,  # noqa: FBT001, FBT002
         opinion: bool = True,  # noqa: FBT001, FBT002
@@ -30,42 +30,55 @@
         :param appname: See `appname`.
         :param appauthor: See `appauthor`.
         :param version: See `version`.
         :param roaming: See `roaming`.
         :param multipath: See `multipath`.
         :param opinion: See `opinion`.
         :param ensure_exists: See `ensure_exists`.
+
         """
         self.appname = appname  #: The name of application.
         self.appauthor = appauthor
         """
-        The name of the app author or distributing body for this application. Typically, it is the owning company name.
-        Defaults to `appname`. You may pass ``False`` to disable it.
+        The name of the app author or distributing body for this application.
+
+        Typically, it is the owning company name. Defaults to `appname`. You may pass ``False`` to disable it.
+
         """
         self.version = version
         """
-        An optional version path element to append to the path. You might want to use this if you want multiple versions
-        of your app to be able to run independently. If used, this would typically be ``<major>.<minor>``.
+        An optional version path element to append to the path.
+
+        You might want to use this if you want multiple versions of your app to be able to run independently. If used,
+        this would typically be ``<major>.<minor>``.
+
         """
         self.roaming = roaming
         """
-        Whether to use the roaming appdata directory on Windows. That means that for users on a Windows network setup
-        for roaming profiles, this user data will be synced on login (see
-        `here <http://technet.microsoft.com/en-us/library/cc766489(WS.10).aspx>`_).
+        Whether to use the roaming appdata directory on Windows.
+
+        That means that for users on a Windows network setup for roaming profiles, this user data will be synced on
+        login (see
+        `here <https://technet.microsoft.com/en-us/library/cc766489(WS.10).aspx>`_).
+
         """
         self.multipath = multipath
         """
         An optional parameter which indicates that the entire list of data dirs should be returned.
+
         By default, the first item would only be returned.
+
         """
         self.opinion = opinion  #: A flag to indicating to use opinionated values.
         self.ensure_exists = ensure_exists
         """
         Optionally create the directory (and any missing parents) upon access if it does not exist.
+
         By default, no directories are created.
+
         """
 
     def _append_app_name_and_version(self, *base: str) -> str:
         params = list(base[1:])
         if self.appname:
             params.append(self.appname)
             if self.version:
@@ -196,15 +209,15 @@
     @property
     def user_log_path(self) -> Path:
         """:return: log path tied to the user"""
         return Path(self.user_log_dir)
 
     @property
     def user_documents_path(self) -> Path:
-        """:return: documents path tied to the user"""
+        """:return: documents a path tied to the user"""
         return Path(self.user_documents_dir)
 
     @property
     def user_downloads_path(self) -> Path:
         """:return: downloads path tied to the user"""
         return Path(self.user_downloads_dir)
```

### Comparing `platformdirs-4.2.0/src/platformdirs/macos.py` & `platformdirs-4.2.1/src/platformdirs/macos.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,36 @@
 import sys
 
 from .api import PlatformDirsABC
 
 
 class MacOS(PlatformDirsABC):
     """
-    Platform directories for the macOS operating system. Follows the guidance from `Apple documentation
-    <https://developer.apple.com/library/archive/documentation/FileManagement/Conceptual/FileSystemProgrammingGuide/MacOSXDirectories/MacOSXDirectories.html>`_.
+    Platform directories for the macOS operating system.
+
+    Follows the guidance from
+    `Apple documentation <https://developer.apple.com/library/archive/documentation/FileManagement/Conceptual/FileSystemProgrammingGuide/MacOSXDirectories/MacOSXDirectories.html>`_.
     Makes use of the `appname <platformdirs.api.PlatformDirsABC.appname>`,
     `version <platformdirs.api.PlatformDirsABC.version>`,
     `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
+
     """
 
     @property
     def user_data_dir(self) -> str:
         """:return: data directory tied to the user, e.g. ``~/Library/Application Support/$appname/$version``"""
         return self._append_app_name_and_version(os.path.expanduser("~/Library/Application Support"))  # noqa: PTH111
 
     @property
     def site_data_dir(self) -> str:
         """
         :return: data directory shared by users, e.g. ``/Library/Application Support/$appname/$version``.
           If we're using a Python binary managed by `Homebrew <https://brew.sh>`_, the directory
           will be under the Homebrew prefix, e.g. ``/opt/homebrew/share/$appname/$version``.
-          If `multipath <platformdirs.api.PlatformDirsABC.multipath>` is enabled and we're in Homebrew,
+          If `multipath <platformdirs.api.PlatformDirsABC.multipath>` is enabled, and we're in Homebrew,
           the response is a multi-path string separated by ":", e.g.
           ``/opt/homebrew/share/$appname/$version:/Library/Application Support/$appname/$version``
         """
         is_homebrew = sys.prefix.startswith("/opt/homebrew")
         path_list = [self._append_app_name_and_version("/opt/homebrew/share")] if is_homebrew else []
         path_list.append(self._append_app_name_and_version("/Library/Application Support"))
         if self.multipath:
@@ -56,15 +59,15 @@
 
     @property
     def site_cache_dir(self) -> str:
         """
         :return: cache directory shared by users, e.g. ``/Library/Caches/$appname/$version``.
           If we're using a Python binary managed by `Homebrew <https://brew.sh>`_, the directory
           will be under the Homebrew prefix, e.g. ``/opt/homebrew/var/cache/$appname/$version``.
-          If `multipath <platformdirs.api.PlatformDirsABC.multipath>` is enabled and we're in Homebrew,
+          If `multipath <platformdirs.api.PlatformDirsABC.multipath>` is enabled, and we're in Homebrew,
           the response is a multi-path string separated by ":", e.g.
           ``/opt/homebrew/var/cache/$appname/$version:/Library/Caches/$appname/$version``
         """
         is_homebrew = sys.prefix.startswith("/opt/homebrew")
         path_list = [self._append_app_name_and_version("/opt/homebrew/var/cache")] if is_homebrew else []
         path_list.append(self._append_app_name_and_version("/Library/Caches"))
         if self.multipath:
```

### Comparing `platformdirs-4.2.0/src/platformdirs/unix.py` & `platformdirs-4.2.1/src/platformdirs/unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 
 from __future__ import annotations
 
 import os
 import sys
 from configparser import ConfigParser
 from pathlib import Path
-from typing import Iterator
+from typing import Iterator, NoReturn
 
 from .api import PlatformDirsABC
 
 if sys.platform == "win32":
 
-    def getuid() -> int:
+    def getuid() -> NoReturn:
         msg = "should only be used on Unix"
         raise RuntimeError(msg)
 
 else:
     from os import getuid
 
 
-class Unix(PlatformDirsABC):
+class Unix(PlatformDirsABC):  # noqa: PLR0904
     """
-    On Unix/Linux, we follow the
-    `XDG Basedir Spec <https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html>`_. The spec allows
-    overriding directories with environment variables. The examples show are the default values, alongside the name of
-    the environment variable that overrides them. Makes use of the
-    `appname <platformdirs.api.PlatformDirsABC.appname>`,
-    `version <platformdirs.api.PlatformDirsABC.version>`,
-    `multipath <platformdirs.api.PlatformDirsABC.multipath>`,
-    `opinion <platformdirs.api.PlatformDirsABC.opinion>`,
-    `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
+    On Unix/Linux, we follow the `XDG Basedir Spec <https://specifications.freedesktop.org/basedir-spec/basedir-spec-
+    latest.html>`_.
+
+    The spec allows overriding directories with environment variables. The examples shown are the default values,
+    alongside the name of the environment variable that overrides them. Makes use of the `appname
+    <platformdirs.api.PlatformDirsABC.appname>`, `version <platformdirs.api.PlatformDirsABC.version>`, `multipath
+    <platformdirs.api.PlatformDirsABC.multipath>`, `opinion <platformdirs.api.PlatformDirsABC.opinion>`, `ensure_exists
+    <platformdirs.api.PlatformDirsABC.ensure_exists>`.
+
     """
 
     @property
     def user_data_dir(self) -> str:
         """
         :return: data directory tied to the user, e.g. ``~/.local/share/$appname/$version`` or
          ``$XDG_DATA_HOME/$appname/$version``
@@ -201,25 +201,25 @@
                 path = "/var/run"
             else:
                 path = "/run"
         return self._append_app_name_and_version(path)
 
     @property
     def site_data_path(self) -> Path:
-        """:return: data path shared by users. Only return first item, even if ``multipath`` is set to ``True``"""
+        """:return: data path shared by users. Only return the first item, even if ``multipath`` is set to ``True``"""
         return self._first_item_as_path_if_multipath(self.site_data_dir)
 
     @property
     def site_config_path(self) -> Path:
-        """:return: config path shared by the users. Only return first item, even if ``multipath`` is set to ``True``"""
+        """:return: config path shared by the users, returns the first item, even if ``multipath`` is set to ``True``"""
         return self._first_item_as_path_if_multipath(self.site_config_dir)
 
     @property
     def site_cache_path(self) -> Path:
-        """:return: cache path shared by users. Only return first item, even if ``multipath`` is set to ``True``"""
+        """:return: cache path shared by users. Only return the first item, even if ``multipath`` is set to ``True``"""
         return self._first_item_as_path_if_multipath(self.site_cache_dir)
 
     def _first_item_as_path_if_multipath(self, directory: str) -> Path:
         if self.multipath:
             # If multipath is True, the first path is returned.
             directory = directory.split(os.pathsep)[0]
         return Path(directory)
@@ -242,15 +242,20 @@
         if not media_dir:
             media_dir = os.path.expanduser(fallback_tilde_path)  # noqa: PTH111
 
     return media_dir
 
 
 def _get_user_dirs_folder(key: str) -> str | None:
-    """Return directory from user-dirs.dirs config file. See https://freedesktop.org/wiki/Software/xdg-user-dirs/."""
+    """
+    Return directory from user-dirs.dirs config file.
+
+    See https://freedesktop.org/wiki/Software/xdg-user-dirs/.
+
+    """
     user_dirs_config_path = Path(Unix().user_config_dir) / "user-dirs.dirs"
     if user_dirs_config_path.exists():
         parser = ConfigParser()
 
         with user_dirs_config_path.open() as stream:
             # Add fake section header, so ConfigParser doesn't complain
             parser.read_string(f"[top]\n{stream.read()}")
```

### Comparing `platformdirs-4.2.0/src/platformdirs/windows.py` & `platformdirs-4.2.1/src/platformdirs/windows.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """Windows."""
 
 from __future__ import annotations
 
-import ctypes
 import os
 import sys
 from functools import lru_cache
 from typing import TYPE_CHECKING
 
 from .api import PlatformDirsABC
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
 
 class Windows(PlatformDirsABC):
     """
-    `MSDN on where to store app data files
-    <http://support.microsoft.com/default.aspx?scid=kb;en-us;310294#XSLTH3194121123120121120120>`_.
-    Makes use of the
-    `appname <platformdirs.api.PlatformDirsABC.appname>`,
-    `appauthor <platformdirs.api.PlatformDirsABC.appauthor>`,
-    `version <platformdirs.api.PlatformDirsABC.version>`,
-    `roaming <platformdirs.api.PlatformDirsABC.roaming>`,
-    `opinion <platformdirs.api.PlatformDirsABC.opinion>`,
-    `ensure_exists <platformdirs.api.PlatformDirsABC.ensure_exists>`.
+    `MSDN on where to store app data files <https://learn.microsoft.com/en-us/windows/win32/shell/knownfolderid>`_.
+
+    Makes use of the `appname <platformdirs.api.PlatformDirsABC.appname>`, `appauthor
+    <platformdirs.api.PlatformDirsABC.appauthor>`, `version <platformdirs.api.PlatformDirsABC.version>`, `roaming
+    <platformdirs.api.PlatformDirsABC.roaming>`, `opinion <platformdirs.api.PlatformDirsABC.opinion>`, `ensure_exists
+    <platformdirs.api.PlatformDirsABC.ensure_exists>`.
+
     """
 
     @property
     def user_data_dir(self) -> str:
         """
         :return: data directory tied to the user, e.g.
          ``%USERPROFILE%\\AppData\\Local\\$appauthor\\$appname`` (not roaming) or
@@ -161,15 +158,15 @@
     if result is None:
         msg = f"Unset environment variable: {env_var_name}"
         raise ValueError(msg)
     return result
 
 
 def get_win_folder_if_csidl_name_not_env_var(csidl_name: str) -> str | None:
-    """Get folder for a CSIDL name that does not exist as an environment variable."""
+    """Get a folder for a CSIDL name that does not exist as an environment variable."""
     if csidl_name == "CSIDL_PERSONAL":
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Documents")  # noqa: PTH118
 
     if csidl_name == "CSIDL_DOWNLOADS":
         return os.path.join(os.path.normpath(os.environ["USERPROFILE"]), "Downloads")  # noqa: PTH118
 
     if csidl_name == "CSIDL_MYPICTURES":
@@ -185,14 +182,15 @@
 
 def get_win_folder_from_registry(csidl_name: str) -> str:
     """
     Get folder from the registry.
 
     This is a fallback technique at best. I'm not sure if using the registry for these guarantees us the correct answer
     for all CSIDL_* names.
+
     """
     shell_folder_name = {
         "CSIDL_APPDATA": "AppData",
         "CSIDL_COMMON_APPDATA": "Common AppData",
         "CSIDL_LOCAL_APPDATA": "Local AppData",
         "CSIDL_PERSONAL": "Personal",
         "CSIDL_DOWNLOADS": "{374DE290-123F-4565-9164-39C4925E467B}",
@@ -201,27 +199,29 @@
         "CSIDL_MYMUSIC": "My Music",
     }.get(csidl_name)
     if shell_folder_name is None:
         msg = f"Unknown CSIDL name: {csidl_name}"
         raise ValueError(msg)
     if sys.platform != "win32":  # only needed for mypy type checker to know that this code runs only on Windows
         raise NotImplementedError
-    import winreg
+    import winreg  # noqa: PLC0415
 
     key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, r"Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders")
     directory, _ = winreg.QueryValueEx(key, shell_folder_name)
     return str(directory)
 
 
 def get_win_folder_via_ctypes(csidl_name: str) -> str:
     """Get folder with ctypes."""
     # There is no 'CSIDL_DOWNLOADS'.
     # Use 'CSIDL_PROFILE' (40) and append the default folder 'Downloads' instead.
     # https://learn.microsoft.com/en-us/windows/win32/shell/knownfolderid
 
+    import ctypes  # noqa: PLC0415
+
     csidl_const = {
         "CSIDL_APPDATA": 26,
         "CSIDL_COMMON_APPDATA": 35,
         "CSIDL_LOCAL_APPDATA": 28,
         "CSIDL_PERSONAL": 5,
         "CSIDL_MYPICTURES": 39,
         "CSIDL_MYVIDEO": 14,
@@ -246,18 +246,23 @@
     if csidl_name == "CSIDL_DOWNLOADS":
         return os.path.join(buf.value, "Downloads")  # noqa: PTH118
 
     return buf.value
 
 
 def _pick_get_win_folder() -> Callable[[str], str]:
-    if hasattr(ctypes, "windll"):
-        return get_win_folder_via_ctypes
     try:
-        import winreg  # noqa: F401
+        import ctypes  # noqa: PLC0415
+    except ImportError:
+        pass
+    else:
+        if hasattr(ctypes, "windll"):
+            return get_win_folder_via_ctypes
+    try:
+        import winreg  # noqa: PLC0415, F401
     except ImportError:
         return get_win_folder_from_env_vars
     else:
         return get_win_folder_from_registry
 
 
 get_win_folder = lru_cache(maxsize=None)(_pick_get_win_folder())
```

### Comparing `platformdirs-4.2.0/tests/conftest.py` & `platformdirs-4.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `platformdirs-4.2.0/tests/test_android.py` & `platformdirs-4.2.1/tests/test_android.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,21 +64,21 @@
     }
     expected = expected_map[func]
 
     assert result == expected
 
 
 def test_android_folder_from_jnius(mocker: MockerFixture) -> None:
-    from platformdirs import PlatformDirs
-    from platformdirs.android import _android_folder
+    from platformdirs import PlatformDirs  # noqa: PLC0415
+    from platformdirs.android import _android_folder  # noqa: PLC0415
 
     _android_folder.cache_clear()
 
     if PlatformDirs is Android:
-        import jnius  # pragma: no cover
+        import jnius  # pragma: no cover # noqa: PLC0415
 
         autoclass = mocker.spy(jnius, "autoclass")  # pragma: no cover
     else:
         parent = MagicMock(return_value=MagicMock(getAbsolutePath=MagicMock(return_value="/A")))  # pragma: no cover
         context = MagicMock(getFilesDir=MagicMock(return_value=MagicMock(getParentFile=parent)))  # pragma: no cover
         autoclass = MagicMock(return_value=context)  # pragma: no cover
         mocker.patch.dict(sys.modules, {"jnius": MagicMock(autoclass=autoclass)})  # pragma: no cover
@@ -99,24 +99,24 @@
         "/data/user/1/a/files",
         "/data/data/a/files",
     ],
 )
 def test_android_folder_from_sys_path(mocker: MockerFixture, path: str, monkeypatch: pytest.MonkeyPatch) -> None:
     mocker.patch.dict(sys.modules, {"jnius": MagicMock(autoclass=MagicMock(side_effect=ModuleNotFoundError))})
 
-    from platformdirs.android import _android_folder
+    from platformdirs.android import _android_folder  # noqa: PLC0415
 
     _android_folder.cache_clear()
     monkeypatch.setattr(sys, "path", ["/A", "/B", path])
 
     result = _android_folder()
     assert result == path[: -len("/files")]
 
 
 def test_android_folder_not_found(mocker: MockerFixture, monkeypatch: pytest.MonkeyPatch) -> None:
     mocker.patch.dict(sys.modules, {"jnius": MagicMock(autoclass=MagicMock(side_effect=ModuleNotFoundError))})
 
-    from platformdirs.android import _android_folder
+    from platformdirs.android import _android_folder  # noqa: PLC0415
 
     _android_folder.cache_clear()
     monkeypatch.setattr(sys, "path", [])
     assert _android_folder() is None
```

### Comparing `platformdirs-4.2.0/tests/test_comp_with_appdirs.py` & `platformdirs-4.2.1/tests/test_comp_with_appdirs.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import appdirs
 import pytest
 
 import platformdirs
 
 
 def test_has_backward_compatible_class() -> None:
-    from platformdirs import AppDirs
+    from platformdirs import AppDirs  # noqa: PLC0415
 
     assert AppDirs is platformdirs.PlatformDirs
 
 
 def test_has_all_functions() -> None:
     # Get all public function names from appdirs
     appdirs_function_names = [f[0] for f in getmembers(appdirs, isfunction) if not f[0].startswith("_")]
```

### Comparing `platformdirs-4.2.0/tests/test_macos.py` & `platformdirs-4.2.1/tests/test_macos.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
 if TYPE_CHECKING:
     from pytest_mock import MockerFixture
 
 
 @pytest.fixture(autouse=True)
 def _fix_os_pathsep(mocker: MockerFixture) -> None:
-    """
-    If we're not actually running on macOS, set `os.pathsep` to what it should be on macOS.
-    """
+    """If we're not running on macOS, set `os.pathsep` to what it should be on macOS."""
     if sys.platform != "darwin":  # pragma: darwin no cover
         mocker.patch("os.pathsep", ":")
         mocker.patch("os.path.pathsep", ":")
 
 
 @pytest.mark.parametrize(
     "params",
```

### Comparing `platformdirs-4.2.0/tests/test_unix.py` & `platformdirs-4.2.1/tests/test_unix.py`

 * *Files identical despite different names*

### Comparing `platformdirs-4.2.0/LICENSE` & `platformdirs-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-4.2.0/README.rst` & `platformdirs-4.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-4.2.0/PKG-INFO` & `platformdirs-4.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: platformdirs
-Version: 4.2.0
-Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
+Version: 4.2.1
+Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a `user data dir`.
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
 License-File: LICENSE
@@ -32,14 +32,16 @@
 Requires-Dist: sphinx>=7.2.6; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: appdirs==1.4.4; extra == 'test'
 Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: pytest-cov>=4.1; extra == 'test'
 Requires-Dist: pytest-mock>=3.12; extra == 'test'
 Requires-Dist: pytest>=7.4.3; extra == 'test'
+Provides-Extra: type
+Requires-Dist: mypy>=1.8; extra == 'type'
 Description-Content-Type: text/x-rst
 
 The problem
 ===========
 
 .. image:: https://github.com/platformdirs/platformdirs/actions/workflows/check.yml/badge.svg
    :target: https://github.com/platformdirs/platformdirs/actions
```

