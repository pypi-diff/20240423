# Comparing `tmp/image_center-2024.3.28.tar.gz` & `tmp/image_center-2024.4.23.tar.gz`

## Comparing `image_center-2024.3.28.tar` & `image_center-2024.4.23.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    16165 2020-02-02 00:00:00.000000 image_center-2024.3.28/image_center/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 image_center-2024.3.28/image_center/__version__.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 image_center-2024.3.28/image_center/conf.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 image_center-2024.3.28/image_center/server.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 image_center-2024.3.28/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-2024.3.28/LICENSE
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 image_center-2024.3.28/README.md
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 image_center-2024.3.28/pyproject.toml
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 image_center-2024.3.28/PKG-INFO
+-rw-r--r--   0        0        0    16300 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/__version__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/conf.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 image_center-2024.4.23/image_center/server.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 image_center-2024.4.23/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-2024.4.23/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 image_center-2024.4.23/README.md
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 image_center-2024.4.23/pyproject.toml
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 image_center-2024.4.23/PKG-INFO
```

### Comparing `image_center-2024.3.28/image_center/__init__.py` & `image_center-2024.4.23/image_center/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import os
 import random
 import time
 from typing import List, Union
 from xmlrpc.client import Binary
 from xmlrpc.client import ServerProxy
 
+import easyprocess
+
 try:
     import cv2 as cv
     import numpy as np
 
     GET_OPENCV_FORM_RPC = False
 except ModuleNotFoundError:
     GET_OPENCV_FORM_RPC = True
@@ -90,15 +92,18 @@
         screen = setting.SCREEN_CACHE
 
         if not picture_abspath:
             if screen_bbox:
                 screen = cls.save_temporary_picture(*screen_bbox) + ".png"
             else:
                 if setting.IS_X11:
-                    pyscreenshot.grab().save(screen)
+                    try:
+                        pyscreenshot.grab().save(screen)
+                    except easyprocess.EasyProcessError:
+                        ...
                 else:
                     screen = os.popen(cls.wayland_screen_dbus).read().strip("\n")
         else:
             screen = picture_abspath
         template_path = os.path.expanduser(f"{image_path}.png")
         if GET_OPENCV_FORM_RPC:
             server = ServerProxy(f"http://{setting.SERVER_IP}:{setting.PORT}", allow_none=True)
@@ -113,15 +118,15 @@
                     tpl_path = server.image_put(Binary(template_rb.read()))
                     template_rb.close()
                     return server.match_image_by_opencv(
                         tpl_path, screen_path, rate, multiple
                     )
                 except OSError as exc:
                     raise EnvironmentError(
-                        f"RPC服务器链接失败. http://{setting.SERVER_IP}:{setting.PORT}"
+                        f"OCR 服务器链接失败. http://{setting.SERVER_IP}:{setting.PORT}"
                     ) from exc
         else:
             if not os.path.exists(template_path):
                 raise TemplatePictureNotExist(template_path)
             screen = cv.imread(screen)
             template = cv.imread(template_path)
             result = cv.matchTemplate(screen, template, cv.TM_CCOEFF_NORMED)
```

### Comparing `image_center-2024.3.28/image_center/conf.py` & `image_center-2024.4.23/image_center/conf.py`

 * *Files identical despite different names*

### Comparing `image_center-2024.3.28/image_center/server.py` & `image_center-2024.4.23/image_center/server.py`

 * *Files identical despite different names*

### Comparing `image_center-2024.3.28/.gitignore` & `image_center-2024.4.23/.gitignore`

 * *Files identical despite different names*

### Comparing `image_center-2024.3.28/LICENSE` & `image_center-2024.4.23/LICENSE`

 * *Files identical despite different names*

### Comparing `image_center-2024.3.28/README.md` & `image_center-2024.4.23/README.md`

 * *Files identical despite different names*

### Comparing `image_center-2024.3.28/pyproject.toml` & `image_center-2024.4.23/pyproject.toml`

 * *Files identical despite different names*

### Comparing `image_center-2024.3.28/PKG-INFO` & `image_center-2024.4.23/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-center
-Version: 2024.3.28
+Version: 2024.4.23
 Summary: image-center
 Project-URL: Source, https://github.com/linuxdeepin/image-center
 Project-URL: Documentation, https://linuxdeepin.github.io/image-center
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: image-center Version: 2024.3.28 Summary: image-
+Metadata-Version: 2.1 Name: image-center Version: 2024.4.23 Summary: image-
 center Project-URL: Source, https://github.com/linuxdeepin/image-center
 Project-URL: Documentation, https://linuxdeepin.github.io/image-center Author-
 email: mikigo <1964191531@qq.com> License-File: LICENSE Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Requires-Python:
 >=3.7 Requires-Dist: pillow Requires-Dist: pyscreenshot Provides-Extra: doc
 Requires-Dist: mkdocs-material; extra == 'doc' Provides-Extra: test Requires-
```

