# Comparing `tmp/PyCorrCPI-0.0.1b0.tar.gz` & `tmp/PyCorrCPI-0.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCorrCPI-0.0.1b0.tar", last modified: Tue Apr 23 17:49:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

