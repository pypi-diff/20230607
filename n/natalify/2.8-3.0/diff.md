# Comparing `tmp/natalify-2.8.tar.gz` & `tmp/natalify-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natalify-2.8.tar", last modified: Wed May 24 08:35:04 2023, max compression
+gzip compressed data, was "natalify-3.0.tar", last modified: Wed Jun  7 14:52:04 2023, max compression
```

## Comparing `natalify-2.8.tar` & `natalify-3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 08:35:04.071459 natalify-2.8/
--rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-2.8/LICENSE
--rw-rw-rw-   0        0        0     2184 2023-05-24 08:35:04.071459 natalify-2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1664 2023-05-22 11:28:41.000000 natalify-2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 08:35:04.055836 natalify-2.8/natalify/
--rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-2.8/natalify/__init__.py
--rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-2.8/natalify/__main__.py
--rw-rw-rw-   0        0        0    64029 2023-05-24 08:33:11.000000 natalify-2.8/natalify/natalify.py
-drwxrwxrwx   0        0        0        0 2023-05-24 08:35:04.071459 natalify-2.8/natalify.egg-info/
--rw-rw-rw-   0        0        0     2184 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-24 08:35:03.000000 natalify-2.8/natalify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-24 08:35:02.000000 natalify-2.8/natalify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 08:35:04.071459 natalify-2.8/setup.cfg
--rw-rw-rw-   0        0        0      852 2023-05-24 08:34:30.000000 natalify-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:52:04.549696 natalify-3.0/
+-rw-rw-rw-   0        0        0     1344 2023-05-22 10:26:13.000000 natalify-3.0/LICENSE
+-rw-rw-rw-   0        0        0     2184 2023-06-07 14:52:04.549696 natalify-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1664 2023-05-22 11:28:41.000000 natalify-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:52:04.534072 natalify-3.0/natalify/
+-rw-rw-rw-   0        0        0       25 2023-05-22 10:10:51.000000 natalify-3.0/natalify/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-05-22 10:11:37.000000 natalify-3.0/natalify/__main__.py
+-rw-rw-rw-   0        0        0    64049 2023-06-07 14:51:01.000000 natalify-3.0/natalify/natalify.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:52:04.534072 natalify-3.0/natalify.egg-info/
+-rw-rw-rw-   0        0        0     2184 2023-06-07 14:52:02.000000 natalify-3.0/natalify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-07 14:52:04.000000 natalify-3.0/natalify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:52:03.000000 natalify-3.0/natalify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-06-07 14:52:03.000000 natalify-3.0/natalify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 14:52:03.000000 natalify-3.0/natalify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:52:04.549696 natalify-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      852 2023-06-07 14:51:55.000000 natalify-3.0/setup.py
```

### Comparing `natalify-2.8/LICENSE` & `natalify-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `natalify-2.8/PKG-INFO` & `natalify-3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 2.8
+Version: 3.0
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `natalify-2.8/README.md` & `natalify-3.0/README.md`

 * *Files identical despite different names*

### Comparing `natalify-2.8/natalify/natalify.py` & `natalify-3.0/natalify/natalify.py`

 * *Files 0% similar despite different names*

```diff
@@ -862,15 +862,15 @@
 
         await self.search(search_key,0)
 
         self.driver.switch_to.window(win_handle[0])
 
         try:
 
-            hashtags_posts=300
+            hashtags_posts=random.randrange(12,20)
 
             for row in range(0,hashtags_posts):
             
                 
                 wait = WebDriverWait(self.driver, 50)  
 
                 post = wait.until(EC.presence_of_all_elements_located((By.CLASS_NAME, '_aabd')))
```

### Comparing `natalify-2.8/natalify.egg-info/PKG-INFO` & `natalify-3.0/natalify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natalify
-Version: 2.8
+Version: 3.0
 Summary: A simple automation software for various tasks
 Author: jack
 Author-email: kinginjack@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `natalify-2.8/setup.py` & `natalify-3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='natalify',
-    version='2.8',
+    version='3.0',
     packages=setuptools.find_packages(),
     license='GPL-3.0',
     author='jack',
     author_email='kinginjack@gmail.com',
     description='A simple automation software for various tasks',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

