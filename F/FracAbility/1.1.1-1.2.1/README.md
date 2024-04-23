# Comparing `tmp/FracAbility-1.1.1.tar.gz` & `tmp/FracAbility-1.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FracAbility-1.1.1.tar", last modified: Fri Nov 24 09:45:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

