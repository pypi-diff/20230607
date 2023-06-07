# Comparing `tmp/aad-token-verify-0.1.4.tar.gz` & `tmp/aad-token-verify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aad-token-verify-0.1.4.tar", last modified: Fri Oct 29 15:46:53 2021, max compression
+gzip compressed data, was "aad-token-verify-0.2.0.tar", last modified: Wed Jun  7 15:38:31 2023, max compression
```

## Comparing `aad-token-verify-0.1.4.tar` & `aad-token-verify-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 15:46:53.129679 aad-token-verify-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-10-29 15:46:44.000000 aad-token-verify-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-10-29 15:46:44.000000 aad-token-verify-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2021-10-29 15:46:53.129679 aad-token-verify-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2021-10-29 15:46:44.000000 aad-token-verify-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 15:46:53.129679 aad-token-verify-0.1.4/aad_token_verify/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-10-29 15:46:44.000000 aad-token-verify-0.1.4/aad_token_verify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2021-10-29 15:46:44.000000 aad-token-verify-0.1.4/aad_token_verify/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2021-10-29 15:46:44.000000 aad-token-verify-0.1.4/aad_token_verify/token_verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 15:46:53.129679 aad-token-verify-0.1.4/aad_token_verify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2021-10-29 15:46:53.000000 aad-token-verify-0.1.4/aad_token_verify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      342 2021-10-29 15:46:53.000000 aad-token-verify-0.1.4/aad_token_verify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-29 15:46:53.000000 aad-token-verify-0.1.4/aad_token_verify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-29 15:46:53.000000 aad-token-verify-0.1.4/aad_token_verify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-29 15:46:53.000000 aad-token-verify-0.1.4/aad_token_verify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      181 2021-10-29 15:46:53.129679 aad-token-verify-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-10-29 15:46:44.000000 aad-token-verify-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:38:31.252236 aad-token-verify-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-07 15:38:31.252236 aad-token-verify-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:38:31.252236 aad-token-verify-0.2.0/aad_token_verify/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/aad_token_verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/aad_token_verify/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/aad_token_verify/token_verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:38:31.252236 aad-token-verify-0.2.0/aad_token_verify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-07 15:38:31.000000 aad-token-verify-0.2.0/aad_token_verify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-07 15:38:31.000000 aad-token-verify-0.2.0/aad_token_verify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:38:31.000000 aad-token-verify-0.2.0/aad_token_verify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-07 15:38:31.000000 aad-token-verify-0.2.0/aad_token_verify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 15:38:31.000000 aad-token-verify-0.2.0/aad_token_verify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 15:38:31.252236 aad-token-verify-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:38:31.252236 aad-token-verify-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 15:38:24.000000 aad-token-verify-0.2.0/tests/test_token_verifier.py
```

### Comparing `aad-token-verify-0.1.4/LICENSE` & `aad-token-verify-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aad-token-verify-0.1.4/PKG-INFO` & `aad-token-verify-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: aad-token-verify
-Version: 0.1.4
+Version: 0.2.0
 Summary: A python utility library to verify an Azure Active Directory OAuth token
 Home-page: https://github.com/GeneralMills/azure-ad-token-verify
 Author: ['Daniel Thompson']
 Author-email: daniel.thompson2@genmills.com 
 License: MIT
 Keywords: azure ad token oauth verify jwt
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/GeneralMills/azure-ad-token-verify/workflows/Test%20and%20Analysis/badge.svg)](https://github.com/GeneralMills/azure-ad-token-verify/actions)
 [![PyPi](https://img.shields.io/pypi/pyversions/aad-token-verify.svg)](https://pypi.python.org/pypi/aad-token-verify)
 # aad-token-verify
 A python utility library to verify an Azure Active Directory OAuth token. Meant for resource servers serving secured API endpoints (eg FastAPI)
@@ -100,9 +99,7 @@
 async def secured_endpoint(user=Depends(get_current_user)):
     return user
 ```
 
 ## Contributing
 
 Feel free to submit issues and pull requests!
-
-
```

### Comparing `aad-token-verify-0.1.4/README.md` & `aad-token-verify-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aad-token-verify-0.1.4/aad_token_verify/token_verifier.py` & `aad-token-verify-0.2.0/aad_token_verify/token_verifier.py`

 * *Files identical despite different names*

### Comparing `aad-token-verify-0.1.4/aad_token_verify.egg-info/PKG-INFO` & `aad-token-verify-0.2.0/aad_token_verify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: aad-token-verify
-Version: 0.1.4
+Version: 0.2.0
 Summary: A python utility library to verify an Azure Active Directory OAuth token
 Home-page: https://github.com/GeneralMills/azure-ad-token-verify
 Author: ['Daniel Thompson']
 Author-email: daniel.thompson2@genmills.com 
 License: MIT
 Keywords: azure ad token oauth verify jwt
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/GeneralMills/azure-ad-token-verify/workflows/Test%20and%20Analysis/badge.svg)](https://github.com/GeneralMills/azure-ad-token-verify/actions)
 [![PyPi](https://img.shields.io/pypi/pyversions/aad-token-verify.svg)](https://pypi.python.org/pypi/aad-token-verify)
 # aad-token-verify
 A python utility library to verify an Azure Active Directory OAuth token. Meant for resource servers serving secured API endpoints (eg FastAPI)
@@ -100,9 +99,7 @@
 async def secured_endpoint(user=Depends(get_current_user)):
     return user
 ```
 
 ## Contributing
 
 Feel free to submit issues and pull requests!
-
-
```

### Comparing `aad-token-verify-0.1.4/setup.py` & `aad-token-verify-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 dir = os.path.dirname(__file__)
 
 with io.open(os.path.join(dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='aad-token-verify',
-    version='0.1.4',
+    version='0.2.0',
     description='A python utility library to verify an Azure Active Directory OAuth token',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/GeneralMills/azure-ad-token-verify',
     author=['Daniel Thompson'],
     author_email='daniel.thompson2@genmills.com ',
     license='MIT',
@@ -24,17 +24,17 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'License :: OSI Approved :: MIT License',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=[
         'requests>=2.25.1,<3',
         'PyJWT>=2.1.0,<3',
-        'cryptography>=3.3.2<4',
-        'cachetools>=4.2.2,<5'
+        'cryptography>=41.0.1,<42',
+        'cachetools>=5.3.1,<6'
     ],
     keywords='azure ad token oauth verify jwt',
     packages=['aad_token_verify'],
 )
```

