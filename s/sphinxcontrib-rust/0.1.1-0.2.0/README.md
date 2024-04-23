# Comparing `tmp/sphinxcontrib_rust-0.1.1.tar.gz` & `tmp/sphinxcontrib_rust-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_rust-0.1.1.tar", last modified: Sat Apr 20 19:56:59 2024, max compression
+gzip compressed data, was "sphinxcontrib_rust-0.2.0.tar", last modified: Tue Apr 23 00:27:26 2024, max compression
```

## Comparing `sphinxcontrib_rust-0.1.1.tar` & `sphinxcontrib_rust-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:56:59.112760 sphinxcontrib_rust-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)    35145 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6605 2024-04-20 19:56:59.112760 sphinxcontrib_rust-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5850 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/index.rst
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-20 19:56:59.112760 sphinxcontrib_rust-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2618 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:56:59.106760 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:56:59.108760 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/src/
--rw-rw-rw-   0 root         (0) root         (0)     9274 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/src/formats.rs
--rw-rw-rw-   0 root         (0) root         (0)     9967 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     1267 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/src/main.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:56:59.109760 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/target/
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-20 19:56:42.000000 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/target/.rustc_info.json
--rw-r--r--   0 root         (0) root         (0)      177 2024-04-20 19:56:36.000000 sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/target/CACHEDIR.TAG
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:56:59.110760 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/
--rw-rw-rw-   0 root         (0) root         (0)     2745 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8355 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/directives.py
--rw-rw-rw-   0 root         (0) root         (0)     6648 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     4353 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/index.py
--rw-rw-rw-   0 root         (0) root         (0)     3634 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:56:59.111760 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6605 2024-04-20 19:56:59.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-20 19:56:59.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-20 19:56:59.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-20 19:56:59.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-20 19:56:59.000000 sphinxcontrib_rust-0.1.1/sphinxcontrib_rust.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-20 19:56:59.111760 sphinxcontrib_rust-0.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1221 2024-04-20 19:55:24.000000 sphinxcontrib_rust-0.1.1/tests/test_sphinx_build.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 00:27:26.723034 sphinxcontrib_rust-0.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35145 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7573 2024-04-23 00:27:26.722034 sphinxcontrib_rust-0.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6734 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/index.rst
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 00:27:26.723034 sphinxcontrib_rust-0.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2424 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 00:27:26.716034 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/
+-rw-rw-rw-   0 root         (0) root         (0)     1301 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/Cargo.lock
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      640 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/rustfmt.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 00:27:26.716034 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 00:27:26.719034 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/
+-rw-rw-rw-   0 root         (0) root         (0)     3289 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/crate_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3439 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/enum_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4077 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/function_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/impl_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/macro_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)    21534 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)     5954 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/module_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4244 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/struct_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3385 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/trait_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2820 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/type_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4949 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/directives/variable_directive.rs
+-rw-rw-rw-   0 root         (0) root         (0)    15002 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/formats.rs
+-rw-rw-rw-   0 root         (0) root         (0)    11220 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/main.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 00:27:26.720034 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/
+-rw-rw-rw-   0 root         (0) root         (0)     3131 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8830 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/directives.py
+-rw-rw-rw-   0 root         (0) root         (0)     6815 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     4353 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2024-04-23 00:26:10.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/items.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 00:27:26.721034 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7573 2024-04-23 00:27:26.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1170 2024-04-23 00:27:26.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 00:27:26.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-23 00:27:26.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-23 00:27:26.000000 sphinxcontrib_rust-0.2.0/sphinxcontrib_rust.egg-info/top_level.txt
```

### Comparing `sphinxcontrib_rust-0.1.1/LICENSE` & `sphinxcontrib_rust-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_rust-0.1.1/PKG-INFO` & `sphinxcontrib_rust-0.2.0/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: sphinxcontrib-rust
-Version: 0.1.1
-Summary: Sphinx extension for documenting Rust projects
-Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Sphinx :: Domain
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Rust
-Classifier: Topic :: Documentation :: Sphinx
-Requires-Python: >=3.9
-Description-Content-Type: text/plain
-License-File: LICENSE
-Requires-Dist: sphinx<8,>=7
-Provides-Extra: dev
-Requires-Dist: beautifulsoup4; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: lxml; extra == "dev"
-Requires-Dist: pylint; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: sphinx_rtd_theme; extra == "dev"
-
 ==================
 Sphinxcontrib-rust
 ==================
 
 .. warning::
 
    This project is still under development. While basic features are
@@ -30,15 +9,15 @@
    can be checked from reading the :doc:`TODO`.
 
 This is a `Sphinx`_ extension for integrating Rust programming language
 projects in Sphinx builds.
 
 You can read this documentation on `Gitlab Pages`_ or `readthedocs`_.
 
