# Comparing `tmp/voila_sepal_ui-0.4.1.tar.gz` & `tmp/voila_sepal_ui-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voila_sepal_ui-0.4.1.tar", last modified: Tue Apr 23 12:17:43 2024, max compression
+gzip compressed data, was "voila_sepal_ui-0.5.0.tar", last modified: Tue Apr 23 14:19:24 2024, max compression
```

## Comparing `voila_sepal_ui-0.4.1.tar` & `voila_sepal_ui-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.738800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/jupyter-clip.js
--rw-r--r--   0 runner    (1001) docker     (127)  4644326 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif
--rw-r--r--   0 runner    (1001) docker     (127)   432225 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_light.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.738800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/app.html
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/conf.json
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/sepal-ui-scripts.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/jupyter-clip.js
--rw-r--r--   0 runner    (1001) docker     (127)  4644326 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_dark.gif
--rw-r--r--   0 runner    (1001) docker     (127)   432225 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/voila/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.730800 voila_sepal_ui-0.4.1/share/jupyter/voila/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/share/jupyter/voila/templates/sepal-ui-base/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 12:17:33.000000 voila_sepal_ui-0.4.1/share/jupyter/voila/templates/sepal-ui-base/index.html.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 12:17:43.746800 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 12:17:43.000000 voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.075902 voila_sepal_ui-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 14:19:24.075902 voila_sepal_ui-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:19:24.075902 voila_sepal_ui-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.063902 voila_sepal_ui-0.5.0/share/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.063902 voila_sepal_ui-0.5.0/share/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.063902 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.063902 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.063902 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.071902 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/jupyter-clip.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4644326 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   432225 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/loading_light.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.071902 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/app.html
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/conf.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/sepal-ui-scripts.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.075902 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/jupyter-clip.js
+-rw-r--r--   0 runner    (1001) docker     (127)   437366 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_dark.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   432225 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.063902 voila_sepal_ui-0.5.0/share/jupyter/voila/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.063902 voila_sepal_ui-0.5.0/share/jupyter/voila/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.075902 voila_sepal_ui-0.5.0/share/jupyter/voila/templates/sepal-ui-base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-23 14:19:15.000000 voila_sepal_ui-0.5.0/share/jupyter/voila/templates/sepal-ui-base/index.html.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:19:24.075902 voila_sepal_ui-0.5.0/voila_sepal_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 14:19:24.000000 voila_sepal_ui-0.5.0/voila_sepal_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-23 14:19:24.000000 voila_sepal_ui-0.5.0/voila_sepal_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:19:24.000000 voila_sepal_ui-0.5.0/voila_sepal_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 14:19:24.000000 voila_sepal_ui-0.5.0/voila_sepal_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 14:19:24.000000 voila_sepal_ui-0.5.0/voila_sepal_ui.egg-info/top_level.txt
```

### Comparing `voila_sepal_ui-0.4.1/setup.py` & `voila_sepal_ui-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         )
 
 
 setup(
     name="voila-sepal-ui",
     description="A sepal-ui template for Voila",
     data_files=data_files,
-    install_requires=["voila>=0.4.1,<0.5"],
-    version="0.4.1",
+    install_requires=["voila>=0.5.0,<0.5"],
+    version="0.5.0",
     include_package_data=True,
     author="Daniel Guerrero Machado",
     author_email="dfgm2006@gmail.com",
     url="https://github.com/dfguerrerom/voila-sepal-ui",
     keywords=["ipython", "jupyter", "widgets", "voila", "sepal-ui"],
     cmdclass={
         "develop": DevelopCmd,
```

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/loading_dark.gif`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/loading_light.gif` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/loading_light.gif`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/lab/static/sepal_ui_styles.css`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/ansi.js`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/app.html` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/app.html`

 * *Files 6% similar despite different names*

```diff
@@ -91,38 +91,40 @@
         <v-card-text
           style="display: flex; flex-direction: column; align-items: center"
         >
           <v-card-title>
             <h2>{{ title }}</h2>
           </v-card-title>
 
-          <v-card-subtitle>
+        <v-card-subtitle>
             <h3>{{ loading_text }}</h3>
           </v-card-subtitle>
           <img
+            v-if="imageUrl" 
             :src="imageUrl"
             alt="SEPAL loading"
             align-center
             justify-center
             width="250px"
           />
         </v-card-text>
       </v-card>
     </v-layout>
   `,
     data() {
       return {
-        base_url: "",
+        base_url: null,
       };
     },
     props: ["loading_text", "loading", "title", "base_url"],
     computed: {
       imageUrl() {
-        // Assuming the Vuetify theme dark status is accessible
-        // via this.$vuetify.theme.dark
+        if (!this.base_url) {
+          return null;
+        }
         return this.$vuetify.theme.dark
           ? this.base_url + "static/loading_dark.gif"
           : this.base_url + "static/loading_light.gif";
       },
     },
     watch: {
       voilaDebugMessages(newVal, oldVal) {
```

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/loading_light.gif`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/static/sepal_ui_styles.css`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/nbconvert/templates/sepal-ui-base/util.js` & `voila_sepal_ui-0.5.0/share/jupyter/nbconvert/templates/sepal-ui-base/util.js`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/share/jupyter/voila/templates/sepal-ui-base/index.html.j2` & `voila_sepal_ui-0.5.0/share/jupyter/voila/templates/sepal-ui-base/index.html.j2`

 * *Files identical despite different names*

### Comparing `voila_sepal_ui-0.4.1/voila_sepal_ui.egg-info/SOURCES.txt` & `voila_sepal_ui-0.5.0/voila_sepal_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

