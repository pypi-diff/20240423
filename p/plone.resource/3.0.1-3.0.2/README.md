# Comparing `tmp/plone.resource-3.0.1.tar.gz` & `tmp/plone_resource-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.resource-3.0.1.tar", last modified: Mon Jan 22 19:53:14 2024, max compression
+gzip compressed data, was "plone_resource-3.0.2.tar", last modified: Tue Apr 23 15:42:20 2024, max compression
```

## Comparing `plone.resource-3.0.1.tar` & `plone_resource-3.0.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.899673 plone.resource-3.0.1/
--rw-r--r--   0 maurits    (501) staff       (20)     4605 2024-01-22 19:53:14.000000 plone.resource-3.0.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2024-01-22 19:53:14.000000 plone.resource-3.0.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2024-01-22 19:53:14.000000 plone.resource-3.0.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    10730 2024-01-22 19:53:14.899242 plone.resource-3.0.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4900 2024-01-22 19:53:14.000000 plone.resource-3.0.1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      279 2024-01-22 19:53:14.000000 plone.resource-3.0.1/TODO.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.881712 plone.resource-3.0.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2024-01-22 19:53:14.000000 plone.resource-3.0.1/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      729 2024-01-22 19:53:14.000000 plone.resource-3.0.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.881985 plone.resource-3.0.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.891123 plone.resource-3.0.1/plone/resource/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      596 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/browser.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      584 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/caching.py
--rw-r--r--   0 maurits    (501) staff       (20)      446 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/caching.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      303 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9151 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/directory.py
--rw-r--r--   0 maurits    (501) staff       (20)      777 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/download.py
--rw-r--r--   0 maurits    (501) staff       (20)      477 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/events.py
--rw-r--r--   0 maurits    (501) staff       (20)     2597 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/file.py
--rw-r--r--   0 maurits    (501) staff       (20)      189 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/file.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3133 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     8659 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/manifest.py
--rw-r--r--   0 maurits    (501) staff       (20)      321 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      205 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.877765 plone.resource-3.0.1/plone/resource/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.892284 plone.resource-3.0.1/plone/resource/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      308 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)       85 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      234 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/profiles/default/rolemap.xml
--rw-r--r--   0 maurits    (501) staff       (20)      178 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/profiles/default/toolset.xml
--rw-r--r--   0 maurits    (501) staff       (20)      472 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/profiles.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1793 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/testing.py
--rw-r--r--   0 maurits    (501) staff       (20)      393 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/testing.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.895561 plone.resource-3.0.1/plone/resource/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.878209 plone.resource-3.0.1/plone/resource/tests/resources/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.878482 plone.resource-3.0.1/plone/resource/tests/resources/demo/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.895838 plone.resource-3.0.1/plone/resource/tests/resources/demo/foo/
--rw-r--r--   0 maurits    (501) staff       (20)        4 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/resources/demo/foo/test.html
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.896440 plone.resource-3.0.1/plone/resource/tests/resources/demo/manifest-test/
--rw-r--r--   0 maurits    (501) staff       (20)       85 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/resources/demo/manifest-test/manifest.cfg
--rw-r--r--   0 maurits    (501) staff       (20)        9 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/resources/demo/manifest-test/test.txt
--rw-r--r--   0 maurits    (501) staff       (20)      912 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/resources.zip
--rw-r--r--   0 maurits    (501) staff       (20)    10453 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_directory.py
--rw-r--r--   0 maurits    (501) staff       (20)     2189 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_file.py
--rw-r--r--   0 maurits    (501) staff       (20)      980 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_integration.py
--rw-r--r--   0 maurits    (501) staff       (20)     9542 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_manifest.py
--rw-r--r--   0 maurits    (501) staff       (20)     4158 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     4096 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     3306 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_zcml.py
--rw-r--r--   0 maurits    (501) staff       (20)     2892 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/test_zip_download.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.897994 plone.resource-3.0.1/plone/resource/tests/zipfiles/
--rw-r--r--   0 maurits    (501) staff       (20)      524 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/zipfiles/manifest-name-override.zip
--rw-r--r--   0 maurits    (501) staff       (20)     1002 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip
--rw-r--r--   0 maurits    (501) staff       (20)      316 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/zipfiles/no-manifest.zip
--rw-r--r--   0 maurits    (501) staff       (20)      348 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/zipfiles/no-top-level-dir.zip
--rw-r--r--   0 maurits    (501) staff       (20)      512 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/tests/zipfiles/normal.zip
--rw-r--r--   0 maurits    (501) staff       (20)     1019 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/traversal.py
--rw-r--r--   0 maurits    (501) staff       (20)     3442 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     2693 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone/resource/zcml.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-01-22 19:53:14.898335 plone.resource-3.0.1/plone.resource.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    10730 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1970 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      159 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-01-22 19:53:14.000000 plone.resource-3.0.1/plone.resource.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4230 2024-01-22 19:53:14.000000 plone.resource-3.0.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-01-22 19:53:14.899759 plone.resource-3.0.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1737 2024-01-22 19:53:14.000000 plone.resource-3.0.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.604147 plone_resource-3.0.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     4717 2024-04-23 15:42:19.000000 plone_resource-3.0.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-23 15:42:19.000000 plone_resource-3.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2024-04-23 15:42:19.000000 plone_resource-3.0.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    10842 2024-04-23 15:42:20.603656 plone_resource-3.0.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4900 2024-04-23 15:42:19.000000 plone_resource-3.0.2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      279 2024-04-23 15:42:19.000000 plone_resource-3.0.2/TODO.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.584181 plone_resource-3.0.2/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2024-04-23 15:42:19.000000 plone_resource-3.0.2/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      729 2024-04-23 15:42:19.000000 plone_resource-3.0.2/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.584610 plone_resource-3.0.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.595507 plone_resource-3.0.2/plone/resource/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      596 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/browser.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      584 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/caching.py
+-rw-r--r--   0 maurits    (501) staff       (20)      446 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/caching.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      303 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9151 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/directory.py
+-rw-r--r--   0 maurits    (501) staff       (20)      777 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/download.py
+-rw-r--r--   0 maurits    (501) staff       (20)      477 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/events.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2597 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      189 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/file.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3133 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8660 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/manifest.py
+-rw-r--r--   0 maurits    (501) staff       (20)      321 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      205 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.579154 plone_resource-3.0.2/plone/resource/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.596665 plone_resource-3.0.2/plone/resource/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      308 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/profiles/default/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/profiles/default/rolemap.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      178 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/profiles/default/toolset.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      465 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/profiles.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1793 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/testing.py
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/testing.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.600063 plone_resource-3.0.2/plone/resource/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.579573 plone_resource-3.0.2/plone/resource/tests/resources/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.579831 plone_resource-3.0.2/plone/resource/tests/resources/demo/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.600354 plone_resource-3.0.2/plone/resource/tests/resources/demo/foo/
+-rw-r--r--   0 maurits    (501) staff       (20)        4 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/resources/demo/foo/test.html
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.600994 plone_resource-3.0.2/plone/resource/tests/resources/demo/manifest-test/
+-rw-r--r--   0 maurits    (501) staff       (20)       85 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/resources/demo/manifest-test/manifest.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/resources/demo/manifest-test/test.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      912 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/resources.zip
+-rw-r--r--   0 maurits    (501) staff       (20)    10453 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_directory.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2189 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_file.py
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_integration.py
+-rw-r--r--   0 maurits    (501) staff       (20)     9542 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_manifest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4158 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4096 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3306 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_zcml.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2892 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/test_zip_download.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.602553 plone_resource-3.0.2/plone/resource/tests/zipfiles/
+-rw-r--r--   0 maurits    (501) staff       (20)      524 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/zipfiles/manifest-name-override.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1002 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      316 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/zipfiles/no-manifest.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      348 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/zipfiles/no-top-level-dir.zip
+-rw-r--r--   0 maurits    (501) staff       (20)      512 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/tests/zipfiles/normal.zip
+-rw-r--r--   0 maurits    (501) staff       (20)     1019 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/traversal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3442 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2687 2024-04-23 15:42:19.000000 plone_resource-3.0.2/plone/resource/zcml.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 15:42:20.602925 plone_resource-3.0.2/plone.resource.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    10842 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1970 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 15:42:20.000000 plone_resource-3.0.2/plone.resource.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4230 2024-04-23 15:42:19.000000 plone_resource-3.0.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-23 15:42:20.604223 plone_resource-3.0.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1737 2024-04-23 15:42:19.000000 plone_resource-3.0.2/setup.py
```

### Comparing `plone.resource-3.0.1/CHANGES.rst` & `plone_resource-3.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Import IPloneSiteRoot from plone.base. @davisagli (#45)
+
+
 3.0.1 (2024-01-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.resource-3.0.1/PKG-INFO` & `plone_resource-3.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.resource
-Version: 3.0.1
+Version: 3.0.2
 Summary: Static files for Plone
 Home-page: https://pypi.org/project/plone.resource
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL version 2 or later
 Keywords: plone resource
 Classifier: Development Status :: 5 - Production/Stable
@@ -183,14 +183,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Import IPloneSiteRoot from plone.base. @davisagli (#45)
+
+
 3.0.1 (2024-01-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.resource-3.0.1/README.rst` & `plone_resource-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/docs/LICENSE.GPL` & `plone_resource-3.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/docs/LICENSE.txt` & `plone_resource-3.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/browser.zcml` & `plone_resource-3.0.2/plone/resource/browser.zcml`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/caching.py` & `plone_resource-3.0.2/plone/resource/caching.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/directory.py` & `plone_resource-3.0.2/plone/resource/directory.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/download.py` & `plone_resource-3.0.2/plone/resource/download.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/file.py` & `plone_resource-3.0.2/plone/resource/file.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/interfaces.py` & `plone_resource-3.0.2/plone/resource/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/manifest.py` & `plone_resource-3.0.2/plone/resource/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     from plone.resource.manifest import getManifest
     manifest = getManifest(fp, FOO_FORMAT)
 
 ``manifest`` will now be a dict with keys ``title``, ``description``, and
 ``bar``. ``title`` and ``description`` will be ``None`` if not found in the
 manifest. ``bar`` will be ``baz`` if not found.
 """
+
 from configparser import ConfigParser
 from plone.resource.directory import FILTERS
 from plone.resource.interfaces import IResourceDirectory
 from plone.resource.utils import iterDirectoriesOfType
 from zope.component import getUtility
 
 import logging
```

### Comparing `plone.resource-3.0.1/plone/resource/testing.py` & `plone_resource-3.0.2/plone/resource/testing.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/resources.zip` & `plone_resource-3.0.2/plone/resource/tests/resources.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_directory.py` & `plone_resource-3.0.2/plone/resource/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_file.py` & `plone_resource-3.0.2/plone/resource/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_integration.py` & `plone_resource-3.0.2/plone/resource/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_manifest.py` & `plone_resource-3.0.2/plone/resource/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_traversal.py` & `plone_resource-3.0.2/plone/resource/tests/test_traversal.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_utils.py` & `plone_resource-3.0.2/plone/resource/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_zcml.py` & `plone_resource-3.0.2/plone/resource/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/test_zip_download.py` & `plone_resource-3.0.2/plone/resource/tests/test_zip_download.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/zipfiles/manifest-name-override.zip` & `plone_resource-3.0.2/plone/resource/tests/zipfiles/manifest-name-override.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip` & `plone_resource-3.0.2/plone/resource/tests/zipfiles/multiple-top-level-dirs.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/tests/zipfiles/normal.zip` & `plone_resource-3.0.2/plone/resource/tests/zipfiles/normal.zip`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/traversal.py` & `plone_resource-3.0.2/plone/resource/traversal.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/utils.py` & `plone_resource-3.0.2/plone/resource/utils.py`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/plone/resource/zcml.py` & `plone_resource-3.0.2/plone/resource/zcml.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,21 +46,21 @@
             "Resource directories in distributions must "
             "be specified as relative paths."
         )
     elif _context.package:
         directory = _context.path(directory)
     elif not _context.package and not os.path.isabs(directory):
         raise ConfigurationError(
-            "Global resource directories must be " "specified as absolute paths."
+            "Global resource directories must be specified as absolute paths."
         )
 
     # TODO: make sure this works in Windows
     if ".." in directory.split("/"):
         raise ConfigurationError(
-            "Traversing to parent directories " "via .. is not allowed."
+            "Traversing to parent directories via .. is not allowed."
         )
     if not os.path.exists(directory):
         raise OSError("Directory not found: %s" % directory)
 
     if name is None and _context.package:
         name = _context.package.__name__
```

### Comparing `plone.resource-3.0.1/plone.resource.egg-info/PKG-INFO` & `plone_resource-3.0.2/plone.resource.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.resource
-Version: 3.0.1
+Version: 3.0.2
 Summary: Static files for Plone
 Home-page: https://pypi.org/project/plone.resource
 Author: David Glick, Plone Foundation
 Author-email: davidglick@groundwire.org
 License: GPL version 2 or later
 Keywords: plone resource
 Classifier: Development Status :: 5 - Production/Stable
@@ -183,14 +183,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.2 (2024-04-23)
+------------------
+
+Bug fixes:
+
+
+- Import IPloneSiteRoot from plone.base. @davisagli (#45)
+
+
 3.0.1 (2024-01-22)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.resource-3.0.1/plone.resource.egg-info/SOURCES.txt` & `plone_resource-3.0.2/plone.resource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/pyproject.toml` & `plone_resource-3.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.resource-3.0.1/setup.py` & `plone_resource-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.1"
+version = "3.0.2"
 
 test_requires = [
     "plone.app.testing",
     "plone.testing",
 ]
 
 long_description = (
```

