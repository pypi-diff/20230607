# Comparing `tmp/pyobjc-framework-FileProvider-9.1b1.tar.gz` & `tmp/pyobjc_framework_FileProvider-9.2-cp39-cp39-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-FileProvider-9.1b1.tar", last modified: Sun Mar 26 11:24:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

