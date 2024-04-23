# Comparing `tmp/Products.CMFCore-3.4.tar.gz` & `tmp/Products.CMFCore-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.CMFCore-3.4.tar", last modified: Fri Apr 12 15:47:29 2024, max compression
+gzip compressed data, was "Products.CMFCore-3.5.tar", last modified: Tue Apr 23 21:38:18 2024, max compression
```

## Comparing `Products.CMFCore-3.4.tar` & `Products.CMFCore-3.5.tar`

### file list

```diff
@@ -1,337 +1,337 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.747461 Products.CMFCore-3.4/
--rw-r--r--   0 jens       (501) staff       (20)      670 2024-04-12 14:32:49.000000 Products.CMFCore-3.4/.readthedocs.yaml
--rw-r--r--   0 jens       (501) staff       (20)    33721 2024-04-12 15:44:13.000000 Products.CMFCore-3.4/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      805 2024-04-12 14:32:49.000000 Products.CMFCore-3.4/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      785 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    36153 2024-04-12 15:47:29.747537 Products.CMFCore-3.4/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1001 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/README.rst
--rw-r--r--   0 jens       (501) staff       (20)      402 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.718732 Products.CMFCore-3.4/docs/
--rw-r--r--   0 jens       (501) staff       (20)     3135 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/Makefile
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.715146 Products.CMFCore-3.4/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.715195 Products.CMFCore-3.4/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.718930 Products.CMFCore-3.4/docs/_build/html/_sources/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.719139 Products.CMFCore-3.4/docs/_build/html/_sources/api/
--rw-r--r--   0 jens       (501) staff       (20)     2841 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/_build/html/_sources/api/content.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5496 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/_build/html/_sources/api/tools.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/_build/html/_sources/changes.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      306 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.719358 Products.CMFCore-3.4/docs/api/
--rw-r--r--   0 jens       (501) staff       (20)     2841 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/api/content.rst
--rw-r--r--   0 jens       (501) staff       (20)     5496 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/api/tools.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/changes.rst
--rw-r--r--   0 jens       (501) staff       (20)     6940 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)      306 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)       43 2023-12-28 12:35:51.000000 Products.CMFCore-3.4/docs/requirements.txt
--rw-r--r--   0 jens       (501) staff       (20)      707 2024-04-12 15:47:29.747889 Products.CMFCore-3.4/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     2848 2024-04-12 15:44:20.000000 Products.CMFCore-3.4/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.715508 Products.CMFCore-3.4/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.719450 Products.CMFCore-3.4/src/Products/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.725924 Products.CMFCore-3.4/src/Products/CMFCore/
--rw-r--r--   0 jens       (501) staff       (20)    20362 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/ActionInformation.py
--rw-r--r--   0 jens       (501) staff       (20)    12217 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/ActionProviderBase.py
--rw-r--r--   0 jens       (501) staff       (20)     6607 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/ActionsTool.py
--rw-r--r--   0 jens       (501) staff       (20)     2306 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/CMFBTreeFolder.py
--rw-r--r--   0 jens       (501) staff       (20)    11373 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/CMFCatalogAware.py
--rw-r--r--   0 jens       (501) staff       (20)    31340 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/CachingPolicyManager.py
--rw-r--r--   0 jens       (501) staff       (20)    12804 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/CatalogTool.py
--rw-r--r--   0 jens       (501) staff       (20)    16841 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/ContentTypeRegistry.py
--rw-r--r--   0 jens       (501) staff       (20)    13312 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/CookieCrumbler.py
--rw-r--r--   0 jens       (501) staff       (20)    19228 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/DirectoryView.py
--rw-r--r--   0 jens       (501) staff       (20)     5417 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/DiscussionTool.py
--rw-r--r--   0 jens       (501) staff       (20)     5711 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/DynamicType.py
--rw-r--r--   0 jens       (501) staff       (20)     4137 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/Expression.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.726018 Products.CMFCore-3.4/src/Products/CMFCore/Extensions/
--rw-r--r--   0 jens       (501) staff       (20)      154 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/Extensions/TestRecord.py
--rw-r--r--   0 jens       (501) staff       (20)     7316 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSDTMLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     7659 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSFile.py
--rw-r--r--   0 jens       (501) staff       (20)     5705 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSImage.py
--rw-r--r--   0 jens       (501) staff       (20)     4937 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSMetadata.py
--rw-r--r--   0 jens       (501) staff       (20)     9420 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSObject.py
--rw-r--r--   0 jens       (501) staff       (20)    10454 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSPageTemplate.py
--rw-r--r--   0 jens       (501) staff       (20)     5502 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSPropertiesObject.py
--rw-r--r--   0 jens       (501) staff       (20)     8037 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSPythonScript.py
--rw-r--r--   0 jens       (501) staff       (20)     6243 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSReSTMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     6295 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSSTXMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     5532 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/FSZSQLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)    12275 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/MemberDataTool.py
--rw-r--r--   0 jens       (501) staff       (20)    20936 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/MembershipTool.py
--rw-r--r--   0 jens       (501) staff       (20)     3007 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/PortalContent.py
--rw-r--r--   0 jens       (501) staff       (20)    20374 2023-07-03 09:53:39.000000 Products.CMFCore-3.4/src/Products/CMFCore/PortalFolder.py
--rw-r--r--   0 jens       (501) staff       (20)     2768 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/PortalObject.py
--rw-r--r--   0 jens       (501) staff       (20)     7212 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/RegistrationTool.py
--rw-r--r--   0 jens       (501) staff       (20)     6695 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/Skinnable.py
--rw-r--r--   0 jens       (501) staff       (20)     3309 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/SkinsContainer.py
--rw-r--r--   0 jens       (501) staff       (20)    13340 2023-04-14 06:37:51.000000 Products.CMFCore-3.4/src/Products/CMFCore/SkinsTool.py
--rw-r--r--   0 jens       (501) staff       (20)    28718 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/TypesTool.py
--rw-r--r--   0 jens       (501) staff       (20)     3534 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/URLTool.py
--rw-r--r--   0 jens       (501) staff       (20)     3918 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/UndoTool.py
--rw-r--r--   0 jens       (501) staff       (20)     2528 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/WorkflowCore.py
--rw-r--r--   0 jens       (501) staff       (20)    21841 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/WorkflowTool.py
--rw-r--r--   0 jens       (501) staff       (20)     5055 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.726396 Products.CMFCore-3.4/src/Products/CMFCore/browser/
--rw-r--r--   0 jens       (501) staff       (20)       14 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/browser/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     4057 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/browser/actions.py
--rw-r--r--   0 jens       (501) staff       (20)     1303 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/browser/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)     3660 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/browser/typeinfo.py
--rw-r--r--   0 jens       (501) staff       (20)      424 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)     1417 2023-07-02 08:47:37.000000 Products.CMFCore-3.4/src/Products/CMFCore/content.zcml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.730255 Products.CMFCore-3.4/src/Products/CMFCore/dtml/
--rw-r--r--   0 jens       (501) staff       (20)     1083 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/addCC.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1558 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/addFSDirView.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1383 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/addInstance.dtml
--rw-r--r--   0 jens       (501) staff       (20)    10284 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/cachingPolicies.dtml
--rw-r--r--   0 jens       (501) staff       (20)     3876 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/catalogFind.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1888 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/compareResults.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2135 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/configureRegistrationTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2865 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custdtml.dtml
--rw-r--r--   0 jens       (501) staff       (20)     3862 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custfile.dtml
--rw-r--r--   0 jens       (501) staff       (20)     4874 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custimage.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2548 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custprops.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2863 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custpt.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2865 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custpy.dtml
--rw-r--r--   0 jens       (501) staff       (20)     3823 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custstx.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2846 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/custzsql.dtml
--rw-r--r--   0 jens       (501) staff       (20)      626 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/dirview_properties.dtml
--rw-r--r--   0 jens       (501) staff       (20)     6207 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/editToolsActions.dtml
--rw-r--r--   0 jens       (501) staff       (20)      844 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainActionsTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      346 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainCatalogTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      314 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainDiscussionTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      303 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainMemberDataTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      410 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainMembershipTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      294 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainRegistrationTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      443 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainSkinsTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      622 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainTypesTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      331 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainURLTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      310 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainUndoTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      465 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainWorkflowTool.dtml
--rw-r--r--   0 jens       (501) staff       (20)      433 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/extensionWidget.dtml
--rw-r--r--   0 jens       (501) staff       (20)     9219 2023-04-14 06:37:51.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/findForm.dtml
--rw-r--r--   0 jens       (501) staff       (20)      596 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/majorMinorWidget.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1694 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/manageActionProviders.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1355 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/memberdataContents.dtml
--rw-r--r--   0 jens       (501) staff       (20)     2110 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/membershipRolemapping.dtml
--rw-r--r--   0 jens       (501) staff       (20)      465 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/mimetypePredEdit.dtml
--rw-r--r--   0 jens       (501) staff       (20)      428 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/patternWidget.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1816 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/registryPredList.dtml
--rw-r--r--   0 jens       (501) staff       (20)      750 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/registryTest.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1941 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/selectWorkflows.dtml
--rw-r--r--   0 jens       (501) staff       (20)     3810 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/skinProps.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1023 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/dtml/zmi_workflows.dtml
--rw-r--r--   0 jens       (501) staff       (20)     1215 2023-07-02 08:47:37.000000 Products.CMFCore-3.4/src/Products/CMFCore/event.zcml
--rw-r--r--   0 jens       (501) staff       (20)     1433 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exceptions.py
--rw-r--r--   0 jens       (501) staff       (20)      921 2023-07-02 08:47:37.000000 Products.CMFCore-3.4/src/Products/CMFCore/explicitacquisition.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.731540 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/
--rw-r--r--   0 jens       (501) staff       (20)      752 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)    10072 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/actions.py
--rw-r--r--   0 jens       (501) staff       (20)     7625 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/cachingpolicymgr.py
--rw-r--r--   0 jens       (501) staff       (20)     1474 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/catalog.py
--rw-r--r--   0 jens       (501) staff       (20)     7129 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/configure.zcml
--rw-r--r--   0 jens       (501) staff       (20)    12158 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/content.py
--rw-r--r--   0 jens       (501) staff       (20)     5673 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/contenttyperegistry.py
--rw-r--r--   0 jens       (501) staff       (20)     3033 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/cookieauth.py
--rw-r--r--   0 jens       (501) staff       (20)     1514 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/mailhost.py
--rw-r--r--   0 jens       (501) staff       (20)     2535 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/memberdata.py
--rw-r--r--   0 jens       (501) staff       (20)     3017 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/properties.py
--rw-r--r--   0 jens       (501) staff       (20)     9014 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/skins.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.733037 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/
--rw-r--r--   0 jens       (501) staff       (20)      664 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     2083 2022-12-16 12:51:22.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/conformance.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.733136 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/four/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/four/placeholder.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.733210 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/one/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/one/placeholder.txt
--rw-r--r--   0 jens       (501) staff       (20)    21071 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_actions.py
--rw-r--r--   0 jens       (501) staff       (20)     8482 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py
--rw-r--r--   0 jens       (501) staff       (20)     7400 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_catalog.py
--rw-r--r--   0 jens       (501) staff       (20)    40943 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_content.py
--rw-r--r--   0 jens       (501) staff       (20)    11181 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py
--rw-r--r--   0 jens       (501) staff       (20)     7131 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_cookieauth.py
--rw-r--r--   0 jens       (501) staff       (20)     4652 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_mailhost.py
--rw-r--r--   0 jens       (501) staff       (20)     5676 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_memberdata.py
--rw-r--r--   0 jens       (501) staff       (20)     8751 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_properties.py
--rw-r--r--   0 jens       (501) staff       (20)    22889 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_skins.py
--rw-r--r--   0 jens       (501) staff       (20)    27200 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_typeinfo.py
--rw-r--r--   0 jens       (501) staff       (20)    12350 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_workflow.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.733290 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/three/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/three/placeholder.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.733368 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/two/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/two/placeholder.txt
--rw-r--r--   0 jens       (501) staff       (20)     8767 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/typeinfo.py
--rw-r--r--   0 jens       (501) staff       (20)     5125 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/exportimport/workflow.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.733538 Products.CMFCore-3.4/src/Products/CMFCore/help/
--rw-r--r--   0 jens       (501) staff       (20)     2049 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/help/Actions.stx
--rw-r--r--   0 jens       (501) staff       (20)     2007 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/help/CPMPolicies.stx
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.734842 Products.CMFCore-3.4/src/Products/CMFCore/images/
--rw-r--r--   0 jens       (501) staff       (20)      148 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/cmf_action.gif
--rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/cmf_action_category.gif
--rw-r--r--   0 jens       (501) staff       (20)      270 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/cookie.gif
--rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/dirview.gif
--rw-r--r--   0 jens       (501) staff       (20)      126 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/fsdtml.gif
--rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/fsfile.gif
--rw-r--r--   0 jens       (501) staff       (20)      174 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/fsimage.gif
--rw-r--r--   0 jens       (501) staff       (20)      205 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/fsprops.gif
--rw-r--r--   0 jens       (501) staff       (20)      181 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/fspt.gif
--rw-r--r--   0 jens       (501) staff       (20)      272 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/fspy.gif
--rw-r--r--   0 jens       (501) staff       (20)      165 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/fssqlmethod.gif
--rw-r--r--   0 jens       (501) staff       (20)      124 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/registry.gif
--rw-r--r--   0 jens       (501) staff       (20)      118 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/images/typeinfo.gif
--rw-r--r--   0 jens       (501) staff       (20)    10417 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/indexing.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.735439 Products.CMFCore-3.4/src/Products/CMFCore/interfaces/
--rw-r--r--   0 jens       (501) staff       (20)      787 2023-07-02 08:47:37.000000 Products.CMFCore-3.4/src/Products/CMFCore/interfaces/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)    18918 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_content.py
--rw-r--r--   0 jens       (501) staff       (20)     2391 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_cookieCrumbler.py
--rw-r--r--   0 jens       (501) staff       (20)     1677 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_events.py
--rw-r--r--   0 jens       (501) staff       (20)      304 2023-07-02 08:47:37.000000 Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_explicitacquisition.py
--rw-r--r--   0 jens       (501) staff       (20)    64829 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_tools.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.735673 Products.CMFCore-3.4/src/Products/CMFCore/locales/
--rw-r--r--   0 jens       (501) staff       (20)     1451 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/locales/cmf_core.pot
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.716488 Products.CMFCore-3.4/src/Products/CMFCore/locales/pt_BR/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.735765 Products.CMFCore-3.4/src/Products/CMFCore/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 jens       (501) staff       (20)     1810 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/locales/pt_BR/LC_MESSAGES/cmf_core.po
--rwxr-xr-x   0 jens       (501) staff       (20)      461 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/locales/update.sh
--rw-r--r--   0 jens       (501) staff       (20)      316 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/meta.zcml
--rw-r--r--   0 jens       (501) staff       (20)     1808 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/namespace.py
--rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/overrides.zcml
--rw-r--r--   0 jens       (501) staff       (20)     5082 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/permissions.py
--rw-r--r--   0 jens       (501) staff       (20)     1760 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/permissions.zcml
--rw-r--r--   0 jens       (501) staff       (20)     3160 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/subscribers.py
--rw-r--r--   0 jens       (501) staff       (20)     1512 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/subscribers.zcml
--rw-r--r--   0 jens       (501) staff       (20)     6920 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/testing.py
--rw-r--r--   0 jens       (501) staff       (20)      712 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/testing.zcml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.740170 Products.CMFCore-3.4/src/Products/CMFCore/tests/
--rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.740743 Products.CMFCore-3.4/src/Products/CMFCore/tests/base/
--rw-r--r--   0 jens       (501) staff       (20)       48 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/base/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     5270 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/base/content.py
--rw-r--r--   0 jens       (501) staff       (20)    12202 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/base/dummy.py
--rw-r--r--   0 jens       (501) staff       (20)     2897 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/base/security.py
--rw-r--r--   0 jens       (501) staff       (20)     8156 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/base/testcase.py
--rw-r--r--   0 jens       (501) staff       (20)     4363 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/base/tidata.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.716747 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.746981 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/#test1.py
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/.test1.py
--rw-r--r--   0 jens       (501) staff       (20)      405 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view.zpt
--rw-r--r--   0 jens       (501) staff       (20)      195 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_1.zpt
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.dtml
--rw-r--r--   0 jens       (501) staff       (20)       62 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.zpt
--rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_1.zpt
--rw-r--r--   0 jens       (501) staff       (20)       46 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_2.zpt
--rw-r--r--   0 jens       (501) staff       (20)       52 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_3.dtml
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_4.dtml
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test1.py
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py
--rw-r--r--   0 jens       (501) staff       (20)       34 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py.metadata
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test5.py
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py
--rw-r--r--   0 jens       (501) staff       (20)      180 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py.metadata
--rw-r--r--   0 jens       (501) staff       (20)       45 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml
--rw-r--r--   0 jens       (501) staff       (20)       47 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml.metadata
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML_CPM3.dtml
--rw-r--r--   0 jens       (501) staff       (20)       41 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)       92 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt
--rw-r--r--   0 jens       (501) staff       (20)       34 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)      140 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt
--rw-r--r--   0 jens       (501) staff       (20)       25 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)       73 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt
--rw-r--r--   0 jens       (501) staff       (20)       24 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)      140 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt
--rw-r--r--   0 jens       (501) staff       (20)       49 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt.metadata
--rw-r--r--   0 jens       (501) staff       (20)      397 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM1.zpt
--rw-r--r--   0 jens       (501) staff       (20)      191 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM2.zpt
--rw-r--r--   0 jens       (501) staff       (20)      183 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_dos.pt
--rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_mac.pt
--rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_unix.pt
--rw-r--r--   0 jens       (501) staff       (20)      169 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_utf8.pt
--rw-r--r--   0 jens       (501) staff       (20)       36 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testPTbad.pt
--rw-r--r--   0 jens       (501) staff       (20)      107 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst.metadata
--rw-r--r--   0 jens       (501) staff       (20)       87 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx.metadata
--rw-r--r--   0 jens       (501) staff       (20)       84 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testUtf8.js
--rw-r--r--   0 jens       (501) staff       (20)      133 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT.pt
--rw-r--r--   0 jens       (501) staff       (20)      151 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT_with_encoding.pt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.747089 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/
--rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/README.txt
--rw-r--r--   0 jens       (501) staff       (20)       39 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory.metadata
--rw-r--r--   0 jens       (501) staff       (20)       74 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dos.py
--rw-r--r--   0 jens       (501) staff       (20)       22 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml
--rw-r--r--   0 jens       (501) staff       (20)       36 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml.metadata
--rw-r--r--   0 jens       (501) staff       (20)    11218 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf
--rw-r--r--   0 jens       (501) staff       (20)       74 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf.metadata
--rw-r--r--   0 jens       (501) staff       (20)    11218 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf
--rw-r--r--   0 jens       (501) staff       (20)       55 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf.metadata
--rw-r--r--   0 jens       (501) staff       (20)      209 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif
--rw-r--r--   0 jens       (501) staff       (20)       75 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif.metadata
--rw-r--r--   0 jens       (501) staff       (20)       77 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_mac.py
--rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_manual_ignore.py
--rw-r--r--   0 jens       (501) staff       (20)      207 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_props.props
--rw-r--r--   0 jens       (501) staff       (20)       25 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.metadata
--rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.txt
--rw-r--r--   0 jens       (501) staff       (20)       18 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt
--rw-r--r--   0 jens       (501) staff       (20)       30 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt.metadata
--rw-r--r--   0 jens       (501) staff       (20)       72 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_unix.py
--rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_warn.py
--rw-r--r--   0 jens       (501) staff       (20)      326 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/testsql.zsql
--rw-r--r--   0 jens       (501) staff       (20)    19603 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ActionInformation.py
--rw-r--r--   0 jens       (501) staff       (20)    10030 2023-12-28 12:35:33.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ActionProviderBase.py
--rw-r--r--   0 jens       (501) staff       (20)     7718 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ActionsTool.py
--rw-r--r--   0 jens       (501) staff       (20)     1245 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CMFBTreeFolder.py
--rw-r--r--   0 jens       (501) staff       (20)    11162 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CMFCatalogAware.py
--rw-r--r--   0 jens       (501) staff       (20)    52032 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CachingPolicyManager.py
--rw-r--r--   0 jens       (501) staff       (20)    17423 2023-04-14 06:40:39.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CatalogIndexing.py
--rw-r--r--   0 jens       (501) staff       (20)    23073 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CatalogTool.py
--rw-r--r--   0 jens       (501) staff       (20)     9439 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ContentTypeRegistry.py
--rw-r--r--   0 jens       (501) staff       (20)     9183 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CookieCrumbler.py
--rw-r--r--   0 jens       (501) staff       (20)    12132 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_DirectoryView.py
--rw-r--r--   0 jens       (501) staff       (20)     1542 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_DiscussionTool.py
--rw-r--r--   0 jens       (501) staff       (20)     7290 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_DynamicType.py
--rw-r--r--   0 jens       (501) staff       (20)     3258 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_Expression.py
--rw-r--r--   0 jens       (501) staff       (20)     6693 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSDTMLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)    10397 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSFile.py
--rw-r--r--   0 jens       (501) staff       (20)     8864 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSImage.py
--rw-r--r--   0 jens       (501) staff       (20)     2493 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSMetadata.py
--rw-r--r--   0 jens       (501) staff       (20)     9035 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSPageTemplate.py
--rw-r--r--   0 jens       (501) staff       (20)     4515 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSPropertiesObject.py
--rw-r--r--   0 jens       (501) staff       (20)    10488 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSPythonScript.py
--rw-r--r--   0 jens       (501) staff       (20)     7830 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSReSTMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     9910 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSSTXMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     7585 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSSecurity.py
--rw-r--r--   0 jens       (501) staff       (20)     4798 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSZSQLMethod.py
--rw-r--r--   0 jens       (501) staff       (20)     7996 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_MemberDataTool.py
--rw-r--r--   0 jens       (501) staff       (20)    13574 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_MembershipTool.py
--rw-r--r--   0 jens       (501) staff       (20)     8825 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_OpaqueItems.py
--rw-r--r--   0 jens       (501) staff       (20)     4875 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_PortalContent.py
--rw-r--r--   0 jens       (501) staff       (20)    48913 2023-07-03 09:53:39.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_PortalFolder.py
--rw-r--r--   0 jens       (501) staff       (20)     1218 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_RegistrationTool.py
--rw-r--r--   0 jens       (501) staff       (20)     4947 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_SkinsTool.py
--rw-r--r--   0 jens       (501) staff       (20)    32890 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_TypesTool.py
--rw-r--r--   0 jens       (501) staff       (20)     2342 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_URLTool.py
--rw-r--r--   0 jens       (501) staff       (20)     1641 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_UndoTool.py
--rw-r--r--   0 jens       (501) staff       (20)    14729 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_WorkflowTool.py
--rw-r--r--   0 jens       (501) staff       (20)     2177 2023-07-02 08:47:37.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_explicitacquisition.py
--rw-r--r--   0 jens       (501) staff       (20)    10219 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_utils.py
--rw-r--r--   0 jens       (501) staff       (20)     2150 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tests/test_zcml.py
--rw-r--r--   0 jens       (501) staff       (20)      166 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tool.gif
--rw-r--r--   0 jens       (501) staff       (20)     1209 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/tool.zcml
--rw-r--r--   0 jens       (501) staff       (20)    28108 2024-04-12 15:43:45.000000 Products.CMFCore-3.4/src/Products/CMFCore/utils.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.747379 Products.CMFCore-3.4/src/Products/CMFCore/www/
--rw-r--r--   0 jens       (501) staff       (20)      624 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/www/cpsDiff.pt
--rw-r--r--   0 jens       (501) staff       (20)     2075 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/www/typeinfoAliases.zpt
--rw-r--r--   0 jens       (501) staff       (20)     2638 2021-11-02 08:51:13.000000 Products.CMFCore-3.4/src/Products/CMFCore/www/typesAliases.zpt
--rw-r--r--   0 jens       (501) staff       (20)     2942 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/CMFCore/zcml.py
--rw-r--r--   0 jens       (501) staff       (20)       76 2023-01-23 15:58:47.000000 Products.CMFCore-3.4/src/Products/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:47:29.720259 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    36153 2024-04-12 15:47:29.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)    14269 2024-04-12 15:47:29.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2024-04-12 15:47:29.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)       66 2024-04-12 15:47:29.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/entry_points.txt
--rw-r--r--   0 jens       (501) staff       (20)        9 2024-04-12 15:47:29.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/namespace_packages.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-12-16 12:53:25.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      370 2024-04-12 15:47:29.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        9 2024-04-12 15:47:29.000000 Products.CMFCore-3.4/src/Products.CMFCore.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     2318 2024-04-12 14:32:49.000000 Products.CMFCore-3.4/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.737908 Products.CMFCore-3.5/
+-rw-r--r--   0 jens       (501) staff       (20)      670 2024-04-23 21:35:19.000000 Products.CMFCore-3.5/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)    33992 2024-04-23 21:36:08.000000 Products.CMFCore-3.5/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      805 2024-04-23 21:35:19.000000 Products.CMFCore-3.5/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      785 2024-04-23 21:35:19.000000 Products.CMFCore-3.5/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    36424 2024-04-23 21:38:18.737985 Products.CMFCore-3.5/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1001 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      402 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.708358 Products.CMFCore-3.5/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     3135 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/Makefile
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.705103 Products.CMFCore-3.5/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.705146 Products.CMFCore-3.5/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.708577 Products.CMFCore-3.5/docs/_build/html/_sources/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.708841 Products.CMFCore-3.5/docs/_build/html/_sources/api/
+-rw-r--r--   0 jens       (501) staff       (20)     2841 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/_build/html/_sources/api/content.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5496 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/_build/html/_sources/api/tools.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/_build/html/_sources/changes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      306 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.709061 Products.CMFCore-3.5/docs/api/
+-rw-r--r--   0 jens       (501) staff       (20)     2841 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/api/content.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5496 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/api/tools.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/changes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     6940 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)      306 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)       43 2023-12-28 12:35:51.000000 Products.CMFCore-3.5/docs/requirements.txt
+-rw-r--r--   0 jens       (501) staff       (20)      707 2024-04-23 21:38:18.738302 Products.CMFCore-3.5/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     2848 2024-04-23 21:36:15.000000 Products.CMFCore-3.5/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.705413 Products.CMFCore-3.5/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.709160 Products.CMFCore-3.5/src/Products/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.715869 Products.CMFCore-3.5/src/Products/CMFCore/
+-rw-r--r--   0 jens       (501) staff       (20)    20362 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/ActionInformation.py
+-rw-r--r--   0 jens       (501) staff       (20)    12217 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/ActionProviderBase.py
+-rw-r--r--   0 jens       (501) staff       (20)     6607 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/ActionsTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     2306 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/CMFBTreeFolder.py
+-rw-r--r--   0 jens       (501) staff       (20)    11373 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/CMFCatalogAware.py
+-rw-r--r--   0 jens       (501) staff       (20)    31340 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/CachingPolicyManager.py
+-rw-r--r--   0 jens       (501) staff       (20)    12804 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/CatalogTool.py
+-rw-r--r--   0 jens       (501) staff       (20)    16841 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/ContentTypeRegistry.py
+-rw-r--r--   0 jens       (501) staff       (20)    13312 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/CookieCrumbler.py
+-rw-r--r--   0 jens       (501) staff       (20)    19228 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/DirectoryView.py
+-rw-r--r--   0 jens       (501) staff       (20)     5417 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/DiscussionTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     5711 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/DynamicType.py
+-rw-r--r--   0 jens       (501) staff       (20)     4137 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/Expression.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.715977 Products.CMFCore-3.5/src/Products/CMFCore/Extensions/
+-rw-r--r--   0 jens       (501) staff       (20)      154 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/Extensions/TestRecord.py
+-rw-r--r--   0 jens       (501) staff       (20)     7316 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSDTMLMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     7659 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSFile.py
+-rw-r--r--   0 jens       (501) staff       (20)     5705 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSImage.py
+-rw-r--r--   0 jens       (501) staff       (20)     4937 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSMetadata.py
+-rw-r--r--   0 jens       (501) staff       (20)     9420 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSObject.py
+-rw-r--r--   0 jens       (501) staff       (20)    10454 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSPageTemplate.py
+-rw-r--r--   0 jens       (501) staff       (20)     5502 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSPropertiesObject.py
+-rw-r--r--   0 jens       (501) staff       (20)     8037 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSPythonScript.py
+-rw-r--r--   0 jens       (501) staff       (20)     6243 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSReSTMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     6295 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSSTXMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     5532 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/FSZSQLMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)    12275 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/MemberDataTool.py
+-rw-r--r--   0 jens       (501) staff       (20)    20936 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/MembershipTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     3007 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/PortalContent.py
+-rw-r--r--   0 jens       (501) staff       (20)    20374 2023-07-03 09:53:39.000000 Products.CMFCore-3.5/src/Products/CMFCore/PortalFolder.py
+-rw-r--r--   0 jens       (501) staff       (20)     2768 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/PortalObject.py
+-rw-r--r--   0 jens       (501) staff       (20)     7212 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/RegistrationTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     6695 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/Skinnable.py
+-rw-r--r--   0 jens       (501) staff       (20)     3309 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/SkinsContainer.py
+-rw-r--r--   0 jens       (501) staff       (20)    13340 2023-04-14 06:37:51.000000 Products.CMFCore-3.5/src/Products/CMFCore/SkinsTool.py
+-rw-r--r--   0 jens       (501) staff       (20)    28718 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/TypesTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     3534 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/URLTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     3918 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/UndoTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     2528 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/WorkflowCore.py
+-rw-r--r--   0 jens       (501) staff       (20)    21841 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/WorkflowTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     5055 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.716387 Products.CMFCore-3.5/src/Products/CMFCore/browser/
+-rw-r--r--   0 jens       (501) staff       (20)       14 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/browser/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     4057 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/browser/actions.py
+-rw-r--r--   0 jens       (501) staff       (20)     1303 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/browser/configure.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     3660 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/browser/typeinfo.py
+-rw-r--r--   0 jens       (501) staff       (20)      424 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/configure.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     1417 2023-07-02 08:47:37.000000 Products.CMFCore-3.5/src/Products/CMFCore/content.zcml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.720645 Products.CMFCore-3.5/src/Products/CMFCore/dtml/
+-rw-r--r--   0 jens       (501) staff       (20)     1083 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/addCC.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1558 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/addFSDirView.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1383 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/addInstance.dtml
+-rw-r--r--   0 jens       (501) staff       (20)    10284 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/cachingPolicies.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     3876 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/catalogFind.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1888 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/compareResults.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     2135 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/configureRegistrationTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     2865 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custdtml.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     3862 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custfile.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     4874 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custimage.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     2548 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custprops.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     2863 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custpt.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     2865 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custpy.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     3823 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custstx.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     2846 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/custzsql.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      626 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/dirview_properties.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     6207 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/editToolsActions.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      844 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainActionsTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      346 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainCatalogTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      314 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainDiscussionTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      303 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainMemberDataTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      410 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainMembershipTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      294 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainRegistrationTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      443 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainSkinsTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      622 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainTypesTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      331 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainURLTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      310 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainUndoTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      465 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainWorkflowTool.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      433 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/extensionWidget.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     9219 2023-04-14 06:37:51.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/findForm.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      596 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/majorMinorWidget.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1694 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/manageActionProviders.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1355 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/memberdataContents.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     2110 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/membershipRolemapping.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      465 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/mimetypePredEdit.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      428 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/patternWidget.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1816 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/registryPredList.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      750 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/registryTest.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1941 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/selectWorkflows.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     3810 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/skinProps.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1023 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/dtml/zmi_workflows.dtml
+-rw-r--r--   0 jens       (501) staff       (20)     1215 2023-07-02 08:47:37.000000 Products.CMFCore-3.5/src/Products/CMFCore/event.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     1433 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exceptions.py
+-rw-r--r--   0 jens       (501) staff       (20)      921 2023-07-02 08:47:37.000000 Products.CMFCore-3.5/src/Products/CMFCore/explicitacquisition.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.722124 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/
+-rw-r--r--   0 jens       (501) staff       (20)      752 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)    10072 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/actions.py
+-rw-r--r--   0 jens       (501) staff       (20)     7625 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/cachingpolicymgr.py
+-rw-r--r--   0 jens       (501) staff       (20)     1474 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/catalog.py
+-rw-r--r--   0 jens       (501) staff       (20)     7129 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/configure.zcml
+-rw-r--r--   0 jens       (501) staff       (20)    12158 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/content.py
+-rw-r--r--   0 jens       (501) staff       (20)     5673 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/contenttyperegistry.py
+-rw-r--r--   0 jens       (501) staff       (20)     3033 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/cookieauth.py
+-rw-r--r--   0 jens       (501) staff       (20)     1514 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/mailhost.py
+-rw-r--r--   0 jens       (501) staff       (20)     2535 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/memberdata.py
+-rw-r--r--   0 jens       (501) staff       (20)     3017 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/properties.py
+-rw-r--r--   0 jens       (501) staff       (20)     9014 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/skins.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.723584 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/
+-rw-r--r--   0 jens       (501) staff       (20)      664 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     2083 2022-12-16 12:51:22.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/conformance.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.723696 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/four/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/four/placeholder.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.723774 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/one/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/one/placeholder.txt
+-rw-r--r--   0 jens       (501) staff       (20)    21071 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_actions.py
+-rw-r--r--   0 jens       (501) staff       (20)     8482 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py
+-rw-r--r--   0 jens       (501) staff       (20)     7400 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_catalog.py
+-rw-r--r--   0 jens       (501) staff       (20)    40943 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_content.py
+-rw-r--r--   0 jens       (501) staff       (20)    11181 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py
+-rw-r--r--   0 jens       (501) staff       (20)     7131 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_cookieauth.py
+-rw-r--r--   0 jens       (501) staff       (20)     4652 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_mailhost.py
+-rw-r--r--   0 jens       (501) staff       (20)     5676 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_memberdata.py
+-rw-r--r--   0 jens       (501) staff       (20)     8751 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_properties.py
+-rw-r--r--   0 jens       (501) staff       (20)    22889 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_skins.py
+-rw-r--r--   0 jens       (501) staff       (20)    27200 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_typeinfo.py
+-rw-r--r--   0 jens       (501) staff       (20)    12350 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_workflow.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.723853 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/three/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/three/placeholder.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.723930 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/two/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/two/placeholder.txt
+-rw-r--r--   0 jens       (501) staff       (20)     8767 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/typeinfo.py
+-rw-r--r--   0 jens       (501) staff       (20)     5125 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/exportimport/workflow.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.724111 Products.CMFCore-3.5/src/Products/CMFCore/help/
+-rw-r--r--   0 jens       (501) staff       (20)     2049 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/help/Actions.stx
+-rw-r--r--   0 jens       (501) staff       (20)     2007 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/help/CPMPolicies.stx
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.725340 Products.CMFCore-3.5/src/Products/CMFCore/images/
+-rw-r--r--   0 jens       (501) staff       (20)      148 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/cmf_action.gif
+-rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/cmf_action_category.gif
+-rw-r--r--   0 jens       (501) staff       (20)      270 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/cookie.gif
+-rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/dirview.gif
+-rw-r--r--   0 jens       (501) staff       (20)      126 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/fsdtml.gif
+-rw-r--r--   0 jens       (501) staff       (20)      143 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/fsfile.gif
+-rw-r--r--   0 jens       (501) staff       (20)      174 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/fsimage.gif
+-rw-r--r--   0 jens       (501) staff       (20)      205 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/fsprops.gif
+-rw-r--r--   0 jens       (501) staff       (20)      181 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/fspt.gif
+-rw-r--r--   0 jens       (501) staff       (20)      272 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/fspy.gif
+-rw-r--r--   0 jens       (501) staff       (20)      165 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/fssqlmethod.gif
+-rw-r--r--   0 jens       (501) staff       (20)      124 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/registry.gif
+-rw-r--r--   0 jens       (501) staff       (20)      118 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/images/typeinfo.gif
+-rw-r--r--   0 jens       (501) staff       (20)    10417 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/indexing.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.725908 Products.CMFCore-3.5/src/Products/CMFCore/interfaces/
+-rw-r--r--   0 jens       (501) staff       (20)      787 2023-07-02 08:47:37.000000 Products.CMFCore-3.5/src/Products/CMFCore/interfaces/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)    18918 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_content.py
+-rw-r--r--   0 jens       (501) staff       (20)     2391 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_cookieCrumbler.py
+-rw-r--r--   0 jens       (501) staff       (20)     1677 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_events.py
+-rw-r--r--   0 jens       (501) staff       (20)      304 2023-07-02 08:47:37.000000 Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_explicitacquisition.py
+-rw-r--r--   0 jens       (501) staff       (20)    64829 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_tools.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.726147 Products.CMFCore-3.5/src/Products/CMFCore/locales/
+-rw-r--r--   0 jens       (501) staff       (20)     1451 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/locales/cmf_core.pot
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.706254 Products.CMFCore-3.5/src/Products/CMFCore/locales/pt_BR/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.726270 Products.CMFCore-3.5/src/Products/CMFCore/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jens       (501) staff       (20)     1810 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/locales/pt_BR/LC_MESSAGES/cmf_core.po
+-rwxr-xr-x   0 jens       (501) staff       (20)      461 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/locales/update.sh
+-rw-r--r--   0 jens       (501) staff       (20)      316 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/meta.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     1808 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/namespace.py
+-rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/overrides.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     5082 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/permissions.py
+-rw-r--r--   0 jens       (501) staff       (20)     1760 2024-04-12 15:43:45.000000 Products.CMFCore-3.5/src/Products/CMFCore/permissions.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     3160 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/subscribers.py
+-rw-r--r--   0 jens       (501) staff       (20)     1512 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/subscribers.zcml
+-rw-r--r--   0 jens       (501) staff       (20)     6920 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/testing.py
+-rw-r--r--   0 jens       (501) staff       (20)      712 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/testing.zcml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.730663 Products.CMFCore-3.5/src/Products/CMFCore/tests/
+-rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.731227 Products.CMFCore-3.5/src/Products/CMFCore/tests/base/
+-rw-r--r--   0 jens       (501) staff       (20)       48 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/base/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     5270 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/base/content.py
+-rw-r--r--   0 jens       (501) staff       (20)    12202 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/base/dummy.py
+-rw-r--r--   0 jens       (501) staff       (20)     2897 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/base/security.py
+-rw-r--r--   0 jens       (501) staff       (20)     8156 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/base/testcase.py
+-rw-r--r--   0 jens       (501) staff       (20)     4363 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/base/tidata.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.706503 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.737391 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/
+-rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/#test1.py
+-rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/.test1.py
+-rw-r--r--   0 jens       (501) staff       (20)      405 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view.zpt
+-rw-r--r--   0 jens       (501) staff       (20)      195 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_1.zpt
+-rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.dtml
+-rw-r--r--   0 jens       (501) staff       (20)       62 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/nested_view_2.zpt
+-rw-r--r--   0 jens       (501) staff       (20)      139 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_1.zpt
+-rw-r--r--   0 jens       (501) staff       (20)       46 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_2.zpt
+-rw-r--r--   0 jens       (501) staff       (20)       52 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_3.dtml
+-rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/output_page_4.dtml
+-rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test1.py
+-rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py
+-rw-r--r--   0 jens       (501) staff       (20)       34 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test4.py.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test5.py
+-rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py
+-rw-r--r--   0 jens       (501) staff       (20)      180 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test6.py.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       45 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml
+-rw-r--r--   0 jens       (501) staff       (20)       47 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML.dtml.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testDTML_CPM3.dtml
+-rw-r--r--   0 jens       (501) staff       (20)       41 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt
+-rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT.pt.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       92 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt
+-rw-r--r--   0 jens       (501) staff       (20)       34 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT2.pt.metadata
+-rw-r--r--   0 jens       (501) staff       (20)      140 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt
+-rw-r--r--   0 jens       (501) staff       (20)       25 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT3.pt.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       73 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt
+-rw-r--r--   0 jens       (501) staff       (20)       24 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT4.pt.metadata
+-rw-r--r--   0 jens       (501) staff       (20)      140 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt
+-rw-r--r--   0 jens       (501) staff       (20)       49 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT5.pt.metadata
+-rw-r--r--   0 jens       (501) staff       (20)      397 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM1.zpt
+-rw-r--r--   0 jens       (501) staff       (20)      191 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_CPM2.zpt
+-rw-r--r--   0 jens       (501) staff       (20)      183 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_dos.pt
+-rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_mac.pt
+-rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_multiline_python_unix.pt
+-rw-r--r--   0 jens       (501) staff       (20)      169 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPT_utf8.pt
+-rw-r--r--   0 jens       (501) staff       (20)       36 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testPTbad.pt
+-rw-r--r--   0 jens       (501) staff       (20)      107 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testReST.rst.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       87 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx
+-rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testSTX.stx.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       84 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testUtf8.js
+-rw-r--r--   0 jens       (501) staff       (20)      133 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT.pt
+-rw-r--r--   0 jens       (501) staff       (20)      151 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testXMLPT_with_encoding.pt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.737519 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/
+-rw-r--r--   0 jens       (501) staff       (20)      179 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory/README.txt
+-rw-r--r--   0 jens       (501) staff       (20)       39 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_directory.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       74 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dos.py
+-rw-r--r--   0 jens       (501) staff       (20)       22 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml
+-rw-r--r--   0 jens       (501) staff       (20)       36 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_dtml.dtml.metadata
+-rw-r--r--   0 jens       (501) staff       (20)    11218 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf
+-rw-r--r--   0 jens       (501) staff       (20)       74 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf.metadata
+-rw-r--r--   0 jens       (501) staff       (20)    11218 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf
+-rw-r--r--   0 jens       (501) staff       (20)       55 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf.metadata
+-rw-r--r--   0 jens       (501) staff       (20)      209 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif
+-rw-r--r--   0 jens       (501) staff       (20)       75 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_image.gif.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       77 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_mac.py
+-rw-r--r--   0 jens       (501) staff       (20)       27 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_manual_ignore.py
+-rw-r--r--   0 jens       (501) staff       (20)      207 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_props.props
+-rw-r--r--   0 jens       (501) staff       (20)       25 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       23 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text.txt
+-rw-r--r--   0 jens       (501) staff       (20)       18 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt
+-rw-r--r--   0 jens       (501) staff       (20)       30 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_text_latin1.txt.metadata
+-rw-r--r--   0 jens       (501) staff       (20)       72 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_unix.py
+-rw-r--r--   0 jens       (501) staff       (20)       26 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_warn.py
+-rw-r--r--   0 jens       (501) staff       (20)      326 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/testsql.zsql
+-rw-r--r--   0 jens       (501) staff       (20)    19603 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ActionInformation.py
+-rw-r--r--   0 jens       (501) staff       (20)    10030 2023-12-28 12:35:33.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ActionProviderBase.py
+-rw-r--r--   0 jens       (501) staff       (20)     7718 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ActionsTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     1245 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CMFBTreeFolder.py
+-rw-r--r--   0 jens       (501) staff       (20)    11162 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CMFCatalogAware.py
+-rw-r--r--   0 jens       (501) staff       (20)    52032 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CachingPolicyManager.py
+-rw-r--r--   0 jens       (501) staff       (20)    17423 2023-04-14 06:40:39.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CatalogIndexing.py
+-rw-r--r--   0 jens       (501) staff       (20)    23073 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CatalogTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     9439 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ContentTypeRegistry.py
+-rw-r--r--   0 jens       (501) staff       (20)     9183 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CookieCrumbler.py
+-rw-r--r--   0 jens       (501) staff       (20)    12132 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_DirectoryView.py
+-rw-r--r--   0 jens       (501) staff       (20)     1542 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_DiscussionTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     7290 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_DynamicType.py
+-rw-r--r--   0 jens       (501) staff       (20)     3258 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_Expression.py
+-rw-r--r--   0 jens       (501) staff       (20)     6693 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSDTMLMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)    10397 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSFile.py
+-rw-r--r--   0 jens       (501) staff       (20)     8864 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSImage.py
+-rw-r--r--   0 jens       (501) staff       (20)     2493 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSMetadata.py
+-rw-r--r--   0 jens       (501) staff       (20)     9035 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSPageTemplate.py
+-rw-r--r--   0 jens       (501) staff       (20)     4515 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSPropertiesObject.py
+-rw-r--r--   0 jens       (501) staff       (20)    10488 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSPythonScript.py
+-rw-r--r--   0 jens       (501) staff       (20)     7830 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSReSTMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     9910 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSSTXMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     7585 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSSecurity.py
+-rw-r--r--   0 jens       (501) staff       (20)     4798 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSZSQLMethod.py
+-rw-r--r--   0 jens       (501) staff       (20)     7996 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_MemberDataTool.py
+-rw-r--r--   0 jens       (501) staff       (20)    13574 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_MembershipTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     8825 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_OpaqueItems.py
+-rw-r--r--   0 jens       (501) staff       (20)     4875 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_PortalContent.py
+-rw-r--r--   0 jens       (501) staff       (20)    48913 2023-07-03 09:53:39.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_PortalFolder.py
+-rw-r--r--   0 jens       (501) staff       (20)     1218 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_RegistrationTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     4947 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_SkinsTool.py
+-rw-r--r--   0 jens       (501) staff       (20)    32890 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_TypesTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     2342 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_URLTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     1641 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_UndoTool.py
+-rw-r--r--   0 jens       (501) staff       (20)    14729 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_WorkflowTool.py
+-rw-r--r--   0 jens       (501) staff       (20)     2177 2023-07-02 08:47:37.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_explicitacquisition.py
+-rw-r--r--   0 jens       (501) staff       (20)    10219 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_utils.py
+-rw-r--r--   0 jens       (501) staff       (20)     2150 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tests/test_zcml.py
+-rw-r--r--   0 jens       (501) staff       (20)      166 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tool.gif
+-rw-r--r--   0 jens       (501) staff       (20)     1209 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/tool.zcml
+-rw-r--r--   0 jens       (501) staff       (20)    28875 2024-04-23 21:33:44.000000 Products.CMFCore-3.5/src/Products/CMFCore/utils.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.737823 Products.CMFCore-3.5/src/Products/CMFCore/www/
+-rw-r--r--   0 jens       (501) staff       (20)      624 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/www/cpsDiff.pt
+-rw-r--r--   0 jens       (501) staff       (20)     2075 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/www/typeinfoAliases.zpt
+-rw-r--r--   0 jens       (501) staff       (20)     2638 2021-11-02 08:51:13.000000 Products.CMFCore-3.5/src/Products/CMFCore/www/typesAliases.zpt
+-rw-r--r--   0 jens       (501) staff       (20)     2942 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/CMFCore/zcml.py
+-rw-r--r--   0 jens       (501) staff       (20)       76 2023-01-23 15:58:47.000000 Products.CMFCore-3.5/src/Products/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-23 21:38:18.709979 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    36424 2024-04-23 21:38:18.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)    14269 2024-04-23 21:38:18.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-04-23 21:38:18.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)       66 2024-04-23 21:38:18.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        9 2024-04-23 21:38:18.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/namespace_packages.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-12-16 12:53:25.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      370 2024-04-23 21:38:18.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        9 2024-04-23 21:38:18.000000 Products.CMFCore-3.5/src/Products.CMFCore.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2318 2024-04-23 21:35:19.000000 Products.CMFCore-3.5/tox.ini
```

### Comparing `Products.CMFCore-3.4/.readthedocs.yaml` & `Products.CMFCore-3.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/CHANGES.rst` & `Products.CMFCore-3.5/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Products.CMFCore Changelog
 ==========================
 
