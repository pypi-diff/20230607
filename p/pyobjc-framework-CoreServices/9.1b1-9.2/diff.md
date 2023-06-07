# Comparing `tmp/pyobjc-framework-CoreServices-9.1b1.tar.gz` & `tmp/pyobjc_framework_CoreServices-9.2-cp36-abi3-macosx_11_0_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobjc-framework-CoreServices-9.1b1.tar", last modified: Sun Mar 26 11:21:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

