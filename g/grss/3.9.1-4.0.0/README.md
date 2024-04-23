# Comparing `tmp/grss-3.9.1.tar.gz` & `tmp/grss-4.0.0-pp310-pypy310_pp73-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grss-3.9.1.tar", last modified: Sun Apr  7 22:17:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

