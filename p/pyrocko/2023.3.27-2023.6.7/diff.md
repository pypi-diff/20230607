# Comparing `tmp/pyrocko-2023.3.27.tar.gz` & `tmp/pyrocko-2023.6.7-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrocko-2023.3.27.tar", last modified: Mon Mar 27 14:04:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

