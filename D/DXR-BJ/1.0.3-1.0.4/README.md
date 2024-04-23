# Comparing `tmp/DXR_BJ-1.0.3.tar.gz` & `tmp/DXR_BJ-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR_BJ-1.0.3.tar", last modified: Mon Apr 22 10:56:43 2024, max compression
+gzip compressed data, was "DXR_BJ-1.0.4.tar", last modified: Tue Apr 23 02:49:22 2024, max compression
```

## Comparing `DXR_BJ-1.0.3.tar` & `DXR_BJ-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.154197 DXR_BJ-1.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-22 10:56:42.998278 DXR_BJ-1.0.3/DXR_BJ/
--rw-rw-rw-   0        0        0        0 2024-04-16 05:08:38.000000 DXR_BJ-1.0.3/DXR_BJ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:56:42.985093 DXR_BJ-1.0.3/DXR_BJ/common/
-drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.119239 DXR_BJ-1.0.3/DXR_BJ/common/dependency/
--rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.3/DXR_BJ/common/dependency/simsun.ttc
--rw-rw-rw-   0        0        0    34480 2024-04-22 10:55:51.000000 DXR_BJ-1.0.3/DXR_BJ/drawer.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.014238 DXR_BJ-1.0.3/DXR_BJ.egg-info/
--rw-rw-rw-   0        0        0      156 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-04-22 10:56:42.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-22 10:56:41.000000 DXR_BJ-1.0.3/DXR_BJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      156 2024-04-22 10:56:43.151206 DXR_BJ-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-22 10:56:43.154197 DXR_BJ-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1767 2024-04-22 10:56:16.000000 DXR_BJ-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 10:56:43.150209 DXR_BJ-1.0.3/tests/
--rw-rw-rw-   0        0        0     1068 2024-04-22 02:24:43.000000 DXR_BJ-1.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 02:49:22.628701 DXR_BJ-1.0.4/
+drwxrwxrwx   0        0        0        0 2024-04-23 02:49:22.329961 DXR_BJ-1.0.4/DXR_BJ/
+-rw-rw-rw-   0        0        0        0 2024-04-16 05:08:38.000000 DXR_BJ-1.0.4/DXR_BJ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 02:49:22.325970 DXR_BJ-1.0.4/DXR_BJ/common/
+drwxrwxrwx   0        0        0        0 2024-04-23 02:49:22.336941 DXR_BJ-1.0.4/DXR_BJ/common/dependency/
+-rw-rw-rw-   0        0        0 10500792 2023-12-04 08:46:42.000000 DXR_BJ-1.0.4/DXR_BJ/common/dependency/simsun.ttc
+-rw-rw-rw-   0        0        0    34344 2024-04-23 02:46:24.000000 DXR_BJ-1.0.4/DXR_BJ/drawer.py
+drwxrwxrwx   0        0        0        0 2024-04-23 02:49:22.336941 DXR_BJ-1.0.4/DXR_BJ.egg-info/
+-rw-rw-rw-   0        0        0      208 2024-04-23 02:49:22.000000 DXR_BJ-1.0.4/DXR_BJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-23 02:49:22.000000 DXR_BJ-1.0.4/DXR_BJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 02:49:22.000000 DXR_BJ-1.0.4/DXR_BJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-23 02:49:22.000000 DXR_BJ-1.0.4/DXR_BJ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 02:49:22.000000 DXR_BJ-1.0.4/DXR_BJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       66 2024-04-16 01:18:00.000000 DXR_BJ-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      208 2024-04-23 02:49:22.374838 DXR_BJ-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-23 02:49:22.628701 DXR_BJ-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1791 2024-04-23 02:35:02.000000 DXR_BJ-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 02:49:22.372846 DXR_BJ-1.0.4/tests/
+-rw-rw-rw-   0        0        0     1068 2024-04-22 02:24:43.000000 DXR_BJ-1.0.4/tests/test.py
```

### Comparing `DXR_BJ-1.0.3/DXR_BJ/common/dependency/simsun.ttc` & `DXR_BJ-1.0.4/DXR_BJ/common/dependency/simsun.ttc`

 * *Files identical despite different names*

### Comparing `DXR_BJ-1.0.3/DXR_BJ/drawer.py` & `DXR_BJ-1.0.4/DXR_BJ/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Time    : 2024/04/22
+# @Time    : 2024/04/23
 # @Author  : zx
 # @File    : Drawer.py
-# @Version : 1.0.3
+# @Version : 1.0.4
 
 
 
 import copy
 import os
 import cv2
 import numpy as np
 import math
 import freetype   ## Freetypechinese
 import traceback  ## log
 
 
 ###全局变量
-Version_num='1.0.3'     ###版本号
+Version_num='1.0.4'     ###版本号
 py_path=os.path.dirname(os.path.abspath(__file__))   ##字体路径
                               
 alg_name = { 
     "smoke": "烟雾",
     "fire": "火焰",
     "person": "行人",
     "car": "车",
@@ -241,24 +241,19 @@
             self.labelclass = FreetypePy(self.import_path)  ##python freetype
         except Exception as e:
             logger.info('标记类初始化错误!!!!!')
             logger.info(traceback.format_exc())
 
 
     ### 软件接口函数
-    def draw_frame_box(self, frame, res):
+    def draw_frame_box(self, frame, outmessage):
         t1 = cv2.getTickCount()
         flag = False
         try:
-            num=0
-            for key, value in res.items():
-                outframe = self.draw_frame_main(frame, value)
-                if num != 0:
-                    frame = outframe.copy()   ##多算法标记类兼容
-                num=num+1
+            outframe = self.draw_frame_main(frame, outmessage)
         except Exception as e:
             logger.info(traceback.format_exc())
             logger.info(f'!!!!!!!!!!!!!!!!!!!!!!!!标记类错误message:{outmessage}')
             outframe = frame
             flag = True
 
         t2 = cv2.getTickCount()
@@ -384,14 +379,15 @@
                         sValues[num][0].split('_')[1]]
                 outimg = self.labelclass.DrawChinesename(outimg, zh_label, position, self.rectcolor, self.labelcolor)
 
         ###新老 车牌
         lprtypes = ['LPR', 'HLPR', 'CarJudge']
         if message["sType"] in lprtypes:
             self.labelcolor = self.blue
+            self.labelclass.background=(0, 0, 0)
             self.rectcolor = self.green
             for num, target_rect in enumerate(rects):
                 ## 特殊处理车辆入侵标记
                 if message["sType"] == 'CarJudge':
                     if texts[0][num] == 'Warning':
                         self.rectcolor = self.red
```

### Comparing `DXR_BJ-1.0.3/setup.py` & `DXR_BJ-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup,find_packages
 setup(
   name='DXR_BJ',      ##from 引入的名称
-  version='1.0.3',    ##发布的版本号
-  description='去除掉相应的安装包',
+  version='1.0.4',    ##发布的版本号
+  description='回复循环遍历，修改车牌标记颜色大小',
   author='zx',
   author_email='450125770@qq.com',
   install_requires= ["freetype-py"], # 定义依赖哪些模块
   packages=find_packages(),  # 系统自动从当前目录开始找包
   include_package_data=True,
   # 如果有的文件不用打包，则只能指定需要打包的文件
   #packages=['代码1','代码2','__init__']  #指定目录中需要打包的py文件，注意不要.py后缀
```

### Comparing `DXR_BJ-1.0.3/tests/test.py` & `DXR_BJ-1.0.4/tests/test.py`

 * *Files identical despite different names*

