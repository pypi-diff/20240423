# Comparing `tmp/chargespot-0.0.2.tar.gz` & `tmp/chargespot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chargespot-0.0.2.tar", last modified: Tue Apr 23 06:28:15 2024, max compression
+gzip compressed data, was "chargespot-0.0.3.tar", last modified: Tue Apr 23 08:59:40 2024, max compression
```

## Comparing `chargespot-0.0.2.tar` & `chargespot-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.012318 chargespot-0.0.2/
--rw-r--r--   0 lzp        (501) staff       (20)    11357 2024-03-25 06:10:08.000000 chargespot-0.0.2/LICENSE
--rw-r--r--   0 lzp        (501) staff       (20)       74 2024-04-23 04:16:18.000000 chargespot-0.0.2/MANIFEST.in
--rw-r--r--   0 lzp        (501) staff       (20)      394 2024-04-23 06:28:15.011782 chargespot-0.0.2/PKG-INFO
--rw-r--r--   0 lzp        (501) staff       (20)    21601 2024-04-19 07:27:07.000000 chargespot-0.0.2/README.md
--rw-r--r--   0 lzp        (501) staff       (20)       38 2024-04-23 06:28:15.012402 chargespot-0.0.2/setup.cfg
--rw-r--r--   0 lzp        (501) staff       (20)      615 2024-04-23 06:27:26.000000 chargespot-0.0.2/setup.py
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:14.995784 chargespot-0.0.2/src/
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.003978 chargespot-0.0.2/src/chargespot/
--rw-r--r--   0 lzp        (501) staff       (20)      383 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/__init__.py
--rw-r--r--   0 lzp        (501) staff       (20)    12118 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/api_decorator.py
--rw-r--r--   0 lzp        (501) staff       (20)     2460 2024-04-23 06:27:26.000000 chargespot-0.0.2/src/chargespot/cli.py
--rw-r--r--   0 lzp        (501) staff       (20)     5415 2024-04-19 07:27:07.000000 chargespot-0.0.2/src/chargespot/config_manager.py
--rw-r--r--   0 lzp        (501) staff       (20)     7887 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/email_report_template.html
--rw-r--r--   0 lzp        (501) staff       (20)      110 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/exceptions.py
--rw-r--r--   0 lzp        (501) staff       (20)      130 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/execute.py
--rw-r--r--   0 lzp        (501) staff       (20)    10691 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/heman_datetime.py
--rw-r--r--   0 lzp        (501) staff       (20)     9624 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/report.py
--rw-r--r--   0 lzp        (501) staff       (20)     4966 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/swagger.py
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.008041 chargespot-0.0.2/src/chargespot/templates/
--rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/templates/.chargespot
--rw-r--r--   0 lzp        (501) staff       (20)     1063 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/templates/.gitignore
--rw-r--r--   0 lzp        (501) staff       (20)     2346 2024-04-19 07:27:07.000000 chargespot-0.0.2/src/chargespot/templates/README.md
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.008926 chargespot-0.0.2/src/chargespot/templates/api/
--rw-r--r--   0 lzp        (501) staff       (20)      340 2024-04-23 05:40:03.000000 chargespot-0.0.2/src/chargespot/templates/api/__init__.py
--rw-r--r--   0 lzp        (501) staff       (20)      470 2024-04-19 07:27:07.000000 chargespot-0.0.2/src/chargespot/templates/api/demo.py
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.009853 chargespot-0.0.2/src/chargespot/templates/common/
--rw-r--r--   0 lzp        (501) staff       (20)       92 2024-04-23 05:40:03.000000 chargespot-0.0.2/src/chargespot/templates/common/__init__.py
--rw-r--r--   0 lzp        (501) staff       (20)      198 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/templates/common/assert_tools.py
--rw-r--r--   0 lzp        (501) staff       (20)      228 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/templates/config.yaml
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.010262 chargespot-0.0.2/src/chargespot/templates/db/
--rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/templates/db/__init__.py
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.010532 chargespot-0.0.2/src/chargespot/templates/report/
--rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/templates/report/.gitkeep
--rw-r--r--   0 lzp        (501) staff       (20)       29 2024-04-19 07:27:07.000000 chargespot-0.0.2/src/chargespot/templates/requirements.txt
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.011327 chargespot-0.0.2/src/chargespot/templates/test_suites/
--rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/templates/test_suites/__init__.py
--rw-r--r--   0 lzp        (501) staff       (20)      446 2024-04-19 07:27:07.000000 chargespot-0.0.2/src/chargespot/templates/test_suites/test_book_list.py
--rw-r--r--   0 lzp        (501) staff       (20)      725 2024-04-19 07:27:07.000000 chargespot-0.0.2/src/chargespot/templates/test_suites/test_login.py
--rw-r--r--   0 lzp        (501) staff       (20)     3331 2024-03-25 06:10:08.000000 chargespot-0.0.2/src/chargespot/utils.py
-drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 06:28:15.005711 chargespot-0.0.2/src/chargespot.egg-info/
--rw-r--r--   0 lzp        (501) staff       (20)      394 2024-04-23 06:28:14.000000 chargespot-0.0.2/src/chargespot.egg-info/PKG-INFO
--rw-r--r--   0 lzp        (501) staff       (20)     1180 2024-04-23 06:28:14.000000 chargespot-0.0.2/src/chargespot.egg-info/SOURCES.txt
--rw-r--r--   0 lzp        (501) staff       (20)        1 2024-04-23 06:28:14.000000 chargespot-0.0.2/src/chargespot.egg-info/dependency_links.txt
--rw-r--r--   0 lzp        (501) staff       (20)       61 2024-04-23 06:28:14.000000 chargespot-0.0.2/src/chargespot.egg-info/entry_points.txt
--rw-r--r--   0 lzp        (501) staff       (20)       58 2024-04-23 06:28:14.000000 chargespot-0.0.2/src/chargespot.egg-info/requires.txt
--rw-r--r--   0 lzp        (501) staff       (20)       11 2024-04-23 06:28:14.000000 chargespot-0.0.2/src/chargespot.egg-info/top_level.txt
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.793447 chargespot-0.0.3/
+-rw-r--r--   0 lzp        (501) staff       (20)    11357 2024-03-25 06:10:08.000000 chargespot-0.0.3/LICENSE
+-rw-r--r--   0 lzp        (501) staff       (20)       74 2024-04-23 04:16:18.000000 chargespot-0.0.3/MANIFEST.in
+-rw-r--r--   0 lzp        (501) staff       (20)      394 2024-04-23 08:59:40.792932 chargespot-0.0.3/PKG-INFO
+-rw-r--r--   0 lzp        (501) staff       (20)    21601 2024-04-19 07:27:07.000000 chargespot-0.0.3/README.md
+-rw-r--r--   0 lzp        (501) staff       (20)       38 2024-04-23 08:59:40.793527 chargespot-0.0.3/setup.cfg
+-rw-r--r--   0 lzp        (501) staff       (20)      615 2024-04-23 08:58:19.000000 chargespot-0.0.3/setup.py
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.776159 chargespot-0.0.3/src/
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.784327 chargespot-0.0.3/src/chargespot/
+-rw-r--r--   0 lzp        (501) staff       (20)      383 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/__init__.py
+-rw-r--r--   0 lzp        (501) staff       (20)    12118 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/api_decorator.py
+-rw-r--r--   0 lzp        (501) staff       (20)     2448 2024-04-23 08:59:28.000000 chargespot-0.0.3/src/chargespot/cli.py
+-rw-r--r--   0 lzp        (501) staff       (20)     5415 2024-04-19 07:27:07.000000 chargespot-0.0.3/src/chargespot/config_manager.py
+-rw-r--r--   0 lzp        (501) staff       (20)     7887 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/email_report_template.html
+-rw-r--r--   0 lzp        (501) staff       (20)      110 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/exceptions.py
+-rw-r--r--   0 lzp        (501) staff       (20)      130 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/execute.py
+-rw-r--r--   0 lzp        (501) staff       (20)    10691 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/heman_datetime.py
+-rw-r--r--   0 lzp        (501) staff       (20)     9624 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/report.py
+-rw-r--r--   0 lzp        (501) staff       (20)     4966 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/swagger.py
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.788305 chargespot-0.0.3/src/chargespot/templates/
+-rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/templates/.chargespot
+-rw-r--r--   0 lzp        (501) staff       (20)     1063 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/templates/.gitignore
+-rw-r--r--   0 lzp        (501) staff       (20)     2346 2024-04-19 07:27:07.000000 chargespot-0.0.3/src/chargespot/templates/README.md
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.789462 chargespot-0.0.3/src/chargespot/templates/api/
+-rw-r--r--   0 lzp        (501) staff       (20)      340 2024-04-23 05:40:03.000000 chargespot-0.0.3/src/chargespot/templates/api/__init__.py
+-rw-r--r--   0 lzp        (501) staff       (20)      470 2024-04-19 07:27:07.000000 chargespot-0.0.3/src/chargespot/templates/api/demo.py
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.790743 chargespot-0.0.3/src/chargespot/templates/common/
+-rw-r--r--   0 lzp        (501) staff       (20)       92 2024-04-23 05:40:03.000000 chargespot-0.0.3/src/chargespot/templates/common/__init__.py
+-rw-r--r--   0 lzp        (501) staff       (20)      198 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/templates/common/assert_tools.py
+-rw-r--r--   0 lzp        (501) staff       (20)      228 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/templates/config.yaml
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.791242 chargespot-0.0.3/src/chargespot/templates/db/
+-rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/templates/db/__init__.py
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.791498 chargespot-0.0.3/src/chargespot/templates/report/
+-rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/templates/report/.gitkeep
+-rw-r--r--   0 lzp        (501) staff       (20)       29 2024-04-19 07:27:07.000000 chargespot-0.0.3/src/chargespot/templates/requirements.txt
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.792284 chargespot-0.0.3/src/chargespot/templates/test_suites/
+-rw-r--r--   0 lzp        (501) staff       (20)        0 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/templates/test_suites/__init__.py
+-rw-r--r--   0 lzp        (501) staff       (20)      446 2024-04-19 07:27:07.000000 chargespot-0.0.3/src/chargespot/templates/test_suites/test_book_list.py
+-rw-r--r--   0 lzp        (501) staff       (20)      725 2024-04-19 07:27:07.000000 chargespot-0.0.3/src/chargespot/templates/test_suites/test_login.py
+-rw-r--r--   0 lzp        (501) staff       (20)     3331 2024-03-25 06:10:08.000000 chargespot-0.0.3/src/chargespot/utils.py
+drwxr-xr-x   0 lzp        (501) staff       (20)        0 2024-04-23 08:59:40.786318 chargespot-0.0.3/src/chargespot.egg-info/
+-rw-r--r--   0 lzp        (501) staff       (20)      394 2024-04-23 08:59:40.000000 chargespot-0.0.3/src/chargespot.egg-info/PKG-INFO
+-rw-r--r--   0 lzp        (501) staff       (20)     1180 2024-04-23 08:59:40.000000 chargespot-0.0.3/src/chargespot.egg-info/SOURCES.txt
+-rw-r--r--   0 lzp        (501) staff       (20)        1 2024-04-23 08:59:40.000000 chargespot-0.0.3/src/chargespot.egg-info/dependency_links.txt
+-rw-r--r--   0 lzp        (501) staff       (20)       61 2024-04-23 08:59:40.000000 chargespot-0.0.3/src/chargespot.egg-info/entry_points.txt
+-rw-r--r--   0 lzp        (501) staff       (20)       58 2024-04-23 08:59:40.000000 chargespot-0.0.3/src/chargespot.egg-info/requires.txt
+-rw-r--r--   0 lzp        (501) staff       (20)       11 2024-04-23 08:59:40.000000 chargespot-0.0.3/src/chargespot.egg-info/top_level.txt
```

### Comparing `chargespot-0.0.2/LICENSE` & `chargespot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/README.md` & `chargespot-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/setup.py` & `chargespot-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chargespot",
-    version="0.0.2",
+    version="0.0.3",
     keywords=("api test", "automation", "testing", "chargespot"),
     description="api test tools",
     long_description="simplify api testing",
     url="",
     author="chargespot",
     author_email="",
     packages=find_packages('src'),
