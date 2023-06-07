# Comparing `tmp/jupyterlab_empinken_extension-0.1.1.tar.gz` & `tmp/jupyterlab_empinken_extension-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_empinken_extension-0.1.1.tar", last modified: Thu Apr 14 12:23:10 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

