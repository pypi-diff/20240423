# Comparing `tmp/stela_publishing-0.2.26.tar.gz` & `tmp/stela_publishing-0.2.27-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stela_publishing-0.2.26.tar", last modified: Sat Apr 20 18:01:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

