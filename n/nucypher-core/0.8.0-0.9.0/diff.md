# Comparing `tmp/nucypher_core-0.8.0.tar.gz` & `tmp/nucypher_core-0.9.0-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucypher_core-0.8.0.tar", last modified: Tue May 23 18:41:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

