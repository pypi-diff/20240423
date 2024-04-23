# Comparing `tmp/hintbot-1.1.0.tar.gz` & `tmp/hintbot-1.2.0.tar.gz`

## Comparing `hintbot-1.1.0.tar` & `hintbot-1.2.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hintbot-1.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hintbot-1.1.0/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hintbot-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 hintbot-1.1.0/RELEASE.md
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hintbot-1.1.0/install.json
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hintbot-1.1.0/setup.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hintbot-1.1.0/tsconfig.json
--rw-r--r--   0        0        0   220911 2020-02-02 00:00:00.000000 hintbot-1.1.0/yarn.lock
--rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 hintbot-1.1.0/example/assignment4.ipynb
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/_version.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/application.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/handlers.py
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/package.json
--rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/schemas/hintbot/package.json.orig
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/schemas/hintbot/plugin.json
--rw-r--r--   0        0        0     7995 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/static/496.6b1ebc6e468d93ac9af2.js
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/static/747.b4f1d80ad223bd2a7f08.js
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/static/remoteEntry.9bdbd9afe7633029ae9a.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hintbot-1.1.0/hintbot/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hintbot-1.1.0/jupyter-config/server-config/hintbot.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.1.0/schema/plugin.json
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 hintbot-1.1.0/src/createHintBanner.ts
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hintbot-1.1.0/src/handler.ts
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 hintbot-1.1.0/src/index.ts
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 hintbot-1.1.0/src/requestHint.ts
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 hintbot-1.1.0/src/showReflectionDialog.tsx
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 hintbot-1.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hintbot-1.1.0/style/index.js
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 hintbot-1.1.0/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 hintbot-1.1.0/LICENSE
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 hintbot-1.1.0/README.md
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hintbot-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5810 2020-02-02 00:00:00.000000 hintbot-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 hintbot-1.2.0/.copier-answers.yml
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 hintbot-1.2.0/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hintbot-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 hintbot-1.2.0/RELEASE.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 hintbot-1.2.0/install.json
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 hintbot-1.2.0/setup.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hintbot-1.2.0/tsconfig.json
+-rw-r--r--   0        0        0   220911 2020-02-02 00:00:00.000000 hintbot-1.2.0/yarn.lock
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 hintbot-1.2.0/example/assignment4.ipynb
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/_version.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/application.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/handlers.py
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/package.json
+-rw-r--r--   0        0        0     6983 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/schemas/hintbot/package.json.orig
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/schemas/hintbot/plugin.json
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/496.116a981237ad27c0bb8f.js
+-rw-r--r--   0        0        0     7450 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/747.ded73249030e62fecded.js
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/remoteEntry.f3930c09f071042e569d.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 hintbot-1.2.0/hintbot/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 hintbot-1.2.0/jupyter-config/server-config/hintbot.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 hintbot-1.2.0/schema/plugin.json
+-rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/createHintBanner.ts
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/handler.ts
+-rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/index.ts
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/requestHint.ts
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/showHintTypeDialog.tsx
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 hintbot-1.2.0/src/showReflectionDialog.tsx
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 hintbot-1.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 hintbot-1.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 hintbot-1.2.0/style/index.js
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 hintbot-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 hintbot-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 hintbot-1.2.0/README.md
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 hintbot-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 hintbot-1.2.0/PKG-INFO
```

### Comparing `hintbot-1.1.0/RELEASE.md` & `hintbot-1.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/package.json` & `hintbot-1.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9774305555555557%*

 * *Differences: {"'dependencies'": "{'jupyterlab-pioneer': '^1.3.0'}", "'version'": "'1.2.0'"}*

```diff
@@ -8,15 +8,15 @@
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/notebook": "^4.0.10",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
-        "jupyterlab-pioneer": "^1.2.0"
+        "jupyterlab-pioneer": "^1.3.0"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
@@ -203,9 +203,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.2.0"
 }
```

### Comparing `hintbot-1.1.0/tsconfig.json` & `hintbot-1.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/yarn.lock` & `hintbot-1.2.0/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3410,15 +3410,15 @@
     "@types/react-addons-linked-state-mixin": ^0.14.22
     "@typescript-eslint/eslint-plugin": ^6.1.0
     "@typescript-eslint/parser": ^6.1.0
     css-loader: ^6.7.1
     eslint: ^8.36.0
     eslint-config-prettier: ^8.8.0
     eslint-plugin-prettier: ^5.0.0
-    jupyterlab-pioneer: ^1.2.0
+    jupyterlab-pioneer: ^1.3.0
     mkdirp: ^1.0.3
     npm-run-all: ^4.1.5
     prettier: ^3.0.0
     rimraf: ^5.0.1
     source-map-loader: ^1.0.2
     style-loader: ^3.3.1
     stylelint: ^15.10.1
@@ -3926,25 +3926,25 @@
 "jsonpointer@npm:^5.0.1":
   version: 5.0.1
   resolution: "jsonpointer@npm:5.0.1"
   checksum: 0b40f712900ad0c846681ea2db23b6684b9d5eedf55807b4708c656f5894b63507d0e28ae10aa1bddbea551241035afe62b6df0800fc94c2e2806a7f3adecd7c
   languageName: node
   linkType: hard
 
-"jupyterlab-pioneer@npm:^1.2.0":
-  version: 1.2.0
-  resolution: "jupyterlab-pioneer@npm:1.2.0"
+"jupyterlab-pioneer@npm:^1.3.0":
+  version: 1.3.0
+  resolution: "jupyterlab-pioneer@npm:1.3.0"
   dependencies:
     "@jupyterlab/application": ^4.0.0
     "@jupyterlab/apputils": ^4.1.9
     "@jupyterlab/coreutils": ^6.0.0
     "@jupyterlab/mainmenu": ^4.0.9
     "@jupyterlab/notebook": ^4.0.5
     "@jupyterlab/services": ^7.0.0
-  checksum: 0cfbeb70f8c1edd1166b4eace6409152ec1bb951836a773d626dbcd7689ed0e75a753132d7e8a64663f0bf49c14e9f3fc0d09824fbeb21776c320780f495bb2f
+  checksum: 260a5a1098cedc5cfa9039deb6e6ec1882abca707f9e9d3bdd967475ac55e0234f5ede2795b1b325a7364deda81bc7cd5f011f192d0633b0d2b31a6bf431146e
   languageName: node
   linkType: hard
 
 "keyv@npm:^4.5.3":
   version: 4.5.4
   resolution: "keyv@npm:4.5.4"
   dependencies:
```

### Comparing `hintbot-1.1.0/example/assignment4.ipynb` & `hintbot-1.2.0/example/assignment4.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973958333333334%*

 * *Differences: {"'cells'": "{2: {'metadata': {delete: ['remaining_hints']}}, 5: {'metadata': {delete: "*

 * *            "['remaining_hints']}}, 8: {'metadata': {delete: ['remaining_hints']}}, 11: "*

 * *            "{'metadata': {delete: ['remaining_hints']}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.12.2'}}"}*

