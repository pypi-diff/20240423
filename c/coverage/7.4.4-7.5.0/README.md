# Comparing `tmp/coverage-7.4.4.tar.gz` & `tmp/coverage-7.5.0-cp39-cp39-musllinux_1_1_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage-7.4.4.tar", last modified: Thu Mar 14 18:57:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

