# Comparing `tmp/stow-1.3.1.tar.gz` & `tmp/stow-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stow-1.3.1.tar", last modified: Sun Jan 21 05:06:37 2024, max compression
+gzip compressed data, was "stow-1.4.0.tar", last modified: Tue Apr 23 10:42:57 2024, max compression
```

## Comparing `stow-1.3.1.tar` & `stow-1.4.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:37.028246 stow-1.3.1/
--rw-rw-rw-   0        0        0    10756 2023-03-26 22:44:13.000000 stow-1.3.1/LICENSE
--rw-rw-rw-   0        0        0    21093 2024-01-21 05:06:37.027240 stow-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-01-21 05:01:45.000000 stow-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:36.984149 stow-1.3.1/docs/
--rw-rw-rw-   0        0        0    19244 2023-08-04 17:54:30.000000 stow-1.3.1/docs/index.md
--rw-rw-rw-   0        0        0       86 2023-03-26 22:44:13.000000 stow-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0     1182 2024-01-21 05:06:37.033249 stow-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:36.992090 stow-1.3.1/stow/
--rw-rw-rw-   0        0        0     1894 2024-01-21 05:01:45.000000 stow-1.3.1/stow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:37.013127 stow-1.3.1/stow/artefacts/
--rw-rw-rw-   0        0        0       86 2024-01-21 05:01:45.000000 stow-1.3.1/stow/artefacts/__init__.py
--rw-rw-rw-   0        0        0    21539 2024-01-21 05:01:45.000000 stow-1.3.1/stow/artefacts/artefacts.py
--rw-rw-rw-   0        0        0     4902 2024-01-21 05:01:45.000000 stow-1.3.1/stow/artefacts/interfaces.py
--rw-rw-rw-   0        0        0      413 2024-01-21 05:01:45.000000 stow-1.3.1/stow/artefacts/types.py
--rw-rw-rw-   0        0        0     7821 2024-01-21 05:03:17.000000 stow-1.3.1/stow/callbacks.py
--rw-rw-rw-   0        0        0    12514 2024-01-21 05:03:17.000000 stow-1.3.1/stow/cli.py
--rw-rw-rw-   0        0        0      938 2024-01-21 05:01:45.000000 stow-1.3.1/stow/exceptions.py
--rw-rw-rw-   0        0        0      517 2024-01-21 05:01:45.000000 stow-1.3.1/stow/localiser.py
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:37.016127 stow-1.3.1/stow/manager/
--rw-rw-rw-   0        0        0       83 2023-03-26 22:44:13.000000 stow-1.3.1/stow/manager/__init__.py
--rw-rw-rw-   0        0        0    12796 2024-01-21 05:01:45.000000 stow-1.3.1/stow/manager/abstract_methods.py
--rw-rw-rw-   0        0        0     7335 2024-01-21 05:01:45.000000 stow-1.3.1/stow/manager/base_managers.py
--rw-rw-rw-   0        0        0    69657 2024-01-21 05:03:17.000000 stow-1.3.1/stow/manager/manager.py
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:37.021226 stow-1.3.1/stow/managers/
--rw-rw-rw-   0        0        0       26 2023-05-23 16:38:50.000000 stow-1.3.1/stow/managers/__init__.py
--rw-rw-rw-   0        0        0    46748 2024-01-21 05:03:17.000000 stow-1.3.1/stow/managers/amazon.py
--rw-rw-rw-   0        0        0    21345 2024-01-21 05:03:17.000000 stow-1.3.1/stow/managers/filesystem.py
--rw-rw-rw-   0        0        0    13549 2024-01-21 05:01:45.000000 stow-1.3.1/stow/managers/kubernetes.py
--rw-rw-rw-   0        0        0    14458 2024-01-21 05:01:45.000000 stow-1.3.1/stow/managers/ssh.py
--rw-rw-rw-   0        0        0     1050 2024-01-21 05:01:45.000000 stow-1.3.1/stow/storage_classes.py
--rw-rw-rw-   0        0        0      411 2024-01-21 05:01:45.000000 stow-1.3.1/stow/types.py
--rw-rw-rw-   0        0        0     3181 2024-01-21 05:01:45.000000 stow-1.3.1/stow/utils.py
--rw-rw-rw-   0        0        0     4155 2024-01-21 05:03:17.000000 stow-1.3.1/stow/worker_config.py
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:37.025222 stow-1.3.1/stow.egg-info/
--rw-rw-rw-   0        0        0    21093 2024-01-21 05:06:36.000000 stow-1.3.1/stow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      817 2024-01-21 05:06:36.000000 stow-1.3.1/stow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-21 05:06:36.000000 stow-1.3.1/stow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2024-01-21 05:06:36.000000 stow-1.3.1/stow.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      243 2024-01-21 05:06:36.000000 stow-1.3.1/stow.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-01-21 05:06:36.000000 stow-1.3.1/stow.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-21 05:06:37.024225 stow-1.3.1/tests/
--rw-rw-rw-   0        0        0     1959 2024-01-21 05:01:45.000000 stow-1.3.1/tests/test_callbacks.py
--rw-rw-rw-   0        0        0    11244 2024-01-21 05:01:45.000000 stow-1.3.1/tests/test_cli.py
--rw-rw-rw-   0        0        0    34145 2024-01-21 05:01:45.000000 stow-1.3.1/tests/test_stateless.py
--rw-rw-rw-   0        0        0     2798 2024-01-21 05:01:45.000000 stow-1.3.1/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.880548 stow-1.4.0/
+-rw-rw-rw-   0        0        0    10756 2023-03-26 22:44:13.000000 stow-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0    21448 2024-04-23 10:42:57.880548 stow-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-01-21 14:29:30.000000 stow-1.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.827375 stow-1.4.0/docs/
+-rw-rw-rw-   0        0        0    19244 2023-08-04 17:54:30.000000 stow-1.4.0/docs/index.md
+-rw-rw-rw-   0        0        0       86 2023-03-26 22:44:13.000000 stow-1.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1382 2024-04-23 10:42:57.886399 stow-1.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.837733 stow-1.4.0/stow/
+-rw-rw-rw-   0        0        0     2022 2024-04-23 10:42:04.000000 stow-1.4.0/stow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.860715 stow-1.4.0/stow/artefacts/
+-rw-rw-rw-   0        0        0       86 2024-01-21 14:29:30.000000 stow-1.4.0/stow/artefacts/__init__.py
+-rw-rw-rw-   0        0        0    22235 2024-04-23 10:42:04.000000 stow-1.4.0/stow/artefacts/artefacts.py
+-rw-rw-rw-   0        0        0     5221 2024-04-23 10:42:04.000000 stow-1.4.0/stow/artefacts/interfaces.py
+-rw-rw-rw-   0        0        0      413 2024-01-21 14:29:30.000000 stow-1.4.0/stow/artefacts/types.py
+-rw-rw-rw-   0        0        0     7895 2024-04-23 10:42:04.000000 stow-1.4.0/stow/callbacks.py
+-rw-rw-rw-   0        0        0    12517 2024-04-23 10:42:04.000000 stow-1.4.0/stow/cli.py
+-rw-rw-rw-   0        0        0      938 2024-01-21 14:29:30.000000 stow-1.4.0/stow/exceptions.py
+-rw-rw-rw-   0        0        0      517 2024-01-21 14:29:30.000000 stow-1.4.0/stow/localiser.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.866034 stow-1.4.0/stow/manager/
+-rw-rw-rw-   0        0        0      130 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/__init__.py
+-rw-rw-rw-   0        0        0    15058 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/abstract_methods.py
+-rw-rw-rw-   0        0        0     7335 2024-01-21 14:29:30.000000 stow-1.4.0/stow/manager/base_managers.py
+-rw-rw-rw-   0        0        0      290 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/configs.py
+-rw-rw-rw-   0        0        0    70711 2024-04-23 10:42:04.000000 stow-1.4.0/stow/manager/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.872093 stow-1.4.0/stow/managers/
+-rw-rw-rw-   0        0        0       26 2023-05-23 16:38:50.000000 stow-1.4.0/stow/managers/__init__.py
+-rw-rw-rw-   0        0        0    52725 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/amazon.py
+-rw-rw-rw-   0        0        0    21754 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/filesystem.py
+-rw-rw-rw-   0        0        0     1775 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/google.py
+-rw-rw-rw-   0        0        0    23022 2024-04-23 10:42:04.000000 stow-1.4.0/stow/managers/kubernetes.py
+-rw-rw-rw-   0        0        0    14458 2024-01-21 14:29:30.000000 stow-1.4.0/stow/managers/ssh.py
+-rw-rw-rw-   0        0        0     1050 2024-01-21 14:29:30.000000 stow-1.4.0/stow/storage_classes.py
+-rw-rw-rw-   0        0        0      411 2024-01-21 14:29:30.000000 stow-1.4.0/stow/types.py
+-rw-rw-rw-   0        0        0     3181 2024-01-21 14:29:30.000000 stow-1.4.0/stow/utils.py
+-rw-rw-rw-   0        0        0     4723 2024-04-23 10:42:04.000000 stow-1.4.0/stow/worker_config.py
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.878042 stow-1.4.0/stow.egg-info/
+-rw-rw-rw-   0        0        0    21448 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      865 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      386 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-23 10:42:57.000000 stow-1.4.0/stow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-23 10:42:57.876774 stow-1.4.0/tests/
+-rw-rw-rw-   0        0        0     1959 2024-01-21 14:29:30.000000 stow-1.4.0/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0    11244 2024-01-22 18:56:13.000000 stow-1.4.0/tests/test_cli.py
+-rw-rw-rw-   0        0        0    34145 2024-01-22 18:55:59.000000 stow-1.4.0/tests/test_stateless.py
+-rw-rw-rw-   0        0        0     2798 2024-01-21 14:29:30.000000 stow-1.4.0/tests/test_utils.py
```

### Comparing `stow-1.3.1/LICENSE` & `stow-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/PKG-INFO` & `stow-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stow
-Version: 1.3.1
+Version: 1.4.0
 Summary: stow artefacts anywhere, with ease
 Author: Kieran Bacon
 Author-email: kieran.bacon@outlook.com
 Project-URL: Homepage, https://github.com/Kieran-Bacon/stow
 Project-URL: Documentation, https://stow.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/Kieran-Bacon/stow/issues
 Keywords: aws s3 boto3 ssh os
