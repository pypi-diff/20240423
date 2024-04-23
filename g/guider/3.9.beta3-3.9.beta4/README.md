# Comparing `tmp/guider-3.9.beta3.tar.gz` & `tmp/guider-3.9.beta4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/guider-3.9.beta3.tar", last modified: Fri Jul 27 06:46:41 2018, max compression
+gzip compressed data, was "dist/guider-3.9.beta4.tar", last modified: Fri Jul 27 07:21:09 2018, max compression
```

## Comparing `guider-3.9.beta3.tar` & `guider-3.9.beta4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-27 06:46:41.000000 guider-3.9.beta3/
--rw-r--r--   0 root         (0) root         (0)      382 2018-07-27 06:46:41.000000 guider-3.9.beta3/PKG-INFO
--rw-rw-r--   0 iipeace   (1000) iipeace   (1000)     1449 2018-07-27 06:46:38.000000 guider-3.9.beta3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-27 06:46:41.000000 guider-3.9.beta3/guider/
--rwxrwxr-x   0 iipeace   (1000) iipeace   (1000)     1375 2018-07-27 05:19:30.000000 guider-3.9.beta3/guider/guider
--rwxr-xr-x   0 iipeace   (1000) iipeace   (1000)  1132825 2018-07-27 05:19:26.000000 guider-3.9.beta3/guider/guider.py
--rw-rw-r--   0 iipeace   (1000) iipeace   (1000)       40 2017-05-08 01:02:45.000000 guider-3.9.beta3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-27 07:21:09.000000 guider-3.9.beta4/
+-rw-r--r--   0 root         (0) root         (0)      382 2018-07-27 07:21:09.000000 guider-3.9.beta4/PKG-INFO
+-rw-rw-r--   0 iipeace   (1000) iipeace   (1000)     1758 2018-07-27 07:19:33.000000 guider-3.9.beta4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-07-27 07:21:09.000000 guider-3.9.beta4/guider/
+-rwxrwxr-x   0 iipeace   (1000) iipeace   (1000)     1375 2018-07-27 05:19:30.000000 guider-3.9.beta4/guider/guider
+-rwxr-xr-x   0 iipeace   (1000) iipeace   (1000)  1132825 2018-07-27 05:19:26.000000 guider-3.9.beta4/guider/guider.py
+-rw-rw-r--   0 iipeace   (1000) iipeace   (1000)       40 2017-05-08 01:02:45.000000 guider-3.9.beta4/setup.cfg
```

### Comparing `guider-3.9.beta3/guider/guider` & `guider-3.9.beta4/guider/guider`

 * *Files identical despite different names*

### Comparing `guider-3.9.beta3/guider/guider.py` & `guider-3.9.beta4/guider/guider.py`

 * *Files identical despite different names*

