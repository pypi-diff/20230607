# Comparing `tmp/geopyv-0.0.8.tar.gz` & `tmp/geopyv-0.0.9-cp38-cp38-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geopyv-0.0.8.tar", last modified: Mon Jun  5 12:07:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

