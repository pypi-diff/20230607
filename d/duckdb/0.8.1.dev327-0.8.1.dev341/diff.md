# Comparing `tmp/duckdb-0.8.1.dev327.tar.gz` & `tmp/duckdb-0.8.1.dev341-cp36-cp36m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/duckdb-0.8.1.dev327.tar", last modified: Tue Jun  6 04:11:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

