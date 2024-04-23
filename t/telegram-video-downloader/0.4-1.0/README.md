# Comparing `tmp/telegram-video-downloader-0.4.tar.gz` & `tmp/telegram-video-downloader-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-video-downloader-0.4.tar", last modified: Wed Apr 17 20:03:14 2024, max compression
+gzip compressed data, was "telegram-video-downloader-1.0.tar", last modified: Tue Apr 23 15:28:29 2024, max compression
```

## Comparing `telegram-video-downloader-0.4.tar` & `telegram-video-downloader-1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 20:03:14.071033 telegram-video-downloader-0.4/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:47:10.000000 telegram-video-downloader-0.4/LICENSE
--rw-rw-rw-   0        0        0      299 2024-04-17 20:03:14.067040 telegram-video-downloader-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       80 2024-04-17 15:43:12.000000 telegram-video-downloader-0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 20:03:14.071033 telegram-video-downloader-0.4/setup.cfg
--rw-rw-rw-   0        0        0      585 2024-04-17 20:03:10.000000 telegram-video-downloader-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:03:14.040470 telegram-video-downloader-0.4/telegram_video_downloader/
--rw-rw-rw-   0        0        0        0 2024-04-17 15:46:52.000000 telegram-video-downloader-0.4/telegram_video_downloader/__init__.py
--rw-rw-rw-   0        0        0     2646 2024-04-17 20:02:34.000000 telegram-video-downloader-0.4/telegram_video_downloader/app.py
-drwxrwxrwx   0        0        0        0 2024-04-17 20:03:14.062036 telegram-video-downloader-0.4/telegram_video_downloader.egg-info/
--rw-rw-rw-   0        0        0      299 2024-04-17 20:03:13.000000 telegram-video-downloader-0.4/telegram_video_downloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2024-04-17 20:03:13.000000 telegram-video-downloader-0.4/telegram_video_downloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 20:03:13.000000 telegram-video-downloader-0.4/telegram_video_downloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-04-17 20:03:13.000000 telegram-video-downloader-0.4/telegram_video_downloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-04-17 20:03:13.000000 telegram-video-downloader-0.4/telegram_video_downloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-17 20:03:13.000000 telegram-video-downloader-0.4/telegram_video_downloader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 15:28:29.091243 telegram-video-downloader-1.0/
+-rw-rw-rw-   0        0        0     1086 2024-04-23 10:40:15.000000 telegram-video-downloader-1.0/LICENSE
+-rw-rw-rw-   0        0        0      311 2024-04-23 15:28:29.088030 telegram-video-downloader-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2823 2024-04-23 15:24:38.000000 telegram-video-downloader-1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 15:28:29.092308 telegram-video-downloader-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      597 2024-04-23 15:26:59.000000 telegram-video-downloader-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:28:29.041527 telegram-video-downloader-1.0/telegram_video_downloader/
+-rw-rw-rw-   0        0        0        0 2024-04-17 15:46:52.000000 telegram-video-downloader-1.0/telegram_video_downloader/__init__.py
+-rw-rw-rw-   0        0        0     4635 2024-04-23 15:26:28.000000 telegram-video-downloader-1.0/telegram_video_downloader/app.py
+drwxrwxrwx   0        0        0        0 2024-04-23 15:28:29.086024 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-23 15:28:28.000000 telegram-video-downloader-1.0/telegram_video_downloader.egg-info/top_level.txt
```

### Comparing `telegram-video-downloader-0.4/setup.py` & `telegram-video-downloader-1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='telegram-video-downloader',
-    version='0.4',
+    version='1.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'quart',
         'telethon',
     ],
     author='David Grau Martínez',
     author_email='fe80grau@gmail.com',
-    description='Command to download a video published on Telegram',
+    description='Command to download or serve HTTP video published on Telegram',
     keywords='telegram video download',
     entry_points={
         'console_scripts': [
             'telegram-video-downloader=telegram_video_downloader.app:main',
         ],
     },
 )
```

