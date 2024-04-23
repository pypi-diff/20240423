# Comparing `tmp/senpwai-2.1.8.tar.gz` & `tmp/senpwai-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "senpwai-2.1.8.tar", max compression
+gzip compressed data, was "senpwai-2.1.9.tar", max compression
```

## Comparing `senpwai-2.1.8.tar` & `senpwai-2.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0    35823 2024-02-27 02:54:57.469943 senpwai-2.1.8/LICENSE
--rw-r--r--   0        0        0     4435 2024-04-11 07:51:23.725066 senpwai-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     6578 2024-04-11 07:23:22.981653 senpwai-2.1.8/README.md
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.615906 senpwai-2.1.8/senpwai/__init__.py
--rw-r--r--   0        0        0       73 2024-02-27 02:54:57.616904 senpwai-2.1.8/senpwai/__main__.py
--rw-r--r--   0        0        0   167773 2024-02-27 02:54:57.620926 senpwai-2.1.8/senpwai/assets/audio/aqua-crying.mp3
--rw-r--r--   0        0        0    28037 2024-02-27 02:54:57.621905 senpwai-2.1.8/senpwai/assets/audio/bunshin-poof.mp3
--rw-r--r--   0        0        0   257620 2024-02-27 02:54:57.625930 senpwai-2.1.8/senpwai/assets/audio/gigachad.mp3
--rw-r--r--   0        0        0    45701 2024-02-27 02:54:57.628908 senpwai-2.1.8/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3
--rw-r--r--   0        0        0    38481 2024-02-27 02:54:57.630908 senpwai-2.1.8/senpwai/assets/audio/merry-chrismasu.mp3
--rw-r--r--   0        0        0    91267 2024-02-27 02:54:57.632906 senpwai-2.1.8/senpwai/assets/audio/morbin-time.mp3
--rw-r--r--   0        0        0   230876 2024-02-27 02:54:57.636908 senpwai-2.1.8/senpwai/assets/audio/one-piece-real-1.mp3
--rw-r--r--   0        0        0   184032 2024-02-27 02:54:57.639940 senpwai-2.1.8/senpwai/assets/audio/one-piece-real-2.mp3
--rw-r--r--   0        0        0   132304 2024-02-27 02:54:57.642941 senpwai-2.1.8/senpwai/assets/audio/sen-favourite.wav
--rw-r--r--   0        0        0    48659 2024-02-27 02:54:57.645909 senpwai-2.1.8/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3
--rw-r--r--   0        0        0   348653 2024-02-27 02:54:57.653909 senpwai-2.1.8/senpwai/assets/audio/what-da-hell.mp3
--rw-r--r--   0        0        0   463516 2024-02-27 02:54:57.664911 senpwai-2.1.8/senpwai/assets/audio/za-warudo.mp3
--rw-r--r--   0        0        0   348902 2024-02-27 02:54:57.671911 senpwai-2.1.8/senpwai/assets/background-images/about.jpg
--rw-r--r--   0        0        0   617045 2024-02-27 02:54:57.681432 senpwai-2.1.8/senpwai/assets/background-images/chopper-crying.png
--rw-r--r--   0        0        0   392654 2024-02-27 02:54:57.688431 senpwai-2.1.8/senpwai/assets/background-images/chosen-anime.jpg
--rw-r--r--   0        0        0   172353 2024-02-27 02:54:57.692430 senpwai-2.1.8/senpwai/assets/background-images/christmas.jpg
--rw-r--r--   0        0        0   884962 2024-02-27 02:54:57.703431 senpwai-2.1.8/senpwai/assets/background-images/downloads.png
--rw-r--r--   0        0        0   357703 2024-02-27 02:54:57.709432 senpwai-2.1.8/senpwai/assets/background-images/search.jpg
--rw-r--r--   0        0        0   247094 2024-02-27 02:54:57.714432 senpwai-2.1.8/senpwai/assets/background-images/settings.jpg
--rw-r--r--   0        0        0   405642 2024-02-27 02:54:57.721432 senpwai-2.1.8/senpwai/assets/background-images/update.jpg
--rw-r--r--   0        0        0     1227 2024-02-27 02:54:57.722432 senpwai-2.1.8/senpwai/assets/download-icons/cancel.png
--rw-r--r--   0        0        0      757 2024-02-27 02:54:57.723432 senpwai-2.1.8/senpwai/assets/download-icons/down.png
--rw-r--r--   0        0        0      694 2024-02-27 02:54:57.724431 senpwai-2.1.8/senpwai/assets/download-icons/pause.png
--rw-r--r--   0        0        0      920 2024-02-27 02:54:57.725432 senpwai-2.1.8/senpwai/assets/download-icons/resume.png
--rw-r--r--   0        0        0      781 2024-02-27 02:54:57.726437 senpwai-2.1.8/senpwai/assets/download-icons/trash.png
--rw-r--r--   0        0        0      641 2024-02-27 02:54:57.727433 senpwai-2.1.8/senpwai/assets/download-icons/up.png
--rw-r--r--   0        0        0    27409 2024-02-27 02:54:57.729464 senpwai-2.1.8/senpwai/assets/link-icons/discord.png
--rw-r--r--   0        0        0    16226 2024-02-27 02:54:57.730425 senpwai-2.1.8/senpwai/assets/link-icons/github-sponsors.svg
--rw-r--r--   0        0        0    22763 2024-02-27 02:54:57.731426 senpwai-2.1.8/senpwai/assets/link-icons/github.png
--rw-r--r--   0        0        0    17064 2024-02-27 02:54:57.732430 senpwai-2.1.8/senpwai/assets/link-icons/patreon.png
--rw-r--r--   0        0        0    35215 2024-02-27 02:54:57.734432 senpwai-2.1.8/senpwai/assets/link-icons/reddit.png
--rw-r--r--   0        0        0    49259 2024-02-27 02:54:57.736432 senpwai-2.1.8/senpwai/assets/mascots/1.png
--rw-r--r--   0        0        0    69802 2024-02-27 02:54:57.739434 senpwai-2.1.8/senpwai/assets/mascots/2.png
--rw-r--r--   0        0        0     4258 2024-02-27 02:54:57.740433 senpwai-2.1.8/senpwai/assets/misc/folder.png
--rw-r--r--   0        0        0   625301 2024-02-27 02:54:57.754464 senpwai-2.1.8/senpwai/assets/misc/loading.gif
--rw-r--r--   0        0        0    89481 2024-02-27 02:54:57.757459 senpwai-2.1.8/senpwai/assets/misc/sadge-piece.gif
--rw-r--r--   0        0        0    99300 2024-02-27 02:54:57.760429 senpwai-2.1.8/senpwai/assets/misc/senpwai-icon.ico
--rw-r--r--   0        0        0     8044 2024-02-27 02:54:57.761438 senpwai-2.1.8/senpwai/assets/misc/task-complete.png
--rw-r--r--   0        0        0    16336 2024-02-27 02:54:57.763436 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/about.png
--rw-r--r--   0        0        0     7749 2024-02-27 02:54:57.764436 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/downloads.png
--rw-r--r--   0        0        0    19245 2024-02-27 02:54:57.765437 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/search.png
--rw-r--r--   0        0        0    10851 2024-02-27 02:54:57.767439 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/settings.png
--rw-r--r--   0        0        0     6454 2024-02-27 02:54:57.768437 senpwai-2.1.8/senpwai/assets/navigation-bar-icons/update.png
--rw-r--r--   0        0        0    96597 2024-02-27 02:54:57.772439 senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/hentai-addict.png
--rw-r--r--   0        0        0    19936 2024-02-27 02:54:57.773439 senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png
--rw-r--r--   0        0        0    52908 2024-02-27 02:54:57.774438 senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/sen.png
--rw-r--r--   0        0        0     1711 2024-04-11 00:05:53.611597 senpwai-2.1.8/senpwai/main.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.777958 senpwai-2.1.8/senpwai/scrapers/__init__.py
--rw-r--r--   0        0        0      109 2024-04-10 16:10:21.056706 senpwai-2.1.8/senpwai/scrapers/gogo/__init__.py
--rw-r--r--   0        0        0     1175 2024-04-11 03:49:40.496718 senpwai-2.1.8/senpwai/scrapers/gogo/constants.py
--rw-r--r--   0        0        0     5196 2024-02-27 02:54:57.781957 senpwai-2.1.8/senpwai/scrapers/gogo/hls.py
--rw-r--r--   0        0        0     8501 2024-04-11 04:42:36.370908 senpwai-2.1.8/senpwai/scrapers/gogo/main.py
--rw-r--r--   0        0        0       78 2024-03-05 08:24:06.852246 senpwai-2.1.8/senpwai/scrapers/pahe/__init__.py
--rw-r--r--   0        0        0     1204 2024-03-05 08:24:06.852246 senpwai-2.1.8/senpwai/scrapers/pahe/constants.py
--rw-r--r--   0        0        0    13674 2024-04-10 16:16:34.960579 senpwai-2.1.8/senpwai/scrapers/pahe/main.py
--rw-r--r--   0        0        0    29198 2024-04-11 04:40:38.021786 senpwai-2.1.8/senpwai/scrapers/test.py
--rw-r--r--   0        0        0       81 2024-02-27 02:54:57.788962 senpwai-2.1.8/senpwai/senpcli/__main__.py
--rw-r--r--   0        0        0    24218 2024-04-11 07:19:23.047038 senpwai-2.1.8/senpwai/senpcli/main.py
--rw-r--r--   0        0        0        0 2024-04-09 01:14:15.123895 senpwai-2.1.8/senpwai/utils/__init__.py
--rw-r--r--   0        0        0    14940 2024-04-11 04:33:27.026164 senpwai-2.1.8/senpwai/utils/classes.py
--rw-r--r--   0        0        0    23014 2024-04-11 07:39:13.161228 senpwai-2.1.8/senpwai/utils/scraper.py
--rw-r--r--   0        0        0     9605 2024-04-11 07:51:23.726065 senpwai-2.1.8/senpwai/utils/static.py
--rw-r--r--   0        0        0    25727 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/utils/widgets.py
--rw-r--r--   0        0        0        0 2024-02-27 02:54:57.800965 senpwai-2.1.8/senpwai/windows/__init__.py
--rw-r--r--   0        0        0     8097 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/about.py
--rw-r--r--   0        0        0     2670 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/abstracts.py
--rw-r--r--   0        0        0    20740 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/chosen_anime.py
--rw-r--r--   0        0        0    54312 2024-04-11 04:19:41.774782 senpwai-2.1.8/senpwai/windows/download.py
--rw-r--r--   0        0        0    10393 2024-02-27 02:54:57.808959 senpwai-2.1.8/senpwai/windows/main.py
--rw-r--r--   0        0        0    11995 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/misc.py
--rw-r--r--   0        0        0    18032 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/search.py
--rw-r--r--   0        0        0    27126 2024-03-05 08:24:06.867880 senpwai-2.1.8/senpwai/windows/settings.py
--rw-r--r--   0        0        0     7828 1970-01-01 00:00:00.000000 senpwai-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2024-02-27 02:54:57.469943 senpwai-2.1.9/LICENSE
+-rw-r--r--   0        0        0     4435 2024-04-23 16:44:09.980267 senpwai-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6578 2024-04-11 08:01:52.307603 senpwai-2.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.615906 senpwai-2.1.9/senpwai/__init__.py
+-rw-r--r--   0        0        0       73 2024-02-27 02:54:57.616904 senpwai-2.1.9/senpwai/__main__.py
+-rw-r--r--   0        0        0   167773 2024-02-27 02:54:57.620926 senpwai-2.1.9/senpwai/assets/audio/aqua-crying.mp3
+-rw-r--r--   0        0        0    28037 2024-02-27 02:54:57.621905 senpwai-2.1.9/senpwai/assets/audio/bunshin-poof.mp3
+-rw-r--r--   0        0        0   257620 2024-02-27 02:54:57.625930 senpwai-2.1.9/senpwai/assets/audio/gigachad.mp3
+-rw-r--r--   0        0        0    45701 2024-02-27 02:54:57.628908 senpwai-2.1.9/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3
+-rw-r--r--   0        0        0    38481 2024-02-27 02:54:57.630908 senpwai-2.1.9/senpwai/assets/audio/merry-chrismasu.mp3
+-rw-r--r--   0        0        0    91267 2024-02-27 02:54:57.632906 senpwai-2.1.9/senpwai/assets/audio/morbin-time.mp3
+-rw-r--r--   0        0        0   230876 2024-02-27 02:54:57.636908 senpwai-2.1.9/senpwai/assets/audio/one-piece-real-1.mp3
+-rw-r--r--   0        0        0   184032 2024-02-27 02:54:57.639940 senpwai-2.1.9/senpwai/assets/audio/one-piece-real-2.mp3
+-rw-r--r--   0        0        0   132304 2024-02-27 02:54:57.642941 senpwai-2.1.9/senpwai/assets/audio/sen-favourite.wav
+-rw-r--r--   0        0        0    48659 2024-02-27 02:54:57.645909 senpwai-2.1.9/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3
+-rw-r--r--   0        0        0   348653 2024-02-27 02:54:57.653909 senpwai-2.1.9/senpwai/assets/audio/what-da-hell.mp3
+-rw-r--r--   0        0        0   463516 2024-02-27 02:54:57.664911 senpwai-2.1.9/senpwai/assets/audio/za-warudo.mp3
+-rw-r--r--   0        0        0   348902 2024-02-27 02:54:57.671911 senpwai-2.1.9/senpwai/assets/background-images/about.jpg
+-rw-r--r--   0        0        0   617045 2024-02-27 02:54:57.681432 senpwai-2.1.9/senpwai/assets/background-images/chopper-crying.png
+-rw-r--r--   0        0        0   392654 2024-02-27 02:54:57.688431 senpwai-2.1.9/senpwai/assets/background-images/chosen-anime.jpg
+-rw-r--r--   0        0        0   172353 2024-02-27 02:54:57.692430 senpwai-2.1.9/senpwai/assets/background-images/christmas.jpg
+-rw-r--r--   0        0        0   884962 2024-02-27 02:54:57.703431 senpwai-2.1.9/senpwai/assets/background-images/downloads.png
+-rw-r--r--   0        0        0   357703 2024-02-27 02:54:57.709432 senpwai-2.1.9/senpwai/assets/background-images/search.jpg
+-rw-r--r--   0        0        0   247094 2024-02-27 02:54:57.714432 senpwai-2.1.9/senpwai/assets/background-images/settings.jpg
+-rw-r--r--   0        0        0   405642 2024-02-27 02:54:57.721432 senpwai-2.1.9/senpwai/assets/background-images/update.jpg
+-rw-r--r--   0        0        0     1227 2024-02-27 02:54:57.722432 senpwai-2.1.9/senpwai/assets/download-icons/cancel.png
+-rw-r--r--   0        0        0      757 2024-02-27 02:54:57.723432 senpwai-2.1.9/senpwai/assets/download-icons/down.png
+-rw-r--r--   0        0        0      694 2024-02-27 02:54:57.724431 senpwai-2.1.9/senpwai/assets/download-icons/pause.png
+-rw-r--r--   0        0        0      920 2024-02-27 02:54:57.725432 senpwai-2.1.9/senpwai/assets/download-icons/resume.png
+-rw-r--r--   0        0        0      781 2024-02-27 02:54:57.726437 senpwai-2.1.9/senpwai/assets/download-icons/trash.png
+-rw-r--r--   0        0        0      641 2024-02-27 02:54:57.727433 senpwai-2.1.9/senpwai/assets/download-icons/up.png
+-rw-r--r--   0        0        0    27409 2024-02-27 02:54:57.729464 senpwai-2.1.9/senpwai/assets/link-icons/discord.png
+-rw-r--r--   0        0        0    16226 2024-02-27 02:54:57.730425 senpwai-2.1.9/senpwai/assets/link-icons/github-sponsors.svg
+-rw-r--r--   0        0        0    22763 2024-02-27 02:54:57.731426 senpwai-2.1.9/senpwai/assets/link-icons/github.png
+-rw-r--r--   0        0        0    17064 2024-02-27 02:54:57.732430 senpwai-2.1.9/senpwai/assets/link-icons/patreon.png
+-rw-r--r--   0        0        0    35215 2024-02-27 02:54:57.734432 senpwai-2.1.9/senpwai/assets/link-icons/reddit.png
+-rw-r--r--   0        0        0    49259 2024-02-27 02:54:57.736432 senpwai-2.1.9/senpwai/assets/mascots/1.png
+-rw-r--r--   0        0        0    69802 2024-02-27 02:54:57.739434 senpwai-2.1.9/senpwai/assets/mascots/2.png
+-rw-r--r--   0        0        0     4258 2024-02-27 02:54:57.740433 senpwai-2.1.9/senpwai/assets/misc/folder.png
+-rw-r--r--   0        0        0   625301 2024-02-27 02:54:57.754464 senpwai-2.1.9/senpwai/assets/misc/loading.gif
+-rw-r--r--   0        0        0    89481 2024-02-27 02:54:57.757459 senpwai-2.1.9/senpwai/assets/misc/sadge-piece.gif
+-rw-r--r--   0        0        0    99300 2024-02-27 02:54:57.760429 senpwai-2.1.9/senpwai/assets/misc/senpwai-icon.ico
+-rw-r--r--   0        0        0     8044 2024-02-27 02:54:57.761438 senpwai-2.1.9/senpwai/assets/misc/task-complete.png
+-rw-r--r--   0        0        0    16336 2024-02-27 02:54:57.763436 senpwai-2.1.9/senpwai/assets/navigation-bar-icons/about.png
+-rw-r--r--   0        0        0     7749 2024-02-27 02:54:57.764436 senpwai-2.1.9/senpwai/assets/navigation-bar-icons/downloads.png
+-rw-r--r--   0        0        0    19245 2024-02-27 02:54:57.765437 senpwai-2.1.9/senpwai/assets/navigation-bar-icons/search.png
+-rw-r--r--   0        0        0    10851 2024-02-27 02:54:57.767439 senpwai-2.1.9/senpwai/assets/navigation-bar-icons/settings.png
+-rw-r--r--   0        0        0     6454 2024-02-27 02:54:57.768437 senpwai-2.1.9/senpwai/assets/navigation-bar-icons/update.png
+-rw-r--r--   0        0        0    96597 2024-02-27 02:54:57.772439 senpwai-2.1.9/senpwai/assets/reviewer-profile-pics/hentai-addict.png
+-rw-r--r--   0        0        0    19936 2024-02-27 02:54:57.773439 senpwai-2.1.9/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png
+-rw-r--r--   0        0        0    52908 2024-02-27 02:54:57.774438 senpwai-2.1.9/senpwai/assets/reviewer-profile-pics/sen.png
+-rw-r--r--   0        0        0     1711 2024-04-11 08:01:52.314391 senpwai-2.1.9/senpwai/main.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.777958 senpwai-2.1.9/senpwai/scrapers/__init__.py
+-rw-r--r--   0        0        0      109 2024-04-10 16:10:21.056706 senpwai-2.1.9/senpwai/scrapers/gogo/__init__.py
+-rw-r--r--   0        0        0     1175 2024-04-23 16:42:41.403018 senpwai-2.1.9/senpwai/scrapers/gogo/constants.py
+-rw-r--r--   0        0        0     5196 2024-02-27 02:54:57.781957 senpwai-2.1.9/senpwai/scrapers/gogo/hls.py
+-rw-r--r--   0        0        0     8827 2024-04-23 16:37:18.414660 senpwai-2.1.9/senpwai/scrapers/gogo/main.py
+-rw-r--r--   0        0        0       78 2024-03-05 08:24:06.852246 senpwai-2.1.9/senpwai/scrapers/pahe/__init__.py
+-rw-r--r--   0        0        0     1204 2024-03-05 08:24:06.852246 senpwai-2.1.9/senpwai/scrapers/pahe/constants.py
+-rw-r--r--   0        0        0    13302 2024-04-23 16:21:08.818378 senpwai-2.1.9/senpwai/scrapers/pahe/main.py
+-rw-r--r--   0        0        0    28485 2024-04-23 16:21:08.849387 senpwai-2.1.9/senpwai/scrapers/test.py
+-rw-r--r--   0        0        0       81 2024-02-27 02:54:57.788962 senpwai-2.1.9/senpwai/senpcli/__main__.py
+-rw-r--r--   0        0        0    24218 2024-04-11 08:01:52.319906 senpwai-2.1.9/senpwai/senpcli/main.py
+-rw-r--r--   0        0        0        0 2024-04-09 01:14:15.123895 senpwai-2.1.9/senpwai/utils/__init__.py
+-rw-r--r--   0        0        0    14940 2024-04-11 08:01:52.321115 senpwai-2.1.9/senpwai/utils/classes.py
+-rw-r--r--   0        0        0    23014 2024-04-23 16:33:52.208095 senpwai-2.1.9/senpwai/utils/scraper.py
+-rw-r--r--   0        0        0     9605 2024-04-23 16:44:09.981268 senpwai-2.1.9/senpwai/utils/static.py
+-rw-r--r--   0        0        0    25727 2024-03-05 08:24:06.867880 senpwai-2.1.9/senpwai/utils/widgets.py
+-rw-r--r--   0        0        0        0 2024-02-27 02:54:57.800965 senpwai-2.1.9/senpwai/windows/__init__.py
+-rw-r--r--   0        0        0     8097 2024-03-05 08:24:06.867880 senpwai-2.1.9/senpwai/windows/about.py
+-rw-r--r--   0        0        0     2670 2024-03-05 08:24:06.867880 senpwai-2.1.9/senpwai/windows/abstracts.py
+-rw-r--r--   0        0        0    20740 2024-03-05 08:24:06.867880 senpwai-2.1.9/senpwai/windows/chosen_anime.py
+-rw-r--r--   0        0        0    54447 2024-04-23 16:24:18.626525 senpwai-2.1.9/senpwai/windows/download.py
+-rw-r--r--   0        0        0    10393 2024-02-27 02:54:57.808959 senpwai-2.1.9/senpwai/windows/main.py
+-rw-r--r--   0        0        0    11995 2024-03-05 08:24:06.867880 senpwai-2.1.9/senpwai/windows/misc.py
+-rw-r--r--   0        0        0    18032 2024-03-05 08:24:06.867880 senpwai-2.1.9/senpwai/windows/search.py
+-rw-r--r--   0        0        0    27126 2024-03-05 08:24:06.867880 senpwai-2.1.9/senpwai/windows/settings.py
+-rw-r--r--   0        0        0     7828 1970-01-01 00:00:00.000000 senpwai-2.1.9/PKG-INFO
```

### Comparing `senpwai-2.1.8/LICENSE` & `senpwai-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/pyproject.toml` & `senpwai-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "senpwai"
-version = "2.1.8"
+version = "2.1.9"
 description = "A desktop app for tracking and batch downloading anime"
 authors = ["SenZmaKi <senzmaki@gmail.com>"]
 license = "GPL v3"
 readme = "README.md"
 include = ["senpwai/assets"]
 packages = [{ include = "senpwai" }, { include = "senpcli", from = "senpwai" }]
 exclude = ["src/**/test.py"]
