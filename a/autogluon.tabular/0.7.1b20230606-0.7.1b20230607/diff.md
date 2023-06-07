# Comparing `tmp/autogluon.tabular-0.7.1b20230606.tar.gz` & `tmp/autogluon.tabular-0.7.1b20230607-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.tabular-0.7.1b20230606.tar", last modified: Tue Jun  6 09:03:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

