# Comparing `tmp/Django-Safe-EmailBackend-1.2.5.tar.gz` & `tmp/Django-Safe-EmailBackend-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Django-Safe-EmailBackend-1.2.5.tar", last modified: Tue Feb 20 19:08:45 2024, max compression
+gzip compressed data, was "Django-Safe-EmailBackend-1.2.6.tar", last modified: Mon Apr 22 22:19:41 2024, max compression
```

## Comparing `Django-Safe-EmailBackend-1.2.5.tar` & `Django-Safe-EmailBackend-1.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 19:08:45.239427 Django-Safe-EmailBackend-1.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 19:08:45.239427 Django-Safe-EmailBackend-1.2.5/Django_Safe_EmailBackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-20 19:08:45.000000 Django-Safe-EmailBackend-1.2.5/Django_Safe_EmailBackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-20 19:08:45.000000 Django-Safe-EmailBackend-1.2.5/Django_Safe_EmailBackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 19:08:45.000000 Django-Safe-EmailBackend-1.2.5/Django_Safe_EmailBackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-20 19:08:45.000000 Django-Safe-EmailBackend-1.2.5/Django_Safe_EmailBackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-20 19:08:45.000000 Django-Safe-EmailBackend-1.2.5/Django_Safe_EmailBackend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-02-20 19:08:35.000000 Django-Safe-EmailBackend-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-20 19:08:35.000000 Django-Safe-EmailBackend-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-20 19:08:45.239427 Django-Safe-EmailBackend-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-20 19:08:35.000000 Django-Safe-EmailBackend-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 19:08:45.239427 Django-Safe-EmailBackend-1.2.5/saferecipient/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-20 19:08:44.000000 Django-Safe-EmailBackend-1.2.5/saferecipient/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-02-20 19:08:35.000000 Django-Safe-EmailBackend-1.2.5/saferecipient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5139 2024-02-20 19:08:35.000000 Django-Safe-EmailBackend-1.2.5/saferecipient/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 19:08:45.239427 Django-Safe-EmailBackend-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-02-20 19:08:35.000000 Django-Safe-EmailBackend-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:41.404163 Django-Safe-EmailBackend-1.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:41.404163 Django-Safe-EmailBackend-1.2.6/Django_Safe_EmailBackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 22:19:41.000000 Django-Safe-EmailBackend-1.2.6/Django_Safe_EmailBackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 22:19:41.000000 Django-Safe-EmailBackend-1.2.6/Django_Safe_EmailBackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 22:19:41.000000 Django-Safe-EmailBackend-1.2.6/Django_Safe_EmailBackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 22:19:41.000000 Django-Safe-EmailBackend-1.2.6/Django_Safe_EmailBackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-22 22:19:41.000000 Django-Safe-EmailBackend-1.2.6/Django_Safe_EmailBackend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-04-22 22:19:33.000000 Django-Safe-EmailBackend-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-22 22:19:33.000000 Django-Safe-EmailBackend-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 22:19:41.404163 Django-Safe-EmailBackend-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-22 22:19:33.000000 Django-Safe-EmailBackend-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 22:19:41.404163 Django-Safe-EmailBackend-1.2.6/saferecipient/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-22 22:19:40.000000 Django-Safe-EmailBackend-1.2.6/saferecipient/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-22 22:19:33.000000 Django-Safe-EmailBackend-1.2.6/saferecipient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-04-22 22:19:33.000000 Django-Safe-EmailBackend-1.2.6/saferecipient/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 22:19:41.404163 Django-Safe-EmailBackend-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-22 22:19:33.000000 Django-Safe-EmailBackend-1.2.6/setup.py
```

### Comparing `Django-Safe-EmailBackend-1.2.5/Django_Safe_EmailBackend.egg-info/PKG-INFO` & `Django-Safe-EmailBackend-1.2.6/Django_Safe_EmailBackend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Safe-EmailBackend
-Version: 1.2.5
+Version: 1.2.6
 Summary: A django email backend that sends all emails to a given address
 Home-page: https://github.com/uw-it-aca/django-saferecipient-email-backend
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Safe-EmailBackend-1.2.5/LICENSE` & `Django-Safe-EmailBackend-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Django-Safe-EmailBackend-1.2.5/PKG-INFO` & `Django-Safe-EmailBackend-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Django-Safe-EmailBackend
-Version: 1.2.5
+Version: 1.2.6
 Summary: A django email backend that sends all emails to a given address
 Home-page: https://github.com/uw-it-aca/django-saferecipient-email-backend
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `Django-Safe-EmailBackend-1.2.5/README.md` & `Django-Safe-EmailBackend-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `Django-Safe-EmailBackend-1.2.5/saferecipient/__init__.py` & `Django-Safe-EmailBackend-1.2.6/saferecipient/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,46 @@
 # Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
