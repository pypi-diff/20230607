# Comparing `tmp/plog-python-1.0.2.tar.gz` & `tmp/plog_python-1.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plog-python-1.0.2.tar", last modified: Wed Jun  7 01:52:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