```diff
@@ -70,16 +70,15 @@
                     "cell_type": "markdown",
                     "checksum": "54f9597da40cf65f246bfe8eca7a8a4b",
                     "grade": false,
                     "grade_id": "cell-7e5190c7ffsf2e42",
                     "locked": true,
                     "schema_version": 3,
                     "solution": false
-                },
-                "remaining_hints": 4
+                }
             },
             "source": [
                 "## Question 1: Data Preprocessing\n",
                 "For this question, perform the following:\n",
                 "\n",
                 "- remove rows with missing values\n",
                 "- keep flights departing from airports (ORIGIN_AIRPORT) that we want to look at (BOS, JFK, SFO and LAX)\n",
@@ -145,16 +144,15 @@
                     "cell_type": "markdown",
                     "checksum": "216fa865128c1f5c793e329d73791c55",
                     "grade": false,
                     "grade_id": "cell-89s80693491a3d33",
                     "locked": true,
                     "schema_version": 3,
                     "solution": false
-                },
-                "remaining_hints": 5
+                }
             },
             "source": [
                 "## Question 2\n",
                 "Merge flights_df dataframe with airports_df dataframe and return the number of departing flights (*NUM_FLIGHTS*) per airport (*IATA_CODE*) across the year."
             ]
         },
         {
@@ -216,16 +214,15 @@
                     "checksum": "6992f2767319208a151e5d807a0e9207",
                     "grade": false,
                     "grade_id": "cell-8f659c09rbae5694",
                     "locked": true,
                     "schema_version": 3,
                     "solution": false,
                     "task": false
-                },
-                "remaining_hints": 5
+                }
             },
             "source": [
                 "## Question 3\n",
                 "For this question, find the top three airline names which have high number of flights and the least percentage of delay compared to other airlines. The result should be a dataframe which has three columns *AIRLINE_NAME*, *NUM_FLIGHTS* and *PERC_DELAY*.\n",
                 "\n",
                 "Hint:\n",
                 "- percentage of delay for each airline is obtained using groupby and apply methods\n",
@@ -292,16 +289,15 @@
                     "checksum": "a9cb8a450b3b70abef792dcbdb0266a2",
                     "grade": false,
                     "grade_id": "cell-fb2846rbbb62c8a7",
                     "locked": true,
                     "schema_version": 3,
                     "solution": false,
                     "task": false
-                },
-                "remaining_hints": 5
+                }
             },
             "source": [
                 "## Question 4\n",
                 "For this question, obtain the monthly percentage of delays for each *ORIGIN_AIRPORT*.\n",
                 "\n",
                 "Example Result:\n",
                 "\n",
@@ -374,13 +370,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.12.1"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `hintbot-1.1.0/hintbot/__init__.py` & `hintbot-1.2.0/hintbot/__init__.py`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/hintbot/handlers.py` & `hintbot-1.2.0/hintbot/handlers.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,25 +59,41 @@
         self.status = STATUS["Cancelled"]
 
 class RouteHandler(ExtensionHandlerMixin, JupyterHandler):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @tornado.web.authenticated
+    async def get(self, resource):
+        try:
+            self.set_header("Content-Type", "application/json")
+            if resource == "version":
+                self.finish(json.dumps(__version__))
+            elif resource == "id":
+                self.finish(json.dumps(os.getenv('WORKSPACE_ID')))
+            else:
+                self.set_status(404)
+        except Exception as e:
+            self.log.error(str(e))
+            self.set_status(500)
+            self.finish(json.dumps(str(e)))
+        
+    @tornado.web.authenticated
     async def post(self, resource):
         try:
             body = json.loads(self.request.body)
             if resource == "hint":
-                student_id = os.getenv('WORKSPACE_ID')
+                # hint_type = body.get('hint_type')
                 problem_id = body.get('problem_id')
                 buggy_notebook_path = body.get('buggy_notebook_path')
                 response = requests.post(
                     HOST_URL,
                     data={
-                        "student_id": student_id,
+                        "student_id": "x",
+                        # "hint_type": hint_type,
                         "problem_id": problem_id,
                     },
                     files={"file": ("notebook.ipynb", open(buggy_notebook_path, "rb"))},
                     timeout=10
                 )
 
                 if response.status_code == 200:
```

### Comparing `hintbot-1.1.0/hintbot/labextension/package.json` & `hintbot-1.2.0/hintbot/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9771412037037038%*

 * *Differences: {"'dependencies'": "{'jupyterlab-pioneer': '^1.3.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f3930c09f071042e569d.js'}}",*

 * * "'version'": "'1.2.0'"}*

```diff
@@ -8,15 +8,15 @@
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/notebook": "^4.0.10",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
-        "jupyterlab-pioneer": "^1.2.0"
+        "jupyterlab-pioneer": "^1.3.0"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
@@ -105,15 +105,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/educational-technology-collective/hintbot",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9bdbd9afe7633029ae9a.js",
+            "load": "static/remoteEntry.f3930c09f071042e569d.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "hintbot"
                 },
@@ -208,9 +208,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.2.0"
 }
```

### Comparing `hintbot-1.1.0/hintbot/labextension/schemas/hintbot/package.json.orig` & `hintbot-1.2.0/hintbot/labextension/schemas/hintbot/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9774305555555557%*

 * *Differences: {"'dependencies'": "{'jupyterlab-pioneer': '^1.3.0'}", "'version'": "'1.2.0'"}*

```diff
@@ -8,15 +8,15 @@
     },
     "dependencies": {
         "@jupyterlab/application": "^4.0.0",
         "@jupyterlab/coreutils": "^6.0.0",
         "@jupyterlab/notebook": "^4.0.10",
         "@jupyterlab/services": "^7.0.0",
         "@jupyterlab/settingregistry": "^4.0.0",
-        "jupyterlab-pioneer": "^1.2.0"
+        "jupyterlab-pioneer": "^1.3.0"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@jupyterlab/builder": "^4.0.0",
         "@types/json-schema": "^7.0.11",
         "@types/react": "^18.0.26",
         "@types/react-addons-linked-state-mixin": "^0.14.22",
@@ -203,9 +203,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.1.0"
+    "version": "1.2.0"
 }
```

