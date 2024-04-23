# Comparing `tmp/mitene_download-0.2.0.tar.gz` & `tmp/mitene_download-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitene_download-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mitene_download-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mitene_download-0.2.0.tar` & `mitene_download-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      444 2023-10-06 14:18:38.275574 mitene_download-0.2.0/.github/workflows/build.yaml
--rw-r--r--   0        0        0      860 2023-10-06 14:18:38.275574 mitene_download-0.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0       15 2023-10-06 14:18:38.275574 mitene_download-0.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2023-10-06 14:18:38.275574 mitene_download-0.2.0/LICENCE
--rw-r--r--   0        0        0      707 2023-10-06 14:18:38.275574 mitene_download-0.2.0/README.md
--rw-r--r--   0        0        0     4792 2023-10-06 14:58:24.715702 mitene_download-0.2.0/mitene_download.py
--rw-r--r--   0        0        0      938 2023-10-06 14:18:38.275574 mitene_download-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mitene_download-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      452 2024-04-23 15:23:29.592038 mitene_download-0.2.1/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      907 2024-04-23 15:23:02.328037 mitene_download-0.2.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0       15 2024-03-30 14:02:18.928890 mitene_download-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1072 2024-03-30 14:02:18.928890 mitene_download-0.2.1/LICENCE
+-rw-r--r--   0        0        0      707 2024-03-30 14:02:18.928890 mitene_download-0.2.1/README.md
+-rw-r--r--   0        0        0     4855 2024-04-23 15:22:04.720035 mitene_download-0.2.1/mitene_download.py
+-rw-r--r--   0        0        0      955 2024-04-23 15:23:41.648039 mitene_download-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mitene_download-0.2.1/PKG-INFO
```

### Comparing `mitene_download-0.2.0/.github/workflows/lint.yml` & `mitene_download-0.2.1/.github/workflows/lint.yml`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 on: [push]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install pylint mypy yapf isort .
+        pip install pylint mypy ruff isort .
     - name: Analysing the code with pylint
       run: |
         pylint `ls -R|grep .py$|xargs`
     - name: Analysing the code with mypy
       run: |
         mypy --strict `ls -R|grep .py$|xargs`
-    - name: Check formatting with yapf
+    - name: Check with ruff
       run: |
-        yapf --diff `ls -R|grep .py$|xargs`
+        ruff check `ls -R|grep .py$|xargs`
+        ruff format --diff `ls -R|grep .py$|xargs`
     - name: Check import order with isort
       uses: jamescurtin/isort-action@master
```

### Comparing `mitene_download-0.2.0/LICENCE` & `mitene_download-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `mitene_download-0.2.0/README.md` & `mitene_download-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mitene_download-0.2.0/mitene_download.py` & `mitene_download-0.2.1/mitene_download.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-"""Download medias from https://mitene.us/ or https://family-album.com/
-"""
-__version__ = '0.2.0'
+"""Download medias from https://mitene.us/ or https://family-album.com/"""
+
+__version__ = "0.2.1"
 
 import argparse
 import asyncio
 import datetime
 import glob
 import json
 import mimetypes
 import os
+import platform
 import sys
 import urllib.parse
 from typing import Awaitable
 
 import aiohttp
 
 
 async def gather_with_concurrency(n: int, *tasks: Awaitable[None]) -> None:
-  """Like asyncio.gather but limit the number of concurent tasks.
-  """
+  """Like asyncio.gather but limit the number of concurent tasks."""
   semaphore = asyncio.Semaphore(n)
 
   async def sem_task(task: Awaitable[None]) -> None:
     async with semaphore:
       await task
 
   await asyncio.gather(*(sem_task(task) for task in tasks))
 
 
 async def download_media(
-    session: aiohttp.ClientSession,
-    url: str,
-    destination_filename: str,
-    media_name: str,
-    verbose: bool,
+  session: aiohttp.ClientSession,
+  url: str,
+  destination_filename: str,
+  media_name: str,
+  verbose: bool,
 ) -> None:
   """Download one media from URL"""
   if not os.path.exists(destination_filename):
     if verbose:
       print(f"Downloading {media_name} ⏳", flush=True)
     with open(destination_filename + ".tmp", "wb") as f:
       r = await session.get(url)
@@ -46,18 +46,18 @@
         f.write(chunk)
     os.rename(destination_filename + ".tmp", destination_filename)
   elif verbose:
     print(f"{media_name} already downloaded ✔️", flush=True)
 
 
 async def async_main() -> None:
