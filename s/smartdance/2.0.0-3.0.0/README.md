# Comparing `tmp/smartdance-2.0.0.tar.gz` & `tmp/smartdance-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdance-2.0.0.tar", last modified: Mon Oct 16 15:26:19 2023, max compression
+gzip compressed data, was "smartdance-3.0.0.tar", last modified: Fri Apr 19 16:41:45 2024, max compression
```

## Comparing `smartdance-2.0.0.tar` & `smartdance-3.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 marcelo    (501) staff       (20)        0 2023-10-16 15:26:19.518697 smartdance-2.0.0/
--rw-r--r--   0 marcelo    (501) staff       (20)     1977 2023-10-16 15:26:19.518539 smartdance-2.0.0/PKG-INFO
--rw-r--r--   0 marcelo    (501) staff       (20)     1342 2023-10-16 13:14:17.000000 smartdance-2.0.0/README.md
--rw-r--r--   0 marcelo    (501) staff       (20)       38 2023-10-16 15:26:19.518761 smartdance-2.0.0/setup.cfg
--rw-r--r--   0 marcelo    (501) staff       (20)      866 2023-10-16 15:25:24.000000 smartdance-2.0.0/setup.py
-drwxr-xr-x   0 marcelo    (501) staff       (20)        0 2023-10-16 15:26:19.517649 smartdance-2.0.0/smartdance/
--rw-r--r--   0 marcelo    (501) staff       (20)       30 2023-09-19 23:47:37.000000 smartdance-2.0.0/smartdance/__init__.py
--rw-r--r--   0 marcelo    (501) staff       (20)        0 2023-09-19 23:38:47.000000 smartdance-2.0.0/smartdance/exceptions.py
--rw-r--r--   0 marcelo    (501) staff       (20)     1639 2023-10-16 15:25:15.000000 smartdance-2.0.0/smartdance/smartdance.py
--rw-r--r--   0 marcelo    (501) staff       (20)        0 2023-09-19 23:38:44.000000 smartdance-2.0.0/smartdance/utils.py
-drwxr-xr-x   0 marcelo    (501) staff       (20)        0 2023-10-16 15:26:19.518308 smartdance-2.0.0/smartdance.egg-info/
--rw-r--r--   0 marcelo    (501) staff       (20)     1977 2023-10-16 15:26:19.000000 smartdance-2.0.0/smartdance.egg-info/PKG-INFO
--rw-r--r--   0 marcelo    (501) staff       (20)      247 2023-10-16 15:26:19.000000 smartdance-2.0.0/smartdance.egg-info/SOURCES.txt
--rw-r--r--   0 marcelo    (501) staff       (20)        1 2023-10-16 15:26:19.000000 smartdance-2.0.0/smartdance.egg-info/dependency_links.txt
--rw-r--r--   0 marcelo    (501) staff       (20)       11 2023-10-16 15:26:19.000000 smartdance-2.0.0/smartdance.egg-info/top_level.txt
+drwxr-xr-x   0 marcelo    (501) staff       (20)        0 2024-04-19 16:41:45.894014 smartdance-3.0.0/
+-rw-r--r--   0 marcelo    (501) staff       (20)     2303 2024-04-19 16:41:45.893850 smartdance-3.0.0/PKG-INFO
+-rw-r--r--   0 marcelo    (501) staff       (20)     1668 2024-04-19 16:41:24.000000 smartdance-3.0.0/README.md
+-rw-r--r--   0 marcelo    (501) staff       (20)       38 2024-04-19 16:41:45.894086 smartdance-3.0.0/setup.cfg
+-rw-r--r--   0 marcelo    (501) staff       (20)      866 2024-04-19 16:41:05.000000 smartdance-3.0.0/setup.py
+drwxr-xr-x   0 marcelo    (501) staff       (20)        0 2024-04-19 16:41:45.892836 smartdance-3.0.0/smartdance/
+-rw-r--r--   0 marcelo    (501) staff       (20)       30 2024-04-19 16:16:34.000000 smartdance-3.0.0/smartdance/__init__.py
+-rw-r--r--   0 marcelo    (501) staff       (20)        0 2024-04-19 16:16:34.000000 smartdance-3.0.0/smartdance/exceptions.py
+-rw-r--r--   0 marcelo    (501) staff       (20)     1687 2024-04-19 16:33:55.000000 smartdance-3.0.0/smartdance/smartdance.py
+-rw-r--r--   0 marcelo    (501) staff       (20)        0 2024-04-19 16:16:34.000000 smartdance-3.0.0/smartdance/utils.py
+drwxr-xr-x   0 marcelo    (501) staff       (20)        0 2024-04-19 16:41:45.893606 smartdance-3.0.0/smartdance.egg-info/
+-rw-r--r--   0 marcelo    (501) staff       (20)     2303 2024-04-19 16:41:45.000000 smartdance-3.0.0/smartdance.egg-info/PKG-INFO
+-rw-r--r--   0 marcelo    (501) staff       (20)      247 2024-04-19 16:41:45.000000 smartdance-3.0.0/smartdance.egg-info/SOURCES.txt
+-rw-r--r--   0 marcelo    (501) staff       (20)        1 2024-04-19 16:41:45.000000 smartdance-3.0.0/smartdance.egg-info/dependency_links.txt
+-rw-r--r--   0 marcelo    (501) staff       (20)       11 2024-04-19 16:41:45.000000 smartdance-3.0.0/smartdance.egg-info/top_level.txt
```

### Comparing `smartdance-2.0.0/PKG-INFO` & `smartdance-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdance
-Version: 2.0.0
+Version: 3.0.0
 Summary: A Python package for template string processing designed for prompt engineering
 Home-page: UNKNOWN
 Author: Marcelo Arias
 Author-email: marcelo@smartup.lat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# SmartDance
