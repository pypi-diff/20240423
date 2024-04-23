# Comparing `tmp/keyhint-0.4.4.tar.gz` & `tmp/keyhint-0.5.0.tar.gz`

## Comparing `keyhint-0.4.4.tar` & `keyhint-0.5.0.tar`

### file list

```diff
@@ -1,36 +1,44 @@
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 keyhint-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 keyhint-0.4.4/CHANGELOG.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 keyhint-0.4.4/.github/workflows/coverage.yml
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 keyhint-0.4.4/.github/workflows/python.yml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/__main__.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/app.py
--rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/utils.py
--rw-r--r--   0        0        0    18727 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/window.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/cli.toml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/firefox.toml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/foot.toml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/github.toml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/gnome-terminal.toml
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/kitty.toml
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/pop-shell.toml
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/tilix.toml
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/tmux.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/tridactyl.toml
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/vim.toml
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/config/vscode.toml
--rw-r--r--   0        0        0   700668 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/keyhint.png
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/keyhint_128.png
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/keyhint_32.png
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/keyhint_48.png
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/keyhint_64.png
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/keyhint_icon.svg
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/style.css
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 keyhint-0.4.4/keyhint/resources/window.ui
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 keyhint-0.4.4/tests/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 keyhint-0.4.4/tests/test_utils.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 keyhint-0.4.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 keyhint-0.4.4/LICENSE
--rw-r--r--   0        0        0     5510 2020-02-02 00:00:00.000000 keyhint-0.4.4/README.md
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 keyhint-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 keyhint-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 keyhint-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 keyhint-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 keyhint-0.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 keyhint-0.5.0/.github/workflows/python.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/__main__.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/app.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/binding.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config.py
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/context.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/css.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/headerbar.py
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/sheets.py
+-rw-r--r--   0        0        0    32732 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/window.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/cli.toml
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/firefox.toml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/foot.toml
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/forge.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/github.toml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/gnome-terminal.toml
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/keyhint.toml
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/kitty.toml
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/pop-shell.toml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/tilix.toml
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/tmux.toml
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/tridactyl.toml
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/vim.toml
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/config/vscode.toml
+-rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/headerbar.ui
+-rw-r--r--   0        0        0   700668 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/keyhint.png
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/keyhint_128.png
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/keyhint_32.png
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/keyhint_48.png
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/keyhint_64.png
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/keyhint_icon.svg
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/style.css
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 keyhint-0.5.0/keyhint/resources/window.ui
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 keyhint-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 keyhint-0.5.0/tests/test_sheets.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 keyhint-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 keyhint-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 keyhint-0.5.0/README.md
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 keyhint-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 keyhint-0.5.0/PKG-INFO
```

### Comparing `keyhint-0.4.4/.pre-commit-config.yaml` & `keyhint-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/CHANGELOG.md` & `keyhint-0.5.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # Changelog
 
-## v0.4.4 (2024-02-14)
+## v0.5.0
 
+- Breaking changes:
+  - Renamed the attribute `regex_process` in `toml`-files to `regex_wmclass`.
+  - Renamed the attribute `source` in `toml`-files to `url`.
+  - Removed cli-args which are now covered by settings menu.
 - Fix duplicate IDs in included sections.
-- Fix error if launched with `--no-section-sort`
+- Add settings menu to ui.
+- Add Support KDE + Wayland.
 - Focus search field on start.
-- Move generic CLI commands into separate cheatsheet and include it in terminal apps.
+- Cheatsheets:
+  - Moved some CLI commands into separate cheatsheet and include it in terminal apps.
+  - Added sheet for Keyhint itself.
 
 ## v0.4.3 (2024-02-13)
 
 - Fix background color in GTK 4.6.
 
 ## v0.4.2 (2024-02-13)
```

### Comparing `keyhint-0.4.4/.github/workflows/coverage.yml` & `keyhint-0.5.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/.github/workflows/python.yml` & `keyhint-0.5.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/keyhint/app.py` & `keyhint-0.5.0/keyhint/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,114 +1,82 @@
 """Cheatsheet for keyboard shortcuts & commands.
 
 Main entry point that get's executed on start.
 """
 
 import logging
 import sys
-from collections.abc import Mapping
-from typing import Any
 
 import gi
 
 gi.require_version("Gtk", "4.0")
 gi.require_version("Adw", "1")
 
-from gi.repository import Adw, Gio, GLib, Gtk  # noqa: E402
+from gi.repository import Adw, Gio, GLib  # noqa: E402
 
 from keyhint.window import KeyhintWindow  # noqa: E402
 
 logging.basicConfig(
-    format="%(asctime)s - %(levelname)s - %(name)s - %(message)s",
+    format="%(asctime)s - %(levelname)-7s - %(module)s.py:%(lineno)d - %(message)s",
     datefmt="%H:%M:%S",
     level="WARNING",
 )
-logger = logging.getLogger(__name__)
+logger = logging.getLogger("keyhint")
 
 
 class Application(Adw.Application):
     """Main application class.
 
     Handle command line options and display the window.
 
     Args:
         Gtk (Gtk.Application): Application Class
     """
 
     def __init__(self, *args, **kwargs) -> None:  # noqa: ANN002, ANN003
         """Initialize application with command line options."""
+        kwargs.update(
+            application_id="com.github.dynobo.keyhint",
+            flags=Gio.ApplicationFlags.HANDLES_COMMAND_LINE,
+        )
         super().__init__(
             *args,
-            application_id="eu.dynobo.keyhint",
-            flags=Gio.ApplicationFlags.HANDLES_COMMAND_LINE,
             **kwargs,
         )
         self.options: dict = {}
 
         self.add_main_option(
             "cheatsheet",
             ord("c"),
             GLib.OptionFlags.NONE,
             GLib.OptionArg.STRING,
             "Show cheatsheet with this ID on startup",
             "SHEET-ID",
         )
         self.add_main_option(
-            "default-cheatsheet",
-            ord("d"),
-            GLib.OptionFlags.NONE,
-            GLib.OptionArg.STRING,
-            "Cheatsheet to show in case no cheatsheet is found for active application",
-            "SHEET-ID",
-        )
-        self.add_main_option(
-            "no-fullscreen",
-            ord("f"),
-            GLib.OptionFlags.NONE,
-            GLib.OptionArg.NONE,
-            "Launch window in normal window state instead of fullscreen mode",
-            None,
-        )
-        self.add_main_option(
-            "no-section-sort",
-            ord("s"),
-            GLib.OptionFlags.NONE,
-            GLib.OptionArg.NONE,
-            "Do not sort sections by size, keep order from config toml file",
-            None,
-        )
-        self.add_main_option(
-            "orientation",
-            ord("o"),
-            GLib.OptionFlags.NONE,
-            GLib.OptionArg.STRING,
-            "Orientation and scroll direction. Default: 'vertical'",
-            "horizontal|vertical",
-        )
-        self.add_main_option(
             "verbose",
             ord("v"),
             GLib.OptionFlags.NONE,
             GLib.OptionArg.NONE,
             "Verbose log output for debugging",
             None,
         )
 
     def do_activate(self, *_, **__) -> None:  # noqa: ANN002, ANN003
         """Create and activate a window."""
         window = KeyhintWindow(self.options)
         window.set_application(self)
         window.present()
 
-    def do_command_line(self, cli: Gtk, **__: Mapping[Any, Any]) -> int:
+    def do_command_line(self, cli: Gio.ApplicationCommandLine) -> int:
         """Store command line options in class attribute for later usage."""
         self.options = cli.get_options_dict().end().unpack()
 
         if "verbose" in self.options:
-            logging.getLogger().setLevel("DEBUG")
+            logger.setLevel("DEBUG")
             logger.debug("CLI Options: %s", self.options)
 
         self.activate()
         return 0
 
 
 def main() -> None:
```

### Comparing `keyhint-0.4.4/keyhint/config/cli.toml` & `keyhint-0.5.0/keyhint/config/cli.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 id = "cli"
-source = ""
+url = ""
 
 [match]
