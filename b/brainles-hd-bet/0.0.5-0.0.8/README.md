# Comparing `tmp/BrainLes_HD-BET-0.0.5.tar.gz` & `tmp/brainles_hd_bet-0.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrainLes_HD-BET-0.0.5.tar", last modified: Wed Oct 18 14:20:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

