# Comparing `tmp/vite_transporter-0.4.0.tar.gz` & `tmp/vite_transporter-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vite_transporter-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vite_transporter-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vite_transporter-0.4.0.tar` & `vite_transporter-0.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.4.0/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.4.0/LICENSE
--rw-r--r--   0        0        0     3718 2024-04-21 15:35:16.830834 vite_transporter-0.4.0/README.md
--rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.4.0/app_flask_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.4.0/app_flask_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 20:38:37.815908 vite_transporter-0.4.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 20:38:37.816282 vite_transporter-0.4.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 20:38:37.816137 vite_transporter-0.4.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.4.0/app_quart_demo/__init__.py
--rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.4.0/app_quart_demo/templates/index.html
--rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.4.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
--rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.4.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css
--rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.4.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js
--rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.4.0/app_vite_demo/Index.jsx
--rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.4.0/app_vite_demo/__router__.jsx
--rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.4.0/app_vite_demo/assets/ili.gif
--rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.4.0/app_vite_demo/index.css
--rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.4.0/app_vite_demo/index.html
--rw-r--r--   0        0        0   105659 2024-04-17 18:51:11.871806 vite_transporter-0.4.0/app_vite_demo/package-lock.json
--rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.4.0/app_vite_demo/package.json
--rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.4.0/app_vite_demo/postcss.config.js
--rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.4.0/app_vite_demo/tailwind.config.js
--rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.4.0/app_vite_demo/vite.config.js
--rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.4.0/requirements/demos.txt
--rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.4.0/requirements/development.txt
--rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.4.0/requirements/main.txt
--rw-r--r--   0        0        0     2185 2024-04-23 08:28:59.829121 vite_transporter-0.4.0/vite_transporter/__init__.py
--rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.4.0/vite_transporter/_headers.py
--rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.4.0/vite_transporter/_html_tags.py
--rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.4.0/vite_transporter/helpers.py
--rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.4.0/vite_transporter/parser.py
--rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.4.0/vite_transporter/platform/__init__.py
--rw-r--r--   0        0        0     4679 2024-04-23 08:25:01.100158 vite_transporter-0.4.0/vite_transporter/platform/flask.py
--rw-r--r--   0        0        0     4743 2024-04-23 08:25:01.103735 vite_transporter-0.4.0/vite_transporter/platform/quart.py
--rw-r--r--   0        0        0     4400 1970-01-01 00:00:00.000000 vite_transporter-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5201 2024-04-17 20:37:21.973545 vite_transporter-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 vite_transporter-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4082 2024-04-23 17:32:46.753620 vite_transporter-0.4.1/README.md
+-rw-r--r--   0        0        0      738 2024-04-21 15:32:14.759993 vite_transporter-0.4.1/app_flask_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:25.368755 vite_transporter-0.4.1/app_flask_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-23 17:26:19.313411 vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    21365 2024-04-23 17:26:19.313250 vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-45b871c7.js
+-rw-r--r--   0        0        0    33644 2024-04-23 17:26:19.312967 vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-cc24c663.css
+-rw-r--r--   0        0        0      750 2024-04-21 15:32:40.857714 vite_transporter-0.4.1/app_quart_demo/__init__.py
+-rw-r--r--   0        0        0      192 2024-04-17 19:56:29.985721 vite_transporter-0.4.1/app_quart_demo/templates/index.html
+-rw-r--r--   0        0        0    39139 2024-04-17 19:55:40.663413 vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif
+-rw-r--r--   0        0        0    33329 2024-04-17 19:55:40.663791 vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-621914e8.css
+-rw-r--r--   0        0        0    20285 2024-04-17 19:55:40.663651 vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-6e585489.js
+-rw-r--r--   0        0        0     2250 2024-04-21 15:33:39.440720 vite_transporter-0.4.1/app_vite_demo/Index.jsx
+-rw-r--r--   0        0        0      536 2024-04-12 20:35:46.642592 vite_transporter-0.4.1/app_vite_demo/__router__.jsx
+-rw-r--r--   0        0        0    39139 2024-03-12 16:01:48.215679 vite_transporter-0.4.1/app_vite_demo/assets/ili.gif
+-rw-r--r--   0        0        0      596 2024-04-21 15:30:17.354196 vite_transporter-0.4.1/app_vite_demo/index.css
+-rw-r--r--   0        0        0      414 2024-04-17 19:46:30.300521 vite_transporter-0.4.1/app_vite_demo/index.html
+-rw-r--r--   0        0        0   105659 2024-04-23 17:26:15.620700 vite_transporter-0.4.1/app_vite_demo/package-lock.json
+-rw-r--r--   0        0        0      570 2024-04-12 14:55:15.273422 vite_transporter-0.4.1/app_vite_demo/package.json
+-rw-r--r--   0        0        0       80 2024-02-23 14:52:24.766425 vite_transporter-0.4.1/app_vite_demo/postcss.config.js
+-rw-r--r--   0        0        0      151 2024-03-31 09:45:49.055622 vite_transporter-0.4.1/app_vite_demo/tailwind.config.js
+-rw-r--r--   0        0        0      440 2024-04-01 09:05:29.649936 vite_transporter-0.4.1/app_vite_demo/vite.config.js
+-rw-r--r--   0        0        0     1257 2024-04-21 15:37:04.537415 vite_transporter-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-17 20:14:50.246973 vite_transporter-0.4.1/requirements/demos.txt
+-rw-r--r--   0        0        0       22 2024-04-17 20:14:46.286993 vite_transporter-0.4.1/requirements/development.txt
+-rw-r--r--   0        0        0       34 2024-04-17 16:11:12.368549 vite_transporter-0.4.1/requirements/main.txt
+-rw-r--r--   0        0        0     2185 2024-04-23 17:33:31.994141 vite_transporter-0.4.1/vite_transporter/__init__.py
+-rw-r--r--   0        0        0     2654 2024-04-21 13:26:49.370076 vite_transporter-0.4.1/vite_transporter/_headers.py
+-rw-r--r--   0        0        0     4871 2024-04-03 07:34:32.709087 vite_transporter-0.4.1/vite_transporter/_html_tags.py
+-rw-r--r--   0        0        0     4002 2024-04-17 20:42:01.707392 vite_transporter-0.4.1/vite_transporter/helpers.py
+-rw-r--r--   0        0        0      909 2024-04-17 15:48:32.502792 vite_transporter-0.4.1/vite_transporter/parser.py
+-rw-r--r--   0        0        0      178 2024-04-23 08:21:21.096283 vite_transporter-0.4.1/vite_transporter/platform/__init__.py
+-rw-r--r--   0        0        0     4679 2024-04-23 08:25:01.100158 vite_transporter-0.4.1/vite_transporter/platform/flask.py
+-rw-r--r--   0        0        0     4743 2024-04-23 08:25:01.103735 vite_transporter-0.4.1/vite_transporter/platform/quart.py
+-rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 vite_transporter-0.4.1/PKG-INFO
```

### Comparing `vite_transporter-0.4.0/.gitignore` & `vite_transporter-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/LICENSE` & `vite_transporter-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/README.md` & `vite_transporter-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 ```
 
 **Currently compatible with:**
 
 - Flask
 - Quart
 
+**Note (Flask/Quart):** When including credentials in fetch requests in the vite app.
+You must visit the serve app add first to set the credentials.
+
+For example, if the serve app is running on `http://127.0.0.1:5001`, you must visit this address first.
+
+This won't be needed in production, as it's expected that the Vite app will be served from the same domain.
+
 ## How it works
 
 ### The pyproject.toml file
 
 The pyproject.toml file is used to store what Vite apps are available.
 
 Adding the following to the pyproject.toml file will transfer all the Vite