-.. _`Gitlab Pages`: https://sphinxcontrib-rust-mmc691-8fb22cc6152ca3a233f41dbc6179d6a5fd539.gitlab.io/
+.. _`Gitlab Pages`: https://munir0b0t.gitlab.io/sphinxcontrib-rust
 
 .. _`readthedocs`: https://sphinxcontrib-rust.readthedocs.io/en/latest/
 
 Motivation
 ----------
 
 This is primarily meant for teams and projects that are already
@@ -70,19 +49,28 @@
 
 Both components are installed when installing the Python package with
 
 .. code-block::
 
    pip install sphinxcontrib-rust
 
-The installation will check for a ``cargo`` executable in the ``$PATH``
-variable in the environment and will use that to install the Rust executable.
+The installation will check for ``cargo`` in the ``$PATH`` environment
+variable and will use that to build and install the Rust executable.
+
+The executable is built with the Rust code shipped with the Python package.
+This ensures that the Rust executable and Python package are always compatible
+with each other.
 
 Make sure that the path where ``cargo`` installs the executable is in
-``$PATH`` as well. The executable is used during the Sphinx build.
+``$PATH`` as well. If the default installation directory is not part of the
+``$PATH`` environment, the installed executable should be specified in the Sphinx
+configuration with ``rust_rustdocgen`` option.
+
+The Rust executable may also be installed independently from crates.io or built
+with the shipped source code.
 
 With reStructuredText
 +++++++++++++++++++++
 
 To use the extension with rst rustdoc comments, simply add the extension to the
 ``conf.py`` file. The various configuration options supported by the extension,
 along with their defaults, are documented below.
@@ -106,15 +94,16 @@
    .. toctree::
 
       docs/crates/my_crate/main
       docs/crates/my_crate/lib
 
 The extension also adds various roles for Rust items. The roles can be used
 within the Sphinx documentation and also within the docstrings themselves.
-The roles are documented in :doc:`docs/roles`.
+The roles can even be used in docstrings of a different language that is part of
+the same Sphinx project. The roles are documented in :doc:`docs/roles`.
 
 The extension also provides various :doc:`docs/directives` and
 :doc:`docs/indices` that can be used in the documentation.
 
 With Markdown
 +++++++++++++
 
@@ -159,26 +148,31 @@
 syntax`_ for the roles.
 
 Options
 +++++++
 
 Options are simply Python variables set in the ``conf.py`` file.
 
-:rust_crates: A dict of crate names and their source code directories.
-:rust_doc_dir: The directory under which to write the docs. Must be a
+:rust_crates: (Required) A dict of crate names and their source code directories.
+:rust_doc_dir: (Required) The directory under which to write the docs. Must be a
                directory that will be read by Sphinx and not under
                the build directory.
-:rust_rustdoc_fmt: Either ``"rst"`` or ``"md"``.
-                   (Default: ``"rst"``, but likely to change once stable).
-:rust_visibilty: Only includes documentation and indexes for items
-                 with visibility greater than or equal to the setting.
-                 The value can be ``"pub"``, ``"crate"`` or ``"pvt"``.
-                 Visibility restrictions like ``super`` and ``in <path>`` are
-                 not supported currently and are treated as private.
-                 (Default: ``"pub"``).
+:rust_rustdocgen: The path to the ``sphinx-rustdocgen`` executable to use.
+                  The path must be an absolute path or relative to Sphinx's
+                  working directory. (Default: Obtained from the ``$PATH``
+                  environment variable.)
+:rust_no_generate: Do not scan the crate and generate documents. Useful
+                   for testing with existing docs. (Default: False)
+:rust_rustdoc_fmt: Either ``rst`` or ``md``. (Default: ``rst``)
+:rust_visibility: Only includes documentation and indexes for items
+                  with visibility greater than or equal to the setting.
+                  The value can be ``pub``, ``crate`` or ``pvt``.
+                  Visibility restrictions like ``super`` and ``in <path>`` are
+                  not supported currently and are treated as private. (Default:
+                  ``pub``).
 
 .. _`Sphinx`: https://www.sphinx-doc.org/en/master/index.html
 .. _`myst-parser`: https://myst-parser.readthedocs.io/en/latest/index.html
 .. _`configured for Markdown builds`: https://www.sphinx-doc.org/en/master/usage/markdown.html
 .. _`configuration options for MyST`: https://myst-parser.readthedocs.io/en/latest/configuration.html
 .. _`myst-parser syntax`:
    https://myst-parser.readthedocs.io/en/latest/syntax/roles-and-directives.html#roles-an-in-line-extension-point
@@ -190,10 +184,12 @@
    :maxdepth: 2
    :glob:
 
    docs/including
    docs/roles
    docs/directives
    docs/indices
+   docs/developing
    docs/sphinx-rustdocgen
    docs/sphinx-extension
    TODO
+   CONTRIBUTING
```