### Comparing `hintbot-1.1.0/hintbot/labextension/schemas/hintbot/plugin.json` & `hintbot-1.2.0/hintbot/labextension/schemas/hintbot/plugin.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/hintbot/labextension/static/496.6b1ebc6e468d93ac9af2.js` & `hintbot-1.2.0/hintbot/labextension/static/496.116a981237ad27c0bb8f.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 "use strict";
 (self.webpackChunkhintbot = self.webpackChunkhintbot || []).push([
     [496], {
         496: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => p
             });
-            var o = n(372),
-                a = n(392),
-                i = n(678),
-                r = n(778),
-                l = n(770),
-                s = n(29),
-                d = n.n(s);
+            var o = n(99),
+                a = n(947),
+                i = n(464),
+                r = n(882),
+                s = n(637),
+                l = n(29),
+                d = n.n(l);
             class c extends i.ReactWidget {
                 constructor(e) {
                     super(), this._message = "", this._message = e
                 }
                 getValue() {
                     var e;
                     return null === (e = this.node.querySelector("textarea")) || void 0 === e ? void 0 : e.value
@@ -29,23 +29,25 @@
                         rows: 10
                     })))
                 }
             }
             const u = e => (0, i.showDialog)({
                 title: "Reflection",
                 body: new c(e),
-                buttons: [i.Dialog.createButton({
-                    label: "Cancel"
+                buttons: [i.Dialog.cancelButton({
+                    label: "Cancel",
+                    className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
                 }), i.Dialog.createButton({
-                    label: "Submit"
+                    label: "Submit",
+                    className: "jp-Dialog-button jp-mod-accept jp-mod-styled"
                 })],
                 hasClose: !1
             });
-            var m = n(170),
-                h = n(387);
+            var m = n(671),
+                h = n(818);
             async function g(e = "", t = {}) {
                 const n = h.ServerConnection.makeSettings(),
                     o = m.URLExt.join(n.baseUrl, "hintbot", e);
                 let a;
                 try {
                     a = await h.ServerConnection.makeRequest(o, t, n)
                 } catch (e) {
@@ -59,15 +61,15 @@
                 }
                 if (!a.ok) throw new h.ServerConnection.ResponseError(a, i.message || i);
                 return i
             }
             const b = async (e, t, n, o) => {
                 var a;
                 const r = null === (a = o.getMetadata("nbgrader")) || void 0 === a ? void 0 : a.grade_id,
-                    l = o.getMetadata("remaining_hints");
+                    s = o.getMetadata("remaining_hints");
                 if (document.getElementById("hint-banner"))(0, i.showDialog)({
                     title: "Please review previous hint first.",
                     buttons: [i.Dialog.createButton({
                         label: "Dismiss",
                         className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
                     })]
                 }), n.exporters.forEach((t => {
@@ -75,15 +77,15 @@
                         eventName: "HintAlreadyExists",
                         eventTime: Date.now(),
                         eventInfo: {
                             gradeId: r
                         }
                     }, t, !1)
                 }));
-                else if (l < 1)(0, i.showDialog)({
+                else if (s < 1)(0, i.showDialog)({
                     title: "No hint left for this question.",
                     buttons: [i.Dialog.createButton({
                         label: "Dismiss",
                         className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
                     })]
                 }), n.exporters.forEach((t => {
                     n.publishEvent(e, {
@@ -91,25 +93,39 @@
                         eventTime: Date.now(),
                         eventInfo: {
                             gradeId: r
                         }
                     }, t, !1)
                 }));
                 else {
-                    const a = t.get("preReflection").composite,
-                        s = t.get("postReflection").composite;
+                    let a = t.get("preReflection").composite,
+                        l = t.get("postReflection").composite;
+                    try {
+                        const e = (await g("id")).split("").map((e => e.charCodeAt(0) - 64)).reduce(((e, t) => e + t), 0) % 3;
+                        console.log(`Condition ${e}`), 0 === e ? (a = !0, l = !1) : 1 === e ? (a = !1, l = !0) : (a = !1, l = !1)
+                    } catch (t) {
+                        n.exporters.forEach((o => {
+                            n.publishEvent(e, {
+                                eventName: "ConvertIDError",
+                                eventTime: Date.now(),
+                                eventInfo: {
+                                    error: t
+                                }
+                            }, o, !0)
+                        })), console.log(t)
+                    }
                     if ((async (e, t, n, o) => {
                             var a;
                             const r = n.getMetadata("nbgrader").grade_id,
-                                l = document.createElement("div");
-                            l.id = "hint-banner-placeholder", e.content.node.insertBefore(l, e.content.node.firstChild);
-                            const s = document.createElement("div");
-                            s.id = "hint-banner", null === (a = e.content.node.parentElement) || void 0 === a || a.insertBefore(s, e.content.node), s.innerHTML = '<p><span class="loader"></span>Retrieving hint... Please do not refresh the page.</p> <p>It usually takes around 2 minutes to generate a hint. You may continue to work on the assignment in the meantime.</p>';
+                                s = document.createElement("div");
+                            s.id = "hint-banner-placeholder", e.content.node.insertBefore(s, e.content.node.firstChild);
+                            const l = document.createElement("div");
+                            l.id = "hint-banner", null === (a = e.content.node.parentElement) || void 0 === a || a.insertBefore(l, e.content.node), l.innerHTML = '<p><span class="loader"></span>Retrieving hint... Please do not refresh the page.</p> <p>It usually takes around 2 minutes to generate a hint. You may continue to work on the assignment in the meantime.</p>';
                             const d = document.createElement("div");
-                            d.id = "hint-banner-cancel-button", d.innerText = "Cancel request", s.appendChild(d), d.onclick = async () => {
+                            d.id = "hint-banner-cancel-button", d.innerText = "Cancel request", l.appendChild(d), d.onclick = async () => {
                                 await g("cancel", {
                                     method: "POST",
                                     body: JSON.stringify({
                                         problem_id: r
                                     })
                                 })
                             };
@@ -117,115 +133,126 @@
                                 const n = await g("hint", {
                                     method: "POST",
                                     body: JSON.stringify({
                                         problem_id: r,
                                         buggy_notebook_path: e.context.path
                                     })
                                 });
-                                if (console.log("create ticket", n), !(null == n ? void 0 : n.request_id)) throw new Error("Unable to create ticket");
+                                console.log("create ticket", n);
+                                const a = null == n ? void 0 : n.request_id;
+                                if (!a) throw new Error;
                                 {
                                     const n = setInterval((async () => {
-                                        const a = await g("check", {
+                                        const c = await g("check", {
                                             method: "POST",
                                             body: JSON.stringify({
                                                 problem_id: r
                                             })
                                         });
-                                        if (0 !== a.status)
-                                            if (1 === a.status) console.log("success"), clearInterval(n), (n => {
+                                        if (0 !== c.status)
+                                            if (1 === c.status) console.log("success"), clearInterval(n), ((n, a) => {
                                                 t.exporters.forEach((o => {
                                                     t.publishEvent(e, {
                                                         eventName: "HintRequestCompleted",
                                                         eventTime: Date.now(),
                                                         eventInfo: {
                                                             hintContent: n,
-                                                            gradeId: r
+                                                            gradeId: r,
+                                                            requestId: a
                                                         }
                                                     }, o, !0)
-                                                })), s.innerText = n, d.remove();
-                                                const a = document.createElement("div");
-                                                a.id = "hint-banner-buttons-container";
+                                                })), l.innerText = n, d.remove();
                                                 const i = document.createElement("div");
-                                                i.id = "hint-banner-buttons";
-                                                const c = document.createElement("button");
-                                                c.classList.add("hint-banner-button"), c.innerText = "Helpful 👍";
+                                                i.id = "hint-banner-buttons-container";
+                                                const c = document.createElement("div");
+                                                c.id = "hint-banner-buttons";
                                                 const m = document.createElement("button");
-                                                m.classList.add("hint-banner-button"), m.innerText = "Unhelpful 👎";
-                                                const h = async a => {
+                                                m.classList.add("hint-banner-button"), m.innerText = "Helpful 👍";
+                                                const h = document.createElement("button");
+                                                h.classList.add("hint-banner-button"), h.innerText = "Unhelpful 👎";
+                                                const g = async i => {
                                                     if (t.exporters.forEach((o => {
                                                             t.publishEvent(e, {
                                                                 eventName: "HintEvaluated",
                                                                 eventTime: Date.now(),
                                                                 eventInfo: {
                                                                     gradeId: r,
+                                                                    requestId: a,
                                                                     hintContent: n,
-                                                                    evaluation: a
+                                                                    evaluation: i
                                                                 }
                                                             }, o, !0)
                                                         })), o) {
                                                         const o = await u("Write a brief statement of what you learned from the hint and how you will use it to solve the problem.");
-                                                        "Submit" === o.button.label && (s.remove(), l.remove()), t.exporters.forEach((a => {
+                                                        "Submit" === o.button.label && (l.remove(), s.remove()), t.exporters.forEach((i => {
                                                             t.publishEvent(e, {
                                                                 eventName: "PostReflection",
                                                                 eventTime: Date.now(),
                                                                 eventInfo: {
                                                                     status: o.button.label,
                                                                     gradeId: r,
+                                                                    requestId: a,
                                                                     hintContent: n,
                                                                     reflection: o.value
                                                                 }
-                                                            }, a, !0)
+                                                            }, i, !0)
                                                         }))
-                                                    } else s.remove(), l.remove()
+                                                    } else l.remove(), s.remove()
                                                 };
-                                                c.onclick = () => {
-                                                    h("helpful")
-                                                }, m.onclick = () => {
-                                                    h("unhelpful")
-                                                }, i.appendChild(m), i.appendChild(c), a.appendChild(i), s.appendChild(a)
-                                            })(a.result.feedback);
+                                                m.onclick = () => {
+                                                    g("helpful")
+                                                }, h.onclick = () => {
+                                                    g("unhelpful")
+                                                }, c.appendChild(h), c.appendChild(m), i.appendChild(c), l.appendChild(i)
+                                            })(c.result.feedback, a);
                                             else {
-                                                if (2 !== a.status) throw clearInterval(n), new Error("Unable to retrieve hint");
-                                                console.log("cancelled"), clearInterval(n), s.remove(), l.remove(), (0, i.showDialog)({
-                                                    title: "Hint Request Cancelled",
-                                                    buttons: [i.Dialog.createButton({
-                                                        label: "Dismiss",
-                                                        className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
-                                                    })]
-                                                }), t.exporters.forEach((n => {
-                                                    t.publishEvent(e, {
-                                                        eventName: "HintRequestCancelled",
-                                                        eventTime: Date.now(),
-                                                        eventInfo: {
-                                                            gradeId: r
-                                                        }
-                                                    }, n, !1)
-                                                }))
+                                                if (2 !== c.status) throw clearInterval(n), new Error(a);
+                                                console.log("cancelled"), clearInterval(n), (n => {
+                                                    l.remove(), s.remove(), (0, i.showDialog)({
+                                                        title: "Hint Request Cancelled",
+                                                        buttons: [i.Dialog.createButton({
+                                                            label: "Dismiss",
+                                                            className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
+                                                        })]
+                                                    }), t.exporters.forEach((o => {
+                                                        t.publishEvent(e, {
+                                                            eventName: "HintRequestCancelled",
+                                                            eventTime: Date.now(),
+                                                            eventInfo: {
+                                                                gradeId: r,
+                                                                requestId: n
+                                                            }
+                                                        }, o, !1)
+                                                    }))
+                                                })(a)
                                             }
                                         else console.log("loading")
                                     }), 1e3)
                                 }
                             } catch (n) {
-                                console.log(n), s.remove(), l.remove(), (0, i.showDialog)({
-                                    title: "Hint Request Error. Please try again later",
-                                    buttons: [i.Dialog.createButton({
-                                        label: "Dismiss",
-                                        className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
-                                    })]
-                                }), t.exporters.forEach((n => {
-                                    t.publishEvent(e, {
-                                        eventName: "HintRequestError",
-                                        eventTime: Date.now(),
-                                        eventInfo: {
-                                            gradeId: r
-                                        }
-                                    }, n, !1)
-                                }))
+                                console.log(n), (n => {
+                                    l.remove(), s.remove(), (0, i.showDialog)({
+                                        title: "Hint Request Error. Please try again later",
+                                        buttons: [i.Dialog.createButton({
+                                            label: "Dismiss",
+                                            className: "jp-Dialog-button jp-mod-reject jp-mod-styled"
+                                        })]
+                                    }), t.exporters.forEach((o => {
+                                        t.publishEvent(e, {
+                                            eventName: "HintRequestError",
+                                            eventTime: Date.now(),
+                                            eventInfo: {
+                                                gradeId: r,
+                                                requestId: null == n ? void 0 : n.message
+                                            }
+                                        }, o, !1)
+                                    }))
+                                })(n)
                             }
-                        })(e, n, o, s), o.setMetadata("remaining_hints", l - 1), document.getElementById(r).innerText = `Hint (${l-1} left for this question)`, e.context.save(), a) {
+                        })(e, n, o, l), o.setMetadata("remaining_hints", s - 1), document.getElementById(r).innerText = `Hint (${s-1} left for this question)`, e.context.save(), a) {
                         document.getElementById("hint-banner").style.filter = "blur(10px)";
                         const t = await u("Write a brief statement of what the problem is that you are facing and why you think your solution is not working.");
                         document.getElementById("hint-banner").style.filter = "none", n.exporters.forEach((o => {
                             n.publishEvent(e, {
                                 eventName: "PreReflection",
                                 eventTime: Date.now(),
                                 eventInfo: {
@@ -242,46 +269,48 @@
                         })
                     }
                 }
             }, v = {
                 id: "hintbot:plugin",
                 description: "A JupyterLab extension.",
                 autoStart: !0,
-                requires: [a.INotebookTracker, o.ISettingRegistry, l.IJupyterLabPioneer],
+                requires: [a.INotebookTracker, o.ISettingRegistry, s.IJupyterLabPioneer],
                 activate: async (e, t, n, o) => {
                     const a = document.createElement("button");
                     a.innerText = "Activate HintBot Extension", a.id = "hintbot-activation-button";
-                    const l = document.createElement("div");
-                    l.appendChild(a);
-                    const s = await n.load(v.id);
+                    const s = document.createElement("div");
+                    s.appendChild(a);
+                    const l = await n.load(v.id);
                     t.widgetAdded.connect((async (e, t) => {
                         await t.revealed, await o.loadExporters(t), t.toolbar.insertAfter("spacer", "hintbot-activation-button", new r.Widget({
-                            node: l
+                            node: s
                         })), a.onclick = async () => {
                             "Confirm activation" === (await (0, i.showDialog)({
                                 body: "The hintbot extension is a prototype and not required to be used for the course. \n The hints generated could be wrong, and it involves sending data to third party services outside of the university.",
-                                buttons: [i.Dialog.createButton({
-                                    label: "Cancel"
+                                buttons: [i.Dialog.cancelButton({
+                                    label: "Cancel",
+                                    className: "jp-mod-reject jp-mod-styled"
                                 }), i.Dialog.createButton({
-                                    label: "Confirm activation"
+                                    label: "Confirm activation",
+                                    className: "jp-mod-accept jp-mod-styled"
                                 })],
                                 hasClose: !1
                             })).button.label && (await (async (e, t, n) => {
                                 var o, a, i, r;
-                                const l = t.get("hintQuantity").composite,
-                                    s = null === (o = e.content.model) || void 0 === o ? void 0 : o.cells;
-                                if (s && e.model.getMetadata("etc_identifier") && "7ca0093b-b622-4463-8696-65f1e0f33522" === e.model.getMetadata("etc_identifier"))
-                                    for (let o = 0; o < s.length; o++)
-                                        if (s.get(o).getMetadata("nbgrader") && "markdown" === (null === (a = s.get(o).getMetadata("nbgrader")) || void 0 === a ? void 0 : a.cell_type) && (null === (i = s.get(o).getMetadata("nbgrader")) || void 0 === i ? void 0 : i.grade_id) && "cell-018440eg2f1b6a62" !== (null === (r = s.get(o).getMetadata("nbgrader")) || void 0 === r ? void 0 : r.grade_id)) {
+                                const s = t.get("hintQuantity").composite,
+                                    l = null === (o = e.content.model) || void 0 === o ? void 0 : o.cells;
+                                if (l && e.model.getMetadata("etc_identifier") && "7ca0093b-b622-4463-8696-65f1e0f33522" === e.model.getMetadata("etc_identifier"))
+                                    for (let o = 0; o < l.length; o++)
+                                        if (l.get(o).getMetadata("nbgrader") && "markdown" === (null === (a = l.get(o).getMetadata("nbgrader")) || void 0 === a ? void 0 : a.cell_type) && (null === (i = l.get(o).getMetadata("nbgrader")) || void 0 === i ? void 0 : i.grade_id) && "cell-018440eg2f1b6a62" !== (null === (r = l.get(o).getMetadata("nbgrader")) || void 0 === r ? void 0 : r.grade_id)) {
                                             const a = document.createElement("button");
-                                            a.classList.add("hint-button"), a.id = s.get(o).getMetadata("nbgrader").grade_id, a.onclick = () => b(e, t, n, s.get(o)), e.content.widgets[o].node.appendChild(a), void 0 === s.get(o).getMetadata("remaining_hints") ? (s.get(o).setMetadata("remaining_hints", l), a.innerText = `Hint (${l} left for this question)`) : a.innerText = `Hint (${s.get(o).getMetadata("remaining_hints")} left for this question)`
+                                            a.classList.add("hint-button"), a.id = l.get(o).getMetadata("nbgrader").grade_id, a.onclick = () => b(e, t, n, l.get(o)), e.content.widgets[o].node.appendChild(a), void 0 === l.get(o).getMetadata("remaining_hints") ? (l.get(o).setMetadata("remaining_hints", s), a.innerText = `Hint (${s} left for this question)`) : a.innerText = `Hint (${l.get(o).getMetadata("remaining_hints")} left for this question)`
                                         }
-                            })(t, s, o), a.remove(), o.exporters.forEach((e => o.publishEvent(t, {
+                            })(t, l, o), a.remove(), o.exporters.forEach((e => o.publishEvent(t, {
                                 eventName: "HintBotActivated",
-                                eventTime: new Date
+                                eventTime: Date.now()
                             }, e, !1))))
                         }
                     }))
                 }
             }, p = v
         }
     }
```

### Comparing `hintbot-1.1.0/hintbot/labextension/static/747.b4f1d80ad223bd2a7f08.js` & `hintbot-1.2.0/hintbot/labextension/static/747.ded73249030e62fecded.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
             t.d(e, {
                 Z: () => c
             });
             var r = t(81),
                 o = t.n(r),
                 i = t(645),
                 a = t.n(i)()(o());
-            a.push([n.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.hint-button {\n  width: 60%;\n  display: block;\n  background-color: #1976d2;\n  border: 1px solid #e0e0e0;\n  border-radius: 3px;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  font-weight: bold;\n  line-height: 1.2;\n  margin: 6px auto;\n  padding: 6px 12px;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n}\n\n:root {\n  --hint-banner-height: 25vh;\n}\n\n#hint-banner-placeholder {\n  width: 100%;\n  height: var(--hint-banner-height);\n  background-color: #fff;\n}\n\n#hint-banner {\n  position: fixed;\n  z-index: 10;\n  left: 0;\n  right: 0;\n  top: 29px;\n  width: calc(100% - 32px);\n  height: calc(var(--hint-banner-height));\n  margin: 0 auto;\n  padding: 0 20px;\n  background-color: #fff;\n  border: 1px solid #e0e0e0;\n  font-size: 14px;\n  display: flex;\n  flex-direction: column;\n  justify-content: space-around;\n  align-items: center;\n}\n\n#hint-banner-cancel-button {\n  background-color: #1976d2;\n  border: 1px solid #e0e0e0;\n  border-radius: 3px;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  line-height: 1.2;\n  margin: 6px;\n  padding: 6px 12px;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n}\n\n#hint-banner p {\n  display: flex;\n  align-items: center;\n}\n\n.loader {\n  width: 24px;\n  height: 24px;\n  margin-right: 50px;\n  border: 3px solid #1976d2;\n  border-bottom-color: transparent;\n  border-radius: 50%;\n  display: inline-block;\n  box-sizing: border-box;\n  animation: rotation 1s linear infinite;\n}\n\n@keyframes rotation {\n  0% {\n    transform: rotate(0deg);\n  }\n\n  100% {\n    transform: rotate(360deg);\n  }\n}\n\n#hint-banner-buttons-container {\n  display: flex;\n  width: 90%;\n  justify-content: flex-end;\n}\n\n.hint-banner-button {\n  background-color: #1976d2;\n  border: 1px solid #e0e0e0;\n  border-radius: 3px;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  line-height: 1.2;\n  margin: 6px;\n  padding: 6px 12px;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n}\n\n.reflection {\n  width: 400px;\n}\n\n.reflection-input {\n  width: 97%;\n  resize: vertical;\n}\n", ""]);
+            a.push([n.id, "/*\n    See the JupyterLab Developer Guide for useful CSS Patterns:\n\n    https://jupyterlab.readthedocs.io/en/stable/developer/css.html\n*/\n.hint {\n  background-color: #f5f5f5;\n  display: flex;\n  margin: 10px auto 10px 72px;\n  justify-content: space-between;\n  border: 1px solid #e0e0e0;\n  padding: 5px 10px;\n}\n\n.hint-left {\n  display: flex;\n  width: 40%;\n  justify-content: flex-start;\n  align-items: center;\n  padding-left: 10px;\n}\n\n.help-text {\n  font-size: 14px;\n  line-height: 1.2;\n}\n\n.hint-type-button {\n  width: 25px;\n  height: 25px;\n  background-color: #bbbaba;\n  border: 0.5px solid #e0e0e0;\n  border-radius: 50%;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  line-height: 1.2;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n  margin-left: 10px;\n}\n\n.hint-buttons {\n  display: flex;\n  justify-content: flex-end;\n  width: 60%;\n}\n\n/* .hint-button {\n  display: inline-block;\n  width: 100px;\n  background-color: #e0e0e0;\n  border: 0.5px solid #e0e0e0;\n  border-radius: 3px;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  line-height: 1.2;\n  margin: 6px 10px;\n  padding: 6px 12px;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n} */\n\n.hint-button {\n  width: 60%;\n  display: block;\n  background-color: #1976d2;\n  border: 1px solid #e0e0e0;\n  border-radius: 3px;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  font-weight: bold;\n  line-height: 1.2;\n  margin: 6px auto;\n  padding: 6px 12px;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n}\n\n.planning {\n  background-color: #81c0ff;\n}\n\n.debugging {\n  background-color: #f87b7b;\n}\n\n.optimizing {\n  background-color: #7fc47f;\n}\n\n.hint-type {\n  line-height: 40px;\n}\n\n:root {\n  --hint-banner-height: 25vh;\n}\n\n#hint-banner-placeholder {\n  width: 100%;\n  height: var(--hint-banner-height);\n  background-color: #fff;\n}\n\n#hint-banner {\n  position: fixed;\n  z-index: 10;\n  left: 0;\n  right: 0;\n  top: 29px;\n  width: calc(100% - 32px);\n  height: calc(var(--hint-banner-height));\n  margin: 0 auto;\n  padding: 0 20px;\n  background-color: #fff;\n  border: 1px solid #e0e0e0;\n  font-size: 14px;\n  display: flex;\n  flex-direction: column;\n  justify-content: space-around;\n  align-items: center;\n}\n\n#hint-banner-cancel-button {\n  background-color: #1976d2;\n  border: 1px solid #e0e0e0;\n  border-radius: 3px;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  line-height: 1.2;\n  margin: 6px;\n  padding: 6px 12px;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n}\n\n#hint-banner p {\n  display: flex;\n  align-items: center;\n}\n\n.loader {\n  width: 24px;\n  height: 24px;\n  margin-right: 50px;\n  border: 3px solid #1976d2;\n  border-bottom-color: transparent;\n  border-radius: 50%;\n  display: inline-block;\n  box-sizing: border-box;\n  animation: rotation 1s linear infinite;\n}\n\n@keyframes rotation {\n  0% {\n    transform: rotate(0deg);\n  }\n\n  100% {\n    transform: rotate(360deg);\n  }\n}\n\n#hint-banner-buttons-container {\n  display: flex;\n  width: 90%;\n  justify-content: flex-end;\n}\n\n.hint-banner-button {\n  background-color: #1976d2;\n  border: 1px solid #e0e0e0;\n  border-radius: 3px;\n  color: #fff;\n  cursor: pointer;\n  font-size: 14px;\n  line-height: 1.2;\n  margin: 6px;\n  padding: 6px 12px;\n  text-align: center;\n  text-decoration: none;\n  white-space: nowrap;\n}\n\n.reflection {\n  width: 400px;\n}\n\n.reflection-input {\n  width: 97%;\n  resize: vertical;\n}\n", ""]);
             const c = a
         },
         645: n => {
             n.exports = function(n) {
                 var e = [];
                 return e.toString = function() {
                     return this.map((function(e) {
@@ -27,17 +27,17 @@
                     ]);
                     var a = {};
                     if (r)
                         for (var c = 0; c < this.length; c++) {
                             var s = this[c][0];
                             null != s && (a[s] = !0)
                         }
-                    for (var d = 0; d < n.length; d++) {
-                        var p = [].concat(n[d]);
-                        r && a[p[0]] || (void 0 !== i && (void 0 === p[5] || (p[1] = "@layer".concat(p[5].length > 0 ? " ".concat(p[5]) : "", " {").concat(p[1], "}")), p[5] = i), t && (p[2] ? (p[1] = "@media ".concat(p[2], " {").concat(p[1], "}"), p[2] = t) : p[2] = t), o && (p[4] ? (p[1] = "@supports (".concat(p[4], ") {").concat(p[1], "}"), p[4] = o) : p[4] = "".concat(o)), e.push(p))
+                    for (var p = 0; p < n.length; p++) {
+                        var d = [].concat(n[p]);
+                        r && a[d[0]] || (void 0 !== i && (void 0 === d[5] || (d[1] = "@layer".concat(d[5].length > 0 ? " ".concat(d[5]) : "", " {").concat(d[1], "}")), d[5] = i), t && (d[2] ? (d[1] = "@media ".concat(d[2], " {").concat(d[1], "}"), d[2] = t) : d[2] = t), o && (d[4] ? (d[1] = "@supports (".concat(d[4], ") {").concat(d[1], "}"), d[4] = o) : d[4] = "".concat(o)), e.push(d))
                     }
                 }, e
             }
         },
         81: n => {
             n.exports = function(n) {
                 return n[1]
@@ -53,18 +53,18 @@
                         break
                     } return t
             }
 
             function r(n, r) {
                 for (var i = {}, a = [], c = 0; c < n.length; c++) {
                     var s = n[c],
-                        d = r.base ? s[0] + r.base : s[0],
-                        p = i[d] || 0,
-                        l = "".concat(d, " ").concat(p);
-                    i[d] = p + 1;
+                        p = r.base ? s[0] + r.base : s[0],
+                        d = i[p] || 0,
+                        l = "".concat(p, " ").concat(d);
+                    i[p] = d + 1;
                     var u = t(l),
                         f = {
                             css: s[1],
                             media: s[2],
                             sourceMap: s[3],
                             supports: s[4],
                             layer: s[5]
@@ -97,17 +97,17 @@
                 var i = r(n = n || [], o = o || {});
                 return function(n) {
                     n = n || [];
                     for (var a = 0; a < i.length; a++) {
                         var c = t(i[a]);
                         e[c].references--
                     }
-                    for (var s = r(n, o), d = 0; d < i.length; d++) {
-                        var p = t(i[d]);
-                        0 === e[p].references && (e[p].updater(), e.splice(p, 1))
+                    for (var s = r(n, o), p = 0; p < i.length; p++) {
+                        var d = t(i[p]);
+                        0 === e[d].references && (e[d].updater(), e.splice(d, 1))
                     }
                     i = s
                 }
             }
         },
         569: n => {
             var e = {};
@@ -180,19 +180,19 @@
             t.r(e);
             var r = t(379),
                 o = t.n(r),
                 i = t(795),
                 a = t.n(i),
                 c = t(569),
                 s = t.n(c),
-                d = t(565),
-                p = t.n(d),
+                p = t(565),
+                d = t.n(p),
                 l = t(216),
                 u = t.n(l),
                 f = t(589),
                 h = t.n(f),
-                b = t(150),
-                x = {};
-            x.styleTagTransform = h(), x.setAttributes = p(), x.insert = s().bind(null, "head"), x.domAPI = a(), x.insertStyleElement = u(), o()(b.Z, x), b.Z && b.Z.locals && b.Z.locals
+                x = t(150),
+                b = {};
+            b.styleTagTransform = h(), b.setAttributes = d(), b.insert = s().bind(null, "head"), b.domAPI = a(), b.insertStyleElement = u(), o()(x.Z, b), x.Z && x.Z.locals && x.Z.locals
         }
     }
 ]);
```

### Comparing `hintbot-1.1.0/hintbot/labextension/static/remoteEntry.9bdbd9afe7633029ae9a.js` & `hintbot-1.2.0/hintbot/labextension/static/remoteEntry.f3930c09f071042e569d.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, u, l, f, s, d, p, c, h, v, b, g, m, y = {
-            380: (e, r, t) => {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, b, g, m, y = {
+            361: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(496).then((() => () => t(496))),
                         "./extension": () => t.e(496).then((() => () => t(496))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
                                 o = t.S[n];
                             if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
                     get: () => o,
-                    init: () => i
+                    init: () => a
                 })
             }
         },
         w = {};
 
     function S(e) {
         var r = w[e];
@@ -43,49 +43,49 @@
         }), r
     }, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        496: "6b1ebc6e468d93ac9af2",
-        747: "b4f1d80ad223bd2a7f08"
+        496: "116a981237ad27c0bb8f",
+        747: "ded73249030e62fecded"
     } [e] + ".js?v=" + {
-        496: "6b1ebc6e468d93ac9af2",
-        747: "b4f1d80ad223bd2a7f08"
+        496: "116a981237ad27c0bb8f",
+        747: "ded73249030e62fecded"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "hintbot:", S.l = (t, n, o, i) => {
+    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "hintbot:", S.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, u;
+            var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
                     var s = l[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        a = s;
+                        i = s;
                         break
                     }
                 }
-            a || (u = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, S.nc && a.setAttribute("nonce", S.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var d = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(p);
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: i
                 }), 12e4);
-            a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), u && document.head.appendChild(a)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, S.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -95,26 +95,26 @@
             r = {};
         S.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
-                var i = S.S[t],
-                    a = "hintbot",
+                var a = S.S[t],
+                    i = "hintbot",
                     u = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var o = i[e] = i[e] || {},
+                    var o = a[e] = a[e] || {},
                         u = o[r];
-                    (!u || !u.loaded && (1 != !u.eager ? n : a > u.from)) && (o[r] = {
+                    (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => S.e(496).then((() => () => S(496))),
-                        from: a,
+                        from: i,
                         eager: !1
                     })
-                })("hintbot", "1.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("hintbot", "1.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -130,50 +130,50 @@
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
             var o = e[n],
-                i = (typeof o)[0];
-            if (n >= r.length) return "u" == i;
-            var a = r[n],
-                u = (typeof a)[0];
-            if (i != u) return "o" == i && "n" == u || "s" == u || "u" == i;
-            if ("o" != i && "u" != i && o != a) return o < a;
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
+            var i = r[n],
+                u = (typeof i)[0];
+            if (a != u) return "o" == a && "n" == u || "s" == u || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
     }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(u = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(u = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, u);
             return t
         }
-        var a = [];
-        for (i = 1; i < e.length; i++) {
-            var u = e[i];
-            a.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? a.pop() + " " + a.pop() : o(u))
+        var i = [];
+        for (a = 1; a < e.length; a++) {
+            var u = e[a];
+            i.push(0 === u ? "not(" + l() + ")" : 1 === u ? "(" + l() + " || " + l() + ")" : 2 === u ? i.pop() + " " + i.pop() : o(u))
         }
         return l();
 
         function l() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
-            for (var a = 0, u = 1, l = !0;; u++, a++) {
+            for (var i = 0, u = 1, l = !0;; u++, i++) {
                 var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
                 if ("u" == s) {
                     if (!l || "u" != d) return !1
                 } else if (l)
                     if (d == s)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
@@ -187,49 +187,49 @@
                     if (u <= n || s < d != o) return !1;
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
-        for (a = 1; a < e.length; a++) {
-            var h = e[a];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+        for (i = 1; i < e.length; i++) {
+            var h = e[i];
+            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
-    }, a = (e, r) => {
+    }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return i(n, o) || d(l(e, t, o, n)), p(e[t][o])
+        return a(n, o) || d(l(e, t, o, n)), p(e[t][o])
     }, s = (e, r, t, n) => {
         var o = u(e, t);
-        if (!i(n, o)) throw new Error(l(e, t, o, n));
+        if (!a(n, o)) throw new Error(l(e, t, o, n));
         return p(e[t][o])
     }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, o) {
-        var i = S.I(r);
-        return i && i.then ? i.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), v = c(((e, r, t, n) => (a(e, t), s(r, 0, t, n)))), b = {}, g = {
+        var a = S.I(r);
+        return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = c(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), b = {}, g = {
         29: () => h("default", "react", [1, 18, 2, 0]),
-        170: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 12]),
-        372: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 12]),
-        387: () => h("default", "@jupyterlab/services", [1, 7, 0, 12]),
-        392: () => h("default", "@jupyterlab/notebook", [1, 4, 0, 12]),
-        678: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 12]),
-        770: () => v("default", "jupyterlab-pioneer", [1, 1, 2, 0]),
-        778: () => h("default", "@lumino/widgets", [1, 2, 0, 1])
+        99: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 6]),
+        464: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        637: () => v("default", "jupyterlab-pioneer", [1, 1, 3, 0]),
+        671: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        818: () => h("default", "@jupyterlab/services", [1, 7, 1, 6]),
+        882: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
+        947: () => h("default", "@jupyterlab/notebook", [1, 4, 1, 6])
     }, m = {
-        496: [29, 170, 372, 387, 392, 678, 770, 778]
+        496: [29, 99, 464, 637, 671, 818, 882, 947]
     }, S.f.consumes = (e, r) => {
         S.o(m, e) && m[e].forEach((e => {
             if (S.o(b, e)) return r.push(b[e]);
             var t = r => {
                     b[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
@@ -253,33 +253,33 @@
         S.f.j = (r, t) => {
             var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => n = e[r] = [t, o]));
                     t.push(n[2] = o);
-                    var i = S.p + S.u(r),
-                        a = new Error;
-                    S.l(i, (t => {
+                    var a = S.p + S.u(r),
+                        i = new Error;
+                    S.l(a, (t => {
                         if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
-                                i = t && t.target && t.target.src;
-                            a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [i, a, u] = t,
+                var n, o, [a, i, u] = t,
                     l = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) S.o(a, n) && (S.m[n] = a[n]);
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in i) S.o(i, n) && (S.m[n] = i[n]);
                     u && u(S)
                 }
-                for (r && r(t); l < i.length; l++) o = i[l], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < a.length; l++) o = a[l], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkhintbot = self.webpackChunkhintbot || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), S.nc = void 0;
-    var E = S(380);
+    var E = S(361);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).hintbot = E
 })();
```

### Comparing `hintbot-1.1.0/hintbot/labextension/static/third-party-licenses.json` & `hintbot-1.2.0/hintbot/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/schema/plugin.json` & `hintbot-1.2.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/src/createHintBanner.ts` & `hintbot-1.2.0/src/createHintBanner.ts`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import { requestAPI } from './handler';
 
 export const createHintBanner = async (
   notebookPanel: NotebookPanel,
   pioneer: IJupyterLabPioneer,
   cell: ICellModel,
   postReflection: boolean
+  // hintType: string
 ) => {
   const gradeId = cell.getMetadata('nbgrader').grade_id;
 
   const hintBannerPlaceholder = document.createElement('div');
   hintBannerPlaceholder.id = 'hint-banner-placeholder';
   notebookPanel.content.node.insertBefore(
     hintBannerPlaceholder,
@@ -38,24 +39,26 @@
       method: 'POST',
       body: JSON.stringify({
         problem_id: gradeId
       })
     });
   };
 
-  const hintRequestCompleted = (hintContent: string) => {
+  const hintRequestCompleted = (hintContent: string, requestId: string) => {
     pioneer.exporters.forEach(exporter => {
       pioneer.publishEvent(
         notebookPanel,
         {
           eventName: 'HintRequestCompleted',
           eventTime: Date.now(),
           eventInfo: {
             hintContent: hintContent,
-            gradeId: gradeId
+            gradeId: gradeId,
+            requestId: requestId
+            // hintType: hintType
           }
         },
         exporter,
         true
       );
     });
     hintBanner.innerText = hintContent;
@@ -78,16 +81,18 @@
         pioneer.publishEvent(
           notebookPanel,
           {
             eventName: 'HintEvaluated',
             eventTime: Date.now(),
             eventInfo: {
               gradeId: gradeId,
+              requestId: requestId,
               hintContent: hintContent,
               evaluation: evaluation
+              // hintType: hintType
             }
           },
           exporter,
           true
         );
       });
       if (postReflection) {
@@ -105,16 +110,18 @@
             notebookPanel,
             {
               eventName: 'PostReflection',
               eventTime: Date.now(),
               eventInfo: {
                 status: dialogResult.button.label,
                 gradeId: gradeId,
+                requestId: requestId,
                 hintContent: hintContent,
                 reflection: dialogResult.value
+                // hintType: hintType
               }
             },
             exporter,
             true
           );
         });
       } else {
@@ -131,15 +138,15 @@
     hintBannerButtons.appendChild(unhelpfulButton);
     hintBannerButtons.appendChild(helpfulButton);
 
     hintBannerButtonsContainer.appendChild(hintBannerButtons);
     hintBanner.appendChild(hintBannerButtonsContainer);
   };
 
-  const hintRequestCancelled = () => {
+  const hintRequestCancelled = (requestId: string) => {
     hintBanner.remove();
     hintBannerPlaceholder.remove();
     showDialog({
       title: 'Hint Request Cancelled',
       buttons: [
         Dialog.createButton({
           label: 'Dismiss',
@@ -150,24 +157,25 @@
     pioneer.exporters.forEach(exporter => {
       pioneer.publishEvent(
         notebookPanel,
         {
           eventName: 'HintRequestCancelled',
           eventTime: Date.now(),
           eventInfo: {
-            gradeId: gradeId
+            gradeId: gradeId,
+            requestId: requestId
           }
         },
         exporter,
         false
       );
     });
   };
 
-  const hintRequestError = () => {
+  const hintRequestError = (e: Error) => {
     hintBanner.remove();
     hintBannerPlaceholder.remove();
     showDialog({
       title: 'Hint Request Error. Please try again later',
       buttons: [
         Dialog.createButton({
           label: 'Dismiss',
@@ -178,15 +186,16 @@
     pioneer.exporters.forEach(exporter => {
       pioneer.publishEvent(
         notebookPanel,
         {
           eventName: 'HintRequestError',
           eventTime: Date.now(),
           eventInfo: {
-            gradeId: gradeId
+            gradeId: gradeId,
+            requestId: e?.message
           }
         },
         exporter,
         false
       );
     });
   };
@@ -198,22 +207,23 @@
     Error: 3
   };
 
   try {
     const response: any = await requestAPI('hint', {
       method: 'POST',
       body: JSON.stringify({
+        // hint_type: hintType,
         problem_id: gradeId,
         buggy_notebook_path: notebookPanel.context.path
       })
     });
     console.log('create ticket', response);
     const requestId = response?.request_id;
     if (!requestId) {
-      throw new Error('Unable to create ticket');
+      throw new Error();
     } else {
       const intervalId = setInterval(async () => {
         const response: any = await requestAPI('check', {
           method: 'POST',
           body: JSON.stringify({
             problem_id: gradeId
           })
@@ -221,23 +231,23 @@
 
         if (response.status === STATUS['Loading']) {
           console.log('loading');
           return;
         } else if (response.status === STATUS['Success']) {
           console.log('success');
           clearInterval(intervalId);
-          hintRequestCompleted(response.result.feedback);
+          hintRequestCompleted(response.result.feedback, requestId);
         } else if (response.status === STATUS['Cancelled']) {
           console.log('cancelled');
           clearInterval(intervalId);
-          hintRequestCancelled();
+          hintRequestCancelled(requestId);
         } else {
           clearInterval(intervalId);
-          throw new Error('Unable to retrieve hint');
+          throw new Error(requestId);
         }
       }, 1000);
     }
   } catch (e) {
     console.log(e);
-    hintRequestError();
+    hintRequestError(e as Error);
   }
 };
```

### Comparing `hintbot-1.1.0/src/handler.ts` & `hintbot-1.2.0/src/handler.ts`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/src/requestHint.ts` & `hintbot-1.2.0/src/requestHint.ts`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import { requestAPI } from './handler';
 
 export const requestHint = async (
   notebookPanel: NotebookPanel,
   settings: ISettingRegistry.ISettings,
   pioneer: IJupyterLabPioneer,
   cell: ICellModel
+  // hintType: string
 ) => {
   const gradeId = cell.getMetadata('nbgrader')?.grade_id;
   const remainingHints = cell.getMetadata('remaining_hints');
 
   if (document.getElementById('hint-banner')) {
     showDialog({
       title: 'Please review previous hint first.',
@@ -61,16 +62,53 @@
           }
         },
         exporter,
         false
       );
     });
   } else {
-    const preReflection = settings.get('preReflection').composite as boolean;
-    const postReflection = settings.get('postReflection').composite as boolean;
+    let preReflection = settings.get('preReflection').composite as boolean;
+    let postReflection = settings.get('postReflection').composite as boolean;
+
+    try {
+      const id: string = await requestAPI('id');
+      const n =
+        id
+          .split('')
+          .map(c => c.charCodeAt(0) - 64)
+          .reduce((acc, val) => acc + val, 0) % 3;
+      console.log(`Condition ${n}`);
+
+      if (n === 0) {
+        preReflection = true;
+        postReflection = false;
+      } else if (n === 1) {
+        preReflection = false;
+        postReflection = true;
+      } else {
+        preReflection = false;
+        postReflection = false;
+      }
+    } catch (e) {
+      pioneer.exporters.forEach(exporter => {
+        pioneer.publishEvent(
+          notebookPanel,
+          {
+            eventName: 'ConvertIDError',
+            eventTime: Date.now(),
+            eventInfo: {
+              error: e
+            }
+          },
+          exporter,
+          true
+        );
+      });
+      console.log(e);
+    }
 
     createHintBanner(notebookPanel, pioneer, cell, postReflection);
 
     cell.setMetadata('remaining_hints', remainingHints - 1);
     document.getElementById(gradeId).innerText = `Hint (${
       remainingHints - 1
     } left for this question)`;
@@ -90,14 +128,15 @@
           {
             eventName: 'PreReflection',
             eventTime: Date.now(),
             eventInfo: {
               status: dialogResult.button.label,
               gradeId: gradeId,
               reflection: dialogResult.value
+              // hintType: hintType
             }
           },
           exporter,
           true
         );
       });
       if (dialogResult.button.label === 'Cancel') {
```

### Comparing `hintbot-1.1.0/src/showReflectionDialog.tsx` & `hintbot-1.2.0/src/showReflectionDialog.tsx`

 * *Files 9% similar despite different names*

```diff
@@ -27,13 +27,19 @@
 }
 
 export const showReflectionDialog = (message: string) => {
   return showDialog({
     title: 'Reflection',
     body: new ReflectionInputWidget(message),
     buttons: [
-      Dialog.createButton({ label: 'Cancel' }),
-      Dialog.createButton({ label: 'Submit' })
+      Dialog.cancelButton({
+        label: 'Cancel',
+        className: 'jp-Dialog-button jp-mod-reject jp-mod-styled'
+      }),
+      Dialog.createButton({
+        label: 'Submit',
+        className: 'jp-Dialog-button jp-mod-accept jp-mod-styled'
+      })
     ],
     hasClose: false
   });
 };