@@ -15,19 +15,26 @@
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: typing_extensions
 Provides-Extra: all
 Requires-Dist: boto3; extra == "all"
 Requires-Dist: click; extra == "all"
 Requires-Dist: click-option-group; extra == "all"
-Provides-Extra: s3
-Requires-Dist: boto3; extra == "s3"
+Requires-Dist: google-api-python-client; extra == "all"
+Requires-Dist: google-auth-httplib2; extra == "all"
+Requires-Dist: google-auth-oauthlib; extra == "all"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 Requires-Dist: click-option-group; extra == "cli"
+Provides-Extra: s3
+Requires-Dist: boto3; extra == "s3"
+Provides-Extra: drive
+Requires-Dist: google-api-python-client; extra == "drive"
+Requires-Dist: google-auth-httplib2; extra == "drive"
+Requires-Dist: google-auth-oauthlib; extra == "drive"
 Provides-Extra: test
 Requires-Dist: pyini; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: moto[s3]>=4.1.5.dev40; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: mkdocstrings[python]==0.22.0; extra == "test"
```

### Comparing `stow-1.3.1/docs/index.md` & `stow-1.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/setup.cfg` & `stow-1.4.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 746f 770d 0a76 6572 7369 6f6e   = stow..version
-00000020: 203d 2031 2e33 2e31 0d0a 6175 7468 6f72   = 1.3.1..author
+00000020: 203d 2031 2e34 2e30 0d0a 6175 7468 6f72   = 1.4.0..author
 00000030: 203d 204b 6965 7261 6e20 4261 636f 6e0d   = Kieran Bacon.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6b69 6572 616e 2e62 6163 6f6e 406f 7574  kieran.bacon@out
 00000060: 6c6f 6f6b 2e63 6f6d 0d0a 6465 7363 7269  look.com..descri
 00000070: 7074 696f 6e20 3d20 7374 6f77 2061 7274  ption = stow art
 00000080: 6566 6163 7473 2061 6e79 7768 6572 652c  efacts anywhere,
 00000090: 2077 6974 6820 6561 7365 0d0a 6c6f 6e67   with ease..long
@@ -43,32 +43,45 @@
 000002a0: 6578 7465 6e73 696f 6e73 0d0a 7061 636b  extensions..pack
 000002b0: 6167 655f 6469 7220 3d20 0d0a 0973 746f  age_dir = ...sto
 000002c0: 7720 3d20 7374 6f77 0d0a 0d0a 5b6f 7074  w = stow....[opt
 000002d0: 696f 6e73 2e65 7874 7261 735f 7265 7175  ions.extras_requ
 000002e0: 6972 655d 0d0a 616c 6c20 3d20 0d0a 0962  ire]..all = ...b
 000002f0: 6f74 6f33 0d0a 0963 6c69 636b 0d0a 0963  oto3...click...c
 00000300: 6c69 636b 2d6f 7074 696f 6e2d 6772 6f75  lick-option-grou
