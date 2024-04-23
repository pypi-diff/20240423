# Comparing `tmp/rst_linker-2.5.0.tar.gz` & `tmp/rst_linker-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rst_linker-2.5.0.tar", last modified: Mon Apr 22 14:17:20 2024, max compression
+gzip compressed data, was "rst_linker-2.6.0.tar", last modified: Tue Apr 23 20:28:56 2024, max compression
```

## Comparing `rst_linker-2.5.0.tar` & `rst_linker-2.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:17:20.321202 rst_linker-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-22 14:17:01.000000 rst_linker-2.5.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 14:17:01.000000 rst_linker-2.5.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:17:20.317202 rst_linker-2.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 14:17:01.000000 rst_linker-2.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:17:20.317202 rst_linker-2.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-22 14:17:01.000000 rst_linker-2.5.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 14:17:01.000000 rst_linker-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-22 14:17:01.000000 rst_linker-2.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-22 14:17:01.000000 rst_linker-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-22 14:17:01.000000 rst_linker-2.5.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-22 14:17:20.321202 rst_linker-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-22 14:17:01.000000 rst_linker-2.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:17:20.321202 rst_linker-2.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-22 14:17:01.000000 rst_linker-2.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-22 14:17:01.000000 rst_linker-2.5.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-22 14:17:01.000000 rst_linker-2.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 14:17:01.000000 rst_linker-2.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-22 14:17:01.000000 rst_linker-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-22 14:17:01.000000 rst_linker-2.5.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:17:20.321202 rst_linker-2.5.0/rst/
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-22 14:17:01.000000 rst_linker-2.5.0/rst/linker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 14:17:20.321202 rst_linker-2.5.0/rst.linker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-22 14:17:20.000000 rst_linker-2.5.0/rst.linker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-22 14:17:20.000000 rst_linker-2.5.0/rst.linker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 14:17:20.000000 rst_linker-2.5.0/rst.linker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-22 14:17:20.000000 rst_linker-2.5.0/rst.linker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-22 14:17:20.000000 rst_linker-2.5.0/rst.linker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-22 14:17:01.000000 rst_linker-2.5.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 14:17:20.321202 rst_linker-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-22 14:17:01.000000 rst_linker-2.5.0/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-22 14:17:01.000000 rst_linker-2.5.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-22 14:17:01.000000 rst_linker-2.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:28:56.209765 rst_linker-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 20:28:30.000000 rst_linker-2.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-23 20:28:30.000000 rst_linker-2.6.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:28:56.205765 rst_linker-2.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 20:28:30.000000 rst_linker-2.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:28:56.205765 rst_linker-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-23 20:28:30.000000 rst_linker-2.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 20:28:30.000000 rst_linker-2.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-23 20:28:30.000000 rst_linker-2.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-23 20:28:30.000000 rst_linker-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-23 20:28:30.000000 rst_linker-2.6.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-23 20:28:56.209765 rst_linker-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-23 20:28:30.000000 rst_linker-2.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:28:56.209765 rst_linker-2.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-23 20:28:30.000000 rst_linker-2.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 20:28:30.000000 rst_linker-2.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-23 20:28:30.000000 rst_linker-2.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 20:28:30.000000 rst_linker-2.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-23 20:28:30.000000 rst_linker-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-23 20:28:30.000000 rst_linker-2.6.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:28:56.209765 rst_linker-2.6.0/rst/
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-23 20:28:30.000000 rst_linker-2.6.0/rst/linker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:28:56.209765 rst_linker-2.6.0/rst.linker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-23 20:28:56.000000 rst_linker-2.6.0/rst.linker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 20:28:56.000000 rst_linker-2.6.0/rst.linker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:28:56.000000 rst_linker-2.6.0/rst.linker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 20:28:56.000000 rst_linker-2.6.0/rst.linker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 20:28:56.000000 rst_linker-2.6.0/rst.linker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-23 20:28:30.000000 rst_linker-2.6.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:28:56.209765 rst_linker-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-23 20:28:30.000000 rst_linker-2.6.0/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 20:28:30.000000 rst_linker-2.6.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 20:28:30.000000 rst_linker-2.6.0/tox.ini
```

### Comparing `rst_linker-2.5.0/.github/workflows/main.yml` & `rst_linker-2.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `rst_linker-2.5.0/LICENSE` & `rst_linker-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rst_linker-2.5.0/NEWS.rst` & `rst_linker-2.6.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v2.6.0
+======
+
+Features
+--------
+
+- Leverage jaraco.vcs for retrieving timestamps from the history.
+
+
 v2.5.0
 ======
 
 Features
 --------
 
 - Convert to PEP 420 native namespace package.
```