```

### Comparing `vite_transporter-0.4.0/app_flask_demo/__init__.py` & `vite_transporter-0.4.1/app_flask_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_flask_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-621914e8.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_flask_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/index-6e585489.js`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_quart_demo/__init__.py` & `vite_transporter-0.4.1/app_quart_demo/__init__.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif` & `vite_transporter-0.4.1/app_quart_demo/vt/app_vite_demo/ili-85e34484.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_quart_demo/vt/app_vite_demo/index-621914e8.css` & `vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-cc24c663.css`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content: ""}html,:host{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,samp,pre{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dl,dd,h1,h2,h3,h4,h5,h6,hr,figure,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}ol,ul,menu{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}button,[role=button]{cursor:pointer}:disabled{cursor:default}img,svg,video,canvas,audio,iframe,embed,object{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,:before,:after{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.container{width:100%}@media (min-width: 640px){.container{max-width:640px}}@media (min-width: 768px){.container{max-width:768px}}@media (min-width: 1024px){.container{max-width:1024px}}@media (min-width: 1280px){.container{max-width:1280px}}@media (min-width: 1536px){.container{max-width:1536px}}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}.not-sr-only{position:static;width:auto;height:auto;padding:0;margin:0;overflow:visible;clip:auto;white-space:normal}.pointer-events-none{pointer-events:none}.pointer-events-auto{pointer-events:auto}.\!visible{visibility:visible!important}.visible{visibility:visible}.invisible{visibility:hidden}.collapse{visibility:collapse}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.\!relative{position:relative!important}.relative{position:relative}.sticky{position:sticky}.-inset-1{inset:-.25rem}.end-1{inset-inline-end:.25rem}.isolate{isolation:isolate}.isolation-auto{isolation:auto}.float-start{float:inline-start}.float-end{float:inline-end}.float-right{float:right}.float-left{float:left}.float-none{float:none}.clear-start{clear:inline-start}.clear-end{clear:inline-end}.clear-left{clear:left}.clear-right{clear:right}.clear-both{clear:both}.clear-none{clear:none}.mt-2{margin-top:.5rem}.box-border{box-sizing:border-box}.box-content{box-sizing:content-box}.line-clamp-none{overflow:visible;display:block;-webkit-box-orient:horizontal;-webkit-line-clamp:none}.block{display:block}.inline-block{display:inline-block}.\!inline{display:inline!important}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.inline-table{display:inline-table}.table-caption{display:table-caption}.table-cell{display:table-cell}.table-column{display:table-column}.table-column-group{display:table-column-group}.table-footer-group{display:table-footer-group}.table-header-group{display:table-header-group}.table-row-group{display:table-row-group}.table-row{display:table-row}.flow-root{display:flow-root}.grid{display:grid}.inline-grid{display:inline-grid}.contents{display:contents}.list-item{display:list-item}.hidden{display:none}.w-\[this-is\\\\\]{width:this-is\\}.w-\[this-is\]{width:this-is}.w-\[weird-and-invalid\]{width:weird-and-invalid}.flex-shrink,.shrink{flex-shrink:1}.flex-grow,.grow{flex-grow:1}.table-auto{table-layout:auto}.table-fixed{table-layout:fixed}.caption-top{caption-side:top}.caption-bottom{caption-side:bottom}.border-collapse{border-collapse:collapse}.border-separate{border-collapse:separate}.\!transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.transform,.transform-cpu{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform-gpu{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform-none{transform:none}.touch-auto{touch-action:auto}.touch-none{touch-action:none}.touch-pan-x{--tw-pan-x: pan-x;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-left{--tw-pan-x: pan-left;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-right{--tw-pan-x: pan-right;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-y{--tw-pan-y: pan-y;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-up{--tw-pan-y: pan-up;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-down{--tw-pan-y: pan-down;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pinch-zoom{--tw-pinch-zoom: pinch-zoom;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-manipulation{touch-action:manipulation}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.select-text{-webkit-user-select:text;-moz-user-select:text;user-select:text}.select-all{-webkit-user-select:all;-moz-user-select:all;user-select:all}.select-auto{-webkit-user-select:auto;-moz-user-select:auto;user-select:auto}.resize-none{resize:none}.resize-y{resize:vertical}.resize-x{resize:horizontal}.resize{resize:both}.snap-none{scroll-snap-type:none}.snap-x{scroll-snap-type:x var(--tw-scroll-snap-strictness)}.snap-y{scroll-snap-type:y var(--tw-scroll-snap-strictness)}.snap-both{scroll-snap-type:both var(--tw-scroll-snap-strictness)}.snap-mandatory{--tw-scroll-snap-strictness: mandatory}.snap-proximity{--tw-scroll-snap-strictness: proximity}.snap-start{scroll-snap-align:start}.snap-end{scroll-snap-align:end}.snap-center{scroll-snap-align:center}.snap-align-none{scroll-snap-align:none}.snap-normal{scroll-snap-stop:normal}.snap-always{scroll-snap-stop:always}.list-inside{list-style-position:inside}.list-outside{list-style-position:outside}.appearance-none{-webkit-appearance:none;-moz-appearance:none;appearance:none}.appearance-auto{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}.break-before-auto{-moz-column-break-before:auto;break-before:auto}.break-before-avoid{-moz-column-break-before:avoid;break-before:avoid}.break-before-all{-moz-column-break-before:all;break-before:all}.break-before-avoid-page{-moz-column-break-before:avoid;break-before:avoid-page}.break-before-page{-moz-column-break-before:page;break-before:page}.break-before-left{-moz-column-break-before:left;break-before:left}.break-before-right{-moz-column-break-before:right;break-before:right}.break-before-column{-moz-column-break-before:column;break-before:column}.break-inside-auto{-moz-column-break-inside:auto;break-inside:auto}.break-inside-avoid{-moz-column-break-inside:avoid;break-inside:avoid}.break-inside-avoid-page{break-inside:avoid-page}.break-inside-avoid-column{-moz-column-break-inside:avoid;break-inside:avoid-column}.break-after-auto{-moz-column-break-after:auto;break-after:auto}.break-after-avoid{-moz-column-break-after:avoid;break-after:avoid}.break-after-all{-moz-column-break-after:all;break-after:all}.break-after-avoid-page{-moz-column-break-after:avoid;break-after:avoid-page}.break-after-page{-moz-column-break-after:page;break-after:page}.break-after-left{-moz-column-break-after:left;break-after:left}.break-after-right{-moz-column-break-after:right;break-after:right}.break-after-column{-moz-column-break-after:column;break-after:column}.grid-flow-row{grid-auto-flow:row}.grid-flow-col{grid-auto-flow:column}.grid-flow-dense{grid-auto-flow:dense}.grid-flow-row-dense{grid-auto-flow:row dense}.grid-flow-col-dense{grid-auto-flow:column dense}.flex-row{flex-direction:row}.flex-row-reverse{flex-direction:row-reverse}.flex-col{flex-direction:column}.flex-col-reverse{flex-direction:column-reverse}.flex-wrap{flex-wrap:wrap}.flex-wrap-reverse{flex-wrap:wrap-reverse}.flex-nowrap{flex-wrap:nowrap}.place-content-center{place-content:center}.place-content-start{place-content:start}.place-content-end{place-content:end}.place-content-between{place-content:space-between}.place-content-around{place-content:space-around}.place-content-evenly{place-content:space-evenly}.place-content-baseline{place-content:baseline}.place-content-stretch{place-content:stretch}.place-items-start{place-items:start}.place-items-end{place-items:end}.place-items-center{place-items:center}.place-items-baseline{place-items:baseline}.place-items-stretch{place-items:stretch}.content-normal{align-content:normal}.content-center{align-content:center}.content-start{align-content:flex-start}.content-end{align-content:flex-end}.content-between{align-content:space-between}.content-around{align-content:space-around}.content-evenly{align-content:space-evenly}.content-baseline{align-content:baseline}.content-stretch{align-content:stretch}.items-start{align-items:flex-start}.items-end{align-items:flex-end}.items-center{align-items:center}.items-baseline{align-items:baseline}.items-stretch{align-items:stretch}.justify-normal{justify-content:normal}.justify-start{justify-content:flex-start}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.justify-around{justify-content:space-around}.justify-evenly{justify-content:space-evenly}.justify-stretch{justify-content:stretch}.justify-items-start{justify-items:start}.justify-items-end{justify-items:end}.justify-items-center{justify-items:center}.justify-items-stretch{justify-items:stretch}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(.5rem * var(--tw-space-x-reverse));margin-left:calc(.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-reverse>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 1}.space-x-reverse>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 1}.divide-x>:not([hidden])~:not([hidden]){--tw-divide-x-reverse: 0;border-right-width:calc(1px * var(--tw-divide-x-reverse));border-left-width:calc(1px * calc(1 - var(--tw-divide-x-reverse)))}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse: 0;border-top-width:calc(1px * calc(1 - var(--tw-divide-y-reverse)));border-bottom-width:calc(1px * var(--tw-divide-y-reverse))}.divide-y-reverse>:not([hidden])~:not([hidden]){--tw-divide-y-reverse: 1}.divide-x-reverse>:not([hidden])~:not([hidden]){--tw-divide-x-reverse: 1}.divide-solid>:not([hidden])~:not([hidden]){border-style:solid}.divide-dashed>:not([hidden])~:not([hidden]){border-style:dashed}.divide-dotted>:not([hidden])~:not([hidden]){border-style:dotted}.divide-double>:not([hidden])~:not([hidden]){border-style:double}.divide-none>:not([hidden])~:not([hidden]){border-style:none}.place-self-auto{place-self:auto}.place-self-start{place-self:start}.place-self-end{place-self:end}.place-self-center{place-self:center}.place-self-stretch{place-self:stretch}.self-auto{align-self:auto}.self-start{align-self:flex-start}.self-end{align-self:flex-end}.self-center{align-self:center}.self-stretch{align-self:stretch}.self-baseline{align-self:baseline}.justify-self-auto{justify-self:auto}.justify-self-start{justify-self:start}.justify-self-end{justify-self:end}.justify-self-center{justify-self:center}.justify-self-stretch{justify-self:stretch}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-clip{overflow:clip}.overflow-visible{overflow:visible}.overflow-scroll{overflow:scroll}.overflow-x-auto{overflow-x:auto}.overflow-y-auto{overflow-y:auto}.overflow-x-hidden{overflow-x:hidden}.overflow-y-hidden{overflow-y:hidden}.overflow-x-clip{overflow-x:clip}.overflow-y-clip{overflow-y:clip}.overflow-x-visible{overflow-x:visible}.overflow-y-visible{overflow-y:visible}.overflow-x-scroll{overflow-x:scroll}.overflow-y-scroll{overflow-y:scroll}.overscroll-auto{overscroll-behavior:auto}.overscroll-contain{overscroll-behavior:contain}.overscroll-none{overscroll-behavior:none}.overscroll-y-auto{overscroll-behavior-y:auto}.overscroll-y-contain{overscroll-behavior-y:contain}.overscroll-y-none{overscroll-behavior-y:none}.overscroll-x-auto{overscroll-behavior-x:auto}.overscroll-x-contain{overscroll-behavior-x:contain}.overscroll-x-none{overscroll-behavior-x:none}.scroll-auto{scroll-behavior:auto}.scroll-smooth{scroll-behavior:smooth}.truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.overflow-ellipsis,.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.hyphens-none{-webkit-hyphens:none;hyphens:none}.hyphens-manual{-webkit-hyphens:manual;hyphens:manual}.hyphens-auto{-webkit-hyphens:auto;hyphens:auto}.whitespace-normal{white-space:normal}.whitespace-nowrap{white-space:nowrap}.whitespace-pre{white-space:pre}.whitespace-pre-line{white-space:pre-line}.whitespace-pre-wrap{white-space:pre-wrap}.whitespace-break-spaces{white-space:break-spaces}.text-wrap{text-wrap:wrap}.text-nowrap{text-wrap:nowrap}.text-balance{text-wrap:balance}.text-pretty{text-wrap:pretty}.break-normal{overflow-wrap:normal;word-break:normal}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.break-keep{word-break:keep-all}.rounded{border-radius:.25rem}.rounded-b{border-bottom-right-radius:.25rem;border-bottom-left-radius:.25rem}.rounded-e{border-start-end-radius:.25rem;border-end-end-radius:.25rem}.rounded-l{border-top-left-radius:.25rem;border-bottom-left-radius:.25rem}.rounded-r{border-top-right-radius:.25rem;border-bottom-right-radius:.25rem}.rounded-s{border-start-start-radius:.25rem;border-end-start-radius:.25rem}.rounded-t{border-top-left-radius:.25rem;border-top-right-radius:.25rem}.rounded-bl{border-bottom-left-radius:.25rem}.rounded-br{border-bottom-right-radius:.25rem}.rounded-ee{border-end-end-radius:.25rem}.rounded-es{border-end-start-radius:.25rem}.rounded-se{border-start-end-radius:.25rem}.rounded-ss{border-start-start-radius:.25rem}.rounded-tl{border-top-left-radius:.25rem}.rounded-tr{border-top-right-radius:.25rem}.border{border-width:1px}.border-x{border-left-width:1px;border-right-width:1px}.border-y{border-top-width:1px;border-bottom-width:1px}.border-b{border-bottom-width:1px}.border-e{border-inline-end-width:1px}.border-l{border-left-width:1px}.border-r{border-right-width:1px}.border-s{border-inline-start-width:1px}.border-t{border-top-width:1px}.border-solid{border-style:solid}.border-dashed{border-style:dashed}.border-dotted{border-style:dotted}.border-double{border-style:double}.border-hidden{border-style:hidden}.border-none{border-style:none}.bg-\[rgb\(255\,0\,0\)\]{--tw-bg-opacity: 1;background-color:rgb(255 0 0 / var(--tw-bg-opacity))}.decoration-slice{-webkit-box-decoration-break:slice;box-decoration-break:slice}.decoration-clone{-webkit-box-decoration-break:clone;box-decoration-break:clone}.box-decoration-slice{-webkit-box-decoration-break:slice;box-decoration-break:slice}.box-decoration-clone{-webkit-box-decoration-break:clone;box-decoration-break:clone}.bg-fixed{background-attachment:fixed}.bg-local{background-attachment:local}.bg-scroll{background-attachment:scroll}.bg-clip-border{background-clip:border-box}.bg-clip-padding{background-clip:padding-box}.bg-clip-content{background-clip:content-box}.bg-clip-text{-webkit-background-clip:text;background-clip:text}.bg-repeat{background-repeat:repeat}.bg-no-repeat{background-repeat:no-repeat}.bg-repeat-x{background-repeat:repeat-x}.bg-repeat-y{background-repeat:repeat-y}.bg-repeat-round{background-repeat:round}.bg-repeat-space{background-repeat:space}.bg-origin-border{background-origin:border-box}.bg-origin-padding{background-origin:padding-box}.bg-origin-content{background-origin:content-box}.object-contain{-o-object-fit:contain;object-fit:contain}.object-cover{-o-object-fit:cover;object-fit:cover}.object-fill{-o-object-fit:fill;object-fit:fill}.object-none{-o-object-fit:none;object-fit:none}.object-scale-down{-o-object-fit:scale-down;object-fit:scale-down}.pt-2{padding-top:.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-right{text-align:right}.text-justify{text-align:justify}.text-start{text-align:start}.text-end{text-align:end}.align-baseline{vertical-align:baseline}.align-top{vertical-align:top}.align-middle{vertical-align:middle}.align-bottom{vertical-align:bottom}.align-text-top{vertical-align:text-top}.align-text-bottom{vertical-align:text-bottom}.align-sub{vertical-align:sub}.align-super{vertical-align:super}.font-bold{font-weight:700}.uppercase{text-transform:uppercase}.lowercase{text-transform:lowercase}.capitalize{text-transform:capitalize}.normal-case{text-transform:none}.italic{font-style:italic}.not-italic{font-style:normal}.normal-nums{font-variant-numeric:normal}.ordinal{--tw-ordinal: ordinal;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.slashed-zero{--tw-slashed-zero: slashed-zero;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.lining-nums{--tw-numeric-figure: lining-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.oldstyle-nums{--tw-numeric-figure: oldstyle-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.proportional-nums{--tw-numeric-spacing: proportional-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.tabular-nums{--tw-numeric-spacing: tabular-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.diagonal-fractions{--tw-numeric-fraction: diagonal-fractions;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.stacked-fractions{--tw-numeric-fraction: stacked-fractions;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.text-\[\#336699\]\/\[\.35\]{color:#33669959}.text-blue-500{--tw-text-opacity: 1;color:rgb(59 130 246 / var(--tw-text-opacity))}.underline{text-decoration-line:underline}.overline{text-decoration-line:overline}.line-through{text-decoration-line:line-through}.no-underline{text-decoration-line:none}.decoration-solid{text-decoration-style:solid}.decoration-double{text-decoration-style:double}.decoration-dotted{text-decoration-style:dotted}.decoration-dashed{text-decoration-style:dashed}.decoration-wavy{text-decoration-style:wavy}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.subpixel-antialiased{-webkit-font-smoothing:auto;-moz-osx-font-smoothing:auto}.bg-blend-normal{background-blend-mode:normal}.bg-blend-multiply{background-blend-mode:multiply}.bg-blend-screen{background-blend-mode:screen}.bg-blend-overlay{background-blend-mode:overlay}.bg-blend-darken{background-blend-mode:darken}.bg-blend-lighten{background-blend-mode:lighten}.bg-blend-color-dodge{background-blend-mode:color-dodge}.bg-blend-color-burn{background-blend-mode:color-burn}.bg-blend-hard-light{background-blend-mode:hard-light}.bg-blend-soft-light{background-blend-mode:soft-light}.bg-blend-difference{background-blend-mode:difference}.bg-blend-exclusion{background-blend-mode:exclusion}.bg-blend-hue{background-blend-mode:hue}.bg-blend-saturation{background-blend-mode:saturation}.bg-blend-color{background-blend-mode:color}.bg-blend-luminosity{background-blend-mode:luminosity}.mix-blend-normal{mix-blend-mode:normal}.mix-blend-multiply{mix-blend-mode:multiply}.mix-blend-screen{mix-blend-mode:screen}.mix-blend-overlay{mix-blend-mode:overlay}.mix-blend-darken{mix-blend-mode:darken}.mix-blend-lighten{mix-blend-mode:lighten}.mix-blend-color-dodge{mix-blend-mode:color-dodge}.mix-blend-color-burn{mix-blend-mode:color-burn}.mix-blend-hard-light{mix-blend-mode:hard-light}.mix-blend-soft-light{mix-blend-mode:soft-light}.mix-blend-difference{mix-blend-mode:difference}.mix-blend-exclusion{mix-blend-mode:exclusion}.mix-blend-hue{mix-blend-mode:hue}.mix-blend-saturation{mix-blend-mode:saturation}.mix-blend-color{mix-blend-mode:color}.mix-blend-luminosity{mix-blend-mode:luminosity}.mix-blend-plus-darker{mix-blend-mode:plus-darker}.mix-blend-plus-lighter{mix-blend-mode:plus-lighter}.\!shadow{--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow{--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.outline-none{outline:2px solid transparent;outline-offset:2px}.outline{outline-style:solid}.outline-dashed{outline-style:dashed}.outline-dotted{outline-style:dotted}.outline-double{outline-style:double}.ring{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.ring-inset{--tw-ring-inset: inset}.blur{--tw-blur: blur(8px);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.drop-shadow{--tw-drop-shadow: drop-shadow(0 1px 2px rgb(0 0 0 / .1)) drop-shadow(0 1px 1px rgb(0 0 0 / .06));filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.grayscale{--tw-grayscale: grayscale(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.invert{--tw-invert: invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.sepia{--tw-sepia: sepia(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.\!filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)!important}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.filter-none{filter:none}.backdrop-blur{--tw-backdrop-blur: blur(8px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-grayscale{--tw-backdrop-grayscale: grayscale(100%);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-invert{--tw-backdrop-invert: invert(100%);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-sepia{--tw-backdrop-sepia: sepia(100%);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-filter{-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-filter-none{-webkit-backdrop-filter:none;backdrop-filter:none}.transition{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.ease-in{transition-timing-function:cubic-bezier(.4,0,1,1)}.ease-in-out{transition-timing-function:cubic-bezier(.4,0,.2,1)}.ease-out{transition-timing-function:cubic-bezier(0,0,.2,1)}.contain-none{contain:none}.contain-content{contain:content}.contain-strict{contain:strict}.contain-size{--tw-contain-size: size;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-inline-size{--tw-contain-size: inline-size;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-layout{--tw-contain-layout: layout;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-paint{--tw-contain-paint: paint;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-style{--tw-contain-style: style;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.content-\[\'this-is-also-valid\]-weirdly-enough\'\]{--tw-content: "this-is-also-valid]-weirdly-enough";content:var(--tw-content)}.forced-color-adjust-auto{forced-color-adjust:auto}.forced-color-adjust-none{forced-color-adjust:none}.\[vite\:css\]{vite:css}.\[vite\:html\]{vite:html}[data-theme=normal]{--html-body-bg-color: #373737;--html-default-text-color: #0b0b0b}body{display:flex;height:100vh;align-items:center;justify-content:center;background-color:var(--html-body-bg-color);color:var(--html-default-text-color)}.container{display:flex;flex-direction:column;align-items:center;justify-content:center;border-radius:.5rem;padding:1.5rem;--tw-shadow: 0 25px 50px -12px rgb(0 0 0 / .25);--tw-shadow-colored: 0 25px 50px -12px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);background:#eeeeee}h1{font-size:1.875rem;line-height:2.25rem;font-weight:700}@media (min-width: 640px){.sm\:container{width:100%}@media (min-width: 640px){.sm\:container{max-width:640px}}@media (min-width: 768px){.sm\:container{max-width:768px}}@media (min-width: 1024px){.sm\:container{max-width:1024px}}@media (min-width: 1280px){.sm\:container{max-width:1280px}}@media (min-width: 1536px){.sm\:container{max-width:1536px}}}.hover\:font-bold:hover{font-weight:700}.before\:hover\:text-center:hover:before{content:var(--tw-content);text-align:center}.hover\:before\:text-center:hover:before{content:var(--tw-content);text-align:center}.focus\:hover\:text-center:hover:focus{text-align:center}.hover\:focus\:text-center:focus:hover{text-align:center}@media (min-width: 640px){.sm\:underline{text-decoration-line:underline}}@media (prefers-color-scheme: dark){@media (min-width: 1024px){.dark\:lg\:hover\:\[paint-order\:markers\]:hover{paint-order:markers}}}
+*,:before,:after{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}:before,:after{--tw-content: ""}html,:host{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,sans-serif,"Apple Color Emoji","Segoe UI Emoji",Segoe UI Symbol,"Noto Color Emoji";font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,samp,pre{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dl,dd,h1,h2,h3,h4,h5,h6,hr,figure,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}ol,ul,menu{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}button,[role=button]{cursor:pointer}:disabled{cursor:default}img,svg,video,canvas,audio,iframe,embed,object{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,:before,:after{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x: 0;--tw-border-spacing-y: 0;--tw-translate-x: 0;--tw-translate-y: 0;--tw-rotate: 0;--tw-skew-x: 0;--tw-skew-y: 0;--tw-scale-x: 1;--tw-scale-y: 1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness: proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width: 0px;--tw-ring-offset-color: #fff;--tw-ring-color: rgb(59 130 246 / .5);--tw-ring-offset-shadow: 0 0 #0000;--tw-ring-shadow: 0 0 #0000;--tw-shadow: 0 0 #0000;--tw-shadow-colored: 0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.container{width:100%}@media (min-width: 640px){.container{max-width:640px}}@media (min-width: 768px){.container{max-width:768px}}@media (min-width: 1024px){.container{max-width:1024px}}@media (min-width: 1280px){.container{max-width:1280px}}@media (min-width: 1536px){.container{max-width:1536px}}.sr-only{position:absolute;width:1px;height:1px;padding:0;margin:-1px;overflow:hidden;clip:rect(0,0,0,0);white-space:nowrap;border-width:0}.not-sr-only{position:static;width:auto;height:auto;padding:0;margin:0;overflow:visible;clip:auto;white-space:normal}.pointer-events-none{pointer-events:none}.pointer-events-auto{pointer-events:auto}.\!visible{visibility:visible!important}.visible{visibility:visible}.invisible{visibility:hidden}.collapse{visibility:collapse}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.\!relative{position:relative!important}.relative{position:relative}.sticky{position:sticky}.-inset-1{inset:-.25rem}.end-1{inset-inline-end:.25rem}.isolate{isolation:isolate}.isolation-auto{isolation:auto}.float-start{float:inline-start}.float-end{float:inline-end}.float-right{float:right}.float-left{float:left}.float-none{float:none}.clear-start{clear:inline-start}.clear-end{clear:inline-end}.clear-left{clear:left}.clear-right{clear:right}.clear-both{clear:both}.clear-none{clear:none}.mt-2{margin-top:.5rem}.mt-4{margin-top:1rem}.box-border{box-sizing:border-box}.box-content{box-sizing:content-box}.line-clamp-none{overflow:visible;display:block;-webkit-box-orient:horizontal;-webkit-line-clamp:none}.block{display:block}.inline-block{display:inline-block}.\!inline{display:inline!important}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.inline-table{display:inline-table}.table-caption{display:table-caption}.table-cell{display:table-cell}.table-column{display:table-column}.table-column-group{display:table-column-group}.table-footer-group{display:table-footer-group}.table-header-group{display:table-header-group}.table-row-group{display:table-row-group}.table-row{display:table-row}.flow-root{display:flow-root}.grid{display:grid}.inline-grid{display:inline-grid}.contents{display:contents}.list-item{display:list-item}.hidden{display:none}.w-\[this-is\\\\\]{width:this-is\\}.w-\[this-is\]{width:this-is}.w-\[weird-and-invalid\]{width:weird-and-invalid}.flex-shrink,.shrink{flex-shrink:1}.flex-grow,.grow{flex-grow:1}.table-auto{table-layout:auto}.table-fixed{table-layout:fixed}.caption-top{caption-side:top}.caption-bottom{caption-side:bottom}.border-collapse{border-collapse:collapse}.border-separate{border-collapse:separate}.\!transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))!important}.transform,.transform-cpu{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform-gpu{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skew(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform-none{transform:none}.touch-auto{touch-action:auto}.touch-none{touch-action:none}.touch-pan-x{--tw-pan-x: pan-x;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-left{--tw-pan-x: pan-left;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-right{--tw-pan-x: pan-right;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-y{--tw-pan-y: pan-y;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-up{--tw-pan-y: pan-up;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pan-down{--tw-pan-y: pan-down;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-pinch-zoom{--tw-pinch-zoom: pinch-zoom;touch-action:var(--tw-pan-x) var(--tw-pan-y) var(--tw-pinch-zoom)}.touch-manipulation{touch-action:manipulation}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.select-text{-webkit-user-select:text;-moz-user-select:text;user-select:text}.select-all{-webkit-user-select:all;-moz-user-select:all;user-select:all}.select-auto{-webkit-user-select:auto;-moz-user-select:auto;user-select:auto}.resize-none{resize:none}.resize-y{resize:vertical}.resize-x{resize:horizontal}.resize{resize:both}.snap-none{scroll-snap-type:none}.snap-x{scroll-snap-type:x var(--tw-scroll-snap-strictness)}.snap-y{scroll-snap-type:y var(--tw-scroll-snap-strictness)}.snap-both{scroll-snap-type:both var(--tw-scroll-snap-strictness)}.snap-mandatory{--tw-scroll-snap-strictness: mandatory}.snap-proximity{--tw-scroll-snap-strictness: proximity}.snap-start{scroll-snap-align:start}.snap-end{scroll-snap-align:end}.snap-center{scroll-snap-align:center}.snap-align-none{scroll-snap-align:none}.snap-normal{scroll-snap-stop:normal}.snap-always{scroll-snap-stop:always}.list-inside{list-style-position:inside}.list-outside{list-style-position:outside}.appearance-none{-webkit-appearance:none;-moz-appearance:none;appearance:none}.appearance-auto{-webkit-appearance:auto;-moz-appearance:auto;appearance:auto}.break-before-auto{-moz-column-break-before:auto;break-before:auto}.break-before-avoid{-moz-column-break-before:avoid;break-before:avoid}.break-before-all{-moz-column-break-before:all;break-before:all}.break-before-avoid-page{-moz-column-break-before:avoid;break-before:avoid-page}.break-before-page{-moz-column-break-before:page;break-before:page}.break-before-left{-moz-column-break-before:left;break-before:left}.break-before-right{-moz-column-break-before:right;break-before:right}.break-before-column{-moz-column-break-before:column;break-before:column}.break-inside-auto{-moz-column-break-inside:auto;break-inside:auto}.break-inside-avoid{-moz-column-break-inside:avoid;break-inside:avoid}.break-inside-avoid-page{break-inside:avoid-page}.break-inside-avoid-column{-moz-column-break-inside:avoid;break-inside:avoid-column}.break-after-auto{-moz-column-break-after:auto;break-after:auto}.break-after-avoid{-moz-column-break-after:avoid;break-after:avoid}.break-after-all{-moz-column-break-after:all;break-after:all}.break-after-avoid-page{-moz-column-break-after:avoid;break-after:avoid-page}.break-after-page{-moz-column-break-after:page;break-after:page}.break-after-left{-moz-column-break-after:left;break-after:left}.break-after-right{-moz-column-break-after:right;break-after:right}.break-after-column{-moz-column-break-after:column;break-after:column}.grid-flow-row{grid-auto-flow:row}.grid-flow-col{grid-auto-flow:column}.grid-flow-dense{grid-auto-flow:dense}.grid-flow-row-dense{grid-auto-flow:row dense}.grid-flow-col-dense{grid-auto-flow:column dense}.flex-row{flex-direction:row}.flex-row-reverse{flex-direction:row-reverse}.flex-col{flex-direction:column}.flex-col-reverse{flex-direction:column-reverse}.flex-wrap{flex-wrap:wrap}.flex-wrap-reverse{flex-wrap:wrap-reverse}.flex-nowrap{flex-wrap:nowrap}.place-content-center{place-content:center}.place-content-start{place-content:start}.place-content-end{place-content:end}.place-content-between{place-content:space-between}.place-content-around{place-content:space-around}.place-content-evenly{place-content:space-evenly}.place-content-baseline{place-content:baseline}.place-content-stretch{place-content:stretch}.place-items-start{place-items:start}.place-items-end{place-items:end}.place-items-center{place-items:center}.place-items-baseline{place-items:baseline}.place-items-stretch{place-items:stretch}.content-normal{align-content:normal}.content-center{align-content:center}.content-start{align-content:flex-start}.content-end{align-content:flex-end}.content-between{align-content:space-between}.content-around{align-content:space-around}.content-evenly{align-content:space-evenly}.content-baseline{align-content:baseline}.content-stretch{align-content:stretch}.items-start{align-items:flex-start}.items-end{align-items:flex-end}.items-center{align-items:center}.items-baseline{align-items:baseline}.items-stretch{align-items:stretch}.justify-normal{justify-content:normal}.justify-start{justify-content:flex-start}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.justify-around{justify-content:space-around}.justify-evenly{justify-content:space-evenly}.justify-stretch{justify-content:stretch}.justify-items-start{justify-items:start}.justify-items-end{justify-items:end}.justify-items-center{justify-items:center}.justify-items-stretch{justify-items:stretch}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 0;margin-right:calc(.5rem * var(--tw-space-x-reverse));margin-left:calc(.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-reverse>:not([hidden])~:not([hidden]){--tw-space-y-reverse: 1}.space-x-reverse>:not([hidden])~:not([hidden]){--tw-space-x-reverse: 1}.divide-x>:not([hidden])~:not([hidden]){--tw-divide-x-reverse: 0;border-right-width:calc(1px * var(--tw-divide-x-reverse));border-left-width:calc(1px * calc(1 - var(--tw-divide-x-reverse)))}.divide-y>:not([hidden])~:not([hidden]){--tw-divide-y-reverse: 0;border-top-width:calc(1px * calc(1 - var(--tw-divide-y-reverse)));border-bottom-width:calc(1px * var(--tw-divide-y-reverse))}.divide-y-reverse>:not([hidden])~:not([hidden]){--tw-divide-y-reverse: 1}.divide-x-reverse>:not([hidden])~:not([hidden]){--tw-divide-x-reverse: 1}.divide-solid>:not([hidden])~:not([hidden]){border-style:solid}.divide-dashed>:not([hidden])~:not([hidden]){border-style:dashed}.divide-dotted>:not([hidden])~:not([hidden]){border-style:dotted}.divide-double>:not([hidden])~:not([hidden]){border-style:double}.divide-none>:not([hidden])~:not([hidden]){border-style:none}.place-self-auto{place-self:auto}.place-self-start{place-self:start}.place-self-end{place-self:end}.place-self-center{place-self:center}.place-self-stretch{place-self:stretch}.self-auto{align-self:auto}.self-start{align-self:flex-start}.self-end{align-self:flex-end}.self-center{align-self:center}.self-stretch{align-self:stretch}.self-baseline{align-self:baseline}.justify-self-auto{justify-self:auto}.justify-self-start{justify-self:start}.justify-self-end{justify-self:end}.justify-self-center{justify-self:center}.justify-self-stretch{justify-self:stretch}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-clip{overflow:clip}.overflow-visible{overflow:visible}.overflow-scroll{overflow:scroll}.overflow-x-auto{overflow-x:auto}.overflow-y-auto{overflow-y:auto}.overflow-x-hidden{overflow-x:hidden}.overflow-y-hidden{overflow-y:hidden}.overflow-x-clip{overflow-x:clip}.overflow-y-clip{overflow-y:clip}.overflow-x-visible{overflow-x:visible}.overflow-y-visible{overflow-y:visible}.overflow-x-scroll{overflow-x:scroll}.overflow-y-scroll{overflow-y:scroll}.overscroll-auto{overscroll-behavior:auto}.overscroll-contain{overscroll-behavior:contain}.overscroll-none{overscroll-behavior:none}.overscroll-y-auto{overscroll-behavior-y:auto}.overscroll-y-contain{overscroll-behavior-y:contain}.overscroll-y-none{overscroll-behavior-y:none}.overscroll-x-auto{overscroll-behavior-x:auto}.overscroll-x-contain{overscroll-behavior-x:contain}.overscroll-x-none{overscroll-behavior-x:none}.scroll-auto{scroll-behavior:auto}.scroll-smooth{scroll-behavior:smooth}.truncate{overflow:hidden;text-overflow:ellipsis;white-space:nowrap}.overflow-ellipsis,.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.hyphens-none{-webkit-hyphens:none;hyphens:none}.hyphens-manual{-webkit-hyphens:manual;hyphens:manual}.hyphens-auto{-webkit-hyphens:auto;hyphens:auto}.whitespace-normal{white-space:normal}.whitespace-nowrap{white-space:nowrap}.whitespace-pre{white-space:pre}.whitespace-pre-line{white-space:pre-line}.whitespace-pre-wrap{white-space:pre-wrap}.whitespace-break-spaces{white-space:break-spaces}.text-wrap{text-wrap:wrap}.text-nowrap{text-wrap:nowrap}.text-balance{text-wrap:balance}.text-pretty{text-wrap:pretty}.break-normal{overflow-wrap:normal;word-break:normal}.break-words{overflow-wrap:break-word}.break-all{word-break:break-all}.break-keep{word-break:keep-all}.rounded{border-radius:.25rem}.rounded-b{border-bottom-right-radius:.25rem;border-bottom-left-radius:.25rem}.rounded-e{border-start-end-radius:.25rem;border-end-end-radius:.25rem}.rounded-l{border-top-left-radius:.25rem;border-bottom-left-radius:.25rem}.rounded-r{border-top-right-radius:.25rem;border-bottom-right-radius:.25rem}.rounded-s{border-start-start-radius:.25rem;border-end-start-radius:.25rem}.rounded-t{border-top-left-radius:.25rem;border-top-right-radius:.25rem}.rounded-bl{border-bottom-left-radius:.25rem}.rounded-br{border-bottom-right-radius:.25rem}.rounded-ee{border-end-end-radius:.25rem}.rounded-es{border-end-start-radius:.25rem}.rounded-se{border-start-end-radius:.25rem}.rounded-ss{border-start-start-radius:.25rem}.rounded-tl{border-top-left-radius:.25rem}.rounded-tr{border-top-right-radius:.25rem}.border{border-width:1px}.border-x{border-left-width:1px;border-right-width:1px}.border-y{border-top-width:1px;border-bottom-width:1px}.border-b{border-bottom-width:1px}.border-e{border-inline-end-width:1px}.border-l{border-left-width:1px}.border-r{border-right-width:1px}.border-s{border-inline-start-width:1px}.border-t{border-top-width:1px}.border-solid{border-style:solid}.border-dashed{border-style:dashed}.border-dotted{border-style:dotted}.border-double{border-style:double}.border-hidden{border-style:hidden}.border-none{border-style:none}.bg-\[rgb\(255\,0\,0\)\]{--tw-bg-opacity: 1;background-color:rgb(255 0 0 / var(--tw-bg-opacity))}.decoration-slice{-webkit-box-decoration-break:slice;box-decoration-break:slice}.decoration-clone{-webkit-box-decoration-break:clone;box-decoration-break:clone}.box-decoration-slice{-webkit-box-decoration-break:slice;box-decoration-break:slice}.box-decoration-clone{-webkit-box-decoration-break:clone;box-decoration-break:clone}.bg-fixed{background-attachment:fixed}.bg-local{background-attachment:local}.bg-scroll{background-attachment:scroll}.bg-clip-border{background-clip:border-box}.bg-clip-padding{background-clip:padding-box}.bg-clip-content{background-clip:content-box}.bg-clip-text{-webkit-background-clip:text;background-clip:text}.bg-repeat{background-repeat:repeat}.bg-no-repeat{background-repeat:no-repeat}.bg-repeat-x{background-repeat:repeat-x}.bg-repeat-y{background-repeat:repeat-y}.bg-repeat-round{background-repeat:round}.bg-repeat-space{background-repeat:space}.bg-origin-border{background-origin:border-box}.bg-origin-padding{background-origin:padding-box}.bg-origin-content{background-origin:content-box}.object-contain{-o-object-fit:contain;object-fit:contain}.object-cover{-o-object-fit:cover;object-fit:cover}.object-fill{-o-object-fit:fill;object-fit:fill}.object-none{-o-object-fit:none;object-fit:none}.object-scale-down{-o-object-fit:scale-down;object-fit:scale-down}.pt-2{padding-top:.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-right{text-align:right}.text-justify{text-align:justify}.text-start{text-align:start}.text-end{text-align:end}.align-baseline{vertical-align:baseline}.align-top{vertical-align:top}.align-middle{vertical-align:middle}.align-bottom{vertical-align:bottom}.align-text-top{vertical-align:text-top}.align-text-bottom{vertical-align:text-bottom}.align-sub{vertical-align:sub}.align-super{vertical-align:super}.font-bold{font-weight:700}.uppercase{text-transform:uppercase}.lowercase{text-transform:lowercase}.capitalize{text-transform:capitalize}.normal-case{text-transform:none}.italic{font-style:italic}.not-italic{font-style:normal}.normal-nums{font-variant-numeric:normal}.ordinal{--tw-ordinal: ordinal;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.slashed-zero{--tw-slashed-zero: slashed-zero;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.lining-nums{--tw-numeric-figure: lining-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.oldstyle-nums{--tw-numeric-figure: oldstyle-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.proportional-nums{--tw-numeric-spacing: proportional-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.tabular-nums{--tw-numeric-spacing: tabular-nums;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.diagonal-fractions{--tw-numeric-fraction: diagonal-fractions;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.stacked-fractions{--tw-numeric-fraction: stacked-fractions;font-variant-numeric:var(--tw-ordinal) var(--tw-slashed-zero) var(--tw-numeric-figure) var(--tw-numeric-spacing) var(--tw-numeric-fraction)}.text-\[\#336699\]\/\[\.35\]{color:#33669959}.text-blue-500{--tw-text-opacity: 1;color:rgb(59 130 246 / var(--tw-text-opacity))}.underline{text-decoration-line:underline}.overline{text-decoration-line:overline}.line-through{text-decoration-line:line-through}.no-underline{text-decoration-line:none}.decoration-solid{text-decoration-style:solid}.decoration-double{text-decoration-style:double}.decoration-dotted{text-decoration-style:dotted}.decoration-dashed{text-decoration-style:dashed}.decoration-wavy{text-decoration-style:wavy}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.subpixel-antialiased{-webkit-font-smoothing:auto;-moz-osx-font-smoothing:auto}.bg-blend-normal{background-blend-mode:normal}.bg-blend-multiply{background-blend-mode:multiply}.bg-blend-screen{background-blend-mode:screen}.bg-blend-overlay{background-blend-mode:overlay}.bg-blend-darken{background-blend-mode:darken}.bg-blend-lighten{background-blend-mode:lighten}.bg-blend-color-dodge{background-blend-mode:color-dodge}.bg-blend-color-burn{background-blend-mode:color-burn}.bg-blend-hard-light{background-blend-mode:hard-light}.bg-blend-soft-light{background-blend-mode:soft-light}.bg-blend-difference{background-blend-mode:difference}.bg-blend-exclusion{background-blend-mode:exclusion}.bg-blend-hue{background-blend-mode:hue}.bg-blend-saturation{background-blend-mode:saturation}.bg-blend-color{background-blend-mode:color}.bg-blend-luminosity{background-blend-mode:luminosity}.mix-blend-normal{mix-blend-mode:normal}.mix-blend-multiply{mix-blend-mode:multiply}.mix-blend-screen{mix-blend-mode:screen}.mix-blend-overlay{mix-blend-mode:overlay}.mix-blend-darken{mix-blend-mode:darken}.mix-blend-lighten{mix-blend-mode:lighten}.mix-blend-color-dodge{mix-blend-mode:color-dodge}.mix-blend-color-burn{mix-blend-mode:color-burn}.mix-blend-hard-light{mix-blend-mode:hard-light}.mix-blend-soft-light{mix-blend-mode:soft-light}.mix-blend-difference{mix-blend-mode:difference}.mix-blend-exclusion{mix-blend-mode:exclusion}.mix-blend-hue{mix-blend-mode:hue}.mix-blend-saturation{mix-blend-mode:saturation}.mix-blend-color{mix-blend-mode:color}.mix-blend-luminosity{mix-blend-mode:luminosity}.mix-blend-plus-darker{mix-blend-mode:plus-darker}.mix-blend-plus-lighter{mix-blend-mode:plus-lighter}.\!shadow{--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1) !important;--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color) !important;box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)!important}.shadow{--tw-shadow: 0 1px 3px 0 rgb(0 0 0 / .1), 0 1px 2px -1px rgb(0 0 0 / .1);--tw-shadow-colored: 0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow)}.outline-none{outline:2px solid transparent;outline-offset:2px}.outline{outline-style:solid}.outline-dashed{outline-style:dashed}.outline-dotted{outline-style:dotted}.outline-double{outline-style:double}.ring{--tw-ring-offset-shadow: var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow: var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow, 0 0 #0000)}.ring-inset{--tw-ring-inset: inset}.blur{--tw-blur: blur(8px);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.drop-shadow{--tw-drop-shadow: drop-shadow(0 1px 2px rgb(0 0 0 / .1)) drop-shadow(0 1px 1px rgb(0 0 0 / .06));filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.grayscale{--tw-grayscale: grayscale(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.invert{--tw-invert: invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.sepia{--tw-sepia: sepia(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.\!filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)!important}.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.filter-none{filter:none}.backdrop-blur{--tw-backdrop-blur: blur(8px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-grayscale{--tw-backdrop-grayscale: grayscale(100%);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-invert{--tw-backdrop-invert: invert(100%);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-sepia{--tw-backdrop-sepia: sepia(100%);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-filter{-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-filter-none{-webkit-backdrop-filter:none;backdrop-filter:none}.transition{transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.ease-in{transition-timing-function:cubic-bezier(.4,0,1,1)}.ease-in-out{transition-timing-function:cubic-bezier(.4,0,.2,1)}.ease-out{transition-timing-function:cubic-bezier(0,0,.2,1)}.contain-none{contain:none}.contain-content{contain:content}.contain-strict{contain:strict}.contain-size{--tw-contain-size: size;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-inline-size{--tw-contain-size: inline-size;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-layout{--tw-contain-layout: layout;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-paint{--tw-contain-paint: paint;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.contain-style{--tw-contain-style: style;contain:var(--tw-contain-size) var(--tw-contain-layout) var(--tw-contain-paint) var(--tw-contain-style)}.content-\[\'this-is-also-valid\]-weirdly-enough\'\]{--tw-content: "this-is-also-valid]-weirdly-enough";content:var(--tw-content)}.forced-color-adjust-auto{forced-color-adjust:auto}.forced-color-adjust-none{forced-color-adjust:none}.\[vite\:css\]{vite:css}.\[vite\:html\]{vite:html}[data-theme=normal]{--html-body-bg-color: #373737;--html-default-text-color: #0b0b0b}body{display:flex;height:100vh;align-items:center;justify-content:center;background-color:var(--html-body-bg-color);color:var(--html-default-text-color)}.container{display:flex;flex-direction:column;align-items:center;justify-content:center;border-radius:.5rem;padding:1.5rem;--tw-shadow: 0 25px 50px -12px rgb(0 0 0 / .25);--tw-shadow-colored: 0 25px 50px -12px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000),var(--tw-ring-shadow, 0 0 #0000),var(--tw-shadow);background:#eeeeee}h1{font-size:1.875rem;line-height:2.25rem;font-weight:700}.button{margin:.25rem;border-radius:.5rem;--tw-bg-opacity: 1;background-color:rgb(59 130 246 / var(--tw-bg-opacity));padding:.5rem 1rem;--tw-text-opacity: 1;color:rgb(255 255 255 / var(--tw-text-opacity))}.button:hover{--tw-bg-opacity: 1;background-color:rgb(29 78 216 / var(--tw-bg-opacity))}@media (min-width: 640px){.sm\:container{width:100%}@media (min-width: 640px){.sm\:container{max-width:640px}}@media (min-width: 768px){.sm\:container{max-width:768px}}@media (min-width: 1024px){.sm\:container{max-width:1024px}}@media (min-width: 1280px){.sm\:container{max-width:1280px}}@media (min-width: 1536px){.sm\:container{max-width:1536px}}}.hover\:font-bold:hover{font-weight:700}.before\:hover\:text-center:hover:before{content:var(--tw-content);text-align:center}.hover\:before\:text-center:hover:before{content:var(--tw-content);text-align:center}.focus\:hover\:text-center:hover:focus{text-align:center}.hover\:focus\:text-center:focus:hover{text-align:center}@media (min-width: 640px){.sm\:underline{text-decoration-line:underline}}@media (prefers-color-scheme: dark){@media (min-width: 1024px){.dark\:lg\:hover\:\[paint-order\:markers\]:hover{paint-order:markers}}}
```

### Comparing `vite_transporter-0.4.0/app_quart_demo/vt/app_vite_demo/index-6e585489.js` & `vite_transporter-0.4.1/app_flask_demo/vt/app_vite_demo/index-45b871c7.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,151 +1,151 @@
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
-    for (const s of document.querySelectorAll('link[rel="modulepreload"]')) r(s);
-    new MutationObserver(s => {
-        for (const i of s)
+    for (const r of document.querySelectorAll('link[rel="modulepreload"]')) s(r);
+    new MutationObserver(r => {
+        for (const i of r)
             if (i.type === "childList")
-                for (const l of i.addedNodes) l.tagName === "LINK" && l.rel === "modulepreload" && r(l)
+                for (const l of i.addedNodes) l.tagName === "LINK" && l.rel === "modulepreload" && s(l)
     }).observe(document, {
         childList: !0,
         subtree: !0
     });
 
-    function n(s) {
+    function n(r) {
         const i = {};
-        return s.integrity && (i.integrity = s.integrity), s.referrerPolicy && (i.referrerPolicy = s.referrerPolicy), s.crossOrigin === "use-credentials" ? i.credentials = "include" : s.crossOrigin === "anonymous" ? i.credentials = "omit" : i.credentials = "same-origin", i
+        return r.integrity && (i.integrity = r.integrity), r.referrerPolicy && (i.referrerPolicy = r.referrerPolicy), r.crossOrigin === "use-credentials" ? i.credentials = "include" : r.crossOrigin === "anonymous" ? i.credentials = "omit" : i.credentials = "same-origin", i
     }
 
-    function r(s) {
-        if (s.ep) return;
-        s.ep = !0;
-        const i = n(s);
-        fetch(s.href, i)
+    function s(r) {
+        if (r.ep) return;
+        r.ep = !0;
+        const i = n(r);
+        fetch(r.href, i)
     }
 })();
-const Ie = (e, t) => e === t,
+const Be = (e, t) => e === t,
     se = Symbol("solid-proxy"),
-    X = {
-        equals: Ie
+    H = {
+        equals: Be
     };
-let qe = Pe;
-const L = 1,
-    G = 2,
+let qe = xe;
+const O = 1,
+    Q = 2,
     pe = {
         owned: null,
         cleanups: null,
         context: null,
         owner: null
     };
 var d = null;
 let te = null,
-    Ke = null,
+    Fe = null,
     g = null,
-    A = null,
-    O = null,
+    S = null,
+    R = null,
     Y = 0;
 
 function ge(e, t) {
     const n = g,
-        r = d,
-        s = e.length === 0,
-        i = t === void 0 ? r : t,
-        l = s ? pe : {
+        s = d,
+        r = e.length === 0,
+        i = t === void 0 ? s : t,
+        l = r ? pe : {
             owned: null,
             cleanups: null,
             context: i ? i.context : null,
             owner: i
         },
-        o = s ? e : () => e(() => x(() => z(l)));
+        o = r ? e : () => e(() => P(() => z(l)));
     d = l, g = null;
     try {
         return T(o, !0)
     } finally {
-        g = n, d = r
+        g = n, d = s
     }
 }
 
-function q(e, t) {
-    t = t ? Object.assign({}, X, t) : X;
+function B(e, t) {
+    t = t ? Object.assign({}, H, t) : H;
     const n = {
             value: e,
             observers: null,
             observerSlots: null,
             comparator: t.equals || void 0
         },
-        r = s => (typeof s == "function" && (s = s(n.value)), ve(n, s));
-    return [be.bind(n), r]
+        s = r => (typeof r == "function" && (r = r(n.value)), ve(n, r));
+    return [be.bind(n), s]
 }
 
-function U(e, t, n) {
-    const r = Ae(e, t, !1, L);
-    Z(r)
+function F(e, t, n) {
+    const s = Se(e, t, !1, O);
+    Z(s)
 }
 
-function S(e, t, n) {
-    n = n ? Object.assign({}, X, n) : X;
-    const r = Ae(e, t, !0, 0);
-    return r.observers = null, r.observerSlots = null, r.comparator = n.equals || void 0, Z(r), be.bind(r)
+function A(e, t, n) {
+    n = n ? Object.assign({}, H, n) : H;
+    const s = Se(e, t, !0, 0);
+    return s.observers = null, s.observerSlots = null, s.comparator = n.equals || void 0, Z(s), be.bind(s)
 }
 
-function x(e) {
+function P(e) {
     if (g === null) return e();
     const t = g;
     g = null;
     try {
         return e()
     } finally {
         g = t
     }
 }
 
 function ye(e, t, n) {
-    const r = Array.isArray(e);
-    let s, i = n && n.defer;
+    const s = Array.isArray(e);
+    let r, i = n && n.defer;
     return l => {
         let o;
-        if (r) {
+        if (s) {
             o = Array(e.length);
             for (let a = 0; a < e.length; a++) o[a] = e[a]()
         } else o = e();
         if (i) return i = !1, l;
-        const u = x(() => t(o, s, l));
-        return s = o, u
+        const u = P(() => t(o, r, l));
+        return r = o, u
     }
 }
 
 function me(e) {
     return d === null || (d.cleanups === null ? d.cleanups = [e] : d.cleanups.push(e)), e
 }
 
-function Ue() {
+function De() {
     return d
 }
 
-function De(e, t) {
+function Ke(e, t) {
     const n = d,
-        r = g;
+        s = g;
     d = e, g = null;
     try {
         return T(t, !0)
-    } catch (s) {
-        ce(s)
+    } catch (r) {
+        ce(r)
     } finally {
-        d = n, g = r
+        d = n, g = s
     }
 }
 
-function Fe(e) {
+function Ue(e) {
     const t = g,
         n = d;
     return Promise.resolve().then(() => {
         g = t, d = n;
-        let r;
-        return T(e, !1), g = d = null, r ? r.done : void 0
+        let s;
+        return T(e, !1), g = d = null, s ? s.done : void 0
     })
 }
 
 function we(e, t) {
     const n = Symbol("context");
     return {
         id: n,
@@ -155,151 +155,151 @@
 }
 
 function le(e) {
     return d && d.context && d.context[e.id] !== void 0 ? d.context[e.id] : e.defaultValue
 }
 
 function ue(e) {
-    const t = S(e),
-        n = S(() => oe(t()));
+    const t = A(e),
+        n = A(() => oe(t()));
     return n.toArray = () => {
-        const r = n();
-        return Array.isArray(r) ? r : r != null ? [r] : []
+        const s = n();
+        return Array.isArray(s) ? s : s != null ? [s] : []
     }, n
 }
 
 function be() {
     if (this.sources && this.state)
-        if (this.state === L) Z(this);
+        if (this.state === O) Z(this);
         else {
-            const e = A;
-            A = null, T(() => J(this), !1), A = e
+            const e = S;
+            S = null, T(() => X(this), !1), S = e
         } if (g) {
         const e = this.observers ? this.observers.length : 0;
         g.sources ? (g.sources.push(this), g.sourceSlots.push(e)) : (g.sources = [this], g.sourceSlots = [e]), this.observers ? (this.observers.push(g), this.observerSlots.push(g.sources.length - 1)) : (this.observers = [g], this.observerSlots = [g.sources.length - 1])
     }
     return this.value
 }
 
 function ve(e, t, n) {
-    let r = e.value;
-    return (!e.comparator || !e.comparator(r, t)) && (e.value = t, e.observers && e.observers.length && T(() => {
-        for (let s = 0; s < e.observers.length; s += 1) {
-            const i = e.observers[s],
+    let s = e.value;
+    return (!e.comparator || !e.comparator(s, t)) && (e.value = t, e.observers && e.observers.length && T(() => {
+        for (let r = 0; r < e.observers.length; r += 1) {
+            const i = e.observers[r],
                 l = te && te.running;
-            l && te.disposed.has(i), (l ? !i.tState : !i.state) && (i.pure ? A.push(i) : O.push(i), i.observers && xe(i)), l || (i.state = L)
+            l && te.disposed.has(i), (l ? !i.tState : !i.state) && (i.pure ? S.push(i) : R.push(i), i.observers && Pe(i)), l || (i.state = O)
         }
-        if (A.length > 1e6) throw A = [], new Error
+        if (S.length > 1e6) throw S = [], new Error
     }, !1)), t
 }
 
 function Z(e) {
     if (!e.fn) return;
     z(e);
     const t = Y;
-    ke(e, e.value, t)
+    Me(e, e.value, t)
 }
 
-function ke(e, t, n) {
-    let r;
-    const s = d,
+function Me(e, t, n) {
+    let s;
+    const r = d,
         i = g;
     g = d = e;
     try {
-        r = e.fn(t)
+        s = e.fn(t)
     } catch (l) {
-        return e.pure && (e.state = L, e.owned && e.owned.forEach(z), e.owned = null), e.updatedAt = n + 1, ce(l)
+        return e.pure && (e.state = O, e.owned && e.owned.forEach(z), e.owned = null), e.updatedAt = n + 1, ce(l)
     } finally {
-        g = i, d = s
-    }(!e.updatedAt || e.updatedAt <= n) && (e.updatedAt != null && "observers" in e ? ve(e, r) : e.value = r, e.updatedAt = n)
+        g = i, d = r
+    }(!e.updatedAt || e.updatedAt <= n) && (e.updatedAt != null && "observers" in e ? ve(e, s) : e.value = s, e.updatedAt = n)
 }
 
-function Ae(e, t, n, r = L, s) {
+function Se(e, t, n, s = O, r) {
     const i = {
         fn: e,
-        state: r,
+        state: s,
         updatedAt: null,
         owned: null,
         sources: null,
         sourceSlots: null,
         cleanups: null,
         value: t,
         owner: d,
         context: d ? d.context : null,
         pure: n
     };
     return d === null || d !== pe && (d.owned ? d.owned.push(i) : d.owned = [i]), i
 }
 
-function Se(e) {
+function Ae(e) {
     if (e.state === 0) return;
-    if (e.state === G) return J(e);
-    if (e.suspense && x(e.suspense.inFallback)) return e.suspense.effects.push(e);
+    if (e.state === Q) return X(e);
+    if (e.suspense && P(e.suspense.inFallback)) return e.suspense.effects.push(e);
     const t = [e];
     for (;
         (e = e.owner) && (!e.updatedAt || e.updatedAt < Y);) e.state && t.push(e);
     for (let n = t.length - 1; n >= 0; n--)
-        if (e = t[n], e.state === L) Z(e);
-        else if (e.state === G) {
-        const r = A;
-        A = null, T(() => J(e, t[0]), !1), A = r
+        if (e = t[n], e.state === O) Z(e);
+        else if (e.state === Q) {
+        const s = S;
+        S = null, T(() => X(e, t[0]), !1), S = s
     }
 }
 
 function T(e, t) {
-    if (A) return e();
+    if (S) return e();
     let n = !1;
-    t || (A = []), O ? n = !0 : O = [], Y++;
+    t || (S = []), R ? n = !0 : R = [], Y++;
     try {
-        const r = e();
-        return Me(n), r
-    } catch (r) {
-        n || (O = null), A = null, ce(r)
+        const s = e();
+        return Ge(n), s
+    } catch (s) {
+        n || (R = null), S = null, ce(s)
     }
 }
 
-function Me(e) {
-    if (A && (Pe(A), A = null), e) return;
-    const t = O;
-    O = null, t.length && T(() => qe(t), !1)
+function Ge(e) {
+    if (S && (xe(S), S = null), e) return;
+    const t = R;
+    R = null, t.length && T(() => qe(t), !1)
 }
 
-function Pe(e) {
-    for (let t = 0; t < e.length; t++) Se(e[t])
+function xe(e) {
+    for (let t = 0; t < e.length; t++) Ae(e[t])
 }
 
-function J(e, t) {
+function X(e, t) {
     e.state = 0;
     for (let n = 0; n < e.sources.length; n += 1) {
-        const r = e.sources[n];
-        if (r.sources) {
-            const s = r.state;
-            s === L ? r !== t && (!r.updatedAt || r.updatedAt < Y) && Se(r) : s === G && J(r, t)
+        const s = e.sources[n];
+        if (s.sources) {
+            const r = s.state;
+            r === O ? s !== t && (!s.updatedAt || s.updatedAt < Y) && Ae(s) : r === Q && X(s, t)
         }
     }
 }
 
-function xe(e) {
+function Pe(e) {
     for (let t = 0; t < e.observers.length; t += 1) {
         const n = e.observers[t];
-        n.state || (n.state = G, n.pure ? A.push(n) : O.push(n), n.observers && xe(n))
+        n.state || (n.state = Q, n.pure ? S.push(n) : R.push(n), n.observers && Pe(n))
     }
 }
 
 function z(e) {
     let t;
     if (e.sources)
         for (; e.sources.length;) {
             const n = e.sources.pop(),
-                r = e.sourceSlots.pop(),
-                s = n.observers;
-            if (s && s.length) {
-                const i = s.pop(),
+                s = e.sourceSlots.pop(),
+                r = n.observers;
+            if (r && r.length) {
+                const i = r.pop(),
                     l = n.observerSlots.pop();
-                r < s.length && (i.sourceSlots[l] = r, s[r] = i, n.observerSlots[r] = l)
+                s < r.length && (i.sourceSlots[l] = s, r[s] = i, n.observerSlots[s] = l)
             }
         }
     if (e.owned) {
         for (t = e.owned.length - 1; t >= 0; t--) z(e.owned[t]);
         e.owned = null
     }
     if (e.cleanups) {
@@ -320,80 +320,80 @@
 }
 
 function oe(e) {
     if (typeof e == "function" && !e.length) return oe(e());
     if (Array.isArray(e)) {
         const t = [];
         for (let n = 0; n < e.length; n++) {
-            const r = oe(e[n]);
-            Array.isArray(r) ? t.push.apply(t, r) : t.push(r)
+            const s = oe(e[n]);
+            Array.isArray(s) ? t.push.apply(t, s) : t.push(s)
         }
         return t
     }
     return e
 }
 
 function Ve(e, t) {
-    return function(r) {
-        let s;
-        return U(() => s = x(() => (d.context = {
+    return function(s) {
+        let r;
+        return F(() => r = P(() => (d.context = {
             ...d.context,
-            [e]: r.value
-        }, ue(() => r.children))), void 0), s
+            [e]: s.value
+        }, ue(() => s.children))), void 0), r
     }
 }
 
-function P(e, t) {
-    return x(() => e(t || {}))
+function x(e, t) {
+    return P(() => e(t || {}))
 }
 
-function V() {
+function W() {
     return !0
 }
 const He = {
     get(e, t, n) {
         return t === se ? n : e.get(t)
     },
     has(e, t) {
         return t === se ? !0 : e.has(t)
     },
-    set: V,
-    deleteProperty: V,
+    set: W,
+    deleteProperty: W,
     getOwnPropertyDescriptor(e, t) {
         return {
             configurable: !0,
             enumerable: !0,
             get() {
                 return e.get(t)
             },
-            set: V,
-            deleteProperty: V
+            set: W,
+            deleteProperty: W
         }
     },
     ownKeys(e) {
         return e.keys()
     }
 };
 
 function ne(e) {
     return (e = typeof e == "function" ? e() : e) ? e : {}
 }
 
-function Xe() {
+function Qe() {
     for (let e = 0, t = this.length; e < t; ++e) {
         const n = this[e]();
         if (n !== void 0) return n
     }
 }
 
-function Ge(...e) {
+function Xe(...e) {
     let t = !1;
     for (let l = 0; l < e.length; l++) {
         const o = e[l];
-        t = t || !!o && se in o, e[l] = typeof o == "function" ? (t = !0, S(o)) : o
+        t = t || !!o && se in o, e[l] = typeof o == "function" ? (t = !0, A(o)) : o
     }
     if (t) return new Proxy({
         get(l) {
             for (let o = e.length - 1; o >= 0; o--) {
                 const u = ne(e[o])[l];
                 if (u !== void 0) return u
             }
@@ -406,251 +406,251 @@
         keys() {
             const l = [];
             for (let o = 0; o < e.length; o++) l.push(...Object.keys(ne(e[o])));
             return [...new Set(l)]
         }
     }, He);
     const n = {},
-        r = Object.create(null);
+        s = Object.create(null);
     for (let l = e.length - 1; l >= 0; l--) {
         const o = e[l];
         if (!o) continue;
         const u = Object.getOwnPropertyNames(o);
         for (let a = u.length - 1; a >= 0; a--) {
             const c = u[a];
             if (c === "__proto__" || c === "constructor") continue;
             const f = Object.getOwnPropertyDescriptor(o, c);
-            if (!r[c]) r[c] = f.get ? {
+            if (!s[c]) s[c] = f.get ? {
                 enumerable: !0,
                 configurable: !0,
-                get: Xe.bind(n[c] = [f.get.bind(o)])
+                get: Qe.bind(n[c] = [f.get.bind(o)])
             } : f.value !== void 0 ? f : void 0;
             else {
                 const h = n[c];
                 h && (f.get ? h.push(f.get.bind(o)) : f.value !== void 0 && h.push(() => f.value))
             }
         }
     }
-    const s = {},
-        i = Object.keys(r);
+    const r = {},
+        i = Object.keys(s);
     for (let l = i.length - 1; l >= 0; l--) {
         const o = i[l],
-            u = r[o];
-        u && u.get ? Object.defineProperty(s, o, u) : s[o] = u ? u.value : void 0
+            u = s[o];
+        u && u.get ? Object.defineProperty(r, o, u) : r[o] = u ? u.value : void 0
     }
-    return s
+    return r
 }
 const Je = e => `Stale read from <${e}>.`;
 
 function Ee(e) {
     const t = e.keyed,
-        n = S(() => e.when, void 0, {
-            equals: (r, s) => t ? r === s : !r == !s
+        n = A(() => e.when, void 0, {
+            equals: (s, r) => t ? s === r : !s == !r
         });
-    return S(() => {
-        const r = n();
-        if (r) {
-            const s = e.children;
-            return typeof s == "function" && s.length > 0 ? x(() => s(t ? r : () => {
-                if (!x(n)) throw Je("Show");
+    return A(() => {
+        const s = n();
+        if (s) {
+            const r = e.children;
+            return typeof r == "function" && r.length > 0 ? P(() => r(t ? s : () => {
+                if (!P(n)) throw Je("Show");
                 return e.when
-            })) : s
+            })) : r
         }
         return e.fallback
     }, void 0, void 0)
 }
 
-function Qe(e, t, n) {
-    let r = n.length,
-        s = t.length,
-        i = r,
+function Ye(e, t, n) {
+    let s = n.length,
+        r = t.length,
+        i = s,
         l = 0,
         o = 0,
-        u = t[s - 1].nextSibling,
+        u = t[r - 1].nextSibling,
         a = null;
-    for (; l < s || o < i;) {
+    for (; l < r || o < i;) {
         if (t[l] === n[o]) {
             l++, o++;
             continue
         }
-        for (; t[s - 1] === n[i - 1];) s--, i--;
-        if (s === l) {
-            const c = i < r ? o ? n[o - 1].nextSibling : n[i - o] : u;
+        for (; t[r - 1] === n[i - 1];) r--, i--;
+        if (r === l) {
+            const c = i < s ? o ? n[o - 1].nextSibling : n[i - o] : u;
             for (; o < i;) e.insertBefore(n[o++], c)
         } else if (i === o)
-            for (; l < s;)(!a || !a.has(t[l])) && t[l].remove(), l++;
-        else if (t[l] === n[i - 1] && n[o] === t[s - 1]) {
-            const c = t[--s].nextSibling;
-            e.insertBefore(n[o++], t[l++].nextSibling), e.insertBefore(n[--i], c), t[s] = n[i]
+            for (; l < r;)(!a || !a.has(t[l])) && t[l].remove(), l++;
+        else if (t[l] === n[i - 1] && n[o] === t[r - 1]) {
+            const c = t[--r].nextSibling;
+            e.insertBefore(n[o++], t[l++].nextSibling), e.insertBefore(n[--i], c), t[r] = n[i]
         } else {
             if (!a) {
                 a = new Map;
                 let f = o;
                 for (; f < i;) a.set(n[f], f++)
             }
             const c = a.get(t[l]);
             if (c != null)
                 if (o < c && c < i) {
                     let f = l,
                         h = 1,
                         w;
-                    for (; ++f < s && f < i && !((w = a.get(t[f])) == null || w !== c + h);) h++;
+                    for (; ++f < r && f < i && !((w = a.get(t[f])) == null || w !== c + h);) h++;
                     if (h > c - o) {
                         const b = t[l];
                         for (; o < c;) e.insertBefore(n[o++], b)
                     } else e.replaceChild(n[o++], t[l++])
                 } else l++;
             else t[l++].remove()
         }
     }
 }
 const he = "_$DX_DELEGATE";
 
-function Ye(e, t, n, r = {}) {
-    let s;
+function Ze(e, t, n, s = {}) {
+    let r;
     return ge(i => {
-        s = i, t === document ? e() : tt(t, e(), t.firstChild ? null : void 0, n)
-    }, r.owner), () => {
-        s(), t.textContent = ""
+        r = i, t === document ? e() : tt(t, e(), t.firstChild ? null : void 0, n)
+    }, s.owner), () => {
+        r(), t.textContent = ""
     }
 }
 
-function Ze(e, t, n) {
-    let r;
-    const s = () => {
+function ze(e, t, n) {
+    let s;
+    const r = () => {
             const l = document.createElement("template");
             return l.innerHTML = e, n ? l.content.firstChild.firstChild : l.content.firstChild
         },
-        i = t ? () => x(() => document.importNode(r || (r = s()), !0)) : () => (r || (r = s())).cloneNode(!0);
+        i = t ? () => P(() => document.importNode(s || (s = r()), !0)) : () => (s || (s = r())).cloneNode(!0);
     return i.cloneNode = i, i
 }
 
-function ze(e, t = window.document) {
+function Ce(e, t = window.document) {
     const n = t[he] || (t[he] = new Set);
-    for (let r = 0, s = e.length; r < s; r++) {
-        const i = e[r];
+    for (let s = 0, r = e.length; s < r; s++) {
+        const i = e[s];
         n.has(i) || (n.add(i), t.addEventListener(i, nt))
     }
 }
 
 function et(e, t, n) {
     n == null ? e.removeAttribute(t) : e.setAttribute(t, n)
 }
 
-function tt(e, t, n, r) {
-    if (n !== void 0 && !r && (r = []), typeof t != "function") return Q(e, t, r, n);
-    U(s => Q(e, t(), s, n), r)
+function tt(e, t, n, s) {
+    if (n !== void 0 && !s && (s = []), typeof t != "function") return J(e, t, s, n);
+    F(r => J(e, t(), r, n), s)
 }
 
 function nt(e) {
     const t = `$$${e.type}`;
     let n = e.composedPath && e.composedPath()[0] || e.target;
     for (e.target !== n && Object.defineProperty(e, "target", {
             configurable: !0,
             value: n
         }), Object.defineProperty(e, "currentTarget", {
             configurable: !0,
             get() {
                 return n || document
             }
         }); n;) {
-        const r = n[t];
-        if (r && !n.disabled) {
-            const s = n[`${t}Data`];
-            if (s !== void 0 ? r.call(n, s, e) : r.call(n, e), e.cancelBubble) return
+        const s = n[t];
+        if (s && !n.disabled) {
+            const r = n[`${t}Data`];
+            if (r !== void 0 ? s.call(n, r, e) : s.call(n, e), e.cancelBubble) return
         }
         n = n._$host || n.parentNode || n.host
     }
 }
 
-function Q(e, t, n, r, s) {
+function J(e, t, n, s, r) {
     for (; typeof n == "function";) n = n();
     if (t === n) return n;
     const i = typeof t,
-        l = r !== void 0;
+        l = s !== void 0;
     if (e = l && n[0] && n[0].parentNode || e, i === "string" || i === "number")
         if (i === "number" && (t = t.toString()), l) {
             let o = n[0];
-            o && o.nodeType === 3 ? o.data !== t && (o.data = t) : o = document.createTextNode(t), n = N(e, n, r, o)
+            o && o.nodeType === 3 ? o.data !== t && (o.data = t) : o = document.createTextNode(t), n = j(e, n, s, o)
         } else n !== "" && typeof n == "string" ? n = e.firstChild.data = t : n = e.textContent = t;
-    else if (t == null || i === "boolean") n = N(e, n, r);
+    else if (t == null || i === "boolean") n = j(e, n, s);
     else {
-        if (i === "function") return U(() => {
+        if (i === "function") return F(() => {
             let o = t();
             for (; typeof o == "function";) o = o();
-            n = Q(e, o, n, r)
+            n = J(e, o, n, s)
         }), () => n;
         if (Array.isArray(t)) {
             const o = [],
                 u = n && Array.isArray(n);
-            if (ie(o, t, n, s)) return U(() => n = Q(e, o, n, r, !0)), () => n;
+            if (ie(o, t, n, r)) return F(() => n = J(e, o, n, s, !0)), () => n;
             if (o.length === 0) {
-                if (n = N(e, n, r), l) return n
-            } else u ? n.length === 0 ? de(e, o, r) : Qe(e, n, o) : (n && N(e), de(e, o));
+                if (n = j(e, n, s), l) return n
+            } else u ? n.length === 0 ? de(e, o, s) : Ye(e, n, o) : (n && j(e), de(e, o));
             n = o
         } else if (t.nodeType) {
             if (Array.isArray(n)) {
-                if (l) return n = N(e, n, r, t);
-                N(e, n, null, t)
+                if (l) return n = j(e, n, s, t);
+                j(e, n, null, t)
             } else n == null || n === "" || !e.firstChild ? e.appendChild(t) : e.replaceChild(t, e.firstChild);
             n = t
         }
     }
     return n
 }
 
-function ie(e, t, n, r) {
-    let s = !1;
+function ie(e, t, n, s) {
+    let r = !1;
     for (let i = 0, l = t.length; i < l; i++) {
         let o = t[i],
             u = n && n[e.length],
             a;
         if (!(o == null || o === !0 || o === !1))
             if ((a = typeof o) == "object" && o.nodeType) e.push(o);
-            else if (Array.isArray(o)) s = ie(e, o, u) || s;
+            else if (Array.isArray(o)) r = ie(e, o, u) || r;
         else if (a === "function")
-            if (r) {
+            if (s) {
                 for (; typeof o == "function";) o = o();
-                s = ie(e, Array.isArray(o) ? o : [o], Array.isArray(u) ? u : [u]) || s
-            } else e.push(o), s = !0;
+                r = ie(e, Array.isArray(o) ? o : [o], Array.isArray(u) ? u : [u]) || r
+            } else e.push(o), r = !0;
         else {
             const c = String(o);
             u && u.nodeType === 3 && u.data === c ? e.push(u) : e.push(document.createTextNode(c))
         }
     }
-    return s
+    return r
 }
 
 function de(e, t, n = null) {
-    for (let r = 0, s = t.length; r < s; r++) e.insertBefore(t[r], n)
+    for (let s = 0, r = t.length; s < r; s++) e.insertBefore(t[s], n)
 }
 
-function N(e, t, n, r) {
+function j(e, t, n, s) {
     if (n === void 0) return e.textContent = "";
-    const s = r || document.createTextNode("");
+    const r = s || document.createTextNode("");
     if (t.length) {
         let i = !1;
         for (let l = t.length - 1; l >= 0; l--) {
             const o = t[l];
-            if (s !== o) {
+            if (r !== o) {
                 const u = o.parentNode === e;
-                !i && !l ? u ? e.replaceChild(s, o) : e.insertBefore(s, n) : u && o.remove()
+                !i && !l ? u ? e.replaceChild(r, o) : e.insertBefore(r, n) : u && o.remove()
             } else i = !0
         }
-    } else e.insertBefore(s, n);
-    return [s]
+    } else e.insertBefore(r, n);
+    return [r]
 }
 const rt = !1;
 
 function st(e, t, n) {
     return e.addEventListener(t, n), () => e.removeEventListener(t, n)
 }
 
-function ot([e, t], n, r) {
-    return [n ? () => n(e()) : e, r ? s => t(r(s)) : t]
+function ot([e, t], n, s) {
+    return [n ? () => n(e()) : e, s ? r => t(s(r)) : t]
 }
 
 function it(e) {
     if (e === "#") return null;
     try {
         return document.querySelector(e)
     } catch {
@@ -659,168 +659,168 @@
 }
 
 function lt(e, t) {
     const n = it(`#${e}`);
     n ? n.scrollIntoView() : t && window.scrollTo(0, 0)
 }
 
-function ut(e, t, n, r) {
-    let s = !1;
+function ut(e, t, n, s) {
+    let r = !1;
     const i = o => typeof o == "string" ? {
             value: o
         } : o,
-        l = ot(q(i(e()), {
+        l = ot(B(i(e()), {
             equals: (o, u) => o.value === u.value
-        }), void 0, o => (!s && t(o), o));
+        }), void 0, o => (!r && t(o), o));
     return n && me(n((o = e()) => {
-        s = !0, l[1](i(o)), s = !1
+        r = !0, l[1](i(o)), r = !1
     })), {
         signal: l,
-        utils: r
+        utils: s
     }
 }
 
 function ct(e) {
     if (e) {
         if (Array.isArray(e)) return {
             signal: e
         }
     } else return {
-        signal: q({
+        signal: B({
             value: ""
         })
     };
     return e
 }
 
 function at() {
     return ut(() => ({
         value: window.location.pathname + window.location.search + window.location.hash,
         state: history.state
     }), ({
         value: e,
         replace: t,
         scroll: n,
-        state: r
+        state: s
     }) => {
-        t ? window.history.replaceState(r, "", e) : window.history.pushState(r, "", e), lt(window.location.hash.slice(1), n)
+        t ? window.history.replaceState(s, "", e) : window.history.pushState(s, "", e), lt(window.location.hash.slice(1), n)
     }, e => st(window, "popstate", () => e()), {
         go: e => window.history.go(e)
     })
 }
 
 function ft() {
     let e = new Set;
 
-    function t(s) {
-        return e.add(s), () => e.delete(s)
+    function t(r) {
+        return e.add(r), () => e.delete(r)
     }
     let n = !1;
 
-    function r(s, i) {
+    function s(r, i) {
         if (n) return !(n = !1);
         const l = {
-            to: s,
+            to: r,
             options: i,
             defaultPrevented: !1,
             preventDefault: () => l.defaultPrevented = !0
         };
         for (const o of e) o.listener({
             ...l,
             from: o.location,
             retry: u => {
-                u && (n = !0), o.navigate(s, i)
+                u && (n = !0), o.navigate(r, i)
             }
         });
         return !l.defaultPrevented
     }
     return {
         subscribe: t,
-        confirm: r
+        confirm: s
     }
 }
 const ht = /^(?:[a-z0-9]+:)?\/\//i,
     dt = /^\/+|(\/)\/+$/g;
 
-function K(e, t = !1) {
+function q(e, t = !1) {
     const n = e.replace(dt, "$1");
     return n ? t || /^[?#]/.test(n) ? n : "/" + n : ""
 }
 
-function H(e, t, n) {
+function V(e, t, n) {
     if (ht.test(t)) return;
-    const r = K(e),
-        s = n && K(n);
+    const s = q(e),
+        r = n && q(n);
     let i = "";
-    return !s || t.startsWith("/") ? i = r : s.toLowerCase().indexOf(r.toLowerCase()) !== 0 ? i = r + s : i = s, (i || "/") + K(t, !i)
+    return !r || t.startsWith("/") ? i = s : r.toLowerCase().indexOf(s.toLowerCase()) !== 0 ? i = s + r : i = r, (i || "/") + q(t, !i)
 }
 
 function pt(e, t) {
     if (e == null) throw new Error(t);
     return e
 }
 
-function Ce(e, t) {
-    return K(e).replace(/\/*(\*.*)?$/g, "") + K(t)
+function $e(e, t) {
+    return q(e).replace(/\/*(\*.*)?$/g, "") + q(t)
 }
 
 function gt(e) {
     const t = {};
-    return e.searchParams.forEach((n, r) => {
-        t[r] = n
+    return e.searchParams.forEach((n, s) => {
+        t[s] = n
     }), t
 }
 
 function yt(e, t, n) {
-    const [r, s] = e.split("/*", 2), i = r.split("/").filter(Boolean), l = i.length;
+    const [s, r] = e.split("/*", 2), i = s.split("/").filter(Boolean), l = i.length;
     return o => {
         const u = o.split("/").filter(Boolean),
             a = u.length - l;
-        if (a < 0 || a > 0 && s === void 0 && !t) return null;
+        if (a < 0 || a > 0 && r === void 0 && !t) return null;
         const c = {
                 path: l ? "" : "/",
                 params: {}
             },
             f = h => n === void 0 ? void 0 : n[h];
         for (let h = 0; h < l; h++) {
             const w = i[h],
                 b = u[h],
-                m = w[0] === ":",
-                R = m ? w.slice(1) : w;
-            if (m && re(b, f(R))) c.params[R] = b;
-            else if (m || !re(b, w)) return null;
+                y = w[0] === ":",
+                $ = y ? w.slice(1) : w;
+            if (y && re(b, f($))) c.params[$] = b;
+            else if (y || !re(b, w)) return null;
             c.path += `/${b}`
         }
-        if (s) {
+        if (r) {
             const h = a ? u.slice(-a).join("/") : "";
-            if (re(h, f(s))) c.params[s] = h;
+            if (re(h, f(r))) c.params[r] = h;
             else return null
         }
         return c
     }
 }
 
 function re(e, t) {
-    const n = r => r.localeCompare(e, void 0, {
+    const n = s => s.localeCompare(e, void 0, {
         sensitivity: "base"
     }) === 0;
     return t === void 0 ? !0 : typeof t == "string" ? n(t) : typeof t == "function" ? t(e) : Array.isArray(t) ? t.some(n) : t instanceof RegExp ? t.test(e) : !1
 }
 
 function mt(e) {
-    const [t, n] = e.pattern.split("/*", 2), r = t.split("/").filter(Boolean);
-    return r.reduce((s, i) => s + (i.startsWith(":") ? 2 : 3), r.length - (n === void 0 ? 0 : 1))
+    const [t, n] = e.pattern.split("/*", 2), s = t.split("/").filter(Boolean);
+    return s.reduce((r, i) => r + (i.startsWith(":") ? 2 : 3), s.length - (n === void 0 ? 0 : 1))
 }
 
 function Re(e) {
     const t = new Map,
-        n = Ue();
+        n = De();
     return new Proxy({}, {
-        get(r, s) {
-            return t.has(s) || De(n, () => t.set(s, S(() => e()[s]))), t.get(s)()
+        get(s, r) {
+            return t.has(r) || Ke(n, () => t.set(r, A(() => e()[r]))), t.get(r)()
         },
         getOwnPropertyDescriptor() {
             return {
                 enumerable: !0,
                 configurable: !0
             }
         },
@@ -830,45 +830,45 @@
     })
 }
 
 function Oe(e) {
     let t = /(\/?\:[^\/]+)\?/.exec(e);
     if (!t) return [e];
     let n = e.slice(0, t.index),
-        r = e.slice(t.index + t[0].length);
-    const s = [n, n += t[1]];
-    for (; t = /^(\/\:[^\/]+)\?/.exec(r);) s.push(n += t[1]), r = r.slice(t[0].length);
-    return Oe(r).reduce((i, l) => [...i, ...s.map(o => o + l)], [])
+        s = e.slice(t.index + t[0].length);
+    const r = [n, n += t[1]];
+    for (; t = /^(\/\:[^\/]+)\?/.exec(s);) r.push(n += t[1]), s = s.slice(t[0].length);
+    return Oe(s).reduce((i, l) => [...i, ...r.map(o => o + l)], [])
 }
 const wt = 100,
-    Le = we(),
+    Te = we(),
     ee = we(),
-    Te = () => pt(le(Le), "Make sure your app is wrapped in a <Router />");
+    _e = () => pt(le(Te), "Make sure your app is wrapped in a <Router />");
 let D;
-const $e = () => D || le(ee) || Te().base;
+const Le = () => D || le(ee) || _e().base;
 
 function bt(e, t = "", n) {
     const {
-        component: r,
-        data: s,
+        component: s,
+        data: r,
         children: i
     } = e, l = !i || Array.isArray(i) && !i.length, o = {
         key: e,
-        element: r ? () => P(r, {}) : () => {
+        element: s ? () => x(s, {}) : () => {
             const {
                 element: u
             } = e;
-            return u === void 0 && n ? P(n, {}) : u
+            return u === void 0 && n ? x(n, {}) : u
         },
-        preload: e.component ? r.preload : e.preload,
-        data: s
+        preload: e.component ? s.preload : e.preload,
+        data: r
     };
     return je(e.path).reduce((u, a) => {
         for (const c of Oe(a)) {
-            const f = Ce(t, c),
+            const f = $e(t, c),
                 h = l ? f : f.split("/*", 1)[0];
             u.push({
                 ...o,
                 originalPath: c,
                 pattern: h,
                 matcher: yt(h, !l, e.matchFilters)
             })
@@ -878,294 +878,294 @@
 }
 
 function vt(e, t = 0) {
     return {
         routes: e,
         score: mt(e[e.length - 1]) * 1e4 - t,
         matcher(n) {
-            const r = [];
-            for (let s = e.length - 1; s >= 0; s--) {
-                const i = e[s],
+            const s = [];
+            for (let r = e.length - 1; r >= 0; r--) {
+                const i = e[r],
                     l = i.matcher(n);
                 if (!l) return null;
-                r.unshift({
+                s.unshift({
                     ...l,
                     route: i
                 })
             }
-            return r
+            return s
         }
     }
 }
 
 function je(e) {
     return Array.isArray(e) ? e : [e]
 }
 
-function Ne(e, t = "", n, r = [], s = []) {
+function Ie(e, t = "", n, s = [], r = []) {
     const i = je(e);
     for (let l = 0, o = i.length; l < o; l++) {
         const u = i[l];
         if (u && typeof u == "object" && u.hasOwnProperty("path")) {
             const a = bt(u, t, n);
             for (const c of a) {
-                r.push(c);
+                s.push(c);
                 const f = Array.isArray(u.children) && u.children.length === 0;
-                if (u.children && !f) Ne(u.children, c.pattern, n, r, s);
+                if (u.children && !f) Ie(u.children, c.pattern, n, s, r);
                 else {
-                    const h = vt([...r], s.length);
-                    s.push(h)
+                    const h = vt([...s], r.length);
+                    r.push(h)
                 }
-                r.pop()
+                s.pop()
             }
         }
     }
-    return r.length ? s : s.sort((l, o) => o.score - l.score)
+    return s.length ? r : r.sort((l, o) => o.score - l.score)
 }
 
-function At(e, t) {
-    for (let n = 0, r = e.length; n < r; n++) {
-        const s = e[n].matcher(t);
-        if (s) return s
+function St(e, t) {
+    for (let n = 0, s = e.length; n < s; n++) {
+        const r = e[n].matcher(t);
+        if (r) return r
     }
     return []
 }
 
-function St(e, t) {
+function At(e, t) {
     const n = new URL("http://sar"),
-        r = S(u => {
+        s = A(u => {
             const a = e();
             try {
                 return new URL(a, n)
             } catch {
                 return console.error(`Invalid path ${a}`), u
             }
         }, n, {
             equals: (u, a) => u.href === a.href
         }),
-        s = S(() => r().pathname),
-        i = S(() => r().search, !0),
-        l = S(() => r().hash),
-        o = S(() => "");
+        r = A(() => s().pathname),
+        i = A(() => s().search, !0),
+        l = A(() => s().hash),
+        o = A(() => "");
     return {
         get pathname() {
-            return s()
+            return r()
         },
         get search() {
             return i()
         },
         get hash() {
             return l()
         },
         get state() {
             return t()
         },
         get key() {
             return o()
         },
-        query: Re(ye(i, () => gt(r())))
+        query: Re(ye(i, () => gt(s())))
     }
 }
 
-function Pt(e, t = "", n, r) {
+function xt(e, t = "", n, s) {
     const {
-        signal: [s, i],
+        signal: [r, i],
         utils: l = {}
-    } = ct(e), o = l.parsePath || (y => y), u = l.renderPath || (y => y), a = l.beforeLeave || ft(), c = H("", t), f = void 0;
+    } = ct(e), o = l.parsePath || (m => m), u = l.renderPath || (m => m), a = l.beforeLeave || ft(), c = V("", t), f = void 0;
     if (c === void 0) throw new Error(`${c} is not a valid base path`);
-    c && !s().value && i({
+    c && !r().value && i({
         value: c,
         replace: !0,
         scroll: !1
     });
-    const [h, w] = q(!1), b = async y => {
+    const [h, w] = B(!1), b = async m => {
         w(!0);
         try {
-            await Fe(y)
+            await Ue(m)
         } finally {
             w(!1)
         }
-    }, [m, R] = q(s().value), [$, F] = q(s().state), k = St(m, $), B = [], j = {
+    }, [y, $] = B(r().value), [_, K] = B(r().state), U = At(y, _), I = [], L = {
         pattern: c,
         params: {},
         path: () => c,
         outlet: () => null,
-        resolvePath(y) {
-            return H(c, y)
+        resolvePath(m) {
+            return V(c, m)
         }
     };
     if (n) try {
-        D = j, j.data = n({
+        D = L, L.data = n({
             data: void 0,
             params: {},
-            location: k,
-            navigate: fe(j)
+            location: U,
+            navigate: fe(L)
         })
     } finally {
         D = void 0
     }
 
-    function ae(y, p, v) {
-        x(() => {
+    function ae(m, p, v) {
+        P(() => {
             if (typeof p == "number") {
                 p && (l.go ? a.confirm(p, v) && l.go(p) : console.warn("Router integration does not support relative routing"));
                 return
             }
             const {
                 replace: M,
-                resolve: W,
+                resolve: G,
                 scroll: E,
-                state: _
+                state: N
             } = {
                 replace: !1,
                 resolve: !0,
                 scroll: !0,
                 ...v
-            }, C = W ? y.resolvePath(p) : H("", p);
+            }, C = G ? m.resolvePath(p) : V("", p);
             if (C === void 0) throw new Error(`Path '${p}' is not a routable path`);
-            if (B.length >= wt) throw new Error("Too many redirects");
-            const I = m();
-            if ((C !== I || _ !== $()) && !rt) {
+            if (I.length >= wt) throw new Error("Too many redirects");
+            const k = y();
+            if ((C !== k || N !== _()) && !rt) {
                 if (a.confirm(C, v)) {
-                    const _e = B.push({
-                        value: I,
+                    const ke = I.push({
+                        value: k,
                         replace: M,
                         scroll: E,
-                        state: $()
+                        state: _()
                     });
                     b(() => {
-                        R(C), F(_)
+                        $(C), K(N)
                     }).then(() => {
-                        B.length === _e && Be({
+                        I.length === ke && Ne({
                             value: C,
-                            state: _
+                            state: N
                         })
                     })
                 }
             }
         })
     }
 
-    function fe(y) {
-        return y = y || le(ee) || j, (p, v) => ae(y, p, v)
+    function fe(m) {
+        return m = m || le(ee) || L, (p, v) => ae(m, p, v)
     }
 
-    function Be(y) {
-        const p = B[0];
-        p && ((y.value !== p.value || y.state !== p.state) && i({
-            ...y,
+    function Ne(m) {
+        const p = I[0];
+        p && ((m.value !== p.value || m.state !== p.state) && i({
+            ...m,
             replace: p.replace,
             scroll: p.scroll
-        }), B.length = 0)
+        }), I.length = 0)
     }
-    U(() => {
+    F(() => {
         const {
-            value: y,
+            value: m,
             state: p
-        } = s();
-        x(() => {
-            y !== m() && b(() => {
-                R(y), F(p)
+        } = r();
+        P(() => {
+            m !== y() && b(() => {
+                $(m), K(p)
             })
         })
     });
     {
-        let y = function(p) {
+        let m = function(p) {
             if (p.defaultPrevented || p.button !== 0 || p.metaKey || p.altKey || p.ctrlKey || p.shiftKey) return;
-            const v = p.composedPath().find(I => I instanceof Node && I.nodeName.toUpperCase() === "A");
+            const v = p.composedPath().find(k => k instanceof Node && k.nodeName.toUpperCase() === "A");
             if (!v || !v.hasAttribute("link")) return;
             const M = v.href;
             if (v.target || !M && !v.hasAttribute("state")) return;
-            const W = (v.getAttribute("rel") || "").split(/\s+/);
-            if (v.hasAttribute("download") || W && W.includes("external")) return;
+            const G = (v.getAttribute("rel") || "").split(/\s+/);
+            if (v.hasAttribute("download") || G && G.includes("external")) return;
             const E = new URL(M);
             if (E.origin !== window.location.origin || c && E.pathname && !E.pathname.toLowerCase().startsWith(c.toLowerCase())) return;
-            const _ = o(E.pathname + E.search + E.hash),
+            const N = o(E.pathname + E.search + E.hash),
                 C = v.getAttribute("state");
-            p.preventDefault(), ae(j, _, {
+            p.preventDefault(), ae(L, N, {
                 resolve: !1,
                 replace: v.hasAttribute("replace"),
                 scroll: !v.hasAttribute("noscroll"),
                 state: C && JSON.parse(C)
             })
         };
-        var Nt = y;
-        ze(["click"]), document.addEventListener("click", y), me(() => document.removeEventListener("click", y))
+        var jt = m;
+        Ce(["click"]), document.addEventListener("click", m), me(() => document.removeEventListener("click", m))
     }
     return {
-        base: j,
+        base: L,
         out: f,
-        location: k,
+        location: U,
         isRouting: h,
         renderPath: u,
         parsePath: o,
         navigatorFactory: fe,
         beforeLeave: a
     }
 }
 
-function xt(e, t, n, r, s) {
+function Pt(e, t, n, s, r) {
     const {
         base: i,
         location: l,
         navigatorFactory: o
     } = e, {
         pattern: u,
         element: a,
         preload: c,
         data: f
-    } = r().route, h = S(() => r().path);
+    } = s().route, h = A(() => s().path);
     c && c();
     const w = {
         parent: t,
         pattern: u,
         get child() {
             return n()
         },
         path: h,
-        params: s,
+        params: r,
         data: t.data,
         outlet: a,
         resolvePath(b) {
-            return H(i.path(), b, h())
+            return V(i.path(), b, h())
         }
     };
     if (f) try {
         D = w, w.data = f({
             data: t.data,
-            params: s,
+            params: r,
             location: l,
             navigate: o(w)
         })
     } finally {
         D = void 0
     }
     return w
 }
 const Et = e => {
         const {
             source: t,
             url: n,
-            base: r,
-            data: s,
+            base: s,
+            data: r,
             out: i
-        } = e, l = t || at(), o = Pt(l, r, s);
-        return P(Le.Provider, {
+        } = e, l = t || at(), o = xt(l, s, r);
+        return x(Te.Provider, {
             value: o,
             get children() {
                 return e.children
             }
         })
     },
     Ct = e => {
-        const t = Te(),
-            n = $e(),
-            r = ue(() => e.children),
-            s = S(() => Ne(r(), Ce(n.pattern, e.base || ""), Ot)),
-            i = S(() => At(s(), t.location.pathname)),
+        const t = _e(),
+            n = Le(),
+            s = ue(() => e.children),
+            r = A(() => Ie(s(), $e(n.pattern, e.base || ""), Rt)),
+            i = A(() => St(r(), t.location.pathname)),
             l = Re(() => {
                 const c = i(),
                     f = {};
                 for (let h = 0; h < c.length; h++) Object.assign(f, c[h].params);
                 return f
             });
         t.out && t.out.matches.push(i().map(({
@@ -1176,81 +1176,134 @@
             originalPath: c.originalPath,
             pattern: c.pattern,
             path: f,
             params: h
         })));
         const o = [];
         let u;
-        const a = S(ye(i, (c, f, h) => {
+        const a = A(ye(i, (c, f, h) => {
             let w = f && c.length === f.length;
             const b = [];
-            for (let m = 0, R = c.length; m < R; m++) {
-                const $ = f && f[m],
-                    F = c[m];
-                h && $ && F.route.key === $.route.key ? b[m] = h[m] : (w = !1, o[m] && o[m](), ge(k => {
-                    o[m] = k, b[m] = xt(t, b[m - 1] || n, () => a()[m + 1], () => i()[m], l)
+            for (let y = 0, $ = c.length; y < $; y++) {
+                const _ = f && f[y],
+                    K = c[y];
+                h && _ && K.route.key === _.route.key ? b[y] = h[y] : (w = !1, o[y] && o[y](), ge(U => {
+                    o[y] = U, b[y] = Pt(t, b[y - 1] || n, () => a()[y + 1], () => i()[y], l)
                 }))
             }
-            return o.splice(c.length).forEach(m => m()), h && w ? h : (u = b[0], b)
+            return o.splice(c.length).forEach(y => y()), h && w ? h : (u = b[0], b)
         }));
-        return P(Ee, {
+        return x(Ee, {
             get when() {
                 return a() && u
             },
             keyed: !0,
-            children: c => P(ee.Provider, {
+            children: c => x(ee.Provider, {
                 value: c,
                 get children() {
                     return c.outlet()
                 }
             })
         })
     },
-    Rt = e => {
+    $t = e => {
         const t = ue(() => e.children);
-        return Ge(e, {
+        return Xe(e, {
             get children() {
                 return t()
             }
         })
     },
-    Ot = () => {
-        const e = $e();
-        return P(Ee, {
+    Rt = () => {
+        const e = Le();
+        return x(Ee, {
             get when() {
                 return e.child
             },
             keyed: !0,
-            children: t => P(ee.Provider, {
+            children: t => x(ee.Provider, {
                 value: t,
                 get children() {
                     return t.outlet()
                 }
             })
         })
     },
-    Lt = "/__vt/app_vite_demo/ili-85e34484.gif";
-var Tt = Ze("<div class=container><h1>🚚 Vite-Transporter</h1><p class=pt-2>Image Asset Example</p><p>👇</p><img width=100 alt=ili><small>🥞 Vite, SolidJS, TailwindCSS");
+    Ot = "/__vt/app_vite_demo/ili-85e34484.gif";
+var Tt = ze("<div class=container><h1>🚚 Vite-Transporter</h1><p class=pt-2>Image Asset Example</p><p>👇</p><img width=100 alt=ili><small>🥞 Vite, SolidJS, TailwindCSS</small><hr><small class=mt-4>Demo tests (open browser inspect console)</small><button class=button>API Flask</button><button class=button>API Flask Session</button><button class=button>API Quart</button><button class=button>API Quart Session");
 
-function $t() {
+function _t() {
+    function e() {
+        fetch("http://127.0.0.1:5001/api", {
+            method: "GET",
+            headers: {
+                "Content-Type": "application/json"
+            }
+        }).then(r => r.json()).then(r => {
+            console.log(r)
+        })
+    }
+
+    function t() {
+        fetch("http://127.0.0.1:5001/api/session", {
+            method: "GET",
+            credentials: "include",
+            headers: {
+                "Content-Type": "application/json"
+            }
+        }).then(r => r.json()).then(r => {
+            console.log(r)
+        })
+    }
+
+    function n() {
+        fetch("http://127.0.0.1:5002/api", {
+            method: "GET",
+            headers: {
+                "Content-Type": "application/json"
+            }
+        }).then(r => r.json()).then(r => {
+            console.log(r)
+        })
+    }
+
+    function s() {
+        fetch("http://127.0.0.1:5002/api/session", {
+            method: "GET",
+            credentials: "include",
+            headers: {
+                "Content-Type": "application/json"
+            }
+        }).then(r => r.json()).then(r => {
+            console.log(r)
+        })
+    }
     return (() => {
-        var e = Tt(),
-            t = e.firstChild,
-            n = t.nextSibling,
-            r = n.nextSibling,
-            s = r.nextSibling;
-        return et(s, "src", Lt), e
+        var r = Tt(),
+            i = r.firstChild,
+            l = i.nextSibling,
+            o = l.nextSibling,
+            u = o.nextSibling,
+            a = u.nextSibling,
+            c = a.nextSibling,
+            f = c.nextSibling,
+            h = f.nextSibling,
+            w = h.nextSibling,
+            b = w.nextSibling,
+            y = b.nextSibling;
+        return et(u, "src", Ot), h.$$click = e, w.$$click = t, b.$$click = n, y.$$click = s, r
     })()
 }
-const jt = document.getElementById("root");
-Ye(() => P(Et, {
+Ce(["click"]);
+const Lt = document.getElementById("root");
+Ze(() => x(Et, {
     get children() {
-        return P(Ct, {
+        return x(Ct, {
             get children() {
-                return P(Rt, {
+                return x($t, {
                     path: "/",
-                    component: $t
+                    component: _t
                 })
             }
         })
     }
-}), jt);
+}), Lt);
```

### Comparing `vite_transporter-0.4.0/app_vite_demo/Index.jsx` & `vite_transporter-0.4.1/app_vite_demo/Index.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_vite_demo/__router__.jsx` & `vite_transporter-0.4.1/app_vite_demo/__router__.jsx`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_vite_demo/assets/ili.gif` & `vite_transporter-0.4.1/app_vite_demo/assets/ili.gif`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_vite_demo/index.css` & `vite_transporter-0.4.1/app_vite_demo/index.css`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_vite_demo/package-lock.json` & `vite_transporter-0.4.1/app_vite_demo/package-lock.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/app_vite_demo/package.json` & `vite_transporter-0.4.1/app_vite_demo/package.json`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/pyproject.toml` & `vite_transporter-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/vite_transporter/__init__.py` & `vite_transporter-0.4.1/vite_transporter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from .helpers import Colr as _Colr
 from .helpers import PyProjectConfig as _PyProjectConfig
 from .helpers import _compile
 from .parser import ArgumentParser as _ArgumentParser
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 def _cli():
     pars = _ArgumentParser(prog="vtf", add_help=False)
     pars.add_argument(
         "--version", "-v", action="version", version=f"vite-to-flask {__version__}"
     )
```

### Comparing `vite_transporter-0.4.0/vite_transporter/_headers.py` & `vite_transporter-0.4.1/vite_transporter/_headers.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/vite_transporter/_html_tags.py` & `vite_transporter-0.4.1/vite_transporter/_html_tags.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/vite_transporter/helpers.py` & `vite_transporter-0.4.1/vite_transporter/helpers.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/vite_transporter/parser.py` & `vite_transporter-0.4.1/vite_transporter/parser.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/vite_transporter/platform/flask.py` & `vite_transporter-0.4.1/vite_transporter/platform/flask.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/vite_transporter/platform/quart.py` & `vite_transporter-0.4.1/vite_transporter/platform/quart.py`

 * *Files identical despite different names*

### Comparing `vite_transporter-0.4.0/PKG-INFO` & `vite_transporter-0.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vite-transporter
-Version: 0.4.0
+Version: 0.4.1
 Summary: Transport Vite apps.
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,14 +26,21 @@
 ```
 
 **Currently compatible with:**
 
 - Flask
 - Quart
 
+**Note (Flask/Quart):** When including credentials in fetch requests in the vite app.
+You must visit the serve app add first to set the credentials.
+
+For example, if the serve app is running on `http://127.0.0.1:5001`, you must visit this address first.
+
+This won't be needed in production, as it's expected that the Vite app will be served from the same domain.
+
 ## How it works
 
 ### The pyproject.toml file
 
 The pyproject.toml file is used to store what Vite apps are available.
 
 Adding the following to the pyproject.toml file will transfer all the Vite
```

