# Comparing `tmp/auth-token-django-0.0.1.tar.gz` & `tmp/auth-token-django-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth-token-django-0.0.1.tar", last modified: Wed Jun  7 15:15:34 2023, max compression
+gzip compressed data, was "auth-token-django-0.0.2.tar", last modified: Wed Jun  7 15:33:52 2023, max compression
```

## Comparing `auth-token-django-0.0.1.tar` & `auth-token-django-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.584598 auth-token-django-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-07 15:15:34.584598 auth-token-django-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/auth_token_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-07 15:15:34.000000 auth-token-django-0.0.1/auth_token_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-07 15:15:34.000000 auth-token-django-0.0.1/auth_token_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 15:15:34.000000 auth-token-django-0.0.1/auth_token_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-07 15:15:34.000000 auth-token-django-0.0.1/auth_token_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-07 15:15:34.000000 auth-token-django-0.0.1/auth_token_django.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/djangoauthtoken/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/djangoauthtoken/middleware/
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/middleware/token_authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/djangoauthtoken/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/djangoauthtoken/models/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/models/base_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/djangoauthtoken/models/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/models/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/models/token.py
--rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/models/token_user.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/djangoauthtoken/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/serializers/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.580597 auth-token-django-0.0.1/djangoauthtoken/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/utils/csrf_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/utils/datetime_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:15:34.584598 auth-token-django-0.0.1/djangoauthtoken/views/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/views/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/views/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/views/sign_up.py
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/views/user.py
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/djangoauthtoken/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 15:15:34.584598 auth-token-django-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-07 15:15:22.000000 auth-token-django-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/auth_token_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1320 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-07 15:33:52.000000 auth-token-django-0.0.2/auth_token_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/middleware/
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2024 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/middleware/token_authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     6688 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.201058 auth-token-django-0.0.2/djangoauthtoken/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/base_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/models/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/custom_fields/case_insensitive_email_field.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1228 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (122)      807 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/models/token_user.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/serializers/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3792 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/utils/csrf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/utils/datetime_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/djangoauthtoken/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/sign_up.py
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/views/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/djangoauthtoken/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 15:33:52.205059 auth-token-django-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-07 15:33:43.000000 auth-token-django-0.0.2/setup.py
```

### Comparing `auth-token-django-0.0.1/PKG-INFO` & `auth-token-django-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.0.1/README.md` & `auth-token-django-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/auth_token_django.egg-info/PKG-INFO` & `auth-token-django-0.0.2/auth_token_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auth-token-django
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django token authentication
 Home-page: https://github.com/Shivin01/django_auth_token
 Author: Shivin Agarwal
 Author-email: shivin.agarwal15@gmail.com
 Keywords: django auth token
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `auth-token-django-0.0.1/auth_token_django.egg-info/SOURCES.txt` & `auth-token-django-0.0.2/auth_token_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/auth_token_django.egg-info/requires.txt` & `auth-token-django-0.0.2/auth_token_django.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -23,10 +23,10 @@
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.4.1
 six==1.16.0
 sqlparse==0.4.4
 twine==4.0.2
 typing_extensions==4.6.2
-urllib3==2.0.3
+urllib3<2.0
 webencodings==0.5.1
 zipp==3.15.0
```

### Comparing `auth-token-django-0.0.1/djangoauthtoken/middleware/token_authentication.py` & `auth-token-django-0.0.2/djangoauthtoken/middleware/token_authentication.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/migrations/0001_initial.py` & `auth-token-django-0.0.2/djangoauthtoken/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/models/token.py` & `auth-token-django-0.0.2/djangoauthtoken/models/token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/models/token_user.py` & `auth-token-django-0.0.2/djangoauthtoken/models/token_user.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/settings.py` & `auth-token-django-0.0.2/djangoauthtoken/settings.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/urls.py` & `auth-token-django-0.0.2/djangoauthtoken/urls.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/views/login.py` & `auth-token-django-0.0.2/djangoauthtoken/views/login.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/views/refresh_token.py` & `auth-token-django-0.0.2/djangoauthtoken/views/refresh_token.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/djangoauthtoken/views/sign_up.py` & `auth-token-django-0.0.2/djangoauthtoken/views/sign_up.py`

 * *Files identical despite different names*

### Comparing `auth-token-django-0.0.1/setup.py` & `auth-token-django-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             install_requires.append(line)
     return install_requires
 
 
 setup(
     name='auth-token-django',
     description='Django token authentication',
-    version = "0.0.1",
+    version = "0.0.2",
     author='Shivin Agarwal',
     long_description=get_file_contents('README.md'),
     author_email='shivin.agarwal15@gmail.com',
     url='https://github.com/Shivin01/django_auth_token',
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
```

