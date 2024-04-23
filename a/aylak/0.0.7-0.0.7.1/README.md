# Comparing `tmp/aylak-0.0.7.tar.gz` & `tmp/aylak-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aylak-0.0.7.tar", last modified: Thu Mar 28 22:51:54 2024, max compression
+gzip compressed data, was "aylak-0.0.7.1.tar", last modified: Tue Apr 23 19:42:47 2024, max compression
```

## Comparing `aylak-0.0.7.tar` & `aylak-0.0.7.1.tar`

### file list

```diff
@@ -1,121 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:54.328316 aylak-0.0.7/
--rw-rw-rw-   0        0        0     1697 2024-03-28 22:51:54.328316 aylak-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-02-07 14:46:28.000000 aylak-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:53.881286 aylak-0.0.7/aylak/
--rw-rw-rw-   0        0        0      165 2024-03-28 22:51:30.000000 aylak-0.0.7/aylak/__init__.py
--rw-rw-rw-   0        0        0      363 2024-03-13 19:28:53.000000 aylak-0.0.7/aylak/__main__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:53.944515 aylak-0.0.7/aylak/colors/
--rw-rw-rw-   0        0        0    13240 2024-02-10 16:31:48.000000 aylak-0.0.7/aylak/colors/__init__.py
--rw-rw-rw-   0        0        0      768 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/colors/_print.py
--rw-rw-rw-   0        0        0     5830 2024-02-08 19:54:37.000000 aylak-0.0.7/aylak/colors/art.py
--rw-rw-rw-   0        0        0      982 2024-03-16 10:40:41.000000 aylak-0.0.7/aylak/colors/handler.py
--rw-rw-rw-   0        0        0     3995 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/colors/hex.py
--rw-rw-rw-   0        0        0     4681 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/colors/rgb.py
--rw-rw-rw-   0        0        0     1046 2024-02-10 16:28:49.000000 aylak-0.0.7/aylak/colors/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:53.954296 aylak-0.0.7/aylak/exceptions/
--rw-rw-rw-   0        0        0       23 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:53.962296 aylak-0.0.7/aylak/exceptions/colors/
--rw-rw-rw-   0        0        0       27 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/exceptions/colors/__init__.py
--rw-rw-rw-   0        0        0     3962 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/exceptions/colors/exceptions.py
--rw-rw-rw-   0        0        0     1011 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/exceptions/rpc_errors.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:53.968318 aylak-0.0.7/aylak/image/
--rw-rw-rw-   0        0        0       36 2024-03-03 19:38:56.000000 aylak-0.0.7/aylak/image/__init__.py
--rw-rw-rw-   0        0        0     8106 2024-03-03 19:38:48.000000 aylak-0.0.7/aylak/image/imagetool.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:54.285317 aylak-0.0.7/aylak/rich/
--rw-rw-rw-   0        0        0     6279 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/__init__.py
--rw-rw-rw-   0        0        0     8709 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/__main__.py
--rw-rw-rw-   0        0        0    10547 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_cell_widths.py
--rw-rw-rw-   0        0        0     2204 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_export_format.py
--rw-rw-rw-   0        0        0      263 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_extension.py
--rw-rw-rw-   0        0        0      823 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_fileno.py
--rw-rw-rw-   0        0        0     9965 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_inspect.py
--rw-rw-rw-   0        0        0     3313 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_log_render.py
--rw-rw-rw-   0        0        0     1279 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_loop.py
--rw-rw-rw-   0        0        0     1456 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_null_file.py
--rw-rw-rw-   0        0        0     7372 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_palettes.py
--rw-rw-rw-   0        0        0      440 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_pick.py
--rw-rw-rw-   0        0        0     5618 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_ratio.py
--rw-rw-rw-   0        0        0    20401 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_spinners.py
--rw-rw-rw-   0        0        0      367 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_stack.py
--rw-rw-rw-   0        0        0      436 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_timer.py
--rw-rw-rw-   0        0        0    23464 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_win32_console.py
--rw-rw-rw-   0        0        0     1984 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_windows.py
--rw-rw-rw-   0        0        0     2827 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_windows_renderer.py
--rw-rw-rw-   0        0        0     3497 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/_wrap.py
--rw-rw-rw-   0        0        0      917 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/abc.py
--rw-rw-rw-   0        0        0    10649 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/align.py
--rw-rw-rw-   0        0        0     7146 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/ansi.py
--rw-rw-rw-   0        0        0     3356 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/bar.py
--rw-rw-rw-   0        0        0    11281 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/box.py
--rw-rw-rw-   0        0        0     4947 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/cells.py
--rw-rw-rw-   0        0        0    18844 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/color.py
--rw-rw-rw-   0        0        0     1092 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/color_triplet.py
--rw-rw-rw-   0        0        0     7318 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/columns.py
--rw-rw-rw-   0        0        0   101864 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/console.py
--rw-rw-rw-   0        0        0     1325 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/constrain.py
--rw-rw-rw-   0        0        0     5669 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/containers.py
--rw-rw-rw-   0        0        0     6837 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/control.py
--rw-rw-rw-   0        0        0     8254 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/default_styles.py
--rw-rw-rw-   0        0        0      985 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/diagnose.py
--rw-rw-rw-   0        0        0      489 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/emoji.py
--rw-rw-rw-   0        0        0      676 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/errors.py
--rw-rw-rw-   0        0        0     1740 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/file_proxy.py
--rw-rw-rw-   0        0        0     2597 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/filesize.py
--rw-rw-rw-   0        0        0     9817 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/highlighter.py
--rw-rw-rw-   0        0        0     5164 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/json.py
--rw-rw-rw-   0        0        0     3341 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/jupyter.py
--rw-rw-rw-   0        0        0    14416 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/layout.py
--rw-rw-rw-   0        0        0    14646 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/live.py
--rw-rw-rw-   0        0        0     3766 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/live_render.py
--rw-rw-rw-   0        0        0    12192 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/logging.py
--rw-rw-rw-   0        0        0    26979 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/markdown.py
--rw-rw-rw-   0        0        0     8503 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/markup.py
--rw-rw-rw-   0        0        0     5480 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/measure.py
--rw-rw-rw-   0        0        0     5105 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/padding.py
--rw-rw-rw-   0        0        0      862 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/pager.py
--rw-rw-rw-   0        0        0     3442 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/palette.py
--rw-rw-rw-   0        0        0    11017 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/panel.py
--rw-rw-rw-   0        0        0    36825 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/pretty.py
--rw-rw-rw-   0        0        0    61402 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/progress.py
--rw-rw-rw-   0        0        0     8387 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/progress_bar.py
--rw-rw-rw-   0        0        0    11673 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/prompt.py
--rw-rw-rw-   0        0        0     1421 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/protocol.py
--rw-rw-rw-   0        0        0        0 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/py.typed
--rw-rw-rw-   0        0        0      176 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/region.py
--rw-rw-rw-   0        0        0     4574 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/repr.py
--rw-rw-rw-   0        0        0     4726 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/rule.py
--rw-rw-rw-   0        0        0     2923 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/scope.py
--rw-rw-rw-   0        0        0     1639 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/screen.py
--rw-rw-rw-   0        0        0    24972 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/segment.py
--rw-rw-rw-   0        0        0     4476 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/spinner.py
--rw-rw-rw-   0        0        0     4555 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/status.py
--rw-rw-rw-   0        0        0    27869 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/style.py
--rw-rw-rw-   0        0        0     1288 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/styled.py
--rw-rw-rw-   0        0        0    36343 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/syntax.py
--rw-rw-rw-   0        0        0    40662 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/table.py
--rw-rw-rw-   0        0        0     3523 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/terminal_theme.py
--rw-rw-rw-   0        0        0    48678 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/text.py
--rw-rw-rw-   0        0        0     3898 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/theme.py
--rw-rw-rw-   0        0        0      107 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/themes.py
--rw-rw-rw-   0        0        0    30288 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/traceback.py
--rw-rw-rw-   0        0        0     9386 2024-02-07 14:46:28.000000 aylak-0.0.7/aylak/rich/tree.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:54.299286 aylak-0.0.7/aylak/telegram/
--rw-rw-rw-   0        0        0      242 2024-03-28 22:49:30.000000 aylak-0.0.7/aylak/telegram/__init__.py
--rw-rw-rw-   0        0        0      799 2024-03-28 22:47:18.000000 aylak-0.0.7/aylak/telegram/keys.py
--rw-rw-rw-   0        0        0     2537 2024-03-28 22:48:13.000000 aylak-0.0.7/aylak/telegram/progress.py
--rw-rw-rw-   0        0        0     5681 2024-03-13 19:26:57.000000 aylak-0.0.7/aylak/telegram/pyrogram.py
--rw-rw-rw-   0        0        0     4310 2024-03-13 19:43:59.000000 aylak-0.0.7/aylak/telegram/telethon.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:54.311313 aylak-0.0.7/aylak/utils/
--rw-rw-rw-   0        0        0       92 2024-03-28 22:50:49.000000 aylak-0.0.7/aylak/utils/__init__.py
--rw-rw-rw-   0        0        0     3184 2024-03-28 22:21:41.000000 aylak-0.0.7/aylak/utils/human.py
--rw-rw-rw-   0        0        0     3277 2024-03-28 22:39:06.000000 aylak-0.0.7/aylak/utils/paste.py
-drwxrwxrwx   0        0        0        0 2024-03-28 22:51:54.323284 aylak-0.0.7/aylak.egg-info/
--rw-rw-rw-   0        0        0     1697 2024-03-28 22:51:53.000000 aylak-0.0.7/aylak.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2516 2024-03-28 22:51:53.000000 aylak-0.0.7/aylak.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       59 2024-03-28 22:51:53.000000 aylak-0.0.7/aylak.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      130 2024-03-28 22:51:53.000000 aylak-0.0.7/aylak.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-28 22:51:53.000000 aylak-0.0.7/aylak.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       95 2024-03-28 22:51:53.000000 aylak-0.0.7/aylak.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-28 22:51:53.000000 aylak-0.0.7/aylak.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 22:51:54.334701 aylak-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2806 2024-03-13 15:16:14.000000 aylak-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:47.723745 aylak-0.0.7.1/
+-rw-rw-rw-   0        0        0     1508 2024-04-23 19:42:47.725742 aylak-0.0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-02-07 14:46:28.000000 aylak-0.0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:46.600748 aylak-0.0.7.1/aylak/
+-rw-rw-rw-   0        0        0      167 2024-04-23 19:41:55.000000 aylak-0.0.7.1/aylak/__init__.py
+-rw-rw-rw-   0        0        0      363 2024-03-13 19:28:53.000000 aylak-0.0.7.1/aylak/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:46.760766 aylak-0.0.7.1/aylak/colors/
+-rw-rw-rw-   0        0        0    13240 2024-02-10 16:31:48.000000 aylak-0.0.7.1/aylak/colors/__init__.py
+-rw-rw-rw-   0        0        0      768 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/colors/_print.py
+-rw-rw-rw-   0        0        0     5830 2024-02-08 19:54:37.000000 aylak-0.0.7.1/aylak/colors/art.py
+-rw-rw-rw-   0        0        0      982 2024-03-16 10:40:41.000000 aylak-0.0.7.1/aylak/colors/handler.py
+-rw-rw-rw-   0        0        0     3995 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/colors/hex.py
+-rw-rw-rw-   0        0        0     4681 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/colors/rgb.py
+-rw-rw-rw-   0        0        0     1046 2024-02-10 16:28:49.000000 aylak-0.0.7.1/aylak/colors/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:46.777725 aylak-0.0.7.1/aylak/exceptions/
+-rw-rw-rw-   0        0        0       23 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:46.785724 aylak-0.0.7.1/aylak/exceptions/colors/
+-rw-rw-rw-   0        0        0       27 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/exceptions/colors/__init__.py
+-rw-rw-rw-   0        0        0     3962 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/exceptions/colors/exceptions.py
+-rw-rw-rw-   0        0        0     1011 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/exceptions/rpc_errors.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:46.797724 aylak-0.0.7.1/aylak/image/
+-rw-rw-rw-   0        0        0       36 2024-03-03 19:38:56.000000 aylak-0.0.7.1/aylak/image/__init__.py
+-rw-rw-rw-   0        0        0     8106 2024-03-03 19:38:48.000000 aylak-0.0.7.1/aylak/image/imagetool.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:47.644765 aylak-0.0.7.1/aylak/rich/
+-rw-rw-rw-   0        0        0     6279 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/__init__.py
+-rw-rw-rw-   0        0        0     8709 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/__main__.py
+-rw-rw-rw-   0        0        0    10547 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_cell_widths.py
+-rw-rw-rw-   0        0        0     2204 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_export_format.py
+-rw-rw-rw-   0        0        0      263 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_extension.py
+-rw-rw-rw-   0        0        0      823 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_fileno.py
+-rw-rw-rw-   0        0        0     9965 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_inspect.py
+-rw-rw-rw-   0        0        0     3313 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_log_render.py
+-rw-rw-rw-   0        0        0     1279 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_loop.py
+-rw-rw-rw-   0        0        0     1456 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_null_file.py
+-rw-rw-rw-   0        0        0     7372 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_palettes.py
+-rw-rw-rw-   0        0        0      440 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_pick.py
+-rw-rw-rw-   0        0        0     5618 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_ratio.py
+-rw-rw-rw-   0        0        0    20401 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_spinners.py
+-rw-rw-rw-   0        0        0      367 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_stack.py
+-rw-rw-rw-   0        0        0      436 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_timer.py
+-rw-rw-rw-   0        0        0    23464 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_win32_console.py
+-rw-rw-rw-   0        0        0     1984 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_windows.py
+-rw-rw-rw-   0        0        0     2827 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_windows_renderer.py
+-rw-rw-rw-   0        0        0     3497 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/_wrap.py
+-rw-rw-rw-   0        0        0      917 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/abc.py
+-rw-rw-rw-   0        0        0    10649 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/align.py
+-rw-rw-rw-   0        0        0     7146 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/ansi.py
+-rw-rw-rw-   0        0        0     3356 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/bar.py
+-rw-rw-rw-   0        0        0    11281 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/box.py
+-rw-rw-rw-   0        0        0     4947 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/cells.py
+-rw-rw-rw-   0        0        0    18844 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/color.py
+-rw-rw-rw-   0        0        0     1092 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/color_triplet.py
+-rw-rw-rw-   0        0        0     7318 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/columns.py
+-rw-rw-rw-   0        0        0   101864 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/console.py
+-rw-rw-rw-   0        0        0     1325 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/constrain.py
+-rw-rw-rw-   0        0        0     5669 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/containers.py
+-rw-rw-rw-   0        0        0     6837 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/control.py
+-rw-rw-rw-   0        0        0     8254 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/default_styles.py
+-rw-rw-rw-   0        0        0      985 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/diagnose.py
+-rw-rw-rw-   0        0        0      489 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/emoji.py
+-rw-rw-rw-   0        0        0      676 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/errors.py
+-rw-rw-rw-   0        0        0     1740 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/file_proxy.py
+-rw-rw-rw-   0        0        0     2597 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/filesize.py
+-rw-rw-rw-   0        0        0     9817 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/highlighter.py
+-rw-rw-rw-   0        0        0     5164 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/json.py
+-rw-rw-rw-   0        0        0     3341 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/jupyter.py
+-rw-rw-rw-   0        0        0    14416 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/layout.py
+-rw-rw-rw-   0        0        0    14646 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/live.py
+-rw-rw-rw-   0        0        0     3766 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/live_render.py
+-rw-rw-rw-   0        0        0    12192 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/logging.py
+-rw-rw-rw-   0        0        0    26979 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/markdown.py
+-rw-rw-rw-   0        0        0     8503 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/markup.py
+-rw-rw-rw-   0        0        0     5480 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/measure.py
+-rw-rw-rw-   0        0        0     5105 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/padding.py
+-rw-rw-rw-   0        0        0      862 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/pager.py
+-rw-rw-rw-   0        0        0     3442 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/palette.py
+-rw-rw-rw-   0        0        0    11017 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/panel.py
+-rw-rw-rw-   0        0        0    36825 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/pretty.py
+-rw-rw-rw-   0        0        0    61402 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/progress.py
+-rw-rw-rw-   0        0        0     8387 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/progress_bar.py
+-rw-rw-rw-   0        0        0    11673 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/prompt.py
+-rw-rw-rw-   0        0        0     1421 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/protocol.py
+-rw-rw-rw-   0        0        0      176 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/region.py
+-rw-rw-rw-   0        0        0     4574 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/repr.py
+-rw-rw-rw-   0        0        0     4726 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/rule.py
+-rw-rw-rw-   0        0        0     2923 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/scope.py
+-rw-rw-rw-   0        0        0     1639 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/screen.py
+-rw-rw-rw-   0        0        0    24972 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/segment.py
+-rw-rw-rw-   0        0        0     4476 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/spinner.py
+-rw-rw-rw-   0        0        0     4555 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/status.py
+-rw-rw-rw-   0        0        0    27869 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/style.py
+-rw-rw-rw-   0        0        0     1288 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/styled.py
+-rw-rw-rw-   0        0        0    36343 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/syntax.py
+-rw-rw-rw-   0        0        0    40662 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/table.py
+-rw-rw-rw-   0        0        0     3523 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/terminal_theme.py
+-rw-rw-rw-   0        0        0    48678 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/text.py
+-rw-rw-rw-   0        0        0     3898 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/theme.py
+-rw-rw-rw-   0        0        0      107 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/themes.py
+-rw-rw-rw-   0        0        0    30288 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/traceback.py
+-rw-rw-rw-   0        0        0     9386 2024-02-07 14:46:28.000000 aylak-0.0.7.1/aylak/rich/tree.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:47.685813 aylak-0.0.7.1/aylak/telegram/
+-rw-rw-rw-   0        0        0      242 2024-03-28 22:49:30.000000 aylak-0.0.7.1/aylak/telegram/__init__.py
+-rw-rw-rw-   0        0        0      799 2024-03-28 22:47:18.000000 aylak-0.0.7.1/aylak/telegram/keys.py
+-rw-rw-rw-   0        0        0     2537 2024-03-28 22:48:13.000000 aylak-0.0.7.1/aylak/telegram/progress.py
+-rw-rw-rw-   0        0        0     5637 2024-04-23 19:42:19.000000 aylak-0.0.7.1/aylak/telegram/pyrogram.py
+-rw-rw-rw-   0        0        0     4310 2024-03-13 19:43:59.000000 aylak-0.0.7.1/aylak/telegram/telethon.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:47.714742 aylak-0.0.7.1/aylak/utils/
+-rw-rw-rw-   0        0        0       92 2024-03-28 22:50:49.000000 aylak-0.0.7.1/aylak/utils/__init__.py
+-rw-rw-rw-   0        0        0     3184 2024-03-28 22:21:41.000000 aylak-0.0.7.1/aylak/utils/human.py
+-rw-rw-rw-   0        0        0     3277 2024-03-28 22:39:06.000000 aylak-0.0.7.1/aylak/utils/paste.py
+drwxrwxrwx   0        0        0        0 2024-04-23 19:42:46.677722 aylak-0.0.7.1/aylak.egg-info/
+-rw-rw-rw-   0        0        0     1508 2024-04-23 19:42:45.000000 aylak-0.0.7.1/aylak.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2496 2024-04-23 19:42:45.000000 aylak-0.0.7.1/aylak.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       59 2024-04-23 19:42:45.000000 aylak-0.0.7.1/aylak.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-04-23 19:42:45.000000 aylak-0.0.7.1/aylak.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-23 19:42:45.000000 aylak-0.0.7.1/aylak.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       74 2024-04-23 19:42:45.000000 aylak-0.0.7.1/aylak.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-23 19:42:45.000000 aylak-0.0.7.1/aylak.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 19:42:47.727741 aylak-0.0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     2777 2024-04-23 19:41:49.000000 aylak-0.0.7.1/setup.py
```

### Comparing `aylak-0.0.7/PKG-INFO` & `aylak-0.0.7.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aylak
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Aylak PyPi
 Home-page: https://github.com/aylak-github/aylak-pypi
 Author: aylak-github
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: aylak,pypi,aylak-pypi,aylak-pypi
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,13 +26,7 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: pythonansi==1.0.2
-Requires-Dist: aiofiles==23.2.1
-Requires-Dist: cryptography==42.0.5
-Requires-Dist: pillow==10.2.0
-Requires-Dist: aiohttp>=3.8.1
-Requires-Dist: telethon
```

### Comparing `aylak-0.0.7/aylak/colors/__init__.py` & `aylak-0.0.7.1/aylak/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/colors/_print.py` & `aylak-0.0.7.1/aylak/colors/_print.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/colors/art.py` & `aylak-0.0.7.1/aylak/colors/art.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/colors/handler.py` & `aylak-0.0.7.1/aylak/colors/handler.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/colors/hex.py` & `aylak-0.0.7.1/aylak/colors/hex.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/colors/rgb.py` & `aylak-0.0.7.1/aylak/colors/rgb.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/colors/utils.py` & `aylak-0.0.7.1/aylak/colors/utils.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/exceptions/colors/exceptions.py` & `aylak-0.0.7.1/aylak/exceptions/colors/exceptions.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/exceptions/rpc_errors.py` & `aylak-0.0.7.1/aylak/exceptions/rpc_errors.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/image/imagetool.py` & `aylak-0.0.7.1/aylak/image/imagetool.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/__init__.py` & `aylak-0.0.7.1/aylak/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/__main__.py` & `aylak-0.0.7.1/aylak/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_cell_widths.py` & `aylak-0.0.7.1/aylak/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_export_format.py` & `aylak-0.0.7.1/aylak/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_fileno.py` & `aylak-0.0.7.1/aylak/rich/_fileno.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_inspect.py` & `aylak-0.0.7.1/aylak/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_log_render.py` & `aylak-0.0.7.1/aylak/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_loop.py` & `aylak-0.0.7.1/aylak/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_null_file.py` & `aylak-0.0.7.1/aylak/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_palettes.py` & `aylak-0.0.7.1/aylak/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_ratio.py` & `aylak-0.0.7.1/aylak/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_spinners.py` & `aylak-0.0.7.1/aylak/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_win32_console.py` & `aylak-0.0.7.1/aylak/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_windows.py` & `aylak-0.0.7.1/aylak/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_windows_renderer.py` & `aylak-0.0.7.1/aylak/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/_wrap.py` & `aylak-0.0.7.1/aylak/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/abc.py` & `aylak-0.0.7.1/aylak/rich/abc.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/align.py` & `aylak-0.0.7.1/aylak/rich/align.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/ansi.py` & `aylak-0.0.7.1/aylak/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/bar.py` & `aylak-0.0.7.1/aylak/rich/bar.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/box.py` & `aylak-0.0.7.1/aylak/rich/box.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/cells.py` & `aylak-0.0.7.1/aylak/rich/cells.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/color.py` & `aylak-0.0.7.1/aylak/rich/color.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/color_triplet.py` & `aylak-0.0.7.1/aylak/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/columns.py` & `aylak-0.0.7.1/aylak/rich/columns.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/console.py` & `aylak-0.0.7.1/aylak/rich/console.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/constrain.py` & `aylak-0.0.7.1/aylak/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/containers.py` & `aylak-0.0.7.1/aylak/rich/containers.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/control.py` & `aylak-0.0.7.1/aylak/rich/control.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/default_styles.py` & `aylak-0.0.7.1/aylak/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/diagnose.py` & `aylak-0.0.7.1/aylak/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/errors.py` & `aylak-0.0.7.1/aylak/rich/errors.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/file_proxy.py` & `aylak-0.0.7.1/aylak/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/filesize.py` & `aylak-0.0.7.1/aylak/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/highlighter.py` & `aylak-0.0.7.1/aylak/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/json.py` & `aylak-0.0.7.1/aylak/rich/json.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/jupyter.py` & `aylak-0.0.7.1/aylak/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/layout.py` & `aylak-0.0.7.1/aylak/rich/layout.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/live.py` & `aylak-0.0.7.1/aylak/rich/live.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/live_render.py` & `aylak-0.0.7.1/aylak/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/logging.py` & `aylak-0.0.7.1/aylak/rich/logging.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/markdown.py` & `aylak-0.0.7.1/aylak/rich/markdown.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/markup.py` & `aylak-0.0.7.1/aylak/rich/markup.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/measure.py` & `aylak-0.0.7.1/aylak/rich/measure.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/padding.py` & `aylak-0.0.7.1/aylak/rich/padding.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/pager.py` & `aylak-0.0.7.1/aylak/rich/pager.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/palette.py` & `aylak-0.0.7.1/aylak/rich/palette.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/panel.py` & `aylak-0.0.7.1/aylak/rich/panel.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/pretty.py` & `aylak-0.0.7.1/aylak/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/progress.py` & `aylak-0.0.7.1/aylak/rich/progress.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/progress_bar.py` & `aylak-0.0.7.1/aylak/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/prompt.py` & `aylak-0.0.7.1/aylak/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/protocol.py` & `aylak-0.0.7.1/aylak/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/repr.py` & `aylak-0.0.7.1/aylak/rich/repr.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/rule.py` & `aylak-0.0.7.1/aylak/rich/rule.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/scope.py` & `aylak-0.0.7.1/aylak/rich/scope.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/screen.py` & `aylak-0.0.7.1/aylak/rich/screen.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/segment.py` & `aylak-0.0.7.1/aylak/rich/segment.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/spinner.py` & `aylak-0.0.7.1/aylak/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/status.py` & `aylak-0.0.7.1/aylak/rich/status.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/style.py` & `aylak-0.0.7.1/aylak/rich/style.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/styled.py` & `aylak-0.0.7.1/aylak/rich/styled.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/syntax.py` & `aylak-0.0.7.1/aylak/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/table.py` & `aylak-0.0.7.1/aylak/rich/table.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/terminal_theme.py` & `aylak-0.0.7.1/aylak/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/text.py` & `aylak-0.0.7.1/aylak/rich/text.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/theme.py` & `aylak-0.0.7.1/aylak/rich/theme.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/traceback.py` & `aylak-0.0.7.1/aylak/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/rich/tree.py` & `aylak-0.0.7.1/aylak/rich/tree.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/telegram/keys.py` & `aylak-0.0.7.1/aylak/telegram/keys.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/telegram/progress.py` & `aylak-0.0.7.1/aylak/telegram/progress.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/telegram/pyrogram.py` & `aylak-0.0.7.1/aylak/telegram/pyrogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from aylak.colors import Renkler
 from aylak.telegram.keys import get_keys
 from pyrogram import Client
 from pyrogram.errors import *
 
 renkler = Renkler()
