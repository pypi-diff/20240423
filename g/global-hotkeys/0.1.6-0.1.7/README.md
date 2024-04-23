# Comparing `tmp/global_hotkeys-0.1.6.tar.gz` & `tmp/global_hotkeys-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.1.6.tar", last modified: Wed Jun 21 13:56:57 2023, max compression
+gzip compressed data, was "global_hotkeys-0.1.7.tar", last modified: Tue Apr 23 07:29:15 2024, max compression
```

## Comparing `global_hotkeys-0.1.6.tar` & `global_hotkeys-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:56:57.178704 global_hotkeys-0.1.6/
--rw-rw-rw-   0        0        0     1703 2023-06-21 13:56:24.000000 global_hotkeys-0.1.6/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0    10028 2023-06-21 13:56:57.178704 global_hotkeys-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     7791 2023-06-21 13:13:54.000000 global_hotkeys-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 13:56:57.160699 global_hotkeys-0.1.6/global_hotkeys/
--rw-rw-rw-   0        0        0     4476 2023-06-21 13:47:36.000000 global_hotkeys-0.1.6/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0    10304 2023-06-21 12:58:55.000000 global_hotkeys-0.1.6/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.6/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:56:57.174704 global_hotkeys-0.1.6/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0    10028 2023-06-21 13:56:57.000000 global_hotkeys-0.1.6/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-06-21 13:56:57.000000 global_hotkeys-0.1.6/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:56:57.000000 global_hotkeys-0.1.6/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 13:56:57.000000 global_hotkeys-0.1.6/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 13:56:57.000000 global_hotkeys-0.1.6/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 13:56:57.178704 global_hotkeys-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-06-21 13:56:30.000000 global_hotkeys-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 13:56:57.177701 global_hotkeys-0.1.6/tests/
--rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.6/tests/_t.py
--rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.6/tests/global_snippets.py
--rw-rw-rw-   0        0        0     2091 2023-06-21 13:05:55.000000 global_hotkeys-0.1.6/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:29:15.962646 global_hotkeys-0.1.7/
+-rw-rw-rw-   0        0        0     1816 2024-04-23 07:24:56.000000 global_hotkeys-0.1.7/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    13486 2024-04-23 07:29:15.961646 global_hotkeys-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    10760 2024-04-23 07:24:22.000000 global_hotkeys-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 07:29:15.925648 global_hotkeys-0.1.7/global_hotkeys/
+-rw-rw-rw-   0        0        0     4476 2023-06-21 13:47:36.000000 global_hotkeys-0.1.7/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0    11125 2024-04-23 06:49:51.000000 global_hotkeys-0.1.7/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0      304 2024-04-23 06:55:28.000000 global_hotkeys-0.1.7/global_hotkeys/keycode_checker.py
+-rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.7/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:29:15.946648 global_hotkeys-0.1.7/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0    13486 2024-04-23 07:29:15.000000 global_hotkeys-0.1.7/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      417 2024-04-23 07:29:15.000000 global_hotkeys-0.1.7/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 07:29:15.000000 global_hotkeys-0.1.7/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-23 07:29:15.000000 global_hotkeys-0.1.7/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-23 07:29:15.000000 global_hotkeys-0.1.7/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 07:29:15.962646 global_hotkeys-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-04-23 06:55:32.000000 global_hotkeys-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 07:29:15.959648 global_hotkeys-0.1.7/tests/
+-rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.7/tests/_t.py
+-rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.7/tests/global_snippets.py
+-rw-rw-rw-   0        0        0     2132 2024-04-23 06:46:39.000000 global_hotkeys-0.1.7/tests/test.py
```

### Comparing `global_hotkeys-0.1.6/CHANGELOG.txt` & `global_hotkeys-0.1.7/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Change Log
 ==========
 