-
-"""SMTP email backend class that only sends email to a safe email address"""
 import re
+import ssl
 from django.conf import settings
 from django.core.mail.backends.smtp import EmailBackend as SMTPEmailBackend
+from django.utils.functional import cached_property
 from email.mime.text import MIMEText
 
 
 class EmailBackend(SMTPEmailBackend):
     """
+    An SMTP email backend class that only sends email to a safe email address.
+
     Re-routes email, so it goes to, and comes from
     settings.SAFE_EMAIL_RECIPIENT.
 
     The original to and from are added to a text file
     that is attached to the message.
     """
 
+    @cached_property
+    def ssl_context(self):
+        """
+        See https://code.djangoproject.com/ticket/34504
+        """
+        try:
+            ssl_context = super().ssl_context
+        except AttributeError:  # Django < 4
+            ssl_context = ssl.SSLContext()
+        ssl_context.check_hostname = False
+        ssl_context.verify_mode = ssl.CERT_NONE
+        return ssl_context
+
     def send_messages(self, email_messages):
         for message in email_messages:
             self._safeguard(message)
-        return super(EmailBackend, self).send_messages(email_messages)
+        return super().send_messages(email_messages)
 
     def _safeguard(self, message):
         originals = ("Original From: {}\nOriginal To: {}\nOriginal CC: {}\n"
                      "Original BCC: {}\n").format(
                          message.from_email, message.to,
                          message.cc, message.bcc)
 
@@ -42,24 +57,25 @@
             text_attachment = MIMEText(originals)
             text_attachment.add_header(
                 'Content-disposition',
                 'attachment; filename="original_emails.txt"')
             message.attach(text_attachment)
 
     def _only_safe_emails(self, emails):
-        """"Given a list of emails, checks whether they are all in the white
-        list."""
-
+        """"
+        Given a list of emails, checks whether they are all in the safe list.
+        """
         email_modified = False
         if any(not self._is_safelisted(email) for email in emails):
             email_modified = True
             emails = [email for email in emails if self._is_safelisted(email)]
             if settings.SAFE_EMAIL_RECIPIENT not in emails:
                 emails.append(settings.SAFE_EMAIL_RECIPIENT)
         return emails, email_modified
 
     def _is_safelisted(self, email):
-        """Check if an email is in the safelist. If there's no safelist,
-        it's assumed it's not safelisted."""
-
-        return hasattr(settings, "SAFE_EMAIL_SAFELIST") and \
-            any(re.match(m, email) for m in settings.SAFE_EMAIL_SAFELIST)
+        """
+        Check if an email is in the safelist. If there's no safelist,
+        it's assumed it's not safelisted.
+        """
+        return (hasattr(settings, "SAFE_EMAIL_SAFELIST") and
+                any(re.match(m, email) for m in settings.SAFE_EMAIL_SAFELIST))
```

### Comparing `Django-Safe-EmailBackend-1.2.5/saferecipient/tests.py` & `Django-Safe-EmailBackend-1.2.6/saferecipient/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Copyright 2024 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
 
 from django.core.mail import EmailMultiAlternatives
 from django.test import TestCase
-
 from saferecipient import EmailBackend
+import ssl
 
 
 class TestEmailBackend(TestCase):
     SAFE_EMAIL = 'safe@example.com'
 
+    def test_ssl_context(self):
+        backend = EmailBackend()
+        ssl_context = backend.ssl_context
+        self.assertFalse(ssl_context.check_hostname)
+        self.assertEqual(ssl_context.verify_mode, ssl.CERT_NONE)
+
     def test_safeguard(self):
         with self.settings(SAFE_EMAIL_RECIPIENT=self.SAFE_EMAIL):
             message = self._setup_message()
             EmailBackend()._safeguard(message)
             self.assertEqual(message.from_email, 'safe@example.com')
             self.assertEqual(message.to, ['safe@example.com'])
             self.assertEqual(message.cc, ['safe@example.com'])
```

### Comparing `Django-Safe-EmailBackend-1.2.5/setup.py` & `Django-Safe-EmailBackend-1.2.6/setup.py`

 * *Files identical despite different names*

