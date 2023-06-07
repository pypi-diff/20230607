# Comparing `tmp/ruptures-1.1.7rc1.tar.gz` & `tmp/ruptures-1.1.8rc1-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ruptures-1.1.7rc1.tar", last modified: Thu Jul  7 11:35:20 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