```

### Comparing `chargespot-0.0.2/src/chargespot/api_decorator.py` & `chargespot-0.0.3/src/chargespot/api_decorator.py`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/cli.py` & `chargespot-0.0.3/src/chargespot/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
         os.mkdir(project_name)
     except OSError as e:
         echo(style("创建 %s 失败, %s" % (project_name, str(e)), fg='red'))
         sys.exit(1)
 
 
 def get_project_path(project_name):
-    return os.path.join(os.getcwd(), project_name)
+    return os.path.join(os.getcwd())
 
 
 def generate_project(project_name):
     echo(style('开始创建%s项目' % project_name, fg='red'))
-    mkdir_project(project_name)
+    # mkdir_project(project_name)
     project_path = get_project_path(project_name)
     templates_file_list = os.listdir(TEMPLATES_DIR)
 
     echo(style('开始渲染...', fg='green'))
     for f in templates_file_list:
         try:
             src = os.path.join(TEMPLATES_DIR, f)
```

### Comparing `chargespot-0.0.2/src/chargespot/config_manager.py` & `chargespot-0.0.3/src/chargespot/config_manager.py`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/email_report_template.html` & `chargespot-0.0.3/src/chargespot/email_report_template.html`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/heman_datetime.py` & `chargespot-0.0.3/src/chargespot/heman_datetime.py`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/report.py` & `chargespot-0.0.3/src/chargespot/report.py`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/swagger.py` & `chargespot-0.0.3/src/chargespot/swagger.py`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/templates/.gitignore` & `chargespot-0.0.3/src/chargespot/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/templates/README.md` & `chargespot-0.0.3/src/chargespot/templates/README.md`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/templates/test_suites/test_login.py` & `chargespot-0.0.3/src/chargespot/templates/test_suites/test_login.py`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot/utils.py` & `chargespot-0.0.3/src/chargespot/utils.py`

 * *Files identical despite different names*

### Comparing `chargespot-0.0.2/src/chargespot.egg-info/SOURCES.txt` & `chargespot-0.0.3/src/chargespot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