-regex_process = "a^"
+regex_wmclass = "a^"
 regex_title = "a^"
 
 [section]
 
 [section."Shell History"]
 "Ctrl + r" = "Reverse cmd search / find next"
 "`history | grep <term>`" = "Search for \"<term>\""
@@ -32,12 +32,17 @@
 hyperfine = "Benchmarking"
 tl = "TooLong log file viewer"
 bat = "cat clone to view files with style"
 eza = "ls clone with coloring"
 duf = "Basic disk usage"
 ncdu = "Recursive disk usage analyzer"
 s-tui = "Stress test and monitor"
+btm = "System resources dashboard"
 
 [section.Navigating]
 pwd = "Print working dir"
 cd = "Change to home dir"
 "`cd -`" = "Change to previous dir"
+
+[section.Debuggin]
+"journalctl --since \"1m ago\"" = "System logs since time"
+"journalctl -k" = "System logs since boot"
```

### Comparing `keyhint-0.4.4/keyhint/config/firefox.toml` & `keyhint-0.5.0/keyhint/config/firefox.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 id = "firefox"
-source = "https://support.mozilla.org/en-US/kb/keyboard-shortcuts-perform-firefox-tasks-quickly"
+url = "https://support.mozilla.org/en-US/kb/keyboard-shortcuts-perform-firefox-tasks-quickly"
 
 [match]
-regex_process = "Firefox"
+regex_wmclass = "Firefox"
 regex_title = ".*"
 
 [section]
 [section."URL Navigation"]
 "Ctrl + L" = "Location bar"
 "Alt + Left" = "Back in History"
 "Alt + Right" = "Forward in History"
```

### Comparing `keyhint-0.4.4/keyhint/config/github.toml` & `keyhint-0.5.0/keyhint/config/github.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 id = "github.com"
-source = "https://help.github.com/en/github/getting-started-with-github/keyboard-shortcuts"
+url = "https://help.github.com/en/github/getting-started-with-github/keyboard-shortcuts"
 hidden = true
 
 [match]
-regex_process = ".*"
+regex_wmclass = ".*"
 regex_title = ".*github\\.com.*"
 
 [section]
-[section."Side Wide"]
+[section."Site Wide"]
 "S / \\/" = "Focus search bar"
 gn = "Goto notifications"
 esc = "Close hovercard, if open"
 
 [section.Repositories]
 gc = "Goto code tab"
 gi = "Goto issues tab"
```

### Comparing `keyhint-0.4.4/keyhint/config/kitty.toml` & `keyhint-0.5.0/keyhint/config/kitty.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 id = "kitty"
-source = "https://sw.kovidgoyal.net/kitty/overview/"
+url = "https://sw.kovidgoyal.net/kitty/overview/"
 include = ["cli"]
 
 [match]
-regex_process = "kitty"
+regex_wmclass = "kitty"
 regex_title = ".*"
 
 [section]
 [section.Scrolling]
 "Ctrl + Shift + UpDown" = "Line up/down"
 "Ctrl + Shift + PageUpDown" = "Page up/down"
 "Ctrl + Shift + Home" = "Top"
```

### Comparing `keyhint-0.4.4/keyhint/config/pop-shell.toml` & `keyhint-0.5.0/keyhint/config/pop-shell.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 id = "pop-shell"
-source = "https://support.system76.com/articles/pop-keyboard-shortcuts/"
+url = "https://support.system76.com/articles/pop-keyboard-shortcuts/"
 
 [match]
-regex_process = "pop-shell"
+regex_wmclass = "pop-shell"
 regex_title = ".*"
 
 [section]
 [section."Manipulate windows"]
 "Super + Direction" = "Move focus"
 "Super + O" = "Switch tiling orientation"
 "Super + M" = "Toggle maximized"
```

### Comparing `keyhint-0.4.4/keyhint/config/tilix.toml` & `keyhint-0.5.0/keyhint/config/tilix.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 id = "tilix"
-source = "https://github.com/gnunn1/tilix/blob/master/data/resources/ui/shortcuts.ui"
+url = "https://github.com/gnunn1/tilix/blob/master/data/resources/ui/shortcuts.ui"
 include = ["cli"]
 
 [match]
-regex_process = "tilix"
+regex_wmclass = "tilix"
 regex_title = ".*"
 
 [section]
 [section.Window]
 F11 = "Toggle fullscreen"
 F12 = "View session sidebar"
```

### Comparing `keyhint-0.4.4/keyhint/config/tmux.toml` & `keyhint-0.5.0/keyhint/config/tmux.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 id = "tmux"
-source = "https://github.com/gnunn1/tilix/blob/master/data/resources/ui/shortcuts.ui"
+url = "https://github.com/gnunn1/tilix/blob/master/data/resources/ui/shortcuts.ui"
 include = ["cli"]
 
 [match]
-regex_process = "foot"
+regex_wmclass = "foot"
 regex_title = "tmux"
 
 [section]
 [section.General]
 "Ctrl + a" = "Prefix key for all shortcuts!"
 "?" = "Show shortcuts"
```

### Comparing `keyhint-0.4.4/keyhint/config/tridactyl.toml` & `keyhint-0.5.0/keyhint/config/tridactyl.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 id = "tridactyl"
-source = "https://github.com/tridactyl/tridactyl"
+url = "https://github.com/tridactyl/tridactyl"
 hidden = true
 
 [match]
-regex_process = "$^"
+regex_wmclass = "$^"
 regex_title = "$^"
 
 [section]
 [section.Modes]
 Esc = "Normal"
 f = "Hint"
 v = "Visual"
```

### Comparing `keyhint-0.4.4/keyhint/config/vim.toml` & `keyhint-0.5.0/keyhint/config/vim.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,83 @@
 id = "vim"
-source = ""
+url = ""
 
 [match]
-regex_process = "(foot|kitty|gnome-terminal)"
+regex_wmclass = "(foot|kitty|gnome-terminal)"
 regex_title = "^(n)?vim( .*)?$"
 
 [section]
-[section.Navigating]
-"f / F + {c}" = "Jump to next / previous char"
-"t / T + {c}" = "Move until next / previous char"
-"; / ," = "Go to next / previous occurance"
-"{ / }" = "Paragraph down / up"
-"Ctrl + D / U\"" = "Half page down / up"
-"gg / G" = "Jump to top/bottom of file"
-gd = "Jump to definition"
-gf = "Jump to file in import"
+
+[section."Verbs (Operators)"]
+"y / Y" = "Yank (copy) / until end"
+"p / ]p" = "Paste / and adjust indent"
+"d / D" = "Delete / until end"
+"c / C" = "Change / until end"
+"v / V" = "Visually select / whole line"
+"> / <" = "Add / remove indentation"
+
+[section.Modifiers]
+i = "Inner"
+a = "Around"
+"{int}" = "x times"
+"t / T + {c}" = "Toward next / previous char"
+"f / F + {c}" = "Find next / previous char"
+"/" = "Search"
+
+[section."Nouns (Motions)"]
+"Ctrl + d / u" = "Half page down / up"
+"H / M / L" = "Top / middle / bottom of screen"
+"0 / ^ / $" = "Line start / first non-blank / end"
+"* / #" = "Next / previous token under cursor"
+"b / B" = "Beginning of word / token"
+"w / W" = "Next word / token"
+"e / E" = "End of word / token"
+"} / {" = "Next paragraph / previous paragraph"
 "%" = "Jump to matching bracket"
+"{mod} + p" = "Paragraph"
+"{mod} + s" = "Sentence"
+"{mod} + b" = "Block"
+"{mod} + t" = "XML Tag"
+"{mod} + \"" = "Quoted string"
+"{mod} + ( / )" = "Paired brackets"
 
 [section.Search]
 "\\/ / ?" = "Search forward / backwards"
-"n / N" = "Jump to next / previous match"
+"n / N" = "Next / previous occurance"
 "* / #" = "Search next / previous word under cursor"
 
+[section.Navigating]
+gd = "Go to definition"
+gf = "Go to file in import"
+"gg / G" = "Go to top/bottom of file"
+5G = "Go to line 5"
+"+" = "Go to first char of next line"
+"ma / `a" = "Mark a / jump to a"
+
 [section.Editing]
