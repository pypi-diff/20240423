# Comparing `tmp/collective.MockMailHost-2.0.0.tar.gz` & `tmp/collective.MockMailHost-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/collective.MockMailHost-2.0.0.tar", last modified: Tue Nov  6 08:12:02 2018, max compression
+gzip compressed data, was "collective.MockMailHost-3.0.0.tar", last modified: Tue Apr 23 16:22:27 2024, max compression
```

## Comparing `collective.MockMailHost-2.0.0.tar` & `collective.MockMailHost-3.0.0.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/
--rw-r--r--   0 maurits    (502) staff       (20)     8301 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/PKG-INFO
--rw-r--r--   0 maurits    (502) staff       (20)       38 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/requirements.txt
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/collective/
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/
--rw-r--r--   0 maurits    (502) staff       (20)      674 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/configure.zcml
--rw-r--r--   0 maurits    (502) staff       (20)       99 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/config.py
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/tests/
--rw-r--r--   0 maurits    (502) staff       (20)     1481 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/tests/SendEmail.txt
--rw-r--r--   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/tests/__init__.py
--rw-r--r--   0 maurits    (502) staff       (20)      697 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/tests/testFunctional.py
--rw-r--r--   0 maurits    (502) staff       (20)      311 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/__init__.py
--rw-r--r--   0 maurits    (502) staff       (20)      537 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/setuphandlers.py
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/browser/
--rw-r--r--   0 maurits    (502) staff       (20)      281 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/browser/configure.zcml
--rw-r--r--   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/browser/__init__.py
--rw-r--r--   0 maurits    (502) staff       (20)      255 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/browser/views.py
--rw-r--r--   0 maurits    (502) staff       (20)      896 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/MailHost_icon.gif
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/profiles/
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/profiles/default/
--rw-r--r--   0 maurits    (502) staff       (20)      154 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/profiles/default/toolset.xml
--rw-r--r--   0 maurits    (502) staff       (20)      393 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/profiles/default/import_steps.xml
--rw-r--r--   0 maurits    (502) staff       (20)       30 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/profiles/default/mockmailhost_various.txt
--rw-r--r--   0 maurits    (502) staff       (20)        9 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/version.txt
--rw-r--r--   0 maurits    (502) staff       (20)     1057 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/testing.py
--rw-r--r--   0 maurits    (502) staff       (20)     1717 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/MockMailHost/MockMailHost.py
--rw-r--r--   0 maurits    (502) staff       (20)      244 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/collective/__init__.py
--rw-r--r--   0 maurits    (502) staff       (20)      352 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/buildout.cfg
--rw-r--r--   0 maurits    (502) staff       (20)       87 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/MANIFEST.in
--rw-r--r--   0 maurits    (502) staff       (20)      119 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/.coveragerc
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/docs/
--rw-r--r--   0 maurits    (502) staff       (20)    17987 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (502) staff       (20)      740 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (502) staff       (20)     1555 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/setup.py
--rw-r--r--   0 maurits    (502) staff       (20)      118 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/.gitignore
-drwxr-xr-x   0 maurits    (502) staff       (20)        0 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/
--rw-r--r--   0 maurits    (502) staff       (20)     8301 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (502) staff       (20)        1 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (502) staff       (20)       11 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (502) staff       (20)     1307 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (502) staff       (20)       82 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (502) staff       (20)      123 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/requires.txt
--rw-r--r--   0 maurits    (502) staff       (20)       11 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/top_level.txt
--rw-r--r--   0 maurits    (502) staff       (20)        1 2018-11-06 08:12:01.000000 collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (502) staff       (20)      103 2018-11-06 08:12:02.000000 collective.MockMailHost-2.0.0/setup.cfg
--rw-r--r--   0 maurits    (502) staff       (20)     2392 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/README.rst
--rw-r--r--   0 maurits    (502) staff       (20)     1818 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/CHANGES.rst
--rw-r--r--   0 maurits    (502) staff       (20)      267 2018-11-06 08:12:00.000000 collective.MockMailHost-2.0.0/.travis.yml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.087964 collective.MockMailHost-3.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/.coveragerc
+-rw-r--r--   0 maurits    (501) staff       (20)      198 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)     2178 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       87 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     8308 2024-04-23 16:22:27.088191 collective.MockMailHost-3.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2392 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1203 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/base.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.079294 collective.MockMailHost-3.0.0/collective/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.084221 collective.MockMailHost-3.0.0/collective/MockMailHost/
+-rw-r--r--   0 maurits    (501) staff       (20)      896 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/MailHost_icon.gif
+-rw-r--r--   0 maurits    (501) staff       (20)     1887 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/MockMailHost.py
+-rw-r--r--   0 maurits    (501) staff       (20)      312 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.085045 collective.MockMailHost-3.0.0/collective/MockMailHost/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      281 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      255 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/browser/views.py
+-rw-r--r--   0 maurits    (501) staff       (20)       99 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/config.py
+-rw-r--r--   0 maurits    (501) staff       (20)      674 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.073649 collective.MockMailHost-3.0.0/collective/MockMailHost/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.085945 collective.MockMailHost-3.0.0/collective/MockMailHost/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/profiles/default/import_steps.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/profiles/default/mockmailhost_various.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      154 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/profiles/default/toolset.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      537 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/setuphandlers.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1064 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.086889 collective.MockMailHost-3.0.0/collective/MockMailHost/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)     2895 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/tests/SendEmail.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1000 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/tests/testFunctional.py
+-rw-r--r--   0 maurits    (501) staff       (20)        9 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/MockMailHost/version.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      244 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/collective/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.081752 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     8308 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1390 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      123 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2024-04-23 16:22:27.000000 collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-23 16:22:27.087634 collective.MockMailHost-3.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      740 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/docs/LICENSE.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      241 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/plone-5.2.x.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      206 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/plone-6.0.x.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       62 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/requirements-5.2.x.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       61 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/requirements-6.0.x.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      103 2024-04-23 16:22:27.088850 collective.MockMailHost-3.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1789 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      790 2024-04-23 16:22:26.000000 collective.MockMailHost-3.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `collective.MockMailHost-2.0.0/PKG-INFO` & `collective.MockMailHost-3.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,264 +1,326 @@
 Metadata-Version: 2.1
 Name: collective.MockMailHost
-Version: 2.0.0
+Version: 3.0.0
 Summary: Used for integration testing with Plone
 Home-page: https://github.com/collective/collective.mockmailhost
 Author: Suresh V.
 Author-email: suresh@grafware.com
 License: GPL
-Description: Introduction
-        ============
-        
-        ``collective.MockMailHost`` enables integration testing of email functionality
-        from Plone_. Simply add this egg to your [test] runner section, and install
-        this product through your ``Layer`` or ``TestCase``.
-        
-        Note
-          THIS IS FOR TESTING PURPOSE ONLY, do not use this product on your
-          running Plone site. It replaces the standard MailHost with a Mock
-          MailHost that you can poke at to check email content and recipients.
-        
-        Has been tested with Plone 4 but should also work with earlier versions.
-        
-        
-        Integration
-        -----------
-        
-        Example how to integrate ``collective.MockMailHost`` to your testing setup
-        based on `plone.app.testing`_. Add the package to your extras_requires section
-        in your package's ``setup.py`` file, so buildout will automatically download
-        the package for you.::
-        
-            setup(name='my.package',
-                  ...
-                  extras_require={
-                    'test': [
-                        'plone.app.testing',
-                        'collective.MockMailHost',
-                    ]
-                  },
-                  ...
-                  )
-        
-        Your test layer setup could look like this example below::
-        
-            from plone.app.testing import helpers, layers
-            from plone.testing import z2
-        
-        
-            class MyLayer(helpers.PloneSandboxLayer):
-                defaultBases = (layers.PLONE_FIXTURE, )
-        
-                def setUpZope(self, app, configurationContext):
-                    # Load zcml
-                    import collective.MockMailHost
-                    self.loadZCML(package=collective.MockMailHost)
-        
-                    # Install product and call its initialize() function
-                    z2.installProduct(app, 'collective.MockMailHost')
-        
-                    # Note: you can skip this if my.product is not a Zope 2-style
-                    # product, i.e. it is not in the Products.* namespace and it
-                    # does not have a <five:registerPackage /> directive in its
-                    # configure.zcml.
-        
-                def tearDownZope(self, app):
-                    # Uninstall product
-                    z2.uninstallProduct(app, 'collective.MockMailHost')
-        
-                    # Note: Again, you can skip this if my.product is not a Zope 2-
-                    # style product
-        
-                def setUpPloneSite(self, portal):
-                    helpers.quickInstallProduct(portal, 'collective.MockMailHost')
-        
-                    helpers.applyProfile(portal, 'collective.MockMailHost:default')
-        
-            MY_FIXTURE = MyLayer()
-        
-        .. _Plone: http://plone.org
-        .. _`plone.app.testing`: http://pypi.python.org/pypi/plone.app.testing
-        
-        Using a member-posting forum
-        ============================
-        
-            >>> from Products.CMFCore.utils import getToolByName
-            >>> from Products.MailHost.interfaces import IMailHost
-            >>> from zope.component import getUtility
-        
-            >>> app = layer['app']
-            >>> portal = layer['portal']
-        
-        Test starting conversations, replying and modifying comments in a default
-        member-posting forum.
-        
-        Let us log all exceptions, which is useful for debugging. Also, clear portlet
-        slots, to make the test browser less confused by things like the recent portlet
-        and the navtree.
-        
-            >>> portal.error_log._ignored_exceptions = ()
-            >>> portal.left_slots = portal.right_slots = []
-            >>> workflow = portal.portal_workflow
-        
-        Validate mailhost replacement
-        -----------------------------
-        
-            >>> portal.MailHost
-            <MockMailHost at ...>
-        
-            >>> getToolByName(portal, 'MailHost')
-            <MockMailHost at ...>
-        
-            >>> getUtility(IMailHost)
-            <MockMailHost at ...>
-        
-        
-        Send email
-        ----------
-        
-            >>> to_ = "member@example.com"
-            >>> from_ = "admin@example.com"
-            >>> msg = """
-            ...
-            ... Dear Sir:
-            ...
-            ... Thank you"""
-            >>> portal.MailHost.send(msg, to_, from_)
-            >>> len(portal.MailHost.messages)
-            1
-            >>> 'To: member@example.com' in portal.MailHost.messages[0]
-            True
-            >>> 'From: admin@example.com' in portal.MailHost.messages[0]
-            True
-            >>> 'Dear Sir:' in portal.MailHost.messages[0]
-            True
-            >>> portal.MailHost.reset()
-            >>> len(portal.MailHost.messages)
-            0
-        
-        
-        Changelog
-        =========
-        
-        2.0.0 (2018-11-06)
-        ------------------
-        
-        Breaking changes:
-        
-        - Do not depend on old SecureMailHost any longer.
-          [pbauer]
-        
-        New features:
-        
-        - Python 3 support.
-          [pbauer]
-        
-        
-        1.1.0 (2018-06-27)
-        ------------------
-        
-        - Fix import location, Globals has been removed.
-          [gforcada]
-        
-        - Rework tests setup.
-          [gforcada]
-        
-        
-        1.0 (2016-01-25)
-        ----------------
-        
-        - Fix MIMEText compatibility (broken since 0.9).
-          [jone]
-        
-        
-        0.9 (2015-07-10)
-        ----------------
-        
-        - Clean up msg before sending. Otherwise Plone self registration
-          email does not work [sureshvv]
-        
-        
-        0.8 (2015-06-13)
-        ----------------
-        
-        - Add browser view for functional testing [Casecarsid]
-        
-        
-        0.7 (2013-07-05)
-        ----------------
-        
-        - MANIFEST [sureshvv]
-        
-        
-        0.6 (2013-07-03)
-        ----------------
-        
-        - Track msg_type also.
-          [sureshvv]
-        
-        - Behave more like ``collective.testcaselayer``'s MockMailHost.
-          [saily]
-        
-        - Documentation updates
-          [saily]
-        
-        
-        0.5 - 2012-09-25
-        ----------------
-        
-        - Remove ZopeSkel and Paster dependency from setup.py
-          [saily]
-        
-        - Moved to github and changed to README.rst, links in setup.py
-          [saily]
-        
-        - Allow multiple paramters for ``send`` and ``secureSend`` method in
-          MockMailHost class.  [saily]
-        
-        
-        0.4 (2011-05-17)
-        ----------------
-        
-        - Register MockMailHost in SiteManager to get MockMailHost when using
-          ``getToolByName(context, 'MailHost')`` or ``getUtility(IMailHost)``.
-          [saily]
-        
-        - Inherit from MailHost instead of SimpleItem
-          [saily]
-        
-        - Implement the secureSend method
-          [saily]
-        
-        
-        0.3 (2011-04-04)
-        ----------------
-        
-        - Add ``**kwargs`` to MockMailHost's send method to support mto, mfrom, ...
-          keyword arguments as default MailHost does.  [saily]
-        
-        - Added file for generic setup various handlers
-          [sureshvv]
-        
-        
-        0.2 (2010-05-21)
-        ----------------
-        
-        - Added tests
-          [sureshvv]
-        
-        
-        0.1 (2010-05-16)
-        ----------------
-        
-        - Initial release
-          [sureshvv]
-        
 Keywords: mock mailhost tests
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Provides-Extra: test
+
+Introduction
+============
+
+``collective.MockMailHost`` enables integration testing of email functionality
+from Plone_. Simply add this egg to your [test] runner section, and install
+this product through your ``Layer`` or ``TestCase``.
+
+Note
+  THIS IS FOR TESTING PURPOSE ONLY, do not use this product on your
+  running Plone site. It replaces the standard MailHost with a Mock
+  MailHost that you can poke at to check email content and recipients.
+
+Has been tested with Plone 4 but should also work with earlier versions.
+
+
+Integration
+-----------
+
+Example how to integrate ``collective.MockMailHost`` to your testing setup
+based on `plone.app.testing`_. Add the package to your extras_requires section
+in your package's ``setup.py`` file, so buildout will automatically download
+the package for you.::
+
+    setup(name='my.package',
+          ...
+          extras_require={
+            'test': [
+                'plone.app.testing',
+                'collective.MockMailHost',
+            ]
+          },
+          ...
+          )
+
+Your test layer setup could look like this example below::
+
+    from plone.app.testing import helpers, layers
+    from plone.testing import z2
+
+
+    class MyLayer(helpers.PloneSandboxLayer):
+        defaultBases = (layers.PLONE_FIXTURE, )
+
+        def setUpZope(self, app, configurationContext):
+            # Load zcml
+            import collective.MockMailHost
+            self.loadZCML(package=collective.MockMailHost)
+
+            # Install product and call its initialize() function
+            z2.installProduct(app, 'collective.MockMailHost')
+
+            # Note: you can skip this if my.product is not a Zope 2-style
+            # product, i.e. it is not in the Products.* namespace and it
+            # does not have a <five:registerPackage /> directive in its
+            # configure.zcml.
+
+        def tearDownZope(self, app):
+            # Uninstall product
+            z2.uninstallProduct(app, 'collective.MockMailHost')
+
+            # Note: Again, you can skip this if my.product is not a Zope 2-
+            # style product
+
+        def setUpPloneSite(self, portal):
+            helpers.quickInstallProduct(portal, 'collective.MockMailHost')
+
+            helpers.applyProfile(portal, 'collective.MockMailHost:default')
+
+    MY_FIXTURE = MyLayer()
+
+.. _Plone: http://plone.org
+.. _`plone.app.testing`: http://pypi.python.org/pypi/plone.app.testing
+
+Using a member-posting forum
+============================
+
+    >>> from Products.CMFCore.utils import getToolByName
+    >>> from Products.MailHost.interfaces import IMailHost
+    >>> from zope.component import getUtility
+
+    >>> app = layer['app']
+    >>> portal = layer['portal']
+
+Test starting conversations, replying and modifying comments in a default
+member-posting forum.
+
+Let us log all exceptions, which is useful for debugging. Also, clear portlet
+slots, to make the test browser less confused by things like the recent portlet
+and the navtree.
+
+    >>> portal.error_log._ignored_exceptions = ()
+    >>> portal.left_slots = portal.right_slots = []
+    >>> workflow = portal.portal_workflow
+
+Validate mailhost replacement
+-----------------------------
+
+    >>> portal.MailHost
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
+
+    >>> getToolByName(portal, 'MailHost')
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
+
+    >>> getUtility(IMailHost)
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
+
+
+Send email
+----------
+
+    >>> to_ = "member@example.com"
+    >>> from_ = "admin@example.com"
+    >>> msg = """
+    ...
+    ... Dear Sir:
+    ...
+    ... Thank you"""
+    >>> portal.MailHost.send(msg, to_, from_)
+    >>> len(portal.MailHost.messages)
+    1
+    >>> b'To: member@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'From: admin@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'Dear Sir:' in portal.MailHost.messages[0]
+    True
+    >>> portal.MailHost.messages_from
+    ['admin@example.com']
+    >>> portal.MailHost.messages_to
+    [['member@example.com']]
+    >>> portal.MailHost.reset()
+    >>> len(portal.MailHost.messages)
+    0
+
+Send an `email.message.EmailMessage` object with cc/bcc recipients
+
+    >>> from email.message import EmailMessage
+    >>> msg = EmailMessage()
+    >>> msg["Subject"] = "Hello"
+    >>> msg["From"] = "me@example.com"
+    >>> msg["To"] = "you@example.com"
+    >>> msg["Cc"] = "foo@example.com"
+    >>> msg["Bcc"] = "bar@example.com"
+    >>> msg.set_content("""
+    ... This message is for you, foo, and bar.
+    ... """)
+    >>> portal.MailHost.send(msg)
+    >>> len(portal.MailHost.messages)
+    1
+    >>> b'To: you@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'From: me@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'Cc: foo@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'bar@example.com' in portal.MailHost.messages[0]
+    False
+    >>> b'This message is for you, foo, and bar.' in portal.MailHost.messages[0]
+    True
+    >>> len(portal.MailHost.messages)
+    1
+    >>> portal.MailHost.messages_from
+    ['me@example.com']
+    >>> portal.MailHost.messages_to
+    [['you@example.com', 'foo@example.com', 'bar@example.com']]
+    >>> portal.MailHost.reset()
+    >>> len(portal.MailHost.messages)
+    0
+
+Changelog
+=========
+
+3.0.0 (2024-04-23)
+------------------
+
+Breaking changes:
+
+- Remove support for Python versions prior to 3.7 and Plone versions
+  prior to 5.2.
+  [mamico]
+
+New features:
+
+- Add `messages_from`, and `messages_to` to record senders and recipients.
+  This is useful for testing `bcc` that is not present in the message.
+  [mamico]
+
+Bug fixes:
+
+- *add item here*
+
+
+2.0.0 (2018-11-06)
+------------------
+
+Breaking changes:
+
+- Do not depend on old SecureMailHost any longer.
+  [pbauer]
+
+New features:
+
+- Python 3 support.
+  [pbauer]
+
+
+1.1.0 (2018-06-27)
+------------------
+
+- Fix import location, Globals has been removed.
+  [gforcada]
+
+- Rework tests setup.
+  [gforcada]
+
+
+1.0 (2016-01-25)
+----------------
+
+- Fix MIMEText compatibility (broken since 0.9).
+  [jone]
+
+
+0.9 (2015-07-10)
+----------------
+
+- Clean up msg before sending. Otherwise Plone self registration
+  email does not work [sureshvv]
+
+
+0.8 (2015-06-13)
+----------------
+
+- Add browser view for functional testing [Casecarsid]
+
+
+0.7 (2013-07-05)
+----------------
+
+- MANIFEST [sureshvv]
+
+
+0.6 (2013-07-03)
+----------------
+
+- Track msg_type also.
+  [sureshvv]
+
+- Behave more like ``collective.testcaselayer``'s MockMailHost.
+  [saily]
+
+- Documentation updates
+  [saily]
+
+
+0.5 - 2012-09-25
+----------------
+
+- Remove ZopeSkel and Paster dependency from setup.py
+  [saily]
+
+- Moved to github and changed to README.rst, links in setup.py
+  [saily]
+
+- Allow multiple paramters for ``send`` and ``secureSend`` method in
+  MockMailHost class.  [saily]
+
+
+0.4 (2011-05-17)
+----------------
+
+- Register MockMailHost in SiteManager to get MockMailHost when using
+  ``getToolByName(context, 'MailHost')`` or ``getUtility(IMailHost)``.
+  [saily]
+
+- Inherit from MailHost instead of SimpleItem
+  [saily]
+
+- Implement the secureSend method
+  [saily]
+
+
+0.3 (2011-04-04)
+----------------
+
+- Add ``**kwargs`` to MockMailHost's send method to support mto, mfrom, ...
+  keyword arguments as default MailHost does.  [saily]
+
+- Added file for generic setup various handlers
+  [sureshvv]
+
+
+0.2 (2010-05-21)
+----------------
+
+- Added tests
+  [sureshvv]
+
+
+0.1 (2010-05-16)
+----------------
+
+- Initial release
+  [sureshvv]
```