-url = "http://basicbots.pw:5000/api-keys/"
 
 
 async def pyrogram_string():
     print(f"{renkler.turkuaz}Pyrogram String Session Oluşturucu")
     ah, ai = get_keys()
 
     client = Client(
```

### Comparing `aylak-0.0.7/aylak/telegram/telethon.py` & `aylak-0.0.7.1/aylak/telegram/telethon.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/utils/human.py` & `aylak-0.0.7.1/aylak/utils/human.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak/utils/paste.py` & `aylak-0.0.7.1/aylak/utils/paste.py`

 * *Files identical despite different names*

### Comparing `aylak-0.0.7/aylak.egg-info/PKG-INFO` & `aylak-0.0.7.1/aylak.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aylak
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Aylak PyPi
 Home-page: https://github.com/aylak-github/aylak-pypi
 Author: aylak-github
 Author-email: contact@yakupkaya.net.tr
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Keywords: aylak,pypi,aylak-pypi,aylak-pypi
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,13 +26,7 @@
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: pythonansi==1.0.2
-Requires-Dist: aiofiles==23.2.1
-Requires-Dist: cryptography==42.0.5
-Requires-Dist: pillow==10.2.0
-Requires-Dist: aiohttp>=3.8.1
-Requires-Dist: telethon
```

### Comparing `aylak-0.0.7/aylak.egg-info/SOURCES.txt` & `aylak-0.0.7.1/aylak.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 aylak/rich/palette.py
 aylak/rich/panel.py
 aylak/rich/pretty.py
 aylak/rich/progress.py
 aylak/rich/progress_bar.py
 aylak/rich/prompt.py
 aylak/rich/protocol.py
-aylak/rich/py.typed
 aylak/rich/region.py
 aylak/rich/repr.py
 aylak/rich/rule.py
 aylak/rich/scope.py
 aylak/rich/screen.py
 aylak/rich/segment.py
 aylak/rich/spinner.py
```

### Comparing `aylak-0.0.7/setup.py` & `aylak-0.0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 """
 with open("requirements.txt", "r", encoding="utf-8") as r:
     requirements = [i.strip() for i in r]"""
 
 requirements = [
     "pythonansi==1.0.2",
     "aiofiles==23.2.1",
-    "cryptography==42.0.5",
     "pillow==10.2.0",
     "aiohttp>=3.8.1",
     "telethon",
     # "git+https://github.com/KurimuzonAkuma/pyrogram.git@v2.1.15",
 ]
 
 with open("aylak/__init__.py", encoding="utf-8") as f:
```