+SmartDance
 
 SmartDance is a Python package that brings the power of template languages to Python. Inspired by Handlebars and similar languages, SmartDance allows you to embed Python function calls and variables directly into your strings, which are then executed and replaced with their results when the string is processed.
 
 > Designed specifically to work as a Prompt Engineering tool, SmartDance is a simple, flexible, and powerful way to generate strings from Python code.
 
 ## Features
 
@@ -46,13 +46,30 @@
 print(dance("{{hello('World')}}", locals()))
 ```
 
 ```
 Output: Hello, World!
 ```
 
+## How to update the package
+
+1. Update the version in `setup.py`
+2. Run the following command to build the package:
+```
+python setup.py sdist bdist_wheel
+```
+3. Run the following command to upload the package to PyPI:
+```
+twine upload dist/*
+```
+4. Update the package in the project:
+```
+pip install --upgrade smartdance
+```
+
+
 ## Future Plans
 
 - Complex Data Types: We plan to add support for complex data types like lists, dictionaries, and objects in the future.
 - Debugging and Testing: We plan to add built-in functionality for debugging and testing in the future.
```

### Comparing `smartdance-2.0.0/README.md` & `smartdance-3.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SmartDance
+SmartDance
 
 SmartDance is a Python package that brings the power of template languages to Python. Inspired by Handlebars and similar languages, SmartDance allows you to embed Python function calls and variables directly into your strings, which are then executed and replaced with their results when the string is processed.
 
 > Designed specifically to work as a Prompt Engineering tool, SmartDance is a simple, flexible, and powerful way to generate strings from Python code.
 
 ## Features
 
@@ -28,11 +28,28 @@
 print(dance("{{hello('World')}}", locals()))
 ```
 
 ```
 Output: Hello, World!
 ```
 
+## How to update the package
+
+1. Update the version in `setup.py`
+2. Run the following command to build the package:
+```
+python setup.py sdist bdist_wheel
+```
+3. Run the following command to upload the package to PyPI:
+```
+twine upload dist/*
+```
+4. Update the package in the project:
+```
+pip install --upgrade smartdance
+```
+
+
 ## Future Plans
 
 - Complex Data Types: We plan to add support for complex data types like lists, dictionaries, and objects in the future.
 - Debugging and Testing: We plan to add built-in functionality for debugging and testing in the future.
```

### Comparing `smartdance-2.0.0/setup.py` & `smartdance-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='smartdance',
-    version='2.0.0',  # Update this for new versions
+    version='3.0.0',  # Update this for new versions
     description='A Python package for template string processing designed for prompt engineering',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marcelo Arias',
     author_email='marcelo@smartup.lat',
     packages=find_packages(),
     install_requires=[],  # List your package dependencies here
```

### Comparing `smartdance-2.0.0/smartdance/smartdance.py` & `smartdance-3.0.0/smartdance/smartdance.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,42 +4,39 @@
     # Regular expression to find function calls or variables in {{}}
     pattern = r"\{\{(.*?)\}\}"
 
     # Find all matches in the template string
     matches = re.findall(pattern, template_string)
 
     for match in matches:
-        # Check if it's a function call
-        if '(' in match and ')' in match:
-            function_name, parameters = match.split('(')
-            parameters = parameters.rstrip(')')
-
-            # Execute the function with the parameters and get the result
-            try:
+        result = ""  # Initialize result to an empty string for each match
+        try:
+            # Check if it's a function call
+            if '(' in match and ')' in match:
+                function_name, parameters = match.split('(')
+                parameters = parameters.rstrip(')')
+                # Execute the function with the parameters and get the result
                 result = eval(f"{function_name}({parameters})", globals(), local_dict)
-            except Exception as e:
-                return f"The function failed to bring the data: {str(e)}"
-
-        else:
-            # It's a variable
-            variable_name = match
-
-            # Get the value of the variable
-            try:
+            else:
+                # It's a variable
+                variable_name = match
+                # Get the value of the variable
                 if hyperparameters and variable_name in hyperparameters:
                     result = hyperparameters[variable_name]
                 else:
                     result = eval(variable_name, globals(), local_dict)
-            except Exception as e:
-                return f"The variable failed to bring the data: {str(e)}"
+        except Exception as e:
+            # If there's an error, result is already an empty string
+            # Optionally, log the error or handle it as needed
+            pass
 
         # Replace the function call or variable in the template string with the result
         template_string = template_string.replace(f"{{{{{match}}}}}", str(result))
 
     return template_string
 
 
 def name() -> str:
-    return f"Marcelo"
+    return "Marcelo"
 
 if __name__ == "__main__":
     print(dance("My name is {{name()}}, from {{country}}!", locals(), {'country': 'Chile'}))
```

### Comparing `smartdance-2.0.0/smartdance.egg-info/PKG-INFO` & `smartdance-3.0.0/smartdance.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdance
-Version: 2.0.0
+Version: 3.0.0
 Summary: A Python package for template string processing designed for prompt engineering
 Home-page: UNKNOWN
 Author: Marcelo Arias
 Author-email: marcelo@smartup.lat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# SmartDance
+SmartDance
 
 SmartDance is a Python package that brings the power of template languages to Python. Inspired by Handlebars and similar languages, SmartDance allows you to embed Python function calls and variables directly into your strings, which are then executed and replaced with their results when the string is processed.
 
 > Designed specifically to work as a Prompt Engineering tool, SmartDance is a simple, flexible, and powerful way to generate strings from Python code.
 
 ## Features
 
@@ -46,13 +46,30 @@
 print(dance("{{hello('World')}}", locals()))
 ```
 
 ```
 Output: Hello, World!
 ```
 
+## How to update the package
+
+1. Update the version in `setup.py`
+2. Run the following command to build the package:
+```
+python setup.py sdist bdist_wheel
+```
+3. Run the following command to upload the package to PyPI:
+```
+twine upload dist/*
+```
+4. Update the package in the project:
+```
+pip install --upgrade smartdance
+```
+
+
 ## Future Plans
 
 - Complex Data Types: We plan to add support for complex data types like lists, dictionaries, and objects in the future.
 - Debugging and Testing: We plan to add built-in functionality for debugging and testing in the future.
```

