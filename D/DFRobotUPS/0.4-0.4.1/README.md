# Comparing `tmp/DFRobotUPS-0.4.tar.gz` & `tmp/DFRobotUPS-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFRobotUPS-0.4.tar", last modified: Mon Apr 22 23:17:54 2024, max compression
+gzip compressed data, was "DFRobotUPS-0.4.1.tar", last modified: Mon Apr 22 23:38:15 2024, max compression
```

## Comparing `DFRobotUPS-0.4.tar` & `DFRobotUPS-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-22 23:17:54.337849 DFRobotUPS-0.4/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-22 23:17:54.327849 DFRobotUPS-0.4/DFRobotUPS/
--rw-r--r--   0 pi        (1000) pi        (1000)      325 2024-04-22 23:14:06.000000 DFRobotUPS-0.4/DFRobotUPS/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6147 2024-04-22 23:12:22.000000 DFRobotUPS-0.4/DFRobotUPS/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4677 2024-04-22 21:59:25.000000 DFRobotUPS-0.4/DFRobotUPS/ups.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-22 23:17:54.327849 DFRobotUPS-0.4/DFRobotUPS.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1709 2024-04-22 23:17:53.000000 DFRobotUPS-0.4/DFRobotUPS.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-22 23:17:54.000000 DFRobotUPS-0.4/DFRobotUPS.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-22 23:17:53.000000 DFRobotUPS-0.4/DFRobotUPS.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-22 23:17:53.000000 DFRobotUPS-0.4/DFRobotUPS.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-22 23:17:53.000000 DFRobotUPS-0.4/DFRobotUPS.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-19 23:42:10.000000 DFRobotUPS-0.4/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1709 2024-04-22 23:17:54.337849 DFRobotUPS-0.4/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-19 23:42:10.000000 DFRobotUPS-0.4/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-22 23:17:54.337849 DFRobotUPS-0.4/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-19 23:42:10.000000 DFRobotUPS-0.4/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-22 23:38:15.908988 DFRobotUPS-0.4.1/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-22 23:38:15.908988 DFRobotUPS-0.4.1/DFRobotUPS/
+-rw-r--r--   0 pi        (1000) pi        (1000)      327 2024-04-22 23:36:11.000000 DFRobotUPS-0.4.1/DFRobotUPS/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6149 2024-04-22 23:35:43.000000 DFRobotUPS-0.4.1/DFRobotUPS/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4677 2024-04-22 21:59:25.000000 DFRobotUPS-0.4.1/DFRobotUPS/ups.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-22 23:38:15.908988 DFRobotUPS-0.4.1/DFRobotUPS.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-22 23:38:15.000000 DFRobotUPS-0.4.1/DFRobotUPS.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-22 23:38:15.000000 DFRobotUPS-0.4.1/DFRobotUPS.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-22 23:38:15.000000 DFRobotUPS-0.4.1/DFRobotUPS.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-22 23:38:15.000000 DFRobotUPS-0.4.1/DFRobotUPS.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-22 23:38:15.000000 DFRobotUPS-0.4.1/DFRobotUPS.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.1/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-22 23:38:15.908988 DFRobotUPS-0.4.1/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.1/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-22 23:38:15.908988 DFRobotUPS-0.4.1/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.1/setup.py
```

### Comparing `DFRobotUPS-0.4/DFRobotUPS/__main__.py` & `DFRobotUPS-0.4.1/DFRobotUPS/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,31 +205,31 @@
             + (" version %d.%d" % ups.fwver))
 
 
 # if we're in shutdown polling mode, do that
 
 if args.shutdown:
     logger.info(
-        f"Polling SoC for shutdown at {args.percent}% with command:"
-        f" { ' '.join(args.cmd) }")
+        f"initial SoC {ups.soc:.2f}%, polling for shutdown at"
+        f" {args.percent}% with command: { ' '.join(args.cmd) }")
 
     while True:
         soc = ups.soc
 
-        logger.debug(
-            f"SoC currently at {soc:.2f}%, shutdown at {args.percent}%")
-
         if soc <= args.percent:
             break
 
-        logger.debug(f"Sleeping for {args.interval}s")
+        logger.debug(
+            f"current SoC {soc:.2f}% - sleeping for {args.interval}s")
+
         sleep(args.interval)
 
-    logger.info(f"SoC at {soc:.2f}% - triggering shutdown with command:"
-                f" { ' '.join(args.cmd) }")
+    logger.info(
+        f"current SoC {soc:.2f}% has reached shutdown trigger at"
+        f" {args.percent}% - executing:" f" { ' '.join(args.cmd) }")
 
     # execute the shutdown command, which will replace this process
     os.execv(args.cmd[0], args.cmd)
 
     # we'll never get here
```

### Comparing `DFRobotUPS-0.4/DFRobotUPS/ups.py` & `DFRobotUPS-0.4.1/DFRobotUPS/ups.py`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4/DFRobotUPS.egg-info/PKG-INFO` & `DFRobotUPS-0.4.1/DFRobotUPS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.4
+Version: 0.4.1
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.4/LICENSE` & `DFRobotUPS-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4/PKG-INFO` & `DFRobotUPS-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.4
+Version: 0.4.1
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.4/README.md` & `DFRobotUPS-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4/setup.py` & `DFRobotUPS-0.4.1/setup.py`

 * *Files identical despite different names*
