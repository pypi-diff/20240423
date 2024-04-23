# Comparing `tmp/gamdl-2.1.8.tar.gz` & `tmp/gamdl-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-2.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-2.1.8.tar` & `gamdl-2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       17 2024-04-17 00:24:01.918930 gamdl-2.1.8/.github/FUNDING.yml
--rw-r--r--   0        0        0     1137 2024-04-17 00:24:01.918930 gamdl-2.1.8/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2024-04-17 00:24:01.918930 gamdl-2.1.8/.gitignore
--rw-r--r--   0        0        0    12010 2024-04-17 00:24:01.918930 gamdl-2.1.8/README.md
--rw-r--r--   0        0        0       22 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/__main__.py
--rw-r--r--   0        0        0     7930 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/apple_music_api.py
--rw-r--r--   0        0        0    26698 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/cli.py
--rw-r--r--   0        0        0     5580 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/constants.py
--rw-r--r--   0        0        0    12691 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader.py
--rw-r--r--   0        0        0    10587 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_music_video.py
--rw-r--r--   0        0        0     2290 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_post.py
--rw-r--r--   0        0        0    14184 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_song.py
--rw-r--r--   0        0        0     3922 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/downloader_song_legacy.py
--rw-r--r--   0        0        0      817 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/enums.py
--rw-r--r--   0        0        0     4015 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/hardcoded_wvd.py
--rw-r--r--   0        0        0     2418 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/itunes_api.py
--rw-r--r--   0        0        0      369 2024-04-17 00:24:01.918930 gamdl-2.1.8/gamdl/models.py
--rw-r--r--   0        0        0      587 2024-04-17 00:24:01.918930 gamdl-2.1.8/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-17 00:24:01.918930 gamdl-2.1.8/requirements.txt
--rw-r--r--   0        0        0    12512 1970-01-01 00:00:00.000000 gamdl-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-04-23 03:51:01.997233 gamdl-2.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1137 2024-04-23 03:51:01.997233 gamdl-2.2/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-23 03:51:01.997233 gamdl-2.2/.gitignore
+-rw-r--r--   0        0        0    12217 2024-04-23 03:51:02.001234 gamdl-2.2/README.md
+-rw-r--r--   0        0        0       20 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/__main__.py
+-rw-r--r--   0        0        0     8853 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26863 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/cli.py
+-rw-r--r--   0        0        0     5570 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/constants.py
+-rw-r--r--   0        0        0    16173 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader.py
+-rw-r--r--   0        0        0    10482 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2202 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    14146 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3922 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      797 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      369 2024-04-23 03:51:02.001234 gamdl-2.2/gamdl/models.py
+-rw-r--r--   0        0        0      593 2024-04-23 03:51:02.001234 gamdl-2.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-23 03:51:02.001234 gamdl-2.2/requirements.txt
+-rw-r--r--   0        0        0    12723 1970-01-01 00:00:00.000000 gamdl-2.2/PKG-INFO
```

### Comparing `gamdl-2.1.8/.github/workflows/main.yml` & `gamdl-2.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.8/README.md` & `gamdl-2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ## Features
 * Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
+* Use artist links to download all of their albums or music videos
 
 ## Prerequisites
 * Python 3.8 or higher
 * The cookies file of your Apple Music account (requires an active subscription)
     * You can get your cookies by using one of the following extensions on your browser of choice at the Apple Music website with your account signed in:
         * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
         * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
@@ -43,23 +44,27 @@
     ```bash
     gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1624945511?i=1624945512"
     ```
 * Download an album
     ```bash
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1624945511"
     ```
+* Choose which albums or music videos to download from an artist
+    ```bash
+    gamdl "https://music.apple.com/us/artist/rick-astley/669771"
+    ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
 | Command line argument / Config file key                         | Description                                                                  | Default value                                |
 | --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
 | `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
 | `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
 | `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
-| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.                       | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                                      |
 | `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
 | `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                                      |
 | `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
 | `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
 | `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
 | `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
 | `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
@@ -81,15 +86,15 @@
 | `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                                    |
 | `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
 | `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
 | `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                                       |
 | `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
 | `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                                 |
 | `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                                        |
-| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264-best`                                  |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264`                                       |
 | `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                                       |
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
@@ -157,16 +162,16 @@
 * `ask`
     * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
-* `h264-best` (up to 1080p, with AAC 256kbps)
-* `h265-best` (up to 2160p, with AAC 256kpbs)
+* `h264` (up to 1080p, with AAC 256kbps)
+* `h265` (up to 2160p, with AAC 256kpbs)
 * `ask`
     * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
   
 ### Post videos/extra videos qualities
 The following qualities are available:
 * `best` (up to 1080p, with AAC 256kbps)
 * `ask`
```

### Comparing `gamdl-2.1.8/gamdl/apple_music_api.py` & `gamdl-2.2/gamdl/apple_music_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import functools
 import re
 import time
+import typing
 from http.cookiejar import MozillaCookieJar
 from pathlib import Path
 
 import requests
 
 
 class AppleMusicApi:
@@ -81,14 +82,39 @@
         except (
             requests.HTTPError,
             requests.exceptions.JSONDecodeError,
             AssertionError,
         ):
             self._raise_response_exception(response)
 
