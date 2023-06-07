# Comparing `tmp/dotpack-0.3.1.tar.gz` & `tmp/dotpack-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotpack-0.3.1.tar", last modified: Thu Sep 15 08:31:23 2022, max compression
+gzip compressed data, was "dotpack-0.3.2.tar", last modified: Mon Oct 31 03:39:53 2022, max compression
```

## Comparing `dotpack-0.3.1.tar` & `dotpack-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-09-15 08:31:23.394542 dotpack-0.3.1/
--rw-r--r--   0 wwj718     (501) staff       (20)      147 2022-05-05 03:06:54.000000 dotpack-0.3.1/AUTHORS.rst
--rw-r--r--   0 wwj718     (501) staff       (20)      235 2022-09-15 08:30:26.000000 dotpack-0.3.1/HISTORY.rst
--rw-r--r--   0 wwj718     (501) staff       (20)     1596 2022-05-05 03:06:54.000000 dotpack-0.3.1/LICENSE
--rw-r--r--   0 wwj718     (501) staff       (20)      303 2022-05-05 03:06:54.000000 dotpack-0.3.1/MANIFEST.in
--rw-r--r--   0 wwj718     (501) staff       (20)     1480 2022-09-15 08:31:23.394637 dotpack-0.3.1/PKG-INFO
--rw-r--r--   0 wwj718     (501) staff       (20)      500 2022-05-18 07:03:29.000000 dotpack-0.3.1/README.rst
-drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-09-15 08:31:23.391803 dotpack-0.3.1/dotpack/
--rw-r--r--   0 wwj718     (501) staff       (20)      147 2022-09-15 08:30:26.000000 dotpack-0.3.1/dotpack/__init__.py
--rw-r--r--   0 wwj718     (501) staff       (20)    24640 2022-09-15 08:30:26.000000 dotpack-0.3.1/dotpack/ledbag.py
--rw-r--r--   0 wwj718     (501) staff       (20)    22160 2022-09-15 08:30:26.000000 dotpack-0.3.1/dotpack/ledpanel.py
--rw-r--r--   0 wwj718     (501) staff       (20)     5592 2022-08-12 09:17:41.000000 dotpack-0.3.1/dotpack/microblocks_client.py
-drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-09-15 08:31:23.392718 dotpack-0.3.1/dotpack/src/
--rw-r--r--   0 wwj718     (501) staff       (20)   676304 2022-05-05 03:06:54.000000 dotpack-0.3.1/dotpack/src/seguiemj.ttf
--rw-r--r--   0 wwj718     (501) staff       (20)      549 2022-08-12 10:17:43.000000 dotpack-0.3.1/dotpack/utils.py
-drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-09-15 08:31:23.392622 dotpack-0.3.1/dotpack.egg-info/
--rw-r--r--   0 wwj718     (501) staff       (20)     1480 2022-09-15 08:31:23.000000 dotpack-0.3.1/dotpack.egg-info/PKG-INFO
--rw-r--r--   0 wwj718     (501) staff       (20)      419 2022-09-15 08:31:23.000000 dotpack-0.3.1/dotpack.egg-info/SOURCES.txt
--rw-r--r--   0 wwj718     (501) staff       (20)        1 2022-09-15 08:31:23.000000 dotpack-0.3.1/dotpack.egg-info/dependency_links.txt
--rw-r--r--   0 wwj718     (501) staff       (20)        1 2022-05-05 03:31:01.000000 dotpack-0.3.1/dotpack.egg-info/not-zip-safe
--rw-r--r--   0 wwj718     (501) staff       (20)      100 2022-09-15 08:31:23.000000 dotpack-0.3.1/dotpack.egg-info/requires.txt
--rw-r--r--   0 wwj718     (501) staff       (20)        8 2022-09-15 08:31:23.000000 dotpack-0.3.1/dotpack.egg-info/top_level.txt
--rw-r--r--   0 wwj718     (501) staff       (20)     1141 2022-08-12 09:21:30.000000 dotpack-0.3.1/readme.md
--rw-r--r--   0 wwj718     (501) staff       (20)      449 2022-09-15 08:31:23.394949 dotpack-0.3.1/setup.cfg
--rw-r--r--   0 wwj718     (501) staff       (20)     1602 2022-09-15 08:30:26.000000 dotpack-0.3.1/setup.py
-drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-09-15 08:31:23.394189 dotpack-0.3.1/tests/
--rw-r--r--   0 wwj718     (501) staff       (20)      622 2022-05-05 03:06:54.000000 dotpack-0.3.1/tests/test_dotpack.py
+drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-10-31 03:39:53.327549 dotpack-0.3.2/
+-rw-r--r--   0 wwj718     (501) staff       (20)      147 2022-05-05 03:06:54.000000 dotpack-0.3.2/AUTHORS.rst
+-rw-r--r--   0 wwj718     (501) staff       (20)      256 2022-10-31 03:37:46.000000 dotpack-0.3.2/HISTORY.rst
+-rw-r--r--   0 wwj718     (501) staff       (20)     1596 2022-05-05 03:06:54.000000 dotpack-0.3.2/LICENSE
+-rw-r--r--   0 wwj718     (501) staff       (20)      303 2022-05-05 03:06:54.000000 dotpack-0.3.2/MANIFEST.in
+-rw-r--r--   0 wwj718     (501) staff       (20)     1501 2022-10-31 03:39:53.327614 dotpack-0.3.2/PKG-INFO
+-rw-r--r--   0 wwj718     (501) staff       (20)      500 2022-05-18 07:03:29.000000 dotpack-0.3.2/README.rst
+drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-10-31 03:39:53.324980 dotpack-0.3.2/dotpack/
+-rw-r--r--   0 wwj718     (501) staff       (20)      147 2022-10-31 03:37:56.000000 dotpack-0.3.2/dotpack/__init__.py
+-rw-r--r--   0 wwj718     (501) staff       (20)    24642 2022-10-31 03:37:24.000000 dotpack-0.3.2/dotpack/ledbag.py
+-rw-r--r--   0 wwj718     (501) staff       (20)    22160 2022-09-15 08:30:26.000000 dotpack-0.3.2/dotpack/ledpanel.py
+-rw-r--r--   0 wwj718     (501) staff       (20)     5592 2022-08-12 09:17:41.000000 dotpack-0.3.2/dotpack/microblocks_client.py
+drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-10-31 03:39:53.326111 dotpack-0.3.2/dotpack/src/
+-rw-r--r--   0 wwj718     (501) staff       (20)   676304 2022-05-05 03:06:54.000000 dotpack-0.3.2/dotpack/src/seguiemj.ttf
+-rw-r--r--   0 wwj718     (501) staff       (20)      549 2022-08-12 10:17:43.000000 dotpack-0.3.2/dotpack/utils.py
+drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-10-31 03:39:53.325984 dotpack-0.3.2/dotpack.egg-info/
+-rw-r--r--   0 wwj718     (501) staff       (20)     1501 2022-10-31 03:39:53.000000 dotpack-0.3.2/dotpack.egg-info/PKG-INFO
+-rw-r--r--   0 wwj718     (501) staff       (20)      419 2022-10-31 03:39:53.000000 dotpack-0.3.2/dotpack.egg-info/SOURCES.txt
+-rw-r--r--   0 wwj718     (501) staff       (20)        1 2022-10-31 03:39:53.000000 dotpack-0.3.2/dotpack.egg-info/dependency_links.txt
+-rw-r--r--   0 wwj718     (501) staff       (20)        1 2022-05-05 03:31:01.000000 dotpack-0.3.2/dotpack.egg-info/not-zip-safe
+-rw-r--r--   0 wwj718     (501) staff       (20)      100 2022-10-31 03:39:53.000000 dotpack-0.3.2/dotpack.egg-info/requires.txt
+-rw-r--r--   0 wwj718     (501) staff       (20)        8 2022-10-31 03:39:53.000000 dotpack-0.3.2/dotpack.egg-info/top_level.txt
+-rw-r--r--   0 wwj718     (501) staff       (20)     1141 2022-08-12 09:21:30.000000 dotpack-0.3.2/readme.md
+-rw-r--r--   0 wwj718     (501) staff       (20)      449 2022-10-31 03:39:53.327874 dotpack-0.3.2/setup.cfg
+-rw-r--r--   0 wwj718     (501) staff       (20)     1602 2022-10-31 03:37:53.000000 dotpack-0.3.2/setup.py
+drwxr-xr-x   0 wwj718     (501) staff       (20)        0 2022-10-31 03:39:53.327326 dotpack-0.3.2/tests/
+-rw-r--r--   0 wwj718     (501) staff       (20)      622 2022-05-05 03:06:54.000000 dotpack-0.3.2/tests/test_dotpack.py
```

### Comparing `dotpack-0.3.1/LICENSE` & `dotpack-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.1/PKG-INFO` & `dotpack-0.3.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotpack
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/longan-link/dotpack_pyclient
 Author: Wenjie Wu
 Author-email: wuwenjie718@gmail.com
 License: GNU General Public License v3
 Keywords: dotpack
 Platform: UNKNOWN