-d = "Delete / whole line"
-c = "Change (delete + insert)"
-y = "Yank / whole line"
-p = "Paste"
-"Shift + i" = "Insert at beginning of line"
+"i / I" = "Insert before cursor / line"
+"a / A" = "Append after cursor / line"
+"o / O" = "Open new line below / above"
+"r / R" = "Replace char / and insert"
+"s / S" = "Substitute char / line"
+J = "Join lines"
+"x / X" = "Exterminate char under / before cursor"
+"u / Ctrl + r" = "Undo / redo"
+
+[section."Useful commands"]
 d5j = "Delete 5 lines downwards"
 "df\"" = "Delete in line until \""
 "dt\"" = "Delete in line until before \""
-"d/foo" = "Delete from cursor util foo"
-"> / <" = "Add / remove indentation"
-"=" = "Format code"
-"Ctrl + v & Up / Down" = "Visual block mode"
-"Shift + i & # & Esc" = "Comment selected visual block"
+ea = "Append to end of word"
+"d/foo" = "Delete from cursor until foo"
+ciw = "Change inner word"
+"gu / gU" = "Lowercase / uppercase"
+"Ctrl + v & j / k" = "Visual block select"
+"I & # & Esc" = "Comment selected visual block"
+"\"ayi\"" = "Yank inner \" to register a"
+"vi\"\"ap" = "Replace inner \" from register a"
 
 [section.Registers]
+"`\"ay`" = "yank to regesiter a"
+"`\"ap`" = "paste from register a"
 "`\"+y`" = "yank to system clipboard"
 "`\"+p`" = "paste from system clipboard"
-
-[section.Syntax]
-cc = "Double modify whole line"
-D = "Capitalize for stronger/alt"
-"{op} + a / i + {obj}" = "around / inner"
-ciw = "Change inner word"
-daw = "Delete a word"
-
-[section."surround.vim"]
-"ysiw)" = "Surround word under cursor with bracket"
-"yss)" = "Surround whole line with bracket"
-"cs)]" = "Change nearest brackets to squared brackets"
-"ds)" = "Delete surrounding brackets"
```

### Comparing `keyhint-0.4.4/keyhint/config/vscode.toml` & `keyhint-0.5.0/keyhint/config/vscode.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 id = "vscode"
-source = "https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf"
+url = "https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf"
 
 [match]
-regex_process = "code"
+regex_wmclass = "code"
 regex_title = ".*"
 
 [section]
 [section."Navigating UI"]
 "Ctrl + 0" = "Focus sidebar"
 "Ctrl + 1" = "Focus editor 1"
 "Ctrl + 2" = "Focus editor 2"
@@ -19,14 +19,17 @@
 
 [section.Panel]
 "Ctrl + J" = "Toggle panel"
 "Ctrl + `" = "Toggle terminal"
 "Ctrl + Shift + M" = "Toggle problems"
 "Ctrl + Shift + Y" = "Toggle debug console"
 
+[section.View]
+"Ctrl + K + Z" = "Zen mode"
+
 [section."Basic Editing"]
 "Ctrl + L" = "Select current line"
 "Ctrl + Backspace" = "Delete last word"
 "Alt + Up Down" = "Move line up/down"
 "Alt + Shift + Up Down" = "Duplicate cursor"
 "Ctrl+ Alt + Shift + Up Down" = "Duplicate line"
 "Shift + Alt + Left Right" = "Expand/shrink selection"
@@ -59,7 +62,16 @@
 F11 = "Step into"
 "Shift + F11" = "Step out"
 F10 = "Step over"
 
 [section."File/Tab Management"]
 "Ctrl + Tab" = "Switch between tabs"
 "Ctrl + P" = "Quick open file"
+
+[section."Extension = NeoVim"]
+"ma / mA" = "Multicursor after cursor / line"
+"mi / mI" = "Multicursor before cursor / line"
+"K" = "Show hover, repeat to focus hover"
+"gd" = "Goto definition"
+"gf" = "Goto declaration"
+"gH" = "Reference Search"
+"Ctrl + n / p" = "Next / previous list item"
```

### Comparing `keyhint-0.4.4/keyhint/resources/keyhint.png` & `keyhint-0.5.0/keyhint/resources/keyhint.png`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/keyhint/resources/keyhint_128.png` & `keyhint-0.5.0/keyhint/resources/keyhint_128.png`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/keyhint/resources/keyhint_32.png` & `keyhint-0.5.0/keyhint/resources/keyhint_32.png`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/keyhint/resources/keyhint_48.png` & `keyhint-0.5.0/keyhint/resources/keyhint_48.png`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/keyhint/resources/keyhint_64.png` & `keyhint-0.5.0/keyhint/resources/keyhint_64.png`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/keyhint/resources/keyhint_icon.svg` & `keyhint-0.5.0/keyhint/resources/keyhint_icon.svg`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/keyhint/resources/style.css` & `keyhint-0.5.0/keyhint/resources/style.css`

 * *Files 24% similar despite different names*

```diff
@@ -6,25 +6,38 @@
 .keycap {
   min-width: 15px;
   min-height: 25px;
   margin-top: 2px;
   padding-bottom: 3px;
   padding-left: 6px;
   padding-right: 6px;
-
   background-color: @bg_color;
   border: 1px solid;
   border-radius: 5px;
   border-color: @borders_color;
   box-shadow: inset 0 -3px @shadow_color;
 }
 
 .bindings-section header label {
   color: @accent_color;
   margin-top: 26px;
   filter: unset;
 }
 
+.popover_menu_box > list > row {
+  border-radius: 10px;
+}
+
+.popover_menu_box .setting_label {
+  font-size: 85%;
+  opacity: 0.8;
+}
+
+.popover_menu_box .menu_entry {
+  font-weight: normal;
+}
+
+.transparent,
 .bindings-section,
 .bindings-section .view {
   background-color: transparent;
 }
```

### Comparing `keyhint-0.4.4/.gitignore` & `keyhint-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/LICENSE` & `keyhint-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `keyhint-0.4.4/README.md` & `keyhint-0.5.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,131 +1,181 @@
 # KeyHint
 
 **_Utility to display keyboard shortcuts or other hints based on the active window on
-Linux. (GTK 4.6+ required!)_**
+Linux._**
 
 <p align="center"><br>
 <img alt="Tests passing" src="https://github.com/dynobo/keyhint/workflows/Test/badge.svg">
 <a href="https://github.com/dynobo/keyhint/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/Code%20style-black-%23000000"></a>
 <a href='https://coveralls.io/github/dynobo/keyhint'><img src='https://coveralls.io/repos/github/dynobo/keyhint/badge.svg' alt='Coverage Status' /></a>
 </p>
 
 ![Keyhint Screenshot](https://raw.githubusercontent.com/dynobo/keyhint/main/keyhint/resources/keyhint.png)
 
 ## Prerequisites
 
 - Python 3.11+
-- GTK 4.6+ (shipped since Ubuntu 22.04) + dev packages:
+- GTK 4.6+ (shipped since Ubuntu 22.04) + related dev packages:
   ```sh
   sudo apt-get install \
      libgirepository1.0-dev \
      libcairo2-dev \
      python3-gi \
      gobject-introspection \
      libgtk-4-dev
   ```
+- Wayland & Gnome: The
+  [Gnome Extension "Window-Calls"](https://extensions.gnome.org/extension/4724/window-calls/)
+  is required to auto-select the cheatsheet based on the current active application.
 
 ## Installation
 
 - `pipx install keyhint` (recommended, requires [pipx](https://pipx.pypa.io/))
 - _or_ `pip install keyhint`
 
 ## Usage
 
 - Configure a **global hotkey** (e.g. `Ctrl + F1`) **via your system settings** to
   launch `keyhint`.
 - If KeyHint is launched via hotkey, it detects the current active application and shows
-  the appropriate hints.
+  the appropriate hints. (This feature won't work reliably when KeyHint ist started via
+  Menu or Launcher.)
 
 ## CLI Options
 
 ```
 Application Options:
   -c, --cheatsheet=SHEET-ID                 Show cheatsheet with this ID on startup
