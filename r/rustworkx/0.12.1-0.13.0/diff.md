# Comparing `tmp/rustworkx-0.12.1.tar.gz` & `tmp/rustworkx-0.13.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rustworkx-0.12.1.tar", last modified: Wed Nov 23 17:36:56 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

