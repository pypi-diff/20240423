# Comparing `tmp/nwb4fp-0.5.9.6.tar.gz` & `tmp/nwb4fp-0.5.9.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.5.9.6.tar", last modified: Tue Apr  9 11:19:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