-  -d, --default-cheatsheet=SHEET-ID         Cheatsheet to show in case no cheatsheet is found for active application
-  -f, --no-fullscreen                       Launch window in normal window state instead of fullscreen mode
-  -s, --no-section-sort                     Do not sort sections by size, keep order from config toml file
-  -o, --orientation=horizontal|vertical     Orientation and scroll direction. Default: 'vertical'
   -v, --verbose                             Verbose log output for debugging
 ```
 
-## Configuration
+## Cheatsheet Configuration
 
-- The **config directory** is `~/.config/keyhint/`.
-- To **customize existing** cheatsheets, copy
+The content which KeyHint displays is configured using [`toml`](https://toml.io/en/)
+configuration files.
+
+KeyHint reads those files from two locations:
+
+1. The [built-in directory](https://github.com/dynobo/keyhint/tree/main/keyhint/config)
+1. The user directory, usually located in `~/.config/keyhint`
+
+### How Keyhint selects the cheatsheet to show
+
+- The cheatsheet to be displayed on startup are selected by comparing the value of
+  `regex_wmclass` with the wm_class of the active window and the value of `regex_title`
+  with the title of the active window.
+- The potential cheatsheets are processed alphabetically by filename, the first file
+  that matches both wm_class and title are getting displayed.
+- Both of `regex_` values are interpreted as **case in-sensitive regular expressions**.
+- Check "Debug Info" in the application menu to get insights about the active window and
+  the selected cheatsheet file.
+
+### Customize or add cheatsheets
+
+- To **change built-in** cheatsheets, copy
   [the corresponding .toml-file](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config)
   into the config directory. Make your changes in a text editor. As long as you don't
   change the `id` it will overwrite the defaults.
-- To **create new** cheatsheets, I suggest you also start with
+- To **create new** cheatsheets, I suggest you start with
   [one of the existing .toml-file](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config):
   - Place it in the config directory and give it a good file name.
   - Change the value `id` to something unique.
-  - Adjust `regex_process` and `regex_title` so it will be selected based on the active
+  - Adjust `regex_wmclass` and `regex_title` so it will be selected based on the active
     window. (See [Tips](#tips))
   - Add the `shortcuts` & `label` to a `section`.
   - If you think your cheatsheet might be useful for others, please consider opening a
-    pull request or an issue.
-- You can always **reset a configuration** to the shipped version by deleting the
-  `.toml` files from the config folder.
-- You can **include shortcuts from other cheatsheets** add
+    pull request or an issue!
+- You can always **reset cheatsheets** to the shipped version by deleting the
+  corresponding `.toml` files from the config folder.
+- You can **include shortcuts from other cheatsheets** by adding
   `include = ["<Cheatsheet ID>"]`
-- You can **hide a cheatsheet** by add `hidden = true` in the top block (same level as
-  `id` and `title`).
 
-## Tips
+### Examples
 
-**Cheatsheet selection:**
+#### Hide existing cheatsheets
 
-- The cheatsheet to be displayed on startup are selected by comparing the value of
-  `regex_process` with the wm_class of the active window and the value of `regex_title`
-  with the title of the active window.
-- The potential cheatsheets are processed alphabetically by filename, the first file
-  that matches both wm_class and title are getting displayed.
-- Both of `regex_` values are interpreted as **case in-sensitive regular expressions**.
-- Check "Debug Info" in the application menu to get insights about the active window and
-  the selected cheatsheet file.
+To hide a cheatsheet, e.g. the
+[built-in](https://github.com/dynobo/keyhint/blob/main/keyhint/config/tilix.toml) one
+with the ID `tilix`, create a new file `~/.config/keyhint/tilix.toml` with the content:
+
+```toml
+id = "tilix"
+hidden = true
+```
 
-**Available cheatsheets:**
+#### Extend existing cheatsheets
 
-- Check the
-  [included toml-files](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config)
-  to see which applications are available by default.
-- Feel free submit additional `toml-files` for further applications.
-
-**Differentiate cheatsheets per website:**
-
-- For showing different browser-cheatsheets depending on the current website, you might
-  want to use a browser extension like
-  "[Add URL To Window Title](https://addons.mozilla.org/en-US/firefox/addon/add-url-to-window-title/)"
-  and then configure the sections in `<cheatsheet>.toml` to look for the URL in the
-  window title.
-
-**KeyHint's shortcuts:**
-
-- `Ctrl+F`: Start filtering
-- `Ctrl+S`: Focus sheet selection dropdown (press `Enter` to open it)
-- `Esc`: Exit KeyHint
-- `→`, `↓`, `l` or `k`: scroll forward
-- `←`, `↑`, `h` or `j`: scroll backward
-- `PageDown`: scroll page forward
-- `PageUP`: scroll page backward
+To add keybindings to an existing cheatsheet, e.g. the
+[built-in](https://github.com/dynobo/keyhint/blob/main/keyhint/config/firefox.toml) one
+with the ID `firefox`, create a new file `~/.config/keyhint/firefox.toml` which only
+contains the ID and the additional bindings:
+
+```toml
+id = "firefox"
+
+[section]
+[section."My Personal Favorites"]  # New section
+"Ctrl + Shift + Tab" = "Show all Tabs"
+# ...
+```
+
+#### Add new cheatsheet which never gets auto-selected
+
+To add a new cheatsheet, which never gets automatically selected and displayed by
+KeyHint, but remains accessible through KeyHint's cheatsheet dropdown, create a file
+`~/.config/keyhint/my-app.toml`:
+
+```toml
+id = "my-app"
+url = "url-to-my-apps-keybindings"
+
+[match]
+regex_wmclass = "a^"  # Patter which never matches
+regex_title = "a^"
+
+[section]
+[section.General]
+"Ctrl + C" = "Copy"
+# ...
+
+```
+
+#### Different cheatsheets for different Websites
+
+For showing different browser-cheatsheets depending on the current website, you might
+want to use a browser extension like
+"[Add URL To Window Title](https://addons.mozilla.org/en-US/firefox/addon/add-url-to-window-title/)"
+and configure the `[match]` section to look for the url in the title. E.g.
+`~/.config/keyhint/github.toml`
+
+```toml
+id = "github.com"
+
+[match]
+regex_wmclass = "Firefox"
+regex_title = ".*github\\.com.*"  # URL added by browser extensions to window title
+
+[section]
+[section.Repositories]
+gc = "Goto code tab"
+# ...
+```
 
 ## Contribute
 
 I'm happy about any contribution! Especially I would appreciate submissions to improve
 the
 [shipped cheatsheets](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config).
 (The current set are the cheatsheets I personally use).
 
 ## Design Principles
 
 - **Don't run as service**<br>It shouldn't consume resources in the background, even if
-  this leads to slower start-up time.
+  this leads to slightly slower start-up time.
 - **No network connection**<br>Everything should run locally without any network
   communication.
 - **Dependencies**<br>The fewer dependencies, the better.
-- **Multi-Monitors**<br>Supports setups with two or more displays
 
 ## Certification
 
 ![WOMM](https://raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,66 +1,78 @@
 # KeyHint **_Utility to display keyboard shortcuts or other hints based on the
-active window on Linux. (GTK 4.6+ required!)_**
+active window on Linux._**
 
        [Tests passing]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]
 ![Keyhint Screenshot](https://raw.githubusercontent.com/dynobo/keyhint/main/
 keyhint/resources/keyhint.png) ## Prerequisites - Python 3.11+ - GTK 4.6+
-(shipped since Ubuntu 22.04) + dev packages: ```sh sudo apt-get install \
-libgirepository1.0-dev \ libcairo2-dev \ python3-gi \ gobject-introspection \
-libgtk-4-dev ``` ## Installation - `pipx install keyhint` (recommended,
-requires [pipx](https://pipx.pypa.io/)) - _or_ `pip install keyhint` ## Usage -
-Configure a **global hotkey** (e.g. `Ctrl + F1`) **via your system settings**
-to launch `keyhint`. - If KeyHint is launched via hotkey, it detects the
-current active application and shows the appropriate hints. ## CLI Options ```
-Application Options: -c, --cheatsheet=SHEET-ID Show cheatsheet with this ID on
-startup -d, --default-cheatsheet=SHEET-ID Cheatsheet to show in case no
-cheatsheet is found for active application -f, --no-fullscreen Launch window in
-normal window state instead of fullscreen mode -s, --no-section-sort Do not
-sort sections by size, keep order from config toml file -o, --
-orientation=horizontal|vertical Orientation and scroll direction. Default:
-'vertical' -v, --verbose Verbose log output for debugging ``` ## Configuration
-- The **config directory** is `~/.config/keyhint/`. - To **customize existing**
-cheatsheets, copy [the corresponding .toml-file](https://github.com/dynobo/
-keyhint/tree/main/src/keyhint/config) into the config directory. Make your
-changes in a text editor. As long as you don't change the `id` it will
-overwrite the defaults. - To **create new** cheatsheets, I suggest you also
-start with [one of the existing .toml-file](https://github.com/dynobo/keyhint/
-tree/main/src/keyhint/config): - Place it in the config directory and give it a
-good file name. - Change the value `id` to something unique. - Adjust
-`regex_process` and `regex_title` so it will be selected based on the active
+(shipped since Ubuntu 22.04) + related dev packages: ```sh sudo apt-get install
+\ libgirepository1.0-dev \ libcairo2-dev \ python3-gi \ gobject-introspection \
+libgtk-4-dev ``` - Wayland & Gnome: The [Gnome Extension "Window-Calls"](https:
+//extensions.gnome.org/extension/4724/window-calls/) is required to auto-select
+the cheatsheet based on the current active application. ## Installation - `pipx
+install keyhint` (recommended, requires [pipx](https://pipx.pypa.io/)) - _or_
+`pip install keyhint` ## Usage - Configure a **global hotkey** (e.g. `Ctrl +
+F1`) **via your system settings** to launch `keyhint`. - If KeyHint is launched
+via hotkey, it detects the current active application and shows the appropriate
+hints. (This feature won't work reliably when KeyHint ist started via Menu or
+Launcher.) ## CLI Options ``` Application Options: -c, --cheatsheet=SHEET-ID
+Show cheatsheet with this ID on startup -v, --verbose Verbose log output for
+debugging ``` ## Cheatsheet Configuration The content which KeyHint displays is
+configured using [`toml`](https://toml.io/en/) configuration files. KeyHint
+reads those files from two locations: 1. The [built-in directory](https://
+github.com/dynobo/keyhint/tree/main/keyhint/config) 1. The user directory,
+usually located in `~/.config/keyhint` ### How Keyhint selects the cheatsheet
+to show - The cheatsheet to be displayed on startup are selected by comparing
+the value of `regex_wmclass` with the wm_class of the active window and the
+value of `regex_title` with the title of the active window. - The potential
+cheatsheets are processed alphabetically by filename, the first file that
+matches both wm_class and title are getting displayed. - Both of `regex_`
+values are interpreted as **case in-sensitive regular expressions**. - Check
+"Debug Info" in the application menu to get insights about the active window
+and the selected cheatsheet file. ### Customize or add cheatsheets - To
+**change built-in** cheatsheets, copy [the corresponding .toml-file](https://
+github.com/dynobo/keyhint/tree/main/src/keyhint/config) into the config
+directory. Make your changes in a text editor. As long as you don't change the
+`id` it will overwrite the defaults. - To **create new** cheatsheets, I suggest
+you start with [one of the existing .toml-file](https://github.com/dynobo/
+keyhint/tree/main/src/keyhint/config): - Place it in the config directory and
+give it a good file name. - Change the value `id` to something unique. - Adjust
+`regex_wmclass` and `regex_title` so it will be selected based on the active
 window. (See [Tips](#tips)) - Add the `shortcuts` & `label` to a `section`. -
 If you think your cheatsheet might be useful for others, please consider
-opening a pull request or an issue. - You can always **reset a configuration**
-to the shipped version by deleting the `.toml` files from the config folder. -
-You can **include shortcuts from other cheatsheets** add `include = [""]` - You
-can **hide a cheatsheet** by add `hidden = true` in the top block (same level
-as `id` and `title`). ## Tips **Cheatsheet selection:** - The cheatsheet to be
-displayed on startup are selected by comparing the value of `regex_process`
-with the wm_class of the active window and the value of `regex_title` with the
-title of the active window. - The potential cheatsheets are processed
-alphabetically by filename, the first file that matches both wm_class and title
-are getting displayed. - Both of `regex_` values are interpreted as **case in-
-sensitive regular expressions**. - Check "Debug Info" in the application menu
-to get insights about the active window and the selected cheatsheet file.
-**Available cheatsheets:** - Check the [included toml-files](https://
-github.com/dynobo/keyhint/tree/main/src/keyhint/config) to see which
-applications are available by default. - Feel free submit additional `toml-
-files` for further applications. **Differentiate cheatsheets per website:** -
-For showing different browser-cheatsheets depending on the current website, you
-might want to use a browser extension like "[Add URL To Window Title](https://
-addons.mozilla.org/en-US/firefox/addon/add-url-to-window-title/)" and then
-configure the sections in `.toml` to look for the URL in the window title.
-**KeyHint's shortcuts:** - `Ctrl+F`: Start filtering - `Ctrl+S`: Focus sheet
-selection dropdown (press `Enter` to open it) - `Esc`: Exit KeyHint - `â`,
-`â`, `l` or `k`: scroll forward - `â`, `â`, `h` or `j`: scroll backward -
-`PageDown`: scroll page forward - `PageUP`: scroll page backward ## Contribute
-I'm happy about any contribution! Especially I would appreciate submissions to
-improve the [shipped cheatsheets](https://github.com/dynobo/keyhint/tree/main/
-src/keyhint/config). (The current set are the cheatsheets I personally use). ##
-Design Principles - **Don't run as service**
-It shouldn't consume resources in the background, even if this leads to slower
-start-up time. - **No network connection**
+opening a pull request or an issue! - You can always **reset cheatsheets** to
+the shipped version by deleting the corresponding `.toml` files from the config
+folder. - You can **include shortcuts from other cheatsheets** by adding
+`include = [""]` ### Examples #### Hide existing cheatsheets To hide a
+cheatsheet, e.g. the [built-in](https://github.com/dynobo/keyhint/blob/main/
+keyhint/config/tilix.toml) one with the ID `tilix`, create a new file
+`~/.config/keyhint/tilix.toml` with the content: ```toml id = "tilix" hidden =
+true ``` #### Extend existing cheatsheets To add keybindings to an existing
+cheatsheet, e.g. the [built-in](https://github.com/dynobo/keyhint/blob/main/
+keyhint/config/firefox.toml) one with the ID `firefox`, create a new file
+`~/.config/keyhint/firefox.toml` which only contains the ID and the additional
+bindings: ```toml id = "firefox" [section] [section."My Personal Favorites"] #
+New section "Ctrl + Shift + Tab" = "Show all Tabs" # ... ``` #### Add new
+cheatsheet which never gets auto-selected To add a new cheatsheet, which never
+gets automatically selected and displayed by KeyHint, but remains accessible
+through KeyHint's cheatsheet dropdown, create a file `~/.config/keyhint/my-
+app.toml`: ```toml id = "my-app" url = "url-to-my-apps-keybindings" [match]
+regex_wmclass = "a^" # Patter which never matches regex_title = "a^" [section]
+[section.General] "Ctrl + C" = "Copy" # ... ``` #### Different cheatsheets for
+different Websites For showing different browser-cheatsheets depending on the
+current website, you might want to use a browser extension like "[Add URL To
+Window Title](https://addons.mozilla.org/en-US/firefox/addon/add-url-to-window-
+title/)" and configure the `[match]` section to look for the url in the title.
+E.g. `~/.config/keyhint/github.toml` ```toml id = "github.com" [match]
+regex_wmclass = "Firefox" regex_title = ".*github\\.com.*" # URL added by
+browser extensions to window title [section] [section.Repositories] gc = "Goto
+code tab" # ... ``` ## Contribute I'm happy about any contribution! Especially
+I would appreciate submissions to improve the [shipped cheatsheets](https://
+github.com/dynobo/keyhint/tree/main/src/keyhint/config). (The current set are
+the cheatsheets I personally use). ## Design Principles - **Don't run as
+service**
+It shouldn't consume resources in the background, even if this leads to
+slightly slower start-up time. - **No network connection**
 Everything should run locally without any network communication. -
 **Dependencies**
