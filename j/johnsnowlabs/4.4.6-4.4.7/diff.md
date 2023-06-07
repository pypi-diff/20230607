# Comparing `tmp/johnsnowlabs-4.4.6.tar.gz` & `tmp/johnsnowlabs-4.4.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "johnsnowlabs-4.4.6.tar", last modified: Sun May 28 18:43:03 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

