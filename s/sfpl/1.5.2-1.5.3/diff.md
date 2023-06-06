# Comparing `tmp/sfpl-1.5.2.tar.gz` & `tmp/sfpl-1.5.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sfpl-1.5.2.tar", last modified: Tue Apr 21 02:19:27 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

