# Comparing `tmp/sphinx_tippy-0.4.1.tar.gz` & `tmp/sphinx_tippy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_tippy-0.4.1.tar", last modified: Sun Jan 15 10:01:47 2023, max compression
+gzip compressed data, was "sphinx_tippy-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_tippy-0.4.1.tar` & `sphinx_tippy-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       66 2023-01-12 04:34:35.177350 sphinx_tippy-0.4.1/.gitattributes
--rw-r--r--   0        0        0     2773 2023-01-12 19:22:19.355801 sphinx_tippy-0.4.1/.gitignore
--rw-r--r--   0        0        0      936 2023-01-15 06:22:16.825585 sphinx_tippy-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      180 2023-01-13 10:08:29.400747 sphinx_tippy-0.4.1/.readthedocs.yml
--rw-r--r--   0        0        0     1069 2023-01-12 04:36:41.962062 sphinx_tippy-0.4.1/LICENSE
--rw-r--r--   0        0        0      101 2023-01-12 04:37:20.793513 sphinx_tippy-0.4.1/README.md
--rw-r--r--   0        0        0     1539 2023-01-15 10:00:53.079110 sphinx_tippy-0.4.1/docs/conf.py
--rw-r--r--   0        0        0     1112 2023-01-13 09:15:29.706324 sphinx_tippy-0.4.1/docs/folder/other.md
--rw-r--r--   0        0        0    92086 2023-01-12 07:10:56.873650 sphinx_tippy-0.4.1/docs/fun-fish.png
--rw-r--r--   0        0        0     6364 2023-01-15 09:58:39.636688 sphinx_tippy-0.4.1/docs/index.md
--rw-r--r--   0        0        0    16642 2023-01-15 06:59:17.857077 sphinx_tippy-0.4.1/docs/tippy-logo.svg
--rw-r--r--   0        0        0     1064 2023-01-14 01:51:49.809809 sphinx_tippy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    26383 2023-01-15 09:58:39.635573 sphinx_tippy-0.4.1/src/sphinx_tippy.py
--rw-r--r--   0        0        0      602 2023-01-13 23:07:31.815745 sphinx_tippy-0.4.1/tests/test_basic.py
--rw-r--r--   0        0        0      987 2023-01-15 07:09:32.214195 sphinx_tippy-0.4.1/tests/test_basic/test_basic.yml
--rw-r--r--   0        0        0      389 2023-01-13 23:24:07.166230 sphinx_tippy-0.4.1/tox.ini
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 sphinx_tippy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2024-01-25 14:25:35.093695 sphinx_tippy-0.4.2/.gitattributes
+-rw-r--r--   0        0        0     2773 2024-01-25 14:25:35.093770 sphinx_tippy-0.4.2/.gitignore
+-rw-r--r--   0        0        0      893 2024-04-22 19:15:39.374843 sphinx_tippy-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      217 2024-01-25 14:25:35.093898 sphinx_tippy-0.4.2/.readthedocs.yml
+-rw-r--r--   0        0        0     1069 2024-01-25 14:25:35.093968 sphinx_tippy-0.4.2/LICENSE
+-rw-r--r--   0        0        0      227 2024-01-25 14:25:35.094046 sphinx_tippy-0.4.2/README.md
+-rw-r--r--   0        0        0     1539 2024-01-25 14:25:35.094150 sphinx_tippy-0.4.2/docs/conf.py
+-rw-r--r--   0        0        0     1112 2024-01-25 14:25:35.094271 sphinx_tippy-0.4.2/docs/folder/other.md
+-rw-r--r--   0        0        0    92086 2024-01-25 14:25:35.094474 sphinx_tippy-0.4.2/docs/fun-fish.png
+-rw-r--r--   0        0        0     7494 2024-04-22 19:15:39.375025 sphinx_tippy-0.4.2/docs/index.md
+-rw-r--r--   0        0        0    16642 2024-01-25 14:25:35.094640 sphinx_tippy-0.4.2/docs/tippy-logo.svg
+-rw-r--r--   0        0        0     1064 2024-01-25 14:25:35.094710 sphinx_tippy-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    27577 2024-04-22 19:15:39.375216 sphinx_tippy-0.4.2/src/sphinx_tippy.py
+-rw-r--r--   0        0        0      602 2024-01-25 14:25:35.094955 sphinx_tippy-0.4.2/tests/test_basic.py
+-rw-r--r--   0        0        0      987 2024-01-25 14:25:35.095068 sphinx_tippy-0.4.2/tests/test_basic/test_basic.yml
+-rw-r--r--   0        0        0      404 2024-04-22 19:15:39.375334 sphinx_tippy-0.4.2/tox.ini
+-rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 sphinx_tippy-0.4.2/PKG-INFO
```

### Comparing `sphinx_tippy-0.4.1/.gitignore` & `sphinx_tippy-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_tippy-0.4.1/.pre-commit-config.yaml` & `sphinx_tippy-0.4.2/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
         - id: trailing-whitespace
         - id: end-of-file-fixer
         - id: check-yaml
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 24.4.0
     hooks:
         - id: black
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.11.4
+    rev: 5.13.2
     hooks:
         - id: isort
 
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.217
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.1
     hooks:
         - id: ruff
