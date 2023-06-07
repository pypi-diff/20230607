# Comparing `tmp/spPersist-0.2.4.tar.gz` & `tmp/spPersist-0.2.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.2.4.tar", last modified: Wed Jun  7 09:55:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

