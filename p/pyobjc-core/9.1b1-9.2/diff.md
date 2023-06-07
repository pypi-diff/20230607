# Comparing `tmp/pyobjc-core-9.1b1.tar.gz` & `tmp/pyobjc_core-9.2-cp311-cp311-macosx_10_9_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-core-9.1b1.tar", last modified: Sun Mar 26 10:48:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

