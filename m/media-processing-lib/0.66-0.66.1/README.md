# Comparing `tmp/media-processing-lib-0.66.tar.gz` & `tmp/media-processing-lib-0.66.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "media-processing-lib-0.66.tar", last modified: Mon Apr  8 06:57:00 2024, max compression
+gzip compressed data, was "media-processing-lib-0.66.1.tar", last modified: Tue Apr 23 19:36:41 2024, max compression
```

## Comparing `media-processing-lib-0.66.tar` & `media-processing-lib-0.66.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2022-07-21 09:37:21.000000 media-processing-lib-0.66/LICENSE.TXT
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2022-07-21 09:37:21.000000 media-processing-lib-0.66/MANIFEST.in
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2024-04-08 06:57:00.604480 media-processing-lib-0.66/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2022-07-21 09:37:21.000000 media-processing-lib-0.66/README.md
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1166 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/audio_reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/audio_resample.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      646 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/audio_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/libs/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/libs/librosa/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/librosa/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      376 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/librosa/reader.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/libs/soundfile/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/soundfile/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/libs/soundfile/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       59 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3397 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/melspectrogram.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3488 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/mpl_audio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2457 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/audio/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/collage_maker/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/collage_maker/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5034 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/collage_maker/collage_maker.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     5179 2024-04-08 06:11:46.000000 media-processing-lib-0.66/media_processing_lib/collage_maker/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      172 2024-04-08 06:38:44.000000 media-processing-lib-0.66/media_processing_lib/image/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      636 2024-04-08 06:32:57.000000 media-processing-lib-0.66/media_processing_lib/image/image_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      589 2024-04-08 06:32:21.000000 media-processing-lib-0.66/media_processing_lib/image/image_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      418 2023-05-21 09:04:49.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      260 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/libs/opencv/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/pil/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      443 2023-05-21 09:04:49.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1357 2024-01-14 11:25:57.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/resize.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      263 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/libs/pil/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/reader.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/libs/skimage/writer.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2958 2024-04-08 06:31:38.000000 media-processing-lib-0.66/media_processing_lib/image/libs_builder.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/resize/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/image/resize/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     3684 2024-04-08 06:34:08.000000 media-processing-lib-0.66/media_processing_lib/image/resize/resize.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2199 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/resize/resize_black_bars.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1435 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/resize/resize_stretch.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/image/transforms/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      154 2024-04-08 06:33:07.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1729 2024-04-08 06:51:20.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/border.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/text.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1472 2024-04-08 06:16:27.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/title.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1029 2024-04-08 06:13:02.000000 media-processing-lib-0.66/media_processing_lib/image/transforms/to_image.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3281 2023-02-12 20:48:38.000000 media-processing-lib-0.66/media_processing_lib/logger.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      495 2023-05-21 09:04:49.000000 media-processing-lib-0.66/media_processing_lib/utils.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.600480 media-processing-lib-0.66/media_processing_lib/video/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2022-07-21 09:37:21.000000 media-processing-lib-0.66/media_processing_lib/video/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/backends/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      436 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1712 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/decord.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4138 2024-01-14 11:25:57.000000 media-processing-lib-0.66/media_processing_lib/video/backends/disk_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2017 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/imageio.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      984 2023-06-03 05:14:02.000000 media-processing-lib-0.66/media_processing_lib/video/backends/memory_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1101 2023-06-02 16:21:04.000000 media-processing-lib-0.66/media_processing_lib/video/backends/mpl_video_backend.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2165 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/backends/opencv.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1526 2023-06-03 05:14:02.000000 media-processing-lib-0.66/media_processing_lib/video/backends/pims.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7220 2023-06-03 05:14:02.000000 media-processing-lib-0.66/media_processing_lib/video/mpl_video.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     4125 2023-06-02 16:21:04.000000 media-processing-lib-0.66/media_processing_lib/video/utils.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      583 2023-06-02 16:21:04.000000 media-processing-lib-0.66/media_processing_lib/video/video_reader.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      902 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/video_writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/writer/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/__init__.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/writer/imageio/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/imageio/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      372 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/imageio/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/media_processing_lib/video/writer/opencv/
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/opencv/__init__.py
--rwxrwxr-x   0 mihai     (1000) mihai     (1000)      521 2023-05-21 08:50:19.000000 media-processing-lib-0.66/media_processing_lib/video/writer/opencv/writer.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.596480 media-processing-lib-0.66/media_processing_lib.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      463 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3242 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2024-04-08 06:57:00.000000 media-processing-lib-0.66/media_processing_lib.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-08 06:11:46.000000 media-processing-lib-0.66/requirements.txt
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-08 06:57:00.604480 media-processing-lib-0.66/resources/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2022-07-21 09:37:21.000000 media-processing-lib-0.66/resources/OpenSans-Bold.ttf
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-04-08 06:57:00.604480 media-processing-lib-0.66/setup.cfg
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1789 2024-04-08 06:54:05.000000 media-processing-lib-0.66/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      485 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/LICENSE.TXT
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       53 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/MANIFEST.in
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      958 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      161 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/README.md
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.476440 media-processing-lib-0.66.1/media_processing_lib/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.476440 media-processing-lib-0.66.1/media_processing_lib/audio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      192 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/audio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     1166 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/audio/audio_reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      478 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/audio/audio_resample.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      646 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/audio/audio_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.476440 media-processing-lib-0.66.1/media_processing_lib/audio/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/audio/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.476440 media-processing-lib-0.66.1/media_processing_lib/audio/libs/librosa/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       47 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/audio/libs/librosa/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      376 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/audio/libs/librosa/reader.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.476440 media-processing-lib-0.66.1/media_processing_lib/audio/libs/soundfile/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       48 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/audio/libs/soundfile/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      312 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/audio/libs/soundfile/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.480440 media-processing-lib-0.66.1/media_processing_lib/audio/melspectrogram/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       59 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/audio/melspectrogram/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3397 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/audio/melspectrogram/melspectrogram.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3488 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/audio/mpl_audio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2457 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/audio/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.480440 media-processing-lib-0.66.1/media_processing_lib/collage_maker/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       86 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/collage_maker/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5034 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/collage_maker/collage_maker.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     5179 2024-04-08 06:11:46.000000 media-processing-lib-0.66.1/media_processing_lib/collage_maker/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.480440 media-processing-lib-0.66.1/media_processing_lib/image/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      172 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      636 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/image_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      589 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/image_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.480440 media-processing-lib-0.66.1/media_processing_lib/image/libs/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.480440 media-processing-lib-0.66.1/media_processing_lib/image/libs/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      114 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      418 2023-05-21 09:04:49.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/opencv/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      992 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/opencv/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      260 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.480440 media-processing-lib-0.66.1/media_processing_lib/image/libs/pil/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      112 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/pil/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      443 2023-05-21 09:04:49.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/pil/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1357 2024-01-14 11:25:57.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/pil/resize.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      263 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/pil/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.480440 media-processing-lib-0.66.1/media_processing_lib/image/libs/skimage/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      112 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/skimage/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      228 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/skimage/reader.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      848 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/skimage/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      242 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs/skimage/writer.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2958 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/libs_builder.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.484440 media-processing-lib-0.66.1/media_processing_lib/image/resize/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       69 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/image/resize/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     3684 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/resize/resize.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2199 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/image/resize/resize_black_bars.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1435 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/image/resize/resize_stretch.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.484440 media-processing-lib-0.66.1/media_processing_lib/image/transforms/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      154 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/transforms/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1729 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/transforms/border.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     6195 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/transforms/text.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1472 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/transforms/title.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1029 2024-04-08 07:03:14.000000 media-processing-lib-0.66.1/media_processing_lib/image/transforms/to_image.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3281 2023-02-12 20:48:38.000000 media-processing-lib-0.66.1/media_processing_lib/logger.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      495 2023-05-21 09:04:49.000000 media-processing-lib-0.66.1/media_processing_lib/utils.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.484440 media-processing-lib-0.66.1/media_processing_lib/video/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      123 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/media_processing_lib/video/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/media_processing_lib/video/backends/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      436 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1712 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/decord.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4165 2024-04-23 19:36:31.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/disk_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2017 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/imageio.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      984 2023-06-03 05:14:02.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/memory_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1101 2023-06-02 16:21:04.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/mpl_video_backend.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2165 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/opencv.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1526 2023-06-03 05:14:02.000000 media-processing-lib-0.66.1/media_processing_lib/video/backends/pims.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)     7220 2023-06-03 05:14:02.000000 media-processing-lib-0.66.1/media_processing_lib/video/mpl_video.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     4125 2023-06-02 16:21:04.000000 media-processing-lib-0.66.1/media_processing_lib/video/utils.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      583 2023-06-02 16:21:04.000000 media-processing-lib-0.66.1/media_processing_lib/video/video_reader.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      902 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/video_writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/media_processing_lib/video/writer/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        0 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/writer/__init__.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/media_processing_lib/video/writer/imageio/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/writer/imageio/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      372 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/writer/imageio/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/media_processing_lib/video/writer/opencv/
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)       48 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/writer/opencv/__init__.py
+-rwxrwxr-x   0 mihai     (1000) mihai     (1000)      521 2023-05-21 08:50:19.000000 media-processing-lib-0.66.1/media_processing_lib/video/writer/opencv/writer.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/media_processing_lib.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)      958 2024-04-23 19:36:41.000000 media-processing-lib-0.66.1/media_processing_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3242 2024-04-23 19:36:41.000000 media-processing-lib-0.66.1/media_processing_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-04-23 19:36:41.000000 media-processing-lib-0.66.1/media_processing_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-23 19:36:41.000000 media-processing-lib-0.66.1/media_processing_lib.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       21 2024-04-23 19:36:41.000000 media-processing-lib-0.66.1/media_processing_lib.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      253 2024-04-08 06:11:46.000000 media-processing-lib-0.66.1/requirements.txt
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/resources/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)   109928 2022-07-21 09:37:21.000000 media-processing-lib-0.66.1/resources/OpenSans-Bold.ttf
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       38 2024-04-23 19:36:41.488440 media-processing-lib-0.66.1/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1791 2024-04-23 19:36:37.000000 media-processing-lib-0.66.1/setup.py
```

### Comparing `media-processing-lib-0.66/media_processing_lib/audio/audio_reader.py` & `media-processing-lib-0.66.1/media_processing_lib/audio/audio_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/audio/audio_writer.py` & `media-processing-lib-0.66.1/media_processing_lib/audio/audio_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/audio/melspectrogram/melspectrogram.py` & `media-processing-lib-0.66.1/media_processing_lib/audio/melspectrogram/melspectrogram.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/audio/mpl_audio.py` & `media-processing-lib-0.66.1/media_processing_lib/audio/mpl_audio.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/audio/utils.py` & `media-processing-lib-0.66.1/media_processing_lib/audio/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/collage_maker/collage_maker.py` & `media-processing-lib-0.66.1/media_processing_lib/collage_maker/collage_maker.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/collage_maker/utils.py` & `media-processing-lib-0.66.1/media_processing_lib/collage_maker/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/image_reader.py` & `media-processing-lib-0.66.1/media_processing_lib/image/image_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/image_writer.py` & `media-processing-lib-0.66.1/media_processing_lib/image/image_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/libs/opencv/resize.py` & `media-processing-lib-0.66.1/media_processing_lib/image/libs/opencv/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/libs/pil/resize.py` & `media-processing-lib-0.66.1/media_processing_lib/image/libs/pil/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/libs/skimage/resize.py` & `media-processing-lib-0.66.1/media_processing_lib/image/libs/skimage/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/libs_builder.py` & `media-processing-lib-0.66.1/media_processing_lib/image/libs_builder.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/resize/resize.py` & `media-processing-lib-0.66.1/media_processing_lib/image/resize/resize.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/resize/resize_black_bars.py` & `media-processing-lib-0.66.1/media_processing_lib/image/resize/resize_black_bars.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/resize/resize_stretch.py` & `media-processing-lib-0.66.1/media_processing_lib/image/resize/resize_stretch.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/transforms/border.py` & `media-processing-lib-0.66.1/media_processing_lib/image/transforms/border.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/transforms/text.py` & `media-processing-lib-0.66.1/media_processing_lib/image/transforms/text.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/transforms/title.py` & `media-processing-lib-0.66.1/media_processing_lib/image/transforms/title.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/image/transforms/to_image.py` & `media-processing-lib-0.66.1/media_processing_lib/image/transforms/to_image.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/logger.py` & `media-processing-lib-0.66.1/media_processing_lib/logger.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/backends/decord.py` & `media-processing-lib-0.66.1/media_processing_lib/video/backends/decord.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/backends/disk_backend.py` & `media-processing-lib-0.66.1/media_processing_lib/video/backends/disk_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,21 +22,21 @@
         super().__init__(image_paths[0].parent)
         logger.debug2(f"DiskBackend using a cache size of {cache_size} and double buffering.")
 
         self.files = np.array([str(x) for x in image_paths])
         self.load_fns = self._build_load_fns(load_fn)
         self._buffer1 = {}
 