```

### Comparing `hintbot-1.1.0/style/base.css` & `hintbot-1.2.0/style/base.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,73 @@
 /*
     See the JupyterLab Developer Guide for useful CSS Patterns:
 
     https://jupyterlab.readthedocs.io/en/stable/developer/css.html
 */
+.hint {
+  background-color: #f5f5f5;
+  display: flex;
+  margin: 10px auto 10px 72px;
+  justify-content: space-between;
+  border: 1px solid #e0e0e0;
+  padding: 5px 10px;
+}
+
+.hint-left {
+  display: flex;
+  width: 40%;
+  justify-content: flex-start;
+  align-items: center;
+  padding-left: 10px;
+}
+
+.help-text {
+  font-size: 14px;
+  line-height: 1.2;
+}
+
+.hint-type-button {
+  width: 25px;
+  height: 25px;
+  background-color: #bbbaba;
+  border: 0.5px solid #e0e0e0;
+  border-radius: 50%;
+  color: #fff;
+  cursor: pointer;
+  font-size: 14px;
+  line-height: 1.2;
+  text-align: center;
+  text-decoration: none;
+  white-space: nowrap;
+  margin-left: 10px;
+}
+
+.hint-buttons {
+  display: flex;
+  justify-content: flex-end;
+  width: 60%;
+}
+
+/* .hint-button {
+  display: inline-block;
+  width: 100px;
+  background-color: #e0e0e0;
+  border: 0.5px solid #e0e0e0;
+  border-radius: 3px;
+  color: #fff;
+  cursor: pointer;
+  font-size: 14px;
+  line-height: 1.2;
+  margin: 6px 10px;
+  padding: 6px 12px;
+  text-align: center;
+  text-decoration: none;
+  white-space: nowrap;
+} */
+
 .hint-button {
   width: 60%;
   display: block;
   background-color: #1976d2;
   border: 1px solid #e0e0e0;
   border-radius: 3px;
   color: #fff;
@@ -17,14 +78,30 @@
   margin: 6px auto;
   padding: 6px 12px;
   text-align: center;
   text-decoration: none;
   white-space: nowrap;
 }
 
+.planning {
+  background-color: #81c0ff;
+}
+
+.debugging {
+  background-color: #f87b7b;
+}
+
+.optimizing {
+  background-color: #7fc47f;
+}
+
+.hint-type {
+  line-height: 40px;
+}
+
 :root {
   --hint-banner-height: 25vh;
 }
 
 #hint-banner-placeholder {
   width: 100%;
   height: var(--hint-banner-height);
```

### Comparing `hintbot-1.1.0/.gitignore` & `hintbot-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/LICENSE` & `hintbot-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/README.md` & `hintbot-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/pyproject.toml` & `hintbot-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hintbot-1.1.0/PKG-INFO` & `hintbot-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hintbot
-Version: 1.1.0
+Version: 1.2.0
+Dynamic: Keywords
 Summary: A JupyterLab extension.
 Project-URL: Homepage, https://github.com/educational-technology-collective/hintbot
 Project-URL: Bug Tracker, https://github.com/educational-technology-collective/hintbot/issues
 Project-URL: Repository, https://github.com/educational-technology-collective/hintbot.git
 Author-email: etc <mengyanw@umich.edu>
 License: BSD 3-Clause License
```

