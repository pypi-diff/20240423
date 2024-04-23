# Comparing `tmp/tinycss2-1.2.1.tar.gz` & `tmp/tinycss2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinycss2-1.2.1.tar", last modified: Tue Oct 18 07:04:53 2022, max compression
+gzip compressed data, was "tinycss2-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tinycss2-1.2.1.tar` & `tinycss2-1.3.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1534 2020-10-30 20:31:41.489813 tinycss2-1.2.1/LICENSE
--rw-r--r--   0        0        0     1328 2022-05-27 16:25:35.352110 tinycss2-1.2.1/README.rst
--rw-r--r--   0        0        0     3038 2021-09-05 09:30:27.902646 tinycss2-1.2.1/docs/api_reference.rst
--rw-r--r--   0        0        0     3007 2022-10-18 07:02:14.044229 tinycss2-1.2.1/docs/changelog.rst
--rw-r--r--   0        0        0     3397 2021-09-05 09:30:27.902646 tinycss2-1.2.1/docs/common_use_cases.rst
--rw-r--r--   0        0        0     2857 2021-09-05 09:30:30.528626 tinycss2-1.2.1/docs/conf.py
--rw-r--r--   0        0        0     1847 2022-09-06 20:33:48.286416 tinycss2-1.2.1/docs/contribute.rst
--rw-r--r--   0        0        0      526 2020-10-30 20:31:41.490813 tinycss2-1.2.1/docs/css_diagram_role.py
--rw-r--r--   0        0        0     2383 2021-09-05 09:30:27.902646 tinycss2-1.2.1/docs/first_steps.rst
--rw-r--r--   0        0        0     2526 2021-09-05 09:30:27.902646 tinycss2-1.2.1/docs/going_further.rst
--rw-r--r--   0        0        0      302 2021-09-05 09:30:30.528626 tinycss2-1.2.1/docs/index.rst
--rw-r--r--   0        0        0      887 2021-09-05 09:30:27.903646 tinycss2-1.2.1/docs/support.rst
--rw-r--r--   0        0        0     1988 2022-09-06 20:33:48.286416 tinycss2-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     2283 2021-11-21 13:33:11.451535 tinycss2-1.2.1/tests/css-parsing-tests/An+B.json
--rw-r--r--   0        0        0      326 2021-11-21 13:33:11.451535 tinycss2-1.2.1/tests/css-parsing-tests/LICENSE
--rw-r--r--   0        0        0     9365 2022-10-18 07:01:07.280243 tinycss2-1.2.1/tests/css-parsing-tests/README.rst
--rw-r--r--   0        0        0     3964 2022-10-18 07:01:07.280243 tinycss2-1.2.1/tests/css-parsing-tests/color3.json
--rw-r--r--   0        0        0   204279 2022-10-18 07:01:07.281243 tinycss2-1.2.1/tests/css-parsing-tests/color3_hsl.json
--rw-r--r--   0        0        0    23390 2022-10-18 07:01:07.282244 tinycss2-1.2.1/tests/css-parsing-tests/color3_keywords.json
--rw-r--r--   0        0        0    14886 2022-10-18 07:01:07.282244 tinycss2-1.2.1/tests/css-parsing-tests/component_value_list.json
--rw-r--r--   0        0        0     1198 2021-11-21 13:33:11.453535 tinycss2-1.2.1/tests/css-parsing-tests/declaration_list.json
--rw-r--r--   0        0        0      635 2022-10-18 07:01:07.282244 tinycss2-1.2.1/tests/css-parsing-tests/make_color3_hsl.py
--rw-r--r--   0        0        0     6890 2022-10-18 07:01:07.282244 tinycss2-1.2.1/tests/css-parsing-tests/make_color3_keywords.py
--rw-r--r--   0        0        0      657 2021-11-21 13:33:11.453535 tinycss2-1.2.1/tests/css-parsing-tests/one_component_value.json
--rw-r--r--   0        0        0     1558 2021-11-21 13:33:11.453535 tinycss2-1.2.1/tests/css-parsing-tests/one_declaration.json
--rw-r--r--   0        0        0     1030 2021-11-21 13:33:11.453535 tinycss2-1.2.1/tests/css-parsing-tests/one_rule.json
--rw-r--r--   0        0        0     1342 2021-11-21 13:33:11.453535 tinycss2-1.2.1/tests/css-parsing-tests/rule_list.json
--rw-r--r--   0        0        0     1341 2021-11-21 13:33:11.453535 tinycss2-1.2.1/tests/css-parsing-tests/stylesheet.json
--rw-r--r--   0        0        0     5055 2021-11-21 13:33:11.453535 tinycss2-1.2.1/tests/css-parsing-tests/stylesheet_bytes.json
--rw-r--r--   0        0        0     7457 2022-10-17 19:08:32.237164 tinycss2-1.2.1/tests/test_tinycss2.py
--rw-r--r--   0        0        0      580 2022-10-18 07:01:42.481755 tinycss2-1.2.1/tinycss2/__init__.py
--rw-r--r--   0        0        0    23499 2022-10-17 19:08:32.237164 tinycss2-1.2.1/tinycss2/ast.py
--rw-r--r--   0        0        0     4768 2020-10-30 20:31:41.490813 tinycss2-1.2.1/tinycss2/bytes.py
--rw-r--r--   0        0        0    11182 2022-10-17 19:08:22.504482 tinycss2-1.2.1/tinycss2/color3.py
--rw-r--r--   0        0        0     3488 2022-01-08 15:21:17.687396 tinycss2-1.2.1/tinycss2/nth.py
--rw-r--r--   0        0        0    13759 2020-10-30 20:31:41.490813 tinycss2-1.2.1/tinycss2/parser.py
--rw-r--r--   0        0        0     4215 2021-06-13 06:35:35.063516 tinycss2-1.2.1/tinycss2/serializer.py
--rw-r--r--   0        0        0    15383 2020-10-30 20:31:41.490813 tinycss2-1.2.1/tinycss2/tokenizer.py
--rw-r--r--   0        0        0     2982 1970-01-01 00:00:00.000000 tinycss2-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1534 2020-10-30 20:31:41.489813 tinycss2-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1328 2023-12-18 20:14:28.869470 tinycss2-1.3.0/README.rst
+-rw-r--r--   0        0        0     3078 2024-03-18 15:02:18.652818 tinycss2-1.3.0/docs/api_reference.rst
+-rw-r--r--   0        0        0     3155 2024-04-23 14:05:00.750084 tinycss2-1.3.0/docs/changelog.rst
+-rw-r--r--   0        0        0     3393 2024-03-18 15:02:18.652818 tinycss2-1.3.0/docs/common_use_cases.rst
+-rw-r--r--   0        0        0     2945 2023-12-18 18:45:27.561892 tinycss2-1.3.0/docs/conf.py
+-rw-r--r--   0        0        0     1702 2024-03-19 11:38:47.867247 tinycss2-1.3.0/docs/contribute.rst
+-rw-r--r--   0        0        0      526 2020-10-30 20:31:41.490813 tinycss2-1.3.0/docs/css_diagram_role.py
+-rw-r--r--   0        0        0     2383 2021-09-05 09:30:27.902646 tinycss2-1.3.0/docs/first_steps.rst
+-rw-r--r--   0        0        0     2526 2021-09-05 09:30:27.902646 tinycss2-1.3.0/docs/going_further.rst
+-rw-r--r--   0        0        0      302 2021-09-05 09:30:30.528626 tinycss2-1.3.0/docs/index.rst
+-rw-r--r--   0        0        0      887 2021-09-05 09:30:27.903646 tinycss2-1.3.0/docs/support.rst
+-rw-r--r--   0        0        0     2072 2024-03-19 11:38:47.868247 tinycss2-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2283 2021-11-21 13:33:11.451535 tinycss2-1.3.0/tests/css-parsing-tests/An+B.json
+-rw-r--r--   0        0        0      326 2021-11-21 13:33:11.451535 tinycss2-1.3.0/tests/css-parsing-tests/LICENSE
+-rw-r--r--   0        0        0     9631 2024-03-17 16:26:04.593720 tinycss2-1.3.0/tests/css-parsing-tests/README.rst
+-rw-r--r--   0        0        0     2063 2024-03-17 16:26:04.593720 tinycss2-1.3.0/tests/css-parsing-tests/blocks_contents.json
+-rw-r--r--   0        0        0     3964 2024-02-10 10:45:30.144310 tinycss2-1.3.0/tests/css-parsing-tests/color3.json
+-rw-r--r--   0        0        0   204279 2024-02-10 10:45:30.145310 tinycss2-1.3.0/tests/css-parsing-tests/color3_hsl.json
+-rw-r--r--   0        0        0    23390 2024-02-10 10:45:30.145310 tinycss2-1.3.0/tests/css-parsing-tests/color3_keywords.json
+-rw-r--r--   0        0        0    14886 2024-02-10 10:45:30.145310 tinycss2-1.3.0/tests/css-parsing-tests/component_value_list.json
+-rw-r--r--   0        0        0     1198 2024-01-21 15:47:04.919289 tinycss2-1.3.0/tests/css-parsing-tests/declaration_list.json
+-rw-r--r--   0        0        0      635 2024-02-10 10:45:30.145310 tinycss2-1.3.0/tests/css-parsing-tests/make_color3_hsl.py
+-rw-r--r--   0        0        0     6890 2024-02-10 10:45:30.145310 tinycss2-1.3.0/tests/css-parsing-tests/make_color3_keywords.py
+-rw-r--r--   0        0        0      657 2021-11-21 13:33:11.453535 tinycss2-1.3.0/tests/css-parsing-tests/one_component_value.json
+-rw-r--r--   0        0        0     1363 2024-03-17 16:26:04.593720 tinycss2-1.3.0/tests/css-parsing-tests/one_declaration.json
+-rw-r--r--   0        0        0     1030 2024-02-04 15:27:18.395130 tinycss2-1.3.0/tests/css-parsing-tests/one_rule.json
+-rw-r--r--   0        0        0     1342 2021-11-21 13:33:11.453535 tinycss2-1.3.0/tests/css-parsing-tests/rule_list.json
+-rw-r--r--   0        0        0     1341 2024-02-04 15:27:18.394130 tinycss2-1.3.0/tests/css-parsing-tests/stylesheet.json
+-rw-r--r--   0        0        0     5055 2021-11-21 13:33:11.453535 tinycss2-1.3.0/tests/css-parsing-tests/stylesheet_bytes.json
+-rw-r--r--   0        0        0     7517 2024-03-19 11:38:47.868247 tinycss2-1.3.0/tests/test_tinycss2.py
+-rw-r--r--   0        0        0      603 2024-04-23 14:06:10.192052 tinycss2-1.3.0/tinycss2/__init__.py
+-rw-r--r--   0        0        0    23499 2023-12-18 18:45:27.562893 tinycss2-1.3.0/tinycss2/ast.py
+-rw-r--r--   0        0        0     4768 2020-10-30 20:31:41.490813 tinycss2-1.3.0/tinycss2/bytes.py
+-rw-r--r--   0        0        0    11182 2024-02-10 23:57:33.474200 tinycss2-1.3.0/tinycss2/color3.py
+-rw-r--r--   0        0        0     3488 2024-03-19 11:38:47.869247 tinycss2-1.3.0/tinycss2/nth.py
+-rw-r--r--   0        0        0    19070 2024-03-19 11:38:47.870247 tinycss2-1.3.0/tinycss2/parser.py
+-rw-r--r--   0        0        0     4197 2024-03-19 11:38:47.870247 tinycss2-1.3.0/tinycss2/serializer.py
+-rw-r--r--   0        0        0    15293 2024-03-19 11:38:47.871247 tinycss2-1.3.0/tinycss2/tokenizer.py
+-rw-r--r--   0        0        0     2993 1970-01-01 00:00:00.000000 tinycss2-1.3.0/PKG-INFO
```

### Comparing `tinycss2-1.2.1/LICENSE` & `tinycss2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/README.rst` & `tinycss2-1.3.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 strings corresponding to these objects.
 
 Based on the CSS Syntax Level 3 specification, tinycss2 knows the grammar of
 CSS but doesn't know specific rules, properties or values supported in various
 CSS modules.
 
 * Free software: BSD license
