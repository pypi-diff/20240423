# Comparing `tmp/melobot-2.5.9.tar.gz` & `tmp/melobot-2.6.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "melobot-2.5.9.tar", last modified: Mon Apr  1 16:24:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