### Comparing `sphinxcontrib_rust-0.1.1/index.rst` & `sphinxcontrib_rust-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: sphinxcontrib-rust
+Version: 0.2.0
+Summary: Sphinx extension for documenting Rust projects
+Home-page: https://gitlab.com/munir0b0t/sphinxcontrib-rust
+Author: Munir Contractor
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: Sphinx :: Domain
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Rust
+Classifier: Topic :: Documentation :: Sphinx
+Requires-Python: >=3.9
+Description-Content-Type: text/plain
+License-File: LICENSE
+Requires-Dist: sphinx<8,>=7
+Provides-Extra: dev
+Requires-Dist: beautifulsoup4; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: lxml; extra == "dev"
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: sphinx_rtd_theme; extra == "dev"
+
 ==================
 Sphinxcontrib-rust
 ==================
 
 .. warning::
 
    This project is still under development. While basic features are
@@ -9,15 +32,15 @@
    can be checked from reading the :doc:`TODO`.
 
 This is a `Sphinx`_ extension for integrating Rust programming language
 projects in Sphinx builds.
 
 You can read this documentation on `Gitlab Pages`_ or `readthedocs`_.
 
-.. _`Gitlab Pages`: https://sphinxcontrib-rust-mmc691-8fb22cc6152ca3a233f41dbc6179d6a5fd539.gitlab.io/
+.. _`Gitlab Pages`: https://munir0b0t.gitlab.io/sphinxcontrib-rust
 
 .. _`readthedocs`: https://sphinxcontrib-rust.readthedocs.io/en/latest/
 
 Motivation
 ----------
 
 This is primarily meant for teams and projects that are already
@@ -49,19 +72,28 @@
 
 Both components are installed when installing the Python package with
 
 .. code-block::
 
    pip install sphinxcontrib-rust
 
-The installation will check for a ``cargo`` executable in the ``$PATH``
-variable in the environment and will use that to install the Rust executable.
+The installation will check for ``cargo`` in the ``$PATH`` environment
+variable and will use that to build and install the Rust executable.
+
+The executable is built with the Rust code shipped with the Python package.
+This ensures that the Rust executable and Python package are always compatible
+with each other.
 
 Make sure that the path where ``cargo`` installs the executable is in
-``$PATH`` as well. The executable is used during the Sphinx build.
+``$PATH`` as well. If the default installation directory is not part of the
+``$PATH`` environment, the installed executable should be specified in the Sphinx
+configuration with ``rust_rustdocgen`` option.
+
+The Rust executable may also be installed independently from crates.io or built
+with the shipped source code.
 
 With reStructuredText
 +++++++++++++++++++++
 
 To use the extension with rst rustdoc comments, simply add the extension to the
 ``conf.py`` file. The various configuration options supported by the extension,
 along with their defaults, are documented below.
@@ -85,15 +117,16 @@
    .. toctree::
 
       docs/crates/my_crate/main
       docs/crates/my_crate/lib
 
 The extension also adds various roles for Rust items. The roles can be used
 within the Sphinx documentation and also within the docstrings themselves.
-The roles are documented in :doc:`docs/roles`.
+The roles can even be used in docstrings of a different language that is part of
+the same Sphinx project. The roles are documented in :doc:`docs/roles`.
 
 The extension also provides various :doc:`docs/directives` and
 :doc:`docs/indices` that can be used in the documentation.
 
 With Markdown
 +++++++++++++
 
@@ -138,26 +171,31 @@
 syntax`_ for the roles.
 
 Options
 +++++++
 
 Options are simply Python variables set in the ``conf.py`` file.
 
-:rust_crates: A dict of crate names and their source code directories.
-:rust_doc_dir: The directory under which to write the docs. Must be a
+:rust_crates: (Required) A dict of crate names and their source code directories.
+:rust_doc_dir: (Required) The directory under which to write the docs. Must be a
                directory that will be read by Sphinx and not under
                the build directory.
-:rust_rustdoc_fmt: Either ``"rst"`` or ``"md"``.
-                   (Default: ``"rst"``, but likely to change once stable).
-:rust_visibilty: Only includes documentation and indexes for items
-                 with visibility greater than or equal to the setting.
-                 The value can be ``"pub"``, ``"crate"`` or ``"pvt"``.
-                 Visibility restrictions like ``super`` and ``in <path>`` are
-                 not supported currently and are treated as private.
-                 (Default: ``"pub"``).
+:rust_rustdocgen: The path to the ``sphinx-rustdocgen`` executable to use.
+                  The path must be an absolute path or relative to Sphinx's
+                  working directory. (Default: Obtained from the ``$PATH``
+                  environment variable.)
+:rust_no_generate: Do not scan the crate and generate documents. Useful
+                   for testing with existing docs. (Default: False)
+:rust_rustdoc_fmt: Either ``rst`` or ``md``. (Default: ``rst``)
+:rust_visibility: Only includes documentation and indexes for items
+                  with visibility greater than or equal to the setting.
+                  The value can be ``pub``, ``crate`` or ``pvt``.
+                  Visibility restrictions like ``super`` and ``in <path>`` are
+                  not supported currently and are treated as private. (Default:
+                  ``pub``).
 
 .. _`Sphinx`: https://www.sphinx-doc.org/en/master/index.html
 .. _`myst-parser`: https://myst-parser.readthedocs.io/en/latest/index.html
 .. _`configured for Markdown builds`: https://www.sphinx-doc.org/en/master/usage/markdown.html
 .. _`configuration options for MyST`: https://myst-parser.readthedocs.io/en/latest/configuration.html
 .. _`myst-parser syntax`:
    https://myst-parser.readthedocs.io/en/latest/syntax/roles-and-directives.html#roles-an-in-line-extension-point
@@ -169,10 +207,12 @@
    :maxdepth: 2
    :glob:
 
    docs/including
    docs/roles
    docs/directives
    docs/indices
+   docs/developing
    docs/sphinx-rustdocgen
    docs/sphinx-extension
    TODO
+   CONTRIBUTING
```