-* For Python 3.7+, tested on CPython and PyPy
+* For Python 3.8+, tested on CPython and PyPy
 * Documentation: https://doc.courtbouillon.org/tinycss2
 * Changelog: https://github.com/Kozea/tinycss2/releases
 * Code, issues, tests: https://github.com/Kozea/tinycss2
 * Code of conduct: https://www.courtbouillon.org/code-of-conduct
 * Professional support: https://www.courtbouillon.org
 * Donation: https://opencollective.com/courtbouillon
```

### Comparing `tinycss2-1.2.1/docs/api_reference.rst` & `tinycss2-1.3.0/docs/api_reference.rst`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 functions.
 
 .. module:: tinycss2
 .. autofunction:: parse_stylesheet_bytes
 .. autofunction:: parse_stylesheet
 .. autofunction:: parse_rule_list
 .. autofunction:: parse_one_rule
+.. autofunction:: parse_blocks_contents
 .. autofunction:: parse_declaration_list
 .. autofunction:: parse_one_declaration
 .. autofunction:: parse_component_value_list
 .. autofunction:: parse_one_component_value
 
 
 Serialization
```

### Comparing `tinycss2-1.2.1/docs/changelog.rst` & `tinycss2-1.3.0/docs/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 Changelog
 =========
 
 
