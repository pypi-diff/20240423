# Comparing `tmp/shinyswatch-0.6.0.tar.gz` & `tmp/shinyswatch-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinyswatch-0.6.0.tar", last modified: Tue Apr 16 15:28:50 2024, max compression
+gzip compressed data, was "shinyswatch-0.6.1.tar", last modified: Tue Apr 23 17:13:09 2024, max compression
```

## Comparing `shinyswatch-0.6.0.tar` & `shinyswatch-0.6.1.tar`

### file list

```diff
@@ -1,108 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.597578 shinyswatch-0.6.0/shinyswatch/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/_assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/_bsw5.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/_get_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/_get_theme_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/_theme_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/_theme_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/_typing_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.597578 shinyswatch-0.6.0/shinyswatch/bs5/
--rw-r--r--   0 runner    (1001) docker     (127)    80668 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bs5/bootstrap.bundle.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.593578 shinyswatch-0.6.0/shinyswatch/bsw5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.601578 shinyswatch-0.6.0/shinyswatch/bsw5/cerulean/
--rw-r--r--   0 runner    (1001) docker     (127)   304343 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/cerulean/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/cerulean/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.601578 shinyswatch-0.6.0/shinyswatch/bsw5/cosmo/
--rw-r--r--   0 runner    (1001) docker     (127)   290992 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/cosmo/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/cosmo/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.601578 shinyswatch-0.6.0/shinyswatch/bsw5/cyborg/
--rw-r--r--   0 runner    (1001) docker     (127)   301666 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/cyborg/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/cyborg/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.601578 shinyswatch-0.6.0/shinyswatch/bsw5/darkly/
--rw-r--r--   0 runner    (1001) docker     (127)   307287 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/darkly/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/darkly/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.601578 shinyswatch-0.6.0/shinyswatch/bsw5/flatly/
--rw-r--r--   0 runner    (1001) docker     (127)   304101 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/flatly/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/flatly/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.601578 shinyswatch-0.6.0/shinyswatch/bsw5/journal/
--rw-r--r--   0 runner    (1001) docker     (127)   301436 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/journal/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/journal/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.605578 shinyswatch-0.6.0/shinyswatch/bsw5/litera/
--rw-r--r--   0 runner    (1001) docker     (127)   303337 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/litera/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/litera/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.605578 shinyswatch-0.6.0/shinyswatch/bsw5/lumen/
--rw-r--r--   0 runner    (1001) docker     (127)   308712 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/lumen/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/lumen/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.605578 shinyswatch-0.6.0/shinyswatch/bsw5/lux/
--rw-r--r--   0 runner    (1001) docker     (127)   292631 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/lux/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/lux/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.605578 shinyswatch-0.6.0/shinyswatch/bsw5/materia/
--rw-r--r--   0 runner    (1001) docker     (127)   329378 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/materia/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/materia/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.605578 shinyswatch-0.6.0/shinyswatch/bsw5/minty/
--rw-r--r--   0 runner    (1001) docker     (127)   302933 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/minty/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/minty/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.609578 shinyswatch-0.6.0/shinyswatch/bsw5/morph/
--rw-r--r--   0 runner    (1001) docker     (127)   327531 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/morph/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/morph/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.609578 shinyswatch-0.6.0/shinyswatch/bsw5/pulse/
--rw-r--r--   0 runner    (1001) docker     (127)   293885 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/pulse/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/pulse/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.609578 shinyswatch-0.6.0/shinyswatch/bsw5/quartz/
--rw-r--r--   0 runner    (1001) docker     (127)   339037 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/quartz/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/quartz/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.609578 shinyswatch-0.6.0/shinyswatch/bsw5/sandstone/
--rw-r--r--   0 runner    (1001) docker     (127)   304166 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/sandstone/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/sandstone/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.609578 shinyswatch-0.6.0/shinyswatch/bsw5/simplex/
--rw-r--r--   0 runner    (1001) docker     (127)   304471 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/simplex/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/simplex/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.613578 shinyswatch-0.6.0/shinyswatch/bsw5/sketchy/
--rw-r--r--   0 runner    (1001) docker     (127)   309210 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/sketchy/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/sketchy/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.613578 shinyswatch-0.6.0/shinyswatch/bsw5/slate/
--rw-r--r--   0 runner    (1001) docker     (127)   322088 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/slate/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/slate/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.613578 shinyswatch-0.6.0/shinyswatch/bsw5/solar/
--rw-r--r--   0 runner    (1001) docker     (127)   301875 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/solar/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/solar/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.613578 shinyswatch-0.6.0/shinyswatch/bsw5/spacelab/
--rw-r--r--   0 runner    (1001) docker     (127)   306108 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/spacelab/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/spacelab/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.613578 shinyswatch-0.6.0/shinyswatch/bsw5/superhero/
--rw-r--r--   0 runner    (1001) docker     (127)   301855 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/superhero/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/superhero/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.613578 shinyswatch-0.6.0/shinyswatch/bsw5/united/
--rw-r--r--   0 runner    (1001) docker     (127)   301317 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/united/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/united/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/shinyswatch/bsw5/vapor/
--rw-r--r--   0 runner    (1001) docker     (127)   319597 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/vapor/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/vapor/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/shinyswatch/bsw5/yeti/
--rw-r--r--   0 runner    (1001) docker     (127)   309218 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/yeti/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/yeti/shinyswatch-ionRangeSlider.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/shinyswatch/bsw5/zephyr/
--rw-r--r--   0 runner    (1001) docker     (127)   309516 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/zephyr/bootswatch.min.css
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/bsw5/zephyr/shinyswatch-ionRangeSlider.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/shinyswatch/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.597578 shinyswatch-0.6.0/shinyswatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-16 15:28:50.000000 shinyswatch-0.6.0/shinyswatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-16 15:28:50.000000 shinyswatch-0.6.0/shinyswatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:28:50.000000 shinyswatch-0.6.0/shinyswatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:28:50.000000 shinyswatch-0.6.0/shinyswatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-16 15:28:50.000000 shinyswatch-0.6.0/shinyswatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 15:28:50.000000 shinyswatch-0.6.0/shinyswatch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:28:50.617578 shinyswatch-0.6.0/tests/bug_0025/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/tests/bug_0025/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-16 15:28:19.000000 shinyswatch-0.6.0/tests/test_themes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.154877 shinyswatch-0.6.1/shinyswatch/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/_bsw5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/_get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/_get_theme_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/_theme_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/_theme_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/_typing_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.154877 shinyswatch-0.6.1/shinyswatch/bs5/
+-rw-r--r--   0 runner    (1001) docker     (127)    80668 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bs5/bootstrap.bundle.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.150877 shinyswatch-0.6.1/shinyswatch/bsw5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.158877 shinyswatch-0.6.1/shinyswatch/bsw5/cerulean/
+-rw-r--r--   0 runner    (1001) docker     (127)   304343 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/cerulean/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/cerulean/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.158877 shinyswatch-0.6.1/shinyswatch/bsw5/cosmo/
+-rw-r--r--   0 runner    (1001) docker     (127)   290992 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/cosmo/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/cosmo/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.158877 shinyswatch-0.6.1/shinyswatch/bsw5/cyborg/
+-rw-r--r--   0 runner    (1001) docker     (127)   301666 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/cyborg/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/cyborg/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.158877 shinyswatch-0.6.1/shinyswatch/bsw5/darkly/
+-rw-r--r--   0 runner    (1001) docker     (127)   307287 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/darkly/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/darkly/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.158877 shinyswatch-0.6.1/shinyswatch/bsw5/flatly/
+-rw-r--r--   0 runner    (1001) docker     (127)   304101 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/flatly/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/flatly/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.162877 shinyswatch-0.6.1/shinyswatch/bsw5/journal/
+-rw-r--r--   0 runner    (1001) docker     (127)   301436 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/journal/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/journal/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.162877 shinyswatch-0.6.1/shinyswatch/bsw5/litera/
+-rw-r--r--   0 runner    (1001) docker     (127)   303337 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/litera/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/litera/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.162877 shinyswatch-0.6.1/shinyswatch/bsw5/lumen/
+-rw-r--r--   0 runner    (1001) docker     (127)   308712 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/lumen/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/lumen/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.162877 shinyswatch-0.6.1/shinyswatch/bsw5/lux/
+-rw-r--r--   0 runner    (1001) docker     (127)   292631 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/lux/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/lux/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.162877 shinyswatch-0.6.1/shinyswatch/bsw5/materia/
+-rw-r--r--   0 runner    (1001) docker     (127)   329378 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/materia/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/materia/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.162877 shinyswatch-0.6.1/shinyswatch/bsw5/minty/
+-rw-r--r--   0 runner    (1001) docker     (127)   302933 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/minty/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/minty/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.166877 shinyswatch-0.6.1/shinyswatch/bsw5/morph/
+-rw-r--r--   0 runner    (1001) docker     (127)   327531 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/morph/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/morph/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.166877 shinyswatch-0.6.1/shinyswatch/bsw5/pulse/
+-rw-r--r--   0 runner    (1001) docker     (127)   293885 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/pulse/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/pulse/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.166877 shinyswatch-0.6.1/shinyswatch/bsw5/quartz/
+-rw-r--r--   0 runner    (1001) docker     (127)   339037 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/quartz/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/quartz/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.166877 shinyswatch-0.6.1/shinyswatch/bsw5/sandstone/
+-rw-r--r--   0 runner    (1001) docker     (127)   304166 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/sandstone/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/sandstone/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.166877 shinyswatch-0.6.1/shinyswatch/bsw5/simplex/
+-rw-r--r--   0 runner    (1001) docker     (127)   304471 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/simplex/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/simplex/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.170877 shinyswatch-0.6.1/shinyswatch/bsw5/sketchy/
+-rw-r--r--   0 runner    (1001) docker     (127)   309210 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/sketchy/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/sketchy/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.170877 shinyswatch-0.6.1/shinyswatch/bsw5/slate/
+-rw-r--r--   0 runner    (1001) docker     (127)   322088 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/slate/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/slate/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.170877 shinyswatch-0.6.1/shinyswatch/bsw5/solar/
+-rw-r--r--   0 runner    (1001) docker     (127)   301875 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/solar/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/solar/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.170877 shinyswatch-0.6.1/shinyswatch/bsw5/spacelab/
+-rw-r--r--   0 runner    (1001) docker     (127)   306108 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/spacelab/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/spacelab/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.170877 shinyswatch-0.6.1/shinyswatch/bsw5/superhero/
+-rw-r--r--   0 runner    (1001) docker     (127)   301855 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/superhero/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/superhero/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.170877 shinyswatch-0.6.1/shinyswatch/bsw5/united/
+-rw-r--r--   0 runner    (1001) docker     (127)   301317 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/united/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/united/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/shinyswatch/bsw5/vapor/
+-rw-r--r--   0 runner    (1001) docker     (127)   319597 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/vapor/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/vapor/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/shinyswatch/bsw5/yeti/
+-rw-r--r--   0 runner    (1001) docker     (127)   309218 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/yeti/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/yeti/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/shinyswatch/bsw5/zephyr/
+-rw-r--r--   0 runner    (1001) docker     (127)   309516 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/zephyr/bootswatch.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/bsw5/zephyr/shinyswatch-ionRangeSlider.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/shinyswatch/picker/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/picker/theme_picker.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/picker/theme_picker.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11629 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/shinyswatch/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.154877 shinyswatch-0.6.1/shinyswatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-23 17:13:09.000000 shinyswatch-0.6.1/shinyswatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-23 17:13:09.000000 shinyswatch-0.6.1/shinyswatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:13:09.000000 shinyswatch-0.6.1/shinyswatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 17:13:09.000000 shinyswatch-0.6.1/shinyswatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-23 17:13:09.000000 shinyswatch-0.6.1/shinyswatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 17:13:09.000000 shinyswatch-0.6.1/shinyswatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 17:13:09.174877 shinyswatch-0.6.1/tests/bug_0025/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/tests/bug_0025/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-23 17:12:15.000000 shinyswatch-0.6.1/tests/test_themes.py
```

### Comparing `shinyswatch-0.6.0/LICENSE` & `shinyswatch-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/PKG-INFO` & `shinyswatch-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.6.0
+Version: 0.6.1
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
 Home-page: https://github.com/rstudio/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinyswatch/issues
 Project-URL: Source Code, https://github.com/rstudio/py-shinyswatch
 Keywords: html