@@ -50,14 +50,15 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
+* 0.3.2 (2022-10-31)
 * 0.3.1 (2022-09-15)
 * 0.3.0 (2022-05-25)
 * 0.2.1 (2022-05-19)
 * 0.2.0 (2022-05-18)
 * 0.1.4 (2022-05-10)
 * 0.1.3 (2022-05-6)
 * 0.1.2 (2022-05-5)
```

### Comparing `dotpack-0.3.1/dotpack/ledbag.py` & `dotpack-0.3.2/dotpack/ledbag.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         if self._microblocks_client:
             self._microblocks_client.disconnect()
 
         with self.__lock:
             self.__event_loop.call_soon_threadsafe(self.__event_loop.stop)
             self.__thread.join()
         self.__event_loop.close()
-        print("disconnected!")
+        # print("disconnected!")
 
     def load(self, filename):
         """加载图像，像素比例自动缩放到 16x16"""
         img = Image.open(filename)
         self._img = img.convert("RGB").resize((16, 16), Image.NEAREST)
         return True
```

### Comparing `dotpack-0.3.1/dotpack/ledpanel.py` & `dotpack-0.3.2/dotpack/ledpanel.py`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.1/dotpack/microblocks_client.py` & `dotpack-0.3.2/dotpack/microblocks_client.py`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.1/dotpack/src/seguiemj.ttf` & `dotpack-0.3.2/dotpack/src/seguiemj.ttf`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.1/dotpack/utils.py` & `dotpack-0.3.2/dotpack/utils.py`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.1/dotpack.egg-info/PKG-INFO` & `dotpack-0.3.2/dotpack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotpack
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/longan-link/dotpack_pyclient
 Author: Wenjie Wu
 Author-email: wuwenjie718@gmail.com
 License: GNU General Public License v3
 Keywords: dotpack
 Platform: UNKNOWN
@@ -50,14 +50,15 @@
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
 =======
 History
 =======
+* 0.3.2 (2022-10-31)
 * 0.3.1 (2022-09-15)
 * 0.3.0 (2022-05-25)
 * 0.2.1 (2022-05-19)
 * 0.2.0 (2022-05-18)
 * 0.1.4 (2022-05-10)
 * 0.1.3 (2022-05-6)
 * 0.1.2 (2022-05-5)
```

### Comparing `dotpack-0.3.1/readme.md` & `dotpack-0.3.2/readme.md`

 * *Files identical despite different names*

### Comparing `dotpack-0.3.1/setup.py` & `dotpack-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,10 +43,10 @@
             # 'dotpack-scan = dotpack.tools.scan:scan',
         ],
     },
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/longan-link/dotpack_pyclient',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False,
 )
```

### Comparing `dotpack-0.3.1/tests/test_dotpack.py` & `dotpack-0.3.2/tests/test_dotpack.py`

 * *Files identical despite different names*

