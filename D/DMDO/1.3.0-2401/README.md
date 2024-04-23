# Comparing `tmp/DMDO-1.3.0.tar.gz` & `tmp/DMDO-2401-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMDO-1.3.0.tar", last modified: Mon Nov 21 00:45:23 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