-00000310: 700d 0a73 3320 3d20 0d0a 0962 6f74 6f33  p..s3 = ...boto3
-00000320: 0d0a 636c 6920 3d20 0d0a 0963 6c69 636b  ..cli = ...click
-00000330: 0d0a 0963 6c69 636b 2d6f 7074 696f 6e2d  ...click-option-
-00000340: 6772 6f75 700d 0a74 6573 7420 3d20 0d0a  group..test = ..
-00000350: 0970 7969 6e69 0d0a 0970 7974 6573 740d  .pyini...pytest.
-00000360: 0a09 7079 7465 7374 2d63 6f76 0d0a 096d  ..pytest-cov...m
-00000370: 6f74 6f5b 7333 5d3e 3d34 2e31 2e35 2e64  oto[s3]>=4.1.5.d
-00000380: 6576 3430 0d0a 096d 6b64 6f63 730d 0a09  ev40...mkdocs...
-00000390: 6d6b 646f 6373 7472 696e 6773 5b70 7974  mkdocstrings[pyt
-000003a0: 686f 6e5d 3d3d 302e 3232 2e30 0d0a 0963  hon]==0.22.0...c
-000003b0: 6c69 636b 0d0a 0963 6c69 636b 2d6f 7074  lick...click-opt
-000003c0: 696f 6e2d 6772 6f75 700d 0a09 626f 746f  ion-group...boto
-000003d0: 332d 7374 7562 735b 7333 5d0d 0a09 6372  3-stubs[s3]...cr
-000003e0: 6333 3263 0d0a 0d0a 5b6f 7074 696f 6e73  c32c....[options
-000003f0: 2e65 6e74 7279 5f70 6f69 6e74 735d 0d0a  .entry_points]..
-00000400: 636f 6e73 6f6c 655f 7363 7269 7074 7320  console_scripts 
-00000410: 3d20 7374 6f77 3d73 746f 772e 636c 693a  = stow=stow.cli:
-00000420: 636c 690d 0a73 746f 775f 6d61 6e61 6765  cli..stow_manage
-00000430: 7273 203d 200d 0a09 6673 203d 2073 746f  rs = ...fs = sto
-00000440: 772e 6d61 6e61 6765 7273 3a46 530d 0a09  w.managers:FS...
-00000450: 7333 203d 2073 746f 772e 6d61 6e61 6765  s3 = stow.manage
-00000460: 7273 2e61 6d61 7a6f 6e3a 416d 617a 6f6e  rs.amazon:Amazon
-00000470: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000480: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000490: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000310: 700d 0a09 676f 6f67 6c65 2d61 7069 2d70  p...google-api-p
+00000320: 7974 686f 6e2d 636c 6965 6e74 0d0a 0967  ython-client...g
+00000330: 6f6f 676c 652d 6175 7468 2d68 7474 706c  oogle-auth-httpl
+00000340: 6962 320d 0a09 676f 6f67 6c65 2d61 7574  ib2...google-aut
+00000350: 682d 6f61 7574 686c 6962 0d0a 636c 6920  h-oauthlib..cli 
+00000360: 3d20 0d0a 0963 6c69 636b 0d0a 0963 6c69  = ...click...cli
+00000370: 636b 2d6f 7074 696f 6e2d 6772 6f75 700d  ck-option-group.
+00000380: 0a73 3320 3d20 0d0a 0962 6f74 6f33 0d0a  .s3 = ...boto3..
+00000390: 6472 6976 6520 3d20 0d0a 0967 6f6f 676c  drive = ...googl
+000003a0: 652d 6170 692d 7079 7468 6f6e 2d63 6c69  e-api-python-cli
+000003b0: 656e 740d 0a09 676f 6f67 6c65 2d61 7574  ent...google-aut
+000003c0: 682d 6874 7470 6c69 6232 0d0a 0967 6f6f  h-httplib2...goo
+000003d0: 676c 652d 6175 7468 2d6f 6175 7468 6c69  gle-auth-oauthli
+000003e0: 620d 0a74 6573 7420 3d20 0d0a 0970 7969  b..test = ...pyi
+000003f0: 6e69 0d0a 0970 7974 6573 740d 0a09 7079  ni...pytest...py
+00000400: 7465 7374 2d63 6f76 0d0a 096d 6f74 6f5b  test-cov...moto[
+00000410: 7333 5d3e 3d34 2e31 2e35 2e64 6576 3430  s3]>=4.1.5.dev40
+00000420: 0d0a 096d 6b64 6f63 730d 0a09 6d6b 646f  ...mkdocs...mkdo
+00000430: 6373 7472 696e 6773 5b70 7974 686f 6e5d  cstrings[python]
+00000440: 3d3d 302e 3232 2e30 0d0a 0963 6c69 636b  ==0.22.0...click
+00000450: 0d0a 0963 6c69 636b 2d6f 7074 696f 6e2d  ...click-option-
+00000460: 6772 6f75 700d 0a09 626f 746f 332d 7374  group...boto3-st
+00000470: 7562 735b 7333 5d0d 0a09 6372 6333 3263  ubs[s3]...crc32c
+00000480: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
+00000490: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
+000004a0: 6f6c 655f 7363 7269 7074 7320 3d20 7374  ole_scripts = st
+000004b0: 6f77 3d73 746f 772e 636c 693a 636c 690d  ow=stow.cli:cli.
+000004c0: 0a73 746f 775f 6d61 6e61 6765 7273 203d  .stow_managers =
+000004d0: 200d 0a09 6673 203d 2073 746f 772e 6d61   ...fs = stow.ma
+000004e0: 6e61 6765 7273 3a46 530d 0a09 7333 203d  nagers:FS...s3 =
+000004f0: 2073 746f 772e 6d61 6e61 6765 7273 2e61   stow.managers.a
+00000500: 6d61 7a6f 6e3a 416d 617a 6f6e 0d0a 096b  mazon:Amazon...k
+00000510: 3873 203d 2073 746f 772e 6d61 6e61 6765  8s = stow.manage
+00000520: 7273 2e6b 7562 6572 6e65 7465 733a 4b75  rs.kubernetes:Ku
+00000530: 6265 726e 6574 6573 0d0a 0d0a 5b65 6767  bernetes....[egg
+00000540: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000550: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000560: 2030 0d0a 0d0a                            0....
```

### Comparing `stow-1.3.1/stow/__init__.py` & `stow-1.4.0/stow/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -50,14 +50,18 @@
 islink = Manager.islink
 ismount = Manager.ismount
 getctime = Manager.getctime
 getmtime = Manager.getmtime
 setmtime = Manager.setmtime
 getatime = Manager.getatime
 setatime = Manager.setatime
+get_tags = Manager.get_tags
+set_tags = Manager.set_tags
+get_metadata = Manager.get_metadata
+set_metadata = Manager.set_metadata
 set_artefact_time = Manager.set_artefact_time
 exists = Manager.exists
 lexists = Manager.lexists
 touch = Manager.touch
 mkdir = Manager.mkdir
 mklink = Manager.mklink
 localise = Manager.localise
```

### Comparing `stow-1.3.1/stow/artefacts/artefacts.py` & `stow-1.4.0/stow/artefacts/artefacts.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,20 +70,35 @@
 
     @property
     def directory(self) -> 'Directory':
         """ Directory object this artefact exists within """
         return self._manager.artefact(self._manager.dirname(self._path), type=Directory)
 
     @property
+    def tags(self):
+        """ Get accessible file metadata as hosted by the manager """
+        if self._tags is None:
+            self._tags = self._manager.get_tags(self)
+        return self._tags
+
+    @tags.setter
+    def tags(self, metadata: Dict[str, str]):
+        self._tags = self._manager.set_tags(self, metadata)
+
+    @property
     def metadata(self):
         """ Get accessible file metadata as hosted by the manager """
         if self._metadata is None:
-            self._metadata = self._manager._metadata(self._path)
+            self._metadata = self._manager.get_metadata(self)
         return self._metadata
 
+    @metadata.setter
+    def metadata(self, metadata: Dict[str, str]):
+        self._metadata = self._manager.set_metadata(self, metadata)
+
     @property
     def createdTime(self) -> datetime.datetime:
         """ UTC localised datetime of time file last modified by a write/append method """
         return self._createdTime or self.modifiedTime
 
     @property
     def modifiedTime(self) -> datetime.datetime:
@@ -159,24 +174,30 @@
             overwrite=force,
             callback=callback,
             modified_time=modified_time,
             accessed_time=accessed_time,
             worker_config=worker_config
         )
 
-    def delete(self, force: bool = False):
+    def delete(
+            self,
+            force: bool = False,
+            *,
+            worker_config: Optional[WorkerPoolConfig] = None,
+            callback: AbstractCallback = DefaultCallback()
+        ):
         """ Delete this artefact from the disk
 
         Args:
             force: An "are you sure" for directories
 
         Raises:
             OperationNotPermitted: If directory and deletion has not been deleted
         """
