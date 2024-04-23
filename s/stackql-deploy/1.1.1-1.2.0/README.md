# Comparing `tmp/stackql_deploy-1.1.1.tar.gz` & `tmp/stackql_deploy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.1.1.tar", last modified: Mon Apr 22 07:21:43 2024, max compression
+gzip compressed data, was "stackql_deploy-1.2.0.tar", last modified: Tue Apr 23 07:47:22 2024, max compression
```

## Comparing `stackql_deploy-1.1.1.tar` & `stackql_deploy-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:43.820931 stackql_deploy-1.1.1/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.1.1/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)    10269 2024-04-22 07:21:43.786317 stackql_deploy-1.1.1/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8359 2024-04-17 09:11:17.000000 stackql_deploy-1.1.1/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-22 07:21:43.824592 stackql_deploy-1.1.1/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1657 2024-04-22 07:19:58.000000 stackql_deploy-1.1.1/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:41.627111 stackql_deploy-1.1.1/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-22 07:19:58.000000 stackql_deploy-1.1.1/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     9131 2024-04-22 04:56:05.000000 stackql_deploy-1.1.1/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:42.587804 stackql_deploy-1.1.1/stackql_deploy/cmd/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.1.1/stackql_deploy/cmd/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6751 2024-04-22 02:45:23.000000 stackql_deploy-1.1.1/stackql_deploy/cmd/build.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.1.1/stackql_deploy/cmd/teardown.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.1.1/stackql_deploy/cmd/test.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:43.098744 stackql_deploy-1.1.1/stackql_deploy/lib/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.1.1/stackql_deploy/lib/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)      192 2024-04-20 03:11:50.000000 stackql_deploy-1.1.1/stackql_deploy/lib/bootstrap.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     4063 2024-04-22 04:56:39.000000 stackql_deploy-1.1.1/stackql_deploy/lib/config.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2821 2024-04-22 04:56:39.000000 stackql_deploy-1.1.1/stackql_deploy/lib/templating.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6011 2024-04-22 05:06:47.000000 stackql_deploy-1.1.1/stackql_deploy/lib/utils.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:43.216228 stackql_deploy-1.1.1/stackql_deploy/templates/
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:43.355217 stackql_deploy-1.1.1/stackql_deploy/templates/stackql_docs/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       62 2024-04-17 05:34:52.000000 stackql_deploy-1.1.1/stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
--rwxrwxrwx   0 javen     (1000) javen     (1000)      712 2024-04-17 05:34:52.000000 stackql_deploy-1.1.1/stackql_deploy/templates/stackql_manifest.yml.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:43.499066 stackql_deploy-1.1.1/stackql_deploy/templates/stackql_resources/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      892 2024-04-17 05:34:52.000000 stackql_deploy-1.1.1/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:43.627982 stackql_deploy-1.1.1/stackql_deploy/templates/stackql_tests/
--rwxrwxrwx   0 javen     (1000) javen     (1000)      726 2024-04-17 05:34:52.000000 stackql_deploy-1.1.1/stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-22 07:21:43.744562 stackql_deploy-1.1.1/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)    10269 2024-04-22 07:21:39.000000 stackql_deploy-1.1.1/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      846 2024-04-22 07:21:41.000000 stackql_deploy-1.1.1/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-22 07:21:39.000000 stackql_deploy-1.1.1/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-22 07:21:39.000000 stackql_deploy-1.1.1/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       44 2024-04-22 07:21:39.000000 stackql_deploy-1.1.1/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-22 07:21:39.000000 stackql_deploy-1.1.1/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.805036 stackql_deploy-1.2.0/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.2.0/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     9078 2024-04-23 07:47:22.769729 stackql_deploy-1.2.0/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8359 2024-04-17 09:11:17.000000 stackql_deploy-1.2.0/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-23 07:47:22.808034 stackql_deploy-1.2.0/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1703 2024-04-23 07:44:56.000000 stackql_deploy-1.2.0/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:12.492136 stackql_deploy-1.2.0/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-23 07:44:56.000000 stackql_deploy-1.2.0/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     9131 2024-04-23 00:07:37.000000 stackql_deploy-1.2.0/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:18.892313 stackql_deploy-1.2.0/stackql_deploy/cmd/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8160 2024-04-23 00:59:43.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/build.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/teardown.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.2.0/stackql_deploy/cmd/test.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.085803 stackql_deploy-1.2.0/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.2.0/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      192 2024-04-20 03:11:50.000000 stackql_deploy-1.2.0/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     4061 2024-04-22 20:59:53.000000 stackql_deploy-1.2.0/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3985 2024-04-22 21:39:51.000000 stackql_deploy-1.2.0/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6689 2024-04-23 05:16:36.000000 stackql_deploy-1.2.0/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.188839 stackql_deploy-1.2.0/stackql_deploy/templates/
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.338029 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_docs/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       62 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_docs/stackql_example_rg.md.template
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      712 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_manifest.yml.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.470565 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_resources/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      892 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.617423 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_tests/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      726 2024-04-17 05:34:52.000000 stackql_deploy-1.2.0/stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-23 07:47:22.731727 stackql_deploy-1.2.0/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     9078 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      846 2024-04-23 07:47:11.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       44 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-23 07:47:04.000000 stackql_deploy-1.2.0/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.1.1/LICENSE` & `stackql_deploy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/PKG-INFO` & `stackql_deploy-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,26 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.1.1
+Version: 1.2.0
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
-License: MIT License
-        
-        Copyright (c) 2022 StackQL Studios
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: jinja2
 Requires-Dist: pystackql>=3.6.1
 
 .. image:: https://stackql.io/img/stackql-logo-bold.png
