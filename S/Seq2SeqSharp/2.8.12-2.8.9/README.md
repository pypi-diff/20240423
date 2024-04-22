# Comparing `tmp/Seq2SeqSharp-2.8.12.tar.gz` & `tmp/Seq2SeqSharp-2.8.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Works/Projects/Seq2SeqSharp/PyPackage/dist/.tmp-kul5wxey/Seq2SeqSharp-2.8.12.tar", last modified: Mon Apr 22 22:38:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