+3.5 (2024-03-23)
+----------------
+
+- Use the new ``resources`` keyword of ``registerClass`` if available.
+  This avoids a deprecation warning for using a non callable constructor in Zope higher than 5.9.
+  (`#1202 <https://github.com/zopefoundation/Zope/issues/1202>`_)
+
+
 3.4 (2024-04-12)
 ----------------
 
 - Add i18n translation support.
   (`#135 <https://github.com/zopefoundation/Products.CMFCore/issues/135>`_)
 
 
 3.3 (2024-01-23)
 ----------------
 
 - Add support for Python 3.12.
 
-- ZMI: added limit of folderish objects for customizing and 
+- ZMI: added limit of folderish objects for customizing and
   handling SVG files as FSImage showing a preview.
   (`#130 <https://github.com/zopefoundation/Products.CMFCore/pull/130>`_)
 
 
 3.2 (2023-07-03)
 ----------------
```

### Comparing `Products.CMFCore-3.4/CONTRIBUTING.md` & `Products.CMFCore-3.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/LICENSE.txt` & `Products.CMFCore-3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/MANIFEST.in` & `Products.CMFCore-3.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/PKG-INFO` & `Products.CMFCore-3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CMFCore
-Version: 3.4
+Version: 3.5
 Summary: Zope Content Management Framework core components
 Home-page: https://github.com/zopefoundation/Products.CMFCore
 Author: Zope Foundation and Contributors
 Author-email: zope-cmf@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zope.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Products.CMFCore/issues