+Version 1.3.0
+-------------
+
+Released on 2024-04-23.
+
+* Support CSS nesting
+* Deprecate parse_declaration_list, use parse_blocks_contents instead
+
+
 Version 1.2.1
 -------------
 
 Released on 2022-10-18.
 
 * Fix tests included in the source tarball
```

### Comparing `tinycss2-1.2.1/docs/common_use_cases.rst` & `tinycss2-1.3.0/docs/common_use_cases.rst`

 * *Files 6% similar despite different names*

```diff
@@ -55,30 +55,30 @@
 -------------
 
 Parsing a list of declarations is possible from a list of tokens (given by the
 ``content`` attribute of :func:`tinycss2.parse_stylesheet` rules) or from a
 string (given by the ``style`` attribute of an HTML element, for example).
 
 The high-level function used to parse declarations is
-:func:`tinycss2.parse_declaration_list`.
+:func:`tinycss2.parse_blocks_contents`.
 
 .. code-block:: python
 
    rules = tinycss2.parse_stylesheet('body div {width: 50%;height: 50%}')
-   tinycss2.parse_declaration_list(rules[0].content)
+   tinycss2.parse_blocks_contents(rules[0].content)
    # [<Declaration width: …>, <Declaration height: …>]
 
-   tinycss2.parse_declaration_list('width: 50%;height: 50%')
+   tinycss2.parse_blocks_contents('width: 50%;height: 50%')
    # [<Declaration width: …>, <Declaration height: …>]
 
 You can then get the name and value of each declaration:
 
 .. code-block:: python
 
-   declarations = tinycss2.parse_declaration_list('width: 50%;height: 50%')
+   declarations = tinycss2.parse_blocks_contents('width: 50%;height: 50%')
    declarations[0].name, declarations[0].value
    # ('width', [<WhitespaceToken>, <PercentageToken 50%>])
 
 This function has the same ``skip_comments`` and ``skip_whitespace`` parameters
 as the ``parse_stylesheet*`` functions.
```

### Comparing `tinycss2-1.2.1/docs/conf.py` & `tinycss2-1.3.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 # a list of builtin themes.
 html_theme = 'sphinx_rtd_theme'
 
 html_theme_options = {
     'collapse_navigation': False,
 }
 
+# Favicon URL
+html_favicon = 'https://www.courtbouillon.org/static/images/favicon.png'
+
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = []
 
 # These paths are either relative to html_static_path
 # or fully qualified paths (eg. https://...)
```

### Comparing `tinycss2-1.2.1/docs/contribute.rst` & `tinycss2-1.3.0/docs/contribute.rst`

 * *Files 12% similar despite different names*

```diff
@@ -41,23 +41,20 @@
 Tests are stored in the ``tests`` folder at the top of the repository. They use
 the pytest_ library.
 
 You can launch tests using the following command::
 
   venv/bin/python -m pytest
 
-tinycss2 also uses isort_ to check imports and flake8_ to check the coding
-style::
+tinycss2 also uses ruff_ to check the coding style::
 
-  venv/bin/python -m isort . --check --diff
-  venv/bin/python -m flake8 --exclude tests/css-parsing-tests
+  venv/bin/python -m ruff check
 
 .. _pytest: https://docs.pytest.org/
-.. _isort: https://pycqa.github.io/isort/
-.. _flake8: https://flake8.pycqa.org/
+.. _ruff: https://docs.astral.sh/ruff/
 
 
 Documentation
 -------------
 
 Documentation is stored in the ``docs`` folder at the top of the repository. It
 relies on the Sphinx_ library.
```

### Comparing `tinycss2-1.2.1/docs/css_diagram_role.py` & `tinycss2-1.3.0/docs/css_diagram_role.py`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/docs/first_steps.rst` & `tinycss2-1.3.0/docs/first_steps.rst`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/docs/going_further.rst` & `tinycss2-1.3.0/docs/going_further.rst`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/docs/support.rst` & `tinycss2-1.3.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/pyproject.toml` & `tinycss2-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,30 +4,31 @@
 
 [project]
 name = 'tinycss2'
 description = 'A tiny CSS parser'
 keywords = ['css', 'parser']
 authors = [{name = 'Simon Sapin', email = 'simon.sapin@exyr.org'}]
 maintainers = [{name = 'CourtBouillon', email = 'contact@courtbouillon.org'}]
-requires-python = '>=3.7'
+requires-python = '>=3.8'
 readme = {file = 'README.rst', content-type = 'text/x-rst'}
 license = {file = 'LICENSE'}
 dependencies = ['webencodings >=0.4']
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
   'License :: OSI Approved :: BSD License',
   'Operating System :: OS Independent',
   'Programming Language :: Python',
   'Programming Language :: Python :: 3',
   'Programming Language :: Python :: 3 :: Only',
-  'Programming Language :: Python :: 3.7',
   'Programming Language :: Python :: 3.8',
   'Programming Language :: Python :: 3.9',
   'Programming Language :: Python :: 3.10',
+  'Programming Language :: Python :: 3.11',
+  'Programming Language :: Python :: 3.12',
   'Programming Language :: Python :: Implementation :: CPython',
   'Programming Language :: Python :: Implementation :: PyPy',
   'Topic :: Text Processing',
 ]
 dynamic = ['version']
 
 [project.urls]
@@ -36,15 +37,15 @@
 Code = 'https://github.com/Kozea/tinycss2/'
 Issues = 'https://github.com/Kozea/tinycss2/issues'
 Changelog = 'https://github.com/Kozea/tinycss2/releases'
 Donation = 'https://opencollective.com/courtbouillon'
 
 [project.optional-dependencies]
 doc = ['sphinx', 'sphinx_rtd_theme']
-test = ['pytest', 'isort', 'flake8']
+test = ['pytest', 'ruff']
 
 [tool.flit.sdist]
 exclude = ['.*']
 
 [tool.pytest.ini_options]
 norecursedirs = ['tests/css-parsing-tests']
 
@@ -52,11 +53,13 @@
 branch = true
 include = ['tests/*', 'tinycss2/*']
 
 [tool.coverage.report]
 exclude_lines = ['pragma: no cover', 'def __repr__', 'raise NotImplementedError']
 omit = ['.*']
 
-[tool.isort]
-default_section = 'FIRSTPARTY'
-multi_line_output = 4
-extend_skip = ['tests/css-parsing-tests']
+[tool.ruff]
+extend-exclude = ['tests/css-parsing-tests']
+
+[tool.ruff.lint]
+select = ['E', 'W', 'F', 'I', 'N', 'RUF']
+ignore = ['RUF001', 'RUF002', 'RUF003']
```

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/An+B.json` & `tinycss2-1.3.0/tests/css-parsing-tests/An+B.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/README.rst` & `tinycss2-1.3.0/tests/css-parsing-tests/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,20 @@
 
 ``declaration_list.json``
     Tests `Parse a list of declarations
     <http://dev.w3.org/csswg/css-syntax-3/#parse-a-list-of-declarations>`_.
     The Unicode input is represented by a JSON string,
     the output as an array of declarations_ and at-rules_.
 
