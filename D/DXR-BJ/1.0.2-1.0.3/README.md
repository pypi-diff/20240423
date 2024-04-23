# Comparing `tmp/DXR_BJ-1.0.2.tar.gz` & `tmp/DXR_BJ-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR_BJ-1.0.2.tar", last modified: Tue Apr 16 06:35:00 2024, max compression
+gzip compressed data, was "DXR_BJ-1.0.3.tar", last modified: Mon Apr 22 10:56:43 2024, max compression
```

## Comparing `DXR_BJ-1.0.2.tar` & `DXR_BJ-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 06:35:00.981819 DXR_BJ-1.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-16 06:35:00.927963 DXR_BJ-1.0.2/DXR_BJ/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:08:38.000000 DXR_BJ-1.0.2/DXR_BJ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:35:00.916992 DXR_BJ-1.0.2/DXR_BJ/common/
-drwxrwxrwx   0        0        0        0 2024-04-16 06:35:00.944918 DXR_BJ-1.0.2/DXR_BJ/common/dependency/
--rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.2/DXR_BJ/common/dependency/simsun.ttc
--rw-rw-rw-   0        0        0    34578 2024-04-16 06:34:41.000000 DXR_BJ-1.0.2/DXR_BJ/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:35:00.943921 DXR_BJ-1.0.2/DXR_BJ.egg-info/
--rw-rw-rw-   0        0        0      156 2024-04-16 06:35:00.000000 DXR_BJ-1.0.2/DXR_BJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-16 06:35:00.000000 DXR_BJ-1.0.2/DXR_BJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 06:35:00.000000 DXR_BJ-1.0.2/DXR_BJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-16 06:35:00.000000 DXR_BJ-1.0.2/DXR_BJ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 06:35:00.000000 DXR_BJ-1.0.2/DXR_BJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      156 2024-04-16 06:35:00.980822 DXR_BJ-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 06:35:00.981819 DXR_BJ-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1767 2024-04-16 06:34:34.000000 DXR_BJ-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:35:00.979825 DXR_BJ-1.0.2/tests/
--rw-rw-rw-   0        0        0       42 2024-04-15 08:31:45.000000 DXR_BJ-1.0.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.154197 DXR_BJ-1.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-22 10:56:42.998278 DXR_BJ-1.0.3/DXR_BJ/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:08:38.000000 DXR_BJ-1.0.3/DXR_BJ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 10:56:42.985093 DXR_BJ-1.0.3/DXR_BJ/common/
+drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.119239 DXR_BJ-1.0.3/DXR_BJ/common/dependency/
+-rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.3/DXR_BJ/common/dependency/simsun.ttc
+-rw-rw-rw-   0        0        0    34480 2024-04-22 10:55:51.000000 DXR_BJ-1.0.3/DXR_BJ/drawer.py
+drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.014238 DXR_BJ-1.0.3/DXR_BJ.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-22 10:56:42.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      156 2024-04-22 10:56:43.151206 DXR_BJ-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-22 10:56:43.154197 DXR_BJ-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1767 2024-04-22 10:56:16.000000 DXR_BJ-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.150209 DXR_BJ-1.0.3/tests/
+-rw-rw-rw-   0        0        0     1068 2024-04-22 02:24:43.000000 DXR_BJ-1.0.3/tests/test.py
```

### Comparing `DXR_BJ-1.0.2/DXR_BJ/common/dependency/simsun.ttc` & `DXR_BJ-1.0.3/DXR_BJ/common/dependency/simsun.ttc`

 * *Files identical despite different names*

### Comparing `DXR_BJ-1.0.2/DXR_BJ/drawer.py` & `DXR_BJ-1.0.3/DXR_BJ/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Time    : 2024/04/16
+# @Time    : 2024/04/22
 # @Author  : zx
 # @File    : Drawer.py
-# @Version : 1.0.9
-# @三种标记方式编写成三个类，加上标记类和颜色类一共五个
-# @ Drawer Colors Freetype2ch  Imagefusion  FreetypePy
-# @ 外部调用接口     drawer = Drawer(字体目录)  outimg,_=drawer.draw_frame_box(img,outmessage)
-# @ 暂时只包含画矩形 区域 线
+# @Version : 1.0.3
+
 
 
 import copy
 import os
 import cv2
 import numpy as np
 import math
 import freetype   ## Freetypechinese
 import traceback  ## log
 
 
 ###全局变量
-Version_num='1.0.2'     ###版本号
+Version_num='1.0.3'     ###版本号
 py_path=os.path.dirname(os.path.abspath(__file__))   ##字体路径
                               
 alg_name = { 
     "smoke": "烟雾",
     "fire": "火焰",
     "person": "行人",
     "car": "车",
@@ -244,19 +241,24 @@
             self.labelclass = FreetypePy(self.import_path)  ##python freetype
         except Exception as e:
             logger.info('标记类初始化错误!!!!!')
             logger.info(traceback.format_exc())
 
 
     ### 软件接口函数
-    def draw_frame_box(self, frame, outmessage):
+    def draw_frame_box(self, frame, res):
         t1 = cv2.getTickCount()
         flag = False
         try:
-            outframe = self.draw_frame_main(frame, outmessage)
+            num=0
+            for key, value in res.items():
+                outframe = self.draw_frame_main(frame, value)
+                if num != 0:
+                    frame = outframe.copy()   ##多算法标记类兼容
+                num=num+1
         except Exception as e:
             logger.info(traceback.format_exc())
             logger.info(f'!!!!!!!!!!!!!!!!!!!!!!!!标记类错误message:{outmessage}')
             outframe = frame
             flag = True
 
         t2 = cv2.getTickCount()
```

### Comparing `DXR_BJ-1.0.2/setup.py` & `DXR_BJ-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup,find_packages
 setup(
   name='DXR_BJ',      ##from 引入的名称
-  version='1.0.2',    ##发布的版本号
+  version='1.0.3',    ##发布的版本号
   description='去除掉相应的安装包',
   author='zx',
   author_email='450125770@qq.com',
   install_requires= ["freetype-py"], # 定义依赖哪些模块
   packages=find_packages(),  # 系统自动从当前目录开始找包
   include_package_data=True,
   # 如果有的文件不用打包，则只能指定需要打包的文件
```

