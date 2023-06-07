# Comparing `tmp/django-passkeys-1.2.1b3.tar.gz` & `tmp/django-passkeys-1.2.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-passkeys-1.2.1b3.tar", last modified: Wed Jun  7 19:39:24 2023, max compression
+gzip compressed data, was "django-passkeys-1.2.1b4.tar", last modified: Wed Jun  7 19:45:42 2023, max compression
```

## Comparing `django-passkeys-1.2.1b3.tar` & `django-passkeys-1.2.1b4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.854774 django-passkeys-1.2.1b3/
--rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.1b3/LICENSE
--rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.1b3/MANIFEST.in
--rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:39:24.854296 django-passkeys-1.2.1b3/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)     5762 2023-06-07 16:55:13.000000 django-passkeys-1.2.1b3/README.md
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.840802 django-passkeys-1.2.1b3/django_passkeys.egg-info/
--rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:39:24.000000 django-passkeys-1.2.1b3/django_passkeys.egg-info/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 19:39:24.000000 django-passkeys-1.2.1b3/django_passkeys.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 19:39:24.000000 django-passkeys-1.2.1b3/django_passkeys.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.1b3/django_passkeys.egg-info/not-zip-safe
--rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 19:39:24.000000 django-passkeys-1.2.1b3/django_passkeys.egg-info/requires.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 19:39:24.000000 django-passkeys-1.2.1b3/django_passkeys.egg-info/top_level.txt
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.845171 django-passkeys-1.2.1b3/passkeys/
--rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b3/passkeys/FIDO2.py
--rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b3/passkeys/backend.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.846839 django-passkeys-1.2.1b3/passkeys/migrations/
--rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/migrations/0001_initial.py
--rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/migrations/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/models.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.833021 django-passkeys-1.2.1b3/passkeys/static/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.833940 django-passkeys-1.2.1b3/passkeys/static/passkeys/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.847308 django-passkeys-1.2.1b3/passkeys/static/passkeys/css/
--rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.847985 django-passkeys-1.2.1b3/passkeys/static/passkeys/imgs/
--rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.850220 django-passkeys-1.2.1b3/passkeys/static/passkeys/js/
--rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/static/passkeys/js/base64url.js
--rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/static/passkeys/js/helpers.js
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:39:24.853535 django-passkeys-1.2.1b3/passkeys/templates/
--rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b3/passkeys/templates/PassKeys.html
--rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/templates/PassKeys_base.html
--rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.1b3/passkeys/templates/check_passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b3/passkeys/templates/modal.html
--rw-r--r--   0 mohamed    (501) admin       (80)     2480 2023-06-07 19:39:10.000000 django-passkeys-1.2.1b3/passkeys/templates/passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.1b3/passkeys/urls.py
--rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.1b3/passkeys/views.py
--rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 19:39:24.855076 django-passkeys-1.2.1b3/setup.cfg
--rw-r--r--   0 mohamed    (501) admin       (80)     1813 2023-06-07 19:39:15.000000 django-passkeys-1.2.1b3/setup.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:42.008316 django-passkeys-1.2.1b4/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.1b4/LICENSE
+-rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.1b4/MANIFEST.in
+-rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:45:42.007409 django-passkeys-1.2.1b4/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)     5762 2023-06-07 16:55:13.000000 django-passkeys-1.2.1b4/README.md
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.934502 django-passkeys-1.2.1b4/django_passkeys.egg-info/
+-rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 19:45:41.000000 django-passkeys-1.2.1b4/django_passkeys.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 19:45:41.000000 django-passkeys-1.2.1b4/django_passkeys.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 19:45:41.000000 django-passkeys-1.2.1b4/django_passkeys.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.1b4/django_passkeys.egg-info/not-zip-safe
+-rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 19:45:41.000000 django-passkeys-1.2.1b4/django_passkeys.egg-info/requires.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 19:45:41.000000 django-passkeys-1.2.1b4/django_passkeys.egg-info/top_level.txt
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.944009 django-passkeys-1.2.1b4/passkeys/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b4/passkeys/FIDO2.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b4/passkeys/backend.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.946386 django-passkeys-1.2.1b4/passkeys/migrations/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/migrations/0001_initial.py
+-rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/migrations/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/models.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.916096 django-passkeys-1.2.1b4/passkeys/static/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.917837 django-passkeys-1.2.1b4/passkeys/static/passkeys/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.947222 django-passkeys-1.2.1b4/passkeys/static/passkeys/css/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.948334 django-passkeys-1.2.1b4/passkeys/static/passkeys/imgs/
+-rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:41.951529 django-passkeys-1.2.1b4/passkeys/static/passkeys/js/
+-rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/static/passkeys/js/base64url.js
+-rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/static/passkeys/js/helpers.js
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 19:45:42.006085 django-passkeys-1.2.1b4/passkeys/templates/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b4/passkeys/templates/PassKeys.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/templates/PassKeys_base.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.1b4/passkeys/templates/check_passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b4/passkeys/templates/modal.html
+-rw-r--r--   0 mohamed    (501) admin       (80)     2491 2023-06-07 19:45:24.000000 django-passkeys-1.2.1b4/passkeys/templates/passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.1b4/passkeys/urls.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.1b4/passkeys/views.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 19:45:42.008528 django-passkeys-1.2.1b4/setup.cfg
+-rw-r--r--   0 mohamed    (501) admin       (80)     1813 2023-06-07 19:45:30.000000 django-passkeys-1.2.1b4/setup.py
```

### Comparing `django-passkeys-1.2.1b3/LICENSE` & `django-passkeys-1.2.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/PKG-INFO` & `django-passkeys-1.2.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.1b3
+Version: 1.2.1b4
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
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b3 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b4 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
```

### Comparing `django-passkeys-1.2.1b3/README.md` & `django-passkeys-1.2.1b4/README.md`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.2.1b4/django_passkeys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.1b3
+Version: 1.2.1b4
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
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b3 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b4 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
```

