# Comparing `tmp/inflect-7.2.0.tar.gz` & `tmp/inflect-7.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inflect-7.2.0.tar", last modified: Sun Mar 31 08:06:56 2024, max compression
+gzip compressed data, was "inflect-7.2.1.tar", last modified: Tue Apr 23 19:54:02 2024, max compression
```

## Comparing `inflect-7.2.0.tar` & `inflect-7.2.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:56.720350 inflect-7.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-31 08:06:32.000000 inflect-7.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-31 08:06:32.000000 inflect-7.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:56.716350 inflect-7.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 08:06:32.000000 inflect-7.2.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-31 08:06:32.000000 inflect-7.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:56.716350 inflect-7.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-03-31 08:06:32.000000 inflect-7.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-31 08:06:32.000000 inflect-7.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-31 08:06:32.000000 inflect-7.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-31 08:06:32.000000 inflect-7.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-31 08:06:32.000000 inflect-7.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-03-31 08:06:32.000000 inflect-7.2.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21004 2024-03-31 08:06:56.720350 inflect-7.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-03-31 08:06:32.000000 inflect-7.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-31 08:06:32.000000 inflect-7.2.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:56.716350 inflect-7.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-31 08:06:32.000000 inflect-7.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-31 08:06:32.000000 inflect-7.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-31 08:06:32.000000 inflect-7.2.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:56.716350 inflect-7.2.0/inflect/
--rw-r--r--   0 runner    (1001) docker     (127)   104293 2024-03-31 08:06:32.000000 inflect-7.2.0/inflect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:32.000000 inflect-7.2.0/inflect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:56.720350 inflect-7.2.0/inflect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21004 2024-03-31 08:06:56.000000 inflect-7.2.0/inflect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-03-31 08:06:56.000000 inflect-7.2.0/inflect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 08:06:56.000000 inflect-7.2.0/inflect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-31 08:06:56.000000 inflect-7.2.0/inflect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-31 08:06:56.000000 inflect-7.2.0/inflect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-31 08:06:32.000000 inflect-7.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-31 08:06:32.000000 inflect-7.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-31 08:06:32.000000 inflect-7.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-31 08:06:32.000000 inflect-7.2.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-03-31 08:06:56.724350 inflect-7.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-31 08:06:32.000000 inflect-7.2.0/tea.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 08:06:56.720350 inflect-7.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    36101 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/inflections.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_an.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_classical_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_classical_ancient.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_classical_herd.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_classical_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_classical_person.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_classical_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_compounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_inflections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_numwords.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_pl_si.py
--rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_pwd.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-31 08:06:32.000000 inflect-7.2.0/tests/test_unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-31 08:06:32.000000 inflect-7.2.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-03-31 08:06:32.000000 inflect-7.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:54:02.860898 inflect-7.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 19:53:40.000000 inflect-7.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-23 19:53:40.000000 inflect-7.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:54:02.852898 inflect-7.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 19:53:40.000000 inflect-7.2.1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 19:53:40.000000 inflect-7.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:54:02.852898 inflect-7.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-23 19:53:40.000000 inflect-7.2.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 19:53:40.000000 inflect-7.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 19:53:40.000000 inflect-7.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-23 19:53:40.000000 inflect-7.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-23 19:53:40.000000 inflect-7.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-23 19:53:40.000000 inflect-7.2.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21049 2024-04-23 19:54:02.860898 inflect-7.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19404 2024-04-23 19:53:40.000000 inflect-7.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 19:53:40.000000 inflect-7.2.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:54:02.852898 inflect-7.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-23 19:53:40.000000 inflect-7.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 19:53:40.000000 inflect-7.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-23 19:53:40.000000 inflect-7.2.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:54:02.856898 inflect-7.2.1/inflect/
+-rw-r--r--   0 runner    (1001) docker     (127)   103796 2024-04-23 19:53:40.000000 inflect-7.2.1/inflect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:53:40.000000 inflect-7.2.1/inflect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:54:02.856898 inflect-7.2.1/inflect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21049 2024-04-23 19:54:02.000000 inflect-7.2.1/inflect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-23 19:54:02.000000 inflect-7.2.1/inflect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:54:02.000000 inflect-7.2.1/inflect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-23 19:54:02.000000 inflect-7.2.1/inflect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 19:54:02.000000 inflect-7.2.1/inflect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 19:53:40.000000 inflect-7.2.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-23 19:53:40.000000 inflect-7.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-23 19:53:40.000000 inflect-7.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-23 19:53:40.000000 inflect-7.2.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:54:02.860898 inflect-7.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 19:53:40.000000 inflect-7.2.1/tea.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:54:02.856898 inflect-7.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    36101 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/inflections.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_an.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_classical_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_classical_ancient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_classical_herd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_classical_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_classical_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_classical_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_compounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_inflections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_numwords.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_pl_si.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42611 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_pwd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-23 19:53:40.000000 inflect-7.2.1/tests/test_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 19:53:40.000000 inflect-7.2.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-23 19:53:40.000000 inflect-7.2.1/tox.ini
```

### Comparing `inflect-7.2.0/.github/workflows/main.yml` & `inflect-7.2.1/.github/workflows/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
```

### Comparing `inflect-7.2.0/LICENSE` & `inflect-7.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/NEWS.rst` & `inflect-7.2.1/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v7.2.1
+======
+
+Bugfixes
+--------
+
+- Refactored number_to_words toward reduced complexity.
+
+
 v7.2.0
 ======
 
 Features
 --------
 
 - Replace pydantic with typeguard (#195)
```

### Comparing `inflect-7.2.0/PKG-INFO` & `inflect-7.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 7.2.0
-Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
-Home-page: https://github.com/jaraco/inflect
-Author: Paul Dyson
-Author-email: pwdyson@yahoo.com
-Maintainer: Jason R. Coombs
-Maintainer-email: jaraco@jaraco.com
+Version: 7.2.1
+Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles
+Author-email: Paul Dyson <pwdyson@yahoo.com>
+Maintainer-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/inflect
+Keywords: plural,inflect,participle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: more_itertools
 Requires-Dist: typeguard>=4.0.1
 Requires-Dist: typing_extensions
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
```

### Comparing `inflect-7.2.0/README.rst` & `inflect-7.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/docs/conf.py` & `inflect-7.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/inflect/__init__.py` & `inflect-7.2.1/inflect/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
  NumOutOfRangeError
  BadUserDefinedPatternError
  BadRcFileError
  BadGenderError
 
 """
 
+from __future__ import annotations
+
 import ast
 import collections
 import contextlib
 import functools
 import itertools
 import re
 from numbers import Number
@@ -3651,24 +3653,15 @@
                     n = int(num)  # type: ignore
             try:
                 post = nth[n % 100]
             except KeyError:
                 post = nth[n % 10]
             return f"{num}{post}"
         else:
-            # Mad props to Damian Conway (?) whose ordinal()
-            # algorithm is type-bendy enough to foil MyPy
-            str_num: str = num  # type: ignore[assignment]
-            mo = ordinal_suff.search(str_num)
-            if mo:
-                post = ordinal[mo.group(1)]
-                rval = ordinal_suff.sub(post, str_num)
-            else:
-                rval = f"{str_num}th"
-            return rval
+            return self._sub_ord(num)
 
     def millfn(self, ind: int = 0) -> str:
         if ind > len(mill) - 1:
             raise NumOutOfRangeError
         return mill[ind]
 
     def unitfn(self, units: int, mindex: int = 0) -> str:
@@ -3779,14 +3772,43 @@
             while mo:
                 num = THREE_DIGITS_WORD.sub(self.hundsub, num, 1)
                 mo = THREE_DIGITS_WORD.search(num)
             num = TWO_DIGITS_WORD.sub(self.tensub, num, 1)
             num = ONE_DIGIT_WORD.sub(self.unitsub, num, 1)
         return num
 
+    @staticmethod
+    def _sub_ord(val):
+        new = ordinal_suff.sub(lambda match: ordinal[match.group(1)], val)
+        return new + "th" * (new == val)
+
+    @classmethod
+    def _chunk_num(cls, num, decimal, group):
+        if decimal:
+            max_split = -1 if group != 0 else 1
+            chunks = num.split(".", max_split)
+        else:
+            chunks = [num]
+        return cls._remove_last_blank(chunks)
+
+    @staticmethod
+    def _remove_last_blank(chunks):
+        """
+        Remove the last item from chunks if it's a blank string.
+
+        Return the resultant chunks and whether the last item was removed.
+        """
+        removed = chunks[-1] == ""
+        result = chunks[:-1] if removed else chunks
+        return result, removed
+
+    @staticmethod
+    def _get_sign(num):
+        return {'+': 'plus', '-': 'minus'}.get(num.lstrip()[0], '')
+
     @typechecked
     def number_to_words(  # noqa: C901
         self,
         num: Union[Number, Word],
         wantlist: bool = False,
         group: int = 0,
         comma: Union[Falsish, str] = ",",
@@ -3826,118 +3848,93 @@
             try:
                 return f"{spnum[0]}.{spnum[1]}"
             except IndexError:
                 return str(spnum[0])
 
         if group < 0 or group > 3:
             raise BadChunkingOptionError
-        nowhite = num.lstrip()
-        if nowhite[0] == "+":
-            sign = "plus"
-        elif nowhite[0] == "-":
-            sign = "minus"
-        else:
-            sign = ""
+
+        sign = self._get_sign(num)
 
         if num in nth_suff:
             num = zero
 
         myord = num[-2:] in nth_suff
         if myord:
             num = num[:-2]
-        finalpoint = False
-        if decimal:
-            if group != 0:
-                chunks = num.split(".")
-            else:
-                chunks = num.split(".", 1)
-            if chunks[-1] == "":  # remove blank string if nothing after decimal
-                chunks = chunks[:-1]
-                finalpoint = True  # add 'point' to end of output
-        else:
-            chunks = [num]
 
-        first: Union[int, str, bool] = 1
-        loopstart = 0
+        chunks, finalpoint = self._chunk_num(num, decimal, group)
 
-        if chunks[0] == "":
-            first = 0
-            if len(chunks) > 1:
-                loopstart = 1
+        loopstart = chunks[0] == ""
+        first: bool | None = not loopstart
+
+        def _handle_chunk(chunk):
+            nonlocal first
 
-        for i in range(loopstart, len(chunks)):
-            chunk = chunks[i]
             # remove all non numeric \D
             chunk = NON_DIGIT.sub("", chunk)
             if chunk == "":
                 chunk = "0"
 
-            if group == 0 and (first == 0 or first == ""):
+            if group == 0 and not first:
                 chunk = self.enword(chunk, 1)
             else:
                 chunk = self.enword(chunk, group)
 
             if chunk[-2:] == ", ":
                 chunk = chunk[:-2]
             chunk = WHITESPACES_COMMA.sub(",", chunk)
 
             if group == 0 and first:
                 chunk = COMMA_WORD.sub(f" {andword} \\1", chunk)
             chunk = WHITESPACES.sub(" ", chunk)
             # chunk = re.sub(r"(\A\s|\s\Z)", self.blankfn, chunk)
             chunk = chunk.strip()
             if first:
-                first = ""
-            chunks[i] = chunk
+                first = None
+            return chunk
+
+        chunks[loopstart:] = map(_handle_chunk, chunks[loopstart:])
 
         numchunks = []
         if first != 0:
             numchunks = chunks[0].split(f"{comma} ")
 
         if myord and numchunks:
-            # TODO: can this be just one re as it is in perl?
-            mo = ordinal_suff.search(numchunks[-1])
-            if mo:
-                numchunks[-1] = ordinal_suff.sub(ordinal[mo.group(1)], numchunks[-1])
-            else:
-                numchunks[-1] += "th"
+            numchunks[-1] = self._sub_ord(numchunks[-1])
 
         for chunk in chunks[1:]:
             numchunks.append(decimal)
             numchunks.extend(chunk.split(f"{comma} "))
 
         if finalpoint:
             numchunks.append(decimal)
 
-        # wantlist: Perl list context. can explicitly specify in Python
         if wantlist:
-            if sign:
-                numchunks = [sign] + numchunks
-            return numchunks
-        elif group:
-            signout = f"{sign} " if sign else ""
-            return f"{signout}{', '.join(numchunks)}"
-        else:
-            signout = f"{sign} " if sign else ""
-            num = f"{signout}{numchunks.pop(0)}"
-            if decimal is None:
-                first = True
-            else:
-                first = not num.endswith(decimal)
-            for nc in numchunks:
-                if nc == decimal:
-                    num += f" {nc}"
-                    first = 0
-                elif first:
-                    num += f"{comma} {nc}"
-                else:
-                    num += f" {nc}"
-            return num
+            return [sign] * bool(sign) + numchunks
+
+        signout = f"{sign} " if sign else ""
+        valout = (
+            ', '.join(numchunks)
+            if group
+            else ''.join(self._render(numchunks, decimal, comma))
+        )
+        return signout + valout
 
-    # Join words with commas and a trailing 'and' (when appropriate)...
+    @staticmethod
+    def _render(chunks, decimal, comma):
+        first_item = chunks.pop(0)
+        yield first_item
+        first = decimal is None or not first_item.endswith(decimal)
+        for nc in chunks:
+            if nc == decimal:
+                first = False
+            elif first:
+                yield comma
+            yield f" {nc}"
 
     @typechecked
     def join(
         self,
         words: Optional[Sequence[Word]],
         sep: Optional[str] = None,
         sep_spaced: bool = True,
```

### Comparing `inflect-7.2.0/inflect.egg-info/PKG-INFO` & `inflect-7.2.1/inflect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: inflect
-Version: 7.2.0
-Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles; convert numbers to words
-Home-page: https://github.com/jaraco/inflect
-Author: Paul Dyson
-Author-email: pwdyson@yahoo.com
-Maintainer: Jason R. Coombs
-Maintainer-email: jaraco@jaraco.com
+Version: 7.2.1
+Summary: Correctly generate plurals, singular nouns, ordinals, indefinite articles
+Author-email: Paul Dyson <pwdyson@yahoo.com>
+Maintainer-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/inflect
+Keywords: plural,inflect,participle
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: more_itertools
 Requires-Dist: typeguard>=4.0.1
 Requires-Dist: typing_extensions
 Provides-Extra: testing
 Requires-Dist: pytest>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
```

### Comparing `inflect-7.2.0/inflect.egg-info/SOURCES.txt` & `inflect-7.2.1/inflect.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 NEWS.rst
 README.rst
 SECURITY.md
 mypy.ini
 pyproject.toml
 pytest.ini
 ruff.toml
-setup.cfg
 tea.yaml
 towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/conf.py
```

### Comparing `inflect-7.2.0/tests/inflections.txt` & `inflect-7.2.1/tests/inflections.txt`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_an.py` & `inflect-7.2.1/tests/test_an.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_classical_all.py` & `inflect-7.2.1/tests/test_classical_all.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_classical_ancient.py` & `inflect-7.2.1/tests/test_classical_ancient.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_classical_herd.py` & `inflect-7.2.1/tests/test_classical_herd.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_classical_names.py` & `inflect-7.2.1/tests/test_classical_names.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_classical_person.py` & `inflect-7.2.1/tests/test_classical_person.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_classical_zero.py` & `inflect-7.2.1/tests/test_classical_zero.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_compounds.py` & `inflect-7.2.1/tests/test_compounds.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_inflections.py` & `inflect-7.2.1/tests/test_inflections.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_join.py` & `inflect-7.2.1/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_numwords.py` & `inflect-7.2.1/tests/test_numwords.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tests/test_pwd.py` & `inflect-7.2.1/tests/test_pwd.py`

 * *Files identical despite different names*

### Comparing `inflect-7.2.0/tox.ini` & `inflect-7.2.1/tox.ini`

 * *Files identical despite different names*

