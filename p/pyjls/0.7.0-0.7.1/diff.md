# Comparing `tmp/pyjls-0.7.0.tar.gz` & `tmp/pyjls-0.7.1-cp311-cp311-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjls-0.7.0.tar", last modified: Wed May 31 12:16:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

