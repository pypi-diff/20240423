# Comparing `tmp/pgn_to_sqlite-2.1.8.tar.gz` & `tmp/pgn_to_sqlite-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgn_to_sqlite-2.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pgn_to_sqlite-2.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pgn_to_sqlite-2.1.8.tar` & `pgn_to_sqlite-2.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       54 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/.coveragerc
--rw-r--r--   0        0        0      602 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/.github/dependabot.yml
--rw-r--r--   0        0        0      582 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/.github/workflows/lint.yml
--rw-r--r--   0        0        0      808 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0      715 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0       78 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/.gitignore
--rw-r--r--   0        0        0     1078 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/LICENSE
--rw-r--r--   0        0        0     3204 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/README.md
--rw-r--r--   0        0        0       88 2024-03-25 23:58:07.518206 pgn_to_sqlite-2.1.8/pgn_to_sqlite/__init__.py
--rw-r--r--   0        0        0     8349 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/pgn_to_sqlite/cli.py
--rw-r--r--   0        0        0      957 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/pyproject.toml
--rw-r--r--   0        0        0      155 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/pytest.ini
--rw-r--r--   0        0        0      185 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/requirements-dev.in
--rw-r--r--   0        0        0    24674 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/requirements-dev.txt
--rw-r--r--   0        0        0      696 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/ruff.toml
--rw-r--r--   0        0        0        0 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/tests/__init__.py
--rw-r--r--   0        0        0      506 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/tests/game_files/test_pgn_file_chess_dotcom.pgn
--rw-r--r--   0        0        0      885 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/tests/game_files/test_pgn_file_lichess.pgn
--rw-r--r--   0        0        0     1434 2024-03-25 23:58:07.522206 pgn_to_sqlite-2.1.8/tests/test_cli.py
--rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/.coveragerc
+-rw-r--r--   0        0        0      602 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      582 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      808 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      715 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0       78 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/.gitignore
+-rw-r--r--   0        0        0     1078 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/LICENSE
+-rw-r--r--   0        0        0     3204 2024-04-23 18:22:54.489327 pgn_to_sqlite-2.1.9/README.md
+-rw-r--r--   0        0        0       88 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/pgn_to_sqlite/__init__.py
+-rw-r--r--   0        0        0     8349 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/pgn_to_sqlite/cli.py
+-rw-r--r--   0        0        0      957 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0      155 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/pytest.ini
+-rw-r--r--   0        0        0      185 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/requirements-dev.in
+-rw-r--r--   0        0        0    24674 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/requirements-dev.txt
+-rw-r--r--   0        0        0      696 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/ruff.toml
+-rw-r--r--   0        0        0        0 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      506 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/tests/game_files/test_pgn_file_chess_dotcom.pgn
+-rw-r--r--   0        0        0      885 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/tests/game_files/test_pgn_file_lichess.pgn
+-rw-r--r--   0        0        0     1434 2024-04-23 18:22:54.493327 pgn_to_sqlite-2.1.9/tests/test_cli.py
+-rw-r--r--   0        0        0     4093 1970-01-01 00:00:00.000000 pgn_to_sqlite-2.1.9/PKG-INFO
```

### Comparing `pgn_to_sqlite-2.1.8/.github/dependabot.yml` & `pgn_to_sqlite-2.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/.github/workflows/lint.yml` & `pgn_to_sqlite-2.1.9/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/.github/workflows/publish.yml` & `pgn_to_sqlite-2.1.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/.github/workflows/run_tests.yml` & `pgn_to_sqlite-2.1.9/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/LICENSE` & `pgn_to_sqlite-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/README.md` & `pgn_to_sqlite-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/pgn_to_sqlite/cli.py` & `pgn_to_sqlite-2.1.9/pgn_to_sqlite/cli.py`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/pyproject.toml` & `pgn_to_sqlite-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 dynamic = ["description"]
 dependencies  = [
     "berserk==0.13.2",
     "click==8.1.7",
     "requests==2.31.0"
 ]
 requires-python=">=3.8"
-version="2.1.8"
+version="2.1.9"
 
 [project.urls]
 Home = "https://github.com/EndlessTrax/pgn-to-sqlite"
 Documentation = "https://github.com/EndlessTrax/pgn-to-sqlite/blob/master/README.md"
 Issues = "https://github.com/EndlessTrax/pgn-to-sqlite/issues"
 
 [project.scripts]
```

### Comparing `pgn_to_sqlite-2.1.8/requirements-dev.txt` & `pgn_to_sqlite-2.1.9/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -166,29 +166,29 @@
     --hash=sha256:6fac8b097794a90302bdbb17b9b815e732d3c4720583ff1b198499d78470466c \
     --hash=sha256:e5323eb936458dccc2582dc6f9c322c852a775a27065ff2b0c4970b9d53d01b3
     # via berserk
 docutils==0.20.1 \
     --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
     --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
     # via flit
-exceptiongroup==1.2.0 \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
+exceptiongroup==1.2.1 \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
     # via -r requirements-dev.in
 flit==3.9.0 \
     --hash=sha256:076c3aaba5ac24cf0ad3251f910900d95a08218e6bcb26f21fef1036cc4679ca \
     --hash=sha256:d75edf5eb324da20d53570a6a6f87f51e606eee8384925cd66a90611140844c7
     # via -r requirements-dev.in
 flit-core==3.9.0 \
     --hash=sha256:72ad266176c4a3fcfab5f2930d76896059851240570ce9a98733b658cb786eba \
     --hash=sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301
     # via flit
-idna==3.4 \
-    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
-    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 ndjson==0.3.1 \
     --hash=sha256:839c22275e6baa3040077b83c005ac24199b94973309a8a1809be962c753a410 \
