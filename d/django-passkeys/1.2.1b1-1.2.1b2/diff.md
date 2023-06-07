# Comparing `tmp/django-passkeys-1.2.1b1.tar.gz` & `tmp/django-passkeys-1.2.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-passkeys-1.2.1b1.tar", last modified: Wed Jun  7 19:28:56 2023, max compression
+gzip compressed data, was "django-passkeys-1.2.1b2.tar", last modified: Wed Jun  7 19:31:12 2023, max compression
```

## Comparing `django-passkeys-1.2.1b1.tar` & `django-passkeys-1.2.1b2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.183152 django-passkeys-1.2.1b1/
--rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.1b1/LICENSE
--rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.1b1/MANIFEST.in
--rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:28:56.182710 django-passkeys-1.2.1b1/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)     5762 2023-06-07 16:55:13.000000 django-passkeys-1.2.1b1/README.md
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.164751 django-passkeys-1.2.1b1/django_passkeys.egg-info/
--rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:28:56.000000 django-passkeys-1.2.1b1/django_passkeys.egg-info/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 19:28:56.000000 django-passkeys-1.2.1b1/django_passkeys.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 19:28:56.000000 django-passkeys-1.2.1b1/django_passkeys.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.1b1/django_passkeys.egg-info/not-zip-safe
--rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 19:28:56.000000 django-passkeys-1.2.1b1/django_passkeys.egg-info/requires.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 19:28:56.000000 django-passkeys-1.2.1b1/django_passkeys.egg-info/top_level.txt
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.171172 django-passkeys-1.2.1b1/passkeys/
--rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b1/passkeys/FIDO2.py
--rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b1/passkeys/backend.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.173468 django-passkeys-1.2.1b1/passkeys/migrations/
--rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/migrations/0001_initial.py
--rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/migrations/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/models.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.159114 django-passkeys-1.2.1b1/passkeys/static/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.159632 django-passkeys-1.2.1b1/passkeys/static/passkeys/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.173968 django-passkeys-1.2.1b1/passkeys/static/passkeys/css/
--rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.175353 django-passkeys-1.2.1b1/passkeys/static/passkeys/imgs/
--rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.178295 django-passkeys-1.2.1b1/passkeys/static/passkeys/js/
--rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/static/passkeys/js/base64url.js
--rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/static/passkeys/js/helpers.js
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:28:56.181618 django-passkeys-1.2.1b1/passkeys/templates/
--rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b1/passkeys/templates/PassKeys.html
--rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/templates/PassKeys_base.html
--rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.1b1/passkeys/templates/check_passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b1/passkeys/templates/modal.html
--rw-r--r--   0 mohamed    (501) admin       (80)     2407 2023-06-07 19:28:43.000000 django-passkeys-1.2.1b1/passkeys/templates/passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.1b1/passkeys/urls.py
--rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.1b1/passkeys/views.py
--rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 19:28:56.183333 django-passkeys-1.2.1b1/setup.cfg
--rw-r--r--   0 mohamed    (501) admin       (80)     1813 2023-06-07 19:28:43.000000 django-passkeys-1.2.1b1/setup.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.194549 django-passkeys-1.2.1b2/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.1b2/LICENSE
+-rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.1b2/MANIFEST.in
+-rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:31:12.194120 django-passkeys-1.2.1b2/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)     5762 2023-06-07 16:55:13.000000 django-passkeys-1.2.1b2/README.md
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.160683 django-passkeys-1.2.1b2/django_passkeys.egg-info/
+-rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:31:12.000000 django-passkeys-1.2.1b2/django_passkeys.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 19:31:12.000000 django-passkeys-1.2.1b2/django_passkeys.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 19:31:12.000000 django-passkeys-1.2.1b2/django_passkeys.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.1b2/django_passkeys.egg-info/not-zip-safe
+-rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 19:31:12.000000 django-passkeys-1.2.1b2/django_passkeys.egg-info/requires.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 19:31:12.000000 django-passkeys-1.2.1b2/django_passkeys.egg-info/top_level.txt
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.174085 django-passkeys-1.2.1b2/passkeys/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b2/passkeys/FIDO2.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b2/passkeys/backend.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.178084 django-passkeys-1.2.1b2/passkeys/migrations/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/migrations/0001_initial.py
+-rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/migrations/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/models.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.134941 django-passkeys-1.2.1b2/passkeys/static/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.136968 django-passkeys-1.2.1b2/passkeys/static/passkeys/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.179511 django-passkeys-1.2.1b2/passkeys/static/passkeys/css/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.181226 django-passkeys-1.2.1b2/passkeys/static/passkeys/imgs/
+-rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.186866 django-passkeys-1.2.1b2/passkeys/static/passkeys/js/
+-rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/static/passkeys/js/base64url.js
+-rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/static/passkeys/js/helpers.js
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:31:12.193045 django-passkeys-1.2.1b2/passkeys/templates/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b2/passkeys/templates/PassKeys.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/templates/PassKeys_base.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.1b2/passkeys/templates/check_passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b2/passkeys/templates/modal.html
+-rw-r--r--   0 mohamed    (501) admin       (80)     2458 2023-06-07 19:30:51.000000 django-passkeys-1.2.1b2/passkeys/templates/passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.1b2/passkeys/urls.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.1b2/passkeys/views.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 19:31:12.194724 django-passkeys-1.2.1b2/setup.cfg
+-rw-r--r--   0 mohamed    (501) admin       (80)     1813 2023-06-07 19:31:03.000000 django-passkeys-1.2.1b2/setup.py
```

### Comparing `django-passkeys-1.2.1b1/LICENSE` & `django-passkeys-1.2.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/PKG-INFO` & `django-passkeys-1.2.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.1b1
+Version: 1.2.1b2
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b1 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b2 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
```

### Comparing `django-passkeys-1.2.1b1/README.md` & `django-passkeys-1.2.1b2/README.md`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.2.1b2/django_passkeys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.1b1
+Version: 1.2.1b2
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b1 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b2 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
```

### Comparing `django-passkeys-1.2.1b1/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.2.1b2/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/FIDO2.py` & `django-passkeys-1.2.1b2/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/backend.py` & `django-passkeys-1.2.1b2/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/migrations/0001_initial.py` & `django-passkeys-1.2.1b2/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/models.py` & `django-passkeys-1.2.1b2/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.2.1b2/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.2.1b2/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.2.1b2/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.2.1b2/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.2.1b2/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/templates/PassKeys.html` & `django-passkeys-1.2.1b2/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/templates/check_passkeys.js` & `django-passkeys-1.2.1b2/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/templates/modal.html` & `django-passkeys-1.2.1b2/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/templates/passkeys.js` & `django-passkeys-1.2.1b2/passkeys/templates/passkeys.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -29,14 +29,15 @@
         allowCred.id = base64url.decode(allowCred.id);
     }
 
     return getAssert
 }
 
 function authn(form) {
+    window.conditionUIAbortSignal.abort();
     window.loginForm = form;
     fetch('{% url '
         passkeys: auth_begin ' %}', {
             method: 'GET',
         }).then(function(response) {
         if (response.ok) {
             return response.json().then(function(req) {
```

### Comparing `django-passkeys-1.2.1b1/passkeys/urls.py` & `django-passkeys-1.2.1b2/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/passkeys/views.py` & `django-passkeys-1.2.1b2/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b1/setup.py` & `django-passkeys-1.2.1b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.2.1b1',
+    version='1.2.1b2',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
```