-        self.cache_size = cache_size
+        self.cache_size = min(len(self.files), cache_size)
         self._executor = concurrent.futures.ThreadPoolExecutor()
         self._buffer2 = {}
         self._future2 = None
         if cache_size > 0:
             # cache first N frames
-            self._future2 = self._executor.submit(self._fetch, range(cache_size))
+            self._future2 = self._executor.submit(self._fetch, range(self.cache_size))
 
     @property
     @overrides
     def is_supported_format(self) -> bool:
         if not self.path.is_dir():
             logger.warning(f"Path '{self.path}' is not a directory")
             return False
```

### Comparing `media-processing-lib-0.66/media_processing_lib/video/backends/imageio.py` & `media-processing-lib-0.66.1/media_processing_lib/video/backends/imageio.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/backends/memory_backend.py` & `media-processing-lib-0.66.1/media_processing_lib/video/backends/memory_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/backends/mpl_video_backend.py` & `media-processing-lib-0.66.1/media_processing_lib/video/backends/mpl_video_backend.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/backends/opencv.py` & `media-processing-lib-0.66.1/media_processing_lib/video/backends/opencv.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/backends/pims.py` & `media-processing-lib-0.66.1/media_processing_lib/video/backends/pims.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/mpl_video.py` & `media-processing-lib-0.66.1/media_processing_lib/video/mpl_video.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/utils.py` & `media-processing-lib-0.66.1/media_processing_lib/video/utils.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/video_reader.py` & `media-processing-lib-0.66.1/media_processing_lib/video/video_reader.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/video_writer.py` & `media-processing-lib-0.66.1/media_processing_lib/video/video_writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib/video/writer/opencv/writer.py` & `media-processing-lib-0.66.1/media_processing_lib/video/writer/opencv/writer.py`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/media_processing_lib.egg-info/SOURCES.txt` & `media-processing-lib-0.66.1/media_processing_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/resources/OpenSans-Bold.ttf` & `media-processing-lib-0.66.1/resources/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `media-processing-lib-0.66/setup.py` & `media-processing-lib-0.66.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 print("git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name")
         else:
             required.append(line)
     return required, dependency_links
 
 
 name = "media-processing-lib"
-version = "0.66"
+version = "0.66.1"
 description = "Media processing library for video, audio and images."
 url = "https://gitlab.com/mihaicristianpirvu/media-processing-lib"
 
 loc = path.abspath(path.dirname(__file__))
 with open(f"{loc}/README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
```