-        self._manager.rm(self, recursive=force)
+        self._manager.rm(self, recursive=force, callback=callback, worker_config=worker_config)
 
 class File(Artefact):
     """ A filesystem file object - a container of bytes representing some data
 
     Args:
         manager: The submanager this file belongs to
         path: The file's relative path
```

### Comparing `stow-1.3.1/stow/artefacts/interfaces.py` & `stow-1.4.0/stow/artefacts/interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import abc
 import typing
-from typing import (IO, Any, Union, Optional, Literal, Dict, Tuple, Generator, overload)
+from typing import (IO, Any, Union, Optional, Literal, Dict, Tuple, Generator, overload, Type)
 import datetime
 
 from ..storage_classes import StorageClassInterface
 from ..worker_config import WorkerPoolConfig
 from ..callbacks import AbstractCallback, DefaultCallback
 from ..types import StrOrPathLike, TimestampLike, HashingAlgorithm
 from ..localiser import Localiser
@@ -21,33 +21,43 @@
     def __getitem__(self, key: StrOrPathLike) -> Any:
         pass
 
     @abc.abstractmethod
     def _abspath(self, path: StrOrPathLike) -> str:
         pass
 
-    def _metadata(self, path: str) -> Dict[str, Any]:
-        ...
 
     def _get_content_type(self, path: str) -> str:
         ...
 
     def _set_content_type(self, path: str, content_type: str):
         ...
 
     def _isMount(self, artefact) -> bool:
         ...
 
     def _isLink(self, artefact) -> bool:
         ...
 
-    def _rm(self, path: StrOrPathLike, *, callback: AbstractCallback):
+    def _rm(self, path: StrOrPathLike, *, callback: AbstractCallback = DefaultCallback(), worker_config: Optional[WorkerPoolConfig] = None):
+        ...
+
+    def get_tags(self, artefact: os.PathLike) -> Dict[str, Any]:
+        ...
+
+    def set_tags(self, artefact: os.PathLike, metadata: Dict[str, str]):
+        ...
+
+    def get_metadata(self, artefact: os.PathLike) -> Dict[str, Any]:
+        ...
+
+    def set_metadata(self, artefact: os.PathLike, metadata: Dict[str, str]):
         ...
 
-    def artefact(self, artefact: StrOrPathLike, type: Optional[os.PathLike[str]] = None) -> os.PathLike[str]:
+    def artefact(self, artefact: StrOrPathLike, type: Type[Artefact]) -> Artefact:
         ...
 
     def exists(self, artefact) -> bool:
         ...
 
     @abc.abstractmethod
     def basename(self, path: StrOrPathLike) -> str:
```

### Comparing `stow-1.3.1/stow/callbacks.py` & `stow-1.4.0/stow/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import abc
 import typing
-from typing import Union, Optional, Tuple, Any
+from typing import Union, Optional, Tuple, Any, Callable
 
 import tqdm
 import tqdm.notebook
 import queue
 
 import logging
 log = logging.getLogger(__name__)
@@ -40,15 +40,15 @@
         ...
 
     @abc.abstractmethod
     def deleted(self, pathOrCount: Union[str, int]):
         ...
 
     @abc.abstractmethod
-    def get_bytes_transfer(self, path: str, bytes: int):
+    def get_bytes_transfer(self, path: str, bytes: Optional[int] = None) -> Callable[[int], None]:
         pass
 
 class NoneImplementedCallback(AbstractCallback):
     def reviewing(self, count: int): return super().reviewing(count)
     def reviewed(self, pathOrCount: Union[str,int]): return super().reviewed(pathOrCount)
     def writing(self, count: int): return super().writing(count)
     def written(self, pathOrCount: Union[str, int]): return super().written(pathOrCount)
@@ -177,15 +177,15 @@
         for i, unit in enumerate(("", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi", "Yi")):
             if abs(num) < 1024.0:
                 return 1024.0**i, num, unit + suffix
             num /= 1024.0
         else:
             raise RuntimeError('File size exceeds all of human data to this point - so probs a problem')
 
-    def get_bytes_transfer(self, path, total_bytes_transfer):
+    def get_bytes_transfer(self, path, total_bytes_transfer: Optional[int] = None):
         log.debug('Initialising transfer for path=%s', path)
 
         if self._notebook:
             return lambda *args, **kwargs: None
 
         # divisor, total, unit = self.sizeof_fmt(total_bytes_transfer)
         divisor = 1
```

### Comparing `stow-1.3.1/stow/cli.py` & `stow-1.4.0/stow/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import click
 from click_option_group import optgroup
 
-import dataclasses
 import logging
 import pkg_resources
 from typing import Tuple, Optional, List
 
 from .manager import Manager
 from .artefacts import File, Directory
 from .types import HashingAlgorithm
-from .callbacks import AbstractCallback, DefaultCallback, ProgressCallback
+from .callbacks import DefaultCallback, ProgressCallback
 
 log = logging.getLogger(__name__)
 
 # Build the initial stow cli options from loaded managers
 managerConfigs = {}
 managerOptions = []
 for entry_point in pkg_resources.iter_entry_points('stow_managers'):
@@ -26,40 +25,37 @@
 
     except:
         # The Manager is not installed or cannot be loaded
         log.warning('Manager %s could not be loaded', entry_point.name)
         continue
 
     managerConfigs[entry_point.name] = config
-    managerOptions.append(
-        optgroup.group(
-            f'{entryManager.__name__} configuration',
-            help=f'Options for the {entryManager.__name__} manager'
+    arguments = config.arguments()
+    if arguments:
+        managerOptions.append(
+            optgroup.group(
+                f'{entryManager.__name__} configuration',
+                help=f'Options for the {entryManager.__name__} manager'
+            )
         )
-    )
-    for args, kwargs in config.arguments():
-        managerOptions.append(optgroup.option(*args, **kwargs))
+        for args, kwargs in arguments:
+            managerOptions.append(optgroup.option(*args, **kwargs))
 
 cli_decorators = [
     click.option(
         '-m', '--manager',
         type=click.Choice(['auto', *managerConfigs.keys()], case_sensitive=False),
         default='auto',
         help='Select the manager you are connecting to - by default the manager will be guessed from the protocol'
     ),
     *managerOptions,
     click.option('--debug/--no-debug', default=False),
     click.pass_context
 ]
 
-@dataclasses.dataclass
-class StowContext:
-    manager: Manager
-    callback: AbstractCallback
-
 def dynamicDecorators(cli_decorators):
     def wraps(func):
         for decorator in cli_decorators[::-1]:
             func = decorator(func)
         return func
     return wraps
 
@@ -228,18 +224,20 @@
         type_ = None
 
     if count:
         artefactObj = manager.artefact(artefact, type=Directory)
         print(f"{artefactObj.path} - Count: {len(manager.ls(artefactObj, recursive=recursive, ignore_missing=True))}")
 
     else:
+        source = manager.artefact(artefact, type=Directory)
+
         print()
         print('Name'.ljust(70)+'|Type'.ljust(10)+' |Creation Date')
         print('='*114)
-        for subArtefacts in manager.iterls(artefact, recursive=recursive, ignore_missing=True):
+        for subArtefacts in manager.iterls(source, recursive=recursive, ignore_missing=True):
             if type_ is not None and not isinstance(subArtefacts, type_):
                 continue
             print(f"{subArtefacts.path.ljust(70)} {subArtefacts.__class__.__name__.ljust(10)} {subArtefacts.modifiedTime}")
         print()
 
 
 @cli.command()
```

### Comparing `stow-1.3.1/stow/exceptions.py` & `stow-1.4.0/stow/exceptions.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/stow/localiser.py` & `stow-1.4.0/stow/localiser.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/stow/manager/abstract_methods.py` & `stow-1.4.0/stow/manager/abstract_methods.py`

 * *Files 20% similar despite different names*

```diff
@@ -73,14 +73,66 @@
 
         Returns:
             typing.Union[Artefact, None]: The artefact object that represents the item on disk or None if nothing exists
         """
         pass
 
     @abstractmethod
