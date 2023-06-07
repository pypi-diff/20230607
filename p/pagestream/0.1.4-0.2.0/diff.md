# Comparing `tmp/pagestream-0.1.4.tar.gz` & `tmp/pagestream-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pagestream-0.1.4.tar", last modified: Mon Jan 23 14:37:40 2023, max compression
+gzip compressed data, was "pagestream-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pagestream-0.1.4.tar` & `pagestream-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.1.4/.gitignore
--rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.1.4/LICENSE
--rw-r--r--   0        0        0      624 2023-01-10 15:22:41.920947 pagestream-0.1.4/README.md
--rw-r--r--   0        0        0      423 2023-01-23 14:36:48.931954 pagestream-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3815 2023-01-23 14:37:23.489338 pagestream-0.1.4/src/pagestream/__init__.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 pagestream-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-01-10 15:37:06.079380 pagestream-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1080 2023-01-10 14:58:19.027912 pagestream-0.2.0/LICENSE
+-rw-r--r--   0        0        0      624 2023-01-10 15:22:41.920947 pagestream-0.2.0/README.md
+-rw-r--r--   0        0        0      487 2023-06-07 12:59:31.135307 pagestream-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2367 2023-06-07 14:50:42.907363 pagestream-0.2.0/src/pagestream/__init__.py
+-rwxr-xr-x   0        0        0      700 2023-06-07 14:48:44.058259 pagestream-0.2.0/src/pagestream/cli.py
+-rw-r--r--   0        0        0      993 1970-01-01 00:00:00.000000 pagestream-0.2.0/PKG-INFO
```

### Comparing `pagestream-0.1.4/LICENSE` & `pagestream-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pagestream-0.1.4/README.md` & `pagestream-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pagestream-0.1.4/PKG-INFO` & `pagestream-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pagestream
-Version: 0.1.4
+Version: 0.2.0
 Summary: Handle PDF pagestreams with PikePDF and split them by outline
 Author-email: Johan Schuijt <johan@ftm.nl>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pikepdf
+Requires-Dist: click
 Project-URL: Home, https://github.com/followthemoney/pagestream
 
 
 # PageStream
 
 Some scanners and PDF merge software results in a single merged PDF that has the
 original document title in the outline. The dutch government uses software like
```