+    def get_artist(
+        self,
+        artist_id: str,
+        include: str = "albums,music-videos",
+        limit: int = 100,
+        fetch_all: bool = True,
+    ) -> dict:
+        response = self.session.get(
+            f"{self.AMP_API_URL}/v1/catalog/{self.storefront}/artists/{artist_id}",
+            params={
+                "include": include,
+                **{f"limit[{_include}]": limit for _include in include.split(",")},
+            },
+        )
+        self._check_amp_api_response(response)
+        artist = response.json()["data"][0]
+        if fetch_all:
+            for _include in include.split(","):
+                for additional_data in self._extend_api_data(
+                    artist["relationships"][_include],
+                    limit,
+                ):
+                    artist["relationships"][_include]["data"].extend(additional_data)
+        return artist
+
     def get_song(
         self,
         song_id: str,
         extend: str = "extendedAssetUrls",
         include: str = "lyrics,albums",
     ) -> dict:
         response = self.session.get(
@@ -142,47 +168,50 @@
 
     def get_playlist(
         self,
         playlist_id: str,
         is_library: bool = False,
         limit_tracks: int = 300,
         extend: str = "extendedAssetUrls",
-        full_playlist: bool = True,
+        fetch_all: bool = True,
     ) -> dict:
         response = self.session.get(
             f"{self.AMP_API_URL}/v1/{'me' if is_library else 'catalog'}/{self.storefront}/playlists/{playlist_id}",
             params={
                 "extend": extend,
                 "limit[tracks]": limit_tracks,
             },
         )
         self._check_amp_api_response(response)
         playlist = response.json()["data"][0]
-        if full_playlist:
-            playlist = self._extend_playlists_tracks(playlist, limit_tracks)
+        if fetch_all:
+            for additional_data in self._extend_api_data(
+                playlist["relationships"]["tracks"],
+                limit_tracks,
+            ):
+                playlist["relationships"]["tracks"]["data"].extend(additional_data)
         return playlist
 
-    def _extend_playlists_tracks(
+    def _extend_api_data(
         self,
-        playlist: dict,
-        limit_tracks: int,
-    ) -> dict:
-        playlist_next_uri = playlist["relationships"]["tracks"].get("next")
-        while playlist_next_uri:
-            playlist_next = self._get_playlist_next(playlist_next_uri, limit_tracks)
-            playlist["relationships"]["tracks"]["data"].extend(playlist_next["data"])
-            playlist_next_uri = playlist_next.get("next")
+        api_response: dict,
+        limit: int,
+    ) -> typing.Generator[list[dict], None, None]:
+        next_uri = api_response.get("next")
+        while next_uri:
+            playlist_next = self._get_next_uri_response(next_uri, limit)
+            yield playlist_next["data"]
+            next_uri = playlist_next.get("next")
             time.sleep(self.WAIT_TIME)
-        return playlist
 
-    def _get_playlist_next(self, playlist_next_uri: str, limit_tracks: int) -> dict:
+    def _get_next_uri_response(self, next_uri: str, limit: int) -> dict:
         response = self.session.get(
-            self.AMP_API_URL + playlist_next_uri,
+            self.AMP_API_URL + next_uri,
             params={
-                "limit[tracks]": limit_tracks,
+                "limit": limit,
             },
         )
         self._check_amp_api_response(response)
         return response.json()
 
     def get_webplayback(
         self,
```

### Comparing `gamdl-2.1.8/gamdl/cli.py` & `gamdl-2.2/gamdl/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     is_flag=True,
     help="Overwrite existing files.",
 )
 @click.option(
     "--read-urls-as-txt",
     "-r",
     is_flag=True,
-    help="Interpret URLs as paths to text files containing URLs.",
+    help="Interpret URLs as paths to text files containing URLs separated by newlines",
 )
 @click.option(
     "--synced-lyrics-only",
     is_flag=True,
     help="Download only the synced lyrics.",
 )
 @click.option(
@@ -436,18 +436,23 @@
         if codec_song not in LEGACY_CODECS:
             logger.warn(
                 "You have chosen a non-legacy codec. Support for non-legacy codecs are not guaranteed, "
                 "as most of the songs cannot be downloaded when using non-legacy codecs."
             )
     error_count = 0
     if read_urls_as_txt:
-        urls = [url.strip() for url in Path(urls[0]).read_text().splitlines()]
+        _urls = []
+        for url in urls:
+            if Path(url).exists():
+                _urls.extend(Path(url).read_text().splitlines())
+        urls = _urls
     for url_index, url in enumerate(urls, start=1):
         url_progress = f"URL {url_index}/{len(urls)}"
         try:
+            logger.info(f'({url_progress}) Checking "{url}"')
             url_info = downloader.get_url_info(url)
             download_queue = downloader.get_download_queue(url_info)
         except Exception as e:
             error_count += 1
             logger.error(
                 f'({url_progress}) Failed to check "{url}"',
                 exc_info=print_exceptions,
@@ -492,16 +497,16 @@
                     if synced_lyrics_only:
                         pass
                     elif final_path.exists() and not overwrite:
                         logger.warning(
                             f'({queue_progress}) Song already exists at "{final_path}", skipping'
                         )
                     else:
+                        logger.debug("Getting stream info")
                         if codec_song in LEGACY_CODECS:
-                            logger.debug("Getting stream info")
                             stream_info = downloader_song_legacy.get_stream_info(
                                 webplayback
                             )
                             logger.debug("Getting decryption key")
                             decryption_key = downloader_song_legacy.get_decryption_key(
                                 stream_info.pssh, track["id"]
                             )
```

### Comparing `gamdl-2.1.8/gamdl/constants.py` & `gamdl-2.2/gamdl/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,16 +193,16 @@
     SongCodec.AAC_HE_DOWNMIX: r"audio-HE-stereo-\d+-downmix",
     SongCodec.ATMOS: r"audio-atmos-.*",
     SongCodec.AC3: r"audio-ac3-.*",
     SongCodec.ALAC: r"audio-alac-.*",
 }
 
 MUSIC_VIDEO_CODEC_MAP = {
-    MusicVideoCodec.H264_BEST: "avc1",
-    MusicVideoCodec.H265_BEST: "hvc1",
+    MusicVideoCodec.H264: "avc1",
+    MusicVideoCodec.H265: "hvc1",
 }
 
 SYNCED_LYRICS_FILE_EXTENSION_MAP = {
     SyncedLyricsFormat.LRC: ".lrc",
     SyncedLyricsFormat.SRT: ".srt",
     SyncedLyricsFormat.TTML: ".ttml",
 }
```

### Comparing `gamdl-2.1.8/gamdl/downloader.py` & `gamdl-2.2/gamdl/downloader_song.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,342 +1,373 @@
 from __future__ import annotations
 
 import base64
-import functools
+import datetime
+import json
 import re
-import shutil
 import subprocess
 from pathlib import Path
+from xml.dom import minidom
+from xml.etree import ElementTree
 
-import ciso8601
-import requests
-from mutagen.mp4 import MP4, MP4Cover
-from pywidevine import PSSH, Cdm, Device
-from yt_dlp import YoutubeDL
-
-from .apple_music_api import AppleMusicApi
-from .constants import MP4_TAGS_MAP
-from .enums import CoverFormat, DownloadMode, RemuxMode
-from .hardcoded_wvd import HARDCODED_WVD
-from .itunes_api import ItunesApi
-from .models import DownloadQueueItem, UrlInfo
-
-
-class Downloader:
-    ILLEGAL_CHARACTERS_REGEX = r'[\\/:*?"<>|;]'
+from InquirerPy import inquirer
+from InquirerPy.base.control import Choice
+import m3u8
+
+from .constants import SONG_CODEC_REGEX_MAP, SYNCED_LYRICS_FILE_EXTENSION_MAP
+from .downloader import Downloader
+from .enums import RemuxMode, SongCodec, SyncedLyricsFormat
+from .models import Lyrics, StreamInfo
+
+
+class DownloaderSong:
+    DEFAULT_DECRYPTION_KEY = "32b8ade1769e26b1ffb8986352793fc6"
+    MP4_FORMAT_CODECS = ["ec-3"]
 
     def __init__(
         self,
-        apple_music_api: AppleMusicApi,
-        itunes_api: ItunesApi,
-        output_path: Path = Path("./Apple Music"),
-        temp_path: Path = Path("./temp"),
-        wvd_path: Path = None,
-        nm3u8dlre_path: str = "N_m3u8dl-RE",
-        mp4decrypt_path: str = "mp4decrypt",
-        ffmpeg_path: str = "ffmpeg",
-        mp4box_path: str = "MP4Box",
-        download_mode: DownloadMode = DownloadMode.YTDLP,
-        remux_mode: RemuxMode = RemuxMode.FFMPEG,
-        cover_format: CoverFormat = CoverFormat.JPG,
-        template_folder_album: str = "{album_artist}/{album}",
-        template_folder_compilation: str = "Compilations/{album}",
-        template_file_single_disc: str = "{track:02d} {title}",
-        template_file_multi_disc: str = "{disc}-{track:02d} {title}",
-        template_folder_no_album: str = "{artist}/Unknown Album",
-        template_file_no_album: str = "{title}",
-        template_date: str = "%Y-%m-%dT%H:%M:%SZ",
-        exclude_tags: str = None,
-        cover_size: int = 1200,
-        truncate: int = 40,
-        silent: bool = False,
+        downloader: Downloader,
+        codec: SongCodec = SongCodec.AAC_LEGACY,
+        synced_lyrics_format: SyncedLyricsFormat = SyncedLyricsFormat.LRC,
     ):
-        self.apple_music_api = apple_music_api
-        self.itunes_api = itunes_api
-        self.output_path = output_path
-        self.temp_path = temp_path
-        self.wvd_path = wvd_path
-        self.nm3u8dlre_path = nm3u8dlre_path
-        self.mp4decrypt_path = mp4decrypt_path
-        self.ffmpeg_path = ffmpeg_path
-        self.mp4box_path = mp4box_path
-        self.download_mode = download_mode
-        self.remux_mode = remux_mode
-        self.cover_format = cover_format
-        self.template_folder_album = template_folder_album
-        self.template_folder_compilation = template_folder_compilation
-        self.template_file_single_disc = template_file_single_disc
-        self.template_file_multi_disc = template_file_multi_disc
-        self.template_folder_no_album = template_folder_no_album
-        self.template_file_no_album = template_file_no_album
-        self.template_date = template_date
-        self.exclude_tags = exclude_tags
-        self.cover_size = cover_size
-        self.truncate = truncate
-        self.silent = silent
-        self._set_binaries_path_full()
-        self._set_exclude_tags_list()
-        self._set_truncate()
-        self._set_subprocess_additional_args()
-
-    def _set_binaries_path_full(self):
-        self.nm3u8dlre_path_full = shutil.which(self.nm3u8dlre_path)
-        self.ffmpeg_path_full = shutil.which(self.ffmpeg_path)
-        self.mp4box_path_full = shutil.which(self.mp4box_path)
-        self.mp4decrypt_path_full = shutil.which(self.mp4decrypt_path)
-
-    def _set_exclude_tags_list(self):
-        self.exclude_tags_list = (
-            [i.lower() for i in self.exclude_tags.split(",")]
-            if self.exclude_tags is not None
-            else []
+        self.downloader = downloader
+        self.codec = codec
+        self.synced_lyrics_format = synced_lyrics_format
+
+    def get_drm_infos(self, m3u8_data: dict) -> dict:
+        drm_info_raw = next(
+            (
+                session_data
+                for session_data in m3u8_data["session_data"]
+                if session_data["data_id"] == "com.apple.hls.AudioSessionKeyInfo"
+            ),
+            None,
+        )
+        if not drm_info_raw:
+            return None
+        return json.loads(base64.b64decode(drm_info_raw["value"]).decode("utf-8"))
+
+    def get_asset_infos(self, m3u8_data: dict) -> dict:
+        return json.loads(
+            base64.b64decode(
+                next(
+                    session_data
+                    for session_data in m3u8_data["session_data"]
+                    if session_data["data_id"] == "com.apple.hls.audioAssetMetadata"
+                )["value"]
+            ).decode("utf-8")
         )
 
-    def _set_truncate(self):
-        self.truncate = None if self.truncate < 4 else self.truncate
+    def get_playlist_from_codec(self, m3u8_data: dict) -> dict | None:
+        m3u8_master_playlists = [
+            playlist
+            for playlist in m3u8_data["playlists"]
+            if re.fullmatch(
+                SONG_CODEC_REGEX_MAP[self.codec], playlist["stream_info"]["audio"]
+            )
+        ]
+        if not m3u8_master_playlists:
+            return None
+        m3u8_master_playlists.sort(key=lambda x: x["stream_info"]["average_bandwidth"])
+        return m3u8_master_playlists[-1]
+
+    def get_playlist_from_user(self, m3u8_data: dict) -> dict | None:
+        m3u8_master_playlists = [playlist for playlist in m3u8_data["playlists"]]
+        choices = [
+            Choice(
+                name=playlist["stream_info"]["audio"],
+                value=playlist,
+            )
+            for playlist in m3u8_master_playlists
+        ]
+        selected = inquirer.select(
+            message="Select which codec to download:",
+            choices=choices,
+        ).execute()
+        return selected
 
-    def _set_subprocess_additional_args(self):
-        if self.silent:
-            self.subprocess_additional_args = {
-                "stdout": subprocess.DEVNULL,
-                "stderr": subprocess.DEVNULL,
-            }
+    def get_pssh(
+        self,
+        drm_infos: dict,
+        drm_ids: list,
+    ) -> str | None:
+        drm_info = next(
+            (
+                drm_infos[drm_id]
+                for drm_id in drm_ids
+                if drm_infos[drm_id].get(
+                    "urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed"
+                )
+                and drm_id != "1"
+            ),
+            None,
+        )
+        if not drm_info:
+            return None
+        return drm_info["urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed"]["URI"]
+
+    def get_stream_info(self, track_metadata: dict) -> StreamInfo:
+        m3u8_url = track_metadata["attributes"]["extendedAssetUrls"].get("enhancedHls")
+        if not m3u8_url:
+            return StreamInfo()
+        return self._get_stream_info(m3u8_url)
+
+    def _get_stream_info(self, m3u8_url: str) -> StreamInfo:
+        stream_info = StreamInfo()
+        m3u8_obj = m3u8.load(m3u8_url)
+        m3u8_data = m3u8_obj.data
+        drm_infos = self.get_drm_infos(m3u8_data)
+        if not drm_infos:
+            return stream_info
+        asset_infos = self.get_asset_infos(m3u8_data)
+        if self.codec == SongCodec.ASK:
+            playlist = self.get_playlist_from_user(m3u8_data)
         else:
-            self.subprocess_additional_args = {}
+            playlist = self.get_playlist_from_codec(m3u8_data)
+        if playlist is None:
+            return stream_info
+        stream_info.stream_url = m3u8_obj.base_uri + playlist["uri"]
+        variant_id = playlist["stream_info"]["stable_variant_id"]
+        drm_ids = asset_infos[variant_id]["AUDIO-SESSION-KEY-IDS"]
+        pssh = self.get_pssh(drm_infos, drm_ids)
+        stream_info.pssh = pssh
+        stream_info.codec = playlist["stream_info"]["codecs"]
+        return stream_info
 
-    def set_cdm(self):
-        if self.wvd_path:
-            self.cdm = Cdm.from_device(Device.load(self.wvd_path))
+    @staticmethod
+    def parse_datetime_obj_from_timestamp_ttml(
+        timestamp_ttml: str,
+    ) -> datetime.datetime:
+        mins_secs_ms = re.findall(r"\d+", timestamp_ttml)
+        ms, secs, mins = 0, 0, 0
+        if len(mins_secs_ms) == 2 and ":" in timestamp_ttml:
+            secs, mins = int(mins_secs_ms[-1]), int(mins_secs_ms[-2])
+        elif len(mins_secs_ms) == 1:
+            ms = int(mins_secs_ms[-1])
         else:
-            self.cdm = Cdm.from_device(Device.loads(HARDCODED_WVD))
+            secs = float(f"{mins_secs_ms[-2]}.{mins_secs_ms[-1]}")
+            if len(mins_secs_ms) > 2:
+                mins = int(mins_secs_ms[-3])
+        return datetime.datetime.fromtimestamp((mins * 60) + secs + (ms / 1000))
+
+    def get_lyrics_synced_timestamp_lrc(self, timestamp_ttml: str) -> str:
+        datetime_obj = self.parse_datetime_obj_from_timestamp_ttml(timestamp_ttml)
+        ms_new = datetime_obj.strftime("%f")[:-3]
+        if int(ms_new[-1]) >= 5:
+            ms = int(f"{int(ms_new[:2]) + 1}") * 10
+            datetime_obj += datetime.timedelta(milliseconds=ms) - datetime.timedelta(
+                microseconds=datetime_obj.microsecond
+            )
+        return datetime_obj.strftime("%M:%S.%f")[:-4]
 
-    def get_url_info(self, url: str) -> UrlInfo:
-        url_info = UrlInfo()
-        url_regex_result = re.search(
-            r"/([a-z]{2})/(album|playlist|song|music-video|post)/([^/]*)(?:/([^/?]*))?(?:\?i=)?([0-9a-z]*)?",
-            url,
-        )
-        url_info.storefront = url_regex_result.group(1)
-        url_info.type = (
-            "song" if url_regex_result.group(5) else url_regex_result.group(2)
-        )
-        url_info.id = (
-            url_regex_result.group(5)
-            or url_regex_result.group(4)
-            or url_regex_result.group(3)
-        )
-        return url_info
+    def get_lyrics_synced_timestamp_srt(self, timestamp_ttml: str) -> str:
+        datetime_obj = self.parse_datetime_obj_from_timestamp_ttml(timestamp_ttml)
+        return datetime_obj.strftime("00:%M:%S,%f")[:-3]
 
-    def get_download_queue(self, url_info: UrlInfo) -> list[DownloadQueueItem]:
-        return self._get_download_queue(url_info.type, url_info.id)
+    def get_lyrics_synced_line_lrc(self, timestamp_ttml: str, text: str) -> str:
+        return f"[{self.get_lyrics_synced_timestamp_lrc(timestamp_ttml)}]{text}"
 
-    def _get_download_queue(self, url_type: str, id: str) -> list[DownloadQueueItem]:
-        download_queue = []
-        if url_type == "song":
-            download_queue.append(DownloadQueueItem(self.apple_music_api.get_song(id)))
-        elif url_type == "album":
-            album = self.apple_music_api.get_album(id)
-            download_queue.extend(
-                DownloadQueueItem(track)
-                for track in album["relationships"]["tracks"]["data"]
-            )
-        elif url_type == "playlist":
-            download_queue.extend(
-                DownloadQueueItem(track)
-                for track in self.apple_music_api.get_playlist(id)["relationships"][
-                    "tracks"
-                ]["data"]
+    def get_lyrics_synced_line_srt(
+        self,
+        index: int,
+        timestamp_ttml_start: str,
+        timestamp_ttml_end: str,
+        text: str,
+    ) -> str:
+        timestamp_srt_start = self.get_lyrics_synced_timestamp_srt(timestamp_ttml_start)
+        timestamp_srt_end = self.get_lyrics_synced_timestamp_srt(timestamp_ttml_end)
+        return f"{index}\n{timestamp_srt_start} --> {timestamp_srt_end}\n{text}\n"
+
+    def get_lyrics(self, track_metadata: dict) -> Lyrics:
+        lyrics = Lyrics()
+        if not track_metadata["attributes"]["hasLyrics"]:
+            return lyrics
+        elif track_metadata.get("relationships") is None:
+            track_metadata = self.downloader.apple_music_api.get_song(
+                track_metadata["id"]
             )
-        elif url_type == "music-video":
-            download_queue.append(
-                DownloadQueueItem(self.apple_music_api.get_music_video(id))
+        if (
+            track_metadata["relationships"].get("lyrics")
+            and track_metadata["relationships"]["lyrics"].get("data")
+            and track_metadata["relationships"]["lyrics"]["data"][0].get("attributes")
+        ):
+            lyrics = self._get_lyrics(
+                track_metadata["relationships"]["lyrics"]["data"][0]["attributes"][
+                    "ttml"
+                ]
             )
-        elif url_type == "post":
-            download_queue.append(DownloadQueueItem(self.apple_music_api.get_post(id)))
-        else:
-            raise Exception(f"Invalid url type: {url_type}")
-        return download_queue
+        return lyrics
 
-    def sanitize_date(self, date: str):
-        datetime_obj = ciso8601.parse_datetime(date)
-        return datetime_obj.strftime(self.template_date)
-
-    def get_decryption_key(self, pssh: str, track_id: str) -> str:
-        pssh_obj = PSSH(pssh.split(",")[-1])
-        cdm_session = self.cdm.open()
-        challenge = base64.b64encode(
-            self.cdm.get_license_challenge(cdm_session, pssh_obj)
-        ).decode()
-        license = self.apple_music_api.get_widevine_license(
-            track_id,
-            pssh,
-            challenge,
-        )
-        self.cdm.parse_license(cdm_session, license)
-        decryption_key = next(
-            i for i in self.cdm.get_keys(cdm_session) if i.type == "CONTENT"
-        ).key.hex()
-        self.cdm.close(cdm_session)
-        return decryption_key
-
-    def download(self, path: Path, stream_url: str):
-        if self.download_mode == DownloadMode.YTDLP:
-            self.download_ytdlp(path, stream_url)
-        elif self.download_mode == DownloadMode.NM3U8DLRE:
-            self.download_nm3u8dlre(path, stream_url)
-
-    def download_ytdlp(self, path: Path, stream_url: str):
-        with YoutubeDL(
-            {
-                "quiet": True,
-                "no_warnings": True,
-                "outtmpl": str(path),
-                "allow_unplayable_formats": True,
-                "fixup": "never",
-                "allowed_extractors": ["generic"],
-                "noprogress": self.silent,
-            }
-        ) as ydl:
-            ydl.download(stream_url)
+    def _get_lyrics(self, lyrics_ttml: str) -> Lyrics:
+        lyrics = Lyrics("", "")
+        lyrics_ttml_et = ElementTree.fromstring(lyrics_ttml)
+        index = 1
+        for div in lyrics_ttml_et.iter("{http://www.w3.org/ns/ttml}div"):
+            for p in div.iter("{http://www.w3.org/ns/ttml}p"):
+                if p.text is not None:
+                    lyrics.unsynced += p.text + "\n"
+                if p.attrib.get("begin"):
+                    if self.synced_lyrics_format == SyncedLyricsFormat.LRC:
+                        lyrics.synced += f"{self.get_lyrics_synced_line_lrc(p.attrib.get('begin'), p.text)}"
+                    elif self.synced_lyrics_format == SyncedLyricsFormat.SRT:
+                        lyrics.synced += f"{self.get_lyrics_synced_line_srt(index, p.attrib.get('begin'), p.attrib.get('end'), p.text)}"
+                    elif self.synced_lyrics_format == SyncedLyricsFormat.TTML:
+                        if not lyrics.synced:
+                            lyrics.synced = minidom.parseString(
+                                lyrics_ttml
+                            ).toprettyxml()
+                        continue
+                    lyrics.synced += "\n"
+                    index += 1
+            lyrics.unsynced += "\n"
+        lyrics.unsynced = lyrics.unsynced[:-2]
+        return lyrics
+
+    def get_tags(self, webplayback: dict, lyrics_unsynced: str) -> dict:
+        tags_raw = webplayback["assets"][0]["metadata"]
+        tags = {
+            "album": tags_raw["playlistName"],
+            "album_artist": tags_raw["playlistArtistName"],
+            "album_id": int(tags_raw["playlistId"]),
+            "album_sort": tags_raw["sort-album"],
+            "artist": tags_raw["artistName"],
+            "artist_id": int(tags_raw["artistId"]),
+            "artist_sort": tags_raw["sort-artist"],
+            "comments": tags_raw.get("comments"),
+            "compilation": tags_raw["compilation"],
+            "composer": tags_raw.get("composerName"),
+            "composer_id": (
+                int(tags_raw.get("composerId")) if tags_raw.get("composerId") else None
+            ),
+            "composer_sort": tags_raw.get("sort-composer"),
+            "copyright": tags_raw.get("copyright"),
+            "date": (
+                self.downloader.sanitize_date(tags_raw["releaseDate"])
+                if tags_raw.get("releaseDate")
+                else None
+            ),
+            "disc": tags_raw["discNumber"],
+            "disc_total": tags_raw["discCount"],
+            "gapless": tags_raw["gapless"],
+            "genre": tags_raw["genre"],
+            "genre_id": tags_raw["genreId"],
+            "lyrics": lyrics_unsynced if lyrics_unsynced else None,
+            "media_type": 1,
+            "rating": tags_raw["explicit"],
+            "storefront": tags_raw["s"],
+            "title": tags_raw["itemName"],
+            "title_id": int(tags_raw["itemId"]),
+            "title_sort": tags_raw["sort-name"],
+            "track": tags_raw["trackNumber"],
+            "track_total": tags_raw["trackCount"],
+            "xid": tags_raw.get("xid"),
+        }
+        return tags
+
+    def get_encrypted_path(self, track_id: str) -> Path:
+        return self.downloader.temp_path / f"{track_id}_encrypted.m4a"
+
+    def get_decrypted_path(self, track_id: str) -> Path:
+        return self.downloader.temp_path / f"{track_id}_decrypted.m4a"
+
+    def get_remuxed_path(self, track_id: str) -> Path:
+        return self.downloader.temp_path / f"{track_id}_remuxed.m4a"
+
+    def fix_key_id(self, encrypted_path: Path):
+        count = 0
+        with open(encrypted_path, "rb+") as file:
+            while data := file.read(4096):
+                pos = file.tell()
+                i = 0
+                while tenc := max(0, data.find(b"tenc", i)):
+                    kid = tenc + 12
+                    file.seek(max(0, pos - 4096) + kid, 0)
+                    file.write(bytes.fromhex(f"{count:032}"))
+                    count += 1
+                    i = kid + 1
+                file.seek(pos, 0)
 
-    def download_nm3u8dlre(self, path: Path, stream_url: str):
-        path.parent.mkdir(parents=True, exist_ok=True)
+    def decrypt(
+        self,
+        encrypted_path: Path,
+        decrypted_path: Path,
+        decryption_key: str,
+    ):
+        self.fix_key_id(encrypted_path)
         subprocess.run(
             [
-                self.nm3u8dlre_path_full,
-                stream_url,
-                "--binary-merge",
-                "--no-log",
-                "--log-level",
-                "off",
-                "--ffmpeg-binary-path",
-                self.ffmpeg_path_full,
-                "--save-name",
-                path.stem,
-                "--save-dir",
-                path.parent,
-                "--tmp-dir",
-                path.parent,
+                self.downloader.mp4decrypt_path_full,
+                encrypted_path,
+                "--key",
+                f"00000000000000000000000000000001:{decryption_key}",
+                "--key",
+                f"00000000000000000000000000000000:{self.DEFAULT_DECRYPTION_KEY}",
+                decrypted_path,
             ],
             check=True,
-            **self.subprocess_additional_args,
+            **self.downloader.subprocess_additional_args,
         )
 
-    def get_sanitized_string(self, dirty_string: str, is_folder: bool) -> str:
-        dirty_string = re.sub(self.ILLEGAL_CHARACTERS_REGEX, "_", dirty_string)
-        if is_folder:
-            dirty_string = dirty_string[: self.truncate]
-            if dirty_string.endswith("."):
-                dirty_string = dirty_string[:-1] + "_"
-        else:
-            if self.truncate is not None:
-                dirty_string = dirty_string[: self.truncate - 4]
-        return dirty_string.strip()
-
-    def get_final_path(self, tags: dict, file_extension: str) -> Path:
-        if tags.get("album"):
-            final_path_folder = (
-                self.template_folder_compilation.split("/")
-                if tags.get("compilation")
-                else self.template_folder_album.split("/")
-            )
-            final_path_file = (
-                self.template_file_multi_disc.split("/")
-                if tags["disc_total"] > 1
-                else self.template_file_single_disc.split("/")
-            )
-        else:
-            final_path_folder = self.template_folder_no_album.split("/")
-            final_path_file = self.template_file_no_album.split("/")
-        final_path_folder = [
-            self.get_sanitized_string(i.format(**tags), True) for i in final_path_folder
-        ]
-        final_path_file = [
-            self.get_sanitized_string(i.format(**tags), True)
-            for i in final_path_file[:-1]
-        ] + [
-            self.get_sanitized_string(final_path_file[-1].format(**tags), False)
-            + file_extension
-        ]
-        return self.output_path.joinpath(*final_path_folder).joinpath(*final_path_file)
+    def remux(self, decrypted_path: Path, remuxed_path: Path, codec: str):
+        if self.downloader.remux_mode == RemuxMode.MP4BOX:
+            self.remux_mp4box(decrypted_path, remuxed_path)
+        elif self.downloader.remux_mode == RemuxMode.FFMPEG:
+            self.remux_ffmpeg(decrypted_path, remuxed_path, codec)
 
-    def get_cover_url(self, metadata: dict) -> str:
-        return self._get_cover_url(metadata["attributes"]["artwork"]["url"])
-
-    def _get_cover_url(self, cover_url_template: str) -> str:
-        return re.sub(
-            r"\{w\}x\{h\}([a-z]{2})\.jpg",
-            f"{self.cover_size}x{self.cover_size}bb.{self.cover_format.value}",
-            cover_url_template,
+    def remux_mp4box(self, decrypted_path: Path, remuxed_path: Path):
+        subprocess.run(
+            [
+                self.downloader.mp4box_path_full,
+                "-quiet",
+                "-add",
+                decrypted_path,
+                "-itags",
+                "artist=placeholder",
+                "-keep-utc",
+                "-new",
+                remuxed_path,
+            ],
+            check=True,
+            **self.downloader.subprocess_additional_args,
         )
 
-    @staticmethod
-    @functools.lru_cache()
-    def get_url_response_bytes(url: str) -> bytes:
-        return requests.get(url).content
-
-    def apply_tags(
-        self,
-        path: Path,
-        tags: dict,
-        cover_url: str,
-    ):
-        to_apply_tags = [
-            tag_name
-            for tag_name in tags.keys()
-            if tag_name not in self.exclude_tags_list
-        ]
-        mp4_tags = {}
-        for tag_name in to_apply_tags:
-            if tag_name in ("disc", "disc_total"):
-                if mp4_tags.get("disk") is None:
-                    mp4_tags["disk"] = [[0, 0]]
-                if tag_name == "disc":
-                    mp4_tags["disk"][0][0] = tags[tag_name]
-                elif tag_name == "disc_total":
-                    mp4_tags["disk"][0][1] = tags[tag_name]
-            elif tag_name in ("track", "track_total"):
-                if mp4_tags.get("trkn") is None:
-                    mp4_tags["trkn"] = [[0, 0]]
-                if tag_name == "track":
-                    mp4_tags["trkn"][0][0] = tags[tag_name]
-                elif tag_name == "track_total":
-                    mp4_tags["trkn"][0][1] = tags[tag_name]
-            elif tag_name == "compilation":
-                mp4_tags["cpil"] = tags["compilation"]
-            elif tag_name == "gapless":
-                mp4_tags["pgap"] = tags["gapless"]
-            elif (
-                MP4_TAGS_MAP.get(tag_name) is not None
-                and tags.get(tag_name) is not None
-            ):
-                mp4_tags[MP4_TAGS_MAP[tag_name]] = [tags[tag_name]]
-        if "cover" not in self.exclude_tags_list:
-            mp4_tags["covr"] = [
-                MP4Cover(
-                    self.get_url_response_bytes(cover_url),
-                    imageformat=(
-                        MP4Cover.FORMAT_JPEG
-                        if self.cover_format == CoverFormat.JPG
-                        else MP4Cover.FORMAT_PNG
-                    ),
-                )
-            ]
-        mp4 = MP4(path)
-        mp4.clear()
-        mp4.update(mp4_tags)
-        mp4.save()
-
-    def move_to_output_path(
+    def remux_ffmpeg(
         self,
+        decrypted_path: Path,
         remuxed_path: Path,
-        final_path: Path,
+        codec: str,
     ):
-        final_path.parent.mkdir(parents=True, exist_ok=True)
-        shutil.move(remuxed_path, final_path)
+        use_mp4_format = any(
+            codec.startswith(possible_codec)
+            for possible_codec in self.MP4_FORMAT_CODECS
+        )
+        subprocess.run(
+            [
+                self.downloader.ffmpeg_path_full,
+                "-loglevel",
+                "error",
+                "-y",
+                "-i",
+                decrypted_path,
+                "-c",
+                "copy",
+                "-f",
+                "mp4" if use_mp4_format else "ipod",
+                "-movflags",
+                "+faststart",
+                remuxed_path,
+            ],
+            check=True,
+            **self.downloader.subprocess_additional_args,
+        )
+
+    def get_lyrics_synced_path(self, final_path: Path) -> Path:
+        return final_path.with_suffix(
+            SYNCED_LYRICS_FILE_EXTENSION_MAP[self.synced_lyrics_format]
+        )
 
-    @functools.lru_cache()
-    def save_cover(self, cover_path: Path, cover_url: str):
-        cover_path.write_bytes(self.get_url_response_bytes(cover_url))
+    def get_cover_path(self, final_path: Path) -> Path:
+        return final_path.parent / f"Cover.{self.downloader.cover_format.value}"
 
-    def cleanup_temp_path(self):
-        shutil.rmtree(self.temp_path)
+    def save_lyrics_synced(self, lyrics_synced_path: Path, lyrics_synced: str):
+        lyrics_synced_path.parent.mkdir(parents=True, exist_ok=True)
+        lyrics_synced_path.write_text(lyrics_synced, encoding="utf8")
```

### Comparing `gamdl-2.1.8/gamdl/downloader_music_video.py` & `gamdl-2.2/gamdl/downloader_music_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from __future__ import annotations
 
 import re
 import subprocess
 import urllib.parse
 from pathlib import Path
-
-import click
 import m3u8
-from tabulate import tabulate
+from InquirerPy import inquirer
+from InquirerPy.base.control import Choice
 
 from .constants import MUSIC_VIDEO_CODEC_MAP
 from .downloader import Downloader
 from .enums import MusicVideoCodec, RemuxMode
 from .models import StreamInfo
 
 
 class DownloaderMusicVideo:
     MP4_FORMAT_CODECS = ["hvc1", "ec-3"]
 
     def __init__(
         self,
         downloader: Downloader,
-        codec: MusicVideoCodec = MusicVideoCodec.H264_BEST,
+        codec: MusicVideoCodec = MusicVideoCodec.H264,
     ):
         self.downloader = downloader
         self.codec = codec
 
     def get_stream_url_master(self, itunes_page: dict) -> str:
         return itunes_page["offers"][0]["assets"][0]["hlsUrl"]
 
@@ -50,42 +49,42 @@
             )
         ]
         if not playlists_filtered:
             playlists_filtered = [
                 playlist
                 for playlist in playlists
                 if playlist["stream_info"]["codecs"].startswith(
-                    MUSIC_VIDEO_CODEC_MAP[MusicVideoCodec.H264_BEST]
+                    MUSIC_VIDEO_CODEC_MAP[MusicVideoCodec.H264]
                 )
             ]
         playlists_filtered.sort(key=lambda x: x["stream_info"]["bandwidth"])
         return playlists_filtered[-1]
 
     def get_playlist_video_from_user(
         self,
         playlists: list[dict],
     ) -> dict:
-        table = [
-            [
-                i,
-                playlist["stream_info"]["codecs"],
-                playlist["stream_info"]["resolution"],
-                playlist["stream_info"]["bandwidth"],
-            ]
-            for i, playlist in enumerate(playlists, 1)
-        ]
-        print(tabulate(table))
-        try:
-            choice = (
-                click.prompt("Choose a video codec", type=click.IntRange(1, len(table)))
-                - 1
+        choices = [
+            Choice(
+                name=" | ".join(
+                    [
+                        playlist["stream_info"]["codecs"][:4],
+                        playlist["stream_info"]["resolution"],
+                        str(playlist["stream_info"]["bandwidth"]),
+                    ]
+                ),
+                value=playlist,
             )
-        except click.exceptions.Abort:
-            raise KeyboardInterrupt()
-        return playlists[choice]
+            for playlist in playlists
+        ]
+        selected = inquirer.select(
+            message="Select which video codec to download: (Codec | Resolution | Bitrate)",
+            choices=choices,
+        ).execute()
+        return selected
 
     def get_playlist_audio(
         self,
         playlists: list[dict],
     ) -> dict:
         stream_url = next(
             (
@@ -97,32 +96,26 @@
         )
         return stream_url
 
     def get_playlist_audio_from_user(
         self,
         playlists: list[dict],
     ) -> dict:
-        table = [
-            [
-                i,
-                playlist["group_id"],
-            ]
-            for i, playlist in enumerate(playlists, 1)
-        ]
-        print(tabulate(table))
-        try:
-            choice = (
-                click.prompt(
-                    "Choose an audio codec", type=click.IntRange(1, len(table))
-                )
-                - 1
+        choices = [
+            Choice(
+                name=playlist["group_id"],
+                value=playlist,
             )
-        except click.exceptions.Abort:
-            raise KeyboardInterrupt()
-        return playlists[choice]
+            for playlist in playlists
+        ]
+        selected = inquirer.select(
+            message="Select which audio codec to download:",
+            choices=choices,
+        ).execute()
+        return selected
 
     def get_pssh(self, m3u8_data: dict):
         return next(
             (
                 key
                 for key in m3u8_data["keys"]
                 if key["keyformat"] == "urn:uuid:edef8ba9-79d6-4ace-a3c8-27dcd51d21ed"
```

### Comparing `gamdl-2.1.8/gamdl/downloader_post.py` & `gamdl-2.2/gamdl/downloader_post.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from pathlib import Path
 
-import click
-from tabulate import tabulate
+from InquirerPy import inquirer
+from InquirerPy.base.control import Choice
 
 from .downloader import Downloader
 from .enums import PostQuality
 
 
 class DownloaderPost:
     QUALITY_RANK = [
@@ -36,29 +36,26 @@
             ),
             None,
         )
         return metadata["attributes"]["assetTokens"][best_quality]
 
     def get_stream_url_from_user(self, metadata: dict) -> str:
         qualities = list(metadata["attributes"]["assetTokens"].keys())
-        table = [
-            [index, quality]
-            for index, quality in enumerate(
-                qualities,
-                start=1,
+        choices = [
+            Choice(
+                name=quality,
+                value=quality,
             )
+            for quality in qualities
         ]
-        print(tabulate(table))
-        try:
-            choice = (
-                click.prompt("Choose a quality", type=click.IntRange(1, len(table))) - 1
-            )
-        except click.exceptions.Abort:
-            raise KeyboardInterrupt()
-        return metadata["attributes"]["assetTokens"][qualities[choice]]
+        selected = inquirer.select(
+            message="Select which quality to download:",
+            choices=choices,
+        ).execute()
+        return metadata["attributes"]["assetTokens"][selected]
 
     def get_stream_url(self, metadata: dict) -> str:
         if self.quality == PostQuality.BEST:
             stream_url = self.get_stream_url_best(metadata)
         elif self.quality == PostQuality.ASK:
             stream_url = self.get_stream_url_from_user(metadata)
         return stream_url
```

### Comparing `gamdl-2.1.8/gamdl/downloader_song_legacy.py` & `gamdl-2.2/gamdl/downloader_song_legacy.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.8/gamdl/enums.py` & `gamdl-2.2/gamdl/enums.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 class SyncedLyricsFormat(Enum):
     LRC = "lrc"
     SRT = "srt"
     TTML = "ttml"
 
 
 class MusicVideoCodec(Enum):
-    H264_BEST = "h264-best"
-    H265_BEST = "h265-best"
+    H264 = "h264"
+    H265 = "h265"
     ASK = "ask"
 
 
 class PostQuality(Enum):
     BEST = "best"
     ASK = "ask"
```

### Comparing `gamdl-2.1.8/gamdl/hardcoded_wvd.py` & `gamdl-2.2/gamdl/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.8/gamdl/itunes_api.py` & `gamdl-2.2/gamdl/itunes_api.py`

 * *Files identical despite different names*

### Comparing `gamdl-2.1.8/pyproject.toml` & `gamdl-2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "gamdl"
-description = "A Python CLI app to download Apple Music songs/music videos/albums/playlists/posts."
+description = "A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts."
 requires-python = ">=3.8"
 authors = [{ name = "glomatico" }]
 dependencies = [
     "ciso8601",
     "click",
+    "inquirerpy",
     "m3u8",
-    "tabulate",
     "pywidevine",
     "pyyaml",
     "yt-dlp",
 ]
 readme = "README.md"
 dynamic = ["version"]
```

### Comparing `gamdl-2.1.8/PKG-INFO` & `gamdl-2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gamdl
-Version: 2.1.8
-Summary: A Python CLI app to download Apple Music songs/music videos/albums/playlists/posts.
+Version: 2.2
+Summary: A Python CLI app for downloading Apple Music songs/music videos/albums/playlists/posts.
 Author: glomatico
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: ciso8601
 Requires-Dist: click
+Requires-Dist: inquirerpy
 Requires-Dist: m3u8
-Requires-Dist: tabulate
 Requires-Dist: pywidevine
 Requires-Dist: pyyaml
 Requires-Dist: yt-dlp
 Project-URL: homepage, https://github.com/glomatico/gamdl
 Project-URL: repository, https://github.com/glomatico/gamdl
 
 # Glomatico's Apple Music Downloader
@@ -23,14 +23,15 @@
 ## Features
 * Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
 * Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
+* Use artist links to download all of their albums or music videos
 
 ## Prerequisites
 * Python 3.8 or higher
 * The cookies file of your Apple Music account (requires an active subscription)
     * You can get your cookies by using one of the following extensions on your browser of choice at the Apple Music website with your account signed in:
         * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
         * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
@@ -60,23 +61,27 @@
     ```bash
     gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1624945511?i=1624945512"
     ```
 * Download an album
     ```bash
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1624945511"
     ```
+* Choose which albums or music videos to download from an artist
+    ```bash
+    gamdl "https://music.apple.com/us/artist/rick-astley/669771"
+    ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
 | Command line argument / Config file key                         | Description                                                                  | Default value                                |
 | --------------------------------------------------------------- | ---------------------------------------------------------------------------- | -------------------------------------------- |
 | `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.                     | `false`                                      |
 | `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                               | `false`                                      |
 | `--overwrite` / `overwrite`                                     | Overwrite existing files.                                                    | `false`                                      |
-| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.                       | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs separated by newlines. | `false`                                      |
 | `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                             | `false`                                      |
 | `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                            | `false`                                      |
 | `--config-path` / -                                             | Path to config file.                                                         | `<home>/.spotify-web-downloader/config.json` |
 | `--log-level` / `log_level`                                     | Log level.                                                                   | `INFO`                                       |
 | `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                            | `false`                                      |
 | `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                                   | `./cookies.txt`                              |
 | `--language`, `-l` / `language`                                 | Metadata language as an ISO-2A language code (don't always work for videos). | `en-US`                                      |
@@ -98,15 +103,15 @@
 | `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.                  | `{title}`                                    |
 | `--template-date` / `template_date`                             | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
 | `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
 | `--cover-size` / `cover_size`                                   | Cover size.                                                                  | `1200`                                       |
 | `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
 | `--codec-song` / `codec_song`                                   | Song codec.                                                                  | `aac-legacy`                                 |
 | `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                                        | `lrc`                                        |
-| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264-best`                                  |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                           | `h264`                                       |
 | `--quality-post` / `quality_post`                               | Post video quality.                                                          | `best`                                       |
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
@@ -174,16 +179,16 @@
 * `ask`
     * When using this option, gamdl will ask you which **non-legacy** codec to use that is available for the song.
 
 **Support for non-legacy codecs are not guaranteed, as most of the songs cannot be downloaded when using non-legacy codecs.**
 
 ### Music videos codecs
 The following codecs are available:
-* `h264-best` (up to 1080p, with AAC 256kbps)
-* `h265-best` (up to 2160p, with AAC 256kpbs)
+* `h264` (up to 1080p, with AAC 256kbps)
+* `h265` (up to 2160p, with AAC 256kpbs)
 * `ask`
     * When using this option, gamdl will ask you which audio and video codec to use that is available for the music video.
   
 ### Post videos/extra videos qualities
 The following qualities are available:
 * `best` (up to 1080p, with AAC 256kbps)
 * `ask`
```

