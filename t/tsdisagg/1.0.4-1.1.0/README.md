# Comparing `tmp/tsdisagg-1.0.4.tar.gz` & `tmp/tsdisagg-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsdisagg-1.0.4.tar", last modified: Sat Nov 25 16:17:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