### Comparing `django-passkeys-1.2.1b3/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.2.1b4/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/FIDO2.py` & `django-passkeys-1.2.1b4/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/backend.py` & `django-passkeys-1.2.1b4/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/migrations/0001_initial.py` & `django-passkeys-1.2.1b4/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/models.py` & `django-passkeys-1.2.1b4/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.2.1b4/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.2.1b4/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.2.1b4/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.2.1b4/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.2.1b4/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/templates/PassKeys.html` & `django-passkeys-1.2.1b4/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/templates/check_passkeys.js` & `django-passkeys-1.2.1b4/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/templates/modal.html` & `django-passkeys-1.2.1b4/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/templates/passkeys.js` & `django-passkeys-1.2.1b4/passkeys/templates/passkeys.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
 script type = "application/javascript"
 src = "{% static 'passkeys/js/base64url.js' %}" > < /script> <
     script type = "application/javascript"
 src = "{% static 'passkeys/js/helpers.js' %}" > < /script> <
     script type = "text/javascript" >
     window.conditionalUI = false;
 window.conditionUIAbortController = new AbortController();
-window.conditionUIAbortSignal = abortController.signal;
+window.conditionUIAbortSignal = conditionUIAbortController.signal;
 
 function checkConditionalUI(form) {
     if (window.PublicKeyCredential && PublicKeyCredential.isConditionalMediationAvailable) {
         // Check if conditional mediation is available.
         PublicKeyCredential.isConditionalMediationAvailable().then((result) => {
             window.conditionalUI = result;
             if (window.conditionalUI) {
```

### Comparing `django-passkeys-1.2.1b3/passkeys/urls.py` & `django-passkeys-1.2.1b4/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/passkeys/views.py` & `django-passkeys-1.2.1b4/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b3/setup.py` & `django-passkeys-1.2.1b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.2.1b3',
+    version='1.2.1b4',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
```