```

### Comparing `senpwai-2.1.8/README.md` & `senpwai-2.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 - **Other**
 
 [Build from source](#building-from-source).
 
 ## Features
 
-- Download any anime from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to).
+- Download any anime from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.so).
 - Keep track of an anime and automatically download new episodes when they release.
 - Download a complete season or episodes within a range (e.g., 69-420).
 - Choose between video qualities: 360p, 480p (Gogoanime only), 720p, or 1080p.
 - Download in sub or dub (if available) depending on the user's preference.
 - Automatically detects episodes you already have and avoids re-downloading them.
 - Robust and graceful download error management.
 - GUI and [CLI](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md).
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 [one-piece-screenshot]## Installation - **Cross-platform (Linux, Mac, Windows
 10/11)** Needs [Python 3.11](https://www.python.org/downloads/release/python-
 3111) installed. ```bash pip install senpwai ``` - **Windows 10/11** Download
 [the setup](https://github.com/SenZmaKi/Senpwai/releases/latest/download/
 Senpwai-setup.exe) then run it. - **Android** Check [Senpcli](https://
 github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md) - **Other**
 [Build from source](#building-from-source). ## Features - Download any anime
-from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to). -
+from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.so). -
 Keep track of an anime and automatically download new episodes when they
 release. - Download a complete season or episodes within a range (e.g., 69-
 420). - Choose between video qualities: 360p, 480p (Gogoanime only), 720p, or
 1080p. - Download in sub or dub (if available) depending on the user's
 preference. - Automatically detects episodes you already have and avoids re-
 downloading them. - Robust and graceful download error management. - GUI and
 [CLI](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md).
```

### Comparing `senpwai-2.1.8/senpwai/assets/audio/aqua-crying.mp3` & `senpwai-2.1.9/senpwai/assets/audio/aqua-crying.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/bunshin-poof.mp3` & `senpwai-2.1.9/senpwai/assets/audio/bunshin-poof.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/gigachad.mp3` & `senpwai-2.1.9/senpwai/assets/audio/gigachad.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3` & `senpwai-2.1.9/senpwai/assets/audio/kage-bunshin-no-jutsu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/merry-chrismasu.mp3` & `senpwai-2.1.9/senpwai/assets/audio/merry-chrismasu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/morbin-time.mp3` & `senpwai-2.1.9/senpwai/assets/audio/morbin-time.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/one-piece-real-1.mp3` & `senpwai-2.1.9/senpwai/assets/audio/one-piece-real-1.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/one-piece-real-2.mp3` & `senpwai-2.1.9/senpwai/assets/audio/one-piece-real-2.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/sen-favourite.wav` & `senpwai-2.1.9/senpwai/assets/audio/sen-favourite.wav`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3` & `senpwai-2.1.9/senpwai/assets/audio/toki-wa-ugoki-dasu.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/what-da-hell.mp3` & `senpwai-2.1.9/senpwai/assets/audio/what-da-hell.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/audio/za-warudo.mp3` & `senpwai-2.1.9/senpwai/assets/audio/za-warudo.mp3`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/about.jpg` & `senpwai-2.1.9/senpwai/assets/background-images/about.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/chopper-crying.png` & `senpwai-2.1.9/senpwai/assets/background-images/chopper-crying.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/chosen-anime.jpg` & `senpwai-2.1.9/senpwai/assets/background-images/chosen-anime.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/christmas.jpg` & `senpwai-2.1.9/senpwai/assets/background-images/christmas.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/downloads.png` & `senpwai-2.1.9/senpwai/assets/background-images/downloads.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/search.jpg` & `senpwai-2.1.9/senpwai/assets/background-images/search.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/settings.jpg` & `senpwai-2.1.9/senpwai/assets/background-images/settings.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/background-images/update.jpg` & `senpwai-2.1.9/senpwai/assets/background-images/update.jpg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/download-icons/cancel.png` & `senpwai-2.1.9/senpwai/assets/download-icons/cancel.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/download-icons/down.png` & `senpwai-2.1.9/senpwai/assets/download-icons/down.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/download-icons/pause.png` & `senpwai-2.1.9/senpwai/assets/download-icons/pause.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/download-icons/resume.png` & `senpwai-2.1.9/senpwai/assets/download-icons/resume.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/download-icons/trash.png` & `senpwai-2.1.9/senpwai/assets/download-icons/trash.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/download-icons/up.png` & `senpwai-2.1.9/senpwai/assets/download-icons/up.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/link-icons/discord.png` & `senpwai-2.1.9/senpwai/assets/link-icons/discord.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/link-icons/github-sponsors.svg` & `senpwai-2.1.9/senpwai/assets/link-icons/github-sponsors.svg`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/link-icons/github.png` & `senpwai-2.1.9/senpwai/assets/link-icons/github.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/link-icons/patreon.png` & `senpwai-2.1.9/senpwai/assets/link-icons/patreon.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/link-icons/reddit.png` & `senpwai-2.1.9/senpwai/assets/link-icons/reddit.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/mascots/1.png` & `senpwai-2.1.9/senpwai/assets/mascots/1.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/mascots/2.png` & `senpwai-2.1.9/senpwai/assets/mascots/2.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/misc/folder.png` & `senpwai-2.1.9/senpwai/assets/misc/folder.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/misc/loading.gif` & `senpwai-2.1.9/senpwai/assets/misc/loading.gif`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/misc/sadge-piece.gif` & `senpwai-2.1.9/senpwai/assets/misc/sadge-piece.gif`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/misc/senpwai-icon.ico` & `senpwai-2.1.9/senpwai/assets/misc/senpwai-icon.ico`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/misc/task-complete.png` & `senpwai-2.1.9/senpwai/assets/misc/task-complete.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/about.png` & `senpwai-2.1.9/senpwai/assets/navigation-bar-icons/about.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/downloads.png` & `senpwai-2.1.9/senpwai/assets/navigation-bar-icons/downloads.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/search.png` & `senpwai-2.1.9/senpwai/assets/navigation-bar-icons/search.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/settings.png` & `senpwai-2.1.9/senpwai/assets/navigation-bar-icons/settings.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/navigation-bar-icons/update.png` & `senpwai-2.1.9/senpwai/assets/navigation-bar-icons/update.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/hentai-addict.png` & `senpwai-2.1.9/senpwai/assets/reviewer-profile-pics/hentai-addict.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png` & `senpwai-2.1.9/senpwai/assets/reviewer-profile-pics/morbius-is-peak.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/assets/reviewer-profile-pics/sen.png` & `senpwai-2.1.9/senpwai/assets/reviewer-profile-pics/sen.png`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/main.py` & `senpwai-2.1.9/senpwai/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/scrapers/gogo/constants.py` & `senpwai-2.1.9/senpwai/scrapers/gogo/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 GOGO = "gogo"
-GOGO_HOME_URL = "https://anitaku.to"
+GOGO_HOME_URL = "https://anitaku.so"
 AJAX_ENTRY_POINT = "https://ajax.gogocdn.net"
 AJAX_SEARCH_URL = f"{AJAX_ENTRY_POINT}/site/loadAjaxSearch?keyword="
 AJAX_LOAD_EPS_URL = (
     f"{AJAX_ENTRY_POINT}/ajax/load-list-episode?ep_start={{}}&ep_end={{}}&id={{}}"
 )
 FULL_SITE_NAME = "Gogoanime"
 DUB_EXTENSION = " (Dub)"
```