-          args: ["--force-exclude"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.9.0
     hooks:
     - id: mypy
       args: [--config-file=pyproject.toml]
       additional_dependencies:
       - docutils-stubs
       - sphinx~=5.0
       - types-beautifulsoup4
```

### Comparing `sphinx_tippy-0.4.1/LICENSE` & `sphinx_tippy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_tippy-0.4.1/docs/conf.py` & `sphinx_tippy-0.4.2/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 myst_enable_extensions = ["deflist", "colon_fence"]
 
 # -- HTML output -------------------------------------------------
 
 html_theme = "furo"
 html_logo = "tippy-logo.svg"
 html_theme_options = {
-    "source_repository": "https://github.com/chrisjsewell/sphinx_tippy/",
+    "source_repository": "https://github.com/chrisjsewell/sphinx-tippy/",
     "source_branch": "main",
     "source_directory": "docs/",
 }
 
 tippy_enable_mathjax = True
 tippy_anchor_parent_selector = "div.content"
 tippy_logo_svg = Path("tippy-logo.svg").read_text("utf8")
```

### Comparing `sphinx_tippy-0.4.1/docs/folder/other.md` & `sphinx_tippy-0.4.2/docs/folder/other.md`

 * *Files identical despite different names*

### Comparing `sphinx_tippy-0.4.1/docs/fun-fish.png` & `sphinx_tippy-0.4.2/docs/fun-fish.png`

 * *Files identical despite different names*

### Comparing `sphinx_tippy-0.4.1/docs/index.md` & `sphinx_tippy-0.4.2/docs/index.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Sphinx Tippy
 
+[![GitHub Repo stars](https://img.shields.io/github/stars/chrisjsewell/sphinx-tippy?label=Like%20and%20Share%21&style=social)](https://github.com/chrisjsewell/sphinx-tippy)
+
 Get rich hover tips in your sphinx documentation.
 
 [**Hover on me!**](https://atomiks.github.io/tippyjs)
 
 ```{toctree}
 :hidden:
 folder/other
@@ -68,14 +70,39 @@
 
 :::
 
 [^1]: This is a footnote
 
     This is another paragraph
 
+:::{important}
+Dependent on the theme you ar using with sphinx,
+you may need to add some CSS to your `conf.py` to make the tooltips show correctly.
+
+For example, for the [Pydata Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io):
+
+`conf.py`:
+
+```python
+html_static_path = ['_static']
+html_css_files = ["tippy.css"]
+```
+
+`_static/tippy.css`:
+
+```css
+.tippy-box {
+    background-color:var(--pst-color-surface);
+    color:var(--pst-color-text-base);
+    border: 1px solid var(--pst-color-border);
+}
+```
+
+:::
+
 ## How does it work?
 
 The extension uses the [tippy.js](https://atomiks.github.io/tippyjs) library to create tooltips.
 
 Currently, all tips are created during the build process, so there is no need for a server and, once loaded, all tips are very responsive
 (although [dynamic fetching](https://atomiks.github.io/tippyjs/v6/ajax/) could be implemented later).
 
@@ -90,18 +117,26 @@
 
 ### Display
 
 :::{confval} tippy_props
 Overrides for the [tippy.js props](https://atomiks.github.io/tippyjs/v6/all-props/) to use, by default:
 
 ```python
-tippy_props = {"placement": "auto-start", "maxWidth": 500, "interactive": False, "arrow": True}
+tippy_props = {"placement": "auto-start", "maxWidth": 500, "interactive": False, "theme": "material", "duration": [200, 100], "delay": [200, 500]}
 ```
 
-Note, only the `placement`, `maxWidth` and `interactive` props are allowed to be overridden currently.
+Note, only the following props are allowed to be overridden currently:
+
+- [placement](https://atomiks.github.io/tippyjs/v6/all-props/#placement)
+- [maxWidth](https://atomiks.github.io/tippyjs/v6/all-props/#maxwidth)
+- [theme](https://atomiks.github.io/tippyjs/v6/all-props/#theme)
+- [interactive](https://atomiks.github.io/tippyjs/v6/all-props/#interactive)
+- [delay](https://atomiks.github.io/tippyjs/v6/all-props/#delay)
+- [duration](https://atomiks.github.io/tippyjs/v6/all-props/#duration)
+
 :::
 
 :::{confval} tippy_add_class
 Add a class name to all elements with tips.
 
 For example this can be used to change the style of the cursor when hovering over a tip (see [`html_css_files`](https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_css_files)):
```

### Comparing `sphinx_tippy-0.4.1/docs/tippy-logo.svg` & `sphinx_tippy-0.4.2/docs/tippy-logo.svg`

 * *Files identical despite different names*

### Comparing `sphinx_tippy-0.4.1/pyproject.toml` & `sphinx_tippy-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "sphinx>4",
     "beautifulsoup4",
     "jinja2",
     "requests",
 ]
 
 [project.urls]
-Home = "https://github.com/chrisjsewell/sphinx_tippy"
+Home = "https://github.com/chrisjsewell/sphinx-tippy"
 Documentation = "https://sphinx-tippy.readthedocs.io"
 
 [project.optional-dependencies]
 testing = [
     "pytest",
     "sphinx-pytest",
     "pytest-regressions",
```

### Comparing `sphinx_tippy-0.4.1/src/sphinx_tippy.py` & `sphinx_tippy-0.4.2/src/sphinx_tippy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Get rich tool tips in your sphinx documentation!"""
+
 from __future__ import annotations
 
 import json
 import posixpath
 import re
 from dataclasses import dataclass
 from pathlib import Path
@@ -21,15 +22,15 @@
 
 try:
     # sphinx 6.1
     from sphinx.util.display import status_iterator  # type: ignore[import]
 except ImportError:
     from sphinx.util import status_iterator
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 
 
 def setup(app: Sphinx):
     """Setup the extension"""
     app.add_config_value("tippy_props", {}, "html")
     # config for filtering tooltip creation/showing
     app.add_config_value("tippy_skip_urls", (), "html", [list, tuple])
@@ -121,17 +122,27 @@
     # validate the props
     updates = app.config.tippy_props or {}
     if not isinstance(updates, dict):
         raise ExtensionError(f"tippy_props must be a dictionary, not a {type(updates)}")
     props = dict(
         {"placement": "auto-start", "maxWidth": 500, "interactive": False}, **updates
     )
-    if set(props.keys()) - {"placement", "maxWidth", "interactive"}:
+
+    supported_properties = {
+        "placement",
+        "maxWidth",
+        "interactive",
+        "theme",
+        "delay",
+        "duration",
+    }
+
+    if set(props.keys()) - supported_properties:
         raise ExtensionError(
-            "tippy_props can only contain keys 'placement', 'maxWidth', 'interactive'"
+            "tippy_props can only contain keys '%s'" % "', '".join(supported_properties)
         )
     allowed_placements = {
         "auto",
         "auto-start",
         "auto-end",
         "top",
         "top-start",
@@ -155,14 +166,26 @@
         raise ExtensionError("tippy_props['maxWidth'] must be an integer or None")
     props["maxWidth"] = (
         "'none'" if props["maxWidth"] is None else str(props["maxWidth"])
     )
     if not isinstance(props["interactive"], bool):
         raise ExtensionError("tippy_props['interactive'] must be a boolean")
     props["interactive"] = "true" if props["interactive"] else "false"
+    if "theme" in props:
+        if not (props["theme"] is None or isinstance(props["theme"], str)):
+            raise ExtensionError("tippy_props['theme'] must be None or a string")
+        props["theme"] = f"'{props['theme']}'" if props["theme"] else "null"
+    if "delay" in props:
+        if not (props["delay"] is None or isinstance(props["delay"], list)):
+            raise ExtensionError("tippy_props['delay'] must be None or a list")
+        props["delay"] = props["delay"] if props["delay"] else "null"
+    if "duration" in props:
+        if not (props["duration"] is None or isinstance(props["duration"], list)):
+            raise ExtensionError("tippy_props['duration'] must be None or a list")
+        props["duration"] = props["duration"] if props["duration"] else "null"
     app.env.tippy_config = TippyConfig(  # type: ignore[attr-defined]
         props=props,
         custom_tips=app.config.tippy_custom_tips,
         skip_url_regexes=skip_url_regexes,
         tip_selector=app.config.tippy_tip_selector,
         skip_anchor_classes=app.config.tippy_skip_anchor_classes,
         anchor_parent_selector=app.config.tippy_anchor_parent_selector,
@@ -241,15 +264,14 @@
     anchor: Tag
     refs_in_page: set[tuple[None | str, str | None]] = set()
     custom_in_page: set[str] = set()
     wiki_titles: set[str] = set()
     doi_names: set[str] = set()
     rtd_urls: set[str] = set()
     for anchor in body.find_all("a", {"href": True}):
-
         if not isinstance(anchor["href"], str):
             continue
 
         if anchor["href"] in custom_tips:
             custom_in_page.add(anchor["href"])
             continue
 
@@ -296,14 +318,16 @@
 
     id_to_tip_html = create_id_to_tip_html(tippy_config, body)
 
     # create path based on pagename
     # we also add a unique ID to the path,
     # which is in order to avoid browsers using old cached versions
     # lets also remove any old versions of the file when running rebuilds
+    # TODO ideally here, we would just add a query string to the script load
+    # see: https://github.com/sphinx-doc/sphinx/issues/11133
     parts = pagename.split("/")
     for old_path in Path(app.outdir, "_static", "tippy", *parts).parent.glob(
         f"{parts[0]}.*.js"
     ):
         old_path.unlink()
     js_path = Path(
         app.outdir, "_static", "tippy", *(pagename + f".{uuid4()}.js").split("/")
@@ -365,15 +389,14 @@
     # these are tags where we simply copy the whole HTML
     for tag in body.select(config.tip_selector):
         if "id" in tag.attrs:
             id_to_html[str(tag["id"])] = str(tag)
 
     # these are tags where we copy the HTML in a bespoke way
     for tag in body.find_all(id=True):
-
         if tag.name == "dt":
             # copy the whole HTML
             id_to_html[str(tag["id"])] = str(strip_classes(tag.__copy__()))
             # if the next tag is a dd, copy that too
             if (next_sibling := next_sibling_tag(tag)) and next_sibling.name == "dd":
                 copy_dd = next_sibling.__copy__()
                 # limit the children to certain numbers and types
@@ -389,15 +412,20 @@
                 id_to_html[str(tag["id"])] += str(copy_dd)
 
         elif tag.name == "section" and (
             header := tag.find(["h1", "h2", "h3", "h4", "h5", "h6"])
         ):
             id_to_html[str(tag["id"])] = _get_header_html(header)
 
-        elif tag.name == "div" and "math-wrapper" in (tag.get("class") or []):
+        elif tag.name == "div" and (
+            all(
+                class_to_check in (tag.get("class") or [])
+                for class_to_check in ("math", "notranslate", "nohighlight")
+            )
+        ):
             # remove an span with eqno class, since it is not needed
             # and it can cause issues with the tooltip
             # (e.g. if the span is the last element in the div)
             tag_copy = tag.__copy__()
             for child in tag_copy.find_all("span"):
                 if isinstance(child, Tag) and "eqno" in (child.get("class") or []):
                     child.decompose()
@@ -641,15 +669,14 @@
     for doi in data["dois"]:
         if doi in doi_cache:
             selector_to_html[f'a[href="{DOI_PATH}{doi}"]'] = doi_cache[doi]
     for rtd in data["rtd_urls"]:
         if rtd in rtd_cache:
             selector_to_html[f'a[href="{rtd}"]'] = rtd_cache[rtd]
     for refpage, target in data["refs_in_page"]:
-
         if refpage is not None:
             relpage = posixpath.normpath(
                 posixpath.relpath(refpage, posixpath.dirname(pagename))
             )
             relfolder = posixpath.dirname(relpage)
             if refpage not in tippy_page_data:
                 pass
```

### Comparing `sphinx_tippy-0.4.1/tests/test_basic.py` & `sphinx_tippy-0.4.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `sphinx_tippy-0.4.1/tests/test_basic/test_basic.yml` & `sphinx_tippy-0.4.2/tests/test_basic/test_basic.yml`

 * *Files identical despite different names*

### Comparing `sphinx_tippy-0.4.1/PKG-INFO` & `sphinx_tippy-0.4.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_tippy
-Version: 0.4.1
+Version: 0.4.2
 Summary: Get rich tool tips in your sphinx documentation!
 Keywords: sphinx,tooltip,tippy
 Author-email: Chris Sewell <chrisj_sewell@hotmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Extension
@@ -17,17 +17,19 @@
 Requires-Dist: requests
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: furo ; extra == "docs"
 Requires-Dist: pytest ; extra == "testing"
 Requires-Dist: sphinx-pytest ; extra == "testing"
 Requires-Dist: pytest-regressions ; extra == "testing"
 Project-URL: Documentation, https://sphinx-tippy.readthedocs.io
-Project-URL: Home, https://github.com/chrisjsewell/sphinx_tippy
+Project-URL: Home, https://github.com/chrisjsewell/sphinx-tippy
 Provides-Extra: docs
 Provides-Extra: testing
 
 # sphinx-tippy
 
+![GitHub Repo stars](https://img.shields.io/github/stars/chrisjsewell/sphinx-tippy?label=Like%20and%20Share%21&style=social)
+
 Get rich tool tips in your sphinx documentation!
 
 See the documentation for details.
```