### Comparing `sphinxcontrib_rust-0.1.1/setup.py` & `sphinxcontrib_rust-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 
 LONG_DESC = Path("index.rst").read_text(encoding="utf-8")
 
-__VERSION__ = "0.1.1"
+__VERSION__ = "0.2.0"
 __THIS_DIR = Path(__file__).parent.absolute()
 __CARGO = which("cargo")
 if not __CARGO:
     raise ValueError("Could not find cargo executable on path")
 
 
 # XXX: Use pip install -vvv -e to debug the build.
@@ -29,32 +29,26 @@
         check=True,
         text=True,
         cwd=f"{__THIS_DIR}/sphinx-rustdocgen",
     )
 
 
 class CargoBuild(develop):
-    """Command to build the cargo crate during installation"""
+    """Command to install debug version of the sphinx-rustdocgen executable"""
 
     def run(self):
-        run_cargo("build")
+        run_cargo("install", "--debug", "--path", ".")
         develop.run(self)
 
 
 class CargoInstall(install):
-    """Command to build the cargo crate during installation"""
+    """Command to install release version of the sphinx-rustdocgen executable"""
 
     def run(self):
-        try:
-            # Try installing the specific version.
-            # This should almost always succeed, except when building a new release.
-            run_cargo("install", f"sphinx-rustdocgen@{__VERSION__}")
-        except subprocess.CalledProcessError:
-            # Try any version if the exact version cannot be installed.
-            run_cargo("install", "sphinx-rustdocgen")
+        run_cargo("install", "--path", ".")
         install.run(self)
 
 
 setup(
     name="sphinxcontrib-rust",
     version=__VERSION__,
     description="Sphinx extension for documenting Rust projects",
@@ -84,8 +78,10 @@
     packages=find_packages(),
     package_data={"sphinxcontrib_rust": ["sphinx-rustdocgen/**"]},
     include_package_data=True,
     cmdclass={
         "develop": CargoBuild,
         "install": CargoInstall,
     },
+    url="https://gitlab.com/munir0b0t/sphinxcontrib-rust",
+    author="Munir Contractor",
 )
```

### Comparing `sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/src/lib.rs` & `sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 mod formats;
 
 use std::fs::{create_dir_all, File};
 use std::io::{Read, Write};
 use std::os::unix::fs::MetadataExt;
 use std::path::{Path, PathBuf};
 
-use directives::extract_doc_from_attrs;
-
-use crate::directives::{CrateDirective, Directive, ModuleDirective};
+pub use crate::directives::DirectiveVisibility;
+use crate::directives::{extract_doc_from_attrs, CrateDirective, Directive, ModuleDirective};
 pub use crate::formats::Format;
 
 /// Read a Rust source code file and generate its AST.
 ///
 /// Args:
 ///     :path: The path to the file to read.
 ///
@@ -173,29 +172,32 @@
             "Could not locate file for module {}",
             &module_directive.ident
         );
     }
     mod_file
 }
 
-/// The different types of module files that can be encountered.
+/// The different types of files that can be encountered.
 enum FileType {
-    /// The file with the main function.
-    Main(String),
-    /// The crate's library module.
+    /// A file that compiles to a binary
+    Bin(String),
+    /// The crate's library file.
     Lib(String),
-    /// All other modules within a crate.
+    /// All other modules within the crate's library.
     Mod(String),
 }
 
 /// Macro to push the module files to the files vec for processing
 ///
