# Comparing `tmp/simpleautogui-0.0.5.tar.gz` & `tmp/simpleautogui-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleautogui-0.0.5.tar", last modified: Wed Jan 17 21:12:17 2024, max compression
+gzip compressed data, was "simpleautogui-0.0.6.tar", last modified: Tue Apr 23 17:05:10 2024, max compression
```

## Comparing `simpleautogui-0.0.5.tar` & `simpleautogui-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.364622 simpleautogui-0.0.5/
--rw-rw-rw-   0        0        0     1083 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     9690 2024-01-17 21:12:17.364622 simpleautogui-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     8880 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/README.md
--rw-rw-rw-   0        0        0      875 2024-01-17 21:12:08.000000 simpleautogui-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-17 21:12:17.364622 simpleautogui-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.336083 simpleautogui-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.336083 simpleautogui-0.0.5/src/docs/
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.340846 simpleautogui-0.0.5/src/docs/source/
--rw-rw-rw-   0        0        0      733 2024-01-17 13:40:11.000000 simpleautogui-0.0.5/src/docs/source/conf.py
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.341596 simpleautogui-0.0.5/src/simpleautogui/
--rw-rw-rw-   0        0        0      127 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.352360 simpleautogui-0.0.5/src/simpleautogui/base/
--rw-rw-rw-   0        0        0       58 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/base/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.356859 simpleautogui-0.0.5/src/simpleautogui/base/classes/
--rw-rw-rw-   0        0        0        0 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/base/classes/__init__.py
--rw-rw-rw-   0        0        0    12611 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/base/classes/base.py
--rw-rw-rw-   0        0        0      509 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/base/classes/notify.py
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.357865 simpleautogui-0.0.5/src/simpleautogui/screen/
--rw-rw-rw-   0        0        0      126 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/screen/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.361624 simpleautogui-0.0.5/src/simpleautogui/screen/utils/
--rw-rw-rw-   0        0        0        0 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/screen/utils/__init__.py
--rw-rw-rw-   0        0        0     3700 2024-01-17 14:28:27.000000 simpleautogui-0.0.5/src/simpleautogui/screen/utils/colors.py
--rw-rw-rw-   0        0        0     3807 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/screen/utils/images.py
--rw-rw-rw-   0        0        0     1281 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/screen/utils/proximity.py
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.362372 simpleautogui-0.0.5/src/simpleautogui/win/
--rw-rw-rw-   0        0        0       22 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/win/__init__.py
--rw-rw-rw-   0        0        0     3471 2024-01-17 03:59:07.000000 simpleautogui-0.0.5/src/simpleautogui/win/windows.py
-drwxrwxrwx   0        0        0        0 2024-01-17 21:12:17.363872 simpleautogui-0.0.5/src/simpleautogui.egg-info/
--rw-rw-rw-   0        0        0     9690 2024-01-17 21:12:17.000000 simpleautogui-0.0.5/src/simpleautogui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      721 2024-01-17 21:12:17.000000 simpleautogui-0.0.5/src/simpleautogui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 21:12:17.000000 simpleautogui-0.0.5/src/simpleautogui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2024-01-17 21:12:17.000000 simpleautogui-0.0.5/src/simpleautogui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-01-17 21:12:17.000000 simpleautogui-0.0.5/src/simpleautogui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.505230 simpleautogui-0.0.6/
+-rw-rw-rw-   0        0        0     1083 2024-01-17 03:59:07.000000 simpleautogui-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    11992 2024-04-23 17:05:10.505230 simpleautogui-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11066 2024-04-23 16:04:45.000000 simpleautogui-0.0.6/README.md
+-rw-rw-rw-   0        0        0      972 2024-04-23 17:05:06.000000 simpleautogui-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 17:05:10.505980 simpleautogui-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.496230 simpleautogui-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.499230 simpleautogui-0.0.6/src/simpleautogui/
+-rw-rw-rw-   0        0        0      250 2024-04-23 11:21:26.000000 simpleautogui-0.0.6/src/simpleautogui/__init__.py
+-rw-rw-rw-   0        0        0      511 2024-04-22 20:19:51.000000 simpleautogui-0.0.6/src/simpleautogui/notify.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.501480 simpleautogui-0.0.6/src/simpleautogui/screen/
+-rw-rw-rw-   0        0        0        0 2024-01-19 21:33:05.000000 simpleautogui-0.0.6/src/simpleautogui/screen/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.502230 simpleautogui-0.0.6/src/simpleautogui/screen/classes/
+-rw-rw-rw-   0        0        0        0 2024-01-19 21:16:07.000000 simpleautogui-0.0.6/src/simpleautogui/screen/classes/__init__.py
+-rw-rw-rw-   0        0        0    22402 2024-04-23 16:02:53.000000 simpleautogui-0.0.6/src/simpleautogui/screen/classes/base.py
+-rw-rw-rw-   0        0        0      147 2024-04-22 20:19:51.000000 simpleautogui-0.0.6/src/simpleautogui/screen/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.502230 simpleautogui-0.0.6/src/simpleautogui/win/
+-rw-rw-rw-   0        0        0        0 2024-01-17 23:50:15.000000 simpleautogui-0.0.6/src/simpleautogui/win/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.502980 simpleautogui-0.0.6/src/simpleautogui/win/console/
+-rw-rw-rw-   0        0        0     1006 2024-04-23 10:28:39.000000 simpleautogui-0.0.6/src/simpleautogui/win/console/base.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.502980 simpleautogui-0.0.6/src/simpleautogui/win/console/exceptions/
+-rw-rw-rw-   0        0        0       51 2024-04-22 20:45:57.000000 simpleautogui-0.0.6/src/simpleautogui/win/console/exceptions/base.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.503731 simpleautogui-0.0.6/src/simpleautogui/win/windows/
+-rw-rw-rw-   0        0        0        0 2024-01-17 23:48:24.000000 simpleautogui-0.0.6/src/simpleautogui/win/windows/__init__.py
+-rw-rw-rw-   0        0        0     9149 2024-04-23 16:02:53.000000 simpleautogui-0.0.6/src/simpleautogui/win/windows/classes.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.504480 simpleautogui-0.0.6/src/simpleautogui/win/windows/exceptions/
+-rw-rw-rw-   0        0        0      445 2024-04-23 11:21:26.000000 simpleautogui-0.0.6/src/simpleautogui/win/windows/exceptions/base.py
+drwxrwxrwx   0        0        0        0 2024-04-23 17:05:10.504480 simpleautogui-0.0.6/src/simpleautogui.egg-info/
+-rw-rw-rw-   0        0        0    11992 2024-04-23 17:05:10.000000 simpleautogui-0.0.6/src/simpleautogui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      704 2024-04-23 17:05:10.000000 simpleautogui-0.0.6/src/simpleautogui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 17:05:10.000000 simpleautogui-0.0.6/src/simpleautogui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2024-04-23 17:05:10.000000 simpleautogui-0.0.6/src/simpleautogui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 17:05:10.000000 simpleautogui-0.0.6/src/simpleautogui.egg-info/top_level.txt
```

### Comparing `simpleautogui-0.0.5/LICENSE` & `simpleautogui-0.0.6/LICENSE`

 * *Files identical despite different names*

