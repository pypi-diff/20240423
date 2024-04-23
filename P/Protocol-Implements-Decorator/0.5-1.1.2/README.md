# Comparing `tmp/protocol-implements-decorator-0.5.tar.gz` & `tmp/protocol_implements_decorator-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protocol-implements-decorator-0.5.tar", last modified: Tue Apr  5 02:32:10 2022, max compression
+gzip compressed data, was "protocol_implements_decorator-1.1.2.tar", last modified: Tue Apr 23 03:15:27 2024, max compression
```

## Comparing `protocol-implements-decorator-0.5.tar` & `protocol_implements_decorator-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,56 @@
-drwxrwxrwx   0        0        0        0 2022-04-05 02:32:10.482350 protocol-implements-decorator-0.5/
--rw-rw-rw-   0        0        0      707 2022-04-05 02:32:10.482350 protocol-implements-decorator-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1870 2022-04-05 01:45:40.000000 protocol-implements-decorator-0.5/README.md
-drwxrwxrwx   0        0        0        0 2022-04-05 02:32:10.452696 protocol-implements-decorator-0.5/protocol_implements_decorator/
--rw-rw-rw-   0        0        0       22 2022-04-05 01:44:07.000000 protocol-implements-decorator-0.5/protocol_implements_decorator/__init__.py
--rw-rw-rw-   0        0        0     3068 2022-04-05 01:36:55.000000 protocol-implements-decorator-0.5/protocol_implements_decorator/implements.py
-drwxrwxrwx   0        0        0        0 2022-04-05 02:32:10.482350 protocol-implements-decorator-0.5/protocol_implements_decorator.egg-info/
--rw-rw-rw-   0        0        0      707 2022-04-05 02:32:10.000000 protocol-implements-decorator-0.5/protocol_implements_decorator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2022-04-05 02:32:10.000000 protocol-implements-decorator-0.5/protocol_implements_decorator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-05 02:32:10.000000 protocol-implements-decorator-0.5/protocol_implements_decorator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2022-04-05 02:32:10.000000 protocol-implements-decorator-0.5/protocol_implements_decorator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      409 2022-04-05 01:44:43.000000 protocol-implements-decorator-0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-04-05 02:32:10.482350 protocol-implements-decorator-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1045 2022-04-05 02:32:06.000000 protocol-implements-decorator-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.572164 protocol_implements_decorator-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.564164 protocol_implements_decorator-1.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/dapperdata.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/gh_pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/tomlsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.github/workflows/tox.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-23 03:15:27.572164 protocol_implements_decorator-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-23 03:15:27.000000 protocol_implements_decorator-1.1.2/Protocol_Implements_Decorator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/check_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/create.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.560164 protocol_implements_decorator-1.1.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/docs/source/protocolimplementsdecorator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 03:15:27.572164 protocol_implements_decorator-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.560164 protocol_implements_decorator-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/implements.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/src/protocolimplementsdecorator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 03:15:27.568164 protocol_implements_decorator-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-23 03:15:23.000000 protocol_implements_decorator-1.1.2/tests/test_protocolimplementsdecorator.py
```

### Comparing `protocol-implements-decorator-0.5/README.md` & `protocol_implements_decorator-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,24 @@
 Adds the "implements" decorator to make using protocols easier and more explicit
 
 
 ## Description
 
 Adds the @implements decorator.
 This will cause a runtime NotImplementedError if the class does not implement all parts of the protocol.
-Also adds the get_protocols_implemented method to the class providing a list of all protocols the decorated class adheres to.
-
-Correct and update type hinting.
+Also adds the get_protocols_implemented method to the class providing a list of all protocols the decorated class adhears to.
 
 Usage:
 ---
 Two example protocols
 
 ```python
 class Printable(Protocol):
   """A test protocol that requires a to_string method."""
-  
+
   def to_string(self) -> str:
     return ""
 
 class Otherable(Protocol):
   """Another example."""
 
   def other(self) -> str:
@@ -36,15 +34,15 @@
 @implements(Printable)
 class Example2:
 
   def to_string(self) -> str:
     return str(self)
 ```
 
-For multiple protocols you can chain decorator or include in a list in one decorator
+For multiple protocols you can chain dectorator or include in a list in one dectorator
 ```python
 @implements(Printable)
 @implements(Otherable)
 class Example1:
   """Test class that uses multiple protocols."""
 
   def to_string(self) -> str:
@@ -74,15 +72,15 @@
 class Example2:
   """Test class that uses multiple protocols."""
 
   def other(self) -> str:
     return str(self)
 ```
 ```text
-NotImplementedError: test.<locals>.Printable requires implementation of ['to_string']
+NotImplementedError: test.<locals>.Printable requires implentation of ['to_string']
 ```
 
 
 
 <!-- pyscaffold-notes -->
 
 ## Note
```