### Comparing `rst_linker-2.5.0/PKG-INFO` & `rst_linker-2.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: rst.linker
-Version: 2.5.0
+Version: 2.6.0
 Summary: Tools for adding metadata and hyperlinks to reStructuredText
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/rst.linker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Sphinx :: Extension
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: python-dateutil
-Requires-Dist: importlib_metadata; python_version < "3.8"
+Requires-Dist: jaraco.vcs>=2.1
+Requires-Dist: jaraco.context
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: path; extra == "testing"
-Requires-Dist: types-python-dateutil; extra == "testing"
+Requires-Dist: pytest-subprocess; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
```

### Comparing `rst_linker-2.5.0/README.rst` & `rst_linker-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `rst_linker-2.5.0/docs/conf.py` & `rst_linker-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rst_linker-2.5.0/pyproject.toml` & `rst_linker-2.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python :: 3",
 	"Programming Language :: Python :: 3 :: Only",
 	"Framework :: Sphinx :: Extension",
 ]
 requires-python = ">=3.8"
 dependencies = [
-	"python-dateutil",
-	'importlib_metadata; python_version < "3.8"',
+	"jaraco.vcs >= 2.1",
+	"jaraco.context",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/jaraco/rst.linker"
 
 [project.optional-dependencies]
@@ -35,15 +35,15 @@
 	"pytest-cov",
 	'pytest-mypy; python_implementation != "PyPy"', # workaround for jaraco/skeleton#22
 	"pytest-enabler >= 2.2",
 	"pytest-ruff >= 0.2.1",
 
 	# local
 	"path",
-	"types-python-dateutil",
+	"pytest-subprocess",
 ]
 docs = [
 	# upstream
 	"sphinx >= 3.5",
 	"jaraco.packaging >= 9.3",
 	"rst.linker >= 1.9",
 	"furo",
```