```

### Comparing `shinyswatch-0.6.0/README.md` & `shinyswatch-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/setup.cfg` & `shinyswatch-0.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/_bsw5.py` & `shinyswatch-0.6.1/shinyswatch/_bsw5.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/_get_theme_deps.py` & `shinyswatch-0.6.1/shinyswatch/_get_theme_deps.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/_theme_picker.py` & `shinyswatch-0.6.1/shinyswatch/_theme_picker.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/_theme_utils.py` & `shinyswatch-0.6.1/shinyswatch/_theme_utils.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/_typing_extensions.py` & `shinyswatch-0.6.1/shinyswatch/_typing_extensions.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bs5/bootstrap.bundle.min.js` & `shinyswatch-0.6.1/shinyswatch/bs5/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/cerulean/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/cerulean/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/cerulean/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/cerulean/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/cosmo/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/cosmo/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/cosmo/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/cosmo/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/cyborg/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/cyborg/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/cyborg/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/cyborg/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/darkly/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/darkly/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/darkly/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/darkly/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/flatly/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/flatly/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/flatly/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/flatly/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/journal/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/journal/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/journal/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/journal/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/litera/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/litera/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/litera/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/litera/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/lumen/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/lumen/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/lumen/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/lumen/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/lux/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/lux/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/lux/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/lux/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/materia/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/materia/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/materia/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/materia/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/minty/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/minty/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/minty/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/minty/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/morph/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/morph/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/morph/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/morph/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/pulse/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/pulse/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/pulse/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/pulse/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/quartz/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/quartz/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/quartz/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/quartz/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/sandstone/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/sandstone/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/sandstone/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/sandstone/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/simplex/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/simplex/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/simplex/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/simplex/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/sketchy/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/sketchy/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/sketchy/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/sketchy/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/slate/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/slate/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/slate/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/slate/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/solar/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/solar/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/solar/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/solar/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/spacelab/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/spacelab/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/spacelab/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/spacelab/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/superhero/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/superhero/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/superhero/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/superhero/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/united/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/united/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/united/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/united/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/vapor/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/vapor/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/vapor/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/vapor/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/yeti/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/yeti/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/yeti/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/yeti/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/zephyr/bootswatch.min.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/zephyr/bootswatch.min.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/bsw5/zephyr/shinyswatch-ionRangeSlider.css` & `shinyswatch-0.6.1/shinyswatch/bsw5/zephyr/shinyswatch-ionRangeSlider.css`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch/theme.py` & `shinyswatch-0.6.1/shinyswatch/theme.py`

 * *Files identical despite different names*