@@ -219,32 +219,32 @@
 requests==2.31.0 \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
     #   -r requirements-dev.in
     #   berserk
     #   flit
-ruff==0.3.4 \
-    --hash=sha256:3f3860057590e810c7ffea75669bdc6927bfd91e29b4baa9258fd48b540a4365 \
-    --hash=sha256:519cf6a0ebed244dce1dc8aecd3dc99add7a2ee15bb68cf19588bb5bf58e0488 \
-    --hash=sha256:60c870a7d46efcbc8385d27ec07fe534ac32f3b251e4fc44b3cbfd9e09609ef4 \
-    --hash=sha256:64abeed785dad51801b423fa51840b1764b35d6c461ea8caef9cf9e5e5ab34d9 \
-    --hash=sha256:6810563cc08ad0096b57c717bd78aeac888a1bfd38654d9113cb3dc4d3f74232 \
-    --hash=sha256:6fc14fa742e1d8f24910e1fff0bd5e26d395b0e0e04cc1b15c7c5e5fe5b4af91 \
-    --hash=sha256:986f2377f7cf12efac1f515fc1a5b753c000ed1e0a6de96747cdf2da20a1b369 \
-    --hash=sha256:98e98300056445ba2cc27d0b325fd044dc17fcc38e4e4d2c7711585bd0a958ed \
-    --hash=sha256:af27ac187c0a331e8ef91d84bf1c3c6a5dea97e912a7560ac0cef25c526a4102 \
-    --hash=sha256:bb0acfb921030d00070539c038cd24bb1df73a2981e9f55942514af8b17be94e \
-    --hash=sha256:c4fd98e85869603e65f554fdc5cddf0712e352fe6e61d29d5a6fe087ec82b76c \
-    --hash=sha256:cf133dd744f2470b347f602452a88e70dadfbe0fcfb5fd46e093d55da65f82f7 \
-    --hash=sha256:cf187a7e7098233d0d0c71175375c5162f880126c4c716fa28a8ac418dcf3378 \
-    --hash=sha256:d3ee7880f653cc03749a3bfea720cf2a192e4f884925b0cf7eecce82f0ce5854 \
-    --hash=sha256:de0d5069b165e5a32b3c6ffbb81c350b1e3d3483347196ffdf86dc0ef9e37dd6 \
-    --hash=sha256:df52972138318bc7546d92348a1ee58449bc3f9eaf0db278906eb511889c4b50 \
-    --hash=sha256:f0f4484c6541a99862b693e13a151435a279b271cff20e37101116a21e2a1ad1
+ruff==0.4.1 \
+    --hash=sha256:0926cefb57fc5fced629603fbd1a23d458b25418681d96823992ba975f050c2b \
+    --hash=sha256:1c859f294f8633889e7d77de228b203eb0e9a03071b72b5989d89a0cf98ee262 \
+    --hash=sha256:2c6e37f2e3cd74496a74af9a4fa67b547ab3ca137688c484749189bf3a686ceb \
+    --hash=sha256:2d9ef6231e3fbdc0b8c72404a1a0c46fd0dcea84efca83beb4681c318ea6a953 \
+    --hash=sha256:6e68d248ed688b9d69fd4d18737edcbb79c98b251bba5a2b031ce2470224bdf9 \
+    --hash=sha256:9485f54a7189e6f7433e0058cf8581bee45c31a25cd69009d2a040d1bd4bfaef \
+    --hash=sha256:a1eaf03d87e6a7cd5e661d36d8c6e874693cb9bc3049d110bc9a97b350680c43 \
+    --hash=sha256:b34510141e393519a47f2d7b8216fec747ea1f2c81e85f076e9f2910588d4b64 \
+    --hash=sha256:b90506f3d6d1f41f43f9b7b5ff845aeefabed6d2494307bc7b178360a8805252 \
+    --hash=sha256:b92f03b4aa9fa23e1799b40f15f8b95cdc418782a567d6c43def65e1bbb7f1cf \
+    --hash=sha256:baa27d9d72a94574d250f42b7640b3bd2edc4c58ac8ac2778a8c82374bb27984 \
+    --hash=sha256:c7d391e5936af5c9e252743d767c564670dc3889aff460d35c518ee76e4b26d7 \
+    --hash=sha256:d2921ac03ce1383e360e8a95442ffb0d757a6a7ddd9a5be68561a671e0e5807e \
+    --hash=sha256:d592116cdbb65f8b1b7e2a2b48297eb865f6bdc20641879aa9d7b9c11d86db79 \
+    --hash=sha256:eec8d185fe193ad053eda3a6be23069e0c8ba8c5d20bc5ace6e3b9e37d246d3f \
+    --hash=sha256:efd703a5975ac1998c2cc5e9494e13b28f31e66c616b0a76e206de2562e0843c \
+    --hash=sha256:f1ee41580bff1a651339eb3337c20c12f4037f6110a36ae4a2d864c52e5ef954
     # via -r requirements-dev.in
 six==1.16.0 \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
     # via python-dateutil
 tomli-w==1.0.0 \
     --hash=sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463 \
```

### Comparing `pgn_to_sqlite-2.1.8/ruff.toml` & `pgn_to_sqlite-2.1.9/ruff.toml`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/tests/game_files/test_pgn_file_lichess.pgn` & `pgn_to_sqlite-2.1.9/tests/game_files/test_pgn_file_lichess.pgn`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/tests/test_cli.py` & `pgn_to_sqlite-2.1.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pgn_to_sqlite-2.1.8/PKG-INFO` & `pgn_to_sqlite-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgn_to_sqlite
-Version: 2.1.8
+Version: 2.1.9
 Summary: Fetch your games from chess.com and lichess.org and add them to a sqlite database
 Author-email: Ricky White <ricky@rickywhite.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