+    def _get_tags(self, artefact: ArtefactType) -> Dict[str, str]:
+        """ Fetch artefact tags
+
+        Args:
+            artefact (ArtefactType): The artefact to fetch the tags from
+
+        Returns:
+            Dict[str, str]: A dict of the artefact tags
+        """
+        raise NotImplementedError(f'Manager {self.__class__} does not support tags')
+
+    @abstractmethod
+    def _set_tags(self, artefact: ArtefactType, metadata: Metadata) -> Dict[str, str]:
+        """ Write the metadata provided as tags to the artefact specified
+
+        Args:
+            artefact (ArtefactType): The artefact the metadata is to be written onto as tags - must exist
+            metadata (Metadata): The metadata being written
+
+        Returns:
+            Dict[str, str]: Returns the metadata that is now set on the artefact - equal to value returned from `get_metadata`
+                it may differ from the metadata provided as managers have required and self managered metadata fields
+        """
+        raise NotImplementedError(f'Manager {self.__class__} does not support setting metadata')
+
+    @abstractmethod
+    def _get_metadata(self, artefact: ArtefactType) -> Dict[str, str]:
+        """ Fetch artefact metadata
+
+        Args:
+            path (str): The manager relative path to the artefact
+
+        Returns:
+            Dict[str, str]: A dict of the metadata key values
+        """
+        raise NotImplementedError(f'Manager {self.__class__} does not support metadata')
+
+    @abstractmethod
+    def _set_metadata(self, artefact: ArtefactType, metadata: Metadata) -> Dict[str, str]:
+        """ Write the metadata provided to the artefact specified
+
+        Args:
+            artefact (ArtefactType): The artefact the metadata is to be written onto - must exist
+            metadata (Metadata): The metadata being written
+
+        Returns:
+            Dict[str, str]: Returns the metadata that is now set on the artefact - equal to value returned from _get_metadata
+                it may differ from the metadata provided as managers have required and self managered metadata fields
+        """
+        raise NotImplementedError(f'Manager {self.__class__} does not support setting metadata')
+
+    @abstractmethod
     def _isLink(self, file: str) -> bool:
         """ Check if the file object given is a link/shortcut to another file """
         pass
 
     @abstractmethod
     def _isMount(self, directory: str) -> bool:
         """ Check if the file object given is a mount point """
@@ -136,14 +188,15 @@
         callback: AbstractCallback,
         metadata: Optional[Metadata],
         modified_time: Optional[TimestampLike],
         accessed_time: Optional[TimestampLike],
         content_type: Optional[str],
         storage_class: Optional[StorageClass],
         worker_config: WorkerPoolConfig,
+        delete_source: bool = False
         ) -> ArtefactType:
         """ Put the local filesystem object onto the underlying manager implementation using the absolute paths given.
 
         To avoid user error - an artefact cannot be placed onto a Directory unless an overwrite toggle has been passed
         which is False by default. This should protect them from accidentally deleting a directory.
 
         In the event that they want to do so - the deletion of the directory will be handled before operating this
```

### Comparing `stow-1.3.1/stow/manager/base_managers.py` & `stow-1.4.0/stow/manager/base_managers.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/stow/manager/manager.py` & `stow-1.4.0/stow/manager/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -706,14 +706,44 @@
         modified_datetime: Optional[TimestampLike] = None,
         accessed_datetime: Optional[TimestampLike] = None
         ) -> Tuple[datetime.datetime, datetime.datetime]:
         """ Update the artefacts access time """
         manager, artefact, _ = self._splitArtefactForm(artefact, require=True, external=False)
         return manager._set_artefact_time(artefact, modified_datetime, accessed_datetime)
 
+    def get_tags(
+            self,
+            artefact: ArtefactOrPathLike
+        ) -> Dict[str, str]:
+        manager, artefact, _ = self._splitArtefactForm(artefact, load=False, require=True, external=False)
+        return manager._get_tags(artefact)
+
+    def set_tags(
+            self,
+            artefact: ArtefactOrPathLike,
+            metadata: Metadata
+        ) -> Dict[str, str]:
+        manager, artefact, _ = self._splitArtefactForm(artefact, load=False, require=True, external=False)
+        return manager._set_tags(artefact, metadata)
+
+    def get_metadata(
+            self,
+            artefact: ArtefactOrPathLike
+        ) -> Dict[str, str]:
+        manager, artefact, _ = self._splitArtefactForm(artefact, load=False, require=True, external=False)
+        return manager._get_metadata(artefact)
+
+    def set_metadata(
+            self,
+            artefact: ArtefactOrPathLike,
+            metadata: Metadata
+        ) -> Dict[str, str]:
+        manager, artefact, _ = self._splitArtefactForm(artefact, load=False, require=True, external=False)
+        return manager._set_metadata(artefact, metadata)
+
     def exists(self, *artefacts: ArtefactOrPathLike) -> bool:
         """ Return true if the given artefact is a member of the manager, or the path is correct for the manager and it
         leads to a File or Directory.
 
         Does not handle protocols
 
         Args:
@@ -1033,15 +1063,15 @@
                     callback=callback,
                     modified_time=utils.timestampToFloatOrNone(modified_time),
                     accessed_time=utils.timestampToFloatOrNone(accessed_time),
                     worker_config=worker_config
                 )
 
                 # Load the downloaded artefact from the local location and return
-                gottenArtefact = PartialArtefact(self.connect(manager="FS"), destination)
+                gottenArtefact = PartialArtefact(self.connect(manager="FS"), destinationAbspath)
 
             else:
                 if not isinstance(obj, File):
                     raise exceptions.ArtefactTypeError("Cannot get file bytes of {}".format(obj))
                 gottenArtefact = manager._getBytes(obj, callback=callback)
 
             return gottenArtefact
@@ -1346,27 +1376,26 @@
                     content_type=content_type,
                     worker_config=worker_config or WorkerPoolConfig(shutdown=True),
                 )
 
             else:
 
                 # Moving between manager types - put the object and then delete the old one
