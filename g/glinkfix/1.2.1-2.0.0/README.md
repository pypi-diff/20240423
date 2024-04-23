# Comparing `tmp/glinkfix-1.2.1.tar.gz` & `tmp/glinkfix-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glinkfix-1.2.1.tar", max compression
+gzip compressed data, was "glinkfix-2.0.0.tar", max compression
```

## Comparing `glinkfix-1.2.1.tar` & `glinkfix-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-12-31 18:43:56.307898 glinkfix-1.2.1/LICENSE
--rw-r--r--   0        0        0     6778 2024-01-24 11:26:05.680266 glinkfix-1.2.1/README.md
--rw-r--r--   0        0        0     1363 2024-01-23 21:57:02.464159 glinkfix-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-01-23 21:57:06.563206 glinkfix-1.2.1/src/glinkfix/__init__.py
--rwxr-xr-x   0        0        0     1217 2024-01-23 21:57:07.997053 glinkfix-1.2.1/src/glinkfix/__main__.py
--rw-r--r--   0        0        0        0 2023-12-31 18:43:56.309251 glinkfix-1.2.1/src/glinkfix/py.typed
--rw-r--r--   0        0        0     2530 2024-01-23 21:41:09.886211 glinkfix-1.2.1/src/glinkfix/tools.py
--rw-r--r--   0        0        0     7872 1970-01-01 00:00:00.000000 glinkfix-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-16 22:09:08.271980 glinkfix-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6731 2024-04-23 15:47:43.326916 glinkfix-2.0.0/README.md
+-rw-r--r--   0        0        0     1402 2024-04-23 14:47:05.083694 glinkfix-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-17 12:07:09.257983 glinkfix-2.0.0/src/glinkfix/__init__.py
+-rwxr-xr-x   0        0        0     1195 2024-04-17 16:50:52.774829 glinkfix-2.0.0/src/glinkfix/__main__.py
+-rw-r--r--   0        0        0        0 2023-12-31 18:43:56.309251 glinkfix-2.0.0/src/glinkfix/py.typed
+-rw-r--r--   0        0        0     2186 2024-04-23 13:09:28.298979 glinkfix-2.0.0/src/glinkfix/tools.py
+-rw-r--r--   0        0        0     7867 1970-01-01 00:00:00.000000 glinkfix-2.0.0/PKG-INFO
```

### Comparing `glinkfix-1.2.1/LICENSE` & `glinkfix-2.0.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 MIT License
 
 Copyright (c) 2021-2024, Peter Nardi
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a
+copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included
+in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `glinkfix-1.2.1/README.md` & `glinkfix-2.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,185 +1,203 @@
+Metadata-Version: 2.1
+Name: glinkfix
+Version: 2.0.0
+Summary: Google Drive Link Fixer
+Home-page: https://github.com/geozeke/glinkfix
+License: MIT
+Keywords: glinkfix,google,drive,link,curl,markdown,embed,image,download
+Author: Peter Nardi
+Author-email: pete@nardi.com
+Maintainer: Peter Nardi
+Maintainer-email: pete@nardi.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Utilities
+Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
+Project-URL: Bug Tracker, https://github.com/geozeke/glinkfix/issues
+Project-URL: Source Code, https://github.com/geozeke/glinkfix
+Description-Content-Type: text/markdown
+
 ![GitHub](https://img.shields.io/github/license/geozeke/glinkfix)
 ![PyPI](https://img.shields.io/pypi/v/glinkfix)
 ![PyPI - Status](https://img.shields.io/pypi/status/glinkfix)
 ![GitHub last commit](https://img.shields.io/github/last-commit/geozeke/glinkfix)
 ![GitHub issues](https://img.shields.io/github/issues/geozeke/glinkfix)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/glinkfix)
 ![GitHub repo size](https://img.shields.io/github/repo-size/geozeke/glinkfix)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/glinkfix)
 
 <br>
 
-<img src="https://github.com/geozeke/glinkfix/blob/main/assets/logo.png?raw=true"
+# glinkfix
+
+<br>
+
+<img src="https://lh3.googleusercontent.com/d/1H04KVAA3ohH_dLXIrC0bXuJXDn3VutKc"
 alt="Dinobox logo" width="120"/>
 
-# Google Drive Link Fixer
+## Google Drive Link Fixer
 
-## A note to developers
+## Notes (please read)
+
+1. It's turning into an arms race. Google keeps changing how links are
+   handled on their servers, which often breaks tools like glinkfix.
+   Direct downloading and embedding G-Drive links is definitely an
+   unsupported "off the books" feature as far as Google is concerned. As
+   of Jan 2024, Google made a significant change, which definitely broke
+   some links created with this tool. This update (Apr 2024) works, *for
+   now*, but if Google changes again, things may break.
+
+2. Viewing links that point to animated gifs may just show up as static
+   images.
+
+3. In the v2 update, in addition to displaying the fixed link on the
+   screen, glinkfix will also attempt to copy the fixed link to the
+   clipboard. Copying to the clipboard only works for Desktop-based
+   operating systems (not Server installs). Even without automatic
+   copying, link fixing will still work and the results will be
+   displayed on the screen, regardless of where you run it (Server or
+   Desktop). glinkfix uses the [pyperclip][def9] library, and automatic
+   copying to the clipboard should work seamlessly on Windows/Mac. If
+   you're running Linux and links are not automatically copied to the
+   clipboard, [refer to this note][def8] from the pyperclip developer.
+
+## To Developers
 
 If you're just using glinkfix, then carry on!
 
-If you're a developer looking to fork this repository and modify glinkfix,
-there are two important considerations:
+If you're a developer looking to fork this repository and modify
+glinkfix, there are two important considerations:
 
-1. glinkfix requires [poetry](https://python-poetry.org/) for dependency
-   management. Poetry is well behaved and if you're a Python developer you
-   should check it out. It installs itself in a virtual environment, uninstalls
-   cleanly and easily, and doesn't require `sudo` for installation. Visit the
-   [poetry site](https://python-poetry.org/) and install it using the
-   instructions for your operating system.
-
-   *Note: When you install poetry, pay careful attention to the message printed
-   by the poetry installer. It provides details on how to modify `$PATH` to
-   access the poetry runtime.*
-
-2. I've included a file called `global-gitignore.txt` which is a copy of the
-   `.gitignore` I placed in my home directory and configured globally for all
-   my development projects. The `global-gitignore.txt` file reflects my
-   development setup (for example using tools like vscode), but yours may be
-   different. Just cherry-pick any necessary elements from
-   `global-gitignore.txt` for your own use.
+1. glinkfix requires [poetry][def] for dependency management. Poetry is
+   well behaved and if you're a Python developer you should check it
+   out. It installs itself in a virtual environment, uninstalls cleanly
+   and easily, and doesn't require `sudo` for installation. Visit the
+   [poetry site][def] and install it using the instructions for your
+   operating system.
+
+   *Note: When you install poetry, pay careful attention to the message
+   printed by the poetry installer. It provides details on how to modify
+   `$PATH` to access the poetry runtime.*
+
+2. I've included a file called `global-gitignore.txt` which is a copy of
+   the `.gitignore` I placed in my home directory and configured
+   globally for all my development projects. The `global-gitignore.txt`
+   file reflects my development setup (for example using tools like
+   vscode), but yours may be different. Just cherry-pick any necessary
+   elements from `global-gitignore.txt` for your own use.
 
-   *Details on gitignore files are available on
-   [GitHub](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files).*
+   *Details on gitignore files are available on [GitHub][def2].*
 
 ## Installation
 
-The Google Drive Link Fixer is lightweight, pure Python, with no third-party
-dependencies. You could install it within a virtual environment using pip3:
+The preferred way to install glinkfix is with [pipx][def3]:
 
-```text
-pip3 install glinkfix  
+```shell
+pipx install glinkfix
 ```
 