```

### Comparing `stackql_deploy-1.1.1/README.rst` & `stackql_deploy-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/setup.py` & `stackql_deploy-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
-with open('LICENSE', encoding='utf-8') as f:
-    license_text = f.read()
+# with open('LICENSE', encoding='utf-8') as f:
+#     license_text = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.1.1',
+    version='1.2.0',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
+    long_description_content_type='text/x-rst',
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
-    license=license_text,
+    license='MIT',
     packages=find_packages(),
     package_data={
         'stackql_deploy': [
             'templates/*.template',
             'templates/stackql_docs/*.template',
             'templates/stackql_resources/*.template',
             'templates/stackql_tests/*.template',
```

### Comparing `stackql_deploy-1.1.1/stackql_deploy/cli.py` & `stackql_deploy-1.2.0/stackql_deploy/cli.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/stackql_deploy/cmd/build.py` & `stackql_deploy-1.2.0/stackql_deploy/cmd/build.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from ..lib.utils import run_test, perform_retries, run_stackql_command, catch_error_and_exit
+from ..lib.utils import run_test, perform_retries, run_stackql_command, catch_error_and_exit, run_stackql_query
 from ..lib.config import setup_environment, load_manifest, get_global_context_and_providers, get_full_context
 from ..lib.templating import get_queries
 
 class StackQLProvisioner:
     
     def __init__(self, stackql, vars, logger, stack_dir, stack_env):
         self.stackql = stackql
@@ -49,26 +49,33 @@
                 createorupdate_query = resource_queries['createorupdate']
 
             if 'update' in resource_queries:
                 update_query = resource_queries['update']
 
             preflight_query = None
             postdeploy_query = None
+            exports_query = None
 
             if test_queries == {}:
                 self.logger.info(f"test query file not found for {resource['name']}. Skipping tests.")
                 continue
             else:
                 if 'preflight' in test_queries:
                     preflight_query = test_queries['preflight']
                 
                 if 'postdeploy' in test_queries:
                     postdeploy_query = test_queries['postdeploy']
                     postdeploy_retries = test_query_options.get('postdeploy', {}).get('retries', 10)
-                    postdeploy_retry_delay = test_query_options.get('postdeploy', {}).get('retry_delay', 10)                    
+                    postdeploy_retry_delay = test_query_options.get('postdeploy', {}).get('retry_delay', 10)  
+
+                if 'exports' in test_queries:
+                    # export variables from resource
+                    exports_query = test_queries['exports']
+                    exports_retries = test_query_options.get('exports', {}).get('retries', 10)
+                    exports_retry_delay = test_query_options.get('exports', {}).get('retry_delay', 10)
 
             #
             # run pre flight check
             #
             resource_exists = False
             if not preflight_query:
                 self.logger.info(f"pre-flight check not configured for [{resource['name']}]")
@@ -124,9 +131,27 @@
                 
             #
             # postdeploy check complete
             #
             if not post_deploy_check_passed:
                 catch_error_and_exit(f"deployment failed for {resource['name']} after post-deploy checks.", self.logger)
 
+            #
+            # exports
+            #
+            if exports_query:
+                if not dry_run:
+                    self.logger.info(f"exporting variables for [{resource['name']}]...")
+                    exports = run_stackql_query(exports_query, self.stackql, True, self.logger, exports_retries, exports_retry_delay)
+                    self.logger.debug(f"exports: {exports}")
+                    if exports:
+                        export = exports[0]
+                        for key, value in export.items():
+                            self.logger.debug(f"set [{key}] to [{value}] in exports")
+                            self.global_context[key] = value  # Update global context with exported values
+                    else:
+                        catch_error_and_exit(f"export variables failed for {resource['name']}.", self.logger)
+                else:
+                    self.logger.info(f"dry run exports query for [{resource['name']}]:\n\n{exports_query}\n")
+
             if not dry_run:
                 self.logger.info(f"successfully deployed {resource['name']}")
```

### Comparing `stackql_deploy-1.1.1/stackql_deploy/cmd/teardown.py` & `stackql_deploy-1.2.0/stackql_deploy/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/stackql_deploy/cmd/test.py` & `stackql_deploy-1.2.0/stackql_deploy/cmd/test.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/stackql_deploy/lib/config.py` & `stackql_deploy-1.2.0/stackql_deploy/lib/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os, yaml, json
 from .utils import pull_providers, catch_error_and_exit
 from jinja2 import Environment, FileSystemLoader, select_autoescape
 from jinja2.utils import markupsafe
 
-
 def render_globals(env, vars, global_vars, stack_env):
     # Render globals with vars and include the stack_env as a special variable
     global_context = {'stack_env': stack_env}
     # Render each global variable defined in the manifest
     for global_var in global_vars:
         # Assume each global_var is a dictionary with 'name' and 'value' keys
         template = env.from_string(global_var['value'])
```

### Comparing `stackql_deploy-1.1.1/stackql_deploy/lib/templating.py` & `stackql_deploy-1.2.0/stackql_deploy/lib/templating.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,53 @@
+import json
 import os
 from .utils import catch_error_and_exit
+from jinja2 import TemplateError
+from jinja2.utils import markupsafe
 
 def parse_anchor(anchor):
     """Parse anchor to extract key and options."""
     parts = anchor.split(',')
     key = parts[0].strip()
     options = {}
     for part in parts[1:]:
         if '=' in part:
             option_key, option_value = part.split('=')
             options[option_key.strip()] = int(option_value.strip())
     return key, options
 
+def is_json(myjson):
+    try:
+        json_object = json.loads(myjson)
+    except (ValueError, TypeError):
+        return False
+    return True
+
 def render_queries(env, queries, context):
-    """Render queries with context using Jinja2."""
     rendered_queries = {}
     for key, query in queries.items():
-        template = env.from_string(query)
-        rendered_queries[key] = template.render(context)
+        try:
+            # Clone the context to avoid modifying the original context outside this function
+            temp_context = context.copy()
+            
+            # Check and render JSON structures in the context
+            for ctx_key, ctx_value in temp_context.items():
+                if isinstance(ctx_value, str) and is_json(ctx_value):
+                    # Process JSON string
+                    properties = json.loads(ctx_value)
+                    properties_rendered = env.from_string(json.dumps(properties)).render(temp_context)
+                    temp_context[ctx_key] = markupsafe.Markup(json.dumps(json.loads(properties_rendered), separators=(',', ':')))
+            # Render the query using the updated context
+            template = env.from_string(query)
+            rendered_queries[key] = template.render(temp_context)
+        except TemplateError as e:
+            raise RuntimeError(f"Error rendering query '{key}': {e}") from e
+        except json.JSONDecodeError as e:
+            continue  # If it's not JSON, just skip it
+
     return rendered_queries
 
 def load_sql_queries(file_path):
     """Loads SQL queries from a file, splits them by anchors, and extracts options."""
     queries = {}
     options = {}
     current_anchor = None
```

### Comparing `stackql_deploy-1.1.1/stackql_deploy/lib/utils.py` & `stackql_deploy-1.2.0/stackql_deploy/lib/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,58 @@
 import time, json, sys
 
 def catch_error_and_exit(errmsg, logger):
 	logger.error(errmsg)
 	sys.exit(errmsg)
 
-def run_stackql_query(query, stackql, suppress_errors, logger):
-    try:
-        logger.debug(f"executing stackql query: {query}")
-        result = stackql.execute(query, suppress_errors)
-        logger.debug(f"stackql query result: {result}, type: {type(result)}")
-
-        # result should be...
-        # [{'error': <error json str>}] if something went wrong; or
-        # [{<row1>},...] if the statement was executed successfully, messages to stderr are ignored; or
-        # [] if the statement was executed successfully, but no rows were returned
-
-        # result should be a list
-        if isinstance(result, list):
-            # if suppress_errors is False, we will detect errors where we werent expecting them...
-            if not suppress_errors:
-                # check if the result contains an error message
-                if len(result) > 0 and 'error' in result[0]:
-                    error_message = result[0]['error']
-                    catch_error_and_exit(f"error occurred during stackql query execution: {error_message}", logger)
 
-            logger.debug(f"stackql query executed successfully, retrieved {len(result)} items.")
-            return result
-       
-        # If result is not a list, it's an unexpected result format
-        catch_error_and_exit("unexpected result format received from stackql query execution.", logger)
-    
-    except Exception as e:
-        # Log the exception and exit
-        catch_error_and_exit(f"an exception occurred during stackql query execution: {str(e)}", logger)
+def run_stackql_query(query, stackql, suppress_errors, logger, retries=0, delay=5):
+    attempt = 0
+    while attempt <= retries:
+        try:
+            logger.debug(f"Executing stackql query on attempt {attempt + 1}: {query}")
+            result = stackql.execute(query, suppress_errors)
+            logger.debug(f"StackQL query result: {result}, type: {type(result)}")
+
+            # Check if result is a list (expected outcome)
+            if isinstance(result, list):
+                if not suppress_errors and result and 'error' in result[0]:
+                    error_message = result[0]['error']
+                    if attempt == retries:
+                        # If retries are exhausted, log the error and exit
+                        catch_error_and_exit(f"Error occurred during stackql query execution: {error_message}", logger)
+                    else:
+                        # Log the error and prepare for another attempt
+                        logger.error(f"Attempt {attempt + 1} failed: {error_message}")
+                else:
+                    # If no errors or errors are suppressed, return the result
+                    logger.debug(f"StackQL query executed successfully, retrieved {len(result)} items.")
+                    return result
+
+            else:
+                # Handle unexpected result format
+                if attempt == retries:
+                    catch_error_and_exit("Unexpected result format received from stackql query execution.", logger)
+                else:
+                    logger.error("Unexpected result format, retrying...")
+
+        except Exception as e:
+            # Log the exception and check if retry attempts are exhausted
+            if attempt == retries:
+                catch_error_and_exit(f"An exception occurred during stackql query execution: {str(e)}", logger)
+            else:
+                logger.error(f"Exception on attempt {attempt + 1}: {str(e)}")
+
+        # Delay before next attempt
+        time.sleep(delay)
+        attempt += 1
+
+    # If all attempts fail and no result is returned, log the final failure
+    logger.error(f"All attempts ({retries + 1}) to execute the query failed.")
+    return None
 
 def run_stackql_command(command, stackql, logger):
     try:
         logger.debug(f"executing stackql command: {command}")
         result = stackql.executeStmt(command)
         logger.debug(f"stackql command result: {result}, type: {type(result)}")
```

### Comparing `stackql_deploy-1.1.1/stackql_deploy/templates/stackql_manifest.yml.template` & `stackql_deploy-1.2.0/stackql_deploy/templates/stackql_manifest.yml.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template` & `stackql_deploy-1.2.0/stackql_deploy/templates/stackql_resources/stackql_example_rg.iql.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template` & `stackql_deploy-1.2.0/stackql_deploy/templates/stackql_tests/stackql_example_rg.iql.template`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.1.1/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.2.0/stackql_deploy.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,26 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.1.1
+Version: 1.2.0
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
-License: MIT License
-        
-        Copyright (c) 2022 StackQL Studios
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: click
 Requires-Dist: python-dotenv
 Requires-Dist: jinja2
 Requires-Dist: pystackql>=3.6.1
 
 .. image:: https://stackql.io/img/stackql-logo-bold.png
```

### Comparing `stackql_deploy-1.1.1/stackql_deploy.egg-info/SOURCES.txt` & `stackql_deploy-1.2.0/stackql_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

