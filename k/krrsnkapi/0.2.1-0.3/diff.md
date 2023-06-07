# Comparing `tmp/krrsnkapi-0.2.1.tar.gz` & `tmp/krrsnkapi-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krrsnkapi-0.2.1.tar", last modified: Thu Apr 13 17:14:25 2023, max compression
+gzip compressed data, was "krrsnkapi-0.3.tar", last modified: Wed Jun  7 17:33:32 2023, max compression
```

## Comparing `krrsnkapi-0.2.1.tar` & `krrsnkapi-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 17:14:25.643639 krrsnkapi-0.2.1/
--rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      665 2023-04-13 17:14:25.644639 krrsnkapi-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 17:14:25.629638 krrsnkapi-0.2.1/krrsnkapi/
--rw-rw-rw-   0        0        0       35 2023-04-13 13:20:12.000000 krrsnkapi-0.2.1/krrsnkapi/__init__.py
--rw-rw-rw-   0        0        0     1881 2023-04-13 16:55:34.000000 krrsnkapi-0.2.1/krrsnkapi/krrsnkapi.py
-drwxrwxrwx   0        0        0        0 2023-04-13 17:14:25.641639 krrsnkapi-0.2.1/krrsnkapi.egg-info/
--rw-rw-rw-   0        0        0      665 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-04-13 17:14:25.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 17:14:24.000000 krrsnkapi-0.2.1/krrsnkapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-13 17:14:25.646639 krrsnkapi-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1536 2023-04-13 17:14:06.000000 krrsnkapi-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:33:32.722921 krrsnkapi-0.3/
+-rw-rw-rw-   0        0        0     1087 2023-04-13 13:12:53.000000 krrsnkapi-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      617 2023-06-07 17:33:32.722921 krrsnkapi-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1569 2023-04-13 12:53:07.000000 krrsnkapi-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 17:33:32.707920 krrsnkapi-0.3/krrsnkapi/
+-rw-rw-rw-   0        0        0       35 2023-04-13 13:20:12.000000 krrsnkapi-0.3/krrsnkapi/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-06-07 17:23:47.000000 krrsnkapi-0.3/krrsnkapi/krrsnkapi.py
+drwxrwxrwx   0        0        0        0 2023-06-07 17:33:32.719921 krrsnkapi-0.3/krrsnkapi.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-07 17:33:31.000000 krrsnkapi-0.3/krrsnkapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-06-07 17:33:32.000000 krrsnkapi-0.3/krrsnkapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 17:33:31.000000 krrsnkapi-0.3/krrsnkapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-07 17:33:31.000000 krrsnkapi-0.3/krrsnkapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-07 17:33:32.000000 krrsnkapi-0.3/krrsnkapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-07 17:33:32.724922 krrsnkapi-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1445 2023-06-07 17:24:34.000000 krrsnkapi-0.3/setup.py
```

### Comparing `krrsnkapi-0.2.1/LICENSE.txt` & `krrsnkapi-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.2.1/PKG-INFO` & `krrsnkapi-0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.2.1
-Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok_gd/krrsnkapi
-Home-page: https://github.com/kararasenok_gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.2.tar.gz
+Version: 0.3
+Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
+Home-page: https://github.com/kararasenok-gd/krrsnkapi
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.3.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
```

### Comparing `krrsnkapi-0.2.1/README.md` & `krrsnkapi-0.3/README.md`

 * *Files identical despite different names*

### Comparing `krrsnkapi-0.2.1/krrsnkapi/krrsnkapi.py` & `krrsnkapi-0.3/krrsnkapi/krrsnkapi.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,7 +71,22 @@
 			self.text = text
 
 			url = f'https://kararasenok.ueuo.com/api/v1/base64/encode/?text={self.text}&apikey={self.apikey}'
 
 			self.response = requests.post(url)
 
 			return self.response.text
+
+class PHPsandbox:
+	def __init__(self, apikey):
+		self.apikey = apikey
+
+	def create_code(self, code):
+		self.code = code
+
+		self.code = self.code.replace("\n", " ")
+
+		url = f'https://kararasenok.ueuo.com/api/v1/runphpscript/?apikey={self.apikey}$code={self.code}'
+
+		self.response = requests.post(url)
+
+		return self.response.text
```

### Comparing `krrsnkapi-0.2.1/krrsnkapi.egg-info/PKG-INFO` & `krrsnkapi-0.3/krrsnkapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: krrsnkapi
-Version: 0.2.1
-Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok_gd/krrsnkapi
-Home-page: https://github.com/kararasenok_gd/krrsnkapi
-Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.2.tar.gz
+Version: 0.3
+Summary: Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi
+Home-page: https://github.com/kararasenok-gd/krrsnkapi
+Download-URL: https://github.com/kararasenok-gd/krrsnkapi/archive/v0.3.tar.gz
 Author: kararasenok_gd
 Author-email: murzikkurzikpro@gmail.com
 License: MIT
 Keywords: api
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
```

### Comparing `krrsnkapi-0.2.1/setup.py` & `krrsnkapi-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup
 
 # ver = input("version: ")
 
 setup(
   name = 'krrsnkapi',         # How you named your package folder (MyLib)
   packages = ['krrsnkapi'],   # Chose the same as "name"
-  version = "0.2.1",      # Start with a small number and increase it with every change you make
+  version = "0.3",      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
-  description = 'Module for easy use of my api | info on GitHub: https://github.com/kararasenok_gd/krrsnkapi',   # Give a short description about your library
+  description = 'Module for easy use of my api | info on GitHub: https://github.com/kararasenok-gd/krrsnkapi',   # Give a short description about your library
   author = 'kararasenok_gd',                   # Type in your name
   author_email = 'murzikkurzikpro@gmail.com',      # Type in your E-Mail
-  url = 'https://github.com/kararasenok_gd/krrsnkapi',   # Provide either the link to your github or to your website
-  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.2.tar.gz',    # I explain this later on
+  url = 'https://github.com/kararasenok-gd/krrsnkapi',   # Provide either the link to your github or to your website
+  download_url = f'https://github.com/kararasenok-gd/krrsnkapi/archive/v0.3.tar.gz',    # I explain this later on
   keywords = ["api"],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests'
       ],
   classifiers=[
-    'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
-    'Intended Audience :: Developers',      # Define that your audience are developers
+    'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3.8'
   ],
 )
```

