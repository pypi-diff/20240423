# Comparing `tmp/gradio_leaderboard-0.0.3.tar.gz` & `tmp/gradio_leaderboard-0.0.4.tar.gz`

## Comparing `gradio_leaderboard-0.0.3.tar` & `gradio_leaderboard-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/__init__.py
--rw-r--r--   0        0        0    17452 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/leaderboard.py
--rw-r--r--   0        0        0    32788 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/leaderboard.pyi
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0  1007331 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/component/index.js
--rw-r--r--   0        0        0  1498909 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/component/style.css
--rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/example/index.js
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/demo/__init__.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/demo/app.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/demo/config.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/demo/css.css
--rw-r--r--   0        0        0    14497 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/demo/docs.md
--rw-r--r--   0        0        0   227857 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/demo/leaderboard_data.json
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/demo/space.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/Example.svelte
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/Index.svelte
--rw-r--r--   0        0        0    50963 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/package-lock.json
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/package.json
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/Checkboxgroup.svelte
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/EditableCell.svelte
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/Example.svelte
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/SimpleTextbox.svelte
--rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/Slider.svelte
--rw-r--r--   0        0        0    24334 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/Table.svelte
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/VirtualTable.svelte
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/frontend/shared/utils.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/.gitignore
--rw-r--r--   0        0        0    14708 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/README.md
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    15830 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/__init__.py
+-rw-r--r--   0        0        0    17452 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/leaderboard.py
+-rw-r--r--   0        0        0    32788 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/leaderboard.pyi
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/component/__vite-browser-external-2447137e.js
+-rw-r--r--   0        0        0  1007331 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/component/index.js
+-rw-r--r--   0        0        0  1498909 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/component/style.css
+-rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/example/index.js
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/demo/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/demo/app.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/demo/config.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/demo/css.css
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/demo/docs.md
+-rw-r--r--   0        0        0   227857 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/demo/leaderboard_data.json
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/demo/space.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/Example.svelte
+-rw-r--r--   0        0        0    10188 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/Index.svelte
+-rw-r--r--   0        0        0    50963 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/package-lock.json
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/package.json
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/Checkboxgroup.svelte
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/EditableCell.svelte
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/Example.svelte
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/SimpleTextbox.svelte
+-rw-r--r--   0        0        0     4775 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/Slider.svelte
+-rw-r--r--   0        0        0    24334 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/Table.svelte
+-rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/VirtualTable.svelte
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/frontend/shared/utils.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/.gitignore
+-rw-r--r--   0        0        0    14692 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/README.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    15814 2020-02-02 00:00:00.000000 gradio_leaderboard-0.0.4/PKG-INFO
```

### Comparing `gradio_leaderboard-0.0.3/backend/gradio_leaderboard/leaderboard.py` & `gradio_leaderboard-0.0.4/backend/gradio_leaderboard/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/backend/gradio_leaderboard/leaderboard.pyi` & `gradio_leaderboard-0.0.4/backend/gradio_leaderboard/leaderboard.pyi`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/component/index.js` & `gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/component/style.css` & `gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js` & `gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/component/wrapper-6f348d45-19fa94bf.js`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/example/index.js` & `gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/backend/gradio_leaderboard/templates/example/style.css` & `gradio_leaderboard-0.0.4/backend/gradio_leaderboard/templates/example/style.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/demo/app.py` & `gradio_leaderboard-0.0.4/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/demo/config.py` & `gradio_leaderboard-0.0.4/demo/config.py`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/demo/css.css` & `gradio_leaderboard-0.0.4/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/demo/docs.md` & `gradio_leaderboard-0.0.4/demo/docs.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # gradio_leaderboard
 
 ## 🔋⚡️🥇 Super fast, batteries included Leaderboards with minimal code.
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.3%20-%20orange">  
+<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.2%20-%20orange">  
 
 
 The `gradio_leaderboard` package helps you build fully functional and performant leaderboard demos with `gradio`.
 
 Place the `gradio_leaderboard.Leaderboard` component anywhere in your Gradio application (and optionally pass in some configuration). That's it!
 
 For example usage, please see the [Usage](#usage) section.
@@ -122,15 +122,15 @@
                                      placeholder="Search by name or country. To search by country, type 'country:<query>'",
                                      label="Search"),
     )
 
 demo.launch()
 ```
 
