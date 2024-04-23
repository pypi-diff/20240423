# Comparing `tmp/django-gmailapi-json-backend-1.8.tar.gz` & `tmp/django_gmailapi_json_backend-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-gmailapi-json-backend-1.8.tar", last modified: Mon Oct 30 11:05:23 2023, max compression
+gzip compressed data, was "django_gmailapi_json_backend-1.9.tar", last modified: Mon Apr 22 08:36:07 2024, max compression
```

## Comparing `django-gmailapi-json-backend-1.8.tar` & `django_gmailapi_json_backend-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2023-10-30 11:05:23.104682 django-gmailapi-json-backend-1.8/
--rw-r--r--   0 matteo     (501) staff       (20)    11357 2021-12-03 10:42:51.000000 django-gmailapi-json-backend-1.8/LICENSE
--rw-r--r--   0 matteo     (501) staff       (20)     3769 2023-10-30 11:05:23.104621 django-gmailapi-json-backend-1.8/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)     3042 2023-10-30 10:57:55.000000 django-gmailapi-json-backend-1.8/README.md
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2023-10-30 11:05:23.103720 django-gmailapi-json-backend-1.8/django_gmailapi_json_backend.egg-info/
--rw-r--r--   0 matteo     (501) staff       (20)     3769 2023-10-30 11:05:23.000000 django-gmailapi-json-backend-1.8/django_gmailapi_json_backend.egg-info/PKG-INFO
--rw-r--r--   0 matteo     (501) staff       (20)      358 2023-10-30 11:05:23.000000 django-gmailapi-json-backend-1.8/django_gmailapi_json_backend.egg-info/SOURCES.txt
--rw-r--r--   0 matteo     (501) staff       (20)        1 2023-10-30 11:05:23.000000 django-gmailapi-json-backend-1.8/django_gmailapi_json_backend.egg-info/dependency_links.txt
--rw-r--r--   0 matteo     (501) staff       (20)       74 2023-10-30 11:05:23.000000 django-gmailapi-json-backend-1.8/django_gmailapi_json_backend.egg-info/requires.txt
--rw-r--r--   0 matteo     (501) staff       (20)       17 2023-10-30 11:05:23.000000 django-gmailapi-json-backend-1.8/django_gmailapi_json_backend.egg-info/top_level.txt
-drwxr-xr-x   0 matteo     (501) staff       (20)        0 2023-10-30 11:05:23.103949 django-gmailapi-json-backend-1.8/gmailapi_backend/
--rw-r--r--   0 matteo     (501) staff       (20)        0 2021-12-03 10:42:51.000000 django-gmailapi-json-backend-1.8/gmailapi_backend/__init__.py
--rw-r--r--   0 matteo     (501) staff       (20)     4748 2023-10-30 10:47:17.000000 django-gmailapi-json-backend-1.8/gmailapi_backend/service.py
--rw-r--r--   0 matteo     (501) staff       (20)      205 2022-01-25 10:30:17.000000 django-gmailapi-json-backend-1.8/pyproject.toml
--rw-r--r--   0 matteo     (501) staff       (20)      770 2023-10-30 11:05:23.104940 django-gmailapi-json-backend-1.8/setup.cfg
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-04-22 08:36:07.913076 django_gmailapi_json_backend-1.9/
+-rw-r--r--   0 matteo     (501) staff       (20)    11357 2021-12-03 10:42:51.000000 django_gmailapi_json_backend-1.9/LICENSE
+-rw-r--r--   0 matteo     (501) staff       (20)     3769 2024-04-22 08:36:07.912988 django_gmailapi_json_backend-1.9/PKG-INFO
+-rw-r--r--   0 matteo     (501) staff       (20)     3042 2023-10-30 10:57:55.000000 django_gmailapi_json_backend-1.9/README.md
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-04-22 08:36:07.912700 django_gmailapi_json_backend-1.9/django_gmailapi_json_backend.egg-info/
+-rw-r--r--   0 matteo     (501) staff       (20)     3769 2024-04-22 08:36:07.000000 django_gmailapi_json_backend-1.9/django_gmailapi_json_backend.egg-info/PKG-INFO
+-rw-r--r--   0 matteo     (501) staff       (20)      358 2024-04-22 08:36:07.000000 django_gmailapi_json_backend-1.9/django_gmailapi_json_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 matteo     (501) staff       (20)        1 2024-04-22 08:36:07.000000 django_gmailapi_json_backend-1.9/django_gmailapi_json_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 matteo     (501) staff       (20)       74 2024-04-22 08:36:07.000000 django_gmailapi_json_backend-1.9/django_gmailapi_json_backend.egg-info/requires.txt
+-rw-r--r--   0 matteo     (501) staff       (20)       17 2024-04-22 08:36:07.000000 django_gmailapi_json_backend-1.9/django_gmailapi_json_backend.egg-info/top_level.txt
+drwxr-xr-x   0 matteo     (501) staff       (20)        0 2024-04-22 08:36:07.912306 django_gmailapi_json_backend-1.9/gmailapi_backend/
+-rw-r--r--   0 matteo     (501) staff       (20)        0 2021-12-03 10:42:51.000000 django_gmailapi_json_backend-1.9/gmailapi_backend/__init__.py
+-rw-r--r--   0 matteo     (501) staff       (20)     5087 2024-04-22 08:22:20.000000 django_gmailapi_json_backend-1.9/gmailapi_backend/service.py
+-rw-r--r--   0 matteo     (501) staff       (20)      205 2022-01-25 10:30:17.000000 django_gmailapi_json_backend-1.9/pyproject.toml
+-rw-r--r--   0 matteo     (501) staff       (20)      770 2024-04-22 08:36:07.913377 django_gmailapi_json_backend-1.9/setup.cfg
```

### Comparing `django-gmailapi-json-backend-1.8/LICENSE` & `django_gmailapi_json_backend-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gmailapi-json-backend-1.8/PKG-INFO` & `django_gmailapi_json_backend-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gmailapi-json-backend
-Version: 1.8
+Version: 1.9
 Summary: Email backend for Django which sends email via the Gmail API through a JSON credential
 Home-page: https://github.com/innoveit/django-gmailapi-json-backend
 Author: Innove
 Author-email: info@innove.it
 Project-URL: Bug Tracker, https://github.com/innoveit/django-gmailapi-json-backend
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-gmailapi-json-backend-1.8/README.md` & `django_gmailapi_json_backend-1.9/README.md`

 * *Files identical despite different names*

### Comparing `django-gmailapi-json-backend-1.8/django_gmailapi_json_backend.egg-info/PKG-INFO` & `django_gmailapi_json_backend-1.9/django_gmailapi_json_backend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gmailapi-json-backend
-Version: 1.8
+Version: 1.9
 Summary: Email backend for Django which sends email via the Gmail API through a JSON credential
 Home-page: https://github.com/innoveit/django-gmailapi-json-backend
 Author: Innove
 Author-email: info@innove.it
 Project-URL: Bug Tracker, https://github.com/innoveit/django-gmailapi-json-backend
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-gmailapi-json-backend-1.8/gmailapi_backend/service.py` & `django_gmailapi_json_backend-1.9/gmailapi_backend/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,29 +24,43 @@
             fail_silently=False,
             google_service_account=None,
             gmail_scopes=None,
             gmail_user=None,
             **kwargs
     ):
         super().__init__(fail_silently=fail_silently)