+0.1.7 (4/23/2024)
+-----------------
+- Support added for specifying keycodes directly inside of keybindings.
+
 0.1.6 (6/21/2023)
 -----------------
 - Changelog updated.
 
 0.1.5 (6/21/2023)
 -----------------
 - Minor fix to the register_hotkey function.
```

### Comparing `global_hotkeys-0.1.6/LICENSE.txt` & `global_hotkeys-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.6/PKG-INFO` & `global_hotkeys-0.1.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,394 +1,376 @@
-Metadata-Version: 2.1
-Name: global_hotkeys
-Version: 0.1.6
-Home-page: https://github.com/btsdev
-Author: btsdev
-Author-email: btsdevman@gmail.com
-License: MIT
-Keywords: hotkeys,shortcuts
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
-# Python Global Hotkey Bindings for Windows
-
-Use this library to set system wide keybindings for your code to respond to.
-
-## Installation
-
-```
-pip install global-hotkeys -U
-```
-
-## Example usage
-
-```python
-from global_hotkeys import *
-
-import time
-
-# Flag to indicate whether the program should continue running.
-is_alive = True
-
-def print_hello():
-    print("Hello")
-
-def print_world():
-    print("World")
-
-def print_foo():
-    print("Foo")
-
-def print_bar():
-    print("Bar")
-
-def print_with_params(params):
-    print(params["test"])
-
-def press_with_params(params):
-    print(params["press_param"])
-
-def release_with_params(params):
-    print(params["release_param"])
-
-def exit_application():
-    global is_alive
-    print("exiting")
-    stop_checking_hotkeys()
-    is_alive = False
-
-
-# Declare some key bindings.
-bindings = [
-    ["control + 7, control + 4", None, print_world, True],
-    ["control + 5", None, print_hello, False],
-    ["control + 6", None, print_with_params, False, {"test":5}],
-    [
-        "control + 8", 
-        press_with_params, 
-        release_with_params, 
-        False, 
-        {"press_param":"pressed!"}, 
-        {"release_param": "released!"}
-    ],
-    # dict style
-    {
-        "hotkey": "control + 4",
-        "on_press_callback": None,
-        "on_release_callback": print_with_params,
-        "actuate_on_partial_release": False,
-        "callback_params": {"test": "testing"},
-
-    },
-    # dict style with differentiating params for press and release callbacks
-    {
-        "hotkey": "control + 9",
-        "on_press_callback": press_with_params,
-        "on_release_callback": release_with_params,
-        "actuate_on_partial_release": False,
-        "press_callback_params": {"press_param":"ctrl+9 pressed!"},
-        "release_callback_params": {"release_param": "ctrl+9 released!"},
-
-    },
-
-    ["window + 1", None, print_foo, False],
-    ["t,m", None, print_bar, False],
-    ["control + Q", None, exit_application, False],
-]
-
-# Bindings take on the form of:
-#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag, callback_params
-#
-# *Note that callback_params will be passed to both press and release callback functions
-#
-# Or in explicit dict format:
-# {
-#     "hotkey": <binding>,
-#     "on_press_callback": <press_callback>,
-#     "on_release_callback": <release_callback>,
-#     "actuate_on_partial_release": False | True,
-#     "callback_params": <a variable or expression can go here>  <-- This applies to both callbacks.
-#     "press_callback_params": <a variable or expression can go here>
-#     "release_callback_params": <a variable or expression can go here>
-# }
-
-# It's useful to have 'actuate_on_partial_release_flag' set to False, 
-# so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
-
-# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
-# and additional key chords are separated by commas. Spaces are ignored.
-
-# Register all of our keybindings
-register_hotkeys(bindings)
-
-# Finally, start listening for keypresses
-start_checking_hotkeys()
-
-# Keep waiting until the user presses the exit_application keybinding.
-# Note that the hotkey listener will exit when the main thread does.
-while is_alive:
-    time.sleep(0.1)
-```
-
-## Also note that I've included a simple global snippets example using this functionality.
-It's in the `tests` folder if you download this project's source from [GitHub](https://github.com/btsdev/global_hotkeys).
-
-It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
-
-It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
-
-Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
-
-### Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
-I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
-
-## Additional functionality
-
-You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
-
-```python
-
-# Just reusing our bindings declaration from above (this is not a complete code example, btw).
-bindings = [
-    ["control + 7, control + 4", None, print_world, True],
-    ["control + 5", None, print_hello, False],
-    ["window + 1", None, print_foo, False],
-    ["t,m", None, print_bar, False],
-    ["control + Q", None, exit_application, False],
-]
-
-# Register a single keybinding (if it's not already registered). 
-# Returns True if the key didn't already exist and was added, 
-# else False (the binding is already registered - remove it first if 
-# you wish to overwrite it with new event handlers).
-register_hotkey(bindings[0])
-
-# Remove a single keybinding (if it exists). 
-# Returns True if the key existed and was removed, else False (the binding is already gone).
-remove_hotkey(bindings[0])
-
-# Register a list of keybindings.
-register_hotkeys(bindings)
-
-# Remove a list of keybindings.
-remove_hotkeys(bindings)
-
-# Remove all keybindings and terminate the hotkey listener thread.
-clear_hotkeys()
-```
-
-## List of the available keys
-
-```
-backspace
-tab
-clear
-enter
-shift
-control
-alt
-pause
-caps_lock
-escape
-space
-page_up
-page_down
-left_window
-right_window
-window
-end
-home
-left
-up
-right
-down
-select
-print
-execute
-enter
-print_screen
-insert
-delete
-help
-0
-1
-2
-3
-4
-5
-6
-7
-8
-9
-a
-b
-c
-d
-e
-f
-g
-h
-i
-j
-k
-l
-m
-n
-o
-p
-q
-r
-s
-t
-u
-v
-w
-x
-y
-z
-numpad_0
-numpad_1
-numpad_2
-numpad_3
-numpad_4
-numpad_5
-numpad_6
-numpad_7
-numpad_8
-numpad_9
-multiply_key
-add_key
-separator_key  <-- '|' also known as the 'pipe'
-|
-subtract_key
-decimal_key
-divide_key
-f1
-f2
-f3
-f4
-f5
-f6
-f7
-f8
-f9
-f10
-f11
-f12
-f13
-f14
-f15
-f16
-f17
-f18
-f19
-f20
-f21
-f22
-f23
-f24
-num_lock
-scroll_lock
-left_shift
-right_shift
-left_control
-right_control
-left_menu
-right_menu
-browser_back
-browser_forward
-browser_refresh
-browser_stop
-browser_search
-browser_favorites
-browser_start_and_home
-volume_mute
-volume_Down
-volume_up
-next_track
-previous_track
-stop_media
-play/pause_media
-start_mail
-select_media
-start_application_1
-start_application_2
-attn_key
-crsel_key
-exsel_key
-play_key
-zoom_key
-clear_key
-+
-,
--
-.
-/
-`
-;
-[
-\
-]
-'
-`
-```
-
-Change Log
-==========
-
-0.1.6 (6/21/2023)
------------------
-- Changelog updated.
-
-0.1.5 (6/21/2023)
------------------
-- Minor fix to the register_hotkey function.
-
-0.1.4 (6/21/2023)
------------------
-- Added optional press and release callback parameter differentiation. Merged fix for press callback function.
-
-0.1.3 (5/28/2023)
------------------
-- Implemented retrofitting for the original hotkey style: e.g. ["control", "alt", "z"]. This is converted automatically to "control + alt + z".
-
-0.1.2 (5/28/2023)
------------------
-- Added dict binding format support. Also added support for supplying callback parameters for bindings.
-
-0.1.1 (5/28/2023)
------------------
-- Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
-
-0.1.0 (5/28/2023)
------------------
-- Code refactoring. Hotkey formatting is updated. Key chord sequences now supported. Now providing option to actuate release callback either on partial release of the last key chord, or on full release of all keys in the last keychord (though if the windows modifier key is used, unfortunately it still just actuates immediately on partial release).
-
-0.0.6 (5/27/2023)
------------------
-- Fixed window key detection.
-
-0.0.5 (5/27/2023)
------------------
-- Fixed unwanted modifier keys bug. Added pywin32 as dependency.
-
-0.0.4 (12/1/2020)
------------------
-- Fixed Development Status: It's now set to Beta.
-
-0.0.3 (12/1/2020)
------------------
-- Readme update: Added some clarification in the example usage.
-
-0.0.2 (12/1/2020)
------------------
-- Readme update.
-
-0.0.1 (12/1/2020)
------------------
-- First Release
+# Python Global Hotkey Bindings for Windows
+
+Use this library to set system wide keybindings for your code to respond to.
+
+## Installation
+
+```
+pip install global-hotkeys -U
+```
+
+## Example usage
+
+```python
+from global_hotkeys import *
+
+import time
+
+# Flag to indicate whether the program should continue running.
+is_alive = True
+
+def print_hello():
+    print("Hello")
+
+def print_world():
+    print("World")
+
+def print_foo():
+    print("Foo")
+
+def print_bar():
+    print("Bar")
+
+def print_with_params(params):
+    print(params["test"])
+
+def press_with_params(params):
+    print(params["press_param"])
+
+def release_with_params(params):
+    print(params["release_param"])
+
+def exit_application():
+    global is_alive
+    print("exiting")
+    stop_checking_hotkeys()
+    is_alive = False
+
+
+# Declare some key bindings.
+bindings = [
+    ["control + 7, control + 4", None, print_world, True],
+    # You can use direct keycodes as well (useful for non-US keyboard layouts):
+    ["control + 0x35", None, print_hello, False], # 0x35 is the keycode for the '5' key
+    ["control + 6", None, print_with_params, False, {"test":5}],
+    [
+        "control + 8", 
+        press_with_params, 
+        release_with_params, 
+        False, 
+        {"press_param":"pressed!"}, 
+        {"release_param": "released!"}
+    ],
+    # dict style
+    {
+        "hotkey": "control + 4",
+        "on_press_callback": None,
+        "on_release_callback": print_with_params,
+        "actuate_on_partial_release": False,
+        "callback_params": {"test": "testing"},
+
+    },
+    # dict style with differentiating params for press and release callbacks
+    {
+        "hotkey": "control + 9",
+        "on_press_callback": press_with_params,
+        "on_release_callback": release_with_params,
+        "actuate_on_partial_release": False,
+        "press_callback_params": {"press_param":"ctrl+9 pressed!"},
+        "release_callback_params": {"release_param": "ctrl+9 released!"},
+
+    },
+
+    ["window + 1", None, print_foo, False],
+    ["t,m", None, print_bar, False],
+    ["control + Q", None, exit_application, False],
+]
+
+# Bindings take on the form of:
+#   <binding>, on_press_callback, on_release_callback, actuate_on_partial_release_flag, callback_params
+#
+# *Note that callback_params will be passed to both press and release callback functions
+#
+# Or in explicit dict format:
+# {
+#     "hotkey": <binding>,
+#     "on_press_callback": <press_callback>,
+#     "on_release_callback": <release_callback>,
+#     "actuate_on_partial_release": False | True,
+#     "callback_params": <a variable or expression can go here>  <-- This applies to both callbacks.
+#     "press_callback_params": <a variable or expression can go here>
+#     "release_callback_params": <a variable or expression can go here>
+# }
+
+# It's useful to have 'actuate_on_partial_release_flag' set to False, 
+# so your modifier keys don't get in the way of any automatic keyboard output you're doing in response.
+
+# Note the actual hotkey syntax. Key combinations are denoted via the '+' character, 
+# and additional key chords are separated by commas. Spaces are ignored.
+
+# Register all of our keybindings
+register_hotkeys(bindings)
+
+# Finally, start listening for keypresses
+start_checking_hotkeys()
+
+# Keep waiting until the user presses the exit_application keybinding.
+# Note that the hotkey listener will exit when the main thread does.
+while is_alive:
+    time.sleep(0.1)
+```
+
+## Explanation of the binding structure
+
+Let's go in more details on how the binding is structured, You have two options either to declare the binding explicitly like this within curly brackets:
+```
+# {
+#     "hotkey": <binding>,
+#     "on_press_callback": <press_callback>,
+#     "on_release_callback": <release_callback>,
+#     "actuate_on_partial_release": False | True,
+#     "callback_params": 1ms": <a variable or expression can go here>
+#     "release_callback_params": <a variable or expression can go here>
+# }
+```
+
+Or implicitly by the position of the parameter:
+```
+["hotkey", on_press_callback, on_release_callback, actuate_on_partial_release,press_callback_params,release_callback_params]
+```
+- **hotkey:** A string representing the key combination that triggers the callbacks, such as "control + 7, control + 4".
+- **on_press_callback:** The function to be called when the hotkey is pressed. Can be None or a function reference.
+- **on_release_callback:** The function to be called when the hotkey is released. Can be None or a function reference.
+- **actuate_on_partial_release:** A boolean indicating whether the release callback should be triggered on a partial release of the key combination.
+- **callback_params:** Parameters to be passed to both the press and release callbacks. This should be a dictionary.
+- **press_callback_params, release_callback_params:** Parameters specifically for the press,release callbacks. This should be a dictionary (key-value pairs Like in this example ```"press_callback_params": {"press_param":"ctrl+9 pressed!"}```) .
+
+## If you are on a non-US keyboard layout...
+You may need to manually figure out the keycodes for the keys you want to bind to, and use those keycodes directly instead of the keynames in your bindings. I've included a useful utility for doing so. 
+
+Just open an interactive shell, and import my keycode_checker module to begin figuring out what your desired keys' keycodes are.
+```python
+>>> from global_hotkeys import keycode_checker
+```
+You'll see the `Press any key (Ctrl+C to exit)` prompt and can begin pressing keys until you've gathered your desired keycodes:
+```
+Key pressed: a
+VK Code: 0x1E
+Key pressed: b
+VK Code: 0x30
+```
+
+And in your code that's actually setting up keybindings maybe you'd use something like:
+```python
+# Assume our previous example setup code from above
+bindings = [
+    ["control + 0x1E", None, print_hello, False],
+    # whatever other bindings...
+]
+```
+
+That said, if your modifier keys' keycodes (e.g. for control, shift, alt) are different than what's listed in [keycodes.py](https://github.com/btsdev/global_hotkeys/blob/master/global_hotkeys/keycodes.py), you'll likely need to just fork this project and modify the source to make things work. CD into your forked copy of the repos and use `pip install -e ./` to apply your changes as you experiment and use your forked version of the library instead. Certainly not a perfect solution, admittedly...
+
+As the code needs to differentiate between modifier keys and non-modifier keys, some further update may be necessary to allow for changing/specifying modifier keycodes as well for non-US keyboard layouts.
+
+## Also note that I've included a simple global snippets example using this functionality.
+It's in the `tests` folder if you download this project's source from [GitHub](https://github.com/btsdev/global_hotkeys).
+
+It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
+
+It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
+
+Also, it uses the winsound library's Beep function to emit a low and subtle visual cue to indicate whether you just toggled the global snippets on or off.
+
+### Try setting up and using the Hyperkey to avoid hotkey conflicts with your applications.
+I personally use the Hyperkey (which is basically Window+Control+Shift+Alt and also known as the 'OfficeKey' on keyboards that have actually have it) to avoid clashing with most applications' own hotkeys, which is normally not available in windows, but it can be setup using [Autohotkey](https://stackoverflow.com/questions/40435980/how-to-emulate-hyper-key-in-windows-10-using-autohotkey) and also applying the [OfficeKeyFix](https://github.com/anthonyheddings/OfficeKeyFix) which you'll need to compile yourself if one is interested. You can read more about the officekey issue on [Super User](https://superuser.com/questions/1455857/how-to-disable-office-key-keyboard-shortcut-opening-office-app). I personally mapped it to my right control key instead of the capslock key; it was just a simple edit to the Autohotkey script. Both of these I placed in my windows startup folder, and then I was all set.
+
+## Additional functionality
+
+You may also add/remove keybindings one at a time, in bulk, or completely clear them all out (which also stops the hotkey listener thread).
+
+```python
+
+# Just reusing our bindings declaration from above (this is not a complete code example, btw).
+bindings = [
+    ["control + 7, control + 4", None, print_world, True],
+    ["control + 5", None, print_hello, False],
+    ["window + 1", None, print_foo, False],
+    ["t,m", None, print_bar, False],
+    ["control + Q", None, exit_application, False],
+]
+
+# Register a single keybinding (if it's not already registered). 
+# Returns True if the key didn't already exist and was added, 
+# else False (the binding is already registered - remove it first if 
+# you wish to overwrite it with new event handlers).
+register_hotkey(bindings[0])
+
+# Remove a single keybinding (if it exists). 
+# Returns True if the key existed and was removed, else False (the binding is already gone).
+remove_hotkey(bindings[0])
+
+# Register a list of keybindings.
+register_hotkeys(bindings)
+
+# Remove a list of keybindings.
+remove_hotkeys(bindings)
+
+# Remove all keybindings and terminate the hotkey listener thread.
+clear_hotkeys()
+```
+
+## List of the available keys
+
+```
+backspace
+tab
+clear
+enter
+shift
+control
+alt
+pause
+caps_lock
+escape
+space
+page_up
+page_down
+left_window
+right_window
+window
+end
+home
+left
+up
+right
+down
+select
+print
+execute
+enter
+print_screen
+insert
+delete
+help
+0
+1
+2
+3
+4
+5
+6
+7
+8
+9
+a
+b
+c
+d
+e
+f
+g
+h
+i
+j
+k
+l
+m
+n
+o
+p
+q
+r
+s
+t
+u
+v
+w
+x
+y
+z
+numpad_0
+numpad_1
+numpad_2
+numpad_3
+numpad_4
+numpad_5
+numpad_6
+numpad_7
+numpad_8
+numpad_9
+multiply_key
+add_key
+separator_key  <-- '|' also known as the 'pipe'
+|
+subtract_key
+decimal_key
+divide_key
+f1
+f2
+f3
+f4
+f5
+f6
+f7
+f8
+f9
+f10
+f11
+f12
+f13
+f14
+f15
+f16
+f17
+f18
+f19
+f20
+f21
+f22
+f23
+f24
+num_lock
+scroll_lock
+left_shift
+right_shift
+left_control
+right_control
+left_menu
+right_menu
+browser_back
+browser_forward
+browser_refresh
+browser_stop
+browser_search
+browser_favorites
+browser_start_and_home
+volume_mute
+volume_Down
+volume_up
+next_track
+previous_track
+stop_media
+play/pause_media
+start_mail
+select_media
+start_application_1
+start_application_2
+attn_key
+crsel_key
+exsel_key
+play_key
+zoom_key
+clear_key
++
+,
+-
+.
+/
+`
+;
+[
+\
+]
+'
+`
+```
```

### Comparing `global_hotkeys-0.1.6/global_hotkeys/__init__.py` & `global_hotkeys-0.1.7/global_hotkeys/__init__.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.6/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.1.7/global_hotkeys/hotkey_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 from threading import Thread, main_thread
 
 import time
 import ctypes
 from ctypes import wintypes
 import win32con
 import win32api
+import re
 
 from .keycodes import vk_key_names, vk_non_modifier_codes
 
+def detect_number_type(input_str):
+    # Regular expression patterns for hex and decimal integers
+    hex_pattern = r'^0x[0-9a-fA-F]+$'
+    decimal_pattern = r'^[0-9]+$'
+
+    # Check if the input string matches hex pattern
+    if re.match(hex_pattern, input_str):
+        return 0  # Hex number
+
+    # Check if the input string matches decimal pattern
+    elif re.match(decimal_pattern, input_str):
+        return 1  # Decimal integer
+
+    # If neither hex nor decimal, consider it as a non-number
+    else:
+        return 2  # Non-number
+
 
 def _to_virtualkey(key):
     virtual_key = None
-    if key.lower() in vk_key_names.keys():
-        virtual_key = vk_key_names[key.lower()]
+    key_lowercase = key.lower()
+    if key_lowercase in vk_key_names.keys():
+        virtual_key = vk_key_names[key_lowercase]
+    else:
+        numtype = detect_number_type(key_lowercase)
+        if(numtype == 0):
+            virtual_key = int(key_lowercase, 16)
+        elif(numtype == 1):
+            virtual_key = int(key_lowercase)
     return virtual_key
 
 full_modifier_list = [
     _to_virtualkey("control"),
     _to_virtualkey("shift"),
     _to_virtualkey("alt"),
     _to_virtualkey("left_window"),
```

### Comparing `global_hotkeys-0.1.6/global_hotkeys/keycodes.py` & `global_hotkeys-0.1.7/global_hotkeys/keycodes.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.6/global_hotkeys.egg-info/PKG-INFO` & `global_hotkeys-0.1.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: global-hotkeys
-Version: 0.1.6
+Name: global_hotkeys
+Version: 0.1.7
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -62,15 +62,16 @@
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
-    ["control + 5", None, print_hello, False],
+    # You can use direct keycodes as well (useful for non-US keyboard layouts):
+    ["control + 0x35", None, print_hello, False], # 0x35 is the keycode for the '5' key
     ["control + 6", None, print_with_params, False, {"test":5}],
     [
         "control + 8", 
         press_with_params, 
         release_with_params, 
         False, 
         {"press_param":"pressed!"}, 
@@ -131,14 +132,67 @@
 
 # Keep waiting until the user presses the exit_application keybinding.
 # Note that the hotkey listener will exit when the main thread does.
 while is_alive:
     time.sleep(0.1)
 ```
 
+## Explanation of the binding structure
+
+Let's go in more details on how the binding is structured, You have two options either to declare the binding explicitly like this within curly brackets:
+```
+# {
+#     "hotkey": <binding>,
+#     "on_press_callback": <press_callback>,
+#     "on_release_callback": <release_callback>,
+#     "actuate_on_partial_release": False | True,
+#     "callback_params": 1ms": <a variable or expression can go here>
+#     "release_callback_params": <a variable or expression can go here>
+# }
+```
+
+Or implicitly by the position of the parameter:
+```
+["hotkey", on_press_callback, on_release_callback, actuate_on_partial_release,press_callback_params,release_callback_params]
+```
+- **hotkey:** A string representing the key combination that triggers the callbacks, such as "control + 7, control + 4".
+- **on_press_callback:** The function to be called when the hotkey is pressed. Can be None or a function reference.
+- **on_release_callback:** The function to be called when the hotkey is released. Can be None or a function reference.
+- **actuate_on_partial_release:** A boolean indicating whether the release callback should be triggered on a partial release of the key combination.
+- **callback_params:** Parameters to be passed to both the press and release callbacks. This should be a dictionary.
+- **press_callback_params, release_callback_params:** Parameters specifically for the press,release callbacks. This should be a dictionary (key-value pairs Like in this example ```"press_callback_params": {"press_param":"ctrl+9 pressed!"}```) .
+
+## If you are on a non-US keyboard layout...
+You may need to manually figure out the keycodes for the keys you want to bind to, and use those keycodes directly instead of the keynames in your bindings. I've included a useful utility for doing so. 
+
+Just open an interactive shell, and import my keycode_checker module to begin figuring out what your desired keys' keycodes are.
+```python
+>>> from global_hotkeys import keycode_checker
+```
+You'll see the `Press any key (Ctrl+C to exit)` prompt and can begin pressing keys until you've gathered your desired keycodes:
+```
+Key pressed: a
+VK Code: 0x1E
+Key pressed: b
+VK Code: 0x30
+```
+
+And in your code that's actually setting up keybindings maybe you'd use something like:
+```python
+# Assume our previous example setup code from above
+bindings = [
+    ["control + 0x1E", None, print_hello, False],
+    # whatever other bindings...
+]
+```
+
+That said, if your modifier keys' keycodes (e.g. for control, shift, alt) are different than what's listed in [keycodes.py](https://github.com/btsdev/global_hotkeys/blob/master/global_hotkeys/keycodes.py), you'll likely need to just fork this project and modify the source to make things work. CD into your forked copy of the repos and use `pip install -e ./` to apply your changes as you experiment and use your forked version of the library instead. Certainly not a perfect solution, admittedly...
+
+As the code needs to differentiate between modifier keys and non-modifier keys, some further update may be necessary to allow for changing/specifying modifier keycodes as well for non-US keyboard layouts.
+
 ## Also note that I've included a simple global snippets example using this functionality.
 It's in the `tests` folder if you download this project's source from [GitHub](https://github.com/btsdev/global_hotkeys).
 
 It's the file `global_snippets.py` and it demonstrates toggling on and off global snippets using a hotkey, and using key chords to inject snippets, in this case the current date time. This is a nod to a user who emailed regarding the addition of this functionality.
 
 It achieves this by pasting in the current date time to any input field after backspacing to erase the snippet's chord from the input field (careful where you use it though. For faster input of snippets, I relied on just placing the date string into the clipboard and emulating CTRL+V to paste).
 
@@ -334,17 +388,22 @@
 [
 \
 ]
 '
 `
 ```
 
+
 Change Log
 ==========
 
+0.1.7 (4/23/2024)
+-----------------
+- Support added for specifying keycodes directly inside of keybindings.
+
 0.1.6 (6/21/2023)
 -----------------
 - Changelog updated.
 
 0.1.5 (6/21/2023)
 -----------------
 - Minor fix to the register_hotkey function.
```

### Comparing `global_hotkeys-0.1.6/setup.py` & `global_hotkeys-0.1.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,23 +6,23 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='global_hotkeys',
-  version='0.1.6',
+  version='0.1.7',
   description='',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/btsdev',
   author='btsdev',
   author_email='btsdevman@gmail.com',
   license='MIT',
   classifiers=classifiers,
   keywords='hotkeys,shortcuts',
   packages=find_packages(),
-  install_requires=["pywin32"], # "some_lib ~= 1.0"
+  install_requires=["pywin32", "keyboard"], # "some_lib ~= 1.0"
   extras_require = {
     "dev": [] # "pytest>=3.7"
   }
 )
```

### Comparing `global_hotkeys-0.1.6/tests/global_snippets.py` & `global_hotkeys-0.1.7/tests/global_snippets.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.6/tests/test.py` & `global_hotkeys-0.1.7/tests/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     stop_checking_hotkeys()
     is_alive = False
 
 
 # Declare some key bindings.
 bindings = [
     ["control + 7, control + 4", None, print_world, True],
-    ["control + 5", None, print_hello, False],
+    ["control + 0x35", None, print_hello, False], # 0x35 is the keycode for the '5' key
     ["control + 6", None, print_with_params, False, {"test":5}],
     ["control + 8", press_with_params, release_with_params, False, {"press_param":"pressed!"}, {"release_param": "released!"}],
     # dict style
     {
         "hotkey": "control + 4",
         "on_press_callback": None,
         "on_release_callback": print_with_params,
```

