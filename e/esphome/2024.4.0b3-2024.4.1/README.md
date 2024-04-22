# Comparing `tmp/esphome-2024.4.0b3.tar.gz` & `tmp/esphome-2024.4.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esphome-2024.4.0b3.tar", last modified: Mon Apr 15 04:05:06 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