-                movedArtefact = self.put(
+                movedArtefact = destinationManager._put(
                     sourceObj,
-                    destination,
-                    overwrite=overwrite,
+                    destinationPath,
                     callback=callback,
                     metadata=metadata,
                     modified_time=utils.timestampToFloatOrNone(modified_time),
                     accessed_time=utils.timestampToFloatOrNone(accessed_time),
                     storage_class=storage_class,
                     worker_config=worker_config,
                     content_type=content_type,
+                    delete_source=True
                 )
-                sourceManager._rm(sourceObj.path, callback=callback, worker_config=worker_config)
 
             return movedArtefact
 
         finally:
             worker_config.conclude()
 
     def rm(
```

### Comparing `stow-1.3.1/stow/managers/amazon.py` & `stow-1.4.0/stow/managers/amazon.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import boto3.exceptions
 from botocore.exceptions import ClientError, UnauthorizedSSOTokenError
 
 from .. import utils as utils
 from ..worker_config import WorkerPoolConfig
 from ..types import HashingAlgorithm
 from ..artefacts import Artefact, PartialArtefact, File, Directory, ArtefactType, Metadata, ArtefactOrPathLike, ArtefactOrStr
-from ..manager import RemoteManager
+from ..manager import RemoteManager, AbstractCommandLineConfig
 from ..storage_classes import StorageClass, StorageClassInterface
 from ..callbacks import AbstractCallback
 from .. import exceptions
 
 log = logging.getLogger(__name__)
 
 def calculateBytesS3ETag(bytes_readable: typing.BinaryIO) -> str:
@@ -84,14 +84,36 @@
         else:
             with f.open('rb') as handle:
                 digests.append(calculateBytesS3ETag(handle))
 
     return all(digests[0] == d for d in digests[1:])
 
 @dataclasses.dataclass
+class DeleteRoot:
+    root: Artefact
+    worker_config: WorkerPoolConfig
+    callback: AbstractCallback
+
+    count: int = 0
+    size: int = 0
+
+    def trigger_delete(self):
+        """ Start the delete process on the source object """
+        # TODO review - going directly avoids having to check the source again
+        # self.root.delete(force=True, callback=callback)
+        self.root._manager._rm(self.root.path, callback=self.callback, worker_config=self.worker_config)
+
+    def finish_task(self):
+        """ Finish a required task before the delete process - increment the count and delete the source if final task
+        """
+        self.count += 1
+        if self.count == self.size:
+            self.trigger_delete()
+
+@dataclasses.dataclass
 class DirStat:
     bucket: Optional[str]
     path: str
     keys: List[str] = dataclasses.field(default_factory=list)
     files: List[File] = dataclasses.field(default_factory=list)
     directory_keys: List[str] = dataclasses.field(default_factory=list)
     directories: List[Directory] = dataclasses.field(default_factory=list)
@@ -107,15 +129,15 @@
     ONEZONE_IA = 'ONEZONE_IA'
     INTELLIGENT_TIERING = 'INTELLIGENT_TIERING'
     GLACIER = 'GLACIER'
     DEEP_ARCHIVE = 'DEEP_ARCHIVE'
     OUTPOSTS = 'OUTPOSTS'
 
     @classmethod
-    def toGeneric(cls, value) -> StorageClass:
+    def toGeneric(cls, value: Self) -> StorageClass:
         value = cls(value)
         if value is cls.STANDARD:
             return StorageClass.STANDARD
         elif value is cls.REDUCED_REDUNDANCY:
             return StorageClass.REDUCED_REDUNDANCY
         elif value in (cls.STANDARD_IA, cls.ONEZONE_IA):
             return StorageClass.INFREQUENT_ACCESS
@@ -271,29 +293,41 @@
         """ Check whether a bucket is accessible - creating it if it doesn't exists and raising errors if a permission
         issues exists
 
         Returns:
             bool: True if the bucket was created - False if it exists and we have permissions to it
         """
         try:
-            self._s3.head_bucket(Bucket=bucket)
+            self._s3.head_bucket(
+                Bucket=bucket
+            )
 
         except ClientError as e:
             status_code = e.response['ResponseMetadata']['HTTPStatusCode']
 
             if status_code == 404:
                 # We can create the bucket as it doesn't exist currently
-                log.warning('Creating s3 bucket=[%s] as it does not already exist and is available')
-                self._s3.create_bucket(Bucket=bucket)
+                log.warning('Creating s3 bucket=[%s] as it does not already exist and is available', bucket)
+                try:
+                    self._s3.create_bucket(
+                        Bucket=bucket,
+                        CreateBucketConfiguration={
+                            'LocationConstraint': self._aws_session.region_name
+                        }
+                    )
+                except:
+                    log.exception("Failed to create bucket [%s]", bucket)
+                    raise
                 return True
 
             elif status_code == 403:
                 # Bucket already exists and cannot be written too
-                raise exceptions.OperationNotPermitted('You do not have permissions to access s3 bucket [%s]') from e
+                raise exceptions.OperationNotPermitted(f'You do not have permissions to access s3 bucket [{bucket}]') from e
 
+            log.exception('Unexpected client error when trying to check connection to [%s] bucket', bucket)
             raise
         return False
 
     def _abspath(self, managerPath: str) -> str:
 
         bucket, path = self._pathComponents(managerPath)
 
@@ -332,14 +366,17 @@
     @overload
     def _pathComponents(self, artefact: ArtefactOrStr, optional: Literal[False]) -> Tuple[str, str]:
         ...
     @overload
     def _pathComponents(self, artefact: ArtefactOrStr, optional: Literal[True] = True) -> Tuple[Optional[str], str]:
         ...
     def _pathComponents(self, artefact: ArtefactOrStr, optional: bool = True) -> Tuple[Optional[str], str]:
+        """ Extract from the artefact provided, the bucket and key of the artefact for s3.
+
+        """
 
         artefactPath = artefact.path if isinstance(artefact, Artefact) else artefact
 
         path = self.join(self._path, self._validatePath(artefactPath), joinAbsolutes=True).lstrip('/')
 
         if not path:
             return None, ''
@@ -392,15 +429,15 @@
 
                 return File(
                     self,
                     self._managerPath(bucket, key),
                     modifiedTime=response['LastModified'],
                     size=response['ContentLength'],
                     metadata=self._getMetadataFromHead(response),
-                    content_type=response['ContentType'],
+                    content_type=response.get('ContentType'),
                 )
 
             except ClientError as e:
 
                 if "ResponseMetadata" in e.response:
                     if e.response['ResponseMetadata']['HTTPStatusCode'] == 404:
                         # No file existed with the given key - check if directory
@@ -417,17 +454,62 @@
                         return None
 
                 raise
 
     def _exists(self, managerPath: str):
         return self._identifyPath(managerPath) is not None
 
-    def _metadata(self, managerPath: str) -> typing.Dict[str, str]:
-        bucket, key = self._pathComponents(managerPath)
+    def _get_tags(self, artefact: ArtefactType) -> typing.Dict[str, str]:
 
+        bucket, key = self._pathComponents(artefact)
+        if bucket is None or key is None:
+            return {}
+
+        # Fetch the object tags - unpack and return
+        object_tagging = self._s3.get_object_tagging(
+            Bucket=bucket,
+            Key=key
+        )
+
+        return {tag['Key']: tag['Value'] for tag in object_tagging['TagSet']}
+
+    def _set_tags(self, artefact: ArtefactType, metadata: Metadata) -> Dict[str, str]:
+
+        # Freeze the metadata for the artefact
+        bucket, key = self._pathComponents(artefact, optional=False)
+        if bucket is None or key is None:
+            raise ValueError(f'S3 does not support setting tags on [{artefact}] - only files')
+
+
+        frozenMetadata = self._freezeMetadata(metadata, artefact)
+
+        # update the tagging on the object
+        self._s3.put_object_tagging(
+            Bucket=bucket,
+            Key=key,
+            Tagging={
+                'TagSet': [
+                    {'Key': k, 'Value': v}
+                    for k, v in frozenMetadata.items()
+                ]
+            }
+        )
+
+        # Fetch the object tags - unpack and return
+        object_tagging = self._s3.get_object_tagging(
+            Bucket=bucket,
+            Key=key
+        )
+
+        return {tag['Key']: tag['Value'] for tag in object_tagging['TagSet']}
+
+
+    def _get_metadata(self, artefact: ArtefactType) -> typing.Dict[str, str]:
+
+        bucket, key = self._pathComponents(artefact)
         if bucket is None or key is None:
             return {}
 
         else:
             try:
                 response = self._s3.head_object(
                     Bucket=bucket,
@@ -441,14 +523,42 @@
                     if e.response['ResponseMetadata']['HTTPStatusCode'] == 404:
                         raise exceptions.ArtefactNoLongerExists(
                             f'Failed to fetch metadata information for {key}'
                         )
 
                 raise
 
+    def _set_metadata(self, artefact: ArtefactType, metadata: Metadata) -> Dict[str, str]:
+
+        # Freeze the metadata for the artefact
+        bucket, key = self._pathComponents(artefact, optional=False)
+        if bucket is None or key is None:
+            raise ValueError(f'S3 does not support setting metadata on [{artefact}] - only files')
+
+        frozenMetadata = self._freezeMetadata(metadata, artefact)
+
+        # To update the metadata we have to replace the object in place
+        self._s3.copy_object(
+            Bucket=bucket,
+            Key=key,
+            CopySource={
+                "Bucket": bucket,
+                "Key": key
+            },
+            Metadata=frozenMetadata,
+            MetadataDirective="REPLACE"
+        )
+
+        response = self._s3.head_object(
+            Bucket=bucket,
+            Key=key
+        )
+
+        return self._getMetadataFromHead(response)
+
     def _digest(self, file: File, algorithm: HashingAlgorithm):
 
         if algorithm is HashingAlgorithm.MD5:
             raise NotImplementedError('AWS does not support conventional MD5 - use the ETag comparison method or localise file to calculate MD5')
 
         else:
 
@@ -685,16 +795,14 @@
                     source,
                     destination,
                     modified_time=modified_time or source.modifiedTime.timestamp(),
                     accessed_time=accessed_time or source.accessedTime.timestamp(),
                     callback=callback,
                 )
 
-        return PartialArtefact(self, destination)
-
     def _getBytes(self, source: File, callback: AbstractCallback) -> bytes:
 
         bucket, key = self._pathComponents(source)
 
         # Get buffer to recieve bytes
         bytes_buffer = io.BytesIO()
         callback.writing(1)
@@ -723,15 +831,17 @@
         self,
         source: File,
         bucket: str,
         key: str,
         extra_args: typing.Dict[str, str],
         callback: AbstractCallback,
         content_type: Optional[str],
-        storage_class: AmazonStorageClass
+        storage_class: AmazonStorageClass,
+        delete_source: bool = False,
+        delete_root: Optional[DeleteRoot] = None
         ):
 
         with source.localise() as abspath:
             try:
                 self._s3.upload_file(
                     abspath,
                     bucket,
@@ -741,14 +851,23 @@
                         "ContentType": (content_type or mimetypes.guess_type(key)[0] or 'application/octet-stream'),
                         **extra_args
                     },
                     Callback=callback.get_bytes_transfer(key, source.size),
                     Config=TransferConfig(use_threads=False)
                 )
 
