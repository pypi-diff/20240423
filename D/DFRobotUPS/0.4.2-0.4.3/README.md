# Comparing `tmp/DFRobotUPS-0.4.2.tar.gz` & `tmp/DFRobotUPS-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DFRobotUPS-0.4.2.tar", last modified: Tue Apr 23 00:31:38 2024, max compression
+gzip compressed data, was "DFRobotUPS-0.4.3.tar", last modified: Tue Apr 23 00:37:33 2024, max compression
```

## Comparing `DFRobotUPS-0.4.2.tar` & `DFRobotUPS-0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:31:38.075101 DFRobotUPS-0.4.2/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:31:38.075101 DFRobotUPS-0.4.2/DFRobotUPS/
--rw-r--r--   0 pi        (1000) pi        (1000)      327 2024-04-23 00:30:13.000000 DFRobotUPS-0.4.2/DFRobotUPS/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6216 2024-04-23 00:29:44.000000 DFRobotUPS-0.4.2/DFRobotUPS/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4677 2024-04-22 21:59:25.000000 DFRobotUPS-0.4.2/DFRobotUPS/ups.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:31:38.075101 DFRobotUPS-0.4.2/DFRobotUPS.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-23 00:31:37.000000 DFRobotUPS-0.4.2/DFRobotUPS.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-23 00:31:37.000000 DFRobotUPS-0.4.2/DFRobotUPS.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-23 00:31:37.000000 DFRobotUPS-0.4.2/DFRobotUPS.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-23 00:31:37.000000 DFRobotUPS-0.4.2/DFRobotUPS.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-23 00:31:37.000000 DFRobotUPS-0.4.2/DFRobotUPS.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.2/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-23 00:31:38.075101 DFRobotUPS-0.4.2/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.2/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-23 00:31:38.085101 DFRobotUPS-0.4.2/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.2/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:37:33.726415 DFRobotUPS-0.4.3/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:37:33.726415 DFRobotUPS-0.4.3/DFRobotUPS/
+-rw-r--r--   0 pi        (1000) pi        (1000)      327 2024-04-23 00:35:59.000000 DFRobotUPS-0.4.3/DFRobotUPS/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6347 2024-04-23 00:35:19.000000 DFRobotUPS-0.4.3/DFRobotUPS/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4677 2024-04-22 21:59:25.000000 DFRobotUPS-0.4.3/DFRobotUPS/ups.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-23 00:37:33.726415 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      269 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        6 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2024-04-23 00:37:33.000000 DFRobotUPS-0.4.3/DFRobotUPS.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)     1072 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.3/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1711 2024-04-23 00:37:33.736415 DFRobotUPS-0.4.3/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      817 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.3/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      102 2024-04-23 00:37:33.736415 DFRobotUPS-0.4.3/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)     1859 2024-04-19 23:42:10.000000 DFRobotUPS-0.4.3/setup.py
```

### Comparing `DFRobotUPS-0.4.2/DFRobotUPS/__main__.py` & `DFRobotUPS-0.4.3/DFRobotUPS/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,34 +131,39 @@
 
 # create logger object and set the overall debugging level (we'll
 # override this in each handler, below, but this level stops anything
 # being logged that is less severe, in any handler)
 logger = logging.getLogger("DFRobotUPS")
 logger.setLevel(logging.DEBUG)
 
-# create logging handler with formatter for syslog - we only log above
-# WARNING here if the shutdown mode is enabled
-syslog_loghandler = logging.handlers.SysLogHandler(address="/dev/log")
-syslog_logformatter = logging.Formatter("%(name)s[%(process)d]: %(message)s")
-syslog_loghandler.setFormatter(syslog_logformatter)
-syslog_loghandler.setLevel(logging.INFO if args.shutdown else logging.WARNING)
-
 # create logging handler with formatter for stderr - the level here
 # depends on the command line options specified
 stderr_loghandler = logging.StreamHandler(stream=sys.stderr)
 stderr_logformatter = logging.Formatter("%(levelname)s: %(message)s")
 stderr_loghandler.setFormatter(stderr_logformatter)
 stderr_loghandler.setLevel(logging.DEBUG if args.debug >= 2
                                else logging.INFO if args.debug >= 1
                                else logging.WARNING)
 
-# add the handlers as logger destinations
-logger.addHandler(syslog_loghandler)
+# add the stderr handler as a logger destination
 logger.addHandler(stderr_loghandler)
 
+# create a syslog handler, if we're running in shutdown mode
+if args.shutdown:
+    # create logging handler with formatter for syslog - we always log
+    # at INFO level here
+    syslog_loghandler = logging.handlers.SysLogHandler(address="/dev/log")
+    syslog_logformatter = logging.Formatter(
+                              "%(name)s[%(process)d]: %(message)s")
+    syslog_loghandler.setFormatter(syslog_logformatter)
+    syslog_loghandler.setLevel(logging.INFO)
+
+    # add the syslog handler as a logger destination
+    logger.addHandler(syslog_loghandler)
+
 
 
 # --- main ---
 
 
 
 logger.info(
```

### Comparing `DFRobotUPS-0.4.2/DFRobotUPS/ups.py` & `DFRobotUPS-0.4.3/DFRobotUPS/ups.py`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4.2/DFRobotUPS.egg-info/PKG-INFO` & `DFRobotUPS-0.4.3/DFRobotUPS.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.4.2
+Version: 0.4.3
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.4.2/LICENSE` & `DFRobotUPS-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4.2/PKG-INFO` & `DFRobotUPS-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DFRobotUPS
-Version: 0.4.2
+Version: 0.4.3
 Summary: DFRobotUPS module
 Home-page: https://github.com/mincebert/DFRobotUPS
 Author: Robert Franklin
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/mincebert/DFRobotUPS/issues
 Project-URL: Source, https://github.com/mincebert/DFRobotUPS
 Description: DFROBOTUPS MODULE
```

### Comparing `DFRobotUPS-0.4.2/README.md` & `DFRobotUPS-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `DFRobotUPS-0.4.2/setup.py` & `DFRobotUPS-0.4.3/setup.py`

 * *Files identical despite different names*