### Comparing `collective.MockMailHost-2.0.0/collective/MockMailHost/configure.zcml` & `collective.MockMailHost-3.0.0/collective/MockMailHost/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.MockMailHost-2.0.0/collective/MockMailHost/tests/SendEmail.txt` & `collective.MockMailHost-3.0.0/collective/MockMailHost/tests/SendEmail.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     >>> portal.left_slots = portal.right_slots = []
     >>> workflow = portal.portal_workflow
 
 Validate mailhost replacement
 -----------------------------
 
     >>> portal.MailHost
-    <MockMailHost at ...>
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
 
     >>> getToolByName(portal, 'MailHost')
-    <MockMailHost at ...>
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
 
     >>> getUtility(IMailHost)
-    <MockMailHost at ...>
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
 
 
 Send email
 ----------
 
     >>> to_ = "member@example.com"
     >>> from_ = "admin@example.com"
@@ -41,17 +41,55 @@
     ...
     ... Dear Sir:
     ...
     ... Thank you"""
     >>> portal.MailHost.send(msg, to_, from_)
     >>> len(portal.MailHost.messages)
     1
-    >>> 'To: member@example.com' in portal.MailHost.messages[0]
+    >>> b'To: member@example.com' in portal.MailHost.messages[0]
     True
-    >>> 'From: admin@example.com' in portal.MailHost.messages[0]
+    >>> b'From: admin@example.com' in portal.MailHost.messages[0]
     True
-    >>> 'Dear Sir:' in portal.MailHost.messages[0]
+    >>> b'Dear Sir:' in portal.MailHost.messages[0]
     True
+    >>> portal.MailHost.messages_from
+    ['admin@example.com']
+    >>> portal.MailHost.messages_to
+    [['member@example.com']]
     >>> portal.MailHost.reset()
     >>> len(portal.MailHost.messages)
     0
 
+Send an `email.message.EmailMessage` object with cc/bcc recipients
+
+    >>> from email.message import EmailMessage
+    >>> msg = EmailMessage()
+    >>> msg["Subject"] = "Hello"
+    >>> msg["From"] = "me@example.com"
+    >>> msg["To"] = "you@example.com"
+    >>> msg["Cc"] = "foo@example.com"
+    >>> msg["Bcc"] = "bar@example.com"
+    >>> msg.set_content("""
+    ... This message is for you, foo, and bar.
+    ... """)
+    >>> portal.MailHost.send(msg)
+    >>> len(portal.MailHost.messages)
+    1
+    >>> b'To: you@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'From: me@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'Cc: foo@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'bar@example.com' in portal.MailHost.messages[0]
+    False
+    >>> b'This message is for you, foo, and bar.' in portal.MailHost.messages[0]
+    True
+    >>> len(portal.MailHost.messages)
+    1
+    >>> portal.MailHost.messages_from
+    ['me@example.com']
+    >>> portal.MailHost.messages_to
+    [['you@example.com', 'foo@example.com', 'bar@example.com']]
+    >>> portal.MailHost.reset()
+    >>> len(portal.MailHost.messages)
+    0
```

### Comparing `collective.MockMailHost-2.0.0/collective/MockMailHost/setuphandlers.py` & `collective.MockMailHost-3.0.0/collective/MockMailHost/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.MockMailHost-2.0.0/collective/MockMailHost/MailHost_icon.gif` & `collective.MockMailHost-3.0.0/collective/MockMailHost/MailHost_icon.gif`

 * *Files identical despite different names*

### Comparing `collective.MockMailHost-2.0.0/collective/MockMailHost/testing.py` & `collective.MockMailHost-3.0.0/collective/MockMailHost/testing.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 import doctest
 
 
 class CollectiveMockMailHostLayer(PloneSandboxLayer):
 
     def setUpZope(self, app, configurationContext):
         import collective.MockMailHost
+
         self.loadZCML(package=collective.MockMailHost)
 
     def setUpPloneSite(self, portal):
-        applyProfile(portal, 'collective.MockMailHost:default')
+        applyProfile(portal, "collective.MockMailHost:default")
+
 
 COLLECTIVE_MOCKMAILHOST_FIXTURE = CollectiveMockMailHostLayer()
 
 COLLECTIVE_MOCKMAILHOST_INTEGRATION_TESTING = IntegrationTesting(
-    bases=(COLLECTIVE_MOCKMAILHOST_FIXTURE, ),
-    name='CollectiveMockMailHostLayer:Integration'
+    bases=(COLLECTIVE_MOCKMAILHOST_FIXTURE,),
+    name="CollectiveMockMailHostLayer:Integration",
 )
 COLLECTIVE_MOCKMAILHOST_FUNCTIONAL_TESTING = FunctionalTesting(
-    bases=(COLLECTIVE_MOCKMAILHOST_FIXTURE, ),
-    name='CollectiveMockMailHostLayer:Functional'
+    bases=(COLLECTIVE_MOCKMAILHOST_FIXTURE,),
+    name="CollectiveMockMailHostLayer:Functional",
 )
 
 optionflags = (
-    doctest.REPORT_ONLY_FIRST_FAILURE
-    | doctest.ELLIPSIS
-    | doctest.NORMALIZE_WHITESPACE
+    doctest.REPORT_ONLY_FIRST_FAILURE | doctest.ELLIPSIS | doctest.NORMALIZE_WHITESPACE  # noqa E501
 )
```

### Comparing `collective.MockMailHost-2.0.0/collective/MockMailHost/MockMailHost.py` & `collective.MockMailHost-3.0.0/collective/MockMailHost/MockMailHost.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,26 +14,30 @@
 
     def __init__(self, id=''):
         super(MockMailHost, self).__init__(id)
         self.reset()
 
     def reset(self):
         self.messages = []
+        self.messages_from = []
+        self.messages_to = []
         self.msg_types = []
         self._p_changed = True
 
     def _send(self, mfrom, mto, messageText, debug=False):
         if isinstance(messageText, email.message.Message):
             if six.PY2:
                 message = messageText.as_string()
             else:
                 message = email.message_from_string(messageText)
         else:
             message = messageText
         self.messages.append(message)
+        self.messages_from.append(mfrom)
+        self.messages_to.append(mto)
         self._p_changed = True
 
     def send(self,
              messageText,
              mto=None,
              mfrom=None,
              subject=None,
@@ -42,15 +46,17 @@
              charset=None,
              msg_type=None,
              ):
 
         # messageText may be an MIMEText object, or something else.
         # We onyl want to clean it up if it is a string.
         if isinstance(messageText, (str, six.text_type)):
-            messageText = '\n'.join([x.strip() for x in messageText.split('\n')])
+            messageText = '\n'.join([
+                x.strip() for x in messageText.split('\n')
+            ])
 
         self.msg_types.append(msg_type)
         super(MockMailHost, self).send(messageText, mto, mfrom,
                                        subject, encode, immediate, charset,
                                        msg_type)
 
     def pop(self, idx=-1):
```

### Comparing `collective.MockMailHost-2.0.0/docs/LICENSE.GPL` & `collective.MockMailHost-3.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.MockMailHost-2.0.0/docs/LICENSE.txt` & `collective.MockMailHost-3.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.MockMailHost-2.0.0/setup.py` & `collective.MockMailHost-3.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 from setuptools import setup, find_packages
 import os
 
-version = '2.0.0'
+version = '3.0.0'
 
 setup(
     name='collective.MockMailHost',
     version=version,
     description="Used for integration testing with Plone",
     long_description="\n".join([
         open("README.rst").read(),
         open(os.path.join("collective", "MockMailHost", "tests",
                           "SendEmail.txt")).read(),
         open("CHANGES.rst").read(),
     ]),
     # Get more strings from https://pypi.org/classifiers
     classifiers=[
+        "Development Status :: 5 - Production/Stable",
         "Framework :: Plone",
         "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords='mock mailhost tests',
     author='Suresh V.',
     author_email='suresh@grafware.com',
     url='https://github.com/collective/collective.mockmailhost',
     license='GPL',
     packages=find_packages(exclude=['ez_setup']),
     namespace_packages=['collective'],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.7",
     install_requires=[
       'setuptools',
       'Products.GenericSetup',
       'Products.MailHost',
       'Products.CMFCore',
       # -*- Extra requirements: -*-
     ],
```

### Comparing `collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/PKG-INFO` & `collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,264 +1,326 @@
 Metadata-Version: 2.1
 Name: collective.MockMailHost
-Version: 2.0.0
+Version: 3.0.0
 Summary: Used for integration testing with Plone
 Home-page: https://github.com/collective/collective.mockmailhost
 Author: Suresh V.
 Author-email: suresh@grafware.com
 License: GPL
-Description: Introduction
-        ============
-        
-        ``collective.MockMailHost`` enables integration testing of email functionality
-        from Plone_. Simply add this egg to your [test] runner section, and install
-        this product through your ``Layer`` or ``TestCase``.
-        
-        Note
-          THIS IS FOR TESTING PURPOSE ONLY, do not use this product on your
-          running Plone site. It replaces the standard MailHost with a Mock
-          MailHost that you can poke at to check email content and recipients.
-        
-        Has been tested with Plone 4 but should also work with earlier versions.
-        
-        
-        Integration
-        -----------
-        
-        Example how to integrate ``collective.MockMailHost`` to your testing setup
-        based on `plone.app.testing`_. Add the package to your extras_requires section
-        in your package's ``setup.py`` file, so buildout will automatically download
-        the package for you.::
-        
-            setup(name='my.package',
-                  ...
-                  extras_require={
-                    'test': [
-                        'plone.app.testing',
-                        'collective.MockMailHost',
-                    ]
-                  },
-                  ...
-                  )
-        
-        Your test layer setup could look like this example below::
-        
-            from plone.app.testing import helpers, layers
-            from plone.testing import z2
-        
-        
-            class MyLayer(helpers.PloneSandboxLayer):
-                defaultBases = (layers.PLONE_FIXTURE, )
-        
-                def setUpZope(self, app, configurationContext):
-                    # Load zcml
-                    import collective.MockMailHost
-                    self.loadZCML(package=collective.MockMailHost)
-        
-                    # Install product and call its initialize() function
-                    z2.installProduct(app, 'collective.MockMailHost')
-        
-                    # Note: you can skip this if my.product is not a Zope 2-style
-                    # product, i.e. it is not in the Products.* namespace and it
-                    # does not have a <five:registerPackage /> directive in its
-                    # configure.zcml.
-        
-                def tearDownZope(self, app):
-                    # Uninstall product
-                    z2.uninstallProduct(app, 'collective.MockMailHost')
-        
-                    # Note: Again, you can skip this if my.product is not a Zope 2-
-                    # style product
-        
-                def setUpPloneSite(self, portal):
-                    helpers.quickInstallProduct(portal, 'collective.MockMailHost')
-        
-                    helpers.applyProfile(portal, 'collective.MockMailHost:default')
-        
-            MY_FIXTURE = MyLayer()
-        
-        .. _Plone: http://plone.org
-        .. _`plone.app.testing`: http://pypi.python.org/pypi/plone.app.testing
-        
-        Using a member-posting forum
-        ============================
-        
-            >>> from Products.CMFCore.utils import getToolByName
-            >>> from Products.MailHost.interfaces import IMailHost
-            >>> from zope.component import getUtility
-        
-            >>> app = layer['app']
-            >>> portal = layer['portal']
-        
-        Test starting conversations, replying and modifying comments in a default
-        member-posting forum.
-        
-        Let us log all exceptions, which is useful for debugging. Also, clear portlet
-        slots, to make the test browser less confused by things like the recent portlet
-        and the navtree.
-        
-            >>> portal.error_log._ignored_exceptions = ()
-            >>> portal.left_slots = portal.right_slots = []
-            >>> workflow = portal.portal_workflow
-        
-        Validate mailhost replacement
-        -----------------------------
-        
-            >>> portal.MailHost
-            <MockMailHost at ...>
-        
-            >>> getToolByName(portal, 'MailHost')
-            <MockMailHost at ...>
-        
-            >>> getUtility(IMailHost)
-            <MockMailHost at ...>
-        
-        
-        Send email
-        ----------
-        
-            >>> to_ = "member@example.com"
-            >>> from_ = "admin@example.com"
-            >>> msg = """
-            ...
-            ... Dear Sir:
-            ...
-            ... Thank you"""
-            >>> portal.MailHost.send(msg, to_, from_)
-            >>> len(portal.MailHost.messages)
-            1
-            >>> 'To: member@example.com' in portal.MailHost.messages[0]
-            True
-            >>> 'From: admin@example.com' in portal.MailHost.messages[0]
-            True
-            >>> 'Dear Sir:' in portal.MailHost.messages[0]
-            True
-            >>> portal.MailHost.reset()
-            >>> len(portal.MailHost.messages)
-            0
-        
-        
-        Changelog
-        =========
-        
-        2.0.0 (2018-11-06)
-        ------------------
-        
-        Breaking changes:
-        
-        - Do not depend on old SecureMailHost any longer.
-          [pbauer]
-        
-        New features:
-        
-        - Python 3 support.
-          [pbauer]
-        
-        
-        1.1.0 (2018-06-27)
-        ------------------
-        
-        - Fix import location, Globals has been removed.
-          [gforcada]
-        
-        - Rework tests setup.
-          [gforcada]
-        
-        
-        1.0 (2016-01-25)
-        ----------------
-        
-        - Fix MIMEText compatibility (broken since 0.9).
-          [jone]
-        
-        
-        0.9 (2015-07-10)
-        ----------------
-        
-        - Clean up msg before sending. Otherwise Plone self registration
-          email does not work [sureshvv]
-        
-        
-        0.8 (2015-06-13)
-        ----------------
-        
-        - Add browser view for functional testing [Casecarsid]
-        
-        
-        0.7 (2013-07-05)
-        ----------------
-        
-        - MANIFEST [sureshvv]
-        
-        
-        0.6 (2013-07-03)
-        ----------------
-        
-        - Track msg_type also.
-          [sureshvv]
-        
-        - Behave more like ``collective.testcaselayer``'s MockMailHost.
-          [saily]
-        
-        - Documentation updates
-          [saily]
-        
-        
-        0.5 - 2012-09-25
-        ----------------
-        
-        - Remove ZopeSkel and Paster dependency from setup.py
-          [saily]
-        
-        - Moved to github and changed to README.rst, links in setup.py
-          [saily]
-        
-        - Allow multiple paramters for ``send`` and ``secureSend`` method in
-          MockMailHost class.  [saily]
-        
-        
-        0.4 (2011-05-17)
-        ----------------
-        
-        - Register MockMailHost in SiteManager to get MockMailHost when using
-          ``getToolByName(context, 'MailHost')`` or ``getUtility(IMailHost)``.
-          [saily]
-        
-        - Inherit from MailHost instead of SimpleItem
-          [saily]
-        
-        - Implement the secureSend method
-          [saily]
-        
-        
-        0.3 (2011-04-04)
-        ----------------
-        
-        - Add ``**kwargs`` to MockMailHost's send method to support mto, mfrom, ...
-          keyword arguments as default MailHost does.  [saily]
-        
-        - Added file for generic setup various handlers
-          [sureshvv]
-        
-        
-        0.2 (2010-05-21)
-        ----------------
-        
-        - Added tests
-          [sureshvv]
-        
-        
-        0.1 (2010-05-16)
-        ----------------
-        
-        - Initial release
-          [sureshvv]
-        
 Keywords: mock mailhost tests
-Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Plone
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
 Provides-Extra: test
+
+Introduction
+============
+
+``collective.MockMailHost`` enables integration testing of email functionality
+from Plone_. Simply add this egg to your [test] runner section, and install
+this product through your ``Layer`` or ``TestCase``.
+
+Note
+  THIS IS FOR TESTING PURPOSE ONLY, do not use this product on your
+  running Plone site. It replaces the standard MailHost with a Mock
+  MailHost that you can poke at to check email content and recipients.
+
+Has been tested with Plone 4 but should also work with earlier versions.
+
+
+Integration
+-----------
+
+Example how to integrate ``collective.MockMailHost`` to your testing setup
+based on `plone.app.testing`_. Add the package to your extras_requires section
+in your package's ``setup.py`` file, so buildout will automatically download
+the package for you.::
+
+    setup(name='my.package',
+          ...
+          extras_require={
+            'test': [
+                'plone.app.testing',
+                'collective.MockMailHost',
+            ]
+          },
+          ...
+          )
+
+Your test layer setup could look like this example below::
+
+    from plone.app.testing import helpers, layers
+    from plone.testing import z2
+
+
+    class MyLayer(helpers.PloneSandboxLayer):
+        defaultBases = (layers.PLONE_FIXTURE, )
+
+        def setUpZope(self, app, configurationContext):
+            # Load zcml
+            import collective.MockMailHost
+            self.loadZCML(package=collective.MockMailHost)
+
+            # Install product and call its initialize() function
+            z2.installProduct(app, 'collective.MockMailHost')
+
+            # Note: you can skip this if my.product is not a Zope 2-style
+            # product, i.e. it is not in the Products.* namespace and it
+            # does not have a <five:registerPackage /> directive in its
+            # configure.zcml.
+
+        def tearDownZope(self, app):
+            # Uninstall product
+            z2.uninstallProduct(app, 'collective.MockMailHost')
+
+            # Note: Again, you can skip this if my.product is not a Zope 2-
+            # style product
+
+        def setUpPloneSite(self, portal):
+            helpers.quickInstallProduct(portal, 'collective.MockMailHost')
+
+            helpers.applyProfile(portal, 'collective.MockMailHost:default')
+
+    MY_FIXTURE = MyLayer()
+
+.. _Plone: http://plone.org
+.. _`plone.app.testing`: http://pypi.python.org/pypi/plone.app.testing
+
+Using a member-posting forum
+============================
+
+    >>> from Products.CMFCore.utils import getToolByName
+    >>> from Products.MailHost.interfaces import IMailHost
+    >>> from zope.component import getUtility
+
+    >>> app = layer['app']
+    >>> portal = layer['portal']
+
+Test starting conversations, replying and modifying comments in a default
+member-posting forum.
+
+Let us log all exceptions, which is useful for debugging. Also, clear portlet
+slots, to make the test browser less confused by things like the recent portlet
+and the navtree.
+
+    >>> portal.error_log._ignored_exceptions = ()
+    >>> portal.left_slots = portal.right_slots = []
+    >>> workflow = portal.portal_workflow
+
+Validate mailhost replacement
+-----------------------------
+
+    >>> portal.MailHost
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
+
+    >>> getToolByName(portal, 'MailHost')
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
+
+    >>> getUtility(IMailHost)
+    <collective.MockMailHost.MockMailHost.MockMailHost object at ...>
+
+
+Send email
+----------
+
+    >>> to_ = "member@example.com"
+    >>> from_ = "admin@example.com"
+    >>> msg = """
+    ...
+    ... Dear Sir:
+    ...
+    ... Thank you"""
+    >>> portal.MailHost.send(msg, to_, from_)
+    >>> len(portal.MailHost.messages)
+    1
+    >>> b'To: member@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'From: admin@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'Dear Sir:' in portal.MailHost.messages[0]
+    True
+    >>> portal.MailHost.messages_from
+    ['admin@example.com']
+    >>> portal.MailHost.messages_to
+    [['member@example.com']]
+    >>> portal.MailHost.reset()
+    >>> len(portal.MailHost.messages)
+    0
+
+Send an `email.message.EmailMessage` object with cc/bcc recipients
+
+    >>> from email.message import EmailMessage
+    >>> msg = EmailMessage()
+    >>> msg["Subject"] = "Hello"
+    >>> msg["From"] = "me@example.com"
+    >>> msg["To"] = "you@example.com"
+    >>> msg["Cc"] = "foo@example.com"
+    >>> msg["Bcc"] = "bar@example.com"
+    >>> msg.set_content("""
+    ... This message is for you, foo, and bar.
+    ... """)
+    >>> portal.MailHost.send(msg)
+    >>> len(portal.MailHost.messages)
+    1
+    >>> b'To: you@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'From: me@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'Cc: foo@example.com' in portal.MailHost.messages[0]
+    True
+    >>> b'bar@example.com' in portal.MailHost.messages[0]
+    False
+    >>> b'This message is for you, foo, and bar.' in portal.MailHost.messages[0]
+    True
+    >>> len(portal.MailHost.messages)
+    1
+    >>> portal.MailHost.messages_from
+    ['me@example.com']
+    >>> portal.MailHost.messages_to
+    [['you@example.com', 'foo@example.com', 'bar@example.com']]
+    >>> portal.MailHost.reset()
+    >>> len(portal.MailHost.messages)
+    0
+
+Changelog
+=========
+
+3.0.0 (2024-04-23)
+------------------
+
+Breaking changes:
+
+- Remove support for Python versions prior to 3.7 and Plone versions
+  prior to 5.2.
+  [mamico]
+
+New features:
+
+- Add `messages_from`, and `messages_to` to record senders and recipients.
+  This is useful for testing `bcc` that is not present in the message.
+  [mamico]
+
+Bug fixes:
+
+- *add item here*
+
+
+2.0.0 (2018-11-06)
+------------------
+
+Breaking changes:
+
+- Do not depend on old SecureMailHost any longer.
+  [pbauer]
+
+New features:
+
+- Python 3 support.
+  [pbauer]
+
+
+1.1.0 (2018-06-27)
+------------------
+
+- Fix import location, Globals has been removed.
+  [gforcada]
+
+- Rework tests setup.
+  [gforcada]
+
+
+1.0 (2016-01-25)
+----------------
+
+- Fix MIMEText compatibility (broken since 0.9).
+  [jone]
+
+
+0.9 (2015-07-10)
+----------------
+
+- Clean up msg before sending. Otherwise Plone self registration
+  email does not work [sureshvv]
+
+
+0.8 (2015-06-13)
+----------------
+
+- Add browser view for functional testing [Casecarsid]
+
+
+0.7 (2013-07-05)
+----------------
+
+- MANIFEST [sureshvv]
+
+
+0.6 (2013-07-03)
+----------------
+
+- Track msg_type also.
+  [sureshvv]
+
+- Behave more like ``collective.testcaselayer``'s MockMailHost.
+  [saily]
+
+- Documentation updates
+  [saily]
+
+
+0.5 - 2012-09-25
+----------------
+
+- Remove ZopeSkel and Paster dependency from setup.py
+  [saily]
+
+- Moved to github and changed to README.rst, links in setup.py
+  [saily]
+
+- Allow multiple paramters for ``send`` and ``secureSend`` method in
+  MockMailHost class.  [saily]
+
+
+0.4 (2011-05-17)
+----------------
+
+- Register MockMailHost in SiteManager to get MockMailHost when using
+  ``getToolByName(context, 'MailHost')`` or ``getUtility(IMailHost)``.
+  [saily]
+
+- Inherit from MailHost instead of SimpleItem
+  [saily]
+
+- Implement the secureSend method
+  [saily]
+
+
+0.3 (2011-04-04)
+----------------
+
+- Add ``**kwargs`` to MockMailHost's send method to support mto, mfrom, ...
+  keyword arguments as default MailHost does.  [saily]
+
+- Added file for generic setup various handlers
+  [sureshvv]
+
+
+0.2 (2010-05-21)
+----------------
+
+- Added tests
+  [sureshvv]
+
+
+0.1 (2010-05-16)
+----------------
+
+- Initial release
+  [sureshvv]
```

### Comparing `collective.MockMailHost-2.0.0/collective.MockMailHost.egg-info/SOURCES.txt` & `collective.MockMailHost-3.0.0/collective.MockMailHost.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 .coveragerc
 .gitignore
-.travis.yml
 CHANGES.rst
 MANIFEST.in
 README.rst
+base.cfg
 buildout.cfg
+plone-5.2.x.cfg
+plone-6.0.x.cfg
+requirements-5.2.x.txt
+requirements-6.0.x.txt
 requirements.txt
 setup.cfg
 setup.py
+tox.ini
 collective/__init__.py
 collective.MockMailHost.egg-info/PKG-INFO
 collective.MockMailHost.egg-info/SOURCES.txt
 collective.MockMailHost.egg-info/dependency_links.txt
 collective.MockMailHost.egg-info/entry_points.txt
 collective.MockMailHost.egg-info/namespace_packages.txt
 collective.MockMailHost.egg-info/not-zip-safe
```

### Comparing `collective.MockMailHost-2.0.0/README.rst` & `collective.MockMailHost-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `collective.MockMailHost-2.0.0/CHANGES.rst` & `collective.MockMailHost-3.0.0/CHANGES.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 Changelog
 =========
 
+3.0.0 (2024-04-23)
+------------------
+
+Breaking changes:
+
+- Remove support for Python versions prior to 3.7 and Plone versions
+  prior to 5.2.
+  [mamico]
+
+New features:
+
+- Add `messages_from`, and `messages_to` to record senders and recipients.
+  This is useful for testing `bcc` that is not present in the message.
+  [mamico]
+
+Bug fixes:
+
+- *add item here*
+
+
 2.0.0 (2018-11-06)
 ------------------
 
 Breaking changes:
 
 - Do not depend on old SecureMailHost any longer.
   [pbauer]
```

