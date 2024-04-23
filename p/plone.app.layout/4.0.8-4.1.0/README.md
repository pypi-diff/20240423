# Comparing `tmp/plone.app.layout-4.0.8.tar.gz` & `tmp/plone_app_layout-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.layout-4.0.8.tar", last modified: Fri Dec 22 08:52:04 2023, max compression
+gzip compressed data, was "plone_app_layout-4.1.0.tar", last modified: Tue Apr 23 16:29:30 2024, max compression
```

## Comparing `plone.app.layout-4.0.8.tar` & `plone_app_layout-4.1.0.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:04.000235 plone.app.layout-4.0.8/
--rw-r--r--   0 maurits    (501) staff       (20)    62610 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    65243 2023-12-22 08:52:03.999832 plone.app.layout-4.0.8/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      740 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.960329 plone.app.layout-4.0.8/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      678 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.960732 plone.app.layout-4.0.8/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.963239 plone.app.layout-4.0.8/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.964702 plone.app.layout-4.0.8/plone/app/layout/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.965870 plone.app.layout-4.0.8/plone/app/layout/analytics/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/analytics/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      322 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/analytics/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.966682 plone.app.layout-4.0.8/plone/app/layout/analytics/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/analytics/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1695 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/analytics/tests/analytics.txt
--rw-r--r--   0 maurits    (501) staff       (20)      637 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/analytics/tests/test_doctests.py
--rw-r--r--   0 maurits    (501) staff       (20)      199 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/analytics/view.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1024 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/analytics/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      550 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.967692 plone.app.layout-4.0.8/plone/app/layout/dashboard/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/dashboard/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      100 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/dashboard/dashboard.py
--rw-r--r--   0 maurits    (501) staff       (20)      103 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/dashboard/user_actions.py
--rw-r--r--   0 maurits    (501) staff       (20)      885 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/favicon_handler.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.970651 plone.app.layout-4.0.8/plone/app/layout/globals/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1327 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     9179 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/context.py
--rw-r--r--   0 maurits    (501) staff       (20)     4098 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     6502 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    12280 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     3805 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/portal.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.972520 plone.app.layout-4.0.8/plone/app/layout/globals/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.972833 plone.app.layout-4.0.8/plone/app/layout/globals/tests/data/
--rw-r--r--   0 maurits    (501) staff       (20)       30 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10563 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_context.py
--rw-r--r--   0 maurits    (501) staff       (20)     3885 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_interface.py
--rw-r--r--   0 maurits    (501) staff       (20)     8497 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_layout.py
--rw-r--r--   0 maurits    (501) staff       (20)     6324 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_portal.py
--rw-r--r--   0 maurits    (501) staff       (20)     1375 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_tools.py
--rw-r--r--   0 maurits    (501) staff       (20)     1060 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/globals/tools.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.974120 plone.app.layout-4.0.8/plone/app/layout/icons/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/icons/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1553 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/icons/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5639 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/icons/icons.py
--rw-r--r--   0 maurits    (501) staff       (20)      759 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/icons/interfaces.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.976183 plone.app.layout-4.0.8/plone/app/layout/links/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      523 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/author.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1166 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      284 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/favicon.pt
--rw-r--r--   0 maurits    (501) staff       (20)      178 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/rsslink.pt
--rw-r--r--   0 maurits    (501) staff       (20)      363 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/search.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.977459 plone.app.layout-4.0.8/plone/app/layout/links/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      803 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/tests/test_canonical_url.py
--rw-r--r--   0 maurits    (501) staff       (20)     2707 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/tests/test_favicon_viewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     1402 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/tests/test_rssviewlet.py
--rw-r--r--   0 maurits    (501) staff       (20)     7019 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/links/viewlets.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.979024 plone.app.layout-4.0.8/plone/app/layout/navigation/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/navigation/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/navigation/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1749 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/navigation/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)    14357 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/navigation/navtree.py
--rw-r--r--   0 maurits    (501) staff       (20)      445 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/navigation/root.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.980986 plone.app.layout-4.0.8/plone/app/layout/nextprevious/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/nextprevious/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      989 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/nextprevious/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/nextprevious/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      909 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/nextprevious/links.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1673 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/nextprevious/nextprevious.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1611 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/nextprevious/view.py
--rw-r--r--   0 maurits    (501) staff       (20)      323 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/permissions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.982625 plone.app.layout-4.0.8/plone/app/layout/sitemap/
--rw-r--r--   0 maurits    (501) staff       (20)      159 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/sitemap/README.txt
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/sitemap/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      301 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/sitemap/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4491 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/sitemap/sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)      820 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/sitemap/sitemap.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.983151 plone.app.layout-4.0.8/plone/app/layout/sitemap/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/sitemap/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    11362 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/sitemap/tests/test_sitemap.py
--rw-r--r--   0 maurits    (501) staff       (20)     1184 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.995683 plone.app.layout-4.0.8/plone/app/layout/viewlets/
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      409 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/anontools.pt
--rw-r--r--   0 maurits    (501) staff       (20)      432 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/colophon.pt
--rw-r--r--   0 maurits    (501) staff       (20)    20134 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/common.py
--rw-r--r--   0 maurits    (501) staff       (20)    10329 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)    18951 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/content.py
--rw-r--r--   0 maurits    (501) staff       (20)     6241 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)      750 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/contentviews.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/default_page_warning.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1239 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/document_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1978 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/document_byline.pt
--rw-r--r--   0 maurits    (501) staff       (20)      980 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/document_contributors.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1833 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/document_relateditems.pt
--rw-r--r--   0 maurits    (501) staff       (20)      375 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/document_rights.pt
--rw-r--r--   0 maurits    (501) staff       (20)      139 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/dublin_core.pt
--rw-r--r--   0 maurits    (501) staff       (20)      793 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/globalstatusmessage.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1579 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/globalstatusmessage.py
--rw-r--r--   0 maurits    (501) staff       (20)      620 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/history_view.pt
--rw-r--r--   0 maurits    (501) staff       (20)      953 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/httpheaders.py
--rw-r--r--   0 maurits    (501) staff       (20)     2331 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      920 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/keywords.pt
--rw-r--r--   0 maurits    (501) staff       (20)      361 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1318 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/membertools.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1816 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/menu.pt
--rw-r--r--   0 maurits    (501) staff       (20)      805 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/path_bar.pt
--rw-r--r--   0 maurits    (501) staff       (20)      515 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/popup_content_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     3320 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/review_history.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1621 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/searchbox.pt
--rw-r--r--   0 maurits    (501) staff       (20)      661 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/sections.pt
--rw-r--r--   0 maurits    (501) staff       (20)      552 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/site_actions.pt
--rw-r--r--   0 maurits    (501) staff       (20)     5451 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/social.py
--rw-r--r--   0 maurits    (501) staff       (20)       80 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/social_tags.pt
--rw-r--r--   0 maurits    (501) staff       (20)      294 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/social_tags_body.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.998150 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      665 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     2621 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/history.txt
--rw-r--r--   0 maurits    (501) staff       (20)    27962 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_common.py
--rw-r--r--   0 maurits    (501) staff       (20)    14111 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_content.py
--rw-r--r--   0 maurits    (501) staff       (20)      590 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     5391 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_history.py
--rw-r--r--   0 maurits    (501) staff       (20)     5586 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_social.py
--rw-r--r--   0 maurits    (501) staff       (20)      192 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/tiny_logo.pt
--rw-r--r--   0 maurits    (501) staff       (20)       66 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/title.pt
--rw-r--r--   0 maurits    (501) staff       (20)      382 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/toc.pt
--rw-r--r--   0 maurits    (501) staff       (20)     2517 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/toolbar.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1779 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/toolbar.py
--rw-r--r--   0 maurits    (501) staff       (20)       79 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone/app/layout/viewlets/viewport.pt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-22 08:52:03.998503 plone.app.layout-4.0.8/plone.app.layout.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    65243 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone.app.layout.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     4921 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone.app.layout.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone.app.layout.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone.app.layout.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone.app.layout.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      440 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone.app.layout.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/plone.app.layout.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4284 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-12-22 08:52:04.000335 plone.app.layout-4.0.8/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2264 2023-12-22 08:52:03.000000 plone.app.layout-4.0.8/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.822849 plone_app_layout-4.1.0/
+-rw-r--r--   0 maurits    (501) staff       (20)    63007 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    65640 2024-04-23 16:29:30.822420 plone_app_layout-4.1.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      740 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.782891 plone_app_layout-4.1.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      678 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.783185 plone_app_layout-4.1.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.785782 plone_app_layout-4.1.0/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.787436 plone_app_layout-4.1.0/plone/app/layout/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.789005 plone_app_layout-4.1.0/plone/app/layout/analytics/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      519 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.789937 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2945 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/analytics.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      637 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/tests/test_doctests.py
+-rw-r--r--   0 maurits    (501) staff       (20)      199 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1193 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      234 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/analytics/view_head.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      550 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.790780 plone_app_layout-4.1.0/plone/app/layout/dashboard/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/dashboard/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      100 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/dashboard/dashboard.py
+-rw-r--r--   0 maurits    (501) staff       (20)      103 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/dashboard/user_actions.py
+-rw-r--r--   0 maurits    (501) staff       (20)      885 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/favicon_handler.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.793385 plone_app_layout-4.1.0/plone/app/layout/globals/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1327 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     9179 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4098 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6502 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12280 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3805 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/portal.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.795316 plone_app_layout-4.1.0/plone/app/layout/globals/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.795672 plone_app_layout-4.1.0/plone/app/layout/globals/tests/data/
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/data/bodyclass_nametest.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10563 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_context.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3885 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_interface.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8497 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_layout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6324 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_portal.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1375 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_tools.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1060 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/globals/tools.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.796996 plone_app_layout-4.1.0/plone/app/layout/icons/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1553 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5639 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/icons.py
+-rw-r--r--   0 maurits    (501) staff       (20)      759 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/icons/interfaces.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.799051 plone_app_layout-4.1.0/plone/app/layout/links/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      523 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/author.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1166 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      284 2024-04-23 16:29:29.000000 plone_app_layout-4.1.0/plone/app/layout/links/favicon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      178 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/rsslink.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      363 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/search.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.800327 plone_app_layout-4.1.0/plone/app/layout/links/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      803 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/test_canonical_url.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2707 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/test_favicon_viewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1402 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/tests/test_rssviewlet.py
+-rw-r--r--   0 maurits    (501) staff       (20)     7079 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/links/viewlets.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.801965 plone_app_layout-4.1.0/plone/app/layout/navigation/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1749 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14357 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/navtree.py
+-rw-r--r--   0 maurits    (501) staff       (20)      445 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/navigation/root.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.803698 plone_app_layout-4.1.0/plone/app/layout/nextprevious/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      989 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      909 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/links.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1673 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/nextprevious.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1611 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/nextprevious/view.py
+-rw-r--r--   0 maurits    (501) staff       (20)      323 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/permissions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.805206 plone_app_layout-4.1.0/plone/app/layout/sitemap/
+-rw-r--r--   0 maurits    (501) staff       (20)      159 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/README.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      301 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4491 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)      820 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.805802 plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11362 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/test_sitemap.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1184 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.818010 plone_app_layout-4.1.0/plone/app/layout/viewlets/
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      409 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/anontools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      432 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/colophon.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    20134 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10329 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)    19042 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/content.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6241 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      750 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/contentviews.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/default_page_warning.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1239 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2062 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_byline.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      980 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_contributors.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1833 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_relateditems.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      375 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/document_rights.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      139 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/dublin_core.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      793 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1579 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.py
+-rw-r--r--   0 maurits    (501) staff       (20)      620 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/history_view.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      953 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/httpheaders.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2331 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      920 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/keywords.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      361 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1318 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/membertools.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1816 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/menu.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      805 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/path_bar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      515 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/popup_content_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     3320 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/review_history.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1621 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/searchbox.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      661 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/sections.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      552 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/site_actions.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     5451 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/social.py
+-rw-r--r--   0 maurits    (501) staff       (20)       80 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/social_tags.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/social_tags_body.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.820686 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      665 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2621 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/history.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    27962 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_common.py
+-rw-r--r--   0 maurits    (501) staff       (20)    14111 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_content.py
+-rw-r--r--   0 maurits    (501) staff       (20)      590 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5391 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_history.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5586 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_social.py
+-rw-r--r--   0 maurits    (501) staff       (20)      192 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/tiny_logo.pt
+-rw-r--r--   0 maurits    (501) staff       (20)       66 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/title.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      382 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/toc.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     2517 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1779 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.py
+-rw-r--r--   0 maurits    (501) staff       (20)       79 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone/app/layout/viewlets/viewport.pt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:29:30.821146 plone_app_layout-4.1.0/plone.app.layout.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    65640 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     4961 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      440 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/plone.app.layout.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4284 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-23 16:29:30.822927 plone_app_layout-4.1.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2264 2024-04-23 16:29:30.000000 plone_app_layout-4.1.0/setup.py
```

### Comparing `plone.app.layout-4.0.8/CHANGES.rst` & `plone_app_layout-4.1.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2024-04-23)
+------------------
+
+New features:
+
+
+- Add a field ``webstats_head_js`` to the Site controlpanel and render its
+  contents in the head section using ``IHtmlHeadLinks`` viewlet manager.
+  See `issue 3931 <https://github.com/plone/Products.CMFPlone/issues/3931>`_:
+  some javascript needs to be loaded at the bottom of the page, and some in the head section.
+  [jladage] (#3931)
+
+
 4.0.8 (2023-12-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix KeyError `time` when missing workflow variables are added later.
```

### Comparing `plone.app.layout-4.0.8/PKG-INFO` & `plone_app_layout-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.8
+Version: 4.1.0
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -74,14 +74,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2024-04-23)
+------------------
+
+New features:
+
+
+- Add a field ``webstats_head_js`` to the Site controlpanel and render its
+  contents in the head section using ``IHtmlHeadLinks`` viewlet manager.
+  See `issue 3931 <https://github.com/plone/Products.CMFPlone/issues/3931>`_:
+  some javascript needs to be loaded at the bottom of the page, and some in the head section.
+  [jladage] (#3931)
+
+
 4.0.8 (2023-12-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix KeyError `time` when missing workflow variables are added later.
```

### Comparing `plone.app.layout-4.0.8/README.rst` & `plone_app_layout-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/docs/LICENSE.GPL` & `plone_app_layout-4.1.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/docs/LICENSE.txt` & `plone_app_layout-4.1.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/analytics/tests/analytics.txt` & `plone_app_layout-4.1.0/plone/app/layout/analytics/tests/analytics.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 We need a view on the content.
 
     >>> request = layer['request']
     >>> portal = layer['portal']
     >>> from zope.publisher.browser import BrowserView
     >>> view = BrowserView(portal, request)
 
-    >>> from plone.app.layout.viewlets.interfaces import IPortalFooter
+    >>> from plone.app.layout.viewlets.interfaces import IHtmlHead, IPortalFooter
     >>> from Products.Five.viewlet.manager import ViewletManager
     >>> Footer = ViewletManager('left', IPortalFooter)
 
 Now we can instantiate the manager.
 
     >>> manager = Footer(portal, request, view)
     >>> manager.update()
     >>> for viewlet in manager.viewlets:
     ...     if viewlet.__name__ == "plone.analytics":
     ...         analytics = viewlet
     ...         break
 
 When no analytics (webstats_js) code is set up the viewlet will not be rendered:
 
-    >>> analytics.webstats_js == u""
+    >>> analytics.webstats_js == ""
     True
     >>> text = manager.render()
     >>> 'id="plone-analytics"' in text
     False
 
 Set the analytics code through the controlpanel and verify it renders properly:
 
@@ -42,9 +42,43 @@
     >>> site_settings.webstats_js in text
     True
 
 Now enter some non-ascii text
 
     >>> site_settings.webstats_js = u"<script>window.title='C\xedsa\u0159'</script>"
     >>> text = manager.render()
-    >>> site_settings.webstats_js in text
+    >>> "<script>window.title='Císař'</script>" in text
+    True
+
+Now instantiate a viewlet manager for the header.
+
+    >>> Head = ViewletManager('left', IHtmlHead)
+    >>> manager = Head(portal, request, view)
+    >>> manager.update()
+    >>> for viewlet in manager.viewlets:
+    ...     if viewlet.__name__ == "plone.analytics.head":
+    ...         analytics_head = viewlet
+    ...         break
+
+When no analytics (webstats_head_js) code is set up the viewlet will not be rendered:
+
+    >>> analytics_head.webstats_js == ""
+    True
+    >>> text = manager.render()
+    >>> 'plone.analytics.head goes here' in text
+    False
+
+Set the analytics code through the controlpanel and verify it renders properly:
+
+    >>> from plone.registry.interfaces import IRegistry
+    >>> from zope.component import getUtility
+    >>> from plone.base.interfaces import ISiteSchema
+    >>> registry = getUtility(IRegistry)
+    >>> site_settings = registry.forInterface(ISiteSchema, prefix="plone")
+    >>> site_settings.webstats_head_js = u"<script>window.title='Hello'</script>"
+    >>> analytics_head.webstats_js == site_settings.webstats_head_js
+    True
+    >>> text = manager.render()
+    >>> 'plone.analytics.head goes here' in text
+    True
+    >>> site_settings.webstats_head_js in text
     True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,21 +1,36 @@
 We need a view on the content. >>> request = layer['request'] >>> portal =
 layer['portal'] >>> from zope.publisher.browser import BrowserView >>> view =
 BrowserView(portal, request) >>> from plone.app.layout.viewlets.interfaces
-import IPortalFooter >>> from Products.Five.viewlet.manager import
+import IHtmlHead, IPortalFooter >>> from Products.Five.viewlet.manager import
 ViewletManager >>> Footer = ViewletManager('left', IPortalFooter) Now we can
 instantiate the manager. >>> manager = Footer(portal, request, view) >>>
 manager.update() >>> for viewlet in manager.viewlets: ... if viewlet.__name__
 == "plone.analytics": ... analytics = viewlet ... break When no analytics
 (webstats_js) code is set up the viewlet will not be rendered: >>>
-analytics.webstats_js == u"" True >>> text = manager.render() >>> 'id="plone-
+analytics.webstats_js == "" True >>> text = manager.render() >>> 'id="plone-
 analytics"' in text False Set the analytics code through the controlpanel and
 verify it renders properly: >>> from plone.registry.interfaces import IRegistry
 >>> from zope.component import getUtility >>> from plone.base.interfaces import
 ISiteSchema >>> registry = getUtility(IRegistry) >>> site_settings =
 registry.forInterface(ISiteSchema, prefix="plone") >>>
 site_settings.webstats_js = u"
 " >>> analytics.webstats_js == site_settings.webstats_js True >>> text =
 manager.render() >>> 'id="plone-analytics"' in text True >>>
 site_settings.webstats_js in text True Now enter some non-ascii text >>>
 site_settings.webstats_js = u"
-" >>> text = manager.render() >>> site_settings.webstats_js in text True
+" >>> text = manager.render() >>> "
+" in text True Now instantiate a viewlet manager for the header. >>> Head =
+ViewletManager('left', IHtmlHead) >>> manager = Head(portal, request, view) >>>
+manager.update() >>> for viewlet in manager.viewlets: ... if viewlet.__name__
+== "plone.analytics.head": ... analytics_head = viewlet ... break When no
+analytics (webstats_head_js) code is set up the viewlet will not be rendered:
+>>> analytics_head.webstats_js == "" True >>> text = manager.render() >>>
+'plone.analytics.head goes here' in text False Set the analytics code through
+the controlpanel and verify it renders properly: >>> from
+plone.registry.interfaces import IRegistry >>> from zope.component import
+getUtility >>> from plone.base.interfaces import ISiteSchema >>> registry =
+getUtility(IRegistry) >>> site_settings = registry.forInterface(ISiteSchema,
+prefix="plone") >>> site_settings.webstats_head_js = u"
+" >>> analytics_head.webstats_js == site_settings.webstats_head_js True >>>
+text = manager.render() >>> 'plone.analytics.head goes here' in text True >>>
+site_settings.webstats_head_js in text True
```

### Comparing `plone.app.layout-4.0.8/plone/app/layout/analytics/tests/test_doctests.py` & `plone_app_layout-4.1.0/plone/app/layout/analytics/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/analytics/view.py` & `plone_app_layout-4.1.0/plone/app/layout/analytics/view.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,36 @@
 from Products.Five.browser import BrowserView
 from Products.Five.browser.pagetemplatefile import ViewPageTemplateFile
 from zope.component import getUtility
 from zope.interface import implementer
 from zope.viewlet.interfaces import IViewlet
 
 
+UNWANTED_TAGS = ["base", "title"]
+
+
 @implementer(IViewlet)
 class AnalyticsViewlet(BrowserView):
     render = ViewPageTemplateFile("view.pt")
+    record_name = "webstats_js"
 
     def __init__(self, context, request, view, manager):
         super().__init__(context, request)
         self.__parent__ = view
         self.view = view
         self.manager = manager
 
     @property
     def webstats_js(self):
         registry = getUtility(IRegistry)
         site_settings = registry.forInterface(ISiteSchema, prefix="plone", check=False)
-        try:
-            return site_settings.webstats_js or ""
-        except AttributeError:
-            return ""
+        return getattr(site_settings, self.record_name, "")
 
     def update(self):
         """The viewlet manager _updateViewlets requires this method"""
         pass
+
+
+@implementer(IViewlet)
+class AnalyticsHeadViewlet(AnalyticsViewlet):
+    render = ViewPageTemplateFile("view_head.pt")
+    record_name = "webstats_head_js"
```

### Comparing `plone.app.layout-4.0.8/plone/app/layout/configure.zcml` & `plone_app_layout-4.1.0/plone/app/layout/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/favicon_handler.py` & `plone_app_layout-4.1.0/plone/app/layout/favicon_handler.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/configure.zcml` & `plone_app_layout-4.1.0/plone/app/layout/globals/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/context.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/context.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/interface.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/interface.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/interfaces.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/layout.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/portal.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/portal.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_context.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_interface.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_layout.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_portal.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_portal.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/tests/test_tools.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/globals/tools.py` & `plone_app_layout-4.1.0/plone/app/layout/globals/tools.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/icons/configure.zcml` & `plone_app_layout-4.1.0/plone/app/layout/icons/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/icons/icons.py` & `plone_app_layout-4.1.0/plone/app/layout/icons/icons.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/icons/interfaces.py` & `plone_app_layout-4.1.0/plone/app/layout/icons/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/links/author.pt` & `plone_app_layout-4.1.0/plone/app/layout/links/author.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/links/configure.zcml` & `plone_app_layout-4.1.0/plone/app/layout/links/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/links/tests/test_canonical_url.py` & `plone_app_layout-4.1.0/plone/app/layout/links/tests/test_canonical_url.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/links/tests/test_favicon_viewlet.py` & `plone_app_layout-4.1.0/plone/app/layout/links/tests/test_favicon_viewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/links/tests/test_rssviewlet.py` & `plone_app_layout-4.1.0/plone/app/layout/links/tests/test_rssviewlet.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/links/viewlets.py` & `plone_app_layout-4.1.0/plone/app/layout/links/viewlets.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,19 @@
 class FaviconViewlet(ViewletBase):
     _template = ViewPageTemplateFile("favicon.pt")
     mimetype: str
     favicon_path: str
 
     def init_favicon(self) -> NoReturn:
         registry = getUtility(IRegistry)
-        settings: ISiteSchema = registry.forInterface(ISiteSchema, prefix="plone")
+        settings: ISiteSchema = registry.forInterface(
+            ISiteSchema,
+            prefix="plone",
+            check=False,
+        )
         self.mimetype: str = getattr(
             settings, "site_favicon_mimetype", "image/vnd.microsoft.icon"
         )
         cachebust = ""
         if getattr(settings, "site_favicon", False):
             # The user has customized the favicon via the Site configlet.
             filename = b64decode_file(settings.site_favicon)[0]
```

### Comparing `plone.app.layout-4.0.8/plone/app/layout/navigation/interfaces.py` & `plone_app_layout-4.1.0/plone/app/layout/navigation/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/navigation/navtree.py` & `plone_app_layout-4.1.0/plone/app/layout/navigation/navtree.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/nextprevious/configure.zcml` & `plone_app_layout-4.1.0/plone/app/layout/nextprevious/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/nextprevious/links.pt` & `plone_app_layout-4.1.0/plone/app/layout/nextprevious/links.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/nextprevious/nextprevious.pt` & `plone_app_layout-4.1.0/plone/app/layout/nextprevious/nextprevious.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/nextprevious/view.py` & `plone_app_layout-4.1.0/plone/app/layout/nextprevious/view.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/sitemap/sitemap.py` & `plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/sitemap/sitemap.xml` & `plone_app_layout-4.1.0/plone/app/layout/sitemap/sitemap.xml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/sitemap/tests/test_sitemap.py` & `plone_app_layout-4.1.0/plone/app/layout/sitemap/tests/test_sitemap.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/testing.py` & `plone_app_layout-4.1.0/plone/app/layout/testing.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/common.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/common.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/configure.zcml` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/content.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         return getToolByName(self.context, "portal_membership")
 
     def show(self):
         registry = getUtility(IRegistry)
         settings = registry.forInterface(
             ISiteSchema,
             prefix="plone",
+            check=False,
         )
         return not self.anonymous or settings.display_publication_date_in_byline
 
     def show_about(self):
         registry = getUtility(IRegistry)
         settings = registry.forInterface(
             ISecuritySchema,
@@ -141,15 +142,15 @@
         """Return object effective date.
 
         Return None if publication date is switched off in global site settings
         or if Effective Date is not set on object.
         """
         # check if we are allowed to display publication date
         registry = getUtility(IRegistry)
-        settings = registry.forInterface(ISiteSchema, prefix="plone")
+        settings = registry.forInterface(ISiteSchema, prefix="plone", check=False)
 
         if not settings.display_publication_date_in_byline:
             return None
 
         # check if we have Effective Date set
         date = self.context.EffectiveDate()
         if not date or date == "None":
@@ -277,15 +278,15 @@
         """Return object effective date.
 
         Return None if publication date is switched off in global site settings
         or if Effective Date is not set on object.
         """
         # check if we are allowed to display publication date
         registry = getUtility(IRegistry)
-        settings = registry.forInterface(ISiteSchema, prefix="plone")
+        settings = registry.forInterface(ISiteSchema, prefix="plone", check=False)
 
         if not settings.display_publication_date_in_byline:
             return None
 
         # check if we have Effective Date set
         date = self.context.EffectiveDate()
         if not date or date == "None":
@@ -474,29 +475,29 @@
                 time=meta["timestamp"],
                 comments=meta["comment"],
                 version_id=version_id,
                 preview_url=preview_url,
             )
             if can_diff:
                 if version_id > 0:
-                    info[
-                        "diff_previous_url"
-                    ] = "{}/@@history?one={}&two={}&_authenticator={}".format(
-                        context_url,
-                        version_id,
-                        version_id - 1,
-                        token,
+                    info["diff_previous_url"] = (
+                        "{}/@@history?one={}&two={}&_authenticator={}".format(
+                            context_url,
+                            version_id,
+                            version_id - 1,
+                            token,
+                        )
                     )
                 if not rt.isUpToDate(context, version_id):
-                    info[
-                        "diff_current_url"
-                    ] = "{}/@@history?one=current&two={}&_authenticator={}".format(
-                        context_url,
-                        version_id,
-                        token,
+                    info["diff_current_url"] = (
+                        "{}/@@history?one=current&two={}&_authenticator={}".format(
+                            context_url,
+                            version_id,
+                            token,
+                        )
                     )
             if can_revert:
                 info["revert_url"] = "%s/revertversion" % context_url
             else:
                 info["revert_url"] = None
             info.update(self.getUserInfo(userid))
             return info
```

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/content_history.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/content_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/contentviews.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/contentviews.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/default_page_warning.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/default_page_warning.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/document_actions.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/document_byline.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_byline.pt`

 * *Files 5% similar despite different names*

```diff
@@ -4,42 +4,45 @@
 >
   <tal:creators tal:define="
                   creator_ids here/creators;
                   navigation_root_url context/@@plone_portal_state/navigation_root_url;
                 "
                 tal:condition="python:creator_ids and view.show_about()"
   >
-    <tal:i18n i18n:translate="">by</tal:i18n>
-    <tal:for repeat="user_id creator_ids">
-      <tal:user define="
-                  url_path python: view.get_url_path(user_id);
-                  fullname python:view.get_fullname(user_id);
-                ">
-        <a class="badge rounded-pill bg-light text-dark fw-normal fs-6"
-           href="${navigation_root_url}/${url_path}"
-           tal:condition="url_path"
-        >${fullname}</a>
-        <span class="badge rounded-pill bg-light text-dark fw-normal fs-6"
-              tal:condition="not:url_path"
-        >${fullname}</span>
-      </tal:user>
-    </tal:for>
+    <span class="label-by-author">
+      <tal:i18n i18n:translate="">by</tal:i18n>
+      <tal:for repeat="user_id creator_ids">
+        <tal:user define="
+                    url_path python: view.get_url_path(user_id);
+                    fullname python:view.get_fullname(user_id);
+                  ">
+          <a class="badge rounded-pill bg-light text-dark fw-normal fs-6"
+             href="${navigation_root_url}/${url_path}"
+             tal:condition="url_path"
+          >${fullname}</a>
+          <span class="badge rounded-pill bg-light text-dark fw-normal fs-6"
+                tal:condition="not:url_path"
+          >${fullname}</span>
+        </tal:user>
+      </tal:for>
     &mdash;
+    </span>
   </tal:creators>
 
   <tal:dates define="
                published view/pub_date;
                modified context/ModificationDate;
                show_modification_date python:view.show_modification_date();
              ">
     <span class="documentPublished"
           tal:condition="published"
     >
       <span i18n:translate="box_published">published</span>
-      <span tal:content="python:context.toLocalizedTime(published)">Published</span><tal:sep condition="show_modification_date">,</tal:sep>
+      <span tal:content="python:context.toLocalizedTime(published)">Published</span>
+      <tal:sep condition="show_modification_date">,</tal:sep>
     </span>
 
     <span class="documentModified"
           tal:condition="show_modification_date"
     >
       <span i18n:translate="box_last_modified">
       last modified
```

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/document_contributors.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_contributors.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/document_relateditems.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/document_relateditems.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/globalstatusmessage.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/globalstatusmessage.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/globalstatusmessage.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/history_view.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/history_view.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/httpheaders.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/httpheaders.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/interfaces.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/keywords.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/keywords.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/membertools.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/membertools.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/menu.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/menu.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/path_bar.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/path_bar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/popup_content_history.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/popup_content_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/review_history.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/review_history.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/searchbox.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/searchbox.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/sections.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/sections.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/site_actions.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/site_actions.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/social.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/social.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/base.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/history.txt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/history.txt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_common.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_content.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_functional.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_history.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/tests/test_social.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/tests/test_social.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/toolbar.pt` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.pt`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone/app/layout/viewlets/toolbar.py` & `plone_app_layout-4.1.0/plone/app/layout/viewlets/toolbar.py`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/plone.app.layout.egg-info/PKG-INFO` & `plone_app_layout-4.1.0/plone.app.layout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.layout
-Version: 4.0.8
+Version: 4.1.0
 Summary: Layout mechanisms for Plone
 Home-page: https://pypi.org/project/plone.app.layout
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: plone layout viewlet
 Classifier: Development Status :: 6 - Mature
@@ -74,14 +74,27 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.1.0 (2024-04-23)
+------------------
+
+New features:
+
+
+- Add a field ``webstats_head_js`` to the Site controlpanel and render its
+  contents in the head section using ``IHtmlHeadLinks`` viewlet manager.
+  See `issue 3931 <https://github.com/plone/Products.CMFPlone/issues/3931>`_:
+  some javascript needs to be loaded at the bottom of the page, and some in the head section.
+  [jladage] (#3931)
+
+
 4.0.8 (2023-12-22)
 ------------------
 
 Bug fixes:
 
 
 - Fix KeyError `time` when missing workflow variables are added later.
```

### Comparing `plone.app.layout-4.0.8/plone.app.layout.egg-info/SOURCES.txt` & `plone_app_layout-4.1.0/plone.app.layout.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 plone/app/layout/favicon_handler.py
 plone/app/layout/permissions.zcml
 plone/app/layout/testing.py
 plone/app/layout/analytics/__init__.py
 plone/app/layout/analytics/configure.zcml
 plone/app/layout/analytics/view.pt
 plone/app/layout/analytics/view.py
+plone/app/layout/analytics/view_head.pt
 plone/app/layout/analytics/tests/__init__.py
 plone/app/layout/analytics/tests/analytics.txt
 plone/app/layout/analytics/tests/test_doctests.py
 plone/app/layout/dashboard/__init__.py
 plone/app/layout/dashboard/dashboard.py
 plone/app/layout/dashboard/user_actions.py
 plone/app/layout/globals/__init__.py
```

### Comparing `plone.app.layout-4.0.8/pyproject.toml` & `plone_app_layout-4.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.layout-4.0.8/setup.py` & `plone_app_layout-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.8"
+version = "4.1.0"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}"
 )
 
 setup(
     name="plone.app.layout",
```