### Comparing `rst_linker-2.5.0/pytest.ini` & `rst_linker-2.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `rst_linker-2.5.0/rst/linker.py` & `rst_linker-2.6.0/rst/linker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """
 Sphinx plugin to add links and timestamps to the changelog.
 """
 
-import re
-import os
-import operator
-import subprocess
-import io
 import functools
+import operator
+import os
+import re
+from collections.abc import Mapping
+from importlib import metadata
 
-try:
-    import importlib.metadata as importlib_metadata  # type: ignore
-except ImportError:
-    import importlib_metadata  # type: ignore
-
-import dateutil.parser
+from jaraco import vcs
+from jaraco.context import suppress
 
 
 class Repl:
     @classmethod
     def from_defn(cls, defn):
         "Return the first Repl subclass that works with this"
         instances = (subcl(defn) for subcl in cls.__subclasses__())
@@ -100,54 +96,32 @@
             return text
         ns = match.groupdict()
         ns.update(vars(self))
         ns.update(replacer_vars)
         return self.with_scm.format(text=text, rev=rev, **ns)
 
     @staticmethod
+    @suppress(Exception)
     def _get_scm_info_for(scm_version):
-        scm = 'hg' if os.path.isdir('.hg') else 'git'
-        commands = dict(
-            hg=[
-                'hg',
-                'log',
-                '-l',
-                '1',
-                '--template',
-                '{date|isodate}',
-                '-r',
-                scm_version,
-            ],
-            git=['git', 'log', '-1', '--format=%ai', scm_version],
-        )
-        cmd = commands[scm]
-        try:
-            with open(os.devnull, 'w', encoding='utf-8') as devnull:
-                out = subprocess.check_output(
-                    cmd, stderr=devnull, text=True, encoding='utf-8'
-                )
-                ts = out.strip()
-            return dict(timestamp=dateutil.parser.parse(ts))
-        except Exception:
-            pass
+        return dict(timestamp=vcs.repo().get_timestamp(scm_version))
 
     def __bool__(self):
         return 'with_scm' in vars(self)
 
 
 class Replacer(list):
     @staticmethod
     def load(filename):
         defn = dict()
         with open(filename) as stream:
             exec(stream.read(), defn)
         return defn
 
     @classmethod
-    def from_definition(cls, defn, names={}):
+    def from_definition(cls, defn, names: Mapping = {}):
         """
         A definition may contain the following members:
 
         - using: a dictionary of variables available for substitution
         - replace: a list of replacement definitions.
         """
         repls = map(Repl.from_defn, defn.get('replace', []))
@@ -164,26 +138,24 @@
     def replace(self, match):
         text = match.group(0)
         # determine which replacement matched
         repl = next(repl for repl in self if repl.matches(text))
         return repl.replace(match, vars(self))
 
     def write_links(self, source, target):
-        with io.open(source, encoding='utf-8') as source:
+        with open(source, encoding='utf-8') as source:
             out = self.run(source.read())
-        with io.open(target, 'w', encoding='utf-8') as dest:
+        with open(target, 'w', encoding='utf-8') as dest:
             dest.write(out)
 
 
 def setup(app):
-    app.add_config_value(str('link_files'), {}, '')
-    app.connect(str('builder-inited'), make_links)
-    return dict(
-        version=importlib_metadata.version('rst.linker'), parallel_read_safe=True
-    )
+    app.add_config_value('link_files', {}, '')
+    app.connect('builder-inited', make_links)
+    return dict(version=metadata.version('rst.linker'), parallel_read_safe=True)
 
 
 def _extend_name(filename):
     base, ext = os.path.splitext(filename)
     return base + ' (links)' + ext
 
 
@@ -208,12 +180,12 @@
     _locate = _locater(app)
     for filename, defn in files_def.items():
         source = _locate(filename)
         replacer = Replacer.from_definition(defn, config_dict(app.config))
         target = _extend_name(source)
         replacer.write_links(source, target)
         remover = functools.partial(_remove, target=target)
-        app.connect(str('build-finished'), remover)
+        app.connect('build-finished', remover)
 
 
 def _remove(app, exception, target):
     os.remove(target)
```

### Comparing `rst_linker-2.5.0/rst.linker.egg-info/PKG-INFO` & `rst_linker-2.6.0/rst.linker.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: rst.linker
-Version: 2.5.0
+Version: 2.6.0
 Summary: Tools for adding metadata and hyperlinks to reStructuredText
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/rst.linker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Sphinx :: Extension
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: python-dateutil
-Requires-Dist: importlib_metadata; python_version < "3.8"
+Requires-Dist: jaraco.vcs>=2.1
+Requires-Dist: jaraco.context
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; platform_python_implementation != "PyPy" and extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: path; extra == "testing"
-Requires-Dist: types-python-dateutil; extra == "testing"
+Requires-Dist: pytest-subprocess; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
```

### Comparing `rst_linker-2.5.0/test_all.py` & `rst_linker-2.6.0/test_all.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import textwrap
-import subprocess
 import locale
+import textwrap
 
-from path import Path
 import pytest
+from path import Path
 
 import rst.linker
 
 
 @pytest.fixture(scope='session', autouse=True)
 def stable_locale():
     """
@@ -71,25 +70,19 @@
                 with_scm="{text}\nTagged {rev[timestamp]}\n",
             )
         ]
     )
 
 
 @pytest.fixture()
-def fake_git(monkeypatch):
-    def _fake_sub(cmd, *args, **kwargs):
-        if cmd[0] != 'git':
-            raise subprocess.CalledProcessError()
-        version = cmd[-1]
-        return {
-            "1.0": '2015-02-24 22:41:28 -0600',
-            "1.3": '2016-02-12 11:05:47 -0500',
-        }[version].encode()
-
-    monkeypatch.setattr(subprocess, 'check_output', _fake_sub)
+def fake_git(fp):
+    fp.register(['git', 'status'])
+    fp.register(['git', 'version'], stdout='git version 2.44.0')
+    fp.register(['git', 'log', fp.any(), '1.0'], stdout='2015-02-24 22:41:28 -0600')
+    fp.register(['git', 'log', fp.any(), '1.3'], stdout='2016-02-12 11:05:47 -0500')
 
 
 def test_scm_example(scm_defn, fake_git):
     repl = rst.linker.Replacer.from_definition(scm_defn)
     input = textwrap.dedent(
         """
         1.0
```

### Comparing `rst_linker-2.5.0/tox.ini` & `rst_linker-2.6.0/tox.ini`

 * *Files identical despite different names*

