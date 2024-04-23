# Comparing `tmp/html_text-0.5.2.tar.gz` & `tmp/html_text-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/html_text-0.5.2.tar", last modified: Wed Jul 22 19:12:24 2020, max compression
+gzip compressed data, was "html_text-0.6.0.tar", last modified: Thu Apr  4 11:29:11 2024, max compression
```

## Comparing `html_text-0.5.2.tar` & `html_text-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.716843 html_text-0.5.2/
--rw-r--r--   0 kmike      (501) staff       (20)     2084 2020-07-22 19:11:16.000000 html_text-0.5.2/CHANGES.rst
--rw-r--r--   0 kmike      (501) staff       (20)     1079 2018-11-01 22:27:25.000000 html_text-0.5.2/LICENSE
--rw-r--r--   0 kmike      (501) staff       (20)      243 2018-11-01 22:27:25.000000 html_text-0.5.2/MANIFEST.in
--rw-r--r--   0 kmike      (501) staff       (20)     9400 2020-07-22 19:12:24.717083 html_text-0.5.2/PKG-INFO
--rw-r--r--   0 kmike      (501) staff       (20)     4796 2018-11-19 17:56:02.000000 html_text-0.5.2/README.rst
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.699226 html_text-0.5.2/html_text/
--rw-r--r--   0 kmike      (501) staff       (20)      240 2020-07-22 19:12:07.000000 html_text-0.5.2/html_text/__init__.py
--rw-r--r--   0 kmike      (501) staff       (20)     7290 2020-07-22 17:55:44.000000 html_text-0.5.2/html_text/html_text.py
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.704512 html_text-0.5.2/html_text.egg-info/
--rw-r--r--   0 kmike      (501) staff       (20)     9400 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/PKG-INFO
--rw-r--r--   0 kmike      (501) staff       (20)      997 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/SOURCES.txt
--rw-r--r--   0 kmike      (501) staff       (20)        1 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/dependency_links.txt
--rw-r--r--   0 kmike      (501) staff       (20)        1 2018-11-12 15:20:23.000000 html_text-0.5.2/html_text.egg-info/not-zip-safe
--rw-r--r--   0 kmike      (501) staff       (20)        5 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/requires.txt
--rw-r--r--   0 kmike      (501) staff       (20)       10 2020-07-22 19:12:24.000000 html_text-0.5.2/html_text.egg-info/top_level.txt
--rw-r--r--   0 kmike      (501) staff       (20)      381 2020-07-22 19:12:24.717984 html_text-0.5.2/setup.cfg
--rwxr-xr-x   0 kmike      (501) staff       (20)     1231 2020-07-22 19:12:07.000000 html_text-0.5.2/setup.py
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.706049 html_text-0.5.2/tests/
--rw-r--r--   0 kmike      (501) staff       (20)       24 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/__init__.py
--rw-r--r--   0 kmike      (501) staff       (20)     7890 2020-07-22 17:55:44.000000 html_text-0.5.2/tests/test_html_text.py
-drwxr-xr-x   0 kmike      (501) staff       (20)        0 2020-07-22 19:12:24.716242 html_text-0.5.2/tests/test_webpages/
--rw-r--r--   0 kmike      (501) staff       (20)     9279 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html
--rw-r--r--   0 kmike      (501) staff       (20)     1539 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt
--rw-r--r--   0 kmike      (501) staff       (20)    10225 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.html
--rw-r--r--   0 kmike      (501) staff       (20)     2852 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt
--rw-r--r--   0 kmike      (501) staff       (20)    67149 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.html
--rw-r--r--   0 kmike      (501) staff       (20)     4635 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.txt
--rw-r--r--   0 kmike      (501) staff       (20)    38239 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html
--rw-r--r--   0 kmike      (501) staff       (20)    10856 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt
--rw-r--r--   0 kmike      (501) staff       (20)    11694 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html
--rw-r--r--   0 kmike      (501) staff       (20)     1228 2018-11-01 22:27:25.000000 html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:29:11.046632 html_text-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-04 11:29:02.000000 html_text-0.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 11:29:02.000000 html_text-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-04 11:29:02.000000 html_text-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-04 11:29:11.046632 html_text-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-04 11:29:02.000000 html_text-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:29:11.042632 html_text-0.6.0/html_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 11:29:02.000000 html_text-0.6.0/html_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-04 11:29:02.000000 html_text-0.6.0/html_text/html_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:29:11.046632 html_text-0.6.0/html_text.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-04-04 11:29:11.000000 html_text-0.6.0/html_text.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-04 11:29:11.000000 html_text-0.6.0/html_text.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:29:11.000000 html_text-0.6.0/html_text.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:29:10.000000 html_text-0.6.0/html_text.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-04 11:29:11.000000 html_text-0.6.0/html_text.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-04 11:29:11.000000 html_text-0.6.0/html_text.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-04 11:29:11.046632 html_text-0.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1195 2024-04-04 11:29:02.000000 html_text-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:29:11.046632 html_text-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_html_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:29:11.046632 html_text-0.6.0/tests/test_webpages/
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/IANA — IANA-managed Reserved Domains.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    67149 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/Scrapinghub Enterprise Solutions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/Scrapinghub Enterprise Solutions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38239 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-04 11:29:02.000000 html_text-0.6.0/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt
```

### Comparing `html_text-0.5.2/CHANGES.rst` & `html_text-0.6.0/CHANGES.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 =======
 History
 =======
 
