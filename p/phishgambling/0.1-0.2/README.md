# Comparing `tmp/phishgambling-0.1.tar.gz` & `tmp/phishgambling-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phishgambling-0.1.tar", last modified: Tue Apr 23 20:25:05 2024, max compression
+gzip compressed data, was "phishgambling-0.2.tar", last modified: Tue Apr 23 20:32:10 2024, max compression
```

## Comparing `phishgambling-0.1.tar` & `phishgambling-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 20:25:05.761701 phishgambling-0.1/
--rw-rw-rw-   0        0        0      128 2024-04-23 20:25:05.707127 phishgambling-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-23 20:17:27.000000 phishgambling-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 20:25:05.686734 phishgambling-0.1/phishgambling/
--rw-rw-rw-   0        0        0       24 2024-04-23 20:20:40.000000 phishgambling-0.1/phishgambling/__init__.py
--rw-rw-rw-   0        0        0     1676 2024-04-23 20:18:36.000000 phishgambling-0.1/phishgambling/main.py
-drwxrwxrwx   0        0        0        0 2024-04-23 20:25:05.705163 phishgambling-0.1/phishgambling.egg-info/
--rw-rw-rw-   0        0        0      128 2024-04-23 20:25:05.000000 phishgambling-0.1/phishgambling.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-23 20:25:05.000000 phishgambling-0.1/phishgambling.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 20:25:05.000000 phishgambling-0.1/phishgambling.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-23 20:25:05.000000 phishgambling-0.1/phishgambling.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-23 20:25:05.000000 phishgambling-0.1/phishgambling.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-23 20:25:05.761701 phishgambling-0.1/setup.cfg
--rw-rw-rw-   0        0        0      439 2024-04-23 20:23:19.000000 phishgambling-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:32:10.554886 phishgambling-0.2/
+-rw-rw-rw-   0        0        0      128 2024-04-23 20:32:10.552891 phishgambling-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-23 20:17:27.000000 phishgambling-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 20:32:10.532241 phishgambling-0.2/phishgambling/
+-rw-rw-rw-   0        0        0       24 2024-04-23 20:20:40.000000 phishgambling-0.2/phishgambling/__init__.py
+-rw-rw-rw-   0        0        0     1696 2024-04-23 20:31:20.000000 phishgambling-0.2/phishgambling/main.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:32:10.550932 phishgambling-0.2/phishgambling.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-23 20:32:10.000000 phishgambling-0.2/phishgambling.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 20:32:10.554886 phishgambling-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      439 2024-04-23 20:31:44.000000 phishgambling-0.2/setup.py
```

### Comparing `phishgambling-0.1/phishgambling/main.py` & `phishgambling-0.2/phishgambling/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,11 +57,12 @@
     print(line)
 
 
 def main():
     victimScan()
     fake_loading()
     fake_credentials()
+    time.sleep(10)
 
 
 if __name__ == "__main__":
     main()
```

