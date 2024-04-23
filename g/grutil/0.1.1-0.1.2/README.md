# Comparing `tmp/grutil-0.1.1.tar.gz` & `tmp/grutil-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grutil-0.1.1.tar", max compression
+gzip compressed data, was "grutil-0.1.2.tar", max compression
```

## Comparing `grutil-0.1.1.tar` & `grutil-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      187 2024-04-23 18:15:10.298364 grutil-0.1.1/grutil/__init__.py
--rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.1.1/grutil/afm.py
--rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.1.1/grutil/amka.py
--rw-r--r--   0        0        0     1370 2024-04-23 18:14:53.678536 grutil-0.1.1/grutil/dates.py
--rw-r--r--   0        0        0      276 2024-04-23 18:37:01.818760 grutil-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.1.1/README.md
--rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-04-23 18:15:10.298364 grutil-0.1.2/grutil/__init__.py
+-rw-r--r--   0        0        0      388 2024-04-23 17:34:27.834727 grutil-0.1.2/grutil/afm.py
+-rw-r--r--   0        0        0      596 2024-04-23 17:40:10.985103 grutil-0.1.2/grutil/amka.py
+-rw-r--r--   0        0        0     1369 2024-04-23 18:51:58.450243 grutil-0.1.2/grutil/dates.py
+-rw-r--r--   0        0        0      276 2024-04-23 18:54:30.809796 grutil-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-23 18:22:42.049682 grutil-0.1.2/README.md
+-rw-r--r--   0        0        0      376 1970-01-01 00:00:00.000000 grutil-0.1.2/PKG-INFO
```

### Comparing `grutil-0.1.1/grutil/amka.py` & `grutil-0.1.2/grutil/amka.py`

 * *Files identical despite different names*

### Comparing `grutil-0.1.1/grutil/dates.py` & `grutil-0.1.2/grutil/dates.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,9 +41,9 @@
         return "1000-01-01"
     day = day if len(day) == 2 else "0" + day
     month = month if len(month) == 2 else "0" + month
     return "%s-%s-%s" % (year, month, day)
 
 
 def grdate2date(grdate: str) -> date:
-    day, month, year = grdate.split("\\")
+    day, month, year = grdate.split("/")
     return date(int(year), int(month), int(day))
```