-or
-
-You could install it using [pipx](https://pipx.pypa.io/stable/):
+Alternatively, you can create a separate virtual environment and install
+it the traditional way:
 
-```text
-pipx install glinkfix
+```shell
+pip3 install glinkfix
 ```
 
 If you just need a quick one-time link fix, and don't want to commit to
 a full installation, use:
 
-```text
+```shell
 pipx run glinkfix -h
 ```
 
 and follow the directions to run it again with the option you want.
 
 ## Purpose / Usage
 
-When you share files with Google Drive, the sharing link you get is only good
-for accessing the content through a web browser. If you want to use a Google
-Drive sharing link to embed an image in a document (e.g. in a markdown or html
-file), or you want to directly download a file pointed-to by a Google Drive
-sharing link using something like `curl` or `wget` in linux, the link needs to
-be adjusted ("fixed") for these purposes.
-
-It's not especially hard to repackage the link, but it's a pain. You have to
-copy the link to a text editor, carve it up manually, and reassemble it. If
-you've got a lot of links to deal with it starts to get very tedious. This tool
-is designed to remove the tedium.
+When you share files with Google Drive, the sharing link you get is only
+good for accessing the content through a web browser. If you want to use
+a Google Drive sharing link to embed an image in a document (e.g. in a
+markdown or html file), or you want to directly download a file
+pointed-to by a Google Drive sharing link using something like `curl` or
+`wget` in linux, the link needs to be adjusted ("fixed") for these
+purposes.
+
+It's not especially hard to repackage the link, but it's a pain. You
+have to copy the link to a text editor, carve it up manually, and
+reassemble it. If you've got a lot of links to deal with it starts to
+get very tedious. This tool is designed to remove the tedium.
 
-*Note: The animated gifs below are actually hosted on Google Drive and the
+*Note: The images below are actually hosted on Google Drive and the
 "fixed" links are embedded into this README file.*
 
 ---
 
-Start by getting a sharing link to a file on Google Drive. Make sure it's set
-up for public access (*Anyone with the link*):
+Start by getting a sharing link to a file on Google Drive. Make sure
+it's set up for public access (*Anyone with the link*):
 
-![Retrieving Google Link](https://drive.google.com/uc?export=view&id=1BJ5cR04cSzHa4xMIPApjLXv0IHPDu9U2)
+<img src="https://lh3.googleusercontent.com/d/1aHqCi_R6S9T9OI8kYLj-bH-Rd1eEgiWd"
+alt="Getting Link" width="450"/>
 
 ---
 
-Now run `glinkfix` and paste the link into the terminal. Copy the "fixed"
-version and use is as required.
+<img src="https://lh3.googleusercontent.com/d/1DM7C91o8K32B95YkVPUv9rVga6lJdYzA"
+alt="Getting Link" width="450"/>
 
-![Using Google Link](https://drive.google.com/uc?export=view&id=1wrrGh-cm_Hf7hH5WN_aCO-wwxIsrk6j5)
+Now run `glinkfix` and paste the link into the terminal. Copy the
+"fixed" version and use it as required.
 
 ---
 
 To display the help menu, run: `glinkfix -h`
 
 ```text
-usage: glinkfix [-h] (-v | -d)
+usage: glinkfix [-h] [-d]
 
-This program takes a Google Drive sharing link for a file and repackages it into a link
-that can be downloaded directly (e.g. using curl) or embedded in a document to be viewed
-(e.g. an image in a markdown document). Note: there is a size limit of 40MB for a single
-file when using Google Drive links in this manner.
+This program takes a Google Drive sharing link for a file and repackages
+it into a link that can be downloaded directly (e.g. using curl) or
+embedded in a document to be viewed (e.g. an image in a markdown
+document). Note: there is a size limit of 40MB for a single file when
+using Google Drive links in this manner.
 
 optional arguments:
   -h, --help      show this help message and exit
-  -v, --view      repackage the link for viewing (e.g. as an embedded link in a markdown
-                  document).
-  -d, --download  repackage the link for downloading (e.g. downloading using curl).
+  -d, --download  The default behavior for glinkfix is to repackage a
+                  Google Drive link to make it suitable for embedding in
+                  a website. Use this option if you want to repackage
+                  Google Drive link for direct downloading (e.g.
+                  downloading using curl).
 ```
 
 ## Usage Notes
 
-* There is a 40MB size limit for a single file when using Google Drive sharing
-  links directly for viewing or downloading. Individual files larger than 40MB
-  will not render/download properly. This limit is a function of how Google
-  Drive works and is not related to `glinkfix`.
-* When creating a download link for use with `curl` make sure to use `curl`'s
-  `-L` option to allow for redirects.
-* `glinkfix` supports links that use Google's [resource
-  key](https://support.google.com/a/answer/10685032) security feature.
+* There is a 40MB size limit for a single file when using Google Drive
+  sharing links directly for viewing or downloading. Individual files
+  larger than 40MB will not render/download properly. This limit is a
+  function of how Google Drive works and is not related to `glinkfix`.
+* When creating a download link for use with `curl` make sure to use
+  `curl`'s `-L` option to allow for redirects.
+* `glinkfix` supports links that use Google's [resource key][def6]
+ security feature.
 
 ## Version History
 
-* 1.2.1 (2024-01-24)
-  * Version re-baseline and documentation corrections. No functional
-    changes in the 1.2.x release cycle.
-    <br><br>
-* 1.2.0 (2024-01-23)
-  * Updated installation options to include [pipx](https://pipx.pypa.io/stable/).
-  <br><br>
-* 1.0.16 (2023-12-31)
-  * Cleaned up packaging for better [PEP
-  561](https://peps.python.org/pep-0561/) compliance.
-  * Dropped support for Python <=3.7
-  <br><br>
-* 1.0.15 (2023-06-23)
-  * Migrated code formatter to *black*.
-  <br><br>
-* 1.0.14 (2023-04-19)
-  * Documentation cleanup.
-  <br><br>
-* 1.0.13 (2022-11-03)
-  * Google made a breaking change to the format for sharing links (not that
-    they checked with me first 😊). This patch updates glinkfix to support the
-    change.
-  <br><br>
-* 1.0.12 (2022-10-22)
-  * Regression bug fixes.
-  <br><br>
-* 1.0.11 (2022-10-21)
-  * Migrated dependency/build management to [poetry](https://python-poetry.org/).
-  <br><br>
-* 1.0.9 (2022-10-13)
-  * Fixed a bug when IDs or resource keys contain underscore characters (`_`)
-  * Additional test case for bug fix.
-  * Moved task runner to make.
-  * Build local virtual environment for development.
-  * Code refactoring and linting.
-  <br><br>
-* 1.0.8 (2022-07-23)
-  * Implemented code coverage for testing infrastructure.
-  * Code refactoring and linting.
-  <br><br>
-* 1.0.7 (2022-07-15)
-  * Fixed handling of URLs with resource keys.
-  * Code cleanup and refactoring.
-  * Implemented custom exception handling.
-  * Implemented testing infrastructure.<br><br>
-* 1.0.6 (2022-01-17)
-  * Code cleanup.<br><br>
-* 1.0.5 (2021-12-23)
-  * Code linting.
-  * Documentation cleanup.<br><br>
-* 1.0.4 (2021-12-19)
-  * Initial release<br>
+View releases on the [glinkfix git repository][def7]
+
+[def]: https://python-poetry.org/
+[def2]: https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files
+[def3]: https://pipx.pypa.io/stable/
+[def6]: https://support.google.com/a/answer/10685032
+[def7]: https://github.com/geozeke/glinkfix
+[def8]: https://pyperclip.readthedocs.io/en/latest/index.html#not-implemented-error
+[def9]: https://pypi.org/project/pyperclip/
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `glinkfix-1.2.1/pyproject.toml` & `glinkfix-2.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glinkfix"
-version = "1.2.1"
+version = "2.0.0"
 description = "Google Drive Link Fixer"
 authors = ["Peter Nardi <pete@nardi.com>"]
 maintainers = ["Peter Nardi <pete@nardi.com>"]
 homepage = "https://github.com/geozeke/glinkfix"
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "glinkfix", from = "src" }]
@@ -38,19 +38,21 @@
 "Bug Tracker" = "https://github.com/geozeke/glinkfix/issues"
 
 [tool.poetry.scripts]
 glinkfix = "glinkfix.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+pyperclip = "^1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
 flake8 = "^5.0.4"
 flake8-docstrings = "^1.6.0"
 mypy = "^0.982"
 black = "^23.3.0"
 pytest = "^7.1.3"
+isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `glinkfix-1.2.1/src/glinkfix/__main__.py` & `glinkfix-2.0.0/src/glinkfix/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,26 +15,28 @@
     """
     msg = """This program takes a Google Drive sharing link for a
     file and repackages it into a link that can be downloaded directly
     (e.g. using curl) or embedded in a document to be viewed (e.g. an
     image in a markdown document). Note: there is a size limit of 40MB
     for a single file when using Google Drive links in this manner."""
 
-    epi = "Version: 1.2.1"
+    epi = "Version: 2.0.0"
 
     parser = argparse.ArgumentParser(description=msg, epilog=epi)
-    group = parser.add_mutually_exclusive_group(required=True)
 
-    msg = """repackage the link for viewing (e.g. as an embedded
-    link in a markdown document)."""
-    group.add_argument("-v", "--view", action="store_true", help=msg)
-
-    msg = """repackage the link for downloading (e.g. downloading
-    using curl)."""
-    group.add_argument("-d", "--download", action="store_true", help=msg)
+    msg = """ The default behavior for glinkfix is to repackage a Google
+    Drive link to make it suitable for embedding in a website. Use this
+    option if you want to repackage Google Drive link for direct
+    downloading (e.g. downloading using curl)."""
+    parser.add_argument(
+        "-d",
+        "--download",
+        action="store_true",
+        help=msg,
+    )
 
     args = parser.parse_args()
     fix_link(args)
     return
 
 
 if __name__ == "__main__":
```

### Comparing `glinkfix-1.2.1/PKG-INFO` & `glinkfix-2.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,214 +1,173 @@
-Metadata-Version: 2.1
-Name: glinkfix
-Version: 1.2.1
-Summary: Google Drive Link Fixer
-Home-page: https://github.com/geozeke/glinkfix
-License: MIT
-Keywords: glinkfix,google,drive,link,curl,markdown,embed,image,download
-Author: Peter Nardi
-Author-email: pete@nardi.com
-Maintainer: Peter Nardi
-Maintainer-email: pete@nardi.com
-Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Utilities
-Project-URL: Bug Tracker, https://github.com/geozeke/glinkfix/issues
-Project-URL: Source Code, https://github.com/geozeke/glinkfix
-Description-Content-Type: text/markdown
-
 ![GitHub](https://img.shields.io/github/license/geozeke/glinkfix)
 ![PyPI](https://img.shields.io/pypi/v/glinkfix)
 ![PyPI - Status](https://img.shields.io/pypi/status/glinkfix)
 ![GitHub last commit](https://img.shields.io/github/last-commit/geozeke/glinkfix)
 ![GitHub issues](https://img.shields.io/github/issues/geozeke/glinkfix)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/glinkfix)
 ![GitHub repo size](https://img.shields.io/github/repo-size/geozeke/glinkfix)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/glinkfix)
 
 <br>
 
-<img src="https://github.com/geozeke/glinkfix/blob/main/assets/logo.png?raw=true"
+# glinkfix
+
+<br>
+
+<img src="https://lh3.googleusercontent.com/d/1H04KVAA3ohH_dLXIrC0bXuJXDn3VutKc"
 alt="Dinobox logo" width="120"/>
 
-# Google Drive Link Fixer
+## Google Drive Link Fixer
+
+## Notes (please read)
+
+1. It's turning into an arms race. Google keeps changing how links are
+   handled on their servers, which often breaks tools like glinkfix.
+   Direct downloading and embedding G-Drive links is definitely an
+   unsupported "off the books" feature as far as Google is concerned. As
+   of Jan 2024, Google made a significant change, which definitely broke
+   some links created with this tool. This update (Apr 2024) works, *for
+   now*, but if Google changes again, things may break.
+
+2. Viewing links that point to animated gifs may just show up as static
+   images.
+
+3. In the v2 update, in addition to displaying the fixed link on the
+   screen, glinkfix will also attempt to copy the fixed link to the
+   clipboard. Copying to the clipboard only works for Desktop-based
+   operating systems (not Server installs). Even without automatic
+   copying, link fixing will still work and the results will be
+   displayed on the screen, regardless of where you run it (Server or
+   Desktop). glinkfix uses the [pyperclip][def9] library, and automatic
+   copying to the clipboard should work seamlessly on Windows/Mac. If
+   you're running Linux and links are not automatically copied to the
+   clipboard, [refer to this note][def8] from the pyperclip developer.
 
-## A note to developers
+## To Developers
 
 If you're just using glinkfix, then carry on!
 
-If you're a developer looking to fork this repository and modify glinkfix,
-there are two important considerations:
+If you're a developer looking to fork this repository and modify
+glinkfix, there are two important considerations:
 
-1. glinkfix requires [poetry](https://python-poetry.org/) for dependency
-   management. Poetry is well behaved and if you're a Python developer you
-   should check it out. It installs itself in a virtual environment, uninstalls
-   cleanly and easily, and doesn't require `sudo` for installation. Visit the
-   [poetry site](https://python-poetry.org/) and install it using the
-   instructions for your operating system.
-
-   *Note: When you install poetry, pay careful attention to the message printed
-   by the poetry installer. It provides details on how to modify `$PATH` to
-   access the poetry runtime.*
-
-2. I've included a file called `global-gitignore.txt` which is a copy of the
-   `.gitignore` I placed in my home directory and configured globally for all
-   my development projects. The `global-gitignore.txt` file reflects my
-   development setup (for example using tools like vscode), but yours may be
-   different. Just cherry-pick any necessary elements from
-   `global-gitignore.txt` for your own use.
+1. glinkfix requires [poetry][def] for dependency management. Poetry is
+   well behaved and if you're a Python developer you should check it
+   out. It installs itself in a virtual environment, uninstalls cleanly
+   and easily, and doesn't require `sudo` for installation. Visit the
+   [poetry site][def] and install it using the instructions for your
+   operating system.
+
+   *Note: When you install poetry, pay careful attention to the message
+   printed by the poetry installer. It provides details on how to modify
+   `$PATH` to access the poetry runtime.*
+
+2. I've included a file called `global-gitignore.txt` which is a copy of
+   the `.gitignore` I placed in my home directory and configured
+   globally for all my development projects. The `global-gitignore.txt`
+   file reflects my development setup (for example using tools like
+   vscode), but yours may be different. Just cherry-pick any necessary
+   elements from `global-gitignore.txt` for your own use.
 
-   *Details on gitignore files are available on
-   [GitHub](https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files).*
+   *Details on gitignore files are available on [GitHub][def2].*
 
 ## Installation
 
-The Google Drive Link Fixer is lightweight, pure Python, with no third-party
-dependencies. You could install it within a virtual environment using pip3:
+The preferred way to install glinkfix is with [pipx][def3]:
 
-```text
-pip3 install glinkfix  
+```shell
+pipx install glinkfix
 ```
 
-or
-
-You could install it using [pipx](https://pipx.pypa.io/stable/):
+Alternatively, you can create a separate virtual environment and install
+it the traditional way:
 
-```text
-pipx install glinkfix
+```shell
+pip3 install glinkfix
 ```
 
 If you just need a quick one-time link fix, and don't want to commit to
 a full installation, use:
 
-```text
+```shell
 pipx run glinkfix -h
 ```
 
 and follow the directions to run it again with the option you want.
 
 ## Purpose / Usage
 
-When you share files with Google Drive, the sharing link you get is only good
-for accessing the content through a web browser. If you want to use a Google
-Drive sharing link to embed an image in a document (e.g. in a markdown or html
-file), or you want to directly download a file pointed-to by a Google Drive
-sharing link using something like `curl` or `wget` in linux, the link needs to
-be adjusted ("fixed") for these purposes.
-
-It's not especially hard to repackage the link, but it's a pain. You have to
-copy the link to a text editor, carve it up manually, and reassemble it. If
-you've got a lot of links to deal with it starts to get very tedious. This tool
-is designed to remove the tedium.
+When you share files with Google Drive, the sharing link you get is only
+good for accessing the content through a web browser. If you want to use
+a Google Drive sharing link to embed an image in a document (e.g. in a
+markdown or html file), or you want to directly download a file
+pointed-to by a Google Drive sharing link using something like `curl` or
+`wget` in linux, the link needs to be adjusted ("fixed") for these
+purposes.
+
+It's not especially hard to repackage the link, but it's a pain. You
+have to copy the link to a text editor, carve it up manually, and
+reassemble it. If you've got a lot of links to deal with it starts to
+get very tedious. This tool is designed to remove the tedium.
 
-*Note: The animated gifs below are actually hosted on Google Drive and the
+*Note: The images below are actually hosted on Google Drive and the
 "fixed" links are embedded into this README file.*
 
 ---
 
-Start by getting a sharing link to a file on Google Drive. Make sure it's set
-up for public access (*Anyone with the link*):
+Start by getting a sharing link to a file on Google Drive. Make sure
+it's set up for public access (*Anyone with the link*):
 
-![Retrieving Google Link](https://drive.google.com/uc?export=view&id=1BJ5cR04cSzHa4xMIPApjLXv0IHPDu9U2)
+<img src="https://lh3.googleusercontent.com/d/1aHqCi_R6S9T9OI8kYLj-bH-Rd1eEgiWd"
+alt="Getting Link" width="450"/>
 
 ---
 
-Now run `glinkfix` and paste the link into the terminal. Copy the "fixed"
-version and use is as required.
+<img src="https://lh3.googleusercontent.com/d/1DM7C91o8K32B95YkVPUv9rVga6lJdYzA"
+alt="Getting Link" width="450"/>
 
-![Using Google Link](https://drive.google.com/uc?export=view&id=1wrrGh-cm_Hf7hH5WN_aCO-wwxIsrk6j5)
+Now run `glinkfix` and paste the link into the terminal. Copy the
+"fixed" version and use it as required.
 
 ---
 
 To display the help menu, run: `glinkfix -h`
 
 ```text
-usage: glinkfix [-h] (-v | -d)
+usage: glinkfix [-h] [-d]
 
-This program takes a Google Drive sharing link for a file and repackages it into a link
-that can be downloaded directly (e.g. using curl) or embedded in a document to be viewed
-(e.g. an image in a markdown document). Note: there is a size limit of 40MB for a single
-file when using Google Drive links in this manner.
+This program takes a Google Drive sharing link for a file and repackages
+it into a link that can be downloaded directly (e.g. using curl) or
+embedded in a document to be viewed (e.g. an image in a markdown
+document). Note: there is a size limit of 40MB for a single file when
+using Google Drive links in this manner.
 
 optional arguments:
   -h, --help      show this help message and exit
-  -v, --view      repackage the link for viewing (e.g. as an embedded link in a markdown
-                  document).
-  -d, --download  repackage the link for downloading (e.g. downloading using curl).
+  -d, --download  The default behavior for glinkfix is to repackage a
+                  Google Drive link to make it suitable for embedding in
+                  a website. Use this option if you want to repackage
+                  Google Drive link for direct downloading (e.g.
+                  downloading using curl).
 ```
 
 ## Usage Notes
 
-* There is a 40MB size limit for a single file when using Google Drive sharing
-  links directly for viewing or downloading. Individual files larger than 40MB
-  will not render/download properly. This limit is a function of how Google
-  Drive works and is not related to `glinkfix`.
-* When creating a download link for use with `curl` make sure to use `curl`'s
-  `-L` option to allow for redirects.
-* `glinkfix` supports links that use Google's [resource
-  key](https://support.google.com/a/answer/10685032) security feature.
+* There is a 40MB size limit for a single file when using Google Drive
+  sharing links directly for viewing or downloading. Individual files
+  larger than 40MB will not render/download properly. This limit is a
+  function of how Google Drive works and is not related to `glinkfix`.
+* When creating a download link for use with `curl` make sure to use
+  `curl`'s `-L` option to allow for redirects.
+* `glinkfix` supports links that use Google's [resource key][def6]
+ security feature.
 
 ## Version History
 
-* 1.2.1 (2024-01-24)
-  * Version re-baseline and documentation corrections. No functional
-    changes in the 1.2.x release cycle.
-    <br><br>
-* 1.2.0 (2024-01-23)
-  * Updated installation options to include [pipx](https://pipx.pypa.io/stable/).
-  <br><br>
-* 1.0.16 (2023-12-31)
-  * Cleaned up packaging for better [PEP
-  561](https://peps.python.org/pep-0561/) compliance.
-  * Dropped support for Python <=3.7
-  <br><br>
-* 1.0.15 (2023-06-23)
-  * Migrated code formatter to *black*.
-  <br><br>
-* 1.0.14 (2023-04-19)
-  * Documentation cleanup.
-  <br><br>
-* 1.0.13 (2022-11-03)
-  * Google made a breaking change to the format for sharing links (not that
-    they checked with me first 😊). This patch updates glinkfix to support the
-    change.
-  <br><br>
-* 1.0.12 (2022-10-22)
-  * Regression bug fixes.
-  <br><br>
-* 1.0.11 (2022-10-21)
-  * Migrated dependency/build management to [poetry](https://python-poetry.org/).
-  <br><br>
-* 1.0.9 (2022-10-13)
-  * Fixed a bug when IDs or resource keys contain underscore characters (`_`)
-  * Additional test case for bug fix.
-  * Moved task runner to make.
-  * Build local virtual environment for development.
-  * Code refactoring and linting.
-  <br><br>
-* 1.0.8 (2022-07-23)
-  * Implemented code coverage for testing infrastructure.
-  * Code refactoring and linting.
-  <br><br>
-* 1.0.7 (2022-07-15)
-  * Fixed handling of URLs with resource keys.
-  * Code cleanup and refactoring.
-  * Implemented custom exception handling.
-  * Implemented testing infrastructure.<br><br>
-* 1.0.6 (2022-01-17)
-  * Code cleanup.<br><br>
-* 1.0.5 (2021-12-23)
-  * Code linting.
-  * Documentation cleanup.<br><br>
-* 1.0.4 (2021-12-19)
-  * Initial release<br>
+View releases on the [glinkfix git repository][def7]
 
+[def]: https://python-poetry.org/
+[def2]: https://docs.github.com/en/get-started/getting-started-with-git/ignoring-files
+[def3]: https://pipx.pypa.io/stable/
+[def6]: https://support.google.com/a/answer/10685032
+[def7]: https://github.com/geozeke/glinkfix
+[def8]: https://pyperclip.readthedocs.io/en/latest/index.html#not-implemented-error
+[def9]: https://pypi.org/project/pyperclip/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

