# Comparing `tmp/botocore-a-la-carte-osis-1.29.147.tar.gz` & `tmp/botocore_a_la_carte_osis-1.29.148-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-osis-1.29.147.tar", last modified: Tue Jun  6 01:40:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