-
+        
         self.google_service_account = settings.GOOGLE_SERVICE_ACCOUNT if google_service_account is None else google_service_account
         self.gmail_scopes = gmail_scopes if gmail_scopes else (settings.GMAIL_SCOPES if settings.GMAIL_SCOPES else 'https://www.googleapis.com/auth/gmail.send')
-        self.gmail_user = settings.GMAIL_USER if gmail_user is None else gmail_user        
-
-        credentials = service_account.Credentials.from_service_account_info(json.loads(
-            self.google_service_account), scopes=self.gmail_scopes, subject=self.gmail_user)
-
-        self.connection = build('gmail', 'v1', cache_discovery=False, credentials=credentials)
+        self.gmail_user = settings.GMAIL_USER if gmail_user is None else gmail_user
+        self.connection = None
+        self.open()
 
     def open(self):
-        pass
-
+        if self.connection: return False
+        try:
+            credentials = service_account.Credentials.from_service_account_info(json.loads(
+                self.google_service_account), scopes=self.gmail_scopes, subject=self.gmail_user)
+            self.connection = build('gmail', 'v1', cache_discovery=False, credentials=credentials)
+            return True
+        except:
+            if not self.fail_silently:
+                self.close()
+                raise
+    
     def close(self):
-        pass
+        if self.connection is None: return
+        try:
+            self.connection.close()
+            self.connection = None
+        except:
+            self.connection = None
+            if self.fail_silently:
+                return
+            raise
 
     def send_messages(self, email_messages):        
         num_sent = 0
         for email_message in email_messages:
             message = create_message(email_message)
             sent = self._send(message)
             if sent:
