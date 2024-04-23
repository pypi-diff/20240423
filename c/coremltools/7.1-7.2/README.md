# Comparing `tmp/coremltools-7.1.tar.gz` & `tmp/coremltools-7.2-cp310-none-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coremltools-7.1.tar", last modified: Tue Oct 31 18:08:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

