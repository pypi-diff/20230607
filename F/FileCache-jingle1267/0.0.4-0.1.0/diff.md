# Comparing `tmp/FileCache-jingle1267-0.0.4.tar.gz` & `tmp/FileCache_jingle1267-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jinzhenguo/Documents/developer/pythonproject/FileCache/dist/tmpxvxturzf/FileCache-jingle1267-0.0.4.tar", last modified: Tue Jun 21 03:16:21 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

