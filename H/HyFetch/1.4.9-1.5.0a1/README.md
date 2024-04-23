# Comparing `tmp/HyFetch-1.4.9.tar.gz` & `tmp/HyFetch-1.5.0a1-py3-none-manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HyFetch-1.4.9.tar", last modified: Fri Jun  2 07:31:03 2023, max compression
+Zip archive data, at least v1.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