### Comparing `senpwai-2.1.8/senpwai/scrapers/gogo/hls.py` & `senpwai-2.1.9/senpwai/scrapers/gogo/hls.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/scrapers/gogo/main.py` & `senpwai-2.1.9/senpwai/scrapers/gogo/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,36 +133,43 @@
             progress_update_callback(1)
         return total_size
 
 
 def get_anime_page_content(anime_page_link: str) -> tuple[bytes, str]:
     global FIRST_REQUEST
     global GOGO_HOME_URL
-    if FIRST_REQUEST:
-        try:
-            FIRST_REQUEST = False
-            response = CLIENT.get(
-                anime_page_link,
-                exceptions_to_raise=(DomainNameError, KeyboardInterrupt),
-            )
-            if response.status_code not in RESOURCE_MOVED_STATUS_CODES:
-                return response.content, anime_page_link
-            new_anime_page_link = response.headers.get("Location", GOGO_HOME_URL)
-            # The url in location seems to be in http instead of https but the http one doesn't work
-            if new_anime_page_link != GOGO_HOME_URL:
-                new_anime_page_link = new_anime_page_link.replace("http://", "https://")
-            match = cast(re.Match[str], BASE_URL_REGEX.search(new_anime_page_link))
-            GOGO_HOME_URL = match.group(1)
-            return get_anime_page_content(new_anime_page_link)
-        except DomainNameError:
-            prev_home_url = GOGO_HOME_URL
-            GOGO_HOME_URL = get_new_home_url_from_readme(FULL_SITE_NAME)
-            return get_anime_page_content(
-                anime_page_link.replace(prev_home_url, GOGO_HOME_URL)
-            )
+    try:
+        response = CLIENT.get(
+            anime_page_link,
+            exceptions_to_raise=(DomainNameError, KeyboardInterrupt),
+        )
+        if response.status_code not in RESOURCE_MOVED_STATUS_CODES:
+            return response.content, anime_page_link
+        new_anime_page_link = response.headers.get("Location", anime_page_link)
+        # The url in location seems to be in http instead of https but the http one doesn't work
+        new_anime_page_link = new_anime_page_link.replace("http://", "https://")
+        # If the link is not different we assume they changed their domain name but didn't pass
+        # the link with the new one in the location headers
+        if new_anime_page_link == anime_page_link:
+            raise DomainNameError(Exception("Received resource moved status code"))
+        match = cast(re.Match[str], BASE_URL_REGEX.search(new_anime_page_link))
+        GOGO_HOME_URL = match.group(1)
+        return get_anime_page_content(new_anime_page_link)
+    except DomainNameError:
+        # Only check for a new domain name in the readme if this was the first raised error
+        # otherwise sth else probably broke
+        if not FIRST_REQUEST:
+            raise
+        FIRST_REQUEST = False
+        prev_home_url = GOGO_HOME_URL
+        GOGO_HOME_URL = get_new_home_url_from_readme(FULL_SITE_NAME)
+        return get_anime_page_content(
+            anime_page_link.replace(prev_home_url, GOGO_HOME_URL)
+        )
+
     response = CLIENT.get(
         anime_page_link,
     )
     return response.content, anime_page_link
 
 
 def extract_anime_metadata(anime_page_content: bytes) -> AnimeMetadata:
```

### Comparing `senpwai-2.1.8/senpwai/scrapers/pahe/constants.py` & `senpwai-2.1.9/senpwai/scrapers/pahe/constants.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/scrapers/pahe/main.py` & `senpwai-2.1.9/senpwai/scrapers/pahe/main.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,372 +1,372 @@
-import re
-import math
-from typing import Any, Callable, cast
-from requests import Response
-from bs4 import BeautifulSoup, Tag
-from senpwai.utils.scraper import (
-    CLIENT,
-    PARSER,
-    AnimeMetadata,
-    DomainNameError,
-    ProgressFunction,
-    get_new_home_url_from_readme,
-    match_quality,
-)
-from .constants import (
-    CHAR_MAP_BASE,
-    CHAR_MAP_DIGITS,
-    PAHE_HOME_URL,
-    FULL_SITE_NAME,
-    API_ENTRY_POINT,
-    ANIME_PAGE_URL,
-    LOAD_EPISODES_URL,
-    DUB_PATTERN,
-    EPISODE_PAGE_URL,
-    EPISODE_SIZE_REGEX,
-    KWIK_PAGE_REGEX,
-    PARAM_REGEX,
-)
-
-FIRST_REQUEST = True
-COOKIES = {"__ddg1_": "", "__ddg2_": ""}
-"""
-For some reason these cookies just need to be set as in they don't even need to be valid
-If something crashes, try updating to something like: 
-COOKIES = {
-    "__ddg1_": f"; Expires=Tue, 19 Jan 2038 03:14:07 GMT; Domain={PAHE_DOMAIN}; Path=/",
-    "__ddg2_": f"; Expires=Tue, 19 Jan 2038 03:14:07 GMT; Domain={PAHE_DOMAIN}; Path=/",
-}
-"""
-
-
-def site_request(url: str) -> Response:
-    """
-    For requests that go specifically to the domain animepahe.ru instead of e.g., pahe.win or kwik.si
-    Typically these requests need the cookies
-    """
-    try:
-        # We only want to handle the domain change incase this is the first request
-        # This is to avoid raising DomainNameError when the something else broke instead
-        global FIRST_REQUEST
-        if FIRST_REQUEST:
-            FIRST_REQUEST = False
-            response = CLIENT.get(
-                url,
-                cookies=COOKIES,
-                exceptions_to_raise=(DomainNameError, KeyboardInterrupt),
-            )
-        else:
-            response = CLIENT.get(url, cookies=COOKIES)
-        COOKIES.update(response.cookies)
-    except DomainNameError:
-        global PAHE_HOME_URL
-        PAHE_HOME_URL = get_new_home_url_from_readme(FULL_SITE_NAME)
-        return site_request(url)
-    return response
-
-
-def search(keyword: str) -> list[dict[str, str]]:
-    search_url = f"{API_ENTRY_POINT}search&q={keyword}"
-    response = site_request(search_url)
-    decoded = cast(dict, response.json())
-    # The search api endpoint won't return json containing the data key if no results are found
-    return decoded.get("data", [])
-
-
-def extract_anime_title_page_link_and_id(
-    result: dict[str, str],
-) -> tuple[str, str, str]:
-    anime_id = result["session"]
-    title = result["title"]
-    page_link = ANIME_PAGE_URL.format(anime_id)
-    return title, page_link, anime_id
-
-
-def get_episode_pages_info(
-    anime_page_link: str, start_episode: int, end_episode: int
-) -> tuple[int, int, int, dict[str, Any]]:
-    page_url = LOAD_EPISODES_URL.format(anime_page_link, 1)
-    decoded = site_request(page_url).json()
-    per_page: int = decoded["per_page"]
-    start_page = math.ceil(start_episode / per_page)
-    end_page = math.ceil(end_episode / per_page)
-    episode_page_count = (end_page - start_page) + 1
-    return start_page, end_page, episode_page_count, decoded
-
-
-class GetEpisodePageLinks(ProgressFunction):
-    def __init__(self) -> None:
-        super().__init__()
-
-    @staticmethod
-    def generate_episode_page_links(
-        start_episode: int,
-        end_episode: int,
-        first_episode: int,
-        episodes_data: list[dict[str, Any]],
-        anime_id: str,
-    ):
-        # These values should theoritically never remain as they are unless something crashes
-        # as in both of the ifs in the for loop should always eventually evaluate to True
-        start_idx = 0
-        end_idx = 0
-
-        for idx, episode in enumerate(episodes_data):
-            # Some times for sequels animepahe continues the episode numbers from the last episode of the previous season
-            # For instance  "Boku no Hero Academia 2nd Season" episode 1 is shown as episode 14
-            # So we do episode - (first_episode - 1) to get the real episode number e.g.,
-            # 14 - (14 - 1) = 1
-            # 15 - (14 - 1) = 2 and so on
-            episode_num = episode["episode"] - (first_episode - 1)
-            if episode_num == start_episode:
-                start_idx = idx
-            if episode_num == end_episode:
-                end_idx = idx
-                break
-        episodes_data = episodes_data[start_idx : end_idx + 1]
-        episode_sessions = [episode["session"] for episode in episodes_data]
-        return [
-            EPISODE_PAGE_URL.format(anime_id, episode_session)
-            for episode_session in episode_sessions
-        ]
-
-    # Retrieves a list of the episode page links (not download links)
-    def get_episode_page_links(
-        self,
-        start_episode: int,
-        end_episode: int,
-        start_page_num: int,
-        end_page_num: int,
-        first_page: dict[str, Any],
-        anime_page_link: str,
-        anime_id: str,
-        progress_update_callback: Callable = lambda _: None,
-    ) -> list[str]:
-        page_url = anime_page_link
-        episodes_data: list[dict[str, Any]] = []
-        if start_page_num == 1:
-            episodes_data.extend(first_page["data"])
-            start_page_num += 1
-            progress_update_callback(1)
-        for page_num in range(start_page_num, end_page_num + 1):
-            page_url = LOAD_EPISODES_URL.format(anime_page_link, page_num)
-            decoded = site_request(page_url).json()
-            # To avoid episodes like 7.5 and 5.5 cause they're usually just recaps
-            episodes = [ep for ep in decoded["data"] if isinstance(ep["episode"], int)]
-            episodes_data.extend(episodes)
-            page_url = decoded["next_page_url"]
-            self.resume.wait()
-            if self.cancelled:
-                return []
-            progress_update_callback(1)
-        first_episode = first_page["data"][0]["episode"]
-        return GetEpisodePageLinks.generate_episode_page_links(
-            start_episode, end_episode, first_episode, episodes_data, anime_id
-        )
-
-
-class GetPahewinPageLinks(ProgressFunction):
-    def __init__(self) -> None:
-        super().__init__()
-
-    def get_pahewin_page_links_and_info(
-        self,
-        episode_page_links: list[str],
-        progress_update_callback: Callable = lambda _: None,
-    ) -> tuple[list[list[str]], list[list[str]]]:
-        pahewin_links: list[list[str]] = []
-        download_info: list[list[str]] = []
-        for episode_page_link in episode_page_links:
-            page_content = site_request(episode_page_link).content
-            soup = BeautifulSoup(page_content, PARSER)
-            pahewin_data = soup.find_all("a", class_="dropdown-item", target="_blank")
-            if pahewin_data:
-                pahewin_links.append([cast(str, link["href"]) for link in pahewin_data])
-                download_info.append([li.text.strip() for li in pahewin_data])
-            self.resume.wait()
-            if self.cancelled:
-                return ([], [])
-            progress_update_callback(1)
-        return (pahewin_links, download_info)
-
-
-def is_dub(anime_info: str) -> bool:
-    return anime_info.endswith(DUB_PATTERN)
-
-
-def dub_available(anime_page_link: str, anime_id: str) -> bool:
-    page_url = LOAD_EPISODES_URL.format(anime_page_link, 1)
-    decoded = site_request(page_url).json()
-    episodes_data = decoded.get("data", None)
-    if episodes_data is None:
-        return False
-    episode_sessions = [episode["session"] for episode in episodes_data]
-    episode_links = [
-        EPISODE_PAGE_URL.format(anime_id, episode_session)
-        for episode_session in episode_sessions
-    ]
-    (
-        _,
-        download_info,
-    ) = GetPahewinPageLinks().get_pahewin_page_links_and_info(episode_links[:1])
-
-    for info in download_info[0]:
-        if is_dub(info):
-            return True
-    return False
-
-
-def bind_sub_or_dub_to_link_info(
-    sub_or_dub: str,
-    pahewin_download_page_links: list[list[str]],
-    download_info: list[list[str]],
-) -> tuple[list[list[str]], list[list[str]]]:
-    bound_links: list[list[str]] = []
-    bound_info: list[list[str]] = []
-    for link_list, episode_info in zip(pahewin_download_page_links, download_info):
-        links: list[str] = []
-        infos: list[str] = []
-        for link, info in zip(link_list, episode_info):
-            is_dub_link = is_dub(info)
-            if (sub_or_dub == "sub" and not is_dub_link) or (
-                sub_or_dub == "dub" and is_dub_link
-            ):
-                links.append(link)
-                infos.append(info)
-        if links and infos:
-            bound_links.append(links)
-            bound_info.append(infos)
-    return (bound_links, bound_info)
-
-
-def bind_quality_to_link_info(
-    quality: str,
-    pahewin_download_page_links: list[list[str]],
-    download_info: list[list[str]],
-) -> tuple[list[str], list[str]]:
-    bound_links: list[str] = []
-    bound_info: list[str] = []
-    for links, infos in zip(pahewin_download_page_links, download_info):
-        index = match_quality(infos, quality)
-        bound_links.append(links[index])
-        bound_info.append(infos[index])
-    return (bound_links, bound_info)
-
-
-def calculate_total_download_size(bound_info: list[str]) -> int:
-    total_size = 0
-    download_sizes: list[int] = []
-    for episode in bound_info:
-        match = cast(re.Match, EPISODE_SIZE_REGEX.search(episode))
-        size = int(match.group(1))
-        download_sizes.append(size)
-        total_size += size
-    return total_size
-
-
-def get_char_code(content: str, s1: int) -> int:
-    j = 0
-    for index, c in enumerate(reversed(content)):
-        j += (int(c) if c.isdigit() else 0) * int(math.pow(s1, index))
-    k = ""
-    while j > 0:
-        k = CHAR_MAP_DIGITS[j % CHAR_MAP_BASE] + k
-        j = (j - (j % CHAR_MAP_BASE)) // CHAR_MAP_BASE
-    return int(k) if k else 0
-
-
-# Courtesy of Saikou app https://github.com/saikou-app/saikou
-# RIP Saikou
-def decrypt_post_form(full_key: str, key: str, v1: int, v2: int) -> str:
-    r = ""
-    i = 0
-    while i < len(full_key):
-        s = ""
-        while full_key[i] != key[v2]:
-            s += full_key[i]
-            i += 1
-        for idx, c in enumerate(key):
-            s = s.replace(c, str(idx))
-        r += chr(get_char_code(s, v2) - v1)
-        i += 1
-    return r
-
-
-class GetDirectDownloadLinks(ProgressFunction):
-    def __init__(self) -> None:
-        super().__init__()
-
-    def get_direct_download_links(
-        self,
-        pahewin_download_page_links: list[str],
-        progress_update_callback: Callable = lambda _: None,
-    ) -> list[str]:
-        direct_download_links: list[str] = []
-        for pahewin_link in pahewin_download_page_links:
-            # Extract kwik page links
-            pahewin_html_page = CLIENT.get(pahewin_link).text
-            kwik_page_link = cast(
-                re.Match[str], KWIK_PAGE_REGEX.search(pahewin_html_page)
-            ).group()
-
-            # Extract direct download links from kwik html page
-            response = CLIENT.get(kwik_page_link)
-            match = cast(re.Match, PARAM_REGEX.search(response.text))
-            full_key, key, v1, v2 = (
-                match.group(1),
-                match.group(2),
-                match.group(3),
-                match.group(4),
-            )
-            form = decrypt_post_form(full_key, key, int(v1), int(v2))
-            soup = BeautifulSoup(form, PARSER)
-            post_url = cast(str, cast(Tag, soup.form)["action"])
-            token_value = cast(str, cast(Tag, soup.input)["value"])
-            response = CLIENT.post(
-                post_url,
-                headers=CLIENT.append_headers({"Referer": kwik_page_link}),
-                cookies=response.cookies,
-                data={"_token": token_value},
-                allow_redirects=False,
-            )
-            direct_download_link = response.headers["Location"]
-            direct_download_links.append(direct_download_link)
-            self.resume.wait()
-            if self.cancelled:
-                return []
-            progress_update_callback(1)
-        return direct_download_links
-
-
-def get_anime_metadata(anime_id: str) -> AnimeMetadata:
-    page_link = f"{PAHE_HOME_URL}/anime/{anime_id}"
-    page_content = site_request(page_link).content
-    soup = BeautifulSoup(page_content, PARSER)
-    poster = soup.find(class_="youtube-preview")
-    if not isinstance(poster, Tag):
-        poster = cast(Tag, soup.find(class_="poster-image"))
-    poster_link = cast(str, poster["href"])
-    summary = cast(Tag, soup.find(class_="anime-synopsis")).get_text()
-    genres_tags = cast(
-        Tag, cast(Tag, soup.find(class_="anime-genre font-weight-bold")).find("ul")
-    ).find_all("li")
-    genres: list[str] = []
-    for genre in genres_tags:
-        genres.append(cast(str, cast(Tag, genre.find("a"))["title"]))
-    season_and_year = cast(
-        str, cast(Tag, soup.select_one('a[href*="/anime/season/"]'))["title"]
-    )
-    _, release_year = season_and_year.split(" ")
-    page_link = ANIME_PAGE_URL.format(anime_id)
-    decoded = site_request(page_link).json()
-    episode_count = decoded["total"]
-    tag = soup.find(title="Currently Airing")
-    if tag:
-        status = "ONGOING"
-    elif episode_count == 0:
-        status = "UPCOMING"
-    else:
-        status = "FINISHED"
-    return AnimeMetadata(
-        poster_link, summary, episode_count, status, genres, int(release_year)
-    )
+import re
+import math
+from typing import Any, Callable, cast
+from requests import Response
+from bs4 import BeautifulSoup, Tag
+from senpwai.utils.scraper import (
+    CLIENT,
+    PARSER,
+    AnimeMetadata,
+    DomainNameError,
+    ProgressFunction,
+    get_new_home_url_from_readme,
+    match_quality,
+)
+from .constants import (
+    CHAR_MAP_BASE,
+    CHAR_MAP_DIGITS,
+    PAHE_HOME_URL,
+    FULL_SITE_NAME,
+    API_ENTRY_POINT,
+    ANIME_PAGE_URL,
+    LOAD_EPISODES_URL,
+    DUB_PATTERN,
+    EPISODE_PAGE_URL,
+    EPISODE_SIZE_REGEX,
+    KWIK_PAGE_REGEX,
+    PARAM_REGEX,
+)
+
+FIRST_REQUEST = True
+COOKIES = {"__ddg1_": "", "__ddg2_": ""}
+"""
+For some reason these cookies just need to be set as in they don't even need to be valid
+If something crashes, try updating to something like: 
+COOKIES = {
+    "__ddg1_": f"; Expires=Tue, 19 Jan 2038 03:14:07 GMT; Domain={PAHE_DOMAIN}; Path=/",
+    "__ddg2_": f"; Expires=Tue, 19 Jan 2038 03:14:07 GMT; Domain={PAHE_DOMAIN}; Path=/",
+}
+"""
+
+
+def site_request(url: str) -> Response:
+    """
+    For requests that go specifically to the domain animepahe.ru instead of e.g., pahe.win or kwik.si
+    Typically these requests need the cookies
+    """
+    try:
+        # We only want to handle the domain change incase this is the first request
+        # This is to avoid raising DomainNameError when the something else broke instead
+        global FIRST_REQUEST
+        if FIRST_REQUEST:
+            FIRST_REQUEST = False
+            response = CLIENT.get(
+                url,
+                cookies=COOKIES,
+                exceptions_to_raise=(DomainNameError, KeyboardInterrupt),
+            )
+        else:
+            response = CLIENT.get(url, cookies=COOKIES)
+        COOKIES.update(response.cookies)
+    except DomainNameError:
+        global PAHE_HOME_URL
+        PAHE_HOME_URL = get_new_home_url_from_readme(FULL_SITE_NAME)
+        return site_request(url)
+    return response
+
+
+def search(keyword: str) -> list[dict[str, str]]:
+    search_url = f"{API_ENTRY_POINT}search&q={keyword}"
+    response = site_request(search_url)
+    decoded = cast(dict, response.json())
+    # The search api endpoint won't return json containing the data key if no results are found
+    return decoded.get("data", [])
+
+
+def extract_anime_title_page_link_and_id(
+    result: dict[str, str],
+) -> tuple[str, str, str]:
+    anime_id = result["session"]
+    title = result["title"]
+    page_link = ANIME_PAGE_URL.format(anime_id)
+    return title, page_link, anime_id
+
+
+def get_episode_pages_info(
+    anime_page_link: str, start_episode: int, end_episode: int
+) -> tuple[int, int, int, dict[str, Any]]:
+    page_url = LOAD_EPISODES_URL.format(anime_page_link, 1)
+    decoded = site_request(page_url).json()
+    per_page: int = decoded["per_page"]
+    start_page = math.ceil(start_episode / per_page)
+    end_page = math.ceil(end_episode / per_page)
+    episode_page_count = (end_page - start_page) + 1
+    return start_page, end_page, episode_page_count, decoded
+
+
+class GetEpisodePageLinks(ProgressFunction):
+    def __init__(self) -> None:
+        super().__init__()
+
+    @staticmethod
+    def generate_episode_page_links(
+        start_episode: int,
+        end_episode: int,
+        first_episode: int,
+        episodes_data: list[dict[str, Any]],
+        anime_id: str,
+    ):
+        # These values should theoritically never remain as they are unless something crashes
+        # as in both of the ifs in the for loop should always eventually evaluate to True
+        start_idx = 0
+        end_idx = 0
+
+        for idx, episode in enumerate(episodes_data):
+            # Some times for sequels animepahe continues the episode numbers from the last episode of the previous season
+            # For instance  "Boku no Hero Academia 2nd Season" episode 1 is shown as episode 14
+            # So we do episode - (first_episode - 1) to get the real episode number e.g.,
+            # 14 - (14 - 1) = 1
+            # 15 - (14 - 1) = 2 and so on
+            episode_num = episode["episode"] - (first_episode - 1)
+            if episode_num == start_episode:
+                start_idx = idx
+            if episode_num == end_episode:
+                end_idx = idx
+                break
+        episodes_data = episodes_data[start_idx : end_idx + 1]
+        episode_sessions = [episode["session"] for episode in episodes_data]
+        return [
+            EPISODE_PAGE_URL.format(anime_id, episode_session)
+            for episode_session in episode_sessions
+        ]
+
+    # Retrieves a list of the episode page links (not download links)
+    def get_episode_page_links(
+        self,
+        start_episode: int,
+        end_episode: int,
+        start_page_num: int,
+        end_page_num: int,
+        first_page: dict[str, Any],
+        anime_page_link: str,
+        anime_id: str,
+        progress_update_callback: Callable = lambda _: None,
+    ) -> list[str]:
+        page_url = anime_page_link
+        episodes_data: list[dict[str, Any]] = []
+        if start_page_num == 1:
+            episodes_data.extend(first_page["data"])
+            start_page_num += 1
+            progress_update_callback(1)
+        for page_num in range(start_page_num, end_page_num + 1):
+            page_url = LOAD_EPISODES_URL.format(anime_page_link, page_num)
+            decoded = site_request(page_url).json()
+            # To avoid episodes like 7.5 and 5.5 cause they're usually just recaps
+            episodes = [ep for ep in decoded["data"] if isinstance(ep["episode"], int)]
+            episodes_data.extend(episodes)
+            page_url = decoded["next_page_url"]
+            self.resume.wait()
+            if self.cancelled:
+                return []
+            progress_update_callback(1)
+        first_episode = first_page["data"][0]["episode"]
+        return GetEpisodePageLinks.generate_episode_page_links(
+            start_episode, end_episode, first_episode, episodes_data, anime_id
+        )
+
+
+class GetPahewinPageLinks(ProgressFunction):
+    def __init__(self) -> None:
+        super().__init__()
+
+    def get_pahewin_page_links_and_info(
+        self,
+        episode_page_links: list[str],
+        progress_update_callback: Callable = lambda _: None,
+    ) -> tuple[list[list[str]], list[list[str]]]:
+        pahewin_links: list[list[str]] = []
+        download_info: list[list[str]] = []
+        for episode_page_link in episode_page_links:
+            page_content = site_request(episode_page_link).content
+            soup = BeautifulSoup(page_content, PARSER)
+            pahewin_data = soup.find_all("a", class_="dropdown-item", target="_blank")
+            if pahewin_data:
+                pahewin_links.append([cast(str, link["href"]) for link in pahewin_data])
+                download_info.append([li.text.strip() for li in pahewin_data])
+            self.resume.wait()
+            if self.cancelled:
+                return ([], [])
+            progress_update_callback(1)
+        return (pahewin_links, download_info)
+
+
+def is_dub(anime_info: str) -> bool:
+    return anime_info.endswith(DUB_PATTERN)
+
+
+def dub_available(anime_page_link: str, anime_id: str) -> bool:
+    page_url = LOAD_EPISODES_URL.format(anime_page_link, 1)
+    decoded = site_request(page_url).json()
+    episodes_data = decoded.get("data", None)
+    if episodes_data is None:
+        return False
+    episode_sessions = [episode["session"] for episode in episodes_data]
+    episode_links = [
+        EPISODE_PAGE_URL.format(anime_id, episode_session)
+        for episode_session in episode_sessions
+    ]
+    (
+        _,
+        download_info,
+    ) = GetPahewinPageLinks().get_pahewin_page_links_and_info(episode_links[:1])
+
+    for info in download_info[0]:
+        if is_dub(info):
+            return True
+    return False
+
+
+def bind_sub_or_dub_to_link_info(
+    sub_or_dub: str,
+    pahewin_download_page_links: list[list[str]],
+    download_info: list[list[str]],
+) -> tuple[list[list[str]], list[list[str]]]:
+    bound_links: list[list[str]] = []
+    bound_info: list[list[str]] = []
+    for link_list, episode_info in zip(pahewin_download_page_links, download_info):
+        links: list[str] = []
+        infos: list[str] = []
+        for link, info in zip(link_list, episode_info):
+            is_dub_link = is_dub(info)
+            if (sub_or_dub == "sub" and not is_dub_link) or (
+                sub_or_dub == "dub" and is_dub_link
+            ):
+                links.append(link)
+                infos.append(info)
+        if links and infos:
+            bound_links.append(links)
+            bound_info.append(infos)
+    return (bound_links, bound_info)
+
+
+def bind_quality_to_link_info(
+    quality: str,
+    pahewin_download_page_links: list[list[str]],
+    download_info: list[list[str]],
+) -> tuple[list[str], list[str]]:
+    bound_links: list[str] = []
+    bound_info: list[str] = []
+    for links, infos in zip(pahewin_download_page_links, download_info):
+        index = match_quality(infos, quality)
+        bound_links.append(links[index])
+        bound_info.append(infos[index])
+    return (bound_links, bound_info)
+
+
+def calculate_total_download_size(bound_info: list[str]) -> int:
+    total_size = 0
+    download_sizes: list[int] = []
+    for episode in bound_info:
+        match = cast(re.Match, EPISODE_SIZE_REGEX.search(episode))
+        size = int(match.group(1))
+        download_sizes.append(size)
+        total_size += size
+    return total_size
+
+
+def get_char_code(content: str, s1: int) -> int:
+    j = 0
+    for index, c in enumerate(reversed(content)):
+        j += (int(c) if c.isdigit() else 0) * int(math.pow(s1, index))
+    k = ""
+    while j > 0:
+        k = CHAR_MAP_DIGITS[j % CHAR_MAP_BASE] + k
+        j = (j - (j % CHAR_MAP_BASE)) // CHAR_MAP_BASE
+    return int(k) if k else 0
+
+
+# Courtesy of Saikou app https://github.com/saikou-app/saikou
+# RIP Saikou
+def decrypt_post_form(full_key: str, key: str, v1: int, v2: int) -> str:
+    r = ""
+    i = 0
+    while i < len(full_key):
+        s = ""
+        while full_key[i] != key[v2]:
+            s += full_key[i]
+            i += 1
+        for idx, c in enumerate(key):
+            s = s.replace(c, str(idx))
+        r += chr(get_char_code(s, v2) - v1)
+        i += 1
+    return r
+
+
+class GetDirectDownloadLinks(ProgressFunction):
+    def __init__(self) -> None:
+        super().__init__()
+
+    def get_direct_download_links(
+        self,
+        pahewin_download_page_links: list[str],
+        progress_update_callback: Callable = lambda _: None,
+    ) -> list[str]:
+        direct_download_links: list[str] = []
+        for pahewin_link in pahewin_download_page_links:
+            # Extract kwik page links
+            pahewin_html_page = CLIENT.get(pahewin_link).text
+            kwik_page_link = cast(
+                re.Match[str], KWIK_PAGE_REGEX.search(pahewin_html_page)
+            ).group()
+
+            # Extract direct download links from kwik html page
+            response = CLIENT.get(kwik_page_link)
+            match = cast(re.Match, PARAM_REGEX.search(response.text))
+            full_key, key, v1, v2 = (
+                match.group(1),
+                match.group(2),
+                match.group(3),
+                match.group(4),
+            )
+            form = decrypt_post_form(full_key, key, int(v1), int(v2))
+            soup = BeautifulSoup(form, PARSER)
+            post_url = cast(str, cast(Tag, soup.form)["action"])
+            token_value = cast(str, cast(Tag, soup.input)["value"])
+            response = CLIENT.post(
+                post_url,
+                headers=CLIENT.append_headers({"Referer": kwik_page_link}),
+                cookies=response.cookies,
+                data={"_token": token_value},
+                allow_redirects=False,
+            )
+            direct_download_link = response.headers["Location"]
+            direct_download_links.append(direct_download_link)
+            self.resume.wait()
+            if self.cancelled:
+                return []
+            progress_update_callback(1)
+        return direct_download_links
+
+
+def get_anime_metadata(anime_id: str) -> AnimeMetadata:
+    page_link = f"{PAHE_HOME_URL}/anime/{anime_id}"
+    page_content = site_request(page_link).content
+    soup = BeautifulSoup(page_content, PARSER)
+    poster = soup.find(class_="youtube-preview")
+    if not isinstance(poster, Tag):
+        poster = cast(Tag, soup.find(class_="poster-image"))
+    poster_link = cast(str, poster["href"])
+    summary = cast(Tag, soup.find(class_="anime-synopsis")).get_text()
+    genres_tags = cast(
+        Tag, cast(Tag, soup.find(class_="anime-genre font-weight-bold")).find("ul")
+    ).find_all("li")
+    genres: list[str] = []
+    for genre in genres_tags:
+        genres.append(cast(str, cast(Tag, genre.find("a"))["title"]))
+    season_and_year = cast(
+        str, cast(Tag, soup.select_one('a[href*="/anime/season/"]'))["title"]
+    )
+    _, release_year = season_and_year.split(" ")
+    page_link = ANIME_PAGE_URL.format(anime_id)
+    decoded = site_request(page_link).json()
+    episode_count = decoded["total"]
+    tag = soup.find(title="Currently Airing")
+    if tag:
+        status = "ONGOING"
+    elif episode_count == 0:
+        status = "UPCOMING"
+    else:
+        status = "FINISHED"
+    return AnimeMetadata(
+        poster_link, summary, episode_count, status, genres, int(release_year)
+    )
```

### Comparing `senpwai-2.1.8/senpwai/scrapers/test.py` & `senpwai-2.1.9/senpwai/scrapers/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,745 +1,745 @@
-import os
-import sys
-from time import time as current_time
-from typing import Any, Callable, cast
-
-from senpwai.utils.scraper import AnimeMetadata, Download, sanitise_title
-from senpwai.utils.static import ROOT_DIRECTORY
-
-from senpwai.scrapers import gogo, pahe
-
-PAHE = pahe.PAHE
-GOGO = gogo.GOGO
-
-DEFAULT_ANIME_TITLE = "Senyuu"
-DEFAULT_QUALITY = "360p"
-DEFAULT_START_EPISODE = "1"
-DEFAULT_END_EPISODE = "2"
-DEFAULT_SUB_OR_DUB = "sub"
-DEFAULT_SITE = "pahe"
-DEFAULT_DOWNLOAD_FOLDER_PATH = os.path.join(ROOT_DIRECTORY, "..", ".test-downloads")
-DEFAULT_VERBOSE = False
-DEFAULT_SILENT = False
-SILENT = DEFAULT_SILENT
-COMMANDS = [
-    "search",
-    "dub_available",
-    "metadata",
-    "episode_page",
-    "download_page",
-    "download_size",
-    "direct_links",
-    "hls_links",
-    "match_links",
-    "segments_urls",
-    "download",
-    "all",
-]
-
-
-class FailedTest(Exception):
-    def __init__(self, msg: str):
-        super().__init__(msg)
-
-
-def conditional_print(text: str):
-    if not SILENT:
-        print(text)
-
-
-def test_start(name: str):
-    conditional_print(f"Running: {name} Test")
-
-
-def fail_test(
-    name: str,
-    expected: Any,
-    got: Any,
-    execution_time: float,
-    test_variables: str | None = None,
-):
-    msg = f"{name} Test\nExpected: {expected}\nGot: {got}\nExecution time: {round(execution_time, 2)}s"
-    if test_variables:
-        msg = f"{msg}\nTest Variables:\n{test_variables}"
-    raise FailedTest(msg)
-
-
-def pass_test(name: str, execution_time: float):
-    conditional_print(f"Passed: {name} Test\nTook: {round(execution_time, 2)}s\n")
-
-
-def test_search(anime_title: str, site: str) -> list[list[str]]:
-    test_name = "Search"
-    test_start(test_name)
-    run_time_getter = get_run_time_later()
-    if site == PAHE:
-        results = pahe.search(anime_title)
-    else:
-        results = gogo.search(anime_title)
-    rt = run_time_getter()
-    if not results:
-        fail_if_list_is_empty(results, test_name, "results", rt)
-    pass_test(test_name, rt)
-    test_name = "Parse search results"
-    test_start(test_name)
-    c = current_time()
-    parsed_results: list[list[str]] = []
-    if site == PAHE:
-        parsed_results = [
-            list(pahe.extract_anime_title_page_link_and_id(r))
-            for r in cast(list[dict[str, str]], results)
-        ]
-    else:
-        for title, page_link in cast(list[tuple[str, str]], results):
-            parsed_results.append([title, page_link])
-    run_timer = current_time() - c
-    if not parsed_results:
-        fail_test(test_name, "List of parsed results", "Empty list", run_timer)
-    pass_test(test_name, run_timer)
-    return parsed_results
-
-
-def get_run_time_later() -> Callable[[], float]:
-    c = current_time()
-    return lambda: current_time() - c
-
-
-def test_check_results_for_anime(
-    anime_title: str,
-    results: list[list[str]] | list[list[str]],
-) -> list[str] | None:
-    test_name = f"Matching results to {anime_title}"
-    test_start(test_name)
-    run_time = get_run_time_later()
-    query = sanitise_title(anime_title, True).lower()
-    for r in results:
-        title = r[0]
-        if query == sanitise_title(title, True).lower():
-            pass_test(test_name, run_time())
-            return r
-    fail_test(
-        test_name,
-        "A perfect match",
-        "No match found",
-        run_time(),
-        f"Anime title was: {anime_title}\nSearch results were: {results}",
-    )
-
-
-def test_get_metadata(
-    site: str, target_result: list[str]
-) -> tuple[AnimeMetadata, bytes]:
-    test_name = "Get Metadata"
-    test_start(test_name)
-    run_time = get_run_time_later()
-    page_content = b""
-    if site == PAHE:
-        target_result = cast(list[str], target_result)
-        metadata = pahe.get_anime_metadata(target_result[2])
-    else:
-        page_content, target_result[1] = gogo.get_anime_page_content(target_result[1])
-        metadata = gogo.extract_anime_metadata(page_content)
-    pass_test(test_name, run_time())
-    return metadata, page_content
-
-
-def test_get_episode_page_links(
-    anime_id: str, anime_page_link: str, start_episode: int, end_episode: int
-) -> list[str]:
-    test_name = "Get Episode page links"
-    test_start(test_name)
-    run_time = get_run_time_later()
-    test_variables = f"Anime ID: {anime_id}"
-    anime_id = cast(str, anime_id)
-    start_page_num, end_page_num, _, first_page = pahe.get_episode_pages_info(
-        anime_page_link, start_episode, end_episode
-    )
-    episode_page_links = pahe.GetEpisodePageLinks().get_episode_page_links(
-        start_episode,
-        end_episode,
-        start_page_num,
-        end_page_num,
-        first_page,
-        anime_page_link,
-        anime_id,
-    )
-    rt = run_time()
-    fail_if_list_is_empty(
-        episode_page_links, test_name, "Episode page links", rt, test_variables
-    )
-    pass_test(test_name, run_time())
-    return episode_page_links
-
-
-def test_get_download_page_links(
-    site: str,
-    quality: str,
-    sub_or_dub: str,
-    eps_page_links: list[str],
-    start_episode: int,
-    end_episode: int,
-    anime_id: int,
-) -> tuple[list[str], list[str]]:
-    test_name = "Get Download page links"
-    test_start(test_name)
-    run_time_getter = get_run_time_later()
-    if site == PAHE:
-        (
-            pahewin_page,
-            pahewin_info,
-        ) = pahe.GetPahewinPageLinks().get_pahewin_page_links_and_info(eps_page_links)
-        download_page_links, download_info = pahe.bind_sub_or_dub_to_link_info(
-            sub_or_dub, pahewin_page, pahewin_info
-        )
-        fail_if_list_is_empty(
-            download_page_links[0],
-            test_name,
-            f"Bound to {sub_or_dub} download page links",
-            run_time_getter(),
-            f"Episode page links were: {eps_page_links}\nPahewin page links were: {pahewin_page}",
-        )
-        download_page_links, download_info = pahe.bind_quality_to_link_info(
-            quality, download_page_links, download_info
-        )
-        rt = run_time_getter()
-        fail_if_list_is_empty(
-            download_page_links,
-            test_name,
-            "Download page links",
-            rt,
-            f"Episode page links were: {eps_page_links}",
-        )
-    else:
-        download_page_links = gogo.get_download_page_links(
-            start_episode, end_episode, anime_id
-        )
-        download_info = []
-        rt = run_time_getter()
-        fail_if_list_is_empty(
-            download_page_links,
-            test_name,
-            "Download page links",
-            rt,
-            f"Anime ID was: {anime_id}\nStart Episode was: {start_episode}\nEnd Episode was: {end_episode}",
-        )
-    pass_test(test_name, run_time_getter())
-    return download_page_links, download_info
-
-
-def fail_if_list_is_empty(
-    array: list[Any],
-    test_name: str,
-    list_of: str,
-    execution_time: float,
-    test_variables: str | None = None,
-):
-    if not array:
-        fail_test(
-            test_name,
-            f"List of {list_of}",
-            "Empty list",
-            execution_time,
-            test_variables,
-        )
-
-
-def test_getting_direct_download_links(
-    site: str, download_page_links: list[str], quality: str
-) -> list[str]:
-    test_name = "Get Direct download links"
-    test_start(test_name)
-    run_time_getter = get_run_time_later()
-    ddls: list[str] = []
-    if site == PAHE:
-        ddls = pahe.GetDirectDownloadLinks().get_direct_download_links(
-            download_page_links
-        )
-    else:
-        ddls = gogo.GetDirectDownloadLinks().get_direct_download_links(
-            download_page_links, quality
-        )
-    rt = run_time_getter()
-    fail_if_list_is_empty(
-        ddls,
-        test_name,
-        "direct download links",
-        rt,
-        f"Download page links were: {download_page_links}",
-    )
-    pass_test(test_name, rt)
-    return ddls
-
-
-def test_getting_hls_links(episode_page_links: list[str]) -> list[str]:
-    test_name = "Get HLS links"
-    test_start(test_name)
-    runtime_getter = get_run_time_later()
-    hls_links = gogo.GetHlsLinks().get_hls_links(episode_page_links)
-    rt = runtime_getter()
-    fail_if_list_is_empty(
-        hls_links,
-        test_name,
-        "HLS links",
-        rt,
-        f"Episode page links were: {episode_page_links}",
-    )
-    pass_test(test_name, rt)
-    return hls_links
-
-
-def test_matching_quality_to_hls_links(hls_links: list[str], quality: str) -> list[str]:
-    test_name = "Match Quality to HLS links"
-    test_start(test_name)
-    runtime_getter = get_run_time_later()
-    hls_links = gogo.GetHlsMatchedQualityLinks().get_hls_matched_quality_links(
-        hls_links, quality
-    )
-    rt = runtime_getter()
-    fail_if_list_is_empty(
-        hls_links,
-        test_name,
-        "Matched HLS links",
-        rt,
-        f"Original HLS links were: {hls_links}",
-    )
-    pass_test(test_name, rt)
-    return hls_links
-
-
-def test_getting_segments_urls(matched_hls_links: list[str]) -> list[list[str]]:
-    test_name = "Get Segments URLs"
-    test_start(test_name)
-    runtime_getter = get_run_time_later()
-    segs_urls = gogo.GetHlsSegmentsUrls().get_hls_segments_urls(matched_hls_links)
-    rt = runtime_getter()
-    fail_if_list_is_empty(
-        segs_urls,
-        test_name,
-        "List containing List of Segment URLs",
-        rt,
-        f"Matched HLS links were: {matched_hls_links}",
-    )
-    fail_if_list_is_empty(
-        segs_urls[0],
-        test_name,
-        "Segment URLs",
-        rt,
-        f"Matched HLS links were: {matched_hls_links}",
-    )
-    pass_test(test_name, runtime_getter())
-    return segs_urls
-
-
-def test_downloading(
-    anime_title: str,
-    ddls_or_segs_urls: list[str] | list[list[str]],
-    is_hls_download: bool,
-    start_eps: int,
-    end_eps: int,
-    download_folder: str,
-):
-    test_name = "Downloading"
-    test_start(test_name)
-    if not os.path.isdir(download_folder):
-        os.makedirs(download_folder)
-    runtime_getter = get_run_time_later()
-    conditional_print(f"Folder: {download_folder}")
-    for eps_no, ddl_or_seg_urls in zip(
-        range(start_eps, end_eps + 1), ddls_or_segs_urls
-    ):
-        runtime_getter = get_run_time_later()
-        eps_number = str(eps_no).zfill(2)
-        eps_title = f"{anime_title} E{eps_number}"
-        inner_test_name = f"Downloading {eps_title}"
-        test_start(test_name)
-        Download(
-            ddl_or_seg_urls, eps_title, download_folder, is_hls_download=is_hls_download
-        ).start_download()
-        full_name = f"{eps_title}.mp4"
-        rt = runtime_getter()
-        downloaded_file = os.path.join(download_folder, full_name)
-        if os.path.isfile(downloaded_file):
-            pass_test(inner_test_name, rt)
-            os.unlink(downloaded_file)
-            continue
-        test_variables = (
-            f"HLS links were: {ddls_or_segs_urls}"
-            if is_hls_download
-            else f"DDLs were: {ddls_or_segs_urls}"
-        )
-        fail_test(
-            inner_test_name,
-            f"{full_name} file in {download_folder}",
-            "Didn't find the file",
-            rt,
-            test_variables,
-        )
-
-    rt = runtime_getter()
-    pass_test(test_name, rt)
-    os.removedirs(download_folder)
-
-
-class ArgParser:
-    arg_site = ("--site", "-s")
-    arg_verbose = ("--verbose", "-v")
-    arg_title = ("--title", "-t")
-    arg_quality = ("--quality", "-q")
-    arg_sub_or_dub = ("--sub_or_dub", "-sd")
-    arg_path = ("--path", "-p")
-    arg_help = ("--help", "-h")
-    arg_silent = ("--silent", "-s")
-
-    def __init__(self, args: list[str]):
-        self.passed_args = args[1:]
-        global SILENT
-        SILENT = self.arg_in_group_was_passed(self.arg_silent)
-        if not self.arg_in_group_was_passed(COMMANDS):
-            print("No valid Command specified")
-            self.print_usage()
-        if self.arg_in_group_was_passed(self.arg_help):
-            self.print_usage()
-
-        self.site = self.arg_value_finder(args, self.arg_site, DEFAULT_SITE)
-        self.validate_arg_value(self.arg_site, (PAHE, GOGO), self.site)
-
-        self.anime_title = self.arg_value_finder(
-            args, self.arg_title, DEFAULT_ANIME_TITLE
-        )
-        self.anime_title = sanitise_title(self.anime_title)
-
-        self.verbose = self.arg_in_group_was_passed(self.arg_verbose)
-        self.start_eps, self.end_eps = self.parse_start_and_end_episode(args)
-
-        self.quality = self.arg_value_finder(args, self.arg_quality, DEFAULT_QUALITY)
-        self.validate_arg_value(
-            self.arg_quality, ("360p", "480p", "720p", "1080p"), self.quality
-        )
-
-        self.sub_or_dub = self.arg_value_finder(
-            args, self.arg_sub_or_dub, DEFAULT_SUB_OR_DUB
-        )
-        self.validate_arg_value(self.arg_sub_or_dub, ("sub", "dub"), self.sub_or_dub)
-
-        self.path = self.arg_value_finder(
-            args, self.arg_path, DEFAULT_DOWNLOAD_FOLDER_PATH
-        )
-
-    def print_usage(self):
-        usage = """
-        Usage: scrapers.test [COMMAND/TEST] [OPTIONS]
-
-        Commands/Tests:
-        search                  Test searching
-        dub_available           Test dub availablity checking
-        metadata                Test getting metadata
-        episode_page            Test getting episode page links (pahe only)
-        download_page           Test getting download page links
-        download_size           Test extraction (pahe)/ getting (gogo) of total download size
-        direct_links            Test getting direct download links
-        hls_links               Test getting hls links
-        match_links             Test matching hls links to user quality
-        segments_urls           Test getting segments urls
-        download                Test downloading (Implicitly performs all tests)
-        all                     Perform all tests (alias to download). Only performs all tests for one site, defaults to pahe
-        
-
-        Options:
-        --site, -s              Specify the site (i.e., pahe, gogo). Default: pahe
-        --title, -t             Specify the anime title. Default: Senyuu
-        --quality, -q           Specify the video quality (i.e., 360p, 480p, 720p, 1080p). Default: 360p
-        --sub_or_dub, -sd       Specify sub or dub. Default: sub
-        --path, -p              Specify the download folder path. Default: ./src/test-downloads
-        --start_episode, -se    Specify the starting episode number. Default: 1
-        --end_episode, -ee      Specify the ending episode number. Default: 2
-        --verbose, -v           Enable verbose mode for more detailed explanations of test results
-        --silent, s             Only output critical information
-        --help, -h              Display this help message
-
-
-        Example:
-        scrapers.test --site pahe --title "Naruto" --quality 720p --sub_or_dub sub
-
-        Note: Tests are hierarchial, if for example episode_page is the command/test to run, both search and metadata test will be performed cause they are required, in order to get episode_page links
-        Note: Tests are site specific, the all command does not perform tests for each site it implicitly defaults to pahe
-        """
-        print(usage)
-        sys.exit(0)
-
-    def arg_in_group_was_passed(self, arg_group: tuple | list[str]):
-        return any(arg in self.passed_args for arg in arg_group)
-
-    def parse_start_and_end_episode(self, args: list[str]) -> tuple[int, int]:
-        s = ("--start_episode", "-se")
-        start_str = self.arg_value_finder(args, s, DEFAULT_START_EPISODE)
-        e = ("--end_episode", "-ee")
-        end_str = self.arg_value_finder(args, e, DEFAULT_END_EPISODE)
-
-        def check_if_digit(x, v):
-            return (
-                self.invalid_usage(f"{x} MUST be a number") if not v.isdigit() else None
-            )
-
-        def check_if_greater_than_zero(x, v):
-            self.invalid_usage(f"{x} MUST be greater than zero") if v <= 0 else None
-
-        check_if_digit(s, start_str)
-        check_if_digit(e, end_str)
-        start_eps = int(start_str)
-        end_eps = int(end_str)
-        check_if_greater_than_zero(s, start_eps)
-        check_if_greater_than_zero(e, end_eps)
-        if start_eps > end_eps:
-            self.invalid_usage(f"{s} CAN'T be greater than {e}")
-        return start_eps, end_eps
-
-    def invalid_usage(self, usage: str):
-        print(f"Invalid Usage:\n{usage}")
-        sys.exit(0)
-
-    def validate_arg_value(self, arg: tuple[str, str], can_bes: tuple, passed: str):
-        if passed not in can_bes:
-            can_be = " or ".join(can_bes)
-            usage = f"{arg} MUST be either {can_be}. Got '{passed}' instead"
-            self.invalid_usage(usage)
-
-    def arg_value_finder(
-        self, args: list[str], target_args: tuple[str, str], default: str | None = None
-    ) -> str:  # type: ignore
-        for arg in target_args:
-            try:
-                idx = args.index(arg)
-                return args[idx + 1]
-            except ValueError:
-                pass
-        if default:
-            conditional_print(f"Using default {target_args}: {default}")
-            return default
-        self.invalid_usage(f"Expected: {target_args}")
-
-
-def test_dub_available(site: str, target_result: list[str]) -> tuple[bool, str]:
-    test_name = "Dub availability checking"
-    test_start(test_name)
-    runtime_getter = get_run_time_later()
-    dub_link = ""
-    if site == PAHE:
-        dub_available = pahe.dub_available(target_result[1], target_result[2])
-    else:
-        dub_available, dub_link = gogo.dub_availability_and_link(target_result[0])
-    rt = runtime_getter()
-    if not isinstance(dub_available, bool):
-        fail_test(
-            test_name,
-            "Boolean value",
-            type(dub_available),
-            rt,
-            f"The returned value was: {dub_available}",
-        )
-    pass_test(test_name, rt)
-    return dub_available, dub_link
-
-
-def run_tests(args: ArgParser):
-    was_hls = False
-    if args.arg_in_group_was_passed(COMMANDS):
-        results = test_search(args.anime_title, args.site)
-        if args.verbose:
-            conditional_print(f"Search Results: {results}\n")
-        target_result = cast(
-            list[str],
-            test_check_results_for_anime(args.anime_title, results),
-        )
-        if args.verbose:
-            conditional_print(f"Target Result: {target_result}\n")
-        COMMANDS.remove("search")
-        if args.arg_in_group_was_passed(COMMANDS):
-            dub_available, dub_link = test_dub_available(args.site, target_result)
-
-            if args.verbose:
-                conditional_print("Dub available") if dub_available else print(
-                    "No Dub available"
-                )
-            COMMANDS.remove("dub_available")
-            if args.arg_in_group_was_passed(COMMANDS):
-                metadata, page_content = test_get_metadata(args.site, target_result)
-                if args.verbose:
-                    if args.site == GOGO:
-                        conditional_print("Sub metadata")
-
-                    def print_metadata(metadata: AnimeMetadata):
-                        conditional_print(
-                            f"Metadata:\nPoster Url: {metadata.poster_url}\nSummary: {metadata.summary[:100]}.. .\nEpisode Count: {metadata.episode_count}\nAiring Status: {metadata.airing_status}\nGenres: {metadata.genres}\nRelease Year: {metadata.release_year}\n"
-                        )
-
-                    print_metadata(metadata)
-                COMMANDS.remove("metadata")
-                if args.arg_in_group_was_passed(COMMANDS) or (
-                    args.site == GOGO and args.sub_or_dub == "dub"
-                ):
-                    if args.end_eps > metadata.episode_count:
-                        return print(
-                            f"The chosen target anime has {metadata.episode_count} episodes yet you specified the ('--end_episode', '-ee') as {args.end_eps}"
-                        )
-                    if args.sub_or_dub == "dub" and not dub_available:
-                        return print(
-                            "Couldn't find Dub for the anime on the specified site"
-                        )
-                    elif args.site == GOGO and dub_available:
-                        metadata, page_content = test_get_metadata(
-                            args.site, ["", dub_link]
-                        )
-                        if args.verbose:
-                            conditional_print("Dub metadata")
-                            print_metadata(metadata)  # type: ignore
-                    if args.site == PAHE:
-                        episode_page_links = test_get_episode_page_links(
-                            target_result[2],
-                            target_result[1],
-                            args.start_eps,
-                            args.end_eps,
-                        )
-                        if args.verbose:
-                            conditional_print(
-                                f"Episode page links: {episode_page_links}\n"
-                            )
-                    else:
-                        episode_page_links = []
-                    COMMANDS.remove("episode_page")
-                    if args.arg_in_group_was_passed(COMMANDS):
-                        anime_id = (
-                            gogo.extract_anime_id(page_content)
-                            if args.site == GOGO
-                            else 0
-                        )
-                        (
-                            download_page_links,
-                            download_info,
-                        ) = test_get_download_page_links(
-                            args.site,
-                            args.quality,
-                            args.sub_or_dub,
-                            episode_page_links,
-                            args.start_eps,
-                            args.end_eps,
-                            anime_id,
-                        )
-                        if args.verbose:
-                            conditional_print(
-                                f"Download page links: {download_page_links}\n"
-                            )
-                        COMMANDS.remove("download_page")
-                        if args.site == PAHE and args.arg_in_group_was_passed(
-                            ["download_size"]
-                        ):
-                            test_name = "Total Download size"
-                            test_start(test_name)
-                            runtime_getter = get_run_time_later()
-                            total_download_size = pahe.calculate_total_download_size(
-                                download_info
-                            )
-                            rt = runtime_getter()
-                            if not isinstance(total_download_size, int):
-                                fail_test(
-                                    test_name,
-                                    "An integer",
-                                    type(total_download_size),
-                                    rt,
-                                    f"Bound download infos were: {download_info}",
-                                )
-                            pass_test(test_name, rt)
-                            if args.verbose:
-                                conditional_print(
-                                    f"Total download size is: {total_download_size}"
-                                )
-                            COMMANDS.remove("download_size")
-                        # HLS testing pipeine
-                        if args.site == GOGO and args.arg_in_group_was_passed(
-                            ["hls_links", "match_links", "segments_urls", "all"]
-                        ):
-                            hls_links = test_getting_hls_links(download_page_links)
-                            if args.verbose:
-                                conditional_print(f"HLS links: {hls_links}\n")
-                            COMMANDS.remove("hls_links")
-                            was_hls = True
-                            if args.arg_in_group_was_passed(
-                                ["segments_urls", "match_links", "all"]
-                            ):
-                                matched_links = test_matching_quality_to_hls_links(
-                                    hls_links, args.quality
-                                )
-                                if args.verbose:
-                                    conditional_print(
-                                        f"Matched Quality links: {matched_links}\n"
-                                    )
-                                COMMANDS.remove("match_links")
-                                if args.arg_in_group_was_passed(
-                                    ["segments_urls", "all"]
-                                ):
-                                    segs_urls = test_getting_segments_urls(
-                                        matched_links
-                                    )
-                                    if args.verbose:
-                                        conditional_print(
-                                            f"Segments URLs: {segs_urls}\n"
-                                        )
-                                    COMMANDS.remove("segments_urls")
-                                    if args.arg_in_group_was_passed(COMMANDS):
-                                        test_downloading(
-                                            args.anime_title,
-                                            segs_urls,
-                                            True,
-                                            args.start_eps,
-                                            args.end_eps,
-                                            args.path,
-                                        )
-                        if args.arg_in_group_was_passed(COMMANDS):
-                            direct_download_links = test_getting_direct_download_links(
-                                args.site, download_page_links, args.quality
-                            )
-                            if args.verbose:
-                                conditional_print(f"DDLs: {direct_download_links}\n")
-                            COMMANDS.remove("direct_links")
-                            if args.site == GOGO and args.arg_in_group_was_passed(
-                                ["download_size"]
-                            ):
-                                test_name = "Download size"
-                                test_start(test_name)
-                                runtime_getter = get_run_time_later()
-                                total_download_size = gogo.CalculateTotalDowloadSize().calculate_total_download_size(
-                                    direct_download_links, in_megabytes=True
-                                )
-                                rt = runtime_getter()
-                                if not isinstance(total_download_size, int):
-                                    fail_test(
-                                        test_name,
-                                        "An integer",
-                                        type(total_download_size),
-                                        rt,
-                                        f"DDLs were: {direct_download_links}",
-                                    )
-                                pass_test(test_name, rt)
-                                if args.verbose:
-                                    conditional_print(
-                                        f"Total download size is: {total_download_size}"
-                                    )
-                                COMMANDS.remove("download_size")
-                            if args.arg_in_group_was_passed(COMMANDS):
-                                test_downloading(
-                                    args.anime_title,
-                                    direct_download_links,
-                                    False,
-                                    args.start_eps,
-                                    args.end_eps,
-                                    args.path,
-                                )
-    if args.site == PAHE:
-        return print(f"Specified {PAHE} tests passed")
-    if was_hls:
-        return print(f"Specified {GOGO} HLS tests passed")
-    return print(f"Specified {GOGO} NORM tests passed")
-
-
-if __name__ == "__main__":
-    args = ArgParser(sys.argv)
-    run_tests(args)
+import os
+import sys
+from time import time as current_time
+from typing import Any, Callable, cast
+
+from senpwai.utils.scraper import AnimeMetadata, Download, sanitise_title
+from senpwai.utils.static import ROOT_DIRECTORY
+
+from senpwai.scrapers import gogo, pahe
+
+PAHE = pahe.PAHE
+GOGO = gogo.GOGO
+
+DEFAULT_ANIME_TITLE = "Boku no Hero Academia"
+DEFAULT_QUALITY = "360p"
+DEFAULT_START_EPISODE = "1"
+DEFAULT_END_EPISODE = "2"
+DEFAULT_SUB_OR_DUB = "sub"
+DEFAULT_SITE = "pahe"
+DEFAULT_DOWNLOAD_FOLDER_PATH = os.path.join(ROOT_DIRECTORY, "..", ".test-downloads")
+DEFAULT_VERBOSE = False
+DEFAULT_SILENT = False
+SILENT = DEFAULT_SILENT
+COMMANDS = [
+    "search",
+    "dub_available",
+    "metadata",
+    "episode_page",
+    "download_page",
+    "download_size",
+    "direct_links",
+    "hls_links",
+    "match_links",
+    "segments_urls",
+    "download",
+    "all",
+]
+
+
+class FailedTest(Exception):
+    def __init__(self, msg: str):
+        super().__init__(msg)
+
+
+def conditional_print(text: str):
+    if not SILENT:
+        print(text)
+
+
+def test_start(name: str):
+    conditional_print(f"Running: {name} Test")
+
+
+def fail_test(
+    name: str,
+    expected: Any,
+    got: Any,
+    execution_time: float,
+    test_variables: str | None = None,
+):
+    msg = f"{name} Test\nExpected: {expected}\nGot: {got}\nExecution time: {round(execution_time, 2)}s"
+    if test_variables:
+        msg = f"{msg}\nTest Variables:\n{test_variables}"
+    raise FailedTest(msg)
+
+
+def pass_test(name: str, execution_time: float):
+    conditional_print(f"Passed: {name} Test\nTook: {round(execution_time, 2)}s\n")
+
+
+def test_search(anime_title: str, site: str) -> list[list[str]]:
+    test_name = "Search"
+    test_start(test_name)
+    run_time_getter = get_run_time_later()
+    if site == PAHE:
+        results = pahe.search(anime_title)
+    else:
+        results = gogo.search(anime_title)
+    rt = run_time_getter()
+    if not results:
+        fail_if_list_is_empty(results, test_name, "results", rt)
+    pass_test(test_name, rt)
+    test_name = "Parse search results"
+    test_start(test_name)
+    c = current_time()
+    parsed_results: list[list[str]] = []
+    if site == PAHE:
+        parsed_results = [
+            list(pahe.extract_anime_title_page_link_and_id(r))
+            for r in cast(list[dict[str, str]], results)
+        ]
+    else:
+        for title, page_link in cast(list[tuple[str, str]], results):
+            parsed_results.append([title, page_link])
+    run_timer = current_time() - c
+    if not parsed_results:
+        fail_test(test_name, "List of parsed results", "Empty list", run_timer)
+    pass_test(test_name, run_timer)
+    return parsed_results
+
+
+def get_run_time_later() -> Callable[[], float]:
+    c = current_time()
+    return lambda: current_time() - c
+
+
+def test_check_results_for_anime(
+    anime_title: str,
+    results: list[list[str]] | list[list[str]],
+) -> list[str] | None:
+    test_name = f"Matching results to {anime_title}"
+    test_start(test_name)
+    run_time = get_run_time_later()
+    query = sanitise_title(anime_title, True).lower()
+    for r in results:
+        title = r[0]
+        if query == sanitise_title(title, True).lower():
+            pass_test(test_name, run_time())
+            return r
+    fail_test(
+        test_name,
+        "A perfect match",
+        "No match found",
+        run_time(),
+        f"Anime title was: {anime_title}\nSearch results were: {results}",
+    )
+
+
+def test_get_metadata(
+    site: str, target_result: list[str]
+) -> tuple[AnimeMetadata, bytes]:
+    test_name = "Get Metadata"
+    test_start(test_name)
+    run_time = get_run_time_later()
+    page_content = b""
+    if site == PAHE:
+        target_result = cast(list[str], target_result)
+        metadata = pahe.get_anime_metadata(target_result[2])
+    else:
+        page_content, target_result[1] = gogo.get_anime_page_content(target_result[1])
+        metadata = gogo.extract_anime_metadata(page_content)
+    pass_test(test_name, run_time())
+    return metadata, page_content
+
+
+def test_get_episode_page_links(
+    anime_id: str, anime_page_link: str, start_episode: int, end_episode: int
+) -> list[str]:
+    test_name = "Get Episode page links"
+    test_start(test_name)
+    run_time = get_run_time_later()
+    test_variables = f"Anime ID: {anime_id}"
+    anime_id = cast(str, anime_id)
+    start_page_num, end_page_num, _, first_page = pahe.get_episode_pages_info(
+        anime_page_link, start_episode, end_episode
+    )
+    episode_page_links = pahe.GetEpisodePageLinks().get_episode_page_links(
+        start_episode,
+        end_episode,
+        start_page_num,
+        end_page_num,
+        first_page,
+        anime_page_link,
+        anime_id,
+    )
+    rt = run_time()
+    fail_if_list_is_empty(
+        episode_page_links, test_name, "Episode page links", rt, test_variables
+    )
+    pass_test(test_name, run_time())
+    return episode_page_links
+
+
+def test_get_download_page_links(
+    site: str,
+    quality: str,
+    sub_or_dub: str,
+    eps_page_links: list[str],
+    start_episode: int,
+    end_episode: int,
+    anime_id: int,
+) -> tuple[list[str], list[str]]:
+    test_name = "Get Download page links"
+    test_start(test_name)
+    run_time_getter = get_run_time_later()
+    if site == PAHE:
+        (
+            pahewin_page,
+            pahewin_info,
+        ) = pahe.GetPahewinPageLinks().get_pahewin_page_links_and_info(eps_page_links)
+        download_page_links, download_info = pahe.bind_sub_or_dub_to_link_info(
+            sub_or_dub, pahewin_page, pahewin_info
+        )
+        fail_if_list_is_empty(
+            download_page_links[0],
+            test_name,
+            f"Bound to {sub_or_dub} download page links",
+            run_time_getter(),
+            f"Episode page links were: {eps_page_links}\nPahewin page links were: {pahewin_page}",
+        )
+        download_page_links, download_info = pahe.bind_quality_to_link_info(
+            quality, download_page_links, download_info
+        )
+        rt = run_time_getter()
+        fail_if_list_is_empty(
+            download_page_links,
+            test_name,
+            "Download page links",
+            rt,
+            f"Episode page links were: {eps_page_links}",
+        )
+    else:
+        download_page_links = gogo.get_download_page_links(
+            start_episode, end_episode, anime_id
+        )
+        download_info = []
+        rt = run_time_getter()
+        fail_if_list_is_empty(
+            download_page_links,
+            test_name,
+            "Download page links",
+            rt,
+            f"Anime ID was: {anime_id}\nStart Episode was: {start_episode}\nEnd Episode was: {end_episode}",
+        )
+    pass_test(test_name, run_time_getter())
+    return download_page_links, download_info
+
+
+def fail_if_list_is_empty(
+    array: list[Any],
+    test_name: str,
+    list_of: str,
+    execution_time: float,
+    test_variables: str | None = None,
+):
+    if not array:
+        fail_test(
+            test_name,
+            f"List of {list_of}",
+            "Empty list",
+            execution_time,
+            test_variables,
+        )
+
+
+def test_getting_direct_download_links(
+    site: str, download_page_links: list[str], quality: str
+) -> list[str]:
+    test_name = "Get Direct download links"
+    test_start(test_name)
+    run_time_getter = get_run_time_later()
+    ddls: list[str] = []
+    if site == PAHE:
+        ddls = pahe.GetDirectDownloadLinks().get_direct_download_links(
+            download_page_links
+        )
+    else:
+        ddls = gogo.GetDirectDownloadLinks().get_direct_download_links(
+            download_page_links, quality
+        )
+    rt = run_time_getter()
+    fail_if_list_is_empty(
+        ddls,
+        test_name,
+        "direct download links",
+        rt,
+        f"Download page links were: {download_page_links}",
+    )
+    pass_test(test_name, rt)
+    return ddls
+
+
+def test_getting_hls_links(episode_page_links: list[str]) -> list[str]:
+    test_name = "Get HLS links"
+    test_start(test_name)
+    runtime_getter = get_run_time_later()
+    hls_links = gogo.GetHlsLinks().get_hls_links(episode_page_links)
+    rt = runtime_getter()
+    fail_if_list_is_empty(
+        hls_links,
+        test_name,
+        "HLS links",
+        rt,
+        f"Episode page links were: {episode_page_links}",
+    )
+    pass_test(test_name, rt)
+    return hls_links
+
+
+def test_matching_quality_to_hls_links(hls_links: list[str], quality: str) -> list[str]:
+    test_name = "Match Quality to HLS links"
+    test_start(test_name)
+    runtime_getter = get_run_time_later()
+    hls_links = gogo.GetHlsMatchedQualityLinks().get_hls_matched_quality_links(
+        hls_links, quality
+    )
+    rt = runtime_getter()
+    fail_if_list_is_empty(
+        hls_links,
+        test_name,
+        "Matched HLS links",
+        rt,
+        f"Original HLS links were: {hls_links}",
+    )
+    pass_test(test_name, rt)
+    return hls_links
+
+
+def test_getting_segments_urls(matched_hls_links: list[str]) -> list[list[str]]:
+    test_name = "Get Segments URLs"
+    test_start(test_name)
+    runtime_getter = get_run_time_later()
+    segs_urls = gogo.GetHlsSegmentsUrls().get_hls_segments_urls(matched_hls_links)
+    rt = runtime_getter()
+    fail_if_list_is_empty(
+        segs_urls,
+        test_name,
+        "List containing List of Segment URLs",
+        rt,
+        f"Matched HLS links were: {matched_hls_links}",
+    )
+    fail_if_list_is_empty(
+        segs_urls[0],
+        test_name,
+        "Segment URLs",
+        rt,
+        f"Matched HLS links were: {matched_hls_links}",
+    )
+    pass_test(test_name, runtime_getter())
+    return segs_urls
+
+
+def test_downloading(
+    anime_title: str,
+    ddls_or_segs_urls: list[str] | list[list[str]],
+    is_hls_download: bool,
+    start_eps: int,
+    end_eps: int,
+    download_folder: str,
+):
+    test_name = "Downloading"
+    test_start(test_name)
+    if not os.path.isdir(download_folder):
+        os.makedirs(download_folder)
+    runtime_getter = get_run_time_later()
+    conditional_print(f"Folder: {download_folder}")
+    for eps_no, ddl_or_seg_urls in zip(
+        range(start_eps, end_eps + 1), ddls_or_segs_urls
+    ):
+        runtime_getter = get_run_time_later()
+        eps_number = str(eps_no).zfill(2)
+        eps_title = f"{anime_title} E{eps_number}"
+        inner_test_name = f"Downloading {eps_title}"
+        test_start(test_name)
+        Download(
+            ddl_or_seg_urls, eps_title, download_folder, is_hls_download=is_hls_download
+        ).start_download()
+        full_name = f"{eps_title}.mp4"
+        rt = runtime_getter()
+        downloaded_file = os.path.join(download_folder, full_name)
+        if os.path.isfile(downloaded_file):
+            pass_test(inner_test_name, rt)
+            os.unlink(downloaded_file)
+            continue
+        test_variables = (
+            f"HLS links were: {ddls_or_segs_urls}"
+            if is_hls_download
+            else f"DDLs were: {ddls_or_segs_urls}"
+        )
+        fail_test(
+            inner_test_name,
+            f"{full_name} file in {download_folder}",
+            "Didn't find the file",
+            rt,
+            test_variables,
+        )
+
+    rt = runtime_getter()
+    pass_test(test_name, rt)
+    os.removedirs(download_folder)
+
+
+class ArgParser:
+    arg_site = ("--site", "-s")
+    arg_verbose = ("--verbose", "-v")
+    arg_title = ("--title", "-t")
+    arg_quality = ("--quality", "-q")
+    arg_sub_or_dub = ("--sub_or_dub", "-sd")
+    arg_path = ("--path", "-p")
+    arg_help = ("--help", "-h")
+    arg_silent = ("--silent", "-s")
+
+    def __init__(self, args: list[str]):
+        self.passed_args = args[1:]
+        global SILENT
+        SILENT = self.arg_in_group_was_passed(self.arg_silent)
+        if not self.arg_in_group_was_passed(COMMANDS):
+            print("No valid Command specified")
+            self.print_usage()
+        if self.arg_in_group_was_passed(self.arg_help):
+            self.print_usage()
+
+        self.site = self.arg_value_finder(args, self.arg_site, DEFAULT_SITE)
+        self.validate_arg_value(self.arg_site, (PAHE, GOGO), self.site)
+
+        self.anime_title = self.arg_value_finder(
+            args, self.arg_title, DEFAULT_ANIME_TITLE
+        )
+        self.anime_title = sanitise_title(self.anime_title)
+
+        self.verbose = self.arg_in_group_was_passed(self.arg_verbose)
+        self.start_eps, self.end_eps = self.parse_start_and_end_episode(args)
+
+        self.quality = self.arg_value_finder(args, self.arg_quality, DEFAULT_QUALITY)
+        self.validate_arg_value(
+            self.arg_quality, ("360p", "480p", "720p", "1080p"), self.quality
+        )
+
+        self.sub_or_dub = self.arg_value_finder(
+            args, self.arg_sub_or_dub, DEFAULT_SUB_OR_DUB
+        )
+        self.validate_arg_value(self.arg_sub_or_dub, ("sub", "dub"), self.sub_or_dub)
+
+        self.path = self.arg_value_finder(
+            args, self.arg_path, DEFAULT_DOWNLOAD_FOLDER_PATH
+        )
+
+    def print_usage(self):
+        usage = """
+        Usage: scrapers.test [COMMAND/TEST] [OPTIONS]
+
+        Commands/Tests:
+        search                  Test searching
+        dub_available           Test dub availablity checking
+        metadata                Test getting metadata
+        episode_page            Test getting episode page links (pahe only)
+        download_page           Test getting download page links
+        download_size           Test extraction (pahe)/ getting (gogo) of total download size
+        direct_links            Test getting direct download links
+        hls_links               Test getting hls links
+        match_links             Test matching hls links to user quality
+        segments_urls           Test getting segments urls
+        download                Test downloading (Implicitly performs all tests)
+        all                     Perform all tests (alias to download). Only performs all tests for one site, defaults to pahe
+        
+
+        Options:
+        --site, -s              Specify the site (i.e., pahe, gogo). Default: pahe
+        --title, -t             Specify the anime title. Default: "Boku no Hero Academia"
+        --quality, -q           Specify the video quality (i.e., 360p, 480p, 720p, 1080p). Default: 360p
+        --sub_or_dub, -sd       Specify sub or dub. Default: sub
+        --path, -p              Specify the download folder path. Default: ./src/test-downloads
+        --start_episode, -se    Specify the starting episode number. Default: 1
+        --end_episode, -ee      Specify the ending episode number. Default: 2
+        --verbose, -v           Enable verbose mode for more detailed explanations of test results
+        --silent, s             Only output critical information
+        --help, -h              Display this help message
+
+
+        Example:
+        scrapers.test --site pahe --title "Naruto" --quality 720p --sub_or_dub sub
+
+        Note: Tests are hierarchial, if for example episode_page is the command/test to run, both search and metadata test will be performed cause they are required, in order to get episode_page links
+        Note: Tests are site specific, the all command does not perform tests for each site it implicitly defaults to pahe
+        """
+        print(usage)
+        sys.exit(0)
+
+    def arg_in_group_was_passed(self, arg_group: tuple | list[str]):
+        return any(arg in self.passed_args for arg in arg_group)
+
+    def parse_start_and_end_episode(self, args: list[str]) -> tuple[int, int]:
+        s = ("--start_episode", "-se")
+        start_str = self.arg_value_finder(args, s, DEFAULT_START_EPISODE)
+        e = ("--end_episode", "-ee")
+        end_str = self.arg_value_finder(args, e, DEFAULT_END_EPISODE)
+
+        def check_if_digit(x, v):
+            return (
+                self.invalid_usage(f"{x} MUST be a number") if not v.isdigit() else None
+            )
+
+        def check_if_greater_than_zero(x, v):
+            self.invalid_usage(f"{x} MUST be greater than zero") if v <= 0 else None
+
+        check_if_digit(s, start_str)
+        check_if_digit(e, end_str)
+        start_eps = int(start_str)
+        end_eps = int(end_str)
+        check_if_greater_than_zero(s, start_eps)
+        check_if_greater_than_zero(e, end_eps)
+        if start_eps > end_eps:
+            self.invalid_usage(f"{s} CAN'T be greater than {e}")
+        return start_eps, end_eps
+
+    def invalid_usage(self, usage: str):
+        print(f"Invalid Usage:\n{usage}")
+        sys.exit(0)
+
+    def validate_arg_value(self, arg: tuple[str, str], can_bes: tuple, passed: str):
+        if passed not in can_bes:
+            can_be = " or ".join(can_bes)
+            usage = f"{arg} MUST be either {can_be}. Got '{passed}' instead"
+            self.invalid_usage(usage)
+
+    def arg_value_finder(
+        self, args: list[str], target_args: tuple[str, str], default: str | None = None
+    ) -> str:  # type: ignore
+        for arg in target_args:
+            try:
+                idx = args.index(arg)
+                return args[idx + 1]
+            except ValueError:
+                pass
+        if default:
+            conditional_print(f"Using default {target_args}: {default}")
+            return default
+        self.invalid_usage(f"Expected: {target_args}")
+
+
+def test_dub_available(site: str, target_result: list[str]) -> tuple[bool, str]:
+    test_name = "Dub availability checking"
+    test_start(test_name)
+    runtime_getter = get_run_time_later()
+    dub_link = ""
+    if site == PAHE:
+        dub_available = pahe.dub_available(target_result[1], target_result[2])
+    else:
+        dub_available, dub_link = gogo.dub_availability_and_link(target_result[0])
+    rt = runtime_getter()
+    if not isinstance(dub_available, bool):
+        fail_test(
+            test_name,
+            "Boolean value",
+            type(dub_available),
+            rt,
+            f"The returned value was: {dub_available}",
+        )
+    pass_test(test_name, rt)
+    return dub_available, dub_link
+
+
+def run_tests(args: ArgParser):
+    was_hls = False
+    if args.arg_in_group_was_passed(COMMANDS):
+        results = test_search(args.anime_title, args.site)
+        if args.verbose:
+            conditional_print(f"Search Results: {results}\n")
+        target_result = cast(
+            list[str],
+            test_check_results_for_anime(args.anime_title, results),
+        )
+        if args.verbose:
+            conditional_print(f"Target Result: {target_result}\n")
+        COMMANDS.remove("search")
+        if args.arg_in_group_was_passed(COMMANDS):
+            dub_available, dub_link = test_dub_available(args.site, target_result)
+
+            if args.verbose:
+                conditional_print("Dub available") if dub_available else print(
+                    "No Dub available"
+                )
+            COMMANDS.remove("dub_available")
+            if args.arg_in_group_was_passed(COMMANDS):
+                metadata, page_content = test_get_metadata(args.site, target_result)
+                if args.verbose:
+                    if args.site == GOGO:
+                        conditional_print("Sub metadata")
+
+                    def print_metadata(metadata: AnimeMetadata):
+                        conditional_print(
+                            f"Metadata:\nPoster Url: {metadata.poster_url}\nSummary: {metadata.summary[:100]}.. .\nEpisode Count: {metadata.episode_count}\nAiring Status: {metadata.airing_status}\nGenres: {metadata.genres}\nRelease Year: {metadata.release_year}\n"
+                        )
+
+                    print_metadata(metadata)
+                COMMANDS.remove("metadata")
+                if args.arg_in_group_was_passed(COMMANDS) or (
+                    args.site == GOGO and args.sub_or_dub == "dub"
+                ):
+                    if args.end_eps > metadata.episode_count:
+                        return print(
+                            f"The chosen target anime has {metadata.episode_count} episodes yet you specified the ('--end_episode', '-ee') as {args.end_eps}"
+                        )
+                    if args.sub_or_dub == "dub" and not dub_available:
+                        return print(
+                            "Couldn't find Dub for the anime on the specified site"
+                        )
+                    elif args.site == GOGO and dub_available:
+                        metadata, page_content = test_get_metadata(
+                            args.site, ["", dub_link]
+                        )
+                        if args.verbose:
+                            conditional_print("Dub metadata")
+                            print_metadata(metadata)  # type: ignore
+                    if args.site == PAHE:
+                        episode_page_links = test_get_episode_page_links(
+                            target_result[2],
+                            target_result[1],
+                            args.start_eps,
+                            args.end_eps,
+                        )
+                        if args.verbose:
+                            conditional_print(
+                                f"Episode page links: {episode_page_links}\n"
+                            )
+                    else:
+                        episode_page_links = []
+                    COMMANDS.remove("episode_page")
+                    if args.arg_in_group_was_passed(COMMANDS):
+                        anime_id = (
+                            gogo.extract_anime_id(page_content)
+                            if args.site == GOGO
+                            else 0
+                        )
+                        (
+                            download_page_links,
+                            download_info,
+                        ) = test_get_download_page_links(
+                            args.site,
+                            args.quality,
+                            args.sub_or_dub,
+                            episode_page_links,
+                            args.start_eps,
+                            args.end_eps,
+                            anime_id,
+                        )
+                        if args.verbose:
+                            conditional_print(
+                                f"Download page links: {download_page_links}\n"
+                            )
+                        COMMANDS.remove("download_page")
+                        if args.site == PAHE and args.arg_in_group_was_passed(
+                            ["download_size"]
+                        ):
+                            test_name = "Total Download size"
+                            test_start(test_name)
+                            runtime_getter = get_run_time_later()
+                            total_download_size = pahe.calculate_total_download_size(
+                                download_info
+                            )
+                            rt = runtime_getter()
+                            if not isinstance(total_download_size, int):
+                                fail_test(
+                                    test_name,
+                                    "An integer",
+                                    type(total_download_size),
+                                    rt,
+                                    f"Bound download infos were: {download_info}",
+                                )
+                            pass_test(test_name, rt)
+                            if args.verbose:
+                                conditional_print(
+                                    f"Total download size is: {total_download_size}"
+                                )
+                            COMMANDS.remove("download_size")
+                        # HLS testing pipeine
+                        if args.site == GOGO and args.arg_in_group_was_passed(
+                            ["hls_links", "match_links", "segments_urls", "all"]
+                        ):
+                            hls_links = test_getting_hls_links(download_page_links)
+                            if args.verbose:
+                                conditional_print(f"HLS links: {hls_links}\n")
+                            COMMANDS.remove("hls_links")
+                            was_hls = True
+                            if args.arg_in_group_was_passed(
+                                ["segments_urls", "match_links", "all"]
+                            ):
+                                matched_links = test_matching_quality_to_hls_links(
+                                    hls_links, args.quality
+                                )
+                                if args.verbose:
+                                    conditional_print(
+                                        f"Matched Quality links: {matched_links}\n"
+                                    )
+                                COMMANDS.remove("match_links")
+                                if args.arg_in_group_was_passed(
+                                    ["segments_urls", "all"]
+                                ):
+                                    segs_urls = test_getting_segments_urls(
+                                        matched_links
+                                    )
+                                    if args.verbose:
+                                        conditional_print(
+                                            f"Segments URLs: {segs_urls}\n"
+                                        )
+                                    COMMANDS.remove("segments_urls")
+                                    if args.arg_in_group_was_passed(COMMANDS):
+                                        test_downloading(
+                                            args.anime_title,
+                                            segs_urls,
+                                            True,
+                                            args.start_eps,
+                                            args.end_eps,
+                                            args.path,
+                                        )
+                        if args.arg_in_group_was_passed(COMMANDS):
+                            direct_download_links = test_getting_direct_download_links(
+                                args.site, download_page_links, args.quality
+                            )
+                            if args.verbose:
+                                conditional_print(f"DDLs: {direct_download_links}\n")
+                            COMMANDS.remove("direct_links")
+                            if args.site == GOGO and args.arg_in_group_was_passed(
+                                ["download_size"]
+                            ):
+                                test_name = "Download size"
+                                test_start(test_name)
+                                runtime_getter = get_run_time_later()
+                                total_download_size = gogo.CalculateTotalDowloadSize().calculate_total_download_size(
+                                    direct_download_links, in_megabytes=True
+                                )
+                                rt = runtime_getter()
+                                if not isinstance(total_download_size, int):
+                                    fail_test(
+                                        test_name,
+                                        "An integer",
+                                        type(total_download_size),
+                                        rt,
+                                        f"DDLs were: {direct_download_links}",
+                                    )
+                                pass_test(test_name, rt)
+                                if args.verbose:
+                                    conditional_print(
+                                        f"Total download size is: {total_download_size}"
+                                    )
+                                COMMANDS.remove("download_size")
+                            if args.arg_in_group_was_passed(COMMANDS):
+                                test_downloading(
+                                    args.anime_title,
+                                    direct_download_links,
+                                    False,
+                                    args.start_eps,
+                                    args.end_eps,
+                                    args.path,
+                                )
+    if args.site == PAHE:
+        return print(f"Specified {PAHE} tests passed")
+    if was_hls:
+        return print(f"Specified {GOGO} HLS tests passed")
+    return print(f"Specified {GOGO} NORM tests passed")
+
+
+if __name__ == "__main__":
+    args = ArgParser(sys.argv)
+    run_tests(args)
```

### Comparing `senpwai-2.1.8/senpwai/senpcli/main.py` & `senpwai-2.1.9/senpwai/senpcli/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/utils/classes.py` & `senpwai-2.1.9/senpwai/utils/classes.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/utils/scraper.py` & `senpwai-2.1.9/senpwai/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/utils/static.py` & `senpwai-2.1.9/senpwai/utils/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from random import choice as random_choice
 from subprocess import Popen
 from types import TracebackType
 import logging
 
 APP_NAME = "Senpwai"
 APP_NAME_LOWER = "senpwai"
