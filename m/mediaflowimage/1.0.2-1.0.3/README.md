# Comparing `tmp/mediaflowimage-1.0.2.tar.gz` & `tmp/mediaflowimage-1.0.3.tar.gz`

## Comparing `mediaflowimage-1.0.2.tar` & `mediaflowimage-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/admin.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/apps.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/blocks.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/forms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/models.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/tests.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/views.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/wagtail_hooks.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/migrations/__init__.py
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/LICENSE
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/README.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/admin.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/apps.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/blocks.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/forms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/models.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/tests.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/views.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/wagtail_hooks.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/migrations/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/static/css/mediaflow-imagechooser-extensions.css
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/README.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 mediaflowimage-1.0.3/PKG-INFO
```

### Comparing `mediaflowimage-1.0.2/src/mediaflowimage/wagtail_hooks.py` & `mediaflowimage-1.0.3/src/mediaflowimage/wagtail_hooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import requests
 from django.conf import settings
 from django.utils.html import format_html
 from django.utils.safestring import mark_safe
 from wagtail import hooks
 from wagtail.images import get_image_model
+from django.templatetags.static import static
 
 
 @hooks.register("insert_editor_js")
 def fileselector_js():
     return format_html(
         '<script src="https://mfstatic.com/js/fileselector.min.js"></script>'
     ) + mark_safe(
@@ -21,15 +22,17 @@
                         window.MediaflowImageModal = e;                             
                         prevChooseHandler(e,t);                        
                     }                    
                 });
             </script>
             """
     )
-
+@hooks.register('insert_global_admin_css')
+def mediaflow_extra_css():
+    return format_html('<link rel="stylesheet" href="{}">', static('css/mediaflow-imagechooser-extensions.css'))
 
 @hooks.register("after_publish_page")
 def register_file_usage(request, page):    
     # Call the process_data method on the page
     for field in page.specific._meta.fields:
         name = str(field)        
         try:
```

### Comparing `mediaflowimage-1.0.2/src/mediaflowimage/widgets.py` & `mediaflowimage-1.0.3/src/mediaflowimage/widgets.py`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.2/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js` & `mediaflowimage-1.0.3/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -218,21 +218,24 @@
         ),
         fileSelectorElement = $(
             '<div id="mf-fileselector" style="position:relative;min-height:460px" class="light"></div>',
         )
 
     newSection.append(fileSelectorElement)
     $('.modal-body .tab-content').append(newSection)
+
+
     $('.modal-body [role=tablist]').append(tabLink)
 
     tabLink.on('click', function(e) {
         e.preventDefault()
         $('.modal-body section').each(function() {
             if ($(this).attr('id') == 'tab-mfp-insert') {
                 $(this).removeAttr('hidden')
+                consolelog('parentNode', $('.tab-content').parent())
             } else {
                 $(this).attr('hidden', '')
             }
         })
         $('.modal-body .w-tabs a').each(function() {
             $(this).attr(
                 'aria-selected',
```

### Comparing `mediaflowimage-1.0.2/LICENSE` & `mediaflowimage-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.2/README.md` & `mediaflowimage-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.2/pyproject.toml` & `mediaflowimage-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "mediaflowimage"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Mediaflow Europe AB", email="support@mediaflow.com" },
 ]
 description = "Wagtail image plugin for Mediaflow"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mediaflowimage-1.0.2/PKG-INFO` & `mediaflowimage-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mediaflowimage
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wagtail image plugin for Mediaflow
 Project-URL: Homepage, https://support.mediaflow.com
 Project-URL: Issues, https://support.mediaflow.com
 Author-email: Mediaflow Europe AB <support@mediaflow.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

