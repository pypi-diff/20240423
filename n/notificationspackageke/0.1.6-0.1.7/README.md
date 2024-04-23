# Comparing `tmp/notificationspackageke-0.1.6.tar.gz` & `tmp/notificationspackageke-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notificationspackageke-0.1.6.tar", last modified: Thu Nov 30 21:05:36 2023, max compression
+gzip compressed data, was "notificationspackageke-0.1.7.tar", last modified: Tue Apr 23 15:09:20 2024, max compression
```

## Comparing `notificationspackageke-0.1.6.tar` & `notificationspackageke-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-30 21:05:36.731398 notificationspackageke-0.1.6/
--rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2023-10-12 14:51:49.000000 notificationspackageke-0.1.6/LICENSE
--rw-r--r--   0 carlos    (1000) carlos    (1000)      307 2023-11-30 21:05:36.731398 notificationspackageke-0.1.6/PKG-INFO
--rw-r--r--   0 carlos    (1000) carlos    (1000)       22 2023-10-11 14:58:18.000000 notificationspackageke-0.1.6/README.md
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-30 21:05:36.731398 notificationspackageke-0.1.6/notificationmethods/
--rw-r--r--   0 carlos    (1000) carlos    (1000)       24 2023-10-27 20:50:10.000000 notificationspackageke-0.1.6/notificationmethods/__init__.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)     2688 2023-11-30 20:52:25.000000 notificationspackageke-0.1.6/notificationmethods/email.py
--rw-r--r--   0 carlos    (1000) carlos    (1000)      118 2023-10-27 19:18:08.000000 notificationspackageke-0.1.6/notificationmethods/notificacion.py
-drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2023-11-30 21:05:36.731398 notificationspackageke-0.1.6/notificationspackageke.egg-info/
--rw-r--r--   0 carlos    (1000) carlos    (1000)      307 2023-11-30 21:05:36.000000 notificationspackageke-0.1.6/notificationspackageke.egg-info/PKG-INFO
--rw-r--r--   0 carlos    (1000) carlos    (1000)      317 2023-11-30 21:05:36.000000 notificationspackageke-0.1.6/notificationspackageke.egg-info/SOURCES.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)        1 2023-11-30 21:05:36.000000 notificationspackageke-0.1.6/notificationspackageke.egg-info/dependency_links.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       20 2023-11-30 21:05:36.000000 notificationspackageke-0.1.6/notificationspackageke.egg-info/top_level.txt
--rw-r--r--   0 carlos    (1000) carlos    (1000)       38 2023-11-30 21:05:36.741398 notificationspackageke-0.1.6/setup.cfg
--rw-r--r--   0 carlos    (1000) carlos    (1000)      535 2023-11-30 21:04:48.000000 notificationspackageke-0.1.6/setup.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-23 15:09:20.083789 notificationspackageke-0.1.7/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        0 2024-04-23 14:09:55.000000 notificationspackageke-0.1.7/LICENSE
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      326 2024-04-23 15:09:20.084181 notificationspackageke-0.1.7/PKG-INFO
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       22 2024-04-23 14:08:08.000000 notificationspackageke-0.1.7/README.md
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-23 15:09:20.072026 notificationspackageke-0.1.7/notificationmethods/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       24 2024-04-23 14:09:55.000000 notificationspackageke-0.1.7/notificationmethods/__init__.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)     2887 2024-04-23 14:58:37.000000 notificationspackageke-0.1.7/notificationmethods/email.py
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      118 2024-04-23 14:09:55.000000 notificationspackageke-0.1.7/notificationmethods/notificacion.py
+drwxr-xr-x   0 carlos    (1000) carlos    (1000)        0 2024-04-23 15:09:20.081607 notificationspackageke-0.1.7/notificationspackageke.egg-info/
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      326 2024-04-23 15:09:20.000000 notificationspackageke-0.1.7/notificationspackageke.egg-info/PKG-INFO
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      317 2024-04-23 15:09:20.000000 notificationspackageke-0.1.7/notificationspackageke.egg-info/SOURCES.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)        1 2024-04-23 15:09:20.000000 notificationspackageke-0.1.7/notificationspackageke.egg-info/dependency_links.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       20 2024-04-23 15:09:20.000000 notificationspackageke-0.1.7/notificationspackageke.egg-info/top_level.txt
+-rw-r--r--   0 carlos    (1000) carlos    (1000)       38 2024-04-23 15:09:20.086233 notificationspackageke-0.1.7/setup.cfg
+-rw-r--r--   0 carlos    (1000) carlos    (1000)      535 2024-04-23 15:06:11.000000 notificationspackageke-0.1.7/setup.py
```

### Comparing `notificationspackageke-0.1.6/notificationmethods/email.py` & `notificationspackageke-0.1.7/notificationmethods/email.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,27 +17,32 @@
         self.mode = mode
         self.psw = psw
         self.port = port
 
     def send(self, to, subject, reply_to, bcc, attachments=None,
              body='<p>--Emtpy--</p>'):
         try:
+            files = []
             if self.mode == 'prod':
+                for attachment in attachments:
+                    file_opened = open(attachment,'rb')
+                    files.append(('attachment',file_opened))
+                    
                 response = requests.post(
                     f"https://api.mailgun.net/v3/{self.host}/messages",
                     auth=("api", self.api_key),
                     data={
                         "from": self.sender,
                         "to": to,
                         "subject": subject,
                         "html": body,
                         'h:Reply_to':reply_to,
                         'bcc':bcc,
-                        'files':attachments
-                    }
+                    },
+                    files = files
                 )
                 return response
             else:
                 context = ssl.create_default_context()
                 server = smtplib.SMTP(self.host, self.port)
                 server.ehlo(name=self.host)
                 server.starttls(context=context)
```

### Comparing `notificationspackageke-0.1.6/setup.py` & `notificationspackageke-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '0.1.6' 
+VERSION = '0.1.7' 
 DESCRIPTION = 'Paquete de notificaciones'
 LONG_DESCRIPTION = 'Paquete de canales de notificaciones de kemok'
 
 # Configurando
 setup(
         name="notificationspackageke", 
         version=VERSION,
```

