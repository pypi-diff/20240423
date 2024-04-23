# Comparing `tmp/mediaflowimage-1.0.4.tar.gz` & `tmp/mediaflowimage-1.0.6.tar.gz`

## Comparing `mediaflowimage-1.0.4.tar` & `mediaflowimage-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/admin.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/apps.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/blocks.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/forms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/models.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/tests.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/views.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/wagtail_hooks.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/migrations/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/static/css/mediaflow-imagechooser-extensions.css
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/LICENSE
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/README.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 mediaflowimage-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/admin.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/apps.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/blocks.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/forms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/models.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/tests.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/views.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/wagtail_hooks.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/migrations/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/static/css/mediaflow-imagechooser-extensions.css
+-rw-r--r--   0        0        0     8153 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/LICENSE
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/README.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 mediaflowimage-1.0.6/PKG-INFO
```

### Comparing `mediaflowimage-1.0.4/src/mediaflowimage/wagtail_hooks.py` & `mediaflowimage-1.0.6/src/mediaflowimage/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.4/src/mediaflowimage/widgets.py` & `mediaflowimage-1.0.6/src/mediaflowimage/widgets.py`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.4/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js` & `mediaflowimage-1.0.6/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -218,24 +218,23 @@
         ),
         fileSelectorElement = $(
             '<div id="mf-fileselector" style="position:relative;min-height:460px" class="light"></div>',
         )
 
     newSection.append(fileSelectorElement)
     $('.modal-body .tab-content').append(newSection)
-
-
     $('.modal-body [role=tablist]').append(tabLink)
 
     tabLink.on('click', function(e) {
         e.preventDefault()
         $('.modal-body section').each(function() {
             if ($(this).attr('id') == 'tab-mfp-insert') {
+                console.log('parentNode', $(this).parent().get(0))
+                $(this).parent().toggleClass('mf-wide')
                 $(this).removeAttr('hidden')
-                consolelog('parentNode', $('.tab-content').parent())
             } else {
                 $(this).attr('hidden', '')
             }
         })
         $('.modal-body .w-tabs a').each(function() {
             $(this).attr(
                 'aria-selected',
@@ -243,14 +242,16 @@
             )
         })
     })
 
     $('.modal-body a.w-tabs__tab').each(function() {
         if ($(this).attr('id') != 'tab-label-mfp-insert') {
             $(this).on('click', function() {
+                console.log('removing mf-wide class')
+                $('.tab-content').removeClass('mf-wide')
                 $('#tab-mfp-insert').attr('hidden', '')
                 $('#tab-label-mfp-insert').attr('aria-selected', 'false')
             })
         }
     })
```

### Comparing `mediaflowimage-1.0.4/LICENSE` & `mediaflowimage-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.4/README.md` & `mediaflowimage-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.4/pyproject.toml` & `mediaflowimage-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "mediaflowimage"
-version = "1.0.4"
+version = "1.0.6"
 authors = [
   { name="Mediaflow Europe AB", email="support@mediaflow.com" },
 ]
 description = "Wagtail image plugin for Mediaflow"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mediaflowimage-1.0.4/PKG-INFO` & `mediaflowimage-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mediaflowimage
-Version: 1.0.4
+Version: 1.0.6
 Summary: Wagtail image plugin for Mediaflow
 Project-URL: Homepage, https://support.mediaflow.com
 Project-URL: Issues, https://support.mediaflow.com
 Author-email: Mediaflow Europe AB <support@mediaflow.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

