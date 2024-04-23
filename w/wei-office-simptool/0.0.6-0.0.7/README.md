# Comparing `tmp/wei_office_simptool-0.0.6.tar.gz` & `tmp/wei_office_simptool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wei_office_simptool-0.0.6.tar", last modified: Mon Apr 22 06:38:11 2024, max compression
+gzip compressed data, was "wei_office_simptool-0.0.7.tar", last modified: Tue Apr 23 08:59:52 2024, max compression
```

## Comparing `wei_office_simptool-0.0.6.tar` & `wei_office_simptool-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.539742 wei_office_simptool-0.0.6/
--rw-rw-rw-   0        0        0     5306 2024-04-22 06:38:11.537740 wei_office_simptool-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4490 2024-04-22 05:51:50.000000 wei_office_simptool-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 06:38:11.539742 wei_office_simptool-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2498 2024-04-22 06:36:05.000000 wei_office_simptool-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.518736 wei_office_simptool-0.0.6/tests/
--rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.6/tests/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.523738 wei_office_simptool-0.0.6/wei_office_simptool/
--rw-rw-rw-   0        0        0     1669 2024-04-19 08:47:36.000000 wei_office_simptool-0.0.6/wei_office_simptool/__init__.py
--rw-rw-rw-   0        0        0    15251 2024-04-22 05:51:50.000000 wei_office_simptool-0.0.6/wei_office_simptool/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 06:38:11.535750 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/
--rw-rw-rw-   0        0        0     5306 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-22 06:38:11.000000 wei_office_simptool-0.0.6/wei_office_simptool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.993323 wei_office_simptool-0.0.7/
+-rw-rw-rw-   0        0        0     5346 2024-04-23 08:59:52.991309 wei_office_simptool-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4530 2024-04-23 08:08:12.000000 wei_office_simptool-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 08:59:52.993323 wei_office_simptool-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2498 2024-04-23 08:08:12.000000 wei_office_simptool-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.974085 wei_office_simptool-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1359 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     2101 2024-04-19 06:49:12.000000 wei_office_simptool-0.0.7/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.977085 wei_office_simptool-0.0.7/wei_office_simptool/
+-rw-rw-rw-   0        0        0     1669 2024-04-19 08:47:36.000000 wei_office_simptool-0.0.7/wei_office_simptool/__init__.py
+-rw-rw-rw-   0        0        0    15286 2024-04-23 08:08:12.000000 wei_office_simptool-0.0.7/wei_office_simptool/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 08:59:52.989077 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/
+-rw-rw-rw-   0        0        0     5346 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-23 08:59:52.000000 wei_office_simptool-0.0.7/wei_office_simptool.egg-info/top_level.txt
```

### Comparing `wei_office_simptool-0.0.6/PKG-INFO` & `wei_office_simptool-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.6
+Version: 0.0.7
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -100,24 +100,24 @@
 from wei_office_simptool import eSend
 
 # 示例代码
 email_sender = eSend(sender,receiver,username,password,smtpserver='smtp.126.com')
 email_sender.send_email(subject='Your Subject', e_content='Your Email Content', file_paths=['/path/to/file/'], file_names=['attachment.txt'])
 ```
 
-## 4 eConstant 类
+## 4 DateFormat 类
 用于获取最近的时间处理。
 
 ```bash
-from wei_office_simptool import eConstant
+from wei_office_simptool import eDateFormat
 
 # 示例代码
-#timeclass:1日期 2时间戳 3时刻
+#timeclass:1日期 date 2时间戳 timestamp 3时刻 time 4datetime
 #获取当日的日期字符串
-x=eConstant(interval_day=0,timeclass=1).get_timeparameter(Format="%Y-%m-%d")
+x=eDateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
 print(x)
 ```
 
 ## 5 FileManagement 类
 用于文件移动并且重命名。
 ```bash
 #latest_folder2 当前目录
```

### Comparing `wei_office_simptool-0.0.6/README.md` & `wei_office_simptool-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,24 +80,24 @@
 from wei_office_simptool import eSend
 
 # 示例代码
 email_sender = eSend(sender,receiver,username,password,smtpserver='smtp.126.com')
 email_sender.send_email(subject='Your Subject', e_content='Your Email Content', file_paths=['/path/to/file/'], file_names=['attachment.txt'])
 ```
 
-## 4 eConstant 类
+## 4 DateFormat 类
 用于获取最近的时间处理。
 
 ```bash
-from wei_office_simptool import eConstant
+from wei_office_simptool import eDateFormat
 
 # 示例代码