+0.6.0 (2024-04-04)
+------------------
+
+* Moved the Git repository to https://github.com/zytedata/html-text.
+* Added official support for Python 3.9-3.12.
+* Removed support for Python 2.7 and 3.5-3.7.
+* Switched the ``lxml`` dependency to ``lxml[html_clean]`` to support
+  ``lxml >= 5.2.0``.
+* Switch from Travis CI to GitHub Actions.
+* CI improvements.
+
 0.5.2 (2020-07-22)
 ------------------
 
 * Handle lxml Cleaner exceptions (a workaround for
   https://bugs.launchpad.net/lxml/+bug/1838497 );
 * Python 3.8 support;
 * testing improvements.
```

### Comparing `html_text-0.5.2/LICENSE` & `html_text-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/PKG-INFO` & `html_text-0.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,238 +1,253 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: html_text
-Version: 0.5.2
+Version: 0.6.0
 Summary: Extract text from HTML
-Home-page: https://github.com/TeamHG-Memex/html-text
+Home-page: https://github.com/zytedata/html-text
 Author: Konstantin Lopukhin
 Author-email: kostia.lopuhin@gmail.com
 License: MIT license
-Description: ============
-        HTML to Text
-        ============
-        
-        
-        .. image:: https://img.shields.io/pypi/v/html-text.svg
-           :target: https://pypi.python.org/pypi/html-text
-           :alt: PyPI Version
-        
-        .. image:: https://img.shields.io/travis/TeamHG-Memex/html-text.svg
-           :target: https://travis-ci.org/TeamHG-Memex/html-text
-           :alt: Build Status
-        
-        .. image:: http://codecov.io/github/TeamHG-Memex/soft404/coverage.svg?branch=master
-           :target: http://codecov.io/github/TeamHG-Memex/html-text?branch=master
-           :alt: Code Coverage
-        
-        Extract text from HTML
-        
-        * Free software: MIT license
-        
-        How is html_text different from ``.xpath('//text()')`` from LXML
-        or ``.get_text()`` from Beautiful Soup?
-        
-        * Text extracted with ``html_text`` does not contain inline styles,
-          javascript, comments and other text that is not normally visible to users;
-        * ``html_text`` normalizes whitespace, but in a way smarter than
-          ``.xpath('normalize-space())``, adding spaces around inline elements
-          (which are often used as block elements in html markup), and trying to
-          avoid adding extra spaces for punctuation;
-        * ``html-text`` can add newlines (e.g. after headers or paragraphs), so
-          that the output text looks more like how it is rendered in browsers.
-        
-        Install
-        -------
-        
-        Install with pip::
-        
-            pip install html-text
-        
-        The package depends on lxml, so you might need to install additional
-        packages: http://lxml.de/installation.html
-        
-        
-        Usage
-        -----
-        
-        Extract text from HTML::
-        
-            >>> import html_text
-            >>> html_text.extract_text('<h1>Hello</h1> world!')
-            'Hello\n\nworld!'
-        
-            >>> html_text.extract_text('<h1>Hello</h1> world!', guess_layout=False)
-            'Hello world!'
-        
-        Passed html is first cleaned from invisible non-text content such
-        as styles, and then text is extracted.
-        
-        You can also pass an already parsed ``lxml.html.HtmlElement``:
-        
-            >>> import html_text
-            >>> tree = html_text.parse_html('<h1>Hello</h1> world!')
-            >>> html_text.extract_text(tree)
-            'Hello\n\nworld!'
-        
-        If you want, you can handle cleaning manually; use lower-level
-        ``html_text.etree_to_text`` in this case:
-        
-            >>> import html_text
-            >>> tree = html_text.parse_html('<h1>Hello<style>.foo{}</style>!</h1>')
-            >>> cleaned_tree = html_text.cleaner.clean_html(tree)
-            >>> html_text.etree_to_text(cleaned_tree)
-            'Hello!'
-        
-        parsel.Selector objects are also supported; you can define
-        a parsel.Selector to extract text only from specific elements:
-        
-            >>> import html_text
-            >>> sel = html_text.cleaned_selector('<h1>Hello</h1> world!')
-            >>> subsel = sel.xpath('//h1')
-            >>> html_text.selector_to_text(subsel)
-            'Hello'
-        
-        NB parsel.Selector objects are not cleaned automatically, you need to call
-        ``html_text.cleaned_selector`` first.
-        
-        Main functions and objects:
-        
-        * ``html_text.extract_text`` accepts html and returns extracted text.
-        * ``html_text.etree_to_text`` accepts parsed lxml Element and returns
-          extracted text; it is a lower-level function, cleaning is not handled
-          here.
-        * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance which
-          can be used with ``html_text.etree_to_text``; its options are tuned for
-          speed and text extraction quality.
-        * ``html_text.cleaned_selector`` accepts html as text or as
-          ``lxml.html.HtmlElement``, and returns cleaned ``parsel.Selector``.
-        * ``html_text.selector_to_text`` accepts ``parsel.Selector`` and returns
-          extracted text.
-        
-        If ``guess_layout`` is True (default), a newline is added before and after
-        ``newline_tags``, and two newlines are added before and after
-        ``double_newline_tags``. This heuristic makes the extracted text
-        more similar to how it is rendered in the browser. Default newline and double
-        newline tags can be found in `html_text.NEWLINE_TAGS`
-        and `html_text.DOUBLE_NEWLINE_TAGS`.
-        
-        It is possible to customize how newlines are added, using ``newline_tags`` and
-        ``double_newline_tags`` arguments (which are `html_text.NEWLINE_TAGS` and
-        `html_text.DOUBLE_NEWLINE_TAGS` by default). For example, don't add a newline
-        after ``<div>`` tags:
-        
-            >>> newline_tags = html_text.NEWLINE_TAGS - {'div'}
-            >>> html_text.extract_text('<div>Hello</div> world!',
-            ...                        newline_tags=newline_tags)
-            'Hello world!'
-        
-        Apart from just getting text from the page (e.g. for display or search),
-        one intended usage of this library is for machine learning (feature extraction).
-        If you want to use the text of the html page as a feature (e.g. for classification),
-        this library gives you plain text that you can later feed into a standard text
-        classification pipeline.
-        If you feel that you need html structure as well, check out
-        `webstruct <http://webstruct.readthedocs.io/en/latest/>`_ library.
-        
-        ----
-        
-        .. image:: https://hyperiongray.s3.amazonaws.com/define-hg.svg
-        	:target: https://www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text
-        	:alt: define hyperiongray
-        
-        
-        =======
-        History
-        =======
-        
-        0.5.2 (2020-07-22)
-        ------------------
-        
-        * Handle lxml Cleaner exceptions (a workaround for
-          https://bugs.launchpad.net/lxml/+bug/1838497 );
-        * Python 3.8 support;
-        * testing improvements.
-        
-        0.5.1 (2019-05-27)
-        ------------------
-        
-        Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
-        producing unnecessary spaces after newlines.
-        
-        0.5.0 (2018-11-19)
-        ------------------
-        
-        Parsel dependency is removed in this release,
-        though parsel is still supported.
-        
-        * ``parsel`` package is no longer required to install and use html-text;
-        * ``html_text.etree_to_text`` function allows to extract text from
-          lxml Elements;
-        * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance with
-          options tuned for text extraction speed and quality;
-        * test and documentation improvements;
-        * Python 3.7 support.
-        
-        0.4.1 (2018-09-25)
-        ------------------
-        
-        Fixed a regression in 0.4.0 release: text was empty when
-        ``html_text.extract_text`` is called with a node with text, but
-        without children.
-        
-        0.4.0 (2018-09-25)
-        ------------------
-        
-        This is a backwards-incompatible release: by default html_text functions
-        now add newlines after elements, if appropriate, to make the extracted text
-        to look more like how it is rendered in a browser.
-        
-        To turn it off, pass ``guess_layout=False`` option to html_text functions.
-        
-        * ``guess_layout`` option to to make extracted text look more like how
-          it is rendered in browser.
-        * Add tests of layout extraction for real webpages.
-        
-        
-        0.3.0 (2017-10-12)
-        ------------------
-        
-        * Expose functions that operate on selectors,
-          use ``.//text()`` to extract text from selector.
-        
-        
-        0.2.1 (2017-05-29)
-        ------------------
-        
-        * Packaging fix (include CHANGES.rst)
-        
-        
-        0.2.0 (2017-05-29)
-        ------------------
-        
-        * Fix unwanted joins of words with inline tags: spaces are added for inline
-          tags too, but a heuristic is used to preserve punctuation without extra spaces.
-        * Accept parsed html trees.
-        
-        
-        0.1.1 (2017-01-16)
-        ------------------
-        
-        * Travis-CI and codecov.io integrations added
-        
-        
-        0.1.0 (2016-09-27)
-        ------------------
-        
-        * First release on PyPI.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+License-File: LICENSE
+Requires-Dist: lxml[html_clean]
+
+============
+HTML to Text
+============
+
+
+.. image:: https://img.shields.io/pypi/v/html-text.svg
+   :target: https://pypi.python.org/pypi/html-text
+   :alt: PyPI Version
+
+.. image:: https://img.shields.io/pypi/pyversions/html-text.svg
+   :target: https://pypi.python.org/pypi/html-text
+   :alt: Supported Python Versions
+
+.. image:: https://github.com/zytedata/html-text/workflows/tox/badge.svg
+   :target: https://github.com/zytedata/html-text/actions
+   :alt: Build Status
+
+.. image:: https://codecov.io/github/zytedata/html-text/coverage.svg?branch=master
+   :target: https://codecov.io/gh/zytedata/html-text
+   :alt: Coverage report
+
+Extract text from HTML
+
+* Free software: MIT license
+
+How is html_text different from ``.xpath('//text()')`` from LXML
+or ``.get_text()`` from Beautiful Soup?
+
+* Text extracted with ``html_text`` does not contain inline styles,
+  javascript, comments and other text that is not normally visible to users;
+* ``html_text`` normalizes whitespace, but in a way smarter than
+  ``.xpath('normalize-space())``, adding spaces around inline elements
+  (which are often used as block elements in html markup), and trying to
+  avoid adding extra spaces for punctuation;
+* ``html-text`` can add newlines (e.g. after headers or paragraphs), so
+  that the output text looks more like how it is rendered in browsers.
+
+Install
+-------
+
+Install with pip::
+
+    pip install html-text
+
+The package depends on lxml, so you might need to install additional
+packages: http://lxml.de/installation.html
+
+
+Usage
+-----
+
+Extract text from HTML::
+
+    >>> import html_text
+    >>> html_text.extract_text('<h1>Hello</h1> world!')
+    'Hello\n\nworld!'
+
+    >>> html_text.extract_text('<h1>Hello</h1> world!', guess_layout=False)
+    'Hello world!'
+
+Passed html is first cleaned from invisible non-text content such
+as styles, and then text is extracted.
+
+You can also pass an already parsed ``lxml.html.HtmlElement``:
+
+    >>> import html_text
+    >>> tree = html_text.parse_html('<h1>Hello</h1> world!')
+    >>> html_text.extract_text(tree)
+    'Hello\n\nworld!'
+
+If you want, you can handle cleaning manually; use lower-level
+``html_text.etree_to_text`` in this case:
+
+    >>> import html_text
+    >>> tree = html_text.parse_html('<h1>Hello<style>.foo{}</style>!</h1>')
+    >>> cleaned_tree = html_text.cleaner.clean_html(tree)
+    >>> html_text.etree_to_text(cleaned_tree)
+    'Hello!'
+
+parsel.Selector objects are also supported; you can define
+a parsel.Selector to extract text only from specific elements:
+
+    >>> import html_text
+    >>> sel = html_text.cleaned_selector('<h1>Hello</h1> world!')
+    >>> subsel = sel.xpath('//h1')
+    >>> html_text.selector_to_text(subsel)
+    'Hello'
+
+NB parsel.Selector objects are not cleaned automatically, you need to call
+``html_text.cleaned_selector`` first.
+
+Main functions and objects:
+
+* ``html_text.extract_text`` accepts html and returns extracted text.
+* ``html_text.etree_to_text`` accepts parsed lxml Element and returns
+  extracted text; it is a lower-level function, cleaning is not handled
+  here.
+* ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance which
+  can be used with ``html_text.etree_to_text``; its options are tuned for
+  speed and text extraction quality.
+* ``html_text.cleaned_selector`` accepts html as text or as
+  ``lxml.html.HtmlElement``, and returns cleaned ``parsel.Selector``.
+* ``html_text.selector_to_text`` accepts ``parsel.Selector`` and returns
+  extracted text.
+
+If ``guess_layout`` is True (default), a newline is added before and after
+``newline_tags``, and two newlines are added before and after
+``double_newline_tags``. This heuristic makes the extracted text
+more similar to how it is rendered in the browser. Default newline and double
+newline tags can be found in `html_text.NEWLINE_TAGS`
+and `html_text.DOUBLE_NEWLINE_TAGS`.
+
+It is possible to customize how newlines are added, using ``newline_tags`` and
+``double_newline_tags`` arguments (which are `html_text.NEWLINE_TAGS` and
+`html_text.DOUBLE_NEWLINE_TAGS` by default). For example, don't add a newline
+after ``<div>`` tags:
+
+    >>> newline_tags = html_text.NEWLINE_TAGS - {'div'}
+    >>> html_text.extract_text('<div>Hello</div> world!',
+    ...                        newline_tags=newline_tags)
+    'Hello world!'
+
+Apart from just getting text from the page (e.g. for display or search),
+one intended usage of this library is for machine learning (feature extraction).
+If you want to use the text of the html page as a feature (e.g. for classification),
+this library gives you plain text that you can later feed into a standard text
+classification pipeline.
+If you feel that you need html structure as well, check out
+`webstruct <http://webstruct.readthedocs.io/en/latest/>`_ library.
+
+----
+
+.. image:: https://hyperiongray.s3.amazonaws.com/define-hg.svg
+	:target: https://www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text
+	:alt: define hyperiongray
+
+
+=======
+History
+=======
+
+0.6.0 (2024-04-04)
+------------------
+
+* Moved the Git repository to https://github.com/zytedata/html-text.
+* Added official support for Python 3.9-3.12.
+* Removed support for Python 2.7 and 3.5-3.7.
+* Switched the ``lxml`` dependency to ``lxml[html_clean]`` to support
+  ``lxml >= 5.2.0``.
+* Switch from Travis CI to GitHub Actions.
+* CI improvements.
+
+0.5.2 (2020-07-22)
+------------------
+
+* Handle lxml Cleaner exceptions (a workaround for
+  https://bugs.launchpad.net/lxml/+bug/1838497 );
+* Python 3.8 support;
+* testing improvements.
+
+0.5.1 (2019-05-27)
+------------------
+
+Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
+producing unnecessary spaces after newlines.
+
+0.5.0 (2018-11-19)
+------------------
+
+Parsel dependency is removed in this release,
+though parsel is still supported.
+
+* ``parsel`` package is no longer required to install and use html-text;
+* ``html_text.etree_to_text`` function allows to extract text from
+  lxml Elements;
+* ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance with
+  options tuned for text extraction speed and quality;
+* test and documentation improvements;
+* Python 3.7 support.
+
+0.4.1 (2018-09-25)
+------------------
+
+Fixed a regression in 0.4.0 release: text was empty when
+``html_text.extract_text`` is called with a node with text, but
+without children.
+
+0.4.0 (2018-09-25)
+------------------
+
+This is a backwards-incompatible release: by default html_text functions
+now add newlines after elements, if appropriate, to make the extracted text
+to look more like how it is rendered in a browser.
+
+To turn it off, pass ``guess_layout=False`` option to html_text functions.
+
+* ``guess_layout`` option to to make extracted text look more like how
+  it is rendered in browser.
+* Add tests of layout extraction for real webpages.
+
+
+0.3.0 (2017-10-12)
+------------------
+
+* Expose functions that operate on selectors,
+  use ``.//text()`` to extract text from selector.
+
+
+0.2.1 (2017-05-29)
+------------------
+
+* Packaging fix (include CHANGES.rst)
+
+
+0.2.0 (2017-05-29)
+------------------
+
+* Fix unwanted joins of words with inline tags: spaces are added for inline
+  tags too, but a heuristic is used to preserve punctuation without extra spaces.
+* Accept parsed html trees.
+
+
+0.1.1 (2017-01-16)
+------------------
+
+* Travis-CI and codecov.io integrations added
+
+
+0.1.0 (2016-09-27)
+------------------
+
+* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,29 +1,38 @@
-Metadata-Version: 1.1 Name: html_text Version: 0.5.2 Summary: Extract text from
-HTML Home-page: https://github.com/TeamHG-Memex/html-text Author: Konstantin
+Metadata-Version: 2.1 Name: html_text Version: 0.6.0 Summary: Extract text from
+HTML Home-page: https://github.com/zytedata/html-text Author: Konstantin
 Lopukhin Author-email: kostia.lopuhin@gmail.com License: MIT license
-Description: ============ HTML to Text ============ .. image:: https://
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 License-File: LICENSE Requires-Dist: lxml
+[html_clean] ============ HTML to Text ============ .. image:: https://
 img.shields.io/pypi/v/html-text.svg :target: https://pypi.python.org/pypi/html-
-text :alt: PyPI Version .. image:: https://img.shields.io/travis/TeamHG-Memex/
-html-text.svg :target: https://travis-ci.org/TeamHG-Memex/html-text :alt: Build
-Status .. image:: http://codecov.io/github/TeamHG-Memex/soft404/
-coverage.svg?branch=master :target: http://codecov.io/github/TeamHG-Memex/html-
-text?branch=master :alt: Code Coverage Extract text from HTML * Free software:
-MIT license How is html_text different from ``.xpath('//text()')`` from LXML or
-``.get_text()`` from Beautiful Soup? * Text extracted with ``html_text`` does
-not contain inline styles, javascript, comments and other text that is not
-normally visible to users; * ``html_text`` normalizes whitespace, but in a way
-smarter than ``.xpath('normalize-space())``, adding spaces around inline
-elements (which are often used as block elements in html markup), and trying to
-avoid adding extra spaces for punctuation; * ``html-text`` can add newlines
-(e.g. after headers or paragraphs), so that the output text looks more like how
-it is rendered in browsers. Install ------- Install with pip:: pip install
-html-text The package depends on lxml, so you might need to install additional
-packages: http://lxml.de/installation.html Usage ----- Extract text from HTML::
->>> import html_text >>> html_text.extract_text('
+text :alt: PyPI Version .. image:: https://img.shields.io/pypi/pyversions/html-
+text.svg :target: https://pypi.python.org/pypi/html-text :alt: Supported Python
+Versions .. image:: https://github.com/zytedata/html-text/workflows/tox/
+badge.svg :target: https://github.com/zytedata/html-text/actions :alt: Build
+Status .. image:: https://codecov.io/github/zytedata/html-text/
+coverage.svg?branch=master :target: https://codecov.io/gh/zytedata/html-text :
+alt: Coverage report Extract text from HTML * Free software: MIT license How is
+html_text different from ``.xpath('//text()')`` from LXML or ``.get_text()``
+from Beautiful Soup? * Text extracted with ``html_text`` does not contain
+inline styles, javascript, comments and other text that is not normally visible
+to users; * ``html_text`` normalizes whitespace, but in a way smarter than
+``.xpath('normalize-space())``, adding spaces around inline elements (which are
+often used as block elements in html markup), and trying to avoid adding extra
+spaces for punctuation; * ``html-text`` can add newlines (e.g. after headers or
+paragraphs), so that the output text looks more like how it is rendered in
+browsers. Install ------- Install with pip:: pip install html-text The package
+depends on lxml, so you might need to install additional packages: http://
+lxml.de/installation.html Usage ----- Extract text from HTML:: >>> import
+html_text >>> html_text.extract_text('
 ************ HHeelllloo ************
 world!') 'Hello\n\nworld!' >>> html_text.extract_text('
 ************ HHeelllloo ************
 world!', guess_layout=False) 'Hello world!' Passed html is first cleaned from
 invisible non-text content such as styles, and then text is extracted. You can
 also pass an already parsed ``lxml.html.HtmlElement``: >>> import html_text >>>
 tree = html_text.parse_html('
@@ -66,41 +75,39 @@
 text of the html page as a feature (e.g. for classification), this library
 gives you plain text that you can later feed into a standard text
 classification pipeline. If you feel that you need html structure as well,
 check out `webstruct
 webstruct.readthedocs.io/en/latest/>`_ library. ---- .. image:: https://
 hyperiongray.s3.amazonaws.com/define-hg.svg :target: https://
 www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text :alt: define
-hyperiongray ======= History ======= 0.5.2 (2020-07-22) ------------------ *
-Handle lxml Cleaner exceptions (a workaround for https://bugs.launchpad.net/
-lxml/+bug/1838497 ); * Python 3.8 support; * testing improvements. 0.5.1 (2019-
-05-27) ------------------ Fixed whitespace handling when ``guess_punct_space``
-is False: html-text was producing unnecessary spaces after newlines. 0.5.0
-(2018-11-19) ------------------ Parsel dependency is removed in this release,
-though parsel is still supported. * ``parsel`` package is no longer required to
-install and use html-text; * ``html_text.etree_to_text`` function allows to
-extract text from lxml Elements; * ``html_text.cleaner`` is an
-``lxml.html.clean.Cleaner`` instance with options tuned for text extraction
-speed and quality; * test and documentation improvements; * Python 3.7 support.
-0.4.1 (2018-09-25) ------------------ Fixed a regression in 0.4.0 release: text
-was empty when ``html_text.extract_text`` is called with a node with text, but
-without children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
+hyperiongray ======= History ======= 0.6.0 (2024-04-04) ------------------ *
+Moved the Git repository to https://github.com/zytedata/html-text. * Added
+official support for Python 3.9-3.12. * Removed support for Python 2.7 and 3.5-
+3.7. * Switched the ``lxml`` dependency to ``lxml[html_clean]`` to support
+``lxml >= 5.2.0``. * Switch from Travis CI to GitHub Actions. * CI
+improvements. 0.5.2 (2020-07-22) ------------------ * Handle lxml Cleaner
+exceptions (a workaround for https://bugs.launchpad.net/lxml/+bug/1838497 ); *
+Python 3.8 support; * testing improvements. 0.5.1 (2019-05-27) ----------------
+-- Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
+producing unnecessary spaces after newlines. 0.5.0 (2018-11-19) ---------------
+--- Parsel dependency is removed in this release, though parsel is still
+supported. * ``parsel`` package is no longer required to install and use html-
+text; * ``html_text.etree_to_text`` function allows to extract text from lxml
+Elements; * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance
+with options tuned for text extraction speed and quality; * test and
+documentation improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ----------
+-------- Fixed a regression in 0.4.0 release: text was empty when
+``html_text.extract_text`` is called with a node with text, but without
+children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
 incompatible release: by default html_text functions now add newlines after
 elements, if appropriate, to make the extracted text to look more like how it
 is rendered in a browser. To turn it off, pass ``guess_layout=False`` option to
 html_text functions. * ``guess_layout`` option to to make extracted text look
 more like how it is rendered in browser. * Add tests of layout extraction for
 real webpages. 0.3.0 (2017-10-12) ------------------ * Expose functions that
 operate on selectors, use ``.//text()`` to extract text from selector. 0.2.1
 (2017-05-29) ------------------ * Packaging fix (include CHANGES.rst) 0.2.0
 (2017-05-29) ------------------ * Fix unwanted joins of words with inline tags:
 spaces are added for inline tags too, but a heuristic is used to preserve
 punctuation without extra spaces. * Accept parsed html trees. 0.1.1 (2017-01-
 16) ------------------ * Travis-CI and codecov.io integrations added 0.1.0
-(2016-09-27) ------------------ * First release on PyPI. Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+(2016-09-27) ------------------ * First release on PyPI.
```

### Comparing `html_text-0.5.2/README.rst` & `html_text-0.6.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 ============
 
 
 .. image:: https://img.shields.io/pypi/v/html-text.svg
    :target: https://pypi.python.org/pypi/html-text
    :alt: PyPI Version
 
-.. image:: https://img.shields.io/travis/TeamHG-Memex/html-text.svg
-   :target: https://travis-ci.org/TeamHG-Memex/html-text
+.. image:: https://img.shields.io/pypi/pyversions/html-text.svg
+   :target: https://pypi.python.org/pypi/html-text
+   :alt: Supported Python Versions
+
+.. image:: https://github.com/zytedata/html-text/workflows/tox/badge.svg
+   :target: https://github.com/zytedata/html-text/actions
    :alt: Build Status
 
-.. image:: http://codecov.io/github/TeamHG-Memex/soft404/coverage.svg?branch=master
-   :target: http://codecov.io/github/TeamHG-Memex/html-text?branch=master
-   :alt: Code Coverage
+.. image:: https://codecov.io/github/zytedata/html-text/coverage.svg?branch=master
+   :target: https://codecov.io/gh/zytedata/html-text
+   :alt: Coverage report
 
 Extract text from HTML
 
 * Free software: MIT license
 
 How is html_text different from ``.xpath('//text()')`` from LXML
 or ``.get_text()`` from Beautiful Soup?
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
 ============ HTML to Text ============ .. image:: https://img.shields.io/pypi/
 v/html-text.svg :target: https://pypi.python.org/pypi/html-text :alt: PyPI
-Version .. image:: https://img.shields.io/travis/TeamHG-Memex/html-text.svg :
-target: https://travis-ci.org/TeamHG-Memex/html-text :alt: Build Status ..
-image:: http://codecov.io/github/TeamHG-Memex/soft404/
-coverage.svg?branch=master :target: http://codecov.io/github/TeamHG-Memex/html-
-text?branch=master :alt: Code Coverage Extract text from HTML * Free software:
-MIT license How is html_text different from ``.xpath('//text()')`` from LXML or
-``.get_text()`` from Beautiful Soup? * Text extracted with ``html_text`` does
-not contain inline styles, javascript, comments and other text that is not
-normally visible to users; * ``html_text`` normalizes whitespace, but in a way
-smarter than ``.xpath('normalize-space())``, adding spaces around inline
-elements (which are often used as block elements in html markup), and trying to
-avoid adding extra spaces for punctuation; * ``html-text`` can add newlines
-(e.g. after headers or paragraphs), so that the output text looks more like how
-it is rendered in browsers. Install ------- Install with pip:: pip install
-html-text The package depends on lxml, so you might need to install additional
-packages: http://lxml.de/installation.html Usage ----- Extract text from HTML::
->>> import html_text >>> html_text.extract_text('
+Version .. image:: https://img.shields.io/pypi/pyversions/html-text.svg :
+target: https://pypi.python.org/pypi/html-text :alt: Supported Python Versions
+.. image:: https://github.com/zytedata/html-text/workflows/tox/badge.svg :
+target: https://github.com/zytedata/html-text/actions :alt: Build Status ..
+image:: https://codecov.io/github/zytedata/html-text/coverage.svg?branch=master
+:target: https://codecov.io/gh/zytedata/html-text :alt: Coverage report Extract
+text from HTML * Free software: MIT license How is html_text different from
+``.xpath('//text()')`` from LXML or ``.get_text()`` from Beautiful Soup? * Text
+extracted with ``html_text`` does not contain inline styles, javascript,
+comments and other text that is not normally visible to users; * ``html_text``
+normalizes whitespace, but in a way smarter than ``.xpath('normalize-space
+())``, adding spaces around inline elements (which are often used as block
+elements in html markup), and trying to avoid adding extra spaces for
+punctuation; * ``html-text`` can add newlines (e.g. after headers or
+paragraphs), so that the output text looks more like how it is rendered in
+browsers. Install ------- Install with pip:: pip install html-text The package
+depends on lxml, so you might need to install additional packages: http://
+lxml.de/installation.html Usage ----- Extract text from HTML:: >>> import
+html_text >>> html_text.extract_text('
 ************ HHeelllloo ************
 world!') 'Hello\n\nworld!' >>> html_text.extract_text('
 ************ HHeelllloo ************
 world!', guess_layout=False) 'Hello world!' Passed html is first cleaned from
 invisible non-text content such as styles, and then text is extracted. You can
 also pass an already parsed ``lxml.html.HtmlElement``: >>> import html_text >>>
 tree = html_text.parse_html('
```

### Comparing `html_text-0.5.2/html_text/html_text.py` & `html_text-0.6.0/html_text/html_text.py`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/html_text.egg-info/PKG-INFO` & `html_text-0.6.0/html_text.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,238 +1,253 @@
-Metadata-Version: 1.1
-Name: html-text
-Version: 0.5.2
+Metadata-Version: 2.1
+Name: html_text
+Version: 0.6.0
 Summary: Extract text from HTML
-Home-page: https://github.com/TeamHG-Memex/html-text
+Home-page: https://github.com/zytedata/html-text
 Author: Konstantin Lopukhin
 Author-email: kostia.lopuhin@gmail.com
 License: MIT license
-Description: ============
-        HTML to Text
-        ============
-        
-        
-        .. image:: https://img.shields.io/pypi/v/html-text.svg
-           :target: https://pypi.python.org/pypi/html-text
-           :alt: PyPI Version
-        
-        .. image:: https://img.shields.io/travis/TeamHG-Memex/html-text.svg
-           :target: https://travis-ci.org/TeamHG-Memex/html-text
-           :alt: Build Status
-        
-        .. image:: http://codecov.io/github/TeamHG-Memex/soft404/coverage.svg?branch=master
-           :target: http://codecov.io/github/TeamHG-Memex/html-text?branch=master
-           :alt: Code Coverage
-        
-        Extract text from HTML
-        
-        * Free software: MIT license
-        
-        How is html_text different from ``.xpath('//text()')`` from LXML
-        or ``.get_text()`` from Beautiful Soup?
-        
-        * Text extracted with ``html_text`` does not contain inline styles,
-          javascript, comments and other text that is not normally visible to users;
-        * ``html_text`` normalizes whitespace, but in a way smarter than
-          ``.xpath('normalize-space())``, adding spaces around inline elements
-          (which are often used as block elements in html markup), and trying to
-          avoid adding extra spaces for punctuation;
-        * ``html-text`` can add newlines (e.g. after headers or paragraphs), so
-          that the output text looks more like how it is rendered in browsers.
-        
-        Install
-        -------
-        
-        Install with pip::
-        
-            pip install html-text
-        
-        The package depends on lxml, so you might need to install additional
-        packages: http://lxml.de/installation.html
-        
-        
-        Usage
-        -----
-        
-        Extract text from HTML::
-        
-            >>> import html_text
-            >>> html_text.extract_text('<h1>Hello</h1> world!')
-            'Hello\n\nworld!'
-        
-            >>> html_text.extract_text('<h1>Hello</h1> world!', guess_layout=False)
-            'Hello world!'
-        
-        Passed html is first cleaned from invisible non-text content such
-        as styles, and then text is extracted.
-        
-        You can also pass an already parsed ``lxml.html.HtmlElement``:
-        
-            >>> import html_text
-            >>> tree = html_text.parse_html('<h1>Hello</h1> world!')
-            >>> html_text.extract_text(tree)
-            'Hello\n\nworld!'
-        
-        If you want, you can handle cleaning manually; use lower-level
-        ``html_text.etree_to_text`` in this case:
-        
-            >>> import html_text
-            >>> tree = html_text.parse_html('<h1>Hello<style>.foo{}</style>!</h1>')
-            >>> cleaned_tree = html_text.cleaner.clean_html(tree)
-            >>> html_text.etree_to_text(cleaned_tree)
-            'Hello!'
-        
-        parsel.Selector objects are also supported; you can define
-        a parsel.Selector to extract text only from specific elements:
-        
-            >>> import html_text
-            >>> sel = html_text.cleaned_selector('<h1>Hello</h1> world!')
-            >>> subsel = sel.xpath('//h1')
-            >>> html_text.selector_to_text(subsel)
-            'Hello'
-        
-        NB parsel.Selector objects are not cleaned automatically, you need to call
-        ``html_text.cleaned_selector`` first.
-        
-        Main functions and objects:
-        
-        * ``html_text.extract_text`` accepts html and returns extracted text.
-        * ``html_text.etree_to_text`` accepts parsed lxml Element and returns
-          extracted text; it is a lower-level function, cleaning is not handled
-          here.
-        * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance which
-          can be used with ``html_text.etree_to_text``; its options are tuned for
-          speed and text extraction quality.
-        * ``html_text.cleaned_selector`` accepts html as text or as
-          ``lxml.html.HtmlElement``, and returns cleaned ``parsel.Selector``.
-        * ``html_text.selector_to_text`` accepts ``parsel.Selector`` and returns
-          extracted text.
-        
-        If ``guess_layout`` is True (default), a newline is added before and after
-        ``newline_tags``, and two newlines are added before and after
-        ``double_newline_tags``. This heuristic makes the extracted text
-        more similar to how it is rendered in the browser. Default newline and double
-        newline tags can be found in `html_text.NEWLINE_TAGS`
-        and `html_text.DOUBLE_NEWLINE_TAGS`.
-        
-        It is possible to customize how newlines are added, using ``newline_tags`` and
-        ``double_newline_tags`` arguments (which are `html_text.NEWLINE_TAGS` and
-        `html_text.DOUBLE_NEWLINE_TAGS` by default). For example, don't add a newline
-        after ``<div>`` tags:
-        
-            >>> newline_tags = html_text.NEWLINE_TAGS - {'div'}
-            >>> html_text.extract_text('<div>Hello</div> world!',
-            ...                        newline_tags=newline_tags)
-            'Hello world!'
-        
-        Apart from just getting text from the page (e.g. for display or search),
-        one intended usage of this library is for machine learning (feature extraction).
-        If you want to use the text of the html page as a feature (e.g. for classification),
-        this library gives you plain text that you can later feed into a standard text
-        classification pipeline.
-        If you feel that you need html structure as well, check out
-        `webstruct <http://webstruct.readthedocs.io/en/latest/>`_ library.
-        
-        ----
-        
-        .. image:: https://hyperiongray.s3.amazonaws.com/define-hg.svg
-        	:target: https://www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text
-        	:alt: define hyperiongray
-        
-        
-        =======
-        History
-        =======
-        
-        0.5.2 (2020-07-22)
-        ------------------
-        
-        * Handle lxml Cleaner exceptions (a workaround for
-          https://bugs.launchpad.net/lxml/+bug/1838497 );
-        * Python 3.8 support;
-        * testing improvements.
-        
-        0.5.1 (2019-05-27)
-        ------------------
-        
-        Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
-        producing unnecessary spaces after newlines.
-        
-        0.5.0 (2018-11-19)
-        ------------------
-        
-        Parsel dependency is removed in this release,
-        though parsel is still supported.
-        
-        * ``parsel`` package is no longer required to install and use html-text;
-        * ``html_text.etree_to_text`` function allows to extract text from
-          lxml Elements;
-        * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance with
-          options tuned for text extraction speed and quality;
-        * test and documentation improvements;
-        * Python 3.7 support.
-        
-        0.4.1 (2018-09-25)
-        ------------------
-        
-        Fixed a regression in 0.4.0 release: text was empty when
-        ``html_text.extract_text`` is called with a node with text, but
-        without children.
-        
-        0.4.0 (2018-09-25)
-        ------------------
-        
-        This is a backwards-incompatible release: by default html_text functions
-        now add newlines after elements, if appropriate, to make the extracted text
-        to look more like how it is rendered in a browser.
-        
-        To turn it off, pass ``guess_layout=False`` option to html_text functions.
-        
-        * ``guess_layout`` option to to make extracted text look more like how
-          it is rendered in browser.
-        * Add tests of layout extraction for real webpages.
-        
-        
-        0.3.0 (2017-10-12)
-        ------------------
-        
-        * Expose functions that operate on selectors,
-          use ``.//text()`` to extract text from selector.
-        
-        
-        0.2.1 (2017-05-29)
-        ------------------
-        
-        * Packaging fix (include CHANGES.rst)
-        
-        
-        0.2.0 (2017-05-29)
-        ------------------
-        
-        * Fix unwanted joins of words with inline tags: spaces are added for inline
-          tags too, but a heuristic is used to preserve punctuation without extra spaces.
-        * Accept parsed html trees.
-        
-        
-        0.1.1 (2017-01-16)
-        ------------------
-        
-        * Travis-CI and codecov.io integrations added
-        
-        
-        0.1.0 (2016-09-27)
-        ------------------
-        
-        * First release on PyPI.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+License-File: LICENSE
+Requires-Dist: lxml[html_clean]
+
+============
+HTML to Text
+============
+
+
+.. image:: https://img.shields.io/pypi/v/html-text.svg
+   :target: https://pypi.python.org/pypi/html-text
+   :alt: PyPI Version
+
+.. image:: https://img.shields.io/pypi/pyversions/html-text.svg
+   :target: https://pypi.python.org/pypi/html-text
+   :alt: Supported Python Versions
+
+.. image:: https://github.com/zytedata/html-text/workflows/tox/badge.svg
+   :target: https://github.com/zytedata/html-text/actions
+   :alt: Build Status
+
+.. image:: https://codecov.io/github/zytedata/html-text/coverage.svg?branch=master
+   :target: https://codecov.io/gh/zytedata/html-text
+   :alt: Coverage report
+
+Extract text from HTML
+
+* Free software: MIT license
+
+How is html_text different from ``.xpath('//text()')`` from LXML
+or ``.get_text()`` from Beautiful Soup?
+
+* Text extracted with ``html_text`` does not contain inline styles,
+  javascript, comments and other text that is not normally visible to users;
+* ``html_text`` normalizes whitespace, but in a way smarter than
+  ``.xpath('normalize-space())``, adding spaces around inline elements
+  (which are often used as block elements in html markup), and trying to
+  avoid adding extra spaces for punctuation;
+* ``html-text`` can add newlines (e.g. after headers or paragraphs), so
+  that the output text looks more like how it is rendered in browsers.
+
+Install
+-------
+
+Install with pip::
+
+    pip install html-text
+
+The package depends on lxml, so you might need to install additional
+packages: http://lxml.de/installation.html
+
+
+Usage
+-----
+
+Extract text from HTML::
+
+    >>> import html_text
+    >>> html_text.extract_text('<h1>Hello</h1> world!')
+    'Hello\n\nworld!'
+
+    >>> html_text.extract_text('<h1>Hello</h1> world!', guess_layout=False)
+    'Hello world!'
+
+Passed html is first cleaned from invisible non-text content such
+as styles, and then text is extracted.
+
+You can also pass an already parsed ``lxml.html.HtmlElement``:
+
+    >>> import html_text
+    >>> tree = html_text.parse_html('<h1>Hello</h1> world!')
+    >>> html_text.extract_text(tree)
+    'Hello\n\nworld!'
+
+If you want, you can handle cleaning manually; use lower-level
+``html_text.etree_to_text`` in this case:
+
+    >>> import html_text
+    >>> tree = html_text.parse_html('<h1>Hello<style>.foo{}</style>!</h1>')
+    >>> cleaned_tree = html_text.cleaner.clean_html(tree)
+    >>> html_text.etree_to_text(cleaned_tree)
+    'Hello!'
+
+parsel.Selector objects are also supported; you can define
+a parsel.Selector to extract text only from specific elements:
+
+    >>> import html_text
+    >>> sel = html_text.cleaned_selector('<h1>Hello</h1> world!')
+    >>> subsel = sel.xpath('//h1')
+    >>> html_text.selector_to_text(subsel)
+    'Hello'
+
+NB parsel.Selector objects are not cleaned automatically, you need to call
+``html_text.cleaned_selector`` first.
+
+Main functions and objects:
+
+* ``html_text.extract_text`` accepts html and returns extracted text.
+* ``html_text.etree_to_text`` accepts parsed lxml Element and returns
+  extracted text; it is a lower-level function, cleaning is not handled
+  here.
+* ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance which
+  can be used with ``html_text.etree_to_text``; its options are tuned for
+  speed and text extraction quality.
+* ``html_text.cleaned_selector`` accepts html as text or as
+  ``lxml.html.HtmlElement``, and returns cleaned ``parsel.Selector``.
+* ``html_text.selector_to_text`` accepts ``parsel.Selector`` and returns
+  extracted text.
+
+If ``guess_layout`` is True (default), a newline is added before and after
+``newline_tags``, and two newlines are added before and after
+``double_newline_tags``. This heuristic makes the extracted text
+more similar to how it is rendered in the browser. Default newline and double
+newline tags can be found in `html_text.NEWLINE_TAGS`
+and `html_text.DOUBLE_NEWLINE_TAGS`.
+
+It is possible to customize how newlines are added, using ``newline_tags`` and
+``double_newline_tags`` arguments (which are `html_text.NEWLINE_TAGS` and
+`html_text.DOUBLE_NEWLINE_TAGS` by default). For example, don't add a newline
+after ``<div>`` tags:
+
+    >>> newline_tags = html_text.NEWLINE_TAGS - {'div'}
+    >>> html_text.extract_text('<div>Hello</div> world!',
+    ...                        newline_tags=newline_tags)
+    'Hello world!'
+
+Apart from just getting text from the page (e.g. for display or search),
+one intended usage of this library is for machine learning (feature extraction).
+If you want to use the text of the html page as a feature (e.g. for classification),
+this library gives you plain text that you can later feed into a standard text
+classification pipeline.
+If you feel that you need html structure as well, check out
+`webstruct <http://webstruct.readthedocs.io/en/latest/>`_ library.
+
+----
+
+.. image:: https://hyperiongray.s3.amazonaws.com/define-hg.svg
+	:target: https://www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text
+	:alt: define hyperiongray
+
+
+=======
+History
+=======
+
+0.6.0 (2024-04-04)
+------------------
+
+* Moved the Git repository to https://github.com/zytedata/html-text.
+* Added official support for Python 3.9-3.12.
+* Removed support for Python 2.7 and 3.5-3.7.
+* Switched the ``lxml`` dependency to ``lxml[html_clean]`` to support
+  ``lxml >= 5.2.0``.
+* Switch from Travis CI to GitHub Actions.
+* CI improvements.
+
+0.5.2 (2020-07-22)
+------------------
+
+* Handle lxml Cleaner exceptions (a workaround for
+  https://bugs.launchpad.net/lxml/+bug/1838497 );
+* Python 3.8 support;
+* testing improvements.
+
+0.5.1 (2019-05-27)
+------------------
+
+Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
+producing unnecessary spaces after newlines.
+
+0.5.0 (2018-11-19)
+------------------
+
+Parsel dependency is removed in this release,
+though parsel is still supported.
+
+* ``parsel`` package is no longer required to install and use html-text;
+* ``html_text.etree_to_text`` function allows to extract text from
+  lxml Elements;
+* ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance with
+  options tuned for text extraction speed and quality;
+* test and documentation improvements;
+* Python 3.7 support.
+
+0.4.1 (2018-09-25)
+------------------
+
+Fixed a regression in 0.4.0 release: text was empty when
+``html_text.extract_text`` is called with a node with text, but
+without children.
+
+0.4.0 (2018-09-25)
+------------------
+
+This is a backwards-incompatible release: by default html_text functions
+now add newlines after elements, if appropriate, to make the extracted text
+to look more like how it is rendered in a browser.
+
+To turn it off, pass ``guess_layout=False`` option to html_text functions.
+
+* ``guess_layout`` option to to make extracted text look more like how
+  it is rendered in browser.
+* Add tests of layout extraction for real webpages.
+
+
+0.3.0 (2017-10-12)
+------------------
+
+* Expose functions that operate on selectors,
+  use ``.//text()`` to extract text from selector.
+
+
+0.2.1 (2017-05-29)
+------------------
+
+* Packaging fix (include CHANGES.rst)
+
+
+0.2.0 (2017-05-29)
+------------------
+
+* Fix unwanted joins of words with inline tags: spaces are added for inline
+  tags too, but a heuristic is used to preserve punctuation without extra spaces.
+* Accept parsed html trees.
+
+
+0.1.1 (2017-01-16)
+------------------
+
+* Travis-CI and codecov.io integrations added
+
+
+0.1.0 (2016-09-27)
+------------------
+
+* First release on PyPI.
```

#### html2text {}

```diff
@@ -1,29 +1,38 @@
-Metadata-Version: 1.1 Name: html-text Version: 0.5.2 Summary: Extract text from
-HTML Home-page: https://github.com/TeamHG-Memex/html-text Author: Konstantin
+Metadata-Version: 2.1 Name: html_text Version: 0.6.0 Summary: Extract text from
+HTML Home-page: https://github.com/zytedata/html-text Author: Konstantin
 Lopukhin Author-email: kostia.lopuhin@gmail.com License: MIT license
-Description: ============ HTML to Text ============ .. image:: https://
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Natural Language :: English Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 License-File: LICENSE Requires-Dist: lxml
+[html_clean] ============ HTML to Text ============ .. image:: https://
 img.shields.io/pypi/v/html-text.svg :target: https://pypi.python.org/pypi/html-
-text :alt: PyPI Version .. image:: https://img.shields.io/travis/TeamHG-Memex/
-html-text.svg :target: https://travis-ci.org/TeamHG-Memex/html-text :alt: Build
-Status .. image:: http://codecov.io/github/TeamHG-Memex/soft404/
-coverage.svg?branch=master :target: http://codecov.io/github/TeamHG-Memex/html-
-text?branch=master :alt: Code Coverage Extract text from HTML * Free software:
-MIT license How is html_text different from ``.xpath('//text()')`` from LXML or
-``.get_text()`` from Beautiful Soup? * Text extracted with ``html_text`` does
-not contain inline styles, javascript, comments and other text that is not
-normally visible to users; * ``html_text`` normalizes whitespace, but in a way
-smarter than ``.xpath('normalize-space())``, adding spaces around inline
-elements (which are often used as block elements in html markup), and trying to
-avoid adding extra spaces for punctuation; * ``html-text`` can add newlines
-(e.g. after headers or paragraphs), so that the output text looks more like how
-it is rendered in browsers. Install ------- Install with pip:: pip install
-html-text The package depends on lxml, so you might need to install additional
-packages: http://lxml.de/installation.html Usage ----- Extract text from HTML::
->>> import html_text >>> html_text.extract_text('
+text :alt: PyPI Version .. image:: https://img.shields.io/pypi/pyversions/html-
+text.svg :target: https://pypi.python.org/pypi/html-text :alt: Supported Python
+Versions .. image:: https://github.com/zytedata/html-text/workflows/tox/
+badge.svg :target: https://github.com/zytedata/html-text/actions :alt: Build
+Status .. image:: https://codecov.io/github/zytedata/html-text/
+coverage.svg?branch=master :target: https://codecov.io/gh/zytedata/html-text :
+alt: Coverage report Extract text from HTML * Free software: MIT license How is
+html_text different from ``.xpath('//text()')`` from LXML or ``.get_text()``
+from Beautiful Soup? * Text extracted with ``html_text`` does not contain
+inline styles, javascript, comments and other text that is not normally visible
+to users; * ``html_text`` normalizes whitespace, but in a way smarter than
+``.xpath('normalize-space())``, adding spaces around inline elements (which are
+often used as block elements in html markup), and trying to avoid adding extra
+spaces for punctuation; * ``html-text`` can add newlines (e.g. after headers or
+paragraphs), so that the output text looks more like how it is rendered in
+browsers. Install ------- Install with pip:: pip install html-text The package
+depends on lxml, so you might need to install additional packages: http://
+lxml.de/installation.html Usage ----- Extract text from HTML:: >>> import
+html_text >>> html_text.extract_text('
 ************ HHeelllloo ************
 world!') 'Hello\n\nworld!' >>> html_text.extract_text('
 ************ HHeelllloo ************
 world!', guess_layout=False) 'Hello world!' Passed html is first cleaned from
 invisible non-text content such as styles, and then text is extracted. You can
 also pass an already parsed ``lxml.html.HtmlElement``: >>> import html_text >>>
 tree = html_text.parse_html('
@@ -66,41 +75,39 @@
 text of the html page as a feature (e.g. for classification), this library
 gives you plain text that you can later feed into a standard text
 classification pipeline. If you feel that you need html structure as well,
 check out `webstruct
 webstruct.readthedocs.io/en/latest/>`_ library. ---- .. image:: https://
 hyperiongray.s3.amazonaws.com/define-hg.svg :target: https://
 www.hyperiongray.com/?pk_campaign=github&pk_kwd=html-text :alt: define
-hyperiongray ======= History ======= 0.5.2 (2020-07-22) ------------------ *
-Handle lxml Cleaner exceptions (a workaround for https://bugs.launchpad.net/
-lxml/+bug/1838497 ); * Python 3.8 support; * testing improvements. 0.5.1 (2019-
-05-27) ------------------ Fixed whitespace handling when ``guess_punct_space``
-is False: html-text was producing unnecessary spaces after newlines. 0.5.0
-(2018-11-19) ------------------ Parsel dependency is removed in this release,
-though parsel is still supported. * ``parsel`` package is no longer required to
-install and use html-text; * ``html_text.etree_to_text`` function allows to
-extract text from lxml Elements; * ``html_text.cleaner`` is an
-``lxml.html.clean.Cleaner`` instance with options tuned for text extraction
-speed and quality; * test and documentation improvements; * Python 3.7 support.
-0.4.1 (2018-09-25) ------------------ Fixed a regression in 0.4.0 release: text
-was empty when ``html_text.extract_text`` is called with a node with text, but
-without children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
+hyperiongray ======= History ======= 0.6.0 (2024-04-04) ------------------ *
+Moved the Git repository to https://github.com/zytedata/html-text. * Added
+official support for Python 3.9-3.12. * Removed support for Python 2.7 and 3.5-
+3.7. * Switched the ``lxml`` dependency to ``lxml[html_clean]`` to support
+``lxml >= 5.2.0``. * Switch from Travis CI to GitHub Actions. * CI
+improvements. 0.5.2 (2020-07-22) ------------------ * Handle lxml Cleaner
+exceptions (a workaround for https://bugs.launchpad.net/lxml/+bug/1838497 ); *
+Python 3.8 support; * testing improvements. 0.5.1 (2019-05-27) ----------------
+-- Fixed whitespace handling when ``guess_punct_space`` is False: html-text was
+producing unnecessary spaces after newlines. 0.5.0 (2018-11-19) ---------------
+--- Parsel dependency is removed in this release, though parsel is still
+supported. * ``parsel`` package is no longer required to install and use html-
+text; * ``html_text.etree_to_text`` function allows to extract text from lxml
+Elements; * ``html_text.cleaner`` is an ``lxml.html.clean.Cleaner`` instance
+with options tuned for text extraction speed and quality; * test and
+documentation improvements; * Python 3.7 support. 0.4.1 (2018-09-25) ----------
+-------- Fixed a regression in 0.4.0 release: text was empty when
+``html_text.extract_text`` is called with a node with text, but without
+children. 0.4.0 (2018-09-25) ------------------ This is a backwards-
 incompatible release: by default html_text functions now add newlines after
 elements, if appropriate, to make the extracted text to look more like how it
 is rendered in a browser. To turn it off, pass ``guess_layout=False`` option to
 html_text functions. * ``guess_layout`` option to to make extracted text look
 more like how it is rendered in browser. * Add tests of layout extraction for
 real webpages. 0.3.0 (2017-10-12) ------------------ * Expose functions that
 operate on selectors, use ``.//text()`` to extract text from selector. 0.2.1
 (2017-05-29) ------------------ * Packaging fix (include CHANGES.rst) 0.2.0
 (2017-05-29) ------------------ * Fix unwanted joins of words with inline tags:
 spaces are added for inline tags too, but a heuristic is used to preserve
 punctuation without extra spaces. * Accept parsed html trees. 0.1.1 (2017-01-
 16) ------------------ * Travis-CI and codecov.io integrations added 0.1.0
-(2016-09-27) ------------------ * First release on PyPI. Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: MIT License Classifier:
-Natural Language :: English Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+(2016-09-27) ------------------ * First release on PyPI.
```

### Comparing `html_text-0.5.2/html_text.egg-info/SOURCES.txt` & `html_text-0.6.0/html_text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/setup.py` & `html_text-0.6.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,34 +8,33 @@
 
 with open('CHANGES.rst') as history_file:
     history = history_file.read()
 
 
 setup(
     name='html_text',
-    version='0.5.2',
+    version='0.6.0',
     description="Extract text from HTML",
     long_description=readme + '\n\n' + history,
     author="Konstantin Lopukhin",
     author_email='kostia.lopuhin@gmail.com',
-    url='https://github.com/TeamHG-Memex/html-text',
+    url='https://github.com/zytedata/html-text',
     packages=['html_text'],
     include_package_data=True,
-    install_requires=['lxml'],
+    install_requires=['lxml[html_clean]'],
     license="MIT license",
     zip_safe=False,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
-        "Programming Language :: Python :: 2",
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     test_suite='tests',
     tests_require=['pytest'],
 )
```

### Comparing `html_text-0.5.2/tests/test_html_text.py` & `html_text-0.6.0/tests/test_html_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 import glob
 import os
 
-import six
 import pytest
 
 from html_text import (extract_text, parse_html, cleaned_selector,
                        etree_to_text, cleaner, selector_to_text, NEWLINE_TAGS,
                        DOUBLE_NEWLINE_TAGS)
 
 
@@ -123,17 +122,14 @@
     subsel = sel.xpath('//a[@id="extract-me"]')
     assert selector_to_text(subsel, **all_options) == ''
     subsel = sel.xpath('//foo')
     assert selector_to_text(subsel, **all_options) == ''
 
 
 def test_nbsp():
-    if six.PY2:
-        raise pytest.xfail("&nbsp; produces '\xa0' in Python 2, "
-                           "but ' ' in Python 3")
     html = "<h1>Foo&nbsp;Bar</h1>"
     assert extract_text(html) == "Foo Bar"
 
 
 def test_guess_layout():
     html = (u'<title>  title  </title><div>text_1.<p>text_2 text_3</p>'
             '<p id="demo"></p><ul><li>text_4</li><li>text_5</li></ul>'
@@ -194,17 +190,12 @@
     with open(path, 'rb') as f:
         return f.read().decode('utf8')
 
 
 @pytest.mark.parametrize(['page', 'extracted'], _webpage_paths())
 def test_webpages(page, extracted):
     html = _load_file(page)
-    if not six.PY3:
-        # FIXME: &nbsp; produces '\xa0' in Python 2, but ' ' in Python 3
-        # this difference is ignored in this test.
-        # What is the correct behavior?
-        html = html.replace('&nbsp;', ' ')
     expected = _load_file(extracted)
     assert extract_text(html) == expected
 
     tree = cleaner.clean_html(parse_html(html))
     assert etree_to_text(tree) == expected
```

### Comparing `html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html` & `html_text-0.6.0/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt` & `html_text-0.6.0/tests/test_webpages/A Light in the Attic | Books to Scrape - Sandbox.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.html` & `html_text-0.6.0/tests/test_webpages/IANA — IANA-managed Reserved Domains.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt` & `html_text-0.6.0/tests/test_webpages/IANA — IANA-managed Reserved Domains.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.html` & `html_text-0.6.0/tests/test_webpages/Scrapinghub Enterprise Solutions.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/Scrapinghub Enterprise Solutions.txt` & `html_text-0.6.0/tests/test_webpages/Scrapinghub Enterprise Solutions.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html` & `html_text-0.6.0/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt` & `html_text-0.6.0/tests/test_webpages/Tutorial — Webstruct 0.6 documentation.txt`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html` & `html_text-0.6.0/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.html`

 * *Files identical despite different names*

### Comparing `html_text-0.5.2/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt` & `html_text-0.6.0/tests/test_webpages/Webstruct — Webstruct 0.6 documentation.txt`

 * *Files identical despite different names*