### Comparing `shinyswatch-0.6.0/shinyswatch.egg-info/PKG-INFO` & `shinyswatch-0.6.1/shinyswatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinyswatch
-Version: 0.6.0
+Version: 0.6.1
 Summary: Bootswatch + Bootstrap 5 themes for Shiny.
 Home-page: https://github.com/rstudio/py-shinyswatch
 Author: Barret Schloerke
 Author-email: barret@posit.co
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinyswatch/issues
 Project-URL: Source Code, https://github.com/rstudio/py-shinyswatch
 Keywords: html
```

### Comparing `shinyswatch-0.6.0/shinyswatch.egg-info/SOURCES.txt` & `shinyswatch-0.6.1/shinyswatch.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -66,10 +66,12 @@
 shinyswatch/bsw5/united/shinyswatch-ionRangeSlider.css
 shinyswatch/bsw5/vapor/bootswatch.min.css
 shinyswatch/bsw5/vapor/shinyswatch-ionRangeSlider.css
 shinyswatch/bsw5/yeti/bootswatch.min.css
 shinyswatch/bsw5/yeti/shinyswatch-ionRangeSlider.css
 shinyswatch/bsw5/zephyr/bootswatch.min.css
 shinyswatch/bsw5/zephyr/shinyswatch-ionRangeSlider.css
+shinyswatch/picker/theme_picker.css
+shinyswatch/picker/theme_picker.js
 tests/__init__.py
 tests/test_themes.py
 tests/bug_0025/app.py
```

### Comparing `shinyswatch-0.6.0/tests/test_themes.py` & `shinyswatch-0.6.1/tests/test_themes.py`

 * *Files identical despite different names*

