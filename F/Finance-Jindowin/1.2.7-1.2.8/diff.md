# Comparing `tmp/Finance-Jindowin-1.2.7.tar.gz` & `tmp/Finance_Jindowin-1.2.8-py3.7.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Jindowin-1.2.7.tar", last modified: Tue Jun  6 10:27:48 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

