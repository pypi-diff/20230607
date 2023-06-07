# Comparing `tmp/heatshrinkpy-0.10.0.tar.gz` & `tmp/heatshrinkpy-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatshrinkpy-0.10.0.tar", last modified: Sun Apr 25 20:40:49 2021, max compression
+gzip compressed data, was "heatshrinkpy-0.11.0.tar", max compression
```

## Comparing `heatshrinkpy-0.10.0.tar` & `heatshrinkpy-0.11.0.tar`

### file list

```diff
@@ -1,29 +1,22 @@
-drwxr-xr-x   0 yawor     (1000) yawor     (1000)        0 2021-04-25 20:40:49.561457 heatshrinkpy-0.10.0/
--rw-r--r--   0 yawor     (1000) yawor     (1000)      898 2021-04-25 20:07:59.000000 heatshrinkpy-0.10.0/LICENSE
--rw-r--r--   0 yawor     (1000) yawor     (1000)       75 2021-04-25 20:27:52.000000 heatshrinkpy-0.10.0/MANIFEST.in
--rw-r--r--   0 yawor     (1000) yawor     (1000)     1414 2021-04-25 20:40:49.561457 heatshrinkpy-0.10.0/PKG-INFO
--rw-r--r--   0 yawor     (1000) yawor     (1000)      703 2021-04-25 20:26:39.000000 heatshrinkpy-0.10.0/README.rst
-drwxr-xr-x   0 yawor     (1000) yawor     (1000)        0 2021-04-25 20:40:49.559457 heatshrinkpy-0.10.0/heatshrinkpy/
--rw-r--r--   0 yawor     (1000) yawor     (1000)     3088 2021-04-25 19:47:00.000000 heatshrinkpy-0.10.0/heatshrinkpy/__init__.py
--rw-r--r--   0 yawor     (1000) yawor     (1000)       36 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/heatshrinkpy/__main__.py
--rw-r--r--   0 yawor     (1000) yawor     (1000)    12855 2021-04-25 20:18:01.000000 heatshrinkpy-0.10.0/heatshrinkpy/streams.py
--rw-r--r--   0 yawor     (1000) yawor     (1000)       23 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/heatshrinkpy/version.py
-drwxr-xr-x   0 yawor     (1000) yawor     (1000)        0 2021-04-25 20:40:49.560457 heatshrinkpy-0.10.0/heatshrinkpy.egg-info/
--rw-r--r--   0 yawor     (1000) yawor     (1000)     1414 2021-04-25 20:40:49.000000 heatshrinkpy-0.10.0/heatshrinkpy.egg-info/PKG-INFO
--rw-r--r--   0 yawor     (1000) yawor     (1000)      478 2021-04-25 20:40:49.000000 heatshrinkpy-0.10.0/heatshrinkpy.egg-info/SOURCES.txt
--rw-r--r--   0 yawor     (1000) yawor     (1000)        1 2021-04-25 20:40:49.000000 heatshrinkpy-0.10.0/heatshrinkpy.egg-info/dependency_links.txt
--rw-r--r--   0 yawor     (1000) yawor     (1000)       13 2021-04-25 20:40:49.000000 heatshrinkpy-0.10.0/heatshrinkpy.egg-info/top_level.txt
--rw-r--r--   0 yawor     (1000) yawor     (1000)      104 2021-04-25 20:39:37.000000 heatshrinkpy-0.10.0/pyproject.toml
--rw-r--r--   0 yawor     (1000) yawor     (1000)       38 2021-04-25 20:40:49.561457 heatshrinkpy-0.10.0/setup.cfg
--rw-r--r--   0 yawor     (1000) yawor     (1000)      849 2021-04-25 20:14:39.000000 heatshrinkpy-0.10.0/setup.py
-drwxr-xr-x   0 yawor     (1000) yawor     (1000)        0 2021-04-25 20:40:49.560457 heatshrinkpy-0.10.0/tests/
--rw-r--r--   0 yawor     (1000) yawor     (1000)        0 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/tests/__init__.py
--rw-r--r--   0 yawor     (1000) yawor     (1000)     2510 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/tests/constants.py
-drwxr-xr-x   0 yawor     (1000) yawor     (1000)        0 2021-04-25 20:40:49.560457 heatshrinkpy-0.10.0/tests/files/
--rw-r--r--   0 yawor     (1000) yawor     (1000)     3281 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/tests/files/foo-8-5.hs
--rw-r--r--   0 yawor     (1000) yawor     (1000)     2727 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/tests/files/foo.hs
--rw-r--r--   0 yawor     (1000) yawor     (1000)     3970 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/tests/files/foo.txt
--rw-r--r--   0 yawor     (1000) yawor     (1000)     2167 2021-04-25 20:17:14.000000 heatshrinkpy-0.10.0/tests/test_command_line.py
--rw-r--r--   0 yawor     (1000) yawor     (1000)     6032 2021-04-25 20:17:29.000000 heatshrinkpy-0.10.0/tests/test_core.py
--rw-r--r--   0 yawor     (1000) yawor     (1000)    11668 2021-04-25 20:17:47.000000 heatshrinkpy-0.10.0/tests/test_streams.py
--rw-r--r--   0 yawor     (1000) yawor     (1000)      795 2021-04-24 07:09:09.000000 heatshrinkpy-0.10.0/tests/utils.py
+-rw-r--r--   0        0        0      898 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/LICENSE
+-rw-r--r--   0        0        0      702 2023-06-07 16:19:00.444244 heatshrinkpy-0.11.0/README.rst
+-rw-r--r--   0        0        0     3088 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/__main__.py
+-rw-r--r--   0        0        0     2693 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/__init__.py
+-rw-r--r--   0        0        0      813 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/common.py
+-rw-r--r--   0        0        0      146 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/consts.py
+-rw-r--r--   0        0        0     7404 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/core/decoder.py
+-rw-r--r--   0        0        0     9892 2023-06-07 16:19:19.162264 heatshrinkpy-0.11.0/heatshrinkpy/core/encoder.py
+-rw-r--r--   0        0        0    12855 2023-06-07 13:53:44.581386 heatshrinkpy-0.11.0/heatshrinkpy/streams.py
+-rw-r--r--   0        0        0      258 2023-06-07 16:19:00.439243 heatshrinkpy-0.11.0/heatshrinkpy/version.py
+-rw-r--r--   0        0        0      730 2023-06-07 16:19:00.443243 heatshrinkpy-0.11.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/__init__.py
+-rw-r--r--   0        0        0     2510 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/constants.py
+-rw-r--r--   0        0        0     3281 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/files/foo-8-5.hs
+-rw-r--r--   0        0        0     2727 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/files/foo.hs
+-rw-r--r--   0        0        0     3970 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/files/foo.txt
+-rw-r--r--   0        0        0     2167 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/test_command_line.py
+-rw-r--r--   0        0        0     6032 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/test_core.py
+-rw-r--r--   0        0        0    11667 2023-06-07 16:19:00.438243 heatshrinkpy-0.11.0/tests/test_streams.py
+-rw-r--r--   0        0        0      795 2023-06-07 13:53:44.622386 heatshrinkpy-0.11.0/tests/utils.py
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 heatshrinkpy-0.11.0/PKG-INFO
```

### Comparing `heatshrinkpy-0.10.0/LICENSE` & `heatshrinkpy-0.11.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/README.rst` & `heatshrinkpy-0.11.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 HeatshrinkPy
 ============
 
 Compression using the `Heatshrink algorithm
 <https://github.com/atomicobject/heatshrink>`__ in Python 3.
 