-/// This tests the macro directive and also removes a clippy warning.
+/// Args:
+///     :files: The files list to push the files to.
+///     :parent: The parent path of the module or crate's file.
+///     :directive: The directive for the module or crate.
 macro_rules! push_module_files {
-    ($parent:expr, $directive:expr, $files:expr) => {
+    ($files:expr, $parent:expr, $directive:expr) => {
         for directive in &$directive.items {
             if let Directive::Module(m) = directive {
                 if m.items.is_empty() {
                     // Push the file to the vec
                     $files.push((
                         find_mod_file($parent, m),
                         FileType::Mod(m.name.clone()),
@@ -211,61 +213,95 @@
 ///
 /// Args:
 ///     :crate_name: The name of the crate.
 ///     :crate_src_dir: The directory with the crate source code.
 ///     :output_dir: The directory where to produce the generated documentation
 ///         files.
 ///     :format: The format of the docstrings.
-pub fn traverse_crate(crate_name: &str, crate_src_dir: &Path, output_dir: &Path, format: Format) {
+pub fn traverse_crate(
+    crate_name: &str,
+    crate_src_dir: &Path,
+    output_dir: &Path,
+    format: Format,
+    max_visibility: DirectiveVisibility,
+) {
     let crate_src_dir = check_crate_src_dir(crate_name, crate_src_dir);
     let output_dir = check_and_create_output_dir(crate_name, output_dir);
 
     // Vec of files that we need to process
     let mut files = vec![];
 
     // Add the main file if it exists.
     // TODO: Make configurable
     let main = crate_src_dir.join("main.rs");
     if main.is_file() {
-        files.push((main, FileType::Main(crate_name.to_string()), None));
+        files.push((main, FileType::Bin(crate_name.to_string()), None));
+    }
+
+    // Check src/bin for other executables
+    let bin_dir = crate_src_dir.join("bin");
+    if bin_dir.is_dir() {
+        for path in bin_dir.read_dir().unwrap() {
+            let path = path.unwrap().path();
+            if path.is_dir() {
+                let executable = path
+                    .components()
+                    .last()
+                    .unwrap()
+                    .as_os_str()
+                    .to_str()
+                    .unwrap()
+                    .to_string();
+                files.push((path.join("main.rs"), FileType::Bin(executable), None));
+            }
+            else if path.extension() == Some("rs".as_ref()) {
+                let executable = path.file_stem().unwrap().to_str().unwrap().to_string();
+                files.push((path, FileType::Bin(executable), None));
+            }
+        }
     }
 
     // Add the lib file if it exists.
     // TODO: Make configurable
     let lib = crate_src_dir.join("lib.rs");
     if lib.is_file() {
         files.push((lib, FileType::Lib(crate_name.to_string()), None));
     }
 
     while let Some((path, file, vis)) = files.pop() {
         log::debug!("Processing file {}", path.to_str().unwrap());
 
         let ast = read_rs_file(&path);
         let text = match file {
-            FileType::Main(crate_name) => {
-                let mut text = format.make_title(&format!("{} documentation", &crate_name));
-                text.append(&mut extract_doc_from_attrs(&ast.attrs));
+            FileType::Bin(exe_name) => {
+                let mut text = format.make_title(&format!("{exe_name} documentation"), false);
+                text.extend(format.format_content(extract_doc_from_attrs(&ast.attrs)));
                 text
             }
             FileType::Lib(crate_name) => {
                 let crate_directive = CrateDirective::new(&crate_name, &ast);
 
-                push_module_files!(path.parent().unwrap(), crate_directive, files);
+                push_module_files!(files, path.parent().unwrap(), crate_directive);
 
-                let mut text = format.make_title(&format!("Crate {crate_name} documentation"));
-                text.append(&mut format.get_content(Directive::Crate(crate_directive)));
+                let mut text =
+                    format.make_title(&format!("Crate {crate_name} documentation"), false);
+                text.extend(
+                    format.format_directive(Directive::Crate(crate_directive), &max_visibility),
+                );
                 text
             }
             FileType::Mod(module) => {
                 let module_directive = ModuleDirective::new(&module, &ast, vis.unwrap());
 
-                push_module_files!(path.parent().unwrap(), module_directive, files);
+                push_module_files!(files, path.parent().unwrap(), module_directive);
 
-                let mut text = format.make_title(&format!("Module {}", &module_directive.ident));
-                text.append(&mut format.get_content(Directive::Module(module_directive)));
+                let mut text = format.make_title(&format!("mod {}", &module_directive.ident), true);
+                text.extend(
+                    format.format_directive(Directive::Module(module_directive), &max_visibility),
+                );
                 text
             }
         };
 
         let (doc_file_name, mut doc_file) = get_doc_file_from_path(
             &output_dir,
             path.strip_prefix(&crate_src_dir).unwrap_or(&path),
@@ -289,10 +325,11 @@
         // creating unnecessary test files when the source code itself can be
         // used.
         traverse_crate(
             "sphinx-rustdocgen",
             Path::new("."),
             Path::new("../docs/crates"),
             Format::Rst,
+            DirectiveVisibility::Pvt,
         );
     }
 }
```

### Comparing `sphinxcontrib_rust-0.1.1/sphinx-rustdocgen/src/main.rs` & `sphinxcontrib_rust-0.2.0/sphinx-rustdocgen/src/main.rs`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,49 @@
 //! crates. It is tightly coupled with the sphinxcontrib-rust extension and is
 //! used by it during the Sphinx build process.
 //!
 //! Usage:
 //!
 //! .. code-block::
 //!
-//!    sphinx-rustdocgen <crate_name> <crate_src_dir> <output_dir> <format>
+//!    sphinx-rustdocgen <crate_name> <crate_src_dir> <output_dir> <format> \
+//!                      <visibility>
 //!
 //! .. toctree::
-//!    :caption: Crate documentation
 //!    :maxdepth: 3
 //!
 //!    /docs/crates/sphinx-rustdocgen/lib
 
 use std::env;
 use std::path::Path;
 use std::str::FromStr;
 
-use sphinx_rustdocgen::{traverse_crate, Format};
+use sphinx_rustdocgen::{traverse_crate, DirectiveVisibility, Format};
 
-static USAGE: &str = "sphinx-rustdocgen <crate_name> <crate_src_dir> <output_dir> <format>";
+static USAGE: &str =
+    "sphinx-rustdocgen <crate_name> <crate_src_dir> <output_dir> <format> <visibility>";
 
 fn main() {
     let args: Vec<String> = env::args().collect();
-    if args.len() < 5 {
+    if args.len() < 6 {
         panic!("Invalid number of arguments: {}\n\n{}", args.len(), USAGE);
     }
 
     // Parse args
     let crate_name = args.get(1).unwrap();
     let crate_src_dir = Path::new(args.get(2).unwrap());
     let output_dir = Path::new(args.get(3).unwrap());
     let format = Format::from_str(args.get(4).unwrap()).unwrap_or_else(|_| {
         panic!(
             "Unknown format \"{}\". Must be one of rst or md.",
             args.get(4).unwrap(),
         )
     });
+    let visibility = DirectiveVisibility::from_str(args.get(5).unwrap()).unwrap_or_else(|_| {
+        panic!(
+            "Unknown visibility \"{}\". Must be one of pub, crate or pvt.",
+            args.get(5).unwrap()
+        )
+    });
 
-    traverse_crate(crate_name, crate_src_dir, output_dir, format)
+    traverse_crate(crate_name, crate_src_dir, output_dir, format, visibility)
 }
```

### Comparing `sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/__init__.py` & `sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Init module for the extension with the ``setup`` function used by Sphinx"""
 
+import os
 from importlib.metadata import version
 import subprocess
 from shutil import which
 from typing import Any, Mapping
 
 import sphinx.config
 from sphinx.application import Sphinx
@@ -18,75 +19,88 @@
 
 """The configuration options added by the extension.
 
 Each entry is tuple consisting of
 * The option name.
 * The default value.
 * The rebuild condition .
+
   * "html": Change needs a full rebuild of HTML.
   * "env": Change needs a full rebuild of the build environment.
   * "": No rebuild required.
+
 * A list of types for the value.
 """
 __CONFIG_OPTIONS = (
     ("rust_crates", None, "env", [dict]),
     ("rust_doc_dir", None, "env", [str]),
+    ("rust_rustdocgen", None, "env", [str]),
+    ("rust_no_generate", False, "env", [bool]),
     ("rust_rustdoc_fmt", "rst", "env", [str]),
     ("rust_visibility", "pub", "html", [str]),  # TODO: Define a type for this
 )
 
 """
 See https://www.sphinx-doc.org/en/master/extdev/index.html#extension-metadata
 """
 __METADATA = {
     "version": __VERSION__,
     "parallel_read_safe": True,
     "parallel_write_safe": True,
 }
-__RUSTDOCGEN = which("sphinx-rustdocgen")
 
 
+# noinspection PyUnusedLocal
 def generate_docs(app: Sphinx, config: sphinx.config.Config):
     """Generate the Rust docs once the configuration has been read
 
     Args:
         :app: The Sphinx application.
         :config: The parsed configuration.
     """
+    # pylint: disable=unused-argument
+    if config.rust_no_generate:
+        return
+
+    executable = config.rust_rustdocgen or which("sphinx-rustdocgen")
+    if executable is None:
+        raise ValueError(
+            "Could not find the sphinx-rustdocgen executable. "
+            "Make sure it is configured or on the system path."
+        )
+    if not os.access(executable, os.X_OK):
+        raise ValueError(f"{executable} is not an executable file.")
+
     for crate, src_dir in config.rust_crates.items():
         __LOGGER.info(
             "[sphinxcontrib_rust] Processing contents of crate %s from directory %s",
             crate,
             src_dir,
         )
         __LOGGER.info(
             "[sphinxcontrib_rust] Generated files will be saved in %s/%s",
             config.rust_doc_dir,
             crate,
         )
         subprocess.run(
             [
-                __RUSTDOCGEN,
+                executable,
                 crate,
                 src_dir,
                 config.rust_doc_dir,
                 config.rust_rustdoc_fmt,
+                config.rust_visibility,
             ],
             check=True,
             text=True,
         )
 
 
 def setup(app: Sphinx) -> Mapping[str, Any]:
     """Set up the extension"""
-    if __RUSTDOCGEN is None:
-        raise ValueError(
-            "Could not find the sphinx-rustdocgen executable. "
-            "Make sure it is installed and available on the default PATH."
-        )
 
     app.require_sphinx("7.0")
 
     for extension in __REQUIRED_EXTENSIONS:
         app.setup_extension(extension)
 
     for option in __CONFIG_OPTIONS:
```

### Comparing `sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/directives.py` & `sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/directives.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,22 @@
 )
 from sphinx.util.nodes import make_id
 
 from sphinxcontrib_rust.items import RustItem, RustItemType
 
 
 class RustDirective(ABC, ObjectDescription[Sequence[str]]):
-    """Base class for Rust directives"""
+    """Base class for Rust directives.
+
+    This class implements most of the logic for the directives. For each directive,
+    there is a subclass that overrides any directive specific behaviour.
+
+    The input for the directives is generated with the Rust code in
+    :rust:enum:`sphinx-rustdocgen::directives::Directive`
+    """
 
     option_spec = {
         "no-index": directives.flag,
         "vis": directives.unchanged_required,
         "sig": directives.unchanged,
         "toc": directives.unchanged,
         "type": directives.unchanged,
@@ -173,14 +180,17 @@
 class RustCrateDirective(RustDirective):
     """Directive for handling crate documentation"""
 
     @property
     def rust_item_type(self) -> RustItemType:
         return RustItemType.CRATE
 
+    def _toc_entry_name(self, sig_node: addnodes.desc_signature) -> str:
+        return ""
+
 
 class RustEnumDirective(RustDirective):
     """Directive for handling enum documentation"""
 
     @property
     def rust_item_type(self) -> RustItemType:
         return RustItemType.ENUM
@@ -213,14 +223,17 @@
 class RustModuleDirective(RustDirective):
     """Directive for handling module documentation"""
 
     @property
     def rust_item_type(self) -> RustItemType:
         return RustItemType.MODULE
 
+    def _toc_entry_name(self, sig_node: addnodes.desc_signature) -> str:
+        return ""
+
 
 class RustStructDirective(RustDirective):
     """Directive for handling struct documentation"""
 
     @property
     def rust_item_type(self) -> RustItemType:
         return RustItemType.STRUCT
```

### Comparing `sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/domain.py` & `sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         fromdocname: str,
         builder: Builder,
         typ: str,
         target: str,
         node: pending_xref,
         contnode: Element,
     ) -> Element | None:
+        """Resolve a reference to a Rust item with the directive type specified"""
         # pylint:disable=too-many-arguments
         match = self._find_match(target, typ)
         return (
             make_refnode(
                 builder,
                 fromdocname,
                 match.docname,
@@ -180,14 +181,15 @@
         env: BuildEnvironment,
         fromdocname: str,
         builder: Builder,
         target: str,
         node: pending_xref,
         contnode: Element,
     ) -> list[tuple[str, Element]]:
+        """Resolve a reference to a Rust item with an unspecified directive type"""
         # pylint:disable=too-many-arguments
         match = self._find_match(target)
         return (
             make_refnode(
                 builder,
                 fromdocname,
                 match.docname,
```

### Comparing `sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/index.py` & `sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/index.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_rust-0.1.1/sphinxcontrib_rust/items.py` & `sphinxcontrib_rust-0.2.0/sphinxcontrib_rust/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sphinx.domains import ObjType
 
 # noinspection PyProtectedMember
 from sphinx.locale import _  # pylint:disable=protected-access
 
 
 class RustItemType(Enum):
-    """The various Rust objects"""
+    """The various Rust items that are supported by the directives"""
 
     # XXX: Python 3.11 has StrEnum that can be used here
     #      but that would limit the Python version supported.
     #      Once older versions are EOL, this can be used.
 
     CRATE = "crate"
     ENUM = "enum"
@@ -84,24 +84,25 @@
     """
 
     NORMAL = 0
     WITH_SUB_ENTRIES = 1
     SUB_ENTRY = 2
 
 
+# pylint: disable=anomalous-backslash-in-string
 @dataclass(frozen=True)
 class RustItem:
     """A dataclass for holding the details of a Sphinx object for Rust domain
 
     Attributes:
         :name: The name of the object.
         :dispname: The name of the object used in directives and references.
-        :type_: The object type.
+        :type\_: The object type.
         :docname: The document the object is defined in. This is the generated
-            reStructured Text document, not the source code.
+                  reStructured Text document, not the source code.
         :qualifier: Qualifier for the description.
         :anchor: Anchor for the entry within the docname.
         :priority: The search priority for the object.
         :entry_type: The Sphinx index entry type for the object.
     """
 
     # pylint: disable=too-many-instance-attributes
```

### Comparing `sphinxcontrib_rust-0.1.1/sphinxcontrib_rust.egg-info/PKG-INFO` & `sphinxcontrib_rust-0.2.0/sphinxcontrib_rust.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-rust
-Version: 0.1.1
+Version: 0.2.0
 Summary: Sphinx extension for documenting Rust projects
+Home-page: https://gitlab.com/munir0b0t/sphinxcontrib-rust
+Author: Munir Contractor
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Domain
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Documentation :: Sphinx
 Requires-Python: >=3.9
 Description-Content-Type: text/plain
@@ -30,15 +32,15 @@
    can be checked from reading the :doc:`TODO`.
 
 This is a `Sphinx`_ extension for integrating Rust programming language
 projects in Sphinx builds.
 
 You can read this documentation on `Gitlab Pages`_ or `readthedocs`_.
 
-.. _`Gitlab Pages`: https://sphinxcontrib-rust-mmc691-8fb22cc6152ca3a233f41dbc6179d6a5fd539.gitlab.io/
+.. _`Gitlab Pages`: https://munir0b0t.gitlab.io/sphinxcontrib-rust
 
 .. _`readthedocs`: https://sphinxcontrib-rust.readthedocs.io/en/latest/
 
 Motivation
 ----------
 
 This is primarily meant for teams and projects that are already
@@ -70,19 +72,28 @@
 
 Both components are installed when installing the Python package with
 
 .. code-block::
 
    pip install sphinxcontrib-rust
 
-The installation will check for a ``cargo`` executable in the ``$PATH``
-variable in the environment and will use that to install the Rust executable.
+The installation will check for ``cargo`` in the ``$PATH`` environment
+variable and will use that to build and install the Rust executable.
+
+The executable is built with the Rust code shipped with the Python package.
+This ensures that the Rust executable and Python package are always compatible
+with each other.
 
 Make sure that the path where ``cargo`` installs the executable is in
-``$PATH`` as well. The executable is used during the Sphinx build.
+``$PATH`` as well. If the default installation directory is not part of the
+``$PATH`` environment, the installed executable should be specified in the Sphinx
+configuration with ``rust_rustdocgen`` option.
+
+The Rust executable may also be installed independently from crates.io or built
+with the shipped source code.
 
 With reStructuredText
 +++++++++++++++++++++
 
 To use the extension with rst rustdoc comments, simply add the extension to the
 ``conf.py`` file. The various configuration options supported by the extension,
 along with their defaults, are documented below.
@@ -106,15 +117,16 @@
    .. toctree::
 
       docs/crates/my_crate/main
       docs/crates/my_crate/lib
 
 The extension also adds various roles for Rust items. The roles can be used
 within the Sphinx documentation and also within the docstrings themselves.
-The roles are documented in :doc:`docs/roles`.
+The roles can even be used in docstrings of a different language that is part of
+the same Sphinx project. The roles are documented in :doc:`docs/roles`.
 
 The extension also provides various :doc:`docs/directives` and
 :doc:`docs/indices` that can be used in the documentation.
 
 With Markdown
 +++++++++++++
 
@@ -159,26 +171,31 @@
 syntax`_ for the roles.
 
 Options
 +++++++
 
 Options are simply Python variables set in the ``conf.py`` file.
 
-:rust_crates: A dict of crate names and their source code directories.
-:rust_doc_dir: The directory under which to write the docs. Must be a
+:rust_crates: (Required) A dict of crate names and their source code directories.
+:rust_doc_dir: (Required) The directory under which to write the docs. Must be a
                directory that will be read by Sphinx and not under
                the build directory.
-:rust_rustdoc_fmt: Either ``"rst"`` or ``"md"``.
-                   (Default: ``"rst"``, but likely to change once stable).
-:rust_visibilty: Only includes documentation and indexes for items
-                 with visibility greater than or equal to the setting.
-                 The value can be ``"pub"``, ``"crate"`` or ``"pvt"``.
-                 Visibility restrictions like ``super`` and ``in <path>`` are
-                 not supported currently and are treated as private.
-                 (Default: ``"pub"``).
+:rust_rustdocgen: The path to the ``sphinx-rustdocgen`` executable to use.
+                  The path must be an absolute path or relative to Sphinx's
+                  working directory. (Default: Obtained from the ``$PATH``
+                  environment variable.)
+:rust_no_generate: Do not scan the crate and generate documents. Useful
+                   for testing with existing docs. (Default: False)
+:rust_rustdoc_fmt: Either ``rst`` or ``md``. (Default: ``rst``)
+:rust_visibility: Only includes documentation and indexes for items
+                  with visibility greater than or equal to the setting.
+                  The value can be ``pub``, ``crate`` or ``pvt``.
+                  Visibility restrictions like ``super`` and ``in <path>`` are
+                  not supported currently and are treated as private. (Default:
+                  ``pub``).
 
 .. _`Sphinx`: https://www.sphinx-doc.org/en/master/index.html
 .. _`myst-parser`: https://myst-parser.readthedocs.io/en/latest/index.html
 .. _`configured for Markdown builds`: https://www.sphinx-doc.org/en/master/usage/markdown.html
 .. _`configuration options for MyST`: https://myst-parser.readthedocs.io/en/latest/configuration.html
 .. _`myst-parser syntax`:
    https://myst-parser.readthedocs.io/en/latest/syntax/roles-and-directives.html#roles-an-in-line-extension-point
@@ -190,10 +207,12 @@
    :maxdepth: 2
    :glob:
 
    docs/including
    docs/roles
    docs/directives
    docs/indices
+   docs/developing
    docs/sphinx-rustdocgen
    docs/sphinx-extension
    TODO
+   CONTRIBUTING
```

