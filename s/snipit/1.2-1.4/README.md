# Comparing `tmp/snipit-1.2.tar.gz` & `tmp/snipit-1.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snipit-1.2.tar", last modified: Tue Nov 28 14:26:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

