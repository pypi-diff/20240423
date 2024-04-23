# Comparing `tmp/voila-sepal-ui-0.3.0.tar.gz` & `tmp/voila_sepal_ui-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila-sepal-ui-0.3.0.tar", last modified: Tue Apr 23 09:59:14 2024, max compression
+gzip compressed data, was "voila_sepal_ui-0.4.1.tar", last modified: Tue Apr 23 12:17:43 2024, max compression
```

## Comparing `voila-sepal-ui-0.3.0.tar` & `voila_sepal_ui-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.344310 voila-sepal-ui-0.3.0/
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)      268 2024-04-23 09:59:14.340310 voila-sepal-ui-0.3.0/PKG-INFO
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)      523 2024-04-23 08:22:05.000000 voila-sepal-ui-0.3.0/README.rst
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)       38 2024-04-23 09:59:14.344310 voila-sepal-ui-0.3.0/setup.cfg
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     1851 2024-04-23 09:53:00.000000 voila-sepal-ui-0.3.0/setup.py
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.328310 voila-sepal-ui-0.3.0/share/
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.328310 voila-sepal-ui-0.3.0/share/jupyter/
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.328310 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.328310 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.328310 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.336310 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)      218 2024-04-22 20:05:29.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/jupyter-clip.js
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)  4644326 2024-04-22 20:05:29.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)   432225 2024-04-22 20:05:29.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/loading_light.gif
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     3635 2024-04-22 20:05:29.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.336310 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     6368 2024-04-22 12:45:12.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     6771 2024-04-23 08:22:05.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/app.html
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)       27 2024-04-22 12:45:12.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/conf.json
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     3036 2024-04-23 09:41:25.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)      486 2024-03-28 07:45:47.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/sepal-ui-scripts.html
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.340310 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)      218 2024-03-19 08:12:36.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/jupyter-clip.js
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)  4644326 2024-03-20 13:25:07.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_dark.gif
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)   432225 2024-03-19 08:38:14.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     3635 2024-04-22 12:45:12.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     9269 2024-04-22 12:45:12.000000 voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/util.js
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.328310 voila-sepal-ui-0.3.0/share/jupyter/voila/
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.328310 voila-sepal-ui-0.3.0/share/jupyter/voila/templates/
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.340310 voila-sepal-ui-0.3.0/share/jupyter/voila/templates/sepal-ui-base/
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     1566 2024-04-22 11:10:40.000000 voila-sepal-ui-0.3.0/share/jupyter/voila/templates/sepal-ui-base/index.html.j2
-drwxrwxr-x   0 dguerrero  (1000) dguerrero  (1000)        0 2024-04-23 09:59:14.340310 voila-sepal-ui-0.3.0/voila_sepal_ui.egg-info/
--rw-r--r--   0 dguerrero  (1000) dguerrero  (1000)      268 2024-04-23 09:59:14.000000 voila-sepal-ui-0.3.0/voila_sepal_ui.egg-info/PKG-INFO
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)     1167 2024-04-23 09:59:14.000000 voila-sepal-ui-0.3.0/voila_sepal_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)        1 2024-04-23 09:59:14.000000 voila-sepal-ui-0.3.0/voila_sepal_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)       18 2024-04-23 09:59:14.000000 voila-sepal-ui-0.3.0/voila_sepal_ui.egg-info/requires.txt
--rw-rw-r--   0 dguerrero  (1000) dguerrero  (1000)        6 2024-04-23 09:59:14.000000 voila-sepal-ui-0.3.0/voila_sepal_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.738800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/jupyter-clip.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4644326 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   432225 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_light.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.738800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/sepal-ui-scripts.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/jupyter-clip.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4644326 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_dark.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   432225 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/share/jupyter/voila/templates/sepal-ui-base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/voila/templates/sepal-ui-base/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/top_level.txt
```

### Comparing `voila-sepal-ui-0.3.0/setup.py` & `voila_sepal_ui-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         )
 
 
 setup(
     name="voila-sepal-ui",
     description="A sepal-ui template for Voila",
     data_files=data_files,
-    install_requires=["voila>=0.3.0,<0.5"],
-    version="0.3.0",
+    install_requires=["voila>=0.4.1,<0.5"],
+    version="0.4.1",
     include_package_data=True,
     author="Daniel Guerrero Machado",
     author_email="dfgm2006@gmail.com",
     url="https://github.com/dfguerrerom/voila-sepal-ui",
     keywords=["ipython", "jupyter", "widgets", "voila", "sepal-ui"],
     cmdclass={
         "develop": DevelopCmd,
```

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/loading_light.gif` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_light.gif`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/app.html` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/app.html`

 * *Files 1% similar despite different names*

```diff
@@ -107,25 +107,25 @@
           />
         </v-card-text>
       </v-card>
     </v-layout>
   `,
     data() {
       return {
-        base_url: "/",
+        base_url: "",
       };
     },
-    props: ["loading_text", "loading", "title"],
+    props: ["loading_text", "loading", "title", "base_url"],
     computed: {
       imageUrl() {
         // Assuming the Vuetify theme dark status is accessible
         // via this.$vuetify.theme.dark
         return this.$vuetify.theme.dark
-          ? this.base_url + "/static/loading_dark.gif"
-          : this.base_url + "/static/loading_light.gif";
+          ? this.base_url + "static/loading_dark.gif"
+          : this.base_url + "static/loading_light.gif";
       },
     },
     watch: {
       voilaDebugMessages(newVal, oldVal) {
         console.log("voilaDebugMessages changed:", newVal);
       },
     },
```

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         {% include "ansi.js" %}
         {% include "util.js" %}
     </script>
 
     {% include "app.html" %}
 
     <script>
-        app.baseUrl = '{{resources.base_url}}voila/';
+        app.base_url = '{{resources.base_url}}voila/';
     </script>
 </body>
 {% block notebook_execute %}
 {% endblock notebook_execute %}
 {% set cell_count = nb.cells|length %}
 
 {% block cell_generator %}
```

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_dark.gif` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_dark.gif`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/nbconvert/templates/sepal-ui-base/util.js` & `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/util.js`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/share/jupyter/voila/templates/sepal-ui-base/index.html.j2` & `voila_sepal_ui-0.4.1/share/jupyter/voila/templates/sepal-ui-base/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila-sepal-ui-0.3.0/voila_sepal_ui.egg-info/SOURCES.txt` & `voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