-The fewer dependencies, the better. - **Multi-Monitors**
-Supports setups with two or more displays ## Certification ![WOMM](https://
+The fewer dependencies, the better. ## Certification ![WOMM](https://
 raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)
```

### Comparing `keyhint-0.4.4/pyproject.toml` & `keyhint-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "keyhint"
-version = "0.4.4"
+version = "0.5.0"
 description = "Cheat-sheets for shortcuts & commands at your fingertips."
 keywords = ["shortcuts", "keybindings", "hints", "helper", "cheatsheet"]
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [{ name = "dynobo", email = "dynobo@mailbox.org" }]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -44,39 +44,42 @@
   "coveralls",
   "types-toml",
   "tbump",
   "ruff",
   "pip-audit",
   "mypy",
   "mdformat",
+  "pygobject-stubs",
 ]
 
 [tool.hatch.envs.default.scripts]
 style = [
-  "ruff {args:.}",
+  "ruff check {args:.}",
   "ruff format --check --diff {args:.}",
   "mdformat --check --end-of-line keep {args:.}",
 ]
 typing = "mypy"
 test = ["pytest {args:tests}", "coverage lcov"]
 security = "pip-audit"
 fmt = [
-  "ruff --fix {args:.}",
+  "ruff check --fix {args:.}",
   "ruff format {args:.}",
   "mdformat --end-of-line keep {args:.}",
 ]
 # Main tasks:
 check = ["style", "typing", "test", "security"]
 pre-commit = ["fmt", "check"]
 version = "tbump {args:current-version}"
 
 [tool.ruff]
 target-version = "py311"
 line-length = 88
 exclude = [".venv"]