-#timeclass:1日期 2时间戳 3时刻
+#timeclass:1日期 date 2时间戳 timestamp 3时刻 time 4datetime
 #获取当日的日期字符串
-x=eConstant(interval_day=0,timeclass=1).get_timeparameter(Format="%Y-%m-%d")
+x=eDateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
 print(x)
 ```
 
 ## 5 FileManagement 类
 用于文件移动并且重命名。
 ```bash
 #latest_folder2 当前目录
```

### Comparing `wei_office_simptool-0.0.6/setup.py` & `wei_office_simptool-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 @email:thisluckyboy@126.com
 """
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='wei_office_simptool',
-    version='0.0.6',
+    version='0.0.7',
     author="Ethan Wilkins",
     author_email="thisluckyboy@126.com",
     description="一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。",  # 包的简述
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoenixlucky/wei_office_simptool",
     packages=find_packages(),
```

### Comparing `wei_office_simptool-0.0.6/tests/__init__.py` & `wei_office_simptool-0.0.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.6/tests/test_utils.py` & `wei_office_simptool-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.6/wei_office_simptool/__init__.py` & `wei_office_simptool-0.0.7/wei_office_simptool/__init__.py`

 * *Files identical despite different names*

### Comparing `wei_office_simptool-0.0.6/wei_office_simptool/utils.py` & `wei_office_simptool-0.0.7/wei_office_simptool/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,32 +335,32 @@
             smtpSsl.sendmail(self.sender, self.receiver, message.as_string())  # 发送
             smtpSsl.quit()
             print("The email with file_names has been send!")
         except Exception as e:
             print(e)
             pass
 
-class eConstant(object):
-    def __init__(self, interval_day,timeclass=1):
+class DateFormat(object):
+    def __init__(self, interval_day,timeclass='date'):
         self.interval_day = interval_day
         self.timeclass=timeclass #1日期 2时间戳 3时刻
 
     def get_timeparameter(self,Format='%Y%m%d'):
-        if self.timeclass==1:
+        if self.timeclass=='date':
             '返回日期'
             realtime = (datetime.date.today() - datetime.timedelta(days=self.interval_day)).strftime(Format)
-        elif self.timeclass==2:
+        elif self.timeclass=='timestamp':
             '返回时间戳'
             realtime = time.localtime(time.time())
-        elif self.timeclass==3:
+        elif self.timeclass=='time':
             ':return time'
             if Format=='%Y%m%d':
                 Format = '%H%M'
             realtime = time.strftime(Format, time.localtime(time.time()))
-        elif self.timeclass==4:
+        elif self.timeclass=='datetime':
             realtime= datetime.datetime.fromtimestamp(int(time.time()))
         else:
             raise TypeError("你输入的参数不合理!")
         return realtime
 
 
 class eExcel:
```

### Comparing `wei_office_simptool-0.0.6/wei_office_simptool.egg-info/PKG-INFO` & `wei_office_simptool-0.0.7/wei_office_simptool.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wei_office_simptool
-Version: 0.0.6
+Version: 0.0.7
 Summary: 一个用于简化办公工作的工具库，提供了数据库操作、Excel 处理、邮件发送、日期时间戳的格式转换、文件移动等常见功能,实现1到3行代码完成相关处理的快捷操作。
 Home-page: https://github.com/phoenixlucky/wei_office_simptool
 Author: Ethan Wilkins
 Author-email: thisluckyboy@126.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -100,24 +100,24 @@
 from wei_office_simptool import eSend
 
 # 示例代码
 email_sender = eSend(sender,receiver,username,password,smtpserver='smtp.126.com')
 email_sender.send_email(subject='Your Subject', e_content='Your Email Content', file_paths=['/path/to/file/'], file_names=['attachment.txt'])
 ```
 
-## 4 eConstant 类
+## 4 DateFormat 类
 用于获取最近的时间处理。
 
 ```bash
-from wei_office_simptool import eConstant
+from wei_office_simptool import eDateFormat
 
 # 示例代码
-#timeclass:1日期 2时间戳 3时刻
+#timeclass:1日期 date 2时间戳 timestamp 3时刻 time 4datetime
 #获取当日的日期字符串
-x=eConstant(interval_day=0,timeclass=1).get_timeparameter(Format="%Y-%m-%d")
+x=eDateFormat(interval_day=0,timeclass='date').get_timeparameter(Format="%Y-%m-%d")
 print(x)
 ```
 
 ## 5 FileManagement 类
 用于文件移动并且重命名。
 ```bash
 #latest_folder2 当前目录
```

