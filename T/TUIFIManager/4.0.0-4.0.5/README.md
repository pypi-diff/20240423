# Comparing `tmp/TUIFIManager-4.0.0.tar.gz` & `tmp/TUIFIManager-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TUIFIManager-4.0.0.tar", last modified: Sat Apr 20 09:35:48 2024, max compression
+gzip compressed data, was "TUIFIManager-4.0.5.tar", last modified: Tue Apr 23 17:46:12 2024, max compression
```

## Comparing `TUIFIManager-4.0.0.tar` & `TUIFIManager-4.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/
--rw-r--r--   0 xou       (1000) xou       (1000)      132 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.gitattributes
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.893235 TUIFIManager-4.0.0/.github/
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.896569 TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 xou       (1000) xou       (1000)      437 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 xou       (1000) xou       (1000)      604 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.896569 TUIFIManager-4.0.0/.github/workflows/
--rw-r--r--   0 xou       (1000) xou       (1000)      652 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.github/workflows/nox_ci.yml
--rw-r--r--   0 xou       (1000) xou       (1000)      605 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.gitignore
--rw-r--r--   0 xou       (1000) xou       (1000)      464 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.scrutinizer.yml
--rw-r--r--   0 xou       (1000) xou       (1000)      492 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/.sourcery.yaml
--rw-r--r--   0 xou       (1000) xou       (1000)     7729 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/CHANGELOG.md
--rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/LICENSE
--rw-r--r--   0 xou       (1000) xou       (1000)    10650 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)  1632442 2024-04-19 15:58:04.000000 TUIFIManager-4.0.0/Peek.gif
--rw-r--r--   0 xou       (1000) xou       (1000)     9552 2024-04-20 09:09:44.000000 TUIFIManager-4.0.0/README.md
--rw-r--r--   0 xou       (1000) xou       (1000)   246555 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/TUIFI.png
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/TUIFIManager/
--rw-r--r--   0 xou       (1000) xou       (1000)    31045 2024-04-20 08:55:24.000000 TUIFIManager-4.0.0/TUIFIManager/TUIFIProfile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     5509 2024-04-11 13:08:50.000000 TUIFIManager-4.0.0/TUIFIManager/TUIFile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     5044 2024-04-19 15:56:05.000000 TUIFIManager-4.0.0/TUIFIManager/TUIMenu.py
--rw-r--r--   0 xou       (1000) xou       (1000)     8377 2024-04-19 15:58:04.000000 TUIFIManager-4.0.0/TUIFIManager/TUISynthXDND.py
--rw-r--r--   0 xou       (1000) xou       (1000)    11793 2024-04-20 08:55:32.000000 TUIFIManager-4.0.0/TUIFIManager/TUItilities.py
--rw-r--r--   0 xou       (1000) xou       (1000)    73488 2024-04-20 09:24:19.000000 TUIFIManager-4.0.0/TUIFIManager/__init__.py
--rw-r--r--   0 xou       (1000) xou       (1000)     3109 2024-04-20 09:24:48.000000 TUIFIManager-4.0.0/TUIFIManager/__main__.py
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/TUIFIManager.egg-info/
--rw-r--r--   0 xou       (1000) xou       (1000)    10650 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)      700 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/SOURCES.txt
--rw-r--r--   0 xou       (1000) xou       (1000)        1 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/dependency_links.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       53 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/entry_points.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       36 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/requires.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       13 2024-04-20 09:35:48.000000 TUIFIManager-4.0.0/TUIFIManager.egg-info/top_level.txt
--rw-r--r--   0 xou       (1000) xou       (1000)     1497 2024-04-05 13:07:00.000000 TUIFIManager-4.0.0/flake.lock
--rw-r--r--   0 xou       (1000) xou       (1000)     1713 2024-04-05 19:20:12.000000 TUIFIManager-4.0.0/flake.nix
--rw-r--r--   0 xou       (1000) xou       (1000)      201 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/noxfile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     1093 2024-04-20 09:23:34.000000 TUIFIManager-4.0.0/pyproject.toml
--rw-r--r--   0 xou       (1000) xou       (1000)       40 2024-04-05 13:07:00.000000 TUIFIManager-4.0.0/requirements.txt
--rw-r--r--   0 xou       (1000) xou       (1000)     1272 2024-04-20 09:35:48.899902 TUIFIManager-4.0.0/setup.cfg
--rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-10-01 12:46:14.000000 TUIFIManager-4.0.0/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/
+-rw-r--r--   0 xou       (1000) xou       (1000)      132 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.gitattributes
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.919638 TUIFIManager-4.0.5/.github/
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.936304 TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 xou       (1000) xou       (1000)      437 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 xou       (1000) xou       (1000)      604 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/.github/workflows/
+-rw-r--r--   0 xou       (1000) xou       (1000)      652 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.github/workflows/nox_ci.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      605 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.gitignore
+-rw-r--r--   0 xou       (1000) xou       (1000)      464 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.scrutinizer.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      492 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/.sourcery.yaml
+-rw-r--r--   0 xou       (1000) xou       (1000)     7868 2024-04-22 12:52:13.000000 TUIFIManager-4.0.5/CHANGELOG.md
+-rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/LICENSE
+-rw-r--r--   0 xou       (1000) xou       (1000)    10668 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)  1632442 2024-04-19 15:58:04.000000 TUIFIManager-4.0.5/Peek.gif
+-rw-r--r--   0 xou       (1000) xou       (1000)     9570 2024-04-23 13:43:58.000000 TUIFIManager-4.0.5/README.md
+-rw-r--r--   0 xou       (1000) xou       (1000)   246555 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/TUIFI.png
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/TUIFIManager/
+-rw-r--r--   0 xou       (1000) xou       (1000)    31045 2024-04-23 17:34:12.000000 TUIFIManager-4.0.5/TUIFIManager/TUIFIProfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     5509 2024-04-11 13:08:50.000000 TUIFIManager-4.0.5/TUIFIManager/TUIFile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     5044 2024-04-19 15:56:05.000000 TUIFIManager-4.0.5/TUIFIManager/TUIMenu.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     8368 2024-04-23 15:42:02.000000 TUIFIManager-4.0.5/TUIFIManager/TUISynthXDND.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    11793 2024-04-20 08:55:32.000000 TUIFIManager-4.0.5/TUIFIManager/TUItilities.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    74525 2024-04-23 17:42:38.000000 TUIFIManager-4.0.5/TUIFIManager/__init__.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     3109 2024-04-23 17:45:25.000000 TUIFIManager-4.0.5/TUIFIManager/__main__.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/TUIFIManager.egg-info/
+-rw-r--r--   0 xou       (1000) xou       (1000)    10668 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)      700 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/SOURCES.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)        1 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/dependency_links.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       53 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/entry_points.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       36 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/requires.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       13 2024-04-23 17:46:12.000000 TUIFIManager-4.0.5/TUIFIManager.egg-info/top_level.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1497 2024-04-05 13:07:00.000000 TUIFIManager-4.0.5/flake.lock
+-rw-r--r--   0 xou       (1000) xou       (1000)     1792 2024-04-23 13:02:57.000000 TUIFIManager-4.0.5/flake.nix
+-rw-r--r--   0 xou       (1000) xou       (1000)      201 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/noxfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     1093 2024-04-23 17:43:22.000000 TUIFIManager-4.0.5/pyproject.toml
+-rw-r--r--   0 xou       (1000) xou       (1000)       40 2024-04-05 13:07:00.000000 TUIFIManager-4.0.5/requirements.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1272 2024-04-23 17:46:12.939638 TUIFIManager-4.0.5/setup.cfg
+-rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-10-01 12:46:14.000000 TUIFIManager-4.0.5/setup.py
```

### Comparing `TUIFIManager-4.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `TUIFIManager-4.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/.github/workflows/nox_ci.yml` & `TUIFIManager-4.0.5/.github/workflows/nox_ci.yml`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/.gitignore` & `TUIFIManager-4.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/CHANGELOG.md` & `TUIFIManager-4.0.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # v.DEVELOPMENT
 
