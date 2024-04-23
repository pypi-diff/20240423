# Comparing `tmp/skill_tagging-0.1.9.tar.gz` & `tmp/skill_tagging-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skill_tagging-0.1.9.tar", last modified: Thu Mar 21 11:21:41 2024, max compression
+gzip compressed data, was "skill_tagging-0.2.0.tar", last modified: Tue Apr 23 14:29:14 2024, max compression
```

## Comparing `skill_tagging-0.1.9.tar` & `skill_tagging-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:21:41.355984 skill_tagging-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-03-21 11:21:41.355984 skill_tagging-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:21:41.351984 skill_tagging-0.1.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-21 11:21:41.355984 skill_tagging-0.1.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5233 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:21:41.351984 skill_tagging-0.1.9/skill_tagging/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/skill_tagging_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:21:41.355984 skill_tagging-0.1.9/skill_tagging/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/brainstorming.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/tagging.css
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/tagging.html
--rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/tagging.js
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/tags_error.html
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/tags_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/tags_thankyou.html
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/static/video_tagging.js
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/skill_tagging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:21:41.351984 skill_tagging-0.1.9/skill_tagging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-03-21 11:21:41.000000 skill_tagging-0.1.9/skill_tagging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-21 11:21:41.000000 skill_tagging-0.1.9/skill_tagging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 11:21:41.000000 skill_tagging-0.1.9/skill_tagging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-21 11:21:41.000000 skill_tagging-0.1.9/skill_tagging.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 11:21:41.000000 skill_tagging-0.1.9/skill_tagging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-21 11:21:41.000000 skill_tagging-0.1.9/skill_tagging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-21 11:21:41.000000 skill_tagging-0.1.9/skill_tagging.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 11:21:41.355984 skill_tagging-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-21 11:21:38.000000 skill_tagging-0.1.9/tests/test_skill_tagging_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:14.789524 skill_tagging-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 14:29:08.000000 skill_tagging-0.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-23 14:29:08.000000 skill_tagging-0.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-23 14:29:08.000000 skill_tagging-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    35139 2024-04-23 14:29:08.000000 skill_tagging-0.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-23 14:29:08.000000 skill_tagging-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12407 2024-04-23 14:29:14.789524 skill_tagging-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-04-23 14:29:08.000000 skill_tagging-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:14.785524 skill_tagging-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-23 14:29:14.789524 skill_tagging-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5233 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:14.785524 skill_tagging-0.2.0/skill_tagging/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/skill_tagging_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:14.785524 skill_tagging-0.2.0/skill_tagging/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/brainstorming.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/tagging.css
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/tagging.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3994 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/tagging.js
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/tags_error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/tags_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/tags_thankyou.html
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/static/video_tagging.js
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/skill_tagging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:14.785524 skill_tagging-0.2.0/skill_tagging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12407 2024-04-23 14:29:14.000000 skill_tagging-0.2.0/skill_tagging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-23 14:29:14.000000 skill_tagging-0.2.0/skill_tagging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:29:14.000000 skill_tagging-0.2.0/skill_tagging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-23 14:29:14.000000 skill_tagging-0.2.0/skill_tagging.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:29:14.000000 skill_tagging-0.2.0/skill_tagging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 14:29:14.000000 skill_tagging-0.2.0/skill_tagging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 14:29:14.000000 skill_tagging-0.2.0/skill_tagging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:29:14.785524 skill_tagging-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-23 14:29:09.000000 skill_tagging-0.2.0/tests/test_skill_tagging_mixin.py
```

### Comparing `skill_tagging-0.1.9/CHANGELOG.rst` & `skill_tagging-0.2.0/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -11,14 +11,32 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 
+[0.2.0] - 2024-04-23
+************************************************
+
+Changed
+=======
+
+* Applied updates required for XBlock 3.0
+
+
+[0.1.10] - 2024-03-22
+************************************************
+
+Changed
+=======
+
+* Remove log statement
+
+
 [0.1.9] - 2024-03-20
 ************************************************
 
 Changed
 =======
 
 * Pass course key as query param to taxonomy skills api
```

### Comparing `skill_tagging-0.1.9/LICENSE` & `skill_tagging-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/LICENSE.txt` & `skill_tagging-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/PKG-INFO` & `skill_tagging-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skill_tagging
-Version: 0.1.9
+Version: 0.2.0
 Summary: Django app plugin for fetching and verifying tags for xblock skills.
 Home-page: https://github.com/openedx/xblock-skill-tagging
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -303,14 +303,32 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 
+[0.2.0] - 2024-04-23
+************************************************
+
+Changed
+=======
+
+* Applied updates required for XBlock 3.0
+
+
+[0.1.10] - 2024-03-22
+************************************************
+
+Changed
+=======
+
+* Remove log statement
+
+
 [0.1.9] - 2024-03-20
 ************************************************
 
 Changed
 =======
 
 * Pass course key as query param to taxonomy skills api