-  parser = argparse.ArgumentParser(prog='mitene_download', description=__doc__)
+  parser = argparse.ArgumentParser(prog="mitene_download", description=__doc__)
   parser.add_argument(
-      "album_url",
-      help="""
+    "album_url",
+    help="""
   URL of the album.
 
   This is the URL obtained by inviting a family member for the web version.
   """,
   )
 
   parser.add_argument("--destination-directory", default="out")
@@ -68,85 +68,90 @@
 
   os.makedirs(args.destination_directory, exist_ok=True)
   # cleanup temp files from previous run, if interrupted
   for tmp_file in glob.glob(os.path.join(args.destination_directory, "*.tmp")):
     os.unlink(tmp_file)
 
   download_coroutines = []
-  async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(
-      total=datetime.timedelta(minutes=30).total_seconds())) as session:
-
+  async with aiohttp.ClientSession(
+    timeout=aiohttp.ClientTimeout(total=datetime.timedelta(minutes=30).total_seconds())
+  ) as session:
     page = 1
     while True:
       r = await session.get(f"{args.album_url}?page={page}")
       response_text = await r.text()
-      if page == 1 and 'Please enter your password' in response_text:
+      if page == 1 and "Please enter your password" in response_text:
         if not args.password:
           print(
-              'Album is password protected, please specify password with --password',
-              file=sys.stderr)
+            "Album is password protected, please specify password with --password",
+            file=sys.stderr,
+          )
           sys.exit(1)
-        authenticity_token = response_text.split(
-            'name="authenticity_token" value="')[1].split('"')[0]
+        authenticity_token = response_text.split('name="authenticity_token" value="')[
+          1
+        ].split('"')[0]
         assert authenticity_token, "Could not parse authenticity token"
         r = await session.post(
-            f"{args.album_url}/login",
-            data={
-                'session[password]': args.password,
-                'authenticity_token': authenticity_token
-            },
+          f"{args.album_url}/login",
+          data={
+            "session[password]": args.password,
+            "authenticity_token": authenticity_token,
+          },
         )
-        if r.url.path.endswith('/login'):
-          print('Could not authenticate, maybe password is incorrect',
-                file=sys.stderr)
+        if r.url.path.endswith("/login"):
+          print("Could not authenticate, maybe password is incorrect", file=sys.stderr)
           sys.exit(1)
         continue
 
-      page_text = response_text.split("//<![CDATA[\nwindow.gon={};gon.media=")[
-          1].split(";gon.familyUserIdToColorMap=")[0]
+      page_text = response_text.split("//<![CDATA[\nwindow.gon={};gon.media=")[1].split(
+        ";gon.familyUserIdToColorMap="
+      )[0]
       data = json.loads(page_text)
 
       page += 1
       if not data["mediaFiles"]:
         break
       for media in data["mediaFiles"]:
         filename = urllib.parse.urlparse(
-            media.get("expiringVideoUrl",
-                      media["expiringUrl"])).path.split("/")[-1]
+          media.get("expiringVideoUrl", media["expiringUrl"])
+        ).path.split("/")[-1]
         filename = f'{media["tookAt"]}-{filename}'
+        if platform.system() == "Windows":
+          filename = filename.replace(":", "")
         if not os.path.splitext(filename)[1]:
-          filename = filename + mimetypes.guess_extension(media['contentType'])
+          filename = filename + mimetypes.guess_extension(media["contentType"])
         destination_filename = os.path.join(
-            args.destination_directory,
-            filename,
+          args.destination_directory,
+          filename,
         )
 
         download_coroutines.append(
-            download_media(
-                session,
-                f"{args.album_url}/media_files/{media['uuid']}/download",
-                destination_filename,
-                media['uuid'],
-                args.verbose,
-            ))
+          download_media(
+            session,
+            f"{args.album_url}/media_files/{media['uuid']}/download",
+            destination_filename,
+            media["uuid"],
+            args.verbose,
+          )
+        )
 
         if media["comments"]:
           comment_filename = os.path.splitext(destination_filename)[0] + ".md"
-          with open(comment_filename + ".tmp", "w") as comment_f:
+          with open(comment_filename + ".tmp", "w", encoding="utf-8") as comment_f:
             for comment in media["comments"]:
               if not comment["isDeleted"]:
                 comment_f.write(
-                    f'**{comment["user"]["nickname"]}**: {comment["body"]}\n\n'
+                  f'**{comment["user"]["nickname"]}**: {comment["body"]}\n\n'
                 )
           os.rename(comment_filename + ".tmp", comment_filename)
 
     await gather_with_concurrency(4, *download_coroutines)
   await session.close()
 
 
 def main() -> None:
   loop = asyncio.get_event_loop()
   loop.run_until_complete(async_main())
 
 
-if __name__ == '__main__':
-  main()
+if __name__ == "__main__":
+  main()
```

### Comparing `mitene_download-0.2.0/pyproject.toml` & `mitene_download-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 
 [project.urls]
 Source = "https://github.com/perrinjerome/mitene_download"
 
 [[project.authors]]
 name = "Jérome Perrin"
 
-[tool.yapf]
-based_on_style = "pep8"
-indent_width = 2
-
 [tool.pylint.messages_control]
 disable = "all"
 enable = [
     "E",
     "unused-variable",
     "unused-import",
+    "unspecified-encoding",
     "unreachable",
     "duplicate-key",
 ]
 
+[tool.ruff]
+indent-width = 2
+
 [tool.tox]
 legacy_tox_ini = """
     [tox]
     isolated_build = True
     package = wheel
     env_list =
         py312
         py311
         py310
         py39
+        py38
 
     [testenv]
     commands = mitene_download --help
 """
 
 [project.scripts]
 mitene_download = "mitene_download:main"
```

### Comparing `mitene_download-0.2.0/PKG-INFO` & `mitene_download-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitene_download
-Version: 0.2.0
+Version: 0.2.1
 Summary: Download medias from https://mitene.us/ or https://family-album.com/
 Author: Jérome Perrin
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: aiohttp[speedups]
 Project-URL: Source, https://github.com/perrinjerome/mitene_download
```