+> [!NOTE]
+> **[CHANGELOG.md is archived, from now on version-logs are at releases](https://github.com/GiorgosXou/TUIFIManager/releases)**
+
 ------------------------
 # v.2.1.9
 - ***Fixed:***
 - - [`ALT_DOWN`](https://github.com/unicurses/unicurses/commit/a185cfb930d783f55c1efccd35e9ae23c0208a6e#diff-4f9493a5a3fb9e08d28013e7923bf5856d4368d076222caaa60c9a5e4a421f8c)
 - - [ncurses not found but existing on macOS](https://github.com/GiorgosXou/TUIFIManager/issues/28)
 - ***Improved:***
 - - [chunk_str method](https://github.com/GiorgosXou/TUIFIManager/pull/31)
```

### Comparing `TUIFIManager-4.0.0/LICENSE` & `TUIFIManager-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/PKG-INFO` & `TUIFIManager-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TUIFIManager
-Version: 4.0.0
+Version: 4.0.5
 Summary: A cross-platform terminal-based termux-oriented file manager.
 Home-page: https://github.com/GiorgosXou/TUIFIManager
 Author: George Chousos
 Author-email: gxousos@gmail.com
 License: General Public License v3.0
 Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
 Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
@@ -70,15 +70,15 @@
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
 
 # 📦 Features 
 ### • 📌 *Current:*
-- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`...')
+- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput PySide6 python-xlib`...')
 - Supports most common mouse events 
 - Can be used as a component
 - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM
 - Strong [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a NCurses\\PDCurses wrapper')
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
@@ -163,15 +163,15 @@
 
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
 </details>
 <details>
 <summary><i>How do I enable synthetic XDND?</i></summary>
 
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
 
 </details>
 <details>
 <summary><i>How do I set the default editor?</i></summary>
 
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.0 Summary: A cross-
+Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.5 Summary: A cross-
 platform terminal-based termux-oriented file manager. Home-page: https://
 github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
 gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
 https://github.com/GiorgosXou/TUIFIManager Keywords: file-
 manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
 platform Platform: unix Platform: linux Platform: osx Platform: cygwin
 Platform: windows Classifier: Intended Audience :: Developers Classifier:
@@ -27,17 +27,17 @@
 # âï¸ Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
 you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
 is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
 ``` for more details look into the `__main__.py` # ð¦ Features ### â¢ ð
 *Current:* - [Supports X11 Drag&Drop from terminals](#-customization 'set
-`tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6
-python-xlib`...') - Supports most common mouse events - Can be used as a
-component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
+`tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput
+PySide6 python-xlib`...') - Supports most common mouse events - Can be used as
+a component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
 [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a
 NCurses\\PDCurses wrapper') - It is pretty snappy - Supports [Termux](https://
 github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* - Macros
 - [Treeview](## 'Via a `WindowPad`') - Undo\Redo - Improved UI - Multiple tabs
 - [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/
 86#issuecomment-2016846146) - Effect on cutted Files - Multithread performance
 # â¨ï¸ Keybindings In `vim_mode` both normal and vim shortcuts work | Normal
@@ -77,16 +77,16 @@
 in `vim_mode`. In this case you can first press space-bar before proceeding
 with `owv` or with any other already reserved starting key, or just change it.
 **Additionally** there are also some "static" ones like the `m`+character which
 marks the current directory into the character, so you can navigate back to it
 by using \` or `;`+that_character # ð Documentation Work in progress
 ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
 `tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput
-PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests
+pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
 slightly, **use it as: Drag&drop + click afterwords where you want the file to
 be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
 discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
 issues/21) How do I set the default editor? > Set `tuifi_default_editor`
 enviroment variable to `vim` or whatever you prefer How do I disable the auto-
 find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
 to `False` How do I change the scroll sensitivity? > You can set either or both
```

### Comparing `TUIFIManager-4.0.0/Peek.gif` & `TUIFIManager-4.0.5/Peek.gif`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/README.md` & `TUIFIManager-4.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
 
 # 📦 Features 
 ### • 📌 *Current:*
-- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`...')
+- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput PySide6 python-xlib`...')
 - Supports most common mouse events 
 - Can be used as a component
 - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM
 - Strong [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a NCurses\\PDCurses wrapper')
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
@@ -134,15 +134,15 @@
 
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
 </details>
 <details>
 <summary><i>How do I enable synthetic XDND?</i></summary>
 
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
 
 </details>
 <details>
 <summary><i>How do I set the default editor?</i></summary>
 
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
```

#### html2text {}

```diff
@@ -12,17 +12,17 @@
 # âï¸ Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
 you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
 is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
 ``` for more details look into the `__main__.py` # ð¦ Features ### â¢ ð
 *Current:* - [Supports X11 Drag&Drop from terminals](#-customization 'set
-`tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6
-python-xlib`...') - Supports most common mouse events - Can be used as a
-component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
+`tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput
+PySide6 python-xlib`...') - Supports most common mouse events - Can be used as
+a component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
 [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a
 NCurses\\PDCurses wrapper') - It is pretty snappy - Supports [Termux](https://
 github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* - Macros
 - [Treeview](## 'Via a `WindowPad`') - Undo\Redo - Improved UI - Multiple tabs
 - [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/
 86#issuecomment-2016846146) - Effect on cutted Files - Multithread performance
 # â¨ï¸ Keybindings In `vim_mode` both normal and vim shortcuts work | Normal
@@ -62,16 +62,16 @@
 in `vim_mode`. In this case you can first press space-bar before proceeding
 with `owv` or with any other already reserved starting key, or just change it.
 **Additionally** there are also some "static" ones like the `m`+character which
 marks the current directory into the character, so you can navigate back to it
 by using \` or `;`+that_character # ð Documentation Work in progress
 ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
 `tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput
-PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests
+pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
 slightly, **use it as: Drag&drop + click afterwords where you want the file to
 be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
 discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
 issues/21) How do I set the default editor? > Set `tuifi_default_editor`
 enviroment variable to `vim` or whatever you prefer How do I disable the auto-
 find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
 to `False` How do I change the scroll sensitivity? > You can set either or both
```

### Comparing `TUIFIManager-4.0.0/TUIFI.png` & `TUIFIManager-4.0.5/TUIFI.png`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/TUIFIManager/TUIFIProfile.py` & `TUIFIManager-4.0.5/TUIFIManager/TUIFIProfile.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/TUIFIManager/TUIFile.py` & `TUIFIManager-4.0.5/TUIFIManager/TUIFile.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/TUIFIManager/TUIMenu.py` & `TUIFIManager-4.0.5/TUIFIManager/TUIMenu.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/TUIFIManager/TUISynthXDND.py` & `TUIFIManager-4.0.5/TUIFIManager/TUISynthXDND.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 import re
 
 
 
 class writerr(object):
     def write(self, data): # Ignore warning
-        if not data == "sys:1: Warning: g_main_context_pop_thread_default: assertion 'stack != NULL' failed\n":
+        if not data.endswith("g_main_context_pop_thread_default: assertion 'stack != NULL' failed\n"):
             print(data)
 
 sys.stderr = writerr() # WARN: pyside\qt getting wild, cause cutie aint thread safe | VERY SuS thought
 
 # os.environ['QT_LOGGING_RULES'] = 'qt.qpa.input*.debug=false; *.debug=false; qt.*.debug=false; driver.*.debug=false'
 # os.environ["QT_LOGGING_RULES"] = '*.debug=false;qt.accessibility.cache.warning=false;qt.qpa.events.warning=false;qt.qpa.fonts.warning=false;qt.qpa.gl.warning=false;qt.qpa.input.devices.warning=false;qt.qpa.screen.warning=false;qt.qpa.xcb.warning=false;qt.text.font.db.warning=false;qt.xkb.compose.warning=false' # https://stackoverflow.com/questions/68809878/how-do-you-silence-console-messages-from-matplotlib-with-pyqt5-backend
```

### Comparing `TUIFIManager-4.0.0/TUIFIManager/TUItilities.py` & `TUIFIManager-4.0.5/TUIFIManager/TUItilities.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/TUIFIManager/__init__.py` & `TUIFIManager-4.0.5/TUIFIManager/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from     contextlib import contextmanager
 from     send2trash import send2trash
 from      functools import partial
 from        pathlib import Path
 from         typing import Optional, Final
 from           time import time
-from             os import sep, access, W_OK
+from             os import sep, access, W_OK, R_OK
 from           math import log10
 from        os.path import basename
 from       .TUIMenu import TUIMenu
 from       .TUIFile import TUIFile
 from   .TUItilities import WindowPad, Cd, Label, END_MOUSE, BEGIN_MOUSE, BEGIN_MOUSE, END_MOUSE, IS_WINDOWS, HOME_DIR, IS_TERMUX
 from  .TUIFIProfile import TUIFIProfiles, DEFAULT_PROFILE , DEFAULT_WITH, DEFAULT_OPENER
 import   subprocess
@@ -19,15 +19,15 @@
 import       shutil
 import       signal
 import         json
 import          ast
 import           re
 import           os
 
-__version__: Final[str] = "4.0.0"
+__version__: Final[str] = "4.0.5"
 
 PADDING_LEFT   = 2
 PADDING_RIGHT  = 2
 PADDING_TOP    = 1
 PADDING_BOTTOM = 0
 
 SCROLL_SENSITIVITY      = int(os.getenv('tuifi_scroll_sensitivity'     , 1))
@@ -259,14 +259,17 @@
         self.files.append(file_)
         self.__set_coordinates(file_)
 
 
     basename = ''
     def load_files(self, directory, suffixes=[]):  # DON'T load and then don't show :P
         directory = os.path.realpath(os.path.normpath(directory))
+        if not access(directory, R_OK):
+            self.__set_label_text(f'NO READ PERMISSION: "{directory}"')
+            return []
         if not os.path.isdir(directory):
             raise FileNotFoundError(f'DirectoryNotFound: "{directory}"')
         if not suffixes:
             suffixes = self.suffixes
 
         order = self.get_order_of(directory)
         self.is_order_reversed = order[1]
@@ -404,17 +407,17 @@
 
         multiple = self.__count_selected > 1
         if not os.path.isdir(directory) or multiple: # if there is at least one file that it is not a directory OR multiple selected files that they are whatever, then: ... (Now it makes sense why `not isdir`)
             prof = f'/{os.path.splitext(directory)[1][1:]}'
             open_with = TUIFIProfiles.get(prof, DEFAULT_PROFILE).open_with
             return self.__try_open_with(directory, open_with, multiple) # TODO: check if the multiple selected files are folders and open them in new tabs
 
-        self.__reset_open()
-        self.load_files(directory, suffixes)
+        if not self.load_files(directory, suffixes): return []
         if not self.is_in_find_mode: self.__set_label_text(f'[{len(self.files)-1:04}]' + (' [▼] ' if self.is_order_reversed else ' [▲] ') + directory ) # just because i know that len is stored as variable,  that's why i don;t count them in for loop
+        self.__reset_open()
         self.draw()
         return self.files
 
 
     def refresh(self):
         super().refresh()
         self.menu.refresh()
@@ -549,27 +552,32 @@
                     if f.is_selected:
                         f_list.append(QUrl.fromLocalFile(self.directory + sep + f.name))
                 return f_list
             elif self.__pre_pressed_file:
                 return [QUrl.fromLocalFile(self.directory + sep + self.__pre_pressed_file.name)]
 
 
-        def handle_gui_to_tui_dropped_file(self, file_url, type): #TODO: Custom user actions on link patterns: eg. clone git, save at folder xy, etc.
+        def handle_gui_to_tui_dropped_file(self, file_url, type): #TODO: Custom user actions on link patterns: eg. clone git, save at folder xy, etc. + TODO: if dropped on folder
+            self.is_focused = False
             self.__set_label_text(f'DROPPED: {file_url}')
             if type == 1:
-                self.__set_label_text("It's on the todo list :P") #TODO: handle files
+                name = os.path.basename(file_url)
+                shutil.move(file_url, self.directory + sep + name)
+                self.__sub_handle_creation_of(name, self.get_profile(file_url)) # TODO: for other non \file_extensions
+                self.__set_label_text(f'MOVED: {name}')
+                self.refresh() #for some reason refresh is needed that's SuS. Should look on download too
             elif type == 0:
                 self.download(file_url, self.directory + sep)
             elif file_url.startswith('data:') and not file_url.find('base64') == -1:
                 extension = mimetypes.guess_extension(file_url.split(';')[0].split(':')[1])
                 filename = self.get_available_filename('download'+extension)
                 self.save(self.directory, filename, base64.b64decode(file_url[file_url.find('4')+1:])) # 4 is from base64
             else:
                 self.__set_label_text(f'DROPPED UNHANDLED: {file_url}')
-
+            self.is_focused = True
                 # r = requests.get(file_url) # , stream=True
                 # r.headers.get('filename')
                 # unicurses.mvwaddwstr(self.pad,0,0,f'is downloadable: {r.headers}')
 
                 # from urllib.request import urlopen 
                 # response = urlopen(file_url)
                 # filename = response.headers.get_filename()
@@ -808,15 +816,15 @@
         """
         self.__is_cut = False
         self.__stack_files_for_action()
 
 
     def __set_label_on_copy(self,size):
         length = len(self.__temp__copied_files)
-        text   = f'{length} files [{size} bytes]' if length > 1 else f'{self.__temp__copied_files[0].name}'  
+        text   = f'{length} files [{self.convert_bytes(size)}]' if length > 1 else f'{self.__temp__copied_files[0].name}'
         action = 'CUTED' if self.__is_cut else 'COPIED'
         self.__set_label_text(f'[{action}]: {text}')
 
 
     def __stack_files_for_action(self):
         """
         this function is TEMPORARY and will be REMOVED,
@@ -975,14 +983,15 @@
             self.__clicked_file                 = self.files[i]
             return False
         elif event in (unicurses.KEY_ENTER,10,unicurses.KEY_RESIZE,unicurses.KEY_MOUSE,unicurses.KEY_HOME , unicurses.KEY_DC) or unicurses.keyname(event) in ('kxOUT','kxIN'): # Ignore this shit :P
             return False
         else:
             self.__temp_findname += unicurses.RCCHAR(event)
 
+        self.__pre_hov = None
         self.find_file(self.__temp_findname)
         self.__set_label_text(f'SEARCH: {self.__temp_findname}')
         i = 0 if len(self.files) == 1 else 1
         self.__clicked_file          = self.files[i]
         self.__index_of_clicked_file = i
 
         self.scroll_to_file(self.__clicked_file, True, True)
@@ -1241,20 +1250,29 @@
 
     def create_new_file  (self): self.create_new('file'  )
     def create_new_folder(self): self.create_new('folder')
 
     def __int_len(self, n): # https://stackoverflow.com/a/2189827/11465149
         return int(log10(n))+1 if n != 0 else 0
 
+    size_units = ('bytes', 'KB', 'MB', 'GB', 'TB')
+    def convert_bytes(self, num): #WARN: https://stackoverflow.com/a/63839503/11465149 | https://stackoverflow.com/a/78117390/11465149
+        step_unit = 1000.0
+        for x in self.size_units:
+            if num < step_unit:
+                if x[0] == 'b': return "%i %s" % (num, x)
+                return "%3.1f %s" % (num, x)
+            num /= step_unit
+
     def __set_label_on_file_selection(self, index=None, file=None):
         if not self.info_label: return
         file = file if file else self.__clicked_file
         index= index if index else self.__index_of_clicked_file
         path = self.directory + sep + file.name
-        info = f'[{os.path.getsize(path)} bytes]' if os.path.isfile(path) else ''
+        info = f'[{self.convert_bytes(os.path.getsize(path))}]' if os.path.isfile(path) else ''
         offset = self.__int_len(max(len(self.files),999)) + 3 + self.__int_len(index) + 3 + len(info) + 2
         self.info_label.text = f'[{len(self.files) - 1:04}] [{index}] {path[max(len(path) - self.info_label.width + offset, 0):]} {info}'
         # just because i know that len is stored as variable,  that's why i don;t count them in for loop
 
     def __open_clicked_file(self):
         return self.open(self.__clicked_file)
```

### Comparing `TUIFIManager-4.0.0/TUIFIManager/__main__.py` & `TUIFIManager-4.0.5/TUIFIManager/__main__.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/TUIFIManager.egg-info/PKG-INFO` & `TUIFIManager-4.0.5/TUIFIManager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TUIFIManager
-Version: 4.0.0
+Version: 4.0.5
 Summary: A cross-platform terminal-based termux-oriented file manager.
 Home-page: https://github.com/GiorgosXou/TUIFIManager
 Author: George Chousos
 Author-email: gxousos@gmail.com
 License: General Public License v3.0
 Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
 Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
@@ -70,15 +70,15 @@
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
 
 # 📦 Features 
 ### • 📌 *Current:*
-- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`...')
+- [Supports X11 Drag&Drop from terminals](#-customization 'set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput PySide6 python-xlib`...')
 - Supports most common mouse events 
 - Can be used as a component
 - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM
 - Strong [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a NCurses\\PDCurses wrapper')
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
@@ -163,15 +163,15 @@
 
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
 </details>
 <details>
 <summary><i>How do I enable synthetic XDND?</i></summary>
 
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it slightly, **use it as: Drag&drop + click afterwords where you want the file to be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/issues/21)
 
 </details>
 <details>
 <summary><i>How do I set the default editor?</i></summary>
 
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.0 Summary: A cross-
+Metadata-Version: 2.1 Name: TUIFIManager Version: 4.0.5 Summary: A cross-
 platform terminal-based termux-oriented file manager. Home-page: https://
 github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
 gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
 https://github.com/GiorgosXou/TUIFIManager Keywords: file-
 manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
 platform Platform: unix Platform: linux Platform: osx Platform: cygwin
 Platform: windows Classifier: Intended Audience :: Developers Classifier:
@@ -27,17 +27,17 @@
 # âï¸ Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
 you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
 is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
 ``` for more details look into the `__main__.py` # ð¦ Features ### â¢ ð
 *Current:* - [Supports X11 Drag&Drop from terminals](#-customization 'set
-`tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput PySide6
-python-xlib`...') - Supports most common mouse events - Can be used as a
-component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
+`tuifi_synth_dnd` enviroment variable to `True`. `pip install requests pynput
+PySide6 python-xlib`...') - Supports most common mouse events - Can be used as
+a component - Uses about [~30MB](## '80mb with synthetic xdnd') of RAM - Strong
 [C TUI backend](https://github.com/unicurses/unicurses 'Via Uni-Curses, a
 NCurses\\PDCurses wrapper') - It is pretty snappy - Supports [Termux](https://
 github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* - Macros
 - [Treeview](## 'Via a `WindowPad`') - Undo\Redo - Improved UI - Multiple tabs
 - [Sixel support](https://github.com/GiorgosXou/TUIFIManager/issues/
 86#issuecomment-2016846146) - Effect on cutted Files - Multithread performance
 # â¨ï¸ Keybindings In `vim_mode` both normal and vim shortcuts work | Normal
@@ -77,16 +77,16 @@
 in `vim_mode`. In this case you can first press space-bar before proceeding
 with `owv` or with any other already reserved starting key, or just change it.
 **Additionally** there are also some "static" ones like the `m`+character which
 marks the current directory into the character, so you can navigate back to it
 by using \` or `;`+that_character # ð Documentation Work in progress
 ð ï¸ð ... # ð­ Customization How do I enable vim_mode? > Set
 `tuifi_vim_mode` enviroment variable to `True` How do I enable synthetic XDND?
-> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install pynput
-PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
+> set `tuifi_synth_dnd` enviroment variable to `True`. `pip install requests
+pynput PySide6 python-xlib`. Know it's expirimental! You'll need to adapt to it
 slightly, **use it as: Drag&drop + click afterwords where you want the file to
 be dropped.** [See also](https://github.com/GiorgosXou/TUIFIManager/
 discussions/92) and [this issue](https://github.com/GiorgosXou/TUIFIManager/
 issues/21) How do I set the default editor? > Set `tuifi_default_editor`
 enviroment variable to `vim` or whatever you prefer How do I disable the auto-
 find-mode? > You can just set `tuifi_auto_find_on_typing` enviroment variable
 to `False` How do I change the scroll sensitivity? > You can set either or both
```

### Comparing `TUIFIManager-4.0.0/TUIFIManager.egg-info/SOURCES.txt` & `TUIFIManager-4.0.5/TUIFIManager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/flake.lock` & `TUIFIManager-4.0.5/flake.lock`

 * *Files identical despite different names*

### Comparing `TUIFIManager-4.0.0/flake.nix` & `TUIFIManager-4.0.5/flake.nix`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,20 @@
   };
 
   outputs = {
     self,
     nixpkgs,
     flake-utils,
   }:
-    flake-utils.lib.eachSystem ["x86_64-linux"] (system: let
+    flake-utils.lib.eachSystem [
+      "x86_64-linux"
+      "aarch64-linux"
+      "aarch64-darwin"
+      "x86_64-darwin"
+    ] (system: let
       pkgs = nixpkgs.legacyPackages.${system};
     in {
       devShells.default = let
         py-env = pkgs.python310.withPackages (p: [
           p.send2trash
           p.unicurses
         ]);
```

### Comparing `TUIFIManager-4.0.0/pyproject.toml` & `TUIFIManager-4.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TUIFIManager"
-version = "4.0.0"
+version = "4.0.5"
 
 description = "A cross-platform terminal-based termux-oriented file manager."
 requires-python = ">=3.8"
 readme = "README.md"
 
 dependencies = [
     "uni-curses >= 2.1.3",
```

### Comparing `TUIFIManager-4.0.0/setup.cfg` & `TUIFIManager-4.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TUIFIManager
-version = 4.0.0
+version = 4.0.5
 description = A cross-platform terminal-based termux-oriented file manager
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 author = George Chousos
 author_email = gxousos@gmail.com
 keywords = file-manager, terminal, tui, ncurses, pdcurses, uni-curses, termux, vim, vim-motions, cross-platform
 license = GPL-3.0
```