+``blocks_contents.json``
+    Tests `Parse a block’s contents
+    <http://dev.w3.org/csswg/css-syntax-3/#parse-block-contents>`_.
+    The Unicode input is represented by a JSON string,
+    the output as an array of declarations_, at-rules_ and `qualified rules`_.
+
 ``one_declaration.json``
     Tests `Parse a declaration
     <http://dev.w3.org/csswg/css-syntax-3/#parse-a-declaration>`_.
     The Unicode input is represented by a JSON string,
     the output as a declaration_.
 
 ``one_rule.json``
```

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/color3.json` & `tinycss2-1.3.0/tests/css-parsing-tests/color3.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/color3_hsl.json` & `tinycss2-1.3.0/tests/css-parsing-tests/color3_hsl.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/color3_keywords.json` & `tinycss2-1.3.0/tests/css-parsing-tests/color3_keywords.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/component_value_list.json` & `tinycss2-1.3.0/tests/css-parsing-tests/component_value_list.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/declaration_list.json` & `tinycss2-1.3.0/tests/css-parsing-tests/declaration_list.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/make_color3_hsl.py` & `tinycss2-1.3.0/tests/css-parsing-tests/make_color3_hsl.py`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/make_color3_keywords.py` & `tinycss2-1.3.0/tests/css-parsing-tests/make_color3_keywords.py`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/one_component_value.json` & `tinycss2-1.3.0/tests/css-parsing-tests/one_component_value.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/one_declaration.json` & `tinycss2-1.3.0/tests/css-parsing-tests/one_declaration.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {'delete': '[43, 42]'}*

```diff
@@ -200,38 +200,9 @@
         [
             [
                 "ident",
                 "important"
             ]
         ],
         false
-    ],
-    "foo: 9000 @bar{ !important",
-    [
-        "declaration",
-        "foo",
-        [
-            " ",
-            [
-                "number",
-                "9000",
-                9000,
-                "integer"
-            ],
-            " ",
-            [
-                "at-keyword",
-                "bar"
-            ],
-            [
-                "{}",
-                " ",
-                "!",
-                [
-                    "ident",
-                    "important"
-                ]
-            ]
-        ],
-        false
     ]
 ]
```

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/one_rule.json` & `tinycss2-1.3.0/tests/css-parsing-tests/one_rule.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/rule_list.json` & `tinycss2-1.3.0/tests/css-parsing-tests/rule_list.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/stylesheet.json` & `tinycss2-1.3.0/tests/css-parsing-tests/stylesheet.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/css-parsing-tests/stylesheet_bytes.json` & `tinycss2-1.3.0/tests/css-parsing-tests/stylesheet_bytes.json`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tests/test_tinycss2.py` & `tinycss2-1.3.0/tests/test_tinycss2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import functools
 import json
 import pprint
 from pathlib import Path
 
 import pytest
-from tinycss2 import (
-    parse_component_value_list, parse_declaration_list,
-    parse_one_component_value, parse_one_declaration, parse_one_rule,
-    parse_rule_list, parse_stylesheet, parse_stylesheet_bytes, serialize)
-from tinycss2.ast import (
-    AtKeywordToken, AtRule, Comment, CurlyBracketsBlock, Declaration,
-    DimensionToken, FunctionBlock, HashToken, IdentToken, LiteralToken,
-    NumberToken, ParenthesesBlock, ParseError, PercentageToken, QualifiedRule,
-    SquareBracketsBlock, StringToken, UnicodeRangeToken, URLToken,
-    WhitespaceToken)
+from webencodings import Encoding, lookup
+
+from tinycss2 import (  # isort:skip
+    parse_blocks_contents, parse_component_value_list, parse_declaration_list,
+    parse_one_component_value, parse_one_declaration, parse_one_rule, parse_rule_list,
+    parse_stylesheet, parse_stylesheet_bytes, serialize)
+from tinycss2.ast import (  # isort:skip
+    AtKeywordToken, AtRule, Comment, CurlyBracketsBlock, Declaration, DimensionToken,
+    FunctionBlock, HashToken, IdentToken, LiteralToken, NumberToken, ParenthesesBlock,
+    ParseError, PercentageToken, QualifiedRule, SquareBracketsBlock, StringToken,
+    UnicodeRangeToken, URLToken, WhitespaceToken)
 from tinycss2.color3 import RGBA, parse_color
 from tinycss2.nth import parse_nth
-from webencodings import Encoding, lookup
 
 
 def generic(func):
     implementations = func()
 
     @functools.wraps(func)
     def run(value):