-VERSION = "2.1.8"
+VERSION = "2.1.9"
 DESCRIPTION = "A desktop app for tracking and batch downloading anime"
 
 IS_PIP_INSTALL = False
 APP_EXE_PATH = ""
 
 
 class OS:
```

### Comparing `senpwai-2.1.8/senpwai/utils/widgets.py` & `senpwai-2.1.9/senpwai/utils/widgets.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/windows/about.py` & `senpwai-2.1.9/senpwai/windows/about.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/windows/abstracts.py` & `senpwai-2.1.9/senpwai/windows/abstracts.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/windows/chosen_anime.py` & `senpwai-2.1.9/senpwai/windows/chosen_anime.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/windows/download.py` & `senpwai-2.1.9/senpwai/windows/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,16 +385,14 @@
     def initiate_download_pipeline(self, anime_details: AnimeDetails):
         if self.first_download_since_app_start:
             self.pause_icon = Icon(30, 30, PAUSE_ICON_PATH)
             self.resume_icon = Icon(30, 30, RESUME_ICON_PATH)
             self.cancel_icon = Icon(30, 30, CANCEL_ICON_PATH)
             self.download_queue = DownloadQueue(self)
 
-        if anime_details.sub_or_dub == DUB:
-            anime_details.anime.page_link = anime_details.dub_page_link
         if anime_details.site == PAHE:
             return PaheGetEpisodePageInfo(
                 self,
                 anime_details.lacked_episode_numbers[0],
                 anime_details.lacked_episode_numbers[-1],
                 anime_details,
                 self.pahe_get_episode_page_links,
@@ -996,14 +994,19 @@
     ):
         super().__init__(download_window)
         self.anime_details = anime_details
         self.hls_finished.connect(callback)
         self.finished.connect(callback)
 
     def run(self):