-![colum_search_gif](https://github.com/freddyaboulton/gradio-leaderboard/assets/41651716/4725f812-ffca-4ef9-951f-77574accd159)
+![](https://github.com/freddyaboulton/gradio-leaderboard/assets/41651716/032a50ef-01e0-48c4-a323-c84d09ccb3db)
 
 
 ### Filtering
 
 You can let users filter out rows from the leaderboard with the `filter_columns` parameter.
 This will display a series of form elements that users can use to select/deselect which rows are displayed.
```

### Comparing `gradio_leaderboard-0.0.3/demo/leaderboard_data.json` & `gradio_leaderboard-0.0.4/demo/leaderboard_data.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/Example.svelte` & `gradio_leaderboard-0.0.4/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/Index.svelte` & `gradio_leaderboard-0.0.4/frontend/Index.svelte`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 	<Row>
 		<Column>
 			{#if search_columns.primary_column}
 				<Row>
 					<Simpletextbox
 						label={search_columns.label ?? "Search"}
 						show_label={true}
-						placeholder={search_columns.placeholder ?? "Separate multiple queries with ';'."}
+						placeholder={ search_columns.placeholder ?? "Separate multiple queries with ';'."}
 						interactive={true}
 						{gradio}
 						on:submit={(e) => search_value = e.detail}
 					/>
 				</Row>
 			{/if}
 			{#if select_columns_config.allow}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 visible} padding={false} {elem_id} {elem_classes} container={false} {scale}
 {min_width} allow_overflow={false} > {#if search_columns.primary_column}
-? "Search"} show_label={true} placeholder={search_columns.placeholder ??
+? "Search"} show_label={true} placeholder={ search_columns.placeholder ??
 "Separate multiple queries with ';'."} interactive={true} {gradio} on:submit={
 (e) => search_value = e.detail} /> {/if} {#if select_columns_config.allow}
 | "Select Columns to Show"} show_label={select_columns_config.show_label} info=
 {select_columns_config.info} {gradio} bind:value={default_selection} choices=
 {headers.filter(s => !(hide_columns.includes(s) ||
 select_columns_config.cant_deselect.includes(s))).map(s => [s, s])}
 {loading_status} /> {/if} {#each filter_columns as col, i} {#if col.type ===
```

### Comparing `gradio_leaderboard-0.0.3/frontend/package-lock.json` & `gradio_leaderboard-0.0.4/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/package.json` & `gradio_leaderboard-0.0.4/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/shared/Checkboxgroup.svelte` & `gradio_leaderboard-0.0.4/frontend/shared/Checkboxgroup.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/shared/EditableCell.svelte` & `gradio_leaderboard-0.0.4/frontend/shared/EditableCell.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/shared/SimpleTextbox.svelte` & `gradio_leaderboard-0.0.4/frontend/shared/SimpleTextbox.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/shared/Slider.svelte` & `gradio_leaderboard-0.0.4/frontend/shared/Slider.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/shared/Table.svelte` & `gradio_leaderboard-0.0.4/frontend/shared/Table.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/shared/VirtualTable.svelte` & `gradio_leaderboard-0.0.4/frontend/shared/VirtualTable.svelte`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/frontend/shared/utils.ts` & `gradio_leaderboard-0.0.4/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_leaderboard-0.0.3/README.md` & `gradio_leaderboard-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                                      placeholder="Search by name or country. To search by country, type 'country:<query>'",
                                      label="Search"),
     )
 
 demo.launch()
 ```
 
-![colum_search_gif](https://github.com/freddyaboulton/gradio-leaderboard/assets/41651716/4725f812-ffca-4ef9-951f-77574accd159)
+![](https://github.com/freddyaboulton/gradio-leaderboard/assets/41651716/032a50ef-01e0-48c4-a323-c84d09ccb3db)
 
 
 ### Filtering
 
 You can let users filter out rows from the leaderboard with the `filter_columns` parameter.
 This will display a series of form elements that users can use to select/deselect which rows are displayed.
```

### Comparing `gradio_leaderboard-0.0.3/pyproject.toml` & `gradio_leaderboard-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_leaderboard"
-version = "0.0.3"
+version = "0.0.4"
 description = "Super fast , batteries included Leaderboard component ⚡️"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "YOUR NAME", email = "YOUREMAIL@domain.com" }]
 keywords = ["gradio-custom-component", "gradio-template-Dataframe", "leaderboard", "dataframe", "data", "table"]
 # Add dependencies here
@@ -32,11 +32,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_leaderboard/templates", "*.pyi", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates"]
+artifacts = ["/backend/gradio_leaderboard/templates", "*.pyi", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates", "backend/gradio_leaderboard/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_leaderboard"]
```

### Comparing `gradio_leaderboard-0.0.3/PKG-INFO` & `gradio_leaderboard-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_leaderboard
-Version: 0.0.3
+Version: 0.0.4
 Summary: Super fast , batteries included Leaderboard component ⚡️
 Author-email: YOUR NAME <YOUREMAIL@domain.com>
 License-Expression: MIT
 Keywords: data,dataframe,gradio-custom-component,gradio-template-Dataframe,leaderboard,table
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -162,15 +162,15 @@
                                      placeholder="Search by name or country. To search by country, type 'country:<query>'",
                                      label="Search"),
     )
 
 demo.launch()
 ```
 
-![colum_search_gif](https://github.com/freddyaboulton/gradio-leaderboard/assets/41651716/4725f812-ffca-4ef9-951f-77574accd159)
+![](https://github.com/freddyaboulton/gradio-leaderboard/assets/41651716/032a50ef-01e0-48c4-a323-c84d09ccb3db)
 
 
 ### Filtering
 
 You can let users filter out rows from the leaderboard with the `filter_columns` parameter.
 This will display a series of form elements that users can use to select/deselect which rows are displayed.
```