@@ -35,44 +35,43 @@
         return [
             t.representation, t.value,
             'integer' if t.int_value is not None else 'number']
     return {
         type(None): lambda _: None,
         str: lambda s: s,
         int: lambda s: s,
-        list: lambda l: [to_json(el) for el in l],
-        tuple: lambda l: [to_json(el) for el in l],
+        list: lambda li: [to_json(el) for el in li],
+        tuple: lambda li: [to_json(el) for el in li],
         Encoding: lambda e: e.name,
         ParseError: lambda e: ['error', e.kind],
 
         Comment: lambda t: '/* … */',
         WhitespaceToken: lambda t: ' ',
         LiteralToken: lambda t: t.value,
         IdentToken: lambda t: ['ident', t.value],
         AtKeywordToken: lambda t: ['at-keyword', t.value],
-        HashToken: lambda t: ['hash', t.value,
-                              'id' if t.is_identifier else 'unrestricted'],
+        HashToken: lambda t: [
+            'hash', t.value, 'id' if t.is_identifier else 'unrestricted'],
         StringToken: lambda t: ['string', t.value],
         URLToken: lambda t: ['url', t.value],
-        NumberToken: lambda t: ['number'] + numeric(t),
-        PercentageToken: lambda t: ['percentage'] + numeric(t),
-        DimensionToken: lambda t: ['dimension'] + numeric(t) + [t.unit],
+        NumberToken: lambda t: ['number', *numeric(t)],
+        PercentageToken: lambda t: ['percentage', *numeric(t)],
+        DimensionToken: lambda t: ['dimension', *numeric(t), t.unit],
         UnicodeRangeToken: lambda t: ['unicode-range', t.start, t.end],
 
-        CurlyBracketsBlock: lambda t: ['{}'] + to_json(t.content),
-        SquareBracketsBlock: lambda t: ['[]'] + to_json(t.content),
-        ParenthesesBlock: lambda t: ['()'] + to_json(t.content),
-        FunctionBlock: lambda t: ['function', t.name] + to_json(t.arguments),
-
-        Declaration: lambda d: ['declaration', d.name,
-                                to_json(d.value), d.important],
-        AtRule: lambda r: ['at-rule', r.at_keyword, to_json(r.prelude),
-                           to_json(r.content)],
-        QualifiedRule: lambda r: ['qualified rule', to_json(r.prelude),
-                                  to_json(r.content)],
+        CurlyBracketsBlock: lambda t: ['{}', *to_json(t.content)],
+        SquareBracketsBlock: lambda t: ['[]', *to_json(t.content)],
+        ParenthesesBlock: lambda t: ['()', *to_json(t.content)],
+        FunctionBlock: lambda t: ['function', t.name, *to_json(t.arguments)],
+
+        Declaration: lambda d: ['declaration', d.name, to_json(d.value), d.important],
+        AtRule: lambda r: [
+            'at-rule', r.at_keyword, to_json(r.prelude), to_json(r.content)],
+        QualifiedRule: lambda r: [
+            'qualified rule', to_json(r.prelude), to_json(r.content)],
 
         RGBA: lambda v: [round(c, 10) for c in v],
     }
 
 
 def load_json(filename):
     path = Path(__file__).parent / 'css-parsing-tests' / filename
@@ -109,14 +108,19 @@
 
 @json_test()
 def test_declaration_list(input):
     return parse_declaration_list(input, **SKIP)
 
 
 @json_test()
+def test_blocks_contents(input):
+    return parse_blocks_contents(input, **SKIP)
+
+
+@json_test()
 def test_one_declaration(input):
     return parse_one_declaration(input, skip_comments=True)
 
 
 @json_test()
 def test_stylesheet(input):
     return parse_stylesheet(input, **SKIP)
@@ -209,15 +213,15 @@
     source = '@import "a.css"; foo#bar.baz { color: red } /**/ @media print{}'
     rules = parse_rule_list(source)
     assert serialize(rules) == source
 
 
 def test_serialize_declarations():
     source = 'color: #123; /**/ @top-left {} width:7px !important;'
