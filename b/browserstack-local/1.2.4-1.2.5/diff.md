# Comparing `tmp/browserstack-local-1.2.4.tar.gz` & `tmp/browserstack-local-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/browserstack-local-1.2.4.tar", last modified: Wed Nov 16 08:05:59 2022, max compression
+gzip compressed data, was "dist/browserstack-local-1.2.5.tar", last modified: Wed Jun  7 09:28:36 2023, max compression
```

## Comparing `browserstack-local-1.2.4.tar` & `browserstack-local-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 aditya     (501) staff       (20)        0 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/
--rw-r--r--   0 aditya     (501) staff       (20)      432 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/PKG-INFO
-drwxr-xr-x   0 aditya     (501) staff       (20)        0 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/tests/
--rw-r--r--   0 aditya     (501) staff       (20)        0 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/tests/__init__.py
--rw-r--r--   0 aditya     (501) staff       (20)     3648 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/tests/test_local.py
-drwxr-xr-x   0 aditya     (501) staff       (20)        0 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/browserstack_local.egg-info/
--rw-r--r--   0 aditya     (501) staff       (20)      432 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/browserstack_local.egg-info/PKG-INFO
--rw-r--r--   0 aditya     (501) staff       (20)      407 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/browserstack_local.egg-info/SOURCES.txt
--rw-r--r--   0 aditya     (501) staff       (20)        7 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/browserstack_local.egg-info/requires.txt
--rw-r--r--   0 aditya     (501) staff       (20)       13 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/browserstack_local.egg-info/top_level.txt
--rw-r--r--   0 aditya     (501) staff       (20)        1 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/browserstack_local.egg-info/dependency_links.txt
--rw-r--r--   0 aditya     (501) staff       (20)      139 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/MANIFEST.in
--rw-r--r--   0 aditya     (501) staff       (20)       66 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/README
--rw-r--r--   0 aditya     (501) staff       (20)     5337 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/README.md
--rw-r--r--   0 aditya     (501) staff       (20)      611 2022-11-16 08:00:01.000000 browserstack-local-1.2.4/setup.py
--rw-r--r--   0 aditya     (501) staff       (20)       79 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/setup.cfg
-drwxr-xr-x   0 aditya     (501) staff       (20)        0 2022-11-16 08:05:59.000000 browserstack-local-1.2.4/browserstack/
--rw-r--r--   0 aditya     (501) staff       (20)      117 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/browserstack/bserrors.py
--rw-r--r--   0 aditya     (501) staff       (20)     3646 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/browserstack/local.py
--rw-r--r--   0 aditya     (501) staff       (20)        0 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/browserstack/__init__.py
--rw-r--r--   0 aditya     (501) staff       (20)     4006 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/browserstack/local_binary.py
--rw-r--r--   0 aditya     (501) staff       (20)     1080 2022-11-16 07:56:17.000000 browserstack-local-1.2.4/LICENSE.txt
+drwxr-xr-x   0 aditya     (503) staff       (20)        0 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/
+-rw-r--r--   0 aditya     (503) staff       (20)      432 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/PKG-INFO
+drwxr-xr-x   0 aditya     (503) staff       (20)        0 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/tests/
+-rw-r--r--   0 aditya     (503) staff       (20)        0 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/tests/__init__.py
+-rw-r--r--   0 aditya     (503) staff       (20)     3648 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/tests/test_local.py
+drwxr-xr-x   0 aditya     (503) staff       (20)        0 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/browserstack_local.egg-info/
+-rw-r--r--   0 aditya     (503) staff       (20)      432 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/browserstack_local.egg-info/PKG-INFO
+-rw-r--r--   0 aditya     (503) staff       (20)      407 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/browserstack_local.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya     (503) staff       (20)        7 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/browserstack_local.egg-info/requires.txt
+-rw-r--r--   0 aditya     (503) staff       (20)       13 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/browserstack_local.egg-info/top_level.txt
+-rw-r--r--   0 aditya     (503) staff       (20)        1 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/browserstack_local.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya     (503) staff       (20)      139 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/MANIFEST.in
+-rw-r--r--   0 aditya     (503) staff       (20)       66 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/README
+-rw-r--r--   0 aditya     (503) staff       (20)     5337 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/README.md
+-rw-r--r--   0 aditya     (503) staff       (20)      611 2023-06-02 08:41:54.000000 browserstack-local-1.2.5/setup.py
+-rw-r--r--   0 aditya     (503) staff       (20)       79 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/setup.cfg
+drwxr-xr-x   0 aditya     (503) staff       (20)        0 2023-06-07 09:28:36.000000 browserstack-local-1.2.5/browserstack/
+-rw-r--r--   0 aditya     (503) staff       (20)      117 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/browserstack/bserrors.py
+-rw-r--r--   0 aditya     (503) staff       (20)     3646 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/browserstack/local.py
+-rw-r--r--   0 aditya     (503) staff       (20)        0 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/browserstack/__init__.py
+-rw-r--r--   0 aditya     (503) staff       (20)     4101 2023-05-25 12:51:37.000000 browserstack-local-1.2.5/browserstack/local_binary.py
+-rw-r--r--   0 aditya     (503) staff       (20)     1080 2023-05-25 12:45:29.000000 browserstack-local-1.2.5/LICENSE.txt
```

### Comparing `browserstack-local-1.2.4/tests/test_local.py` & `browserstack-local-1.2.5/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `browserstack-local-1.2.4/README.md` & `browserstack-local-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `browserstack-local-1.2.4/setup.py` & `browserstack-local-1.2.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 setup(
   name = 'browserstack-local',
   packages = ['browserstack'],
-  version = '1.2.4',
+  version = '1.2.5',
   description = 'Python bindings for Browserstack Local',
   author = 'BrowserStack',
   author_email = 'support@browserstack.com',
   url = 'https://github.com/browserstack/browserstack-local-python',
   download_url = 'https://github.com/browserstack/browserstack-local-python/archive/master.zip',
   keywords = ['BrowserStack', 'Local', 'selenium', 'testing'],
   classifiers = [],
```

### Comparing `browserstack-local-1.2.4/browserstack/local.py` & `browserstack-local-1.2.5/browserstack/local.py`

 * *Files identical despite different names*

### Comparing `browserstack-local-1.2.4/browserstack/local_binary.py` & `browserstack-local-1.2.5/browserstack/local_binary.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 class LocalBinary:
   def __init__(self):
     is_64bits = sys.maxsize > 2**32
     self.is_windows = False
     osname = platform.system()
     if osname == 'Darwin':
-      self.http_path = "https://bstack-local-prod.s3.amazonaws.com/BrowserStackLocal-darwin-x64"
+      self.http_path = "https://www.browserstack.com/local-testing/downloads/binaries/BrowserStackLocal-darwin-x64"
     elif osname == 'Linux':
       if self.is_alpine():
-        self.http_path = "https://bstack-local-prod.s3.amazonaws.com/BrowserStackLocal-alpine"
+        self.http_path = "https://www.browserstack.com/local-testing/downloads/binaries/BrowserStackLocal-alpine"
       else:
         if is_64bits:
-          self.http_path = "https://bstack-local-prod.s3.amazonaws.com/BrowserStackLocal-linux-x64"
+          self.http_path = "https://www.browserstack.com/local-testing/downloads/binaries/BrowserStackLocal-linux-x64"
         else:
-          self.http_path = "https://bstack-local-prod.s3.amazonaws.com/BrowserStackLocal-linux-ia32"
+          self.http_path = "https://www.browserstack.com/local-testing/downloads/binaries/BrowserStackLocal-linux-ia32"
     else:
       self.is_windows = True
-      self.http_path = "https://bstack-local-prod.s3.amazonaws.com/BrowserStackLocal.exe"
+      self.http_path = "https://www.browserstack.com/local-testing/downloads/binaries/BrowserStackLocal.exe"
 
     self.ordered_paths = [
       os.path.join(os.path.expanduser('~'), '.browserstack'),
       os.getcwd(),
       tempfile.gettempdir()
     ]
     self.path_index = 0
```

### Comparing `browserstack-local-1.2.4/LICENSE.txt` & `browserstack-local-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