-This library is a pure Python rewrite and a drop-in replacenment of `heatshrink2 <https://github.com/eerimoq/pyheatshrink>`__ library.
+This library is a pure Python rewrite and a drop-in replacement of `heatshrink2 <https://github.com/eerimoq/pyheatshrink>`__ library.
 
 It is significantly slower than the native one. It can be used as a fallback if building a native extension is not an
 option.
 
 Installation
 ------------
```

### Comparing `heatshrinkpy-0.10.0/heatshrinkpy/__init__.py` & `heatshrinkpy-0.11.0/heatshrinkpy/__init__.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/heatshrinkpy/streams.py` & `heatshrinkpy-0.11.0/heatshrinkpy/streams.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/tests/constants.py` & `heatshrinkpy-0.11.0/tests/constants.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/tests/files/foo-8-5.hs` & `heatshrinkpy-0.11.0/tests/files/foo-8-5.hs`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/tests/files/foo.hs` & `heatshrinkpy-0.11.0/tests/files/foo.hs`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/tests/files/foo.txt` & `heatshrinkpy-0.11.0/tests/files/foo.txt`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/tests/test_command_line.py` & `heatshrinkpy-0.11.0/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/tests/test_core.py` & `heatshrinkpy-0.11.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `heatshrinkpy-0.10.0/tests/test_streams.py` & `heatshrinkpy-0.11.0/tests/test_streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
                 self.assertEqual(str(cm.exception), message)
 
     def test_invalid_modes(self):
         data = io.BytesIO()
 
         for mode in ['a+', 'w+', 'ab', 'r+', 'U', 'x', 'xb']:
-            with self.assertRaisesRegexp(ValueError, '^Invalid mode: .*$'):
+            with self.assertRaisesRegex(ValueError, '^Invalid mode: .*$'):
                 HeatshrinkFile(data, mode=mode)
 
     def test_round_trip(self):
         write_str = b'Testing\nAnd Stuff'
 
         self.fp.write(write_str)
         self.fp.close()
```

### Comparing `heatshrinkpy-0.10.0/tests/utils.py` & `heatshrinkpy-0.11.0/tests/utils.py`

 * *Files identical despite different names*

