# Comparing `tmp/image_center-1.0.1.tar.gz` & `tmp/image_center-1.1.2.tar.gz`

## Comparing `image_center-1.0.1.tar` & `image_center-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/__version__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/conf.py
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 image_center-1.0.1/image_center/server.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 image_center-1.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-1.0.1/LICENSE
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 image_center-1.0.1/README.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 image_center-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 image_center-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15319 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/__version__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/conf.py
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 image_center-1.1.2/image_center/server.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 image_center-1.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 image_center-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 image_center-1.1.2/README.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 image_center-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 image_center-1.1.2/PKG-INFO
```

### Comparing `image_center-1.0.1/image_center/conf.py` & `image_center-1.1.2/image_center/conf.py`

 * *Files identical despite different names*

### Comparing `image_center-1.0.1/image_center/server.py` & `image_center-1.1.2/image_center/server.py`

 * *Files identical despite different names*

### Comparing `image_center-1.0.1/.gitignore` & `image_center-1.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `image_center-1.0.1/LICENSE` & `image_center-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image_center-1.0.1/README.md` & `image_center-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `image_center-1.0.1/pyproject.toml` & `image_center-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `image_center-1.0.1/PKG-INFO` & `image_center-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-center
-Version: 1.0.1
+Version: 1.1.2
 Summary: image-center
 Project-URL: Source, https://github.com/funny-test/image-center
 Project-URL: Documentation, https://funny-test.github.io/image-center
 Author-email: mikigo <1964191531@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: image-center Version: 1.0.1 Summary: image-center
+Metadata-Version: 2.1 Name: image-center Version: 1.1.2 Summary: image-center
 Project-URL: Source, https://github.com/funny-test/image-center Project-URL:
 Documentation, https://funny-test.github.io/image-center Author-email: mikigo
 <1964191531@qq.com> License-File: LICENSE Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Requires-Python: >=3.7
 Requires-Dist: pillow Requires-Dist: pyscreenshot Provides-Extra: doc Requires-
 Dist: mkdocs-material; extra == 'doc' Provides-Extra: test Requires-Dist:
```

