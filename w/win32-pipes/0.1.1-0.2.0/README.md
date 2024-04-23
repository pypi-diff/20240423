# Comparing `tmp/win32_pipes-0.1.1.tar.gz` & `tmp/win32_pipes-0.2.0-cp38-cp38-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win32_pipes-0.1.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