+                if delete_source:
+                    # Delete the source that is being put - straight away
+                    source._manager._rm(path=source.path, callback=callback)
+
+                elif delete_root is not None:
+                    # Update the delete root shared object - delete source root once all tasks complete
+                    delete_root.finish_task()
+
+
             except boto3.exceptions.S3UploadFailedError as e:
 
                 if self._ensureBucket(bucket):
                     # The bucket was not present but it has now been created - we should be able to put item now
 
                     self._s3.upload_file(
                         abspath,
@@ -761,26 +880,32 @@
                         },
                         Callback=callback.get_bytes_transfer(key, source.size)
                     )
 
                 else:
                     raise
 
+            except:
+                log.exception('Unhandled error on file put')
+                raise
+
         callback.written(key)
 
     def _put(
         self,
         source: ArtefactType,
         destination: str,
         *,
         callback: AbstractCallback,
         worker_config: WorkerPoolConfig,
         content_type: Optional[str],
         storage_class: Optional[StorageClass],
         metadata: Optional[Metadata] = None,
+        delete_source: bool = False,
+        delete_root: Optional[DeleteRoot] = None,
         **kwargs
         ):
 
         # Mark that we are writting this source
         callback.writing(1)
 
         # Parse the destination string into the full bucket path
@@ -788,53 +913,78 @@
 
         if bucket is None:
             if isinstance(source, File):
                 raise exceptions.OperationNotPermitted(
                     f'Attempting to overwrite... s3 [{destination}]. With a... file [{source}]'
                 )
 
+            if delete_source:
+                delete_root = DeleteRoot(
+                    root=source,
+                    callback=callback,
+                    worker_config=worker_config
+                )
+
+            # We are putting this directory at the bucket level - each artefact inside will become a bucket
             for artefact in source.iterls():
                 if isinstance(artefact, Directory):
                     self._ensureBucket(artefact.basename)
 
                     # Put the contents of the directory into the bucket
                     self._put(
                         artefact,
                         '/' + artefact.basename,
                         callback=callback,
                         worker_config=worker_config,
                         content_type=content_type,
                         metadata=metadata,
-                        storage_class=storage_class
+                        storage_class=storage_class,
+                        delete_source=delete_source,
+                        delete_root=delete_root
                     )
 
                 else:
                     raise exceptions.OperationNotPermitted(
                         f'S3 bucket level cannot store files - {destination} is invalid for source {source}'
                     )
 
         else:
 
+            # Ensure that the bucket that we are writting to is available
+            self._ensureBucket(bucket)
+
             # Setup metadata about the objects being put
             amazon_storage_class = AmazonStorageClass.convert(storage_class or self.storage_class)
             extra_args = {}
 
             if isinstance(source, Directory):
+                # Putting a directory of artefacts - iterate through all subartefacts and put
 
+                # Set the initial directory to process + add a delete directory if needed
                 directories = [source]
+                if delete_source and delete_root is None:
+                    delete_root = DeleteRoot(
+                        root=source,
+                        callback=callback,
+                        worker_config=worker_config
+                    )
 
+                # Continue to process sub directories
                 while directories:
                     directory = directories.pop(0)
 
                     artefact = None
                     for artefact in directory.iterls():
                         callback.writing(1)
 
                         if isinstance(artefact, File):
 
+                            if delete_root is not None:
+                                delete_root.size += 1
+
                             file_destination = self.join(
                                 key,
                                 source.relpath(artefact, separator='/'),
                                 separator='/'
                             )
 
                             if metadata is not None:
@@ -844,15 +994,17 @@
                                 self._localise_put_file,
                                 artefact,
                                 bucket,
                                 file_destination,
                                 extra_args=extra_args,
                                 callback=callback,
                                 content_type=content_type,
-                                storage_class=amazon_storage_class
+                                storage_class=amazon_storage_class,
+                                delete_source=False,
+                                delete_root=delete_root
                             )
 
                         else:
                             directories.append(artefact)
 
                     if artefact is None:
                         # The directory was empty and therefore nothing was uploaded.
@@ -868,28 +1020,34 @@
                             Key=s3DirectoryFilepath + '/',
                             # callback=callback,
                             # StorageClass=amazon_storage_class.value  # This is a dictionary file so I don't know if its needed
                         )
 
                     callback.written(directory.path)
 
