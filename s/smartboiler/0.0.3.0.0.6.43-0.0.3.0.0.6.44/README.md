# Comparing `tmp/smartboiler-0.0.3.0.0.6.43.tar.gz` & `tmp/smartboiler-0.0.3.0.0.6.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartboiler-0.0.3.0.0.6.43.tar", last modified: Mon Apr 22 19:58:49 2024, max compression
+gzip compressed data, was "smartboiler-0.0.3.0.0.6.44.tar", last modified: Mon Apr 22 20:18:47 2024, max compression
```

## Comparing `smartboiler-0.0.3.0.0.6.43.tar` & `smartboiler-0.0.3.0.0.6.44.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:49.614137 smartboiler-0.0.3.0.0.6.43/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-22 19:58:49.614137 smartboiler-0.0.3.0.0.6.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:58:49.614137 smartboiler-0.0.3.0.0.6.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-22 19:58:48.000000 smartboiler-0.0.3.0.0.6.43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:49.610137 smartboiler-0.0.3.0.0.6.43/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:49.614137 smartboiler-0.0.3.0.0.6.43/src/smartboiler/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/boiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/event_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/fotovoltaics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/time_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-22 19:58:46.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler/week_planner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:58:49.614137 smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-22 19:58:49.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-22 19:58:49.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:58:49.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 19:58:49.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 19:58:49.000000 smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:18:47.737041 smartboiler-0.0.3.0.0.6.44/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-22 20:18:47.737041 smartboiler-0.0.3.0.0.6.44/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 20:18:47.737041 smartboiler-0.0.3.0.0.6.44/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-22 20:18:46.000000 smartboiler-0.0.3.0.0.6.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:18:47.733041 smartboiler-0.0.3.0.0.6.44/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:18:47.733041 smartboiler-0.0.3.0.0.6.44/src/smartboiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/event_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/fotovoltaics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17340 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/retrieve_hass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/time_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14501 2024-04-22 20:18:42.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler/week_planner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 20:18:47.737041 smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-22 20:18:47.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-22 20:18:47.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 20:18:47.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 20:18:47.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 20:18:47.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 20:18:47.000000 smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/top_level.txt
```

### Comparing `smartboiler-0.0.3.0.0.6.43/PKG-INFO` & `smartboiler-0.0.3.0.0.6.44/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: smartboiler
-Version: 0.0.3.0.0.6.43
-Summary: Smart boiling of household
-Home-page: https://github.com/grinwi/smartboiler
-Author: Adam GRUNWALD
-Author-email: grunwald.adam24@gmail.com
-Keywords: energy,management,optimization,hass
-Requires-Python: >=3.6, <=3.7
-Description-Content-Type: text/markdown
-
 # SMART BOILER
 From dumb boiler smart with help of smart plug. 
 
 Recursive link to the github repository: <https://github.com/grinwi/smart_boiler>.
 
 
 ## What's it all about?
```

### Comparing `smartboiler-0.0.3.0.0.6.43/README.md` & `smartboiler-0.0.3.0.0.6.44/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: smartboiler
+Version: 0.0.3.0.0.6.44
+Summary: Smart boiling of household
+Home-page: https://github.com/grinwi/smartboiler
+Author: Adam GRUNWALD
+Author-email: grunwald.adam24@gmail.com
+Keywords: energy,management,optimization,hass
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9, <=3.10
+Description-Content-Type: text/markdown
+
 # SMART BOILER
 From dumb boiler smart with help of smart plug. 
 
 Recursive link to the github repository: <https://github.com/grinwi/smart_boiler>.
 
 
 ## What's it all about?