-    rules = parse_declaration_list(source)
+    rules = parse_blocks_contents(source)
     assert serialize(rules) == source
 
 
 def test_serialize_rules_with_functions():
     source = '''
         foo#bar.baz {
             background: url();
```

### Comparing `tinycss2-1.2.1/tinycss2/__init__.py` & `tinycss2-1.3.0/tinycss2/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 Python objects representing tokens and blocks, and generate CSS strings
 corresponding to these objects.
 
 """
 
 from .bytes import parse_stylesheet_bytes  # noqa
 from .parser import (  # noqa
-    parse_declaration_list, parse_one_component_value, parse_one_declaration,
-    parse_one_rule, parse_rule_list, parse_stylesheet)
+    parse_blocks_contents, parse_declaration_list, parse_one_component_value,
+    parse_one_declaration, parse_one_rule, parse_rule_list, parse_stylesheet)
 from .serializer import serialize, serialize_identifier  # noqa
 from .tokenizer import parse_component_value_list  # noqa
 
-VERSION = __version__ = '1.2.1'
+VERSION = __version__ = '1.3.0'
```

### Comparing `tinycss2-1.2.1/tinycss2/ast.py` & `tinycss2-1.3.0/tinycss2/ast.py`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tinycss2/bytes.py` & `tinycss2-1.3.0/tinycss2/bytes.py`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tinycss2/color3.py` & `tinycss2-1.3.0/tinycss2/color3.py`

 * *Files identical despite different names*

### Comparing `tinycss2-1.2.1/tinycss2/nth.py` & `tinycss2-1.3.0/tinycss2/nth.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
           token.representation[0] in '-+'):
         return parse_end(tokens, a, token.int_value)
 
 
 def parse_signless_b(tokens, a, b_sign):
     token = _next_significant(tokens)
     if (token.type == 'number' and token.is_integer and
-            not token.representation[0] in '-+'):
+            token.representation[0] not in '-+'):
         return parse_end(tokens, a, b_sign * token.int_value)
 
 
 def parse_end(tokens, a, b):
     if _next_significant(tokens) is None:
         return (a, b)
```

### Comparing `tinycss2-1.2.1/tinycss2/parser.py` & `tinycss2-1.3.0/tinycss2/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from itertools import chain
+
 from .ast import AtRule, Declaration, ParseError, QualifiedRule
 from .tokenizer import parse_component_value_list
 
 
 def _to_token_iterator(input, skip_comments=False):
     """Iterate component values out of string or component values iterable.
 
     :type input: :obj:`str` or :term:`iterable`
     :param input: A string or an iterable of :term:`component values`.
     :type skip_comments: :obj:`bool`
     :param skip_comments: If the input is a string, ignore all CSS comments.
     :returns: An iterator yielding :term:`component values`.
 
     """
-    # Accept ASCII-only byte strings on Python 2, with implicit conversion.
     if isinstance(input, str):
         input = parse_component_value_list(input, skip_comments)
     return iter(input)
 
 
 def _next_significant(tokens):
     """Return the next significant (neither whitespace or comment) token.
@@ -79,83 +80,195 @@
     tokens = _to_token_iterator(input, skip_comments)
     first_token = _next_significant(tokens)
     if first_token is None:
         return ParseError(1, 1, 'empty', 'Input is empty')
     return _parse_declaration(first_token, tokens)
 
 
-def _parse_declaration(first_token, tokens):
+def _consume_remnants(input, nested):
+    for token in input:
+        if token == ';':
+            return
+        elif nested and token == '}':
+            return
+
+
+def _parse_declaration(first_token, tokens, nested=True):
     """Parse a declaration.
 
     Consume :obj:`tokens` until the end of the declaration or the first error.
 
     :type first_token: :term:`component value`
     :param first_token: The first component value of the rule.
     :type tokens: :term:`iterator`
     :param tokens: An iterator yielding :term:`component values`.
+    :type nested: :obj:`bool`
+    :param nested: Whether the declaration is nested or top-level.
     :returns:
         A :class:`~tinycss2.ast.Declaration`
         or :class:`~tinycss2.ast.ParseError`.
 
     """
     name = first_token
     if name.type != 'ident':
-        return ParseError(name.source_line, name.source_column, 'invalid',
-                          'Expected <ident> for declaration name, got %s.'
-                          % name.type)
+        _consume_remnants(tokens, nested)
+        return ParseError(
+            name.source_line, name.source_column, 'invalid',
+            f'Expected <ident> for declaration name, got {name.type}.')
 
     colon = _next_significant(tokens)
     if colon is None:
-        return ParseError(name.source_line, name.source_column, 'invalid',
-                          "Expected ':' after declaration name, got EOF")
+        _consume_remnants(tokens, nested)
+        return ParseError(
+            name.source_line, name.source_column, 'invalid',
+            "Expected ':' after declaration name, got EOF")
     elif colon != ':':
-        return ParseError(colon.source_line, colon.source_column, 'invalid',
-                          "Expected ':' after declaration name, got %s."
-                          % colon.type)
+        _consume_remnants(tokens, nested)
+        return ParseError(
+            colon.source_line, colon.source_column, 'invalid',
+            "Expected ':' after declaration name, got {colon.type}.")
 
     value = []
     state = 'value'
+    contains_non_whitespace = False
+    contains_simple_block = False
     for i, token in enumerate(tokens):
         if state == 'value' and token == '!':
             state = 'bang'
             bang_position = i
-        elif state == 'bang' and token.type == 'ident' \
-                and token.lower_value == 'important':
+        elif (state == 'bang' and token.type == 'ident'
+                and token.lower_value == 'important'):
             state = 'important'
         elif token.type not in ('whitespace', 'comment'):
             state = 'value'
+            if token.type == '{} block':
+                if contains_non_whitespace:
+                    contains_simple_block = True
+                else:
+                    contains_non_whitespace = True
+            else:
+                contains_non_whitespace = True
         value.append(token)
 
     if state == 'important':
         del value[bang_position:]
 
-    return Declaration(name.source_line, name.source_column, name.value,
-                       name.lower_value, value, state == 'important')
+    # TODO: Handle custom property names
+
+    if contains_simple_block and contains_non_whitespace:
+        return ParseError(
+            colon.source_line, colon.source_column, 'invalid',
+            'Declaration contains {} block')
+
+    # TODO: Handle unicode-range
+
+    return Declaration(
+        name.source_line, name.source_column, name.value, name.lower_value,
+        value, state == 'important')
+
+
+def _consume_blocks_content(first_token, tokens):
+    """Consume declaration or nested rule."""
+    declaration_tokens = []
+    semicolon_token = []
+    if first_token != ';' and first_token.type != '{} block':
+        for token in tokens:
+            if token == ';':
+                semicolon_token.append(token)
+                break
+            declaration_tokens.append(token)
+            if token.type == '{} block':
+                break
+    declaration = _parse_declaration(
+        first_token, iter(declaration_tokens), nested=True)
+    if declaration.type == 'declaration':
+        return declaration
+    else:
+        tokens = chain(declaration_tokens, semicolon_token, tokens)
+        return _consume_qualified_rule(first_token, tokens, stop_token=';', nested=True)
 
 
 def _consume_declaration_in_list(first_token, tokens):
-    """Like :func:`_parse_declaration`, but stop at the first ``;``."""
+    """Like :func:`_parse_declaration`, but stop at the first ``;``.
+
+    Deprecated, use :func:`_consume_blocks_content` instead.
+
+    """
     other_declaration_tokens = []
     for token in tokens:
         if token == ';':
             break
         other_declaration_tokens.append(token)
     return _parse_declaration(first_token, iter(other_declaration_tokens))
 
 
+def parse_blocks_contents(input, skip_comments=False, skip_whitespace=False):
+    """Parse a block’s contents.
+
+    This is used e.g. for the :attr:`~tinycss2.ast.QualifiedRule.content`
+    of a style rule or ``@page`` rule, or for the ``style`` attribute of an
+    HTML element.
+
+    In contexts that don’t expect any at-rule and/or qualified rule,
+    all :class:`~tinycss2.ast.AtRule` and/or
+    :class:`~tinycss2.ast.QualifiedRule` objects should simply be rejected as
+    invalid.
+
+    :type input: :obj:`str` or :term:`iterable`
+    :param input: A string or an iterable of :term:`component values`.
+    :type skip_comments: :obj:`bool`
+    :param skip_comments:
+        Ignore CSS comments at the top-level of the list.
+        If the input is a string, ignore all comments.
+    :type skip_whitespace: :obj:`bool`
+    :param skip_whitespace:
+        Ignore whitespace at the top-level of the list.
+        Whitespace is still preserved
+        in the :attr:`~tinycss2.ast.Declaration.value` of declarations
+        and the :attr:`~tinycss2.ast.AtRule.prelude`
+        and :attr:`~tinycss2.ast.AtRule.content` of at-rules.
+    :returns:
+        A list of
+        :class:`~tinycss2.ast.Declaration`,
+        :class:`~tinycss2.ast.AtRule`,
+        :class:`~tinycss2.ast.QualifiedRule`,
+        :class:`~tinycss2.ast.Comment` (if ``skip_comments`` is false),
+        :class:`~tinycss2.ast.WhitespaceToken`
+        (if ``skip_whitespace`` is false),
+        and :class:`~tinycss2.ast.ParseError` objects
+
+    """
+    tokens = _to_token_iterator(input, skip_comments)
+    result = []
+    for token in tokens:
+        if token.type == 'whitespace':
+            if not skip_whitespace:
+                result.append(token)
+        elif token.type == 'comment':
+            if not skip_comments:
+                result.append(token)
+        elif token.type == 'at-keyword':
+            result.append(_consume_at_rule(token, tokens))
+        elif token != ';':
+            result.append(_consume_blocks_content(token, tokens))
+    return result
+
+
 def parse_declaration_list(input, skip_comments=False, skip_whitespace=False):
     """Parse a :diagram:`declaration list` (which may also contain at-rules).
 
+    Deprecated and removed from CSS Syntax Level 3. Use
+    :func:`parse_blocks_contents` instead.
+
     This is used e.g. for the :attr:`~tinycss2.ast.QualifiedRule.content`
-    of a style rule or ``@page`` rule,
-    or for the ``style`` attribute of an HTML element.
+    of a style rule or ``@page`` rule, or for the ``style`` attribute of an
+    HTML element.
 
-    In contexts that don’t expect any at-rule,
-    all :class:`~tinycss2.ast.AtRule` objects
-    should simply be rejected as invalid.
+    In contexts that don’t expect any at-rule, all
+    :class:`~tinycss2.ast.AtRule` objects should simply be rejected as invalid.
 
     :type input: :obj:`str` or :term:`iterable`
     :param input: A string or an iterable of :term:`component values`.
     :type skip_comments: :obj:`bool`
     :param skip_comments:
         Ignore CSS comments at the top-level of the list.
         If the input is a string, ignore all comments.
@@ -225,14 +338,17 @@
             'Expected a single rule, got %s after the first rule.' % next.type)
     return rule
 
 
 def parse_rule_list(input, skip_comments=False, skip_whitespace=False):
     """Parse a non-top-level :diagram:`rule list`.
 
+    Deprecated and removed from CSS Syntax. Use :func:`parse_blocks_content`
+    instead.
+
     This is used for parsing the :attr:`~tinycss2.ast.AtRule.content`
     of nested rules like ``@media``.
     This differs from :func:`parse_stylesheet` in that
     top-level ``<!--`` and ``-->`` tokens are not ignored.
 
     :type input: :obj:`str` or :term:`iterable`
     :param input: A string or an iterable of :term:`component values`.
@@ -328,50 +444,85 @@
         A :class:`~tinycss2.ast.QualifiedRule`,
         :class:`~tinycss2.ast.AtRule`,
         or :class:`~tinycss2.ast.ParseError`.
 
     """
     if first_token.type == 'at-keyword':
         return _consume_at_rule(first_token, tokens)
-    if first_token.type == '{} block':
-        prelude = []
-        block = first_token
-    else:
-        prelude = [first_token]
-        for token in tokens:
-            if token.type == '{} block':
-                block = token
-                break
-            prelude.append(token)
-        else:
-            return ParseError(
-                prelude[-1].source_line, prelude[-1].source_column, 'invalid',
-                'EOF reached before {} block for a qualified rule.')
-    return QualifiedRule(first_token.source_line, first_token.source_column,
-                         prelude, block.content)
+    return _consume_qualified_rule(first_token, tokens)
 
 
 def _consume_at_rule(at_keyword, tokens):
     """Parse an at-rule.
 
     Consume just enough of :obj:`tokens` for this rule.
 
     :type at_keyword: :class:`AtKeywordToken`
     :param at_keyword: The at-rule keyword token starting this rule.
     :type tokens: :term:`iterator`
     :param tokens: An iterator yielding :term:`component values`.
+    :type nested: :obj:`bool`
+    :param nested: Whether the at-rule is nested or top-level.
     :returns:
         A :class:`~tinycss2.ast.QualifiedRule`,
         or :class:`~tinycss2.ast.ParseError`.
 
     """
     prelude = []
     content = None
     for token in tokens:
         if token.type == '{} block':
+            # TODO: handle nested at-rules
+            # https://drafts.csswg.org/css-syntax-3/#consume-at-rule
             content = token.content
             break
         elif token == ';':
             break
         prelude.append(token)
-    return AtRule(at_keyword.source_line, at_keyword.source_column,
-                  at_keyword.value, at_keyword.lower_value, prelude, content)
+    return AtRule(
+        at_keyword.source_line, at_keyword.source_column, at_keyword.value,
+        at_keyword.lower_value, prelude, content)
+
+
+def _rule_error(token, name):
+    """Create rule parse error raised because of given token."""
+    return ParseError(
+        token.source_line, token.source_column, 'invalid',
+        f'{name} reached before {{}} block for a qualified rule.')
+
+
+def _consume_qualified_rule(first_token, tokens, nested=False,
+                            stop_token=None):
+    """Consume a qualified rule.
+
+    Consume just enough of :obj:`tokens` for this rule.
+
+    :type first_token: :term:`component value`
+    :param first_token: The first component value of the rule.
+    :type tokens: :term:`iterator`
+    :param tokens: An iterator yielding :term:`component values`.
+    :type nested: :obj:`bool`
+    :param nested: Whether the rule is nested or top-level.
+    :type stop_token: :class:`~tinycss2.ast.Node`
+    :param stop_token: A token that ends rule parsing when met.
+
+    """
+    if first_token == stop_token:
+        return _rule_error(first_token, 'Stop token')
+    if first_token.type == '{} block':
+        prelude = []
+        block = first_token
+    else:
+        prelude = [first_token]
+        for token in tokens:
+            if token == stop_token:
+                return _rule_error(token, 'Stop token')
+            if token.type == '{} block':
+                block = token
+                # TODO: handle special case for CSS variables (using "nested")
+                # https://drafts.csswg.org/css-syntax-3/#consume-qualified-rule
+                break
+            prelude.append(token)
+        else:
+            return _rule_error(prelude[-1], 'EOF')
+    return QualifiedRule(
+        first_token.source_line, first_token.source_column, prelude, block.content)
```

### Comparing `tinycss2-1.2.1/tinycss2/serializer.py` & `tinycss2-1.3.0/tinycss2/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,15 @@
         if serialization_type == 'declaration':
             write(';')
         previous_type = serialization_type
 
 
 BAD_PAIRS = set(
     [(a, b)
-        for a in ('ident', 'at-keyword', 'hash', 'dimension', '#', '-',
-                  'number')
+        for a in ('ident', 'at-keyword', 'hash', 'dimension', '#', '-', 'number')
         for b in ('ident', 'function', 'url', 'number', 'percentage',
                   'dimension', 'unicode-range')] +
     [(a, b)
         for a in ('ident', 'at-keyword', 'hash', 'dimension')
         for b in ('-', '-->')] +
     [(a, b)
         for a in ('#', '-', 'number', '@')
```

### Comparing `tinycss2-1.2.1/tinycss2/tokenizer.py` & `tinycss2-1.3.0/tinycss2/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 import sys
 
 from webencodings import ascii_lower
 
-from .ast import (
+from .ast import (  # isort: skip
     AtKeywordToken, Comment, CurlyBracketsBlock, DimensionToken, FunctionBlock,
-    HashToken, IdentToken, LiteralToken, NumberToken, ParenthesesBlock,
-    ParseError, PercentageToken, SquareBracketsBlock, StringToken,
-    UnicodeRangeToken, URLToken, WhitespaceToken)
+    HashToken, IdentToken, LiteralToken, NumberToken, ParenthesesBlock, ParseError,
+    PercentageToken, SquareBracketsBlock, StringToken, UnicodeRangeToken, URLToken,
+    WhitespaceToken)
 from .serializer import serialize_string_value, serialize_url
 
 _NUMBER_RE = re.compile(r'[-+]?([0-9]*\.)?[0-9]+([eE][+-]?[0-9]+)?')
 _HEX_ESCAPE_RE = re.compile(r'([0-9A-Fa-f]{1,6})[ \n\t]?')
 
 
 def parse_component_value_list(css, skip_comments=False):
@@ -104,19 +104,17 @@
             int_value = int(repr_) if not any(match.groups()) else None
             if pos < length and _is_ident_start(css, pos):
                 unit, pos = _consume_ident(css, pos)
                 tokens.append(DimensionToken(
                     line, column, value, int_value, repr_, unit))
             elif css.startswith('%', pos):
                 pos += 1
-                tokens.append(PercentageToken(
-                    line, column, value, int_value, repr_))
+                tokens.append(PercentageToken(line, column, value, int_value, repr_))
             else:
-                tokens.append(NumberToken(
-                    line, column, value, int_value, repr_))
+                tokens.append(NumberToken(line, column, value, int_value, repr_))
         elif c == '@':
             pos += 1
             if pos < length and _is_ident_start(css, pos):
                 value, pos = _consume_ident(css, pos)
                 tokens.append(AtKeywordToken(line, column, value))
             else:
                 tokens.append(LiteralToken(line, column, '@'))
@@ -171,20 +169,18 @@
                 tokens.append(StringToken(line, column, value, repr))
             if error is not None:
                 tokens.append(ParseError(line, column, *error))
         elif css.startswith('/*', pos):  # Comment
             pos = css.find('*/', pos + 2)
             if pos == -1:
                 if not skip_comments:
-                    tokens.append(
-                        Comment(line, column, css[token_start_pos + 2:]))
+                    tokens.append(Comment(line, column, css[token_start_pos + 2:]))
                 break
             if not skip_comments:
-                tokens.append(
-                    Comment(line, column, css[token_start_pos + 2:pos]))
+                tokens.append(Comment(line, column, css[token_start_pos + 2:pos]))
             pos += 2
         elif css.startswith('<!--', pos):
             tokens.append(LiteralToken(line, column, '<!--'))
             pos += 4
         elif css.startswith('||', pos):
             tokens.append(LiteralToken(line, column, '||'))
             pos += 2
@@ -215,16 +211,15 @@
     # https://drafts.csswg.org/css-syntax/#would-start-an-identifier
     if _is_name_start(css, pos):
         return True
     elif css[pos] == '-':
         pos += 1
         return (
             # Name-start code point or hyphen:
-            (pos < len(css) and (
-                _is_name_start(css, pos) or css[pos] == '-')) or
+            (pos < len(css) and (_is_name_start(css, pos) or css[pos] == '-')) or
             # Valid escape:
             (css.startswith('\\', pos) and not css.startswith('\\\n', pos)))
     elif css[pos] == '\\':
         return not css.startswith('\\\n', pos)
     return False
```

### Comparing `tinycss2-1.2.1/PKG-INFO` & `tinycss2-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: tinycss2
-Version: 1.2.1
+Version: 1.3.0
 Summary: A tiny CSS parser
 Keywords: css,parser
 Author-email: Simon Sapin <simon.sapin@exyr.org>
 Maintainer-email: CourtBouillon <contact@courtbouillon.org>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Text Processing
 Requires-Dist: webencodings >=0.4
 Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx_rtd_theme ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
-Requires-Dist: isort ; extra == "test"
-Requires-Dist: flake8 ; extra == "test"
+Requires-Dist: ruff ; extra == "test"
 Project-URL: Changelog, https://github.com/Kozea/tinycss2/releases
 Project-URL: Code, https://github.com/Kozea/tinycss2/
 Project-URL: Documentation, https://doc.courtbouillon.org/tinycss2/
 Project-URL: Donation, https://opencollective.com/courtbouillon
 Project-URL: Homepage, https://www.courtbouillon.org/tinycss2
 Project-URL: Issues, https://github.com/Kozea/tinycss2/issues
 Provides-Extra: doc
@@ -41,15 +41,15 @@
 strings corresponding to these objects.
 
 Based on the CSS Syntax Level 3 specification, tinycss2 knows the grammar of
 CSS but doesn't know specific rules, properties or values supported in various
 CSS modules.
 
 * Free software: BSD license
-* For Python 3.7+, tested on CPython and PyPy
+* For Python 3.8+, tested on CPython and PyPy
 * Documentation: https://doc.courtbouillon.org/tinycss2
 * Changelog: https://github.com/Kozea/tinycss2/releases
 * Code, issues, tests: https://github.com/Kozea/tinycss2
 * Code of conduct: https://www.courtbouillon.org/code-of-conduct
 * Professional support: https://www.courtbouillon.org
 * Donation: https://opencollective.com/courtbouillon
```