+                if delete_root is not None and delete_root.size == 0:
+                    # We moved a number of directories that didn't have any files inside them
+                    # We are safe to trigger the delete in the main thread of the directory source
+                    delete_root.trigger_delete()
+
             else:
 
                 if metadata is not None:
                     extra_args['Metadata'] = self._freezeMetadata(metadata, source)
 
                 worker_config.submit(
                     self._localise_put_file,
                     source,
                     bucket,
                     key,
                     extra_args=extra_args,
                     callback=callback,
                     content_type=content_type,
-                    storage_class=amazon_storage_class
+                    storage_class=amazon_storage_class,
+                    delete_source=delete_source
                 )
 
         return PartialArtefact(self, destination)
 
     def _putBytes(
         self,
         fileBytes: bytes,
@@ -1268,15 +1426,15 @@
     def s3_max_keys(self, value: int):
         self._s3_max_keys = value
 
     @property
     def config(self):
         return self._config
 
-    class CommandLineConfig:
+    class CommandLineConfig(AbstractCommandLineConfig):
 
         def __init__(self, manager: Type["Amazon"]):
             self._manager = manager
 
         @staticmethod
         def arguments() -> typing.List[typing.Tuple]:
             return [
```

### Comparing `stow-1.3.1/stow/managers/filesystem.py` & `stow-1.4.0/stow/managers/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,28 @@
     if os.name == 'nt':
         COPY_BUFFER_SIZE = 1024 * 1024
 
     else:
         COPY_BUFFER_SIZE = 64 * 1024
 
     def _abspath(self, path: str) -> str:
+
+        abspath = os.path.join(
+            self._path or self.SEPARATOR,
+            path.lstrip(self.SEPARATORS_STRING)
+        )
+
+        drive = self._drive
+        if os.name == 'nt' and len(abspath) > 258:
+            drive = '\\\\?\\' + drive
+
         return os.path.abspath(
             os.path.join(
-                self._drive,
-                self._path or self.SEPARATOR,
-                path.lstrip(self.SEPARATORS_STRING)
+                drive,
+                abspath
             )
         )
 
     def _relative(self, abspath: str) -> str:
         _, path = os.path.splitdrive(abspath)
         return path.removeprefix(self._path) or self.SEPARATOR
         # relpath = path.removeprefix(self._path)
@@ -442,14 +451,15 @@
         source: Artefact,
         destination: str,
         /,
         callback: AbstractCallback,
         modified_time: Optional[float] = None,
         accessed_time: Optional[float] = None,
         worker_config: Optional[WorkerPoolConfig] = None,
+        delete_source: bool = False,
         **kwargs
         ):
         """ For remote sources - we want to 'get' the artefact and place it directly at the destination location. This
         is exactly what remote managers are expecting when get is called. As such, by relying on the `artefact.save`
         which in turn calls get, we can handle local and remote managers by ensuring that our local get method copies
         files to the destination, and remote managers download the data to target location.
 
@@ -467,14 +477,18 @@
             callback=callback,
             modified_time=modified_time,
             accessed_time=accessed_time,
             worker_config=worker_config,
             force=True
         )
 
+        # Trigger delete of source
+        if delete_source:
+            source._manager._rm(source.path, callback=callback, worker_config=worker_config)
+
         # Create a partial artefact for the newly downloaded file
         return PartialArtefact(self, destination)
 
     def _putBytes(
         self,
         fileBytes: bytes,
         destination: str,
@@ -610,15 +624,15 @@
 
     @property
     def config(self):
         return {'path': os.path.join(self._drive, self._path)}
 
     @classmethod
     def _signatureFromURL(cls, url: urllib.parse.ParseResult):
-        return {'path': url.scheme and url.scheme + ':'}, os.path.join(os.getcwd(), url.path)
+        return {'path': url.scheme and url.scheme + ':'}, os.path.join(os.getcwd(), url.path) if not os.path.isabs(url.path) else url.path
 
     class CommandLineConfig:
         def __init__(self, manager):
             self._manager = manager
 
         @staticmethod
         def arguments() -> typing.List[typing.Tuple]:
```

### Comparing `stow-1.3.1/stow/managers/ssh.py` & `stow-1.4.0/stow/managers/ssh.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/stow/storage_classes.py` & `stow-1.4.0/stow/storage_classes.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/stow/utils.py` & `stow-1.4.0/stow/utils.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/stow/worker_config.py` & `stow-1.4.0/stow/worker_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,18 +86,29 @@
         config.futures = self.futures
         return config
 
     def detach(self):
         return WorkerPoolConfig(self._executor, join=True, shutdown=False)
 
     def join(self):
+        """ Join the active tasks - for all enqueued futures iterate through them and wait for them to complete.
+        """
         for future in concurrent.futures.as_completed(self.futures):
             future.result()
 
     def conclude(self, cancel: bool = False):
+        """ Trigger as per the config the finalisation of the work - If the join and shutdown is False then do nothing
+        else do what ever the config declares. Handle exceptions from the futures and ensure the internal worker pool is
+        cleaned up
+
+        Args:
+            cancel (bool): Interupt the work, cancelling any unstarted tasks and return early. Will still wait in-progress
+                tasks to finish.
+
+        """
         exception = None
         try:
             if not cancel and self._executor is not None and (self.will_shutdown or self.will_join):
                 self.join()
 
         except Exception as e:
             logger.exception('Exception in worker pool - cancelling command')
```

### Comparing `stow-1.3.1/stow.egg-info/PKG-INFO` & `stow-1.4.0/stow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stow
-Version: 1.3.1
+Version: 1.4.0
 Summary: stow artefacts anywhere, with ease
 Author: Kieran Bacon
 Author-email: kieran.bacon@outlook.com
 Project-URL: Homepage, https://github.com/Kieran-Bacon/stow
 Project-URL: Documentation, https://stow.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/Kieran-Bacon/stow/issues
 Keywords: aws s3 boto3 ssh os
@@ -15,19 +15,26 @@
 License-File: LICENSE
 Requires-Dist: tqdm
 Requires-Dist: typing_extensions
 Provides-Extra: all
 Requires-Dist: boto3; extra == "all"
 Requires-Dist: click; extra == "all"
 Requires-Dist: click-option-group; extra == "all"
-Provides-Extra: s3
-Requires-Dist: boto3; extra == "s3"
+Requires-Dist: google-api-python-client; extra == "all"
+Requires-Dist: google-auth-httplib2; extra == "all"
+Requires-Dist: google-auth-oauthlib; extra == "all"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 Requires-Dist: click-option-group; extra == "cli"
+Provides-Extra: s3
+Requires-Dist: boto3; extra == "s3"
+Provides-Extra: drive
+Requires-Dist: google-api-python-client; extra == "drive"
+Requires-Dist: google-auth-httplib2; extra == "drive"
+Requires-Dist: google-auth-oauthlib; extra == "drive"
 Provides-Extra: test
 Requires-Dist: pyini; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: moto[s3]>=4.1.5.dev40; extra == "test"
 Requires-Dist: mkdocs; extra == "test"
 Requires-Dist: mkdocstrings[python]==0.22.0; extra == "test"
```

### Comparing `stow-1.3.1/stow.egg-info/SOURCES.txt` & `stow-1.4.0/stow.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,19 @@
 stow/artefacts/__init__.py
 stow/artefacts/artefacts.py
 stow/artefacts/interfaces.py
 stow/artefacts/types.py
 stow/manager/__init__.py
 stow/manager/abstract_methods.py
 stow/manager/base_managers.py
+stow/manager/configs.py
 stow/manager/manager.py
 stow/managers/__init__.py
 stow/managers/amazon.py
 stow/managers/filesystem.py
+stow/managers/google.py
 stow/managers/kubernetes.py
 stow/managers/ssh.py
 tests/test_callbacks.py
 tests/test_cli.py
 tests/test_stateless.py
 tests/test_utils.py
```

### Comparing `stow-1.3.1/tests/test_callbacks.py` & `stow-1.4.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/tests/test_cli.py` & `stow-1.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/tests/test_stateless.py` & `stow-1.4.0/tests/test_stateless.py`

 * *Files identical despite different names*

### Comparing `stow-1.3.1/tests/test_utils.py` & `stow-1.4.0/tests/test_utils.py`

 * *Files identical despite different names*