@@ -60,15 +74,17 @@
         except Exception as error:
             logger.error('Error sending email', error)
             if settings.EMAIL_BACKEND and settings.EMAIL_BACKEND == "mailer.backend.DbBackend":
                 # If using "django-mailer" https://github.com/pinax/django-mailer, tt marks the related message as
                 # deferred only for some exceptions, so we raise one of them to save the error on the db
                 raise socket.error(error)
             else:
-                raise
+                if not self.fail_silently:
+                    raise
+                return False
         return True
 
 
 def create_message(email_message):
     if email_message.attachments:
         message = MIMEMultipart()
         msg = MIMEText(email_message.body, email_message.content_subtype)
@@ -83,38 +99,32 @@
         message['cc'] = ','.join(map(str, email_message.cc))
     if email_message.bcc:
         message['bcc'] = ','.join(map(str, email_message.bcc))
     message['subject'] = str(email_message.subject)
 
     if email_message.attachments:
         for attachment in email_message.attachments:
-            content_type, encoding = mimetypes.guess_type(attachment[0])
-            if content_type is None or encoding is not None:
-                content_type = 'application/octet-stream'
+            if isinstance(attachment, MIMEBase):
+                message.attach(attachment)
+                continue
+            if bool(attachment[2]): content_type = attachment[2]
+            else:
+                content_type, encoding = mimetypes.guess_type(attachment[0])
+                if content_type is None or encoding is not None:
+                    content_type = 'application/octet-stream'
             main_type, sub_type = content_type.split('/', 1)
             if main_type == 'text':
-                fp = open(attachment[1], 'rb')
-                msg = MIMEText(fp.read(), _subtype=sub_type)
-                fp.close()
+                msg = MIMEText(attachment[1], _subtype=sub_type)
             elif main_type == 'image':
-                fp = open(attachment[1], 'rb')
-                msg = MIMEImage(fp.read(), _subtype=sub_type)
-                fp.close()
+                msg = MIMEImage(attachment[1], _subtype=sub_type)
             elif main_type == 'audio':
-                fp = open(attachment[1], 'rb')
-                msg = MIMEAudio(fp.read(), _subtype=sub_type)
-                fp.close()
-            elif type(attachment[1]) is bytes:
-                msg = MIMEBase(main_type, sub_type)
-                msg.set_payload(attachment[1])
+                msg = MIMEAudio(attachment[1], _subtype=sub_type)
             else:
-                fp = open(attachment[1], 'rb')
                 msg = MIMEBase(main_type, sub_type)
-                msg.set_payload(fp.read())
-                fp.close()
+                msg.set_payload(attachment[1])
 
             filename = attachment[0]
 
             msg.add_header('Content-Disposition', 'attachment', filename=filename)
             encoder.encode_base64(msg)
             message.attach(msg)
```

### Comparing `django-gmailapi-json-backend-1.8/setup.cfg` & `django_gmailapi_json_backend-1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-gmailapi-json-backend
-version = 1.8
+version = 1.9
 author = Innove
 author_email = info@innove.it
 description = Email backend for Django which sends email via the Gmail API through a JSON credential
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/innoveit/django-gmailapi-json-backend
 project_urls =
```