+        if self.anime_details.sub_or_dub == DUB:
+            (
+                self.anime_details.anime_page_content,
+                self.anime_details.anime.page_link,
+            ) = gogo.get_anime_page_content(self.anime_details.dub_page_link)
         anime_id = gogo.extract_anime_id(self.anime_details.anime_page_content)
         download_page_links = gogo.get_download_page_links(
             self.anime_details.lacked_episode_numbers[0],
             self.anime_details.lacked_episode_numbers[-1],
             anime_id,
         )
         download_page_links = lacked_episodes(
```

### Comparing `senpwai-2.1.8/senpwai/windows/main.py` & `senpwai-2.1.9/senpwai/windows/main.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/windows/misc.py` & `senpwai-2.1.9/senpwai/windows/misc.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/windows/search.py` & `senpwai-2.1.9/senpwai/windows/search.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/senpwai/windows/settings.py` & `senpwai-2.1.9/senpwai/windows/settings.py`

 * *Files identical despite different names*

### Comparing `senpwai-2.1.8/PKG-INFO` & `senpwai-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senpwai
-Version: 2.1.8
+Version: 2.1.9
 Summary: A desktop app for tracking and batch downloading anime
 Home-page: https://github.com/SenZmaKi/Senpwai
 License: GPL v3
 Keywords: anime,app,cli,desktop app,anime downloader,anime cli,anime app,anime tracker,batch anime downloader,bulk anime  downloader,anime desktop app,anime tracker app
 Author: SenZmaKi
 Author-email: senzmaki@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -73,15 +73,15 @@
 
 - **Other**
 
 [Build from source](#building-from-source).
 
 ## Features
 
-- Download any anime from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to).
+- Download any anime from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.so).
 - Keep track of an anime and automatically download new episodes when they release.
 - Download a complete season or episodes within a range (e.g., 69-420).
 - Choose between video qualities: 360p, 480p (Gogoanime only), 720p, or 1080p.
 - Download in sub or dub (if available) depending on the user's preference.
 - Automatically detects episodes you already have and avoids re-downloading them.
 - Robust and graceful download error management.
 - GUI and [CLI](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: senpwai Version: 2.1.8 Summary: A desktop app for
+Metadata-Version: 2.1 Name: senpwai Version: 2.1.9 Summary: A desktop app for
 tracking and batch downloading anime Home-page: https://github.com/SenZmaKi/
 Senpwai License: GPL v3 Keywords: anime,app,cli,desktop app,anime
 downloader,anime cli,anime app,anime tracker,batch anime downloader,bulk anime
 downloader,anime desktop app,anime tracker app Author: SenZmaKi Author-email:
 senzmaki@gmail.com Requires-Python: >=3.11,<4.0 Classifier: License :: Other/
 Proprietary License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
@@ -26,15 +26,15 @@
 [one-piece-screenshot]## Installation - **Cross-platform (Linux, Mac, Windows
 10/11)** Needs [Python 3.11](https://www.python.org/downloads/release/python-
 3111) installed. ```bash pip install senpwai ``` - **Windows 10/11** Download
 [the setup](https://github.com/SenZmaKi/Senpwai/releases/latest/download/
 Senpwai-setup.exe) then run it. - **Android** Check [Senpcli](https://
 github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md) - **Other**
 [Build from source](#building-from-source). ## Features - Download any anime
-from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.to). -
+from [Animepahe](https://animepahe.ru) or [Gogoanime](https://anitaku.so). -
 Keep track of an anime and automatically download new episodes when they
 release. - Download a complete season or episodes within a range (e.g., 69-
 420). - Choose between video qualities: 360p, 480p (Gogoanime only), 720p, or
 1080p. - Download in sub or dub (if available) depending on the user's
 preference. - Automatically detects episodes you already have and avoids re-
 downloading them. - Robust and graceful download error management. - GUI and
 [CLI](https://github.com/SenZmaKi/Senpwai/blob/master/docs/senpcli-guide.md).
```