+
+[tool.ruff.lint]
 select = [
   "F",    # Pyflakes
   "E",    # pycodestyle
   "I",    # Isort
   "D",    # pydocstyle
   "W",    # warning
   "UP",   # pyupgrad
@@ -112,25 +115,26 @@
   "D105",   # Missing docstring in magic method
   "D107",   # Missing docstring in __init__
   "ANN101", # Missing type annotation for `self` in method
   "TRY003", # Avoid specifying long messages outside the exception class
   "ISC001", # Rule conflicts with ruff's formaatter
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.lint.per-file-ignores]
 "tests/**/*" = ["PLR2004", "PLR0913", "S101", "TID252", "ANN", "D"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["keyhint"]
 
-[tool.ruff.flake8-tidy-imports]
-ban-relative-imports = "all"
 
 [tool.mypy]
 files = ["keyhint/**/*.py", "tests/**/*.py"]
 follow_imports = "skip"
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
@@ -153,15 +157,15 @@
 wrap = 88
 number = true
 end_of_line = "keep"
 
 [tool.tbump]
 
 [tool.tbump.version]
-current = "0.4.4"
+current = "0.5.0"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   ((?P<extra>.+))?
```

### Comparing `keyhint-0.4.4/PKG-INFO` & `keyhint-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: keyhint
-Version: 0.4.4
+Version: 0.5.0
 Summary: Cheat-sheets for shortcuts & commands at your fingertips.
 Project-URL: Documentation, https://github.com/dynobo/keyhint#readme
 Project-URL: Issues, https://github.com/dynobo/keyhint/issues
 Project-URL: Source, https://github.com/dynobo/keyhint
 Author-email: dynobo <dynobo@mailbox.org>
 License-File: LICENSE
 Keywords: cheatsheet,helper,hints,keybindings,shortcuts
@@ -21,135 +21,185 @@
 Requires-Python: >=3.11
 Requires-Dist: pygobject>=3.42.2
 Description-Content-Type: text/markdown
 
 # KeyHint
 
 **_Utility to display keyboard shortcuts or other hints based on the active window on
-Linux. (GTK 4.6+ required!)_**
+Linux._**
 
 <p align="center"><br>
 <img alt="Tests passing" src="https://github.com/dynobo/keyhint/workflows/Test/badge.svg">
 <a href="https://github.com/dynobo/keyhint/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/Code%20style-black-%23000000"></a>
 <a href='https://coveralls.io/github/dynobo/keyhint'><img src='https://coveralls.io/repos/github/dynobo/keyhint/badge.svg' alt='Coverage Status' /></a>
 </p>
 
 ![Keyhint Screenshot](https://raw.githubusercontent.com/dynobo/keyhint/main/keyhint/resources/keyhint.png)
 
 ## Prerequisites
 
 - Python 3.11+
-- GTK 4.6+ (shipped since Ubuntu 22.04) + dev packages:
+- GTK 4.6+ (shipped since Ubuntu 22.04) + related dev packages:
   ```sh
   sudo apt-get install \
      libgirepository1.0-dev \
      libcairo2-dev \
      python3-gi \
      gobject-introspection \
      libgtk-4-dev
   ```
+- Wayland & Gnome: The
+  [Gnome Extension "Window-Calls"](https://extensions.gnome.org/extension/4724/window-calls/)
+  is required to auto-select the cheatsheet based on the current active application.
 
 ## Installation
 
 - `pipx install keyhint` (recommended, requires [pipx](https://pipx.pypa.io/))
 - _or_ `pip install keyhint`
 
 ## Usage
 
 - Configure a **global hotkey** (e.g. `Ctrl + F1`) **via your system settings** to
   launch `keyhint`.
 - If KeyHint is launched via hotkey, it detects the current active application and shows
-  the appropriate hints.
+  the appropriate hints. (This feature won't work reliably when KeyHint ist started via
+  Menu or Launcher.)
 
 ## CLI Options
 
 ```
 Application Options:
   -c, --cheatsheet=SHEET-ID                 Show cheatsheet with this ID on startup
-  -d, --default-cheatsheet=SHEET-ID         Cheatsheet to show in case no cheatsheet is found for active application
-  -f, --no-fullscreen                       Launch window in normal window state instead of fullscreen mode
-  -s, --no-section-sort                     Do not sort sections by size, keep order from config toml file
-  -o, --orientation=horizontal|vertical     Orientation and scroll direction. Default: 'vertical'
   -v, --verbose                             Verbose log output for debugging
 ```
 
-## Configuration
+## Cheatsheet Configuration
 
-- The **config directory** is `~/.config/keyhint/`.
-- To **customize existing** cheatsheets, copy
+The content which KeyHint displays is configured using [`toml`](https://toml.io/en/)
+configuration files.
+
+KeyHint reads those files from two locations:
+
+1. The [built-in directory](https://github.com/dynobo/keyhint/tree/main/keyhint/config)
+1. The user directory, usually located in `~/.config/keyhint`
+
+### How Keyhint selects the cheatsheet to show
+
+- The cheatsheet to be displayed on startup are selected by comparing the value of
+  `regex_wmclass` with the wm_class of the active window and the value of `regex_title`
+  with the title of the active window.
+- The potential cheatsheets are processed alphabetically by filename, the first file
+  that matches both wm_class and title are getting displayed.
+- Both of `regex_` values are interpreted as **case in-sensitive regular expressions**.
+- Check "Debug Info" in the application menu to get insights about the active window and
+  the selected cheatsheet file.
+
+### Customize or add cheatsheets
+
+- To **change built-in** cheatsheets, copy
   [the corresponding .toml-file](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config)
   into the config directory. Make your changes in a text editor. As long as you don't
   change the `id` it will overwrite the defaults.
-- To **create new** cheatsheets, I suggest you also start with
+- To **create new** cheatsheets, I suggest you start with
   [one of the existing .toml-file](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config):
   - Place it in the config directory and give it a good file name.
   - Change the value `id` to something unique.
-  - Adjust `regex_process` and `regex_title` so it will be selected based on the active
+  - Adjust `regex_wmclass` and `regex_title` so it will be selected based on the active
     window. (See [Tips](#tips))
   - Add the `shortcuts` & `label` to a `section`.
   - If you think your cheatsheet might be useful for others, please consider opening a
-    pull request or an issue.
-- You can always **reset a configuration** to the shipped version by deleting the
-  `.toml` files from the config folder.
-- You can **include shortcuts from other cheatsheets** add
+    pull request or an issue!
+- You can always **reset cheatsheets** to the shipped version by deleting the
+  corresponding `.toml` files from the config folder.
+- You can **include shortcuts from other cheatsheets** by adding
   `include = ["<Cheatsheet ID>"]`
-- You can **hide a cheatsheet** by add `hidden = true` in the top block (same level as
-  `id` and `title`).
 
-## Tips
+### Examples
 
-**Cheatsheet selection:**
+#### Hide existing cheatsheets
 
-- The cheatsheet to be displayed on startup are selected by comparing the value of
-  `regex_process` with the wm_class of the active window and the value of `regex_title`
-  with the title of the active window.
-- The potential cheatsheets are processed alphabetically by filename, the first file
-  that matches both wm_class and title are getting displayed.
-- Both of `regex_` values are interpreted as **case in-sensitive regular expressions**.
-- Check "Debug Info" in the application menu to get insights about the active window and
-  the selected cheatsheet file.
+To hide a cheatsheet, e.g. the
+[built-in](https://github.com/dynobo/keyhint/blob/main/keyhint/config/tilix.toml) one
+with the ID `tilix`, create a new file `~/.config/keyhint/tilix.toml` with the content:
+
+```toml
+id = "tilix"
+hidden = true
+```
 
-**Available cheatsheets:**
+#### Extend existing cheatsheets
 
-- Check the
-  [included toml-files](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config)
-  to see which applications are available by default.
-- Feel free submit additional `toml-files` for further applications.
-
-**Differentiate cheatsheets per website:**
-
-- For showing different browser-cheatsheets depending on the current website, you might
-  want to use a browser extension like
-  "[Add URL To Window Title](https://addons.mozilla.org/en-US/firefox/addon/add-url-to-window-title/)"
-  and then configure the sections in `<cheatsheet>.toml` to look for the URL in the
-  window title.
-
-**KeyHint's shortcuts:**
-
-- `Ctrl+F`: Start filtering
-- `Ctrl+S`: Focus sheet selection dropdown (press `Enter` to open it)
-- `Esc`: Exit KeyHint
-- `→`, `↓`, `l` or `k`: scroll forward
-- `←`, `↑`, `h` or `j`: scroll backward
-- `PageDown`: scroll page forward
-- `PageUP`: scroll page backward
+To add keybindings to an existing cheatsheet, e.g. the
+[built-in](https://github.com/dynobo/keyhint/blob/main/keyhint/config/firefox.toml) one
+with the ID `firefox`, create a new file `~/.config/keyhint/firefox.toml` which only
+contains the ID and the additional bindings:
+
+```toml
+id = "firefox"
+
+[section]
+[section."My Personal Favorites"]  # New section
+"Ctrl + Shift + Tab" = "Show all Tabs"
+# ...
+```
+
+#### Add new cheatsheet which never gets auto-selected
+
+To add a new cheatsheet, which never gets automatically selected and displayed by
+KeyHint, but remains accessible through KeyHint's cheatsheet dropdown, create a file
+`~/.config/keyhint/my-app.toml`:
+
+```toml
+id = "my-app"
+url = "url-to-my-apps-keybindings"
+
+[match]
+regex_wmclass = "a^"  # Patter which never matches
+regex_title = "a^"
+
+[section]
+[section.General]
+"Ctrl + C" = "Copy"
+# ...
+
+```
+
+#### Different cheatsheets for different Websites
+
+For showing different browser-cheatsheets depending on the current website, you might
+want to use a browser extension like
+"[Add URL To Window Title](https://addons.mozilla.org/en-US/firefox/addon/add-url-to-window-title/)"
+and configure the `[match]` section to look for the url in the title. E.g.
+`~/.config/keyhint/github.toml`
+
+```toml
+id = "github.com"
+
+[match]
+regex_wmclass = "Firefox"
+regex_title = ".*github\\.com.*"  # URL added by browser extensions to window title
+
+[section]
+[section.Repositories]
+gc = "Goto code tab"
+# ...
+```
 
 ## Contribute
 
 I'm happy about any contribution! Especially I would appreciate submissions to improve
 the
 [shipped cheatsheets](https://github.com/dynobo/keyhint/tree/main/src/keyhint/config).
 (The current set are the cheatsheets I personally use).
 
 ## Design Principles
 
 - **Don't run as service**<br>It shouldn't consume resources in the background, even if
-  this leads to slower start-up time.
+  this leads to slightly slower start-up time.
 - **No network connection**<br>Everything should run locally without any network
   communication.
 - **Dependencies**<br>The fewer dependencies, the better.
-- **Multi-Monitors**<br>Supports setups with two or more displays
 
 ## Certification
 
 ![WOMM](https://raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,80 +1,92 @@
-Metadata-Version: 2.1 Name: keyhint Version: 0.4.4 Summary: Cheat-sheets for
+Metadata-Version: 2.3 Name: keyhint Version: 0.5.0 Summary: Cheat-sheets for
 shortcuts & commands at your fingertips. Project-URL: Documentation, https://
 github.com/dynobo/keyhint#readme Project-URL: Issues, https://github.com/
 dynobo/keyhint/issues Project-URL: Source, https://github.com/dynobo/keyhint
 Author-email: dynobo
 mailbox.org> License-File: LICENSE Keywords:
 cheatsheet,helper,hints,keybindings,shortcuts Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: End Users/Desktop Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Classifier: Topic ::
 Utilities Requires-Python: >=3.11 Requires-Dist: pygobject>=3.42.2 Description-
 Content-Type: text/markdown # KeyHint **_Utility to display keyboard shortcuts
-or other hints based on the active window on Linux. (GTK 4.6+ required!)_**
+or other hints based on the active window on Linux._**
 
        [Tests passing]_[_L_i_c_e_n_s_e_:_ _M_I_T_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]
 ![Keyhint Screenshot](https://raw.githubusercontent.com/dynobo/keyhint/main/
 keyhint/resources/keyhint.png) ## Prerequisites - Python 3.11+ - GTK 4.6+
-(shipped since Ubuntu 22.04) + dev packages: ```sh sudo apt-get install \
-libgirepository1.0-dev \ libcairo2-dev \ python3-gi \ gobject-introspection \
-libgtk-4-dev ``` ## Installation - `pipx install keyhint` (recommended,
-requires [pipx](https://pipx.pypa.io/)) - _or_ `pip install keyhint` ## Usage -
-Configure a **global hotkey** (e.g. `Ctrl + F1`) **via your system settings**
-to launch `keyhint`. - If KeyHint is launched via hotkey, it detects the
-current active application and shows the appropriate hints. ## CLI Options ```
-Application Options: -c, --cheatsheet=SHEET-ID Show cheatsheet with this ID on
-startup -d, --default-cheatsheet=SHEET-ID Cheatsheet to show in case no
-cheatsheet is found for active application -f, --no-fullscreen Launch window in
-normal window state instead of fullscreen mode -s, --no-section-sort Do not
-sort sections by size, keep order from config toml file -o, --
-orientation=horizontal|vertical Orientation and scroll direction. Default:
-'vertical' -v, --verbose Verbose log output for debugging ``` ## Configuration
-- The **config directory** is `~/.config/keyhint/`. - To **customize existing**
-cheatsheets, copy [the corresponding .toml-file](https://github.com/dynobo/
-keyhint/tree/main/src/keyhint/config) into the config directory. Make your
-changes in a text editor. As long as you don't change the `id` it will
-overwrite the defaults. - To **create new** cheatsheets, I suggest you also
-start with [one of the existing .toml-file](https://github.com/dynobo/keyhint/
-tree/main/src/keyhint/config): - Place it in the config directory and give it a
-good file name. - Change the value `id` to something unique. - Adjust
-`regex_process` and `regex_title` so it will be selected based on the active
+(shipped since Ubuntu 22.04) + related dev packages: ```sh sudo apt-get install
+\ libgirepository1.0-dev \ libcairo2-dev \ python3-gi \ gobject-introspection \
+libgtk-4-dev ``` - Wayland & Gnome: The [Gnome Extension "Window-Calls"](https:
+//extensions.gnome.org/extension/4724/window-calls/) is required to auto-select
+the cheatsheet based on the current active application. ## Installation - `pipx
+install keyhint` (recommended, requires [pipx](https://pipx.pypa.io/)) - _or_
+`pip install keyhint` ## Usage - Configure a **global hotkey** (e.g. `Ctrl +
+F1`) **via your system settings** to launch `keyhint`. - If KeyHint is launched
+via hotkey, it detects the current active application and shows the appropriate
+hints. (This feature won't work reliably when KeyHint ist started via Menu or
+Launcher.) ## CLI Options ``` Application Options: -c, --cheatsheet=SHEET-ID
+Show cheatsheet with this ID on startup -v, --verbose Verbose log output for
+debugging ``` ## Cheatsheet Configuration The content which KeyHint displays is
+configured using [`toml`](https://toml.io/en/) configuration files. KeyHint
+reads those files from two locations: 1. The [built-in directory](https://
+github.com/dynobo/keyhint/tree/main/keyhint/config) 1. The user directory,
+usually located in `~/.config/keyhint` ### How Keyhint selects the cheatsheet
+to show - The cheatsheet to be displayed on startup are selected by comparing
+the value of `regex_wmclass` with the wm_class of the active window and the
+value of `regex_title` with the title of the active window. - The potential
+cheatsheets are processed alphabetically by filename, the first file that
+matches both wm_class and title are getting displayed. - Both of `regex_`
+values are interpreted as **case in-sensitive regular expressions**. - Check
+"Debug Info" in the application menu to get insights about the active window
+and the selected cheatsheet file. ### Customize or add cheatsheets - To
+**change built-in** cheatsheets, copy [the corresponding .toml-file](https://
+github.com/dynobo/keyhint/tree/main/src/keyhint/config) into the config
+directory. Make your changes in a text editor. As long as you don't change the
+`id` it will overwrite the defaults. - To **create new** cheatsheets, I suggest
+you start with [one of the existing .toml-file](https://github.com/dynobo/
+keyhint/tree/main/src/keyhint/config): - Place it in the config directory and
+give it a good file name. - Change the value `id` to something unique. - Adjust
+`regex_wmclass` and `regex_title` so it will be selected based on the active
 window. (See [Tips](#tips)) - Add the `shortcuts` & `label` to a `section`. -
 If you think your cheatsheet might be useful for others, please consider
-opening a pull request or an issue. - You can always **reset a configuration**
-to the shipped version by deleting the `.toml` files from the config folder. -
-You can **include shortcuts from other cheatsheets** add `include = [""]` - You
-can **hide a cheatsheet** by add `hidden = true` in the top block (same level
-as `id` and `title`). ## Tips **Cheatsheet selection:** - The cheatsheet to be
-displayed on startup are selected by comparing the value of `regex_process`
-with the wm_class of the active window and the value of `regex_title` with the
-title of the active window. - The potential cheatsheets are processed
-alphabetically by filename, the first file that matches both wm_class and title
-are getting displayed. - Both of `regex_` values are interpreted as **case in-
-sensitive regular expressions**. - Check "Debug Info" in the application menu
-to get insights about the active window and the selected cheatsheet file.
-**Available cheatsheets:** - Check the [included toml-files](https://
-github.com/dynobo/keyhint/tree/main/src/keyhint/config) to see which
-applications are available by default. - Feel free submit additional `toml-
-files` for further applications. **Differentiate cheatsheets per website:** -
-For showing different browser-cheatsheets depending on the current website, you
-might want to use a browser extension like "[Add URL To Window Title](https://
-addons.mozilla.org/en-US/firefox/addon/add-url-to-window-title/)" and then
-configure the sections in `.toml` to look for the URL in the window title.
-**KeyHint's shortcuts:** - `Ctrl+F`: Start filtering - `Ctrl+S`: Focus sheet
-selection dropdown (press `Enter` to open it) - `Esc`: Exit KeyHint - `â`,
-`â`, `l` or `k`: scroll forward - `â`, `â`, `h` or `j`: scroll backward -
-`PageDown`: scroll page forward - `PageUP`: scroll page backward ## Contribute
-I'm happy about any contribution! Especially I would appreciate submissions to
-improve the [shipped cheatsheets](https://github.com/dynobo/keyhint/tree/main/
-src/keyhint/config). (The current set are the cheatsheets I personally use). ##
-Design Principles - **Don't run as service**
-It shouldn't consume resources in the background, even if this leads to slower
-start-up time. - **No network connection**
+opening a pull request or an issue! - You can always **reset cheatsheets** to
+the shipped version by deleting the corresponding `.toml` files from the config
+folder. - You can **include shortcuts from other cheatsheets** by adding
+`include = [""]` ### Examples #### Hide existing cheatsheets To hide a
+cheatsheet, e.g. the [built-in](https://github.com/dynobo/keyhint/blob/main/
+keyhint/config/tilix.toml) one with the ID `tilix`, create a new file
+`~/.config/keyhint/tilix.toml` with the content: ```toml id = "tilix" hidden =
+true ``` #### Extend existing cheatsheets To add keybindings to an existing
+cheatsheet, e.g. the [built-in](https://github.com/dynobo/keyhint/blob/main/
+keyhint/config/firefox.toml) one with the ID `firefox`, create a new file
+`~/.config/keyhint/firefox.toml` which only contains the ID and the additional
+bindings: ```toml id = "firefox" [section] [section."My Personal Favorites"] #
+New section "Ctrl + Shift + Tab" = "Show all Tabs" # ... ``` #### Add new
+cheatsheet which never gets auto-selected To add a new cheatsheet, which never
+gets automatically selected and displayed by KeyHint, but remains accessible
+through KeyHint's cheatsheet dropdown, create a file `~/.config/keyhint/my-
+app.toml`: ```toml id = "my-app" url = "url-to-my-apps-keybindings" [match]
+regex_wmclass = "a^" # Patter which never matches regex_title = "a^" [section]
+[section.General] "Ctrl + C" = "Copy" # ... ``` #### Different cheatsheets for
+different Websites For showing different browser-cheatsheets depending on the
+current website, you might want to use a browser extension like "[Add URL To
+Window Title](https://addons.mozilla.org/en-US/firefox/addon/add-url-to-window-
+title/)" and configure the `[match]` section to look for the url in the title.
+E.g. `~/.config/keyhint/github.toml` ```toml id = "github.com" [match]
+regex_wmclass = "Firefox" regex_title = ".*github\\.com.*" # URL added by
+browser extensions to window title [section] [section.Repositories] gc = "Goto
+code tab" # ... ``` ## Contribute I'm happy about any contribution! Especially
+I would appreciate submissions to improve the [shipped cheatsheets](https://
+github.com/dynobo/keyhint/tree/main/src/keyhint/config). (The current set are
+the cheatsheets I personally use). ## Design Principles - **Don't run as
+service**
+It shouldn't consume resources in the background, even if this leads to
+slightly slower start-up time. - **No network connection**
 Everything should run locally without any network communication. -
 **Dependencies**
-The fewer dependencies, the better. - **Multi-Monitors**
-Supports setups with two or more displays ## Certification ![WOMM](https://
+The fewer dependencies, the better. ## Certification ![WOMM](https://
 raw.githubusercontent.com/dynobo/lmdiag/master/badge.png)
```