@@ -58,27 +58,35 @@
 
 
 ------------------------------------------------------------
 
 Products.CMFCore Changelog
 ==========================
 
+3.5 (2024-03-23)
+----------------
+
+- Use the new ``resources`` keyword of ``registerClass`` if available.
+  This avoids a deprecation warning for using a non callable constructor in Zope higher than 5.9.
+  (`#1202 <https://github.com/zopefoundation/Zope/issues/1202>`_)
+
+
 3.4 (2024-04-12)
 ----------------
 
 - Add i18n translation support.
   (`#135 <https://github.com/zopefoundation/Products.CMFCore/issues/135>`_)
 
 
 3.3 (2024-01-23)
 ----------------
 
 - Add support for Python 3.12.
 
-- ZMI: added limit of folderish objects for customizing and 
+- ZMI: added limit of folderish objects for customizing and
   handling SVG files as FSImage showing a preview.
   (`#130 <https://github.com/zopefoundation/Products.CMFCore/pull/130>`_)
 
 
 3.2 (2023-07-03)
 ----------------
```

### Comparing `Products.CMFCore-3.4/README.rst` & `Products.CMFCore-3.5/README.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/docs/Makefile` & `Products.CMFCore-3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/docs/_build/html/_sources/api/content.rst.txt` & `Products.CMFCore-3.5/docs/_build/html/_sources/api/content.rst.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/docs/_build/html/_sources/api/tools.rst.txt` & `Products.CMFCore-3.5/docs/_build/html/_sources/api/tools.rst.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/docs/api/content.rst` & `Products.CMFCore-3.5/docs/api/content.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/docs/api/tools.rst` & `Products.CMFCore-3.5/docs/api/tools.rst`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/docs/conf.py` & `Products.CMFCore-3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/setup.cfg` & `Products.CMFCore-3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/setup.py` & `Products.CMFCore-3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 _boundary = '\n' + ('-' * 60) + '\n\n'
 README = _boundary.join([
     _package_doc('README.rst'),
     _package_doc('CHANGES.rst'),
 ])
 
 setup(name='Products.%s' % NAME,
-      version='3.4',
+      version='3.5',
       description='Zope Content Management Framework core components',
       long_description=README,
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Framework :: Plone',
           'Framework :: Zope :: 5',
           'Intended Audience :: Developers',
```

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/ActionInformation.py` & `Products.CMFCore-3.5/src/Products/CMFCore/ActionInformation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/ActionProviderBase.py` & `Products.CMFCore-3.5/src/Products/CMFCore/ActionProviderBase.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/ActionsTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/ActionsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/CMFBTreeFolder.py` & `Products.CMFCore-3.5/src/Products/CMFCore/CMFBTreeFolder.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/CMFCatalogAware.py` & `Products.CMFCore-3.5/src/Products/CMFCore/CMFCatalogAware.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/CachingPolicyManager.py` & `Products.CMFCore-3.5/src/Products/CMFCore/CachingPolicyManager.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/CatalogTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/CatalogTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/ContentTypeRegistry.py` & `Products.CMFCore-3.5/src/Products/CMFCore/ContentTypeRegistry.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/CookieCrumbler.py` & `Products.CMFCore-3.5/src/Products/CMFCore/CookieCrumbler.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/DirectoryView.py` & `Products.CMFCore-3.5/src/Products/CMFCore/DirectoryView.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/DiscussionTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/DiscussionTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/DynamicType.py` & `Products.CMFCore-3.5/src/Products/CMFCore/DynamicType.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/Expression.py` & `Products.CMFCore-3.5/src/Products/CMFCore/Expression.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSDTMLMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSDTMLMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSFile.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSFile.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSImage.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSImage.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSMetadata.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSMetadata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSObject.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSObject.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSPageTemplate.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSPageTemplate.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSPropertiesObject.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSPropertiesObject.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSPythonScript.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSPythonScript.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSReSTMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSReSTMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSSTXMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSSTXMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/FSZSQLMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/FSZSQLMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/MemberDataTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/MemberDataTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/MembershipTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/MembershipTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/PortalContent.py` & `Products.CMFCore-3.5/src/Products/CMFCore/PortalContent.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/PortalFolder.py` & `Products.CMFCore-3.5/src/Products/CMFCore/PortalFolder.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/PortalObject.py` & `Products.CMFCore-3.5/src/Products/CMFCore/PortalObject.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/RegistrationTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/RegistrationTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/Skinnable.py` & `Products.CMFCore-3.5/src/Products/CMFCore/Skinnable.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/SkinsContainer.py` & `Products.CMFCore-3.5/src/Products/CMFCore/SkinsContainer.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/SkinsTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/SkinsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/TypesTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/TypesTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/URLTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/URLTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/UndoTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/UndoTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/WorkflowCore.py` & `Products.CMFCore-3.5/src/Products/CMFCore/WorkflowCore.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/WorkflowTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/WorkflowTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/__init__.py` & `Products.CMFCore-3.5/src/Products/CMFCore/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/browser/actions.py` & `Products.CMFCore-3.5/src/Products/CMFCore/browser/actions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/browser/configure.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/browser/typeinfo.py` & `Products.CMFCore-3.5/src/Products/CMFCore/browser/typeinfo.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/content.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/content.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/addCC.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/addCC.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/addFSDirView.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/addFSDirView.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/addInstance.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/addInstance.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/cachingPolicies.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/cachingPolicies.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/catalogFind.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/catalogFind.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/compareResults.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/compareResults.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/configureRegistrationTool.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/configureRegistrationTool.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custdtml.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custdtml.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custfile.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custfile.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custimage.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custimage.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custprops.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custprops.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custpt.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custpt.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custpy.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custpy.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custstx.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custstx.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/custzsql.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/custzsql.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/dirview_properties.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/dirview_properties.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/editToolsActions.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/editToolsActions.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainActionsTool.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainActionsTool.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/explainTypesTool.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/explainTypesTool.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/findForm.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/findForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/majorMinorWidget.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/majorMinorWidget.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/manageActionProviders.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/manageActionProviders.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/memberdataContents.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/memberdataContents.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/membershipRolemapping.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/membershipRolemapping.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/registryPredList.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/registryPredList.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/registryTest.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/registryTest.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/selectWorkflows.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/selectWorkflows.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/skinProps.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/skinProps.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/dtml/zmi_workflows.dtml` & `Products.CMFCore-3.5/src/Products/CMFCore/dtml/zmi_workflows.dtml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/event.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/event.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exceptions.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exceptions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/explicitacquisition.py` & `Products.CMFCore-3.5/src/Products/CMFCore/explicitacquisition.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/__init__.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/actions.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/actions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/cachingpolicymgr.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/cachingpolicymgr.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/catalog.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/catalog.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/configure.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/content.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/content.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/contenttyperegistry.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/contenttyperegistry.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/cookieauth.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/cookieauth.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/mailhost.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/mailhost.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/memberdata.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/memberdata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/properties.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/properties.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/skins.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/skins.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/__init__.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/conformance.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/conformance.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_actions.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_cachingpolicymgr.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_catalog.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_content.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_contenttyperegistry.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_cookieauth.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_cookieauth.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_mailhost.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_mailhost.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_memberdata.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_memberdata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_properties.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_skins.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_skins.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_typeinfo.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_typeinfo.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/tests/test_workflow.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/typeinfo.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/typeinfo.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/exportimport/workflow.py` & `Products.CMFCore-3.5/src/Products/CMFCore/exportimport/workflow.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/help/Actions.stx` & `Products.CMFCore-3.5/src/Products/CMFCore/help/Actions.stx`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/help/CPMPolicies.stx` & `Products.CMFCore-3.5/src/Products/CMFCore/help/CPMPolicies.stx`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/indexing.py` & `Products.CMFCore-3.5/src/Products/CMFCore/indexing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/interfaces/__init__.py` & `Products.CMFCore-3.5/src/Products/CMFCore/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_content.py` & `Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_content.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_cookieCrumbler.py` & `Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_cookieCrumbler.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_events.py` & `Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_events.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/interfaces/_tools.py` & `Products.CMFCore-3.5/src/Products/CMFCore/interfaces/_tools.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/locales/cmf_core.pot` & `Products.CMFCore-3.5/src/Products/CMFCore/locales/cmf_core.pot`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/locales/pt_BR/LC_MESSAGES/cmf_core.po` & `Products.CMFCore-3.5/src/Products/CMFCore/locales/pt_BR/LC_MESSAGES/cmf_core.po`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/namespace.py` & `Products.CMFCore-3.5/src/Products/CMFCore/namespace.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/permissions.py` & `Products.CMFCore-3.5/src/Products/CMFCore/permissions.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/permissions.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/permissions.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/subscribers.py` & `Products.CMFCore-3.5/src/Products/CMFCore/subscribers.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/subscribers.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/subscribers.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/testing.py` & `Products.CMFCore-3.5/src/Products/CMFCore/testing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/testing.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/base/content.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/base/content.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/base/dummy.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/base/dummy.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/base/security.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/base/security.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/base/testcase.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/base/testcase.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/base/tidata.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/base/tidata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file.swf`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/fake_skins/fake_skin/test_file_two.swf`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ActionInformation.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ActionInformation.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ActionProviderBase.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ActionProviderBase.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ActionsTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ActionsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CMFBTreeFolder.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CMFBTreeFolder.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CMFCatalogAware.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CMFCatalogAware.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CachingPolicyManager.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CachingPolicyManager.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CatalogIndexing.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CatalogIndexing.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CatalogTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CatalogTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_ContentTypeRegistry.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_ContentTypeRegistry.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_CookieCrumbler.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_CookieCrumbler.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_DirectoryView.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_DirectoryView.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_DiscussionTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_DiscussionTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_DynamicType.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_DynamicType.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_Expression.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_Expression.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSDTMLMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSDTMLMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSFile.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSFile.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSImage.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSImage.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSMetadata.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSMetadata.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSPageTemplate.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSPageTemplate.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSPropertiesObject.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSPropertiesObject.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSPythonScript.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSPythonScript.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSReSTMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSReSTMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSSTXMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSSTXMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSSecurity.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSSecurity.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_FSZSQLMethod.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_FSZSQLMethod.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_MemberDataTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_MemberDataTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_MembershipTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_MembershipTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_OpaqueItems.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_OpaqueItems.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_PortalContent.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_PortalContent.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_PortalFolder.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_PortalFolder.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_RegistrationTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_RegistrationTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_SkinsTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_SkinsTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_TypesTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_TypesTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_URLTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_URLTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_UndoTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_UndoTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_WorkflowTool.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_WorkflowTool.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_explicitacquisition.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_explicitacquisition.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_utils.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tests/test_zcml.py` & `Products.CMFCore-3.5/src/Products/CMFCore/tests/test_zcml.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/tool.zcml` & `Products.CMFCore-3.5/src/Products/CMFCore/tool.zcml`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/utils.py` & `Products.CMFCore-3.5/src/Products/CMFCore/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -595,21 +595,28 @@
                  DeprecationWarning, stacklevel=2)
         self.icon = icon
 
     def initialize(self, context):
         # Add only one meta type to the folder add list.
         productObject = context._ProductContext__prod
         self.product_name = productObject.id
-        context.registerClass(
-            meta_type=self.meta_type,
-            # This is a little sneaky: we add self to the
-            # FactoryDispatcher under the name "toolinit".
-            # manage_addTool() can then grab it.
-            constructors=(manage_addToolForm, manage_addTool, self),
-            icon=self.icon)
+        # We add self to the FactoryDispatcher under the name 'toolinit'.
+        # manage_addContentType() can then grab it.
+        try:
+            context.registerClass(
+                meta_type=self.meta_type,
+                constructors=(manage_addToolForm, manage_addTool),
+                resources=(self, ),
+                icon=self.icon)
+        except TypeError:
+            # The 'resources' keyword was only introduced after Zope 5.9.
+            context.registerClass(
+                meta_type=self.meta_type,
+                constructors=(manage_addToolForm, manage_addTool, self),
+                icon=self.icon)
 
         if self.icon:
             icon = os_path.split(self.icon)[1]
         else:
             icon = None
         for tool in self.tools:
             tool.__factory_meta_type__ = self.meta_type
@@ -676,23 +683,35 @@
         self.content_types = content_types
         self.permission = permission
         self.extra_constructors = extra_constructors
         self.visibility = visibility
 
     def initialize(self, context):
         # Add only one meta type to the folder add list.
-        context.registerClass(
-            meta_type=self.meta_type,
-            # This is a little sneaky: we add self to the
-            # FactoryDispatcher under the name "contentinit".
-            # manage_addContentType() can then grab it.
-            constructors=(manage_addContentForm, manage_addContent,
-                          self) + self.extra_constructors,
-            permission=self.permission,
-            visibility=self.visibility)
+        # We add self to the FactoryDispatcher under the name 'contentinit'.
+        # manage_addContentType() can then grab it.
+        try:
+            context.registerClass(
+                meta_type=self.meta_type,
+                constructors=(
+                    manage_addContentForm,
+                    manage_addContent,
+                    ) + self.extra_constructors,
+                resources=(self, ),
+                permission=self.permission,
+                visibility=self.visibility)
+        except TypeError:
+            # The 'resources' keyword was only introduced after Zope 5.9.
+            context.registerClass(
+                meta_type=self.meta_type,
+                constructors=(
+                    manage_addContentForm, manage_addContent, self,
+                    ) + self.extra_constructors,
+                permission=self.permission,
+                visibility=self.visibility)
 
         for ct in self.content_types:
             ct.__factory_meta_type__ = self.meta_type
 
 
 InitializeClass(ContentInit)
```

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/www/cpsDiff.pt` & `Products.CMFCore-3.5/src/Products/CMFCore/www/cpsDiff.pt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/www/typeinfoAliases.zpt` & `Products.CMFCore-3.5/src/Products/CMFCore/www/typeinfoAliases.zpt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/www/typesAliases.zpt` & `Products.CMFCore-3.5/src/Products/CMFCore/www/typesAliases.zpt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products/CMFCore/zcml.py` & `Products.CMFCore-3.5/src/Products/CMFCore/zcml.py`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/src/Products.CMFCore.egg-info/PKG-INFO` & `Products.CMFCore-3.5/src/Products.CMFCore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.CMFCore
-Version: 3.4
+Version: 3.5
 Summary: Zope Content Management Framework core components
 Home-page: https://github.com/zopefoundation/Products.CMFCore
 Author: Zope Foundation and Contributors
 Author-email: zope-cmf@zope.org
 License: ZPL 2.1
 Project-URL: Documentation, https://zope.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Products.CMFCore/issues
@@ -58,27 +58,35 @@
 
 
 ------------------------------------------------------------
 
 Products.CMFCore Changelog
 ==========================
 
+3.5 (2024-03-23)
+----------------
+
+- Use the new ``resources`` keyword of ``registerClass`` if available.
+  This avoids a deprecation warning for using a non callable constructor in Zope higher than 5.9.
+  (`#1202 <https://github.com/zopefoundation/Zope/issues/1202>`_)
+
+
 3.4 (2024-04-12)
 ----------------
 
 - Add i18n translation support.
   (`#135 <https://github.com/zopefoundation/Products.CMFCore/issues/135>`_)
 
 
 3.3 (2024-01-23)
 ----------------
 
 - Add support for Python 3.12.
 
-- ZMI: added limit of folderish objects for customizing and 
+- ZMI: added limit of folderish objects for customizing and
   handling SVG files as FSImage showing a preview.
   (`#130 <https://github.com/zopefoundation/Products.CMFCore/pull/130>`_)
 
 
 3.2 (2023-07-03)
 ----------------
```

### Comparing `Products.CMFCore-3.4/src/Products.CMFCore.egg-info/SOURCES.txt` & `Products.CMFCore-3.5/src/Products.CMFCore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.CMFCore-3.4/tox.ini` & `Products.CMFCore-3.5/tox.ini`

 * *Files identical despite different names*

