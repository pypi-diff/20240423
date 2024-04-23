# Comparing `tmp/LbAdmin-0.0.8.tar.gz` & `tmp/LbAdmin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "public/lbadmin/LbAdmin-0.0.8.tar", last modified: Wed Jan 15 15:23:03 2020, max compression
+gzip compressed data, was "public/LbAdmin-0.0.9.tar", last modified: Fri Aug 28 09:29:44 2020, max compression
```

## Comparing `LbAdmin-0.0.8.tar` & `LbAdmin-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1445 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin/
--rw-rw-rw-   0 root         (0) root         (0)     2606 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/LbAdmin/ProjectDataExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3316 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/LbAdmin/CreateAllSpecs.py
--rwxrwxrwx   0 root         (0) root         (0)     6542 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/LbAdmin/LbDeploymentUpdateSdb.py
--rw-rw-rw-   0 root         (0) root         (0)    11237 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/LbAdmin/CreateLHCbLCGMetaSpec.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/LbAdmin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7289 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/LbAdmin/RpmRelease.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1445 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       44 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-01-15 15:22:39.000000 LbAdmin-0.0.8/LbAdmin.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      434 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      362 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        8 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/LbAdmin.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1366 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       57 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      151 2020-01-15 15:23:03.000000 LbAdmin-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     7543 2020-01-15 15:22:32.000000 LbAdmin-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1458 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)    32472 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin/
+-rw-rw-rw-   0 root         (0) root         (0)     3316 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/LbAdmin/CreateAllSpecs.py
+-rw-rw-rw-   0 root         (0) root         (0)    11275 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/LbAdmin/CreateLHCbLCGMetaSpec.py
+-rwxrwxrwx   0 root         (0) root         (0)     6542 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/LbAdmin/LbDeploymentUpdateSdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/LbAdmin/ProjectDataExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7289 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/LbAdmin/RpmRelease.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/LbAdmin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1445 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      442 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      362 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/LbAdmin.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1445 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      518 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      151 2020-08-28 09:29:44.000000 LbAdmin-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     7543 2020-08-28 09:29:41.000000 LbAdmin-0.0.9/setup.py
```

### Comparing `LbAdmin-0.0.8/PKG-INFO` & `LbAdmin-0.0.9/LbAdmin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: LbAdmin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Administration tools for the LHCb environment and software
 Home-page: https://gitlab.cern.ch/lhcb-core/LbAdmin
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: GPLv3+
 Description: LHCb Admin tools 
         ====================================
```

### Comparing `LbAdmin-0.0.8/LbAdmin/ProjectDataExporter.py` & `LbAdmin-0.0.9/LbAdmin/ProjectDataExporter.py`

 * *Files identical despite different names*

### Comparing `LbAdmin-0.0.8/LbAdmin/CreateAllSpecs.py` & `LbAdmin-0.0.9/LbAdmin/CreateAllSpecs.py`

 * *Files identical despite different names*

### Comparing `LbAdmin-0.0.8/LbAdmin/LbDeploymentUpdateSdb.py` & `LbAdmin-0.0.9/LbAdmin/LbDeploymentUpdateSdb.py`

 * *Files identical despite different names*

### Comparing `LbAdmin-0.0.8/LbAdmin/CreateLHCbLCGMetaSpec.py` & `LbAdmin-0.0.9/LbAdmin/CreateLHCbLCGMetaSpec.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,17 +81,19 @@
             lhcb_installer = Installer(self.siteroot)
         if self.packages is None:
             self.packages = set([p.name for p in lhcb_installer.remoteListPackages('LCG_%s_' % self.lcgVersion)])
 
     def find(self, package):
         self.setup()
         extName = "^%s.*$" % buildLCGName(self.lcgVersion, package,".*", self.cmtconfig.replace("-", "_"))
+        plist = []
         for p in self.packages:
             if re.match(extName, p):
-                return p
+                plist.append(p)
+        return plist
 
     def check(self, package, version):
         self.setup()
         extName = buildLCGName(self.lcgVersion, package, version, self.cmtconfig.replace("-", "_"))
         return extName in self.packages
 
 def buildLCGName(lcgVersion, package, version, cmtconfig):
@@ -107,19 +109,19 @@
 
     found = []
     missing = []
 
     # Looking up the versions of packages specified without version first
     for package in externals_list:
         res = vf.find(package)
-        if res is None:
+        if not res:
             missing.append(package)
             log.warning("Could not find package %s in LCG %s %s" % (package, lcgVer, cmtconfig))
         else:
-            found.append(res)
+            found += res
 
     # Checking if the packages specified with version are correct
     for (package, version) in external_versions_list:
         if not vf.check(package, version):
             missing.append(package)
             log.warning("Could not find package %s %s in LCG %s %s" % (package, version, lcgVer, cmtconfig))
         else:
```

### Comparing `LbAdmin-0.0.8/LbAdmin/RpmRelease.py` & `LbAdmin-0.0.9/LbAdmin/RpmRelease.py`

 * *Files identical despite different names*

### Comparing `LbAdmin-0.0.8/README.rst` & `LbAdmin-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `LbAdmin-0.0.8/LbAdmin.egg-info/PKG-INFO` & `LbAdmin-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: LbAdmin
-Version: 0.0.8
+Version: 0.0.9
 Summary: Administration tools for the LHCb environment and software
 Home-page: https://gitlab.cern.ch/lhcb-core/LbAdmin
 Author: CERN - LHCb Core Software
 Author-email: lhcb-core-soft@cern.ch
 License: GPLv3+
 Description: LHCb Admin tools 
         ====================================
```

### Comparing `LbAdmin-0.0.8/.gitlab-ci.yml` & `LbAdmin-0.0.9/.gitlab-ci.yml`

 * *Files 10% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 
 # see https://gitlab.cern.ch/gitlabci-examples/deploy_eos for the details
 # of the configuration
 deploy-packages:
   stage: deploy
   only:
     - tags
-  dependencies:
-    - python2.7
+  dependencies: []
   image: gitlab-registry.cern.ch/lhcb-docker/python-deployment:python-3.7
   script:
+    - python setup.py sdist --dist-dir public/     
+    - python setup.py bdist_wheel --dist-dir public/
     - if [ -z "$TWINE_PASSWORD" ] ; then echo "Set TWINE_PASSWORD in CI variables" ; exit 1 ; fi
     - twine upload -u __token__ public/*
   before_script: []
   after_script: []
```

### Comparing `LbAdmin-0.0.8/setup.py` & `LbAdmin-0.0.9/setup.py`

 * *Files identical despite different names*