```

### Comparing `smartboiler-0.0.3.0.0.6.43/setup.py` & `smartboiler-0.0.3.0.0.6.44/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,50 +15,50 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='smartboiler',  # Required
-    version='0.0.3.0.0.6.43',  # Required
+    version='0.0.3.0.0.6.44',  # Required
     description='Smart boiling of household',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/grinwi/smartboiler',  # Optional
     author='Adam GRUNWALD',  # Optional
     author_email='grunwald.adam24@gmail.com',  # Optional
     classifiers=[  # Optional
-        # 'Development Status :: 5 - Production/Stable',
-        # 'Intended Audience :: Developers',
-        # 'Topic :: Software Development :: Build Tools',
-        # 'License :: OSI Approved :: MIT License',
-        # 'Programming Language :: Python :: 3.10',
-        # "Operating System :: OS Independent",
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.10',
+        "Operating System :: OS Independent",
     ],
     keywords='energy, management, optimization, hass',  # Optional
     package_dir={'': 'src'},  # Optional
     packages=find_packages(where='src'),  # Required
-    python_requires='>=3.6, <=3.7',
+    python_requires='>=3.9, <=3.10',
     install_requires=[
-        # 'wheel', 
-        # 'numpy>=1.22.2',
-        # 'scipy<1.9.0',
-        # 'pandas>=1.4.1',
-        # 'pvlib>=0.10.1',
-        # 'protobuf>=3.0.0',
-        # 'pytz>=2021.1',
-        # 'requests>=2.25.1',
-        # 'beautifulsoup4>=4.9.3',
-        # 'pulp>=2.4',
-        # 'pyyaml>=5.4.1',
-        # 'tables==3.7.0',
-        # 'skforecast==0.10.1',
-        # 'influxdb==5.3.1',
-        # 'matplotlib==3.5.1',
-        # 'flask>=2.0.2',
+        'wheel', 
+        'numpy>=1.22.2',
+        'scipy<1.9.0',
+        'pandas>=1.4.1',
+        'pvlib>=0.10.1',
+        'protobuf>=3.0.0',
+        'pytz>=2021.1',
+        'requests>=2.25.1',
+        'beautifulsoup4>=4.9.3',
+        'pulp>=2.4',
+        'pyyaml>=5.4.1',
+        'tables==3.7.0',
+        'skforecast==0.10.1',
+        'influxdb==5.3.1',
+        'matplotlib==3.5.1',
+        'flask>=2.0.2',
         
     ],  
     # Optional
     entry_points={  # Optional
         'console_scripts': [
             'smartboiler=smartboiler.command_line:main',
         ],
```

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/boiler.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/boiler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/controller.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/controller.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/data_handler.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/data_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/event_checker.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/event_checker.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/forecast.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/forecast.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/fotovoltaics.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/fotovoltaics.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/main.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/main.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/retrieve_hass.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/switch.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/switch.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/time_handler.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/time_handler.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler/week_planner.py` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler/week_planner.py`

 * *Files identical despite different names*

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/PKG-INFO` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: smartboiler
-Version: 0.0.3.0.0.6.43
+Version: 0.0.3.0.0.6.44
 Summary: Smart boiling of household
 Home-page: https://github.com/grinwi/smartboiler
 Author: Adam GRUNWALD
 Author-email: grunwald.adam24@gmail.com
 Keywords: energy,management,optimization,hass
-Requires-Python: >=3.6, <=3.7
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9, <=3.10
 Description-Content-Type: text/markdown
 
 # SMART BOILER
 From dumb boiler smart with help of smart plug. 
 
 Recursive link to the github repository: <https://github.com/grinwi/smart_boiler>.
```

### Comparing `smartboiler-0.0.3.0.0.6.43/src/smartboiler.egg-info/SOURCES.txt` & `smartboiler-0.0.3.0.0.6.44/src/smartboiler.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 src/smartboiler/switch.py
 src/smartboiler/time_handler.py
 src/smartboiler/week_planner.py
 src/smartboiler.egg-info/PKG-INFO
 src/smartboiler.egg-info/SOURCES.txt
 src/smartboiler.egg-info/dependency_links.txt
 src/smartboiler.egg-info/entry_points.txt
+src/smartboiler.egg-info/requires.txt
 src/smartboiler.egg-info/top_level.txt
```