```

### Comparing `skill_tagging-0.1.9/README.rst` & `skill_tagging-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/requirements/constraints.txt` & `skill_tagging-0.2.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/setup.py` & `skill_tagging-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/apps.py` & `skill_tagging-0.2.0/skill_tagging/apps.py`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/handlers.py` & `skill_tagging-0.2.0/skill_tagging/handlers.py`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/pipeline.py` & `skill_tagging-0.2.0/skill_tagging/pipeline.py`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/skill_tagging_mixin.py` & `skill_tagging-0.2.0/skill_tagging/skill_tagging_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 from urllib.parse import urljoin
 
 from django.conf import settings
 from django.utils.timezone import datetime, timezone
 from django.utils.translation import gettext as _
 from openedx_events.learning.data import XBlockSkillVerificationData
 from openedx_events.learning.signals import XBLOCK_SKILL_VERIFIED
-from xblock.core import XBlock
+from xblock.core import XBlock, XBlockMixin
 from xblock.fields import Boolean, Scope
-from xblock.internal import NamedAttributesMetaclass
 from xblock.runtime import NoSuchServiceError
 
 from .utils import get_api_client
 
 LOGGER = logging.getLogger(__name__)
 PAGE_SIZE = getattr(settings, "TAXONOMY_API_SKILL_PAGE_SIZE", 100)
 
 
 # Make '_' a no-op so we can scrape strings
 def _(text):
     return text
 
 
-class SkillTaggingMixin(metaclass=NamedAttributesMetaclass):
+class SkillTaggingMixin(XBlockMixin):
     """
     XBlock Mixin for fetching and verifying skill tags
     """
     has_verified_tags = Boolean(
         display_name=_("Has verified tags"),
         default=False,
         help=_("Has user verified tags for this XBlock?"),
@@ -66,17 +65,14 @@
             return []
 
         user = user_service.get_user_by_anonymous_id()
         api_client = get_api_client(user=user)
 
         course_key_str = str(self.scope_ids.usage_id.context_key)
         usage_id_str = str(self.scope_ids.usage_id)
-        LOGGER.info(
-            f"[XBLOCK_SKILL_TAGGING] Fetching Skills. XBlock: [{usage_id_str}], Course: [{course_key_str}]."
-        )
         XBLOCK_SKILL_TAGS_API = urljoin(
             settings.TAXONOMY_API_BASE_URL,
             '/taxonomy/api/v1/xblocks/'
         )
         response = api_client.get(
             XBLOCK_SKILL_TAGS_API,
             params={
```

### Comparing `skill_tagging-0.1.9/skill_tagging/static/brainstorming.svg` & `skill_tagging-0.2.0/skill_tagging/static/brainstorming.svg`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/static/tagging.css` & `skill_tagging-0.2.0/skill_tagging/static/tagging.css`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/static/tagging.js` & `skill_tagging-0.2.0/skill_tagging/static/tagging.js`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/static/tags_form.html` & `skill_tagging-0.2.0/skill_tagging/static/tags_form.html`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging/static/video_tagging.js` & `skill_tagging-0.2.0/skill_tagging/static/video_tagging.js`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/skill_tagging.egg-info/PKG-INFO` & `skill_tagging-0.2.0/skill_tagging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skill-tagging
-Version: 0.1.9
+Version: 0.2.0
 Summary: Django app plugin for fetching and verifying tags for xblock skills.
 Home-page: https://github.com/openedx/xblock-skill-tagging
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -303,14 +303,32 @@
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 
+[0.2.0] - 2024-04-23
+************************************************
+
+Changed
+=======
+
+* Applied updates required for XBlock 3.0
+
+
+[0.1.10] - 2024-03-22
+************************************************
+
+Changed
+=======
+
+* Remove log statement
+
+
 [0.1.9] - 2024-03-20
 ************************************************
 
 Changed
 =======
 
 * Pass course key as query param to taxonomy skills api
```

### Comparing `skill_tagging-0.1.9/skill_tagging.egg-info/SOURCES.txt` & `skill_tagging-0.2.0/skill_tagging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/tests/test_pipeline.py` & `skill_tagging-0.2.0/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `skill_tagging-0.1.9/tests/test_skill_tagging_mixin.py` & `skill_tagging-0.2.0/tests/test_skill_tagging_mixin.py`

 * *Files identical despite different names*

