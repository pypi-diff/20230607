# Comparing `tmp/django-passkeys-1.2.1b8.tar.gz` & `tmp/django-passkeys-1.2.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-passkeys-1.2.1b8.tar", last modified: Wed Jun  7 20:12:52 2023, max compression
+gzip compressed data, was "django-passkeys-1.2.1b9.tar", last modified: Wed Jun  7 20:20:07 2023, max compression
```

## Comparing `django-passkeys-1.2.1b8.tar` & `django-passkeys-1.2.1b9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.651517 django-passkeys-1.2.1b8/
--rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.1b8/LICENSE
--rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.1b8/MANIFEST.in
--rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 20:12:52.650922 django-passkeys-1.2.1b8/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)     5762 2023-06-07 16:55:13.000000 django-passkeys-1.2.1b8/README.md
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.634504 django-passkeys-1.2.1b8/django_passkeys.egg-info/
--rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 20:12:52.000000 django-passkeys-1.2.1b8/django_passkeys.egg-info/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 20:12:52.000000 django-passkeys-1.2.1b8/django_passkeys.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 20:12:52.000000 django-passkeys-1.2.1b8/django_passkeys.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.1b8/django_passkeys.egg-info/not-zip-safe
--rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 20:12:52.000000 django-passkeys-1.2.1b8/django_passkeys.egg-info/requires.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 20:12:52.000000 django-passkeys-1.2.1b8/django_passkeys.egg-info/top_level.txt
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.638644 django-passkeys-1.2.1b8/passkeys/
--rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b8/passkeys/FIDO2.py
--rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b8/passkeys/backend.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.640856 django-passkeys-1.2.1b8/passkeys/migrations/
--rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/migrations/0001_initial.py
--rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/migrations/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/models.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.628597 django-passkeys-1.2.1b8/passkeys/static/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.629033 django-passkeys-1.2.1b8/passkeys/static/passkeys/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.641240 django-passkeys-1.2.1b8/passkeys/static/passkeys/css/
--rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.642056 django-passkeys-1.2.1b8/passkeys/static/passkeys/imgs/
--rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.645974 django-passkeys-1.2.1b8/passkeys/static/passkeys/js/
--rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/static/passkeys/js/base64url.js
--rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/static/passkeys/js/helpers.js
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:12:52.649780 django-passkeys-1.2.1b8/passkeys/templates/
--rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b8/passkeys/templates/PassKeys.html
--rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/templates/PassKeys_base.html
--rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.1b8/passkeys/templates/check_passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b8/passkeys/templates/modal.html
--rw-r--r--   0 mohamed    (501) admin       (80)     2598 2023-06-07 20:12:37.000000 django-passkeys-1.2.1b8/passkeys/templates/passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.1b8/passkeys/urls.py
--rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.1b8/passkeys/views.py
--rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 20:12:52.651705 django-passkeys-1.2.1b8/setup.cfg
--rw-r--r--   0 mohamed    (501) admin       (80)     1813 2023-06-07 20:10:40.000000 django-passkeys-1.2.1b8/setup.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.342942 django-passkeys-1.2.1b9/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.1b9/LICENSE
+-rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.1b9/MANIFEST.in
+-rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 20:20:07.342456 django-passkeys-1.2.1b9/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)     5762 2023-06-07 16:55:13.000000 django-passkeys-1.2.1b9/README.md
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.324040 django-passkeys-1.2.1b9/django_passkeys.egg-info/
+-rw-r--r--   0 mohamed    (501) admin       (80)     7128 2023-06-07 20:20:07.000000 django-passkeys-1.2.1b9/django_passkeys.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 20:20:07.000000 django-passkeys-1.2.1b9/django_passkeys.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 20:20:07.000000 django-passkeys-1.2.1b9/django_passkeys.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.1b9/django_passkeys.egg-info/not-zip-safe
+-rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 20:20:07.000000 django-passkeys-1.2.1b9/django_passkeys.egg-info/requires.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 20:20:07.000000 django-passkeys-1.2.1b9/django_passkeys.egg-info/top_level.txt
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.328957 django-passkeys-1.2.1b9/passkeys/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b9/passkeys/FIDO2.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b9/passkeys/backend.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.332981 django-passkeys-1.2.1b9/passkeys/migrations/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/migrations/0001_initial.py
+-rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/migrations/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/models.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.318498 django-passkeys-1.2.1b9/passkeys/static/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.319071 django-passkeys-1.2.1b9/passkeys/static/passkeys/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.333642 django-passkeys-1.2.1b9/passkeys/static/passkeys/css/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.334464 django-passkeys-1.2.1b9/passkeys/static/passkeys/imgs/
+-rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.337258 django-passkeys-1.2.1b9/passkeys/static/passkeys/js/
+-rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/static/passkeys/js/base64url.js
+-rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/static/passkeys/js/helpers.js
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 20:20:07.341392 django-passkeys-1.2.1b9/passkeys/templates/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.1b9/passkeys/templates/PassKeys.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/templates/PassKeys_base.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.1b9/passkeys/templates/check_passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.1b9/passkeys/templates/modal.html
+-rw-r--r--   0 mohamed    (501) admin       (80)     2615 2023-06-07 20:19:42.000000 django-passkeys-1.2.1b9/passkeys/templates/passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.1b9/passkeys/urls.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.1b9/passkeys/views.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 20:20:07.343142 django-passkeys-1.2.1b9/setup.cfg
+-rw-r--r--   0 mohamed    (501) admin       (80)     1813 2023-06-07 20:19:47.000000 django-passkeys-1.2.1b9/setup.py
```

### Comparing `django-passkeys-1.2.1b8/LICENSE` & `django-passkeys-1.2.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/PKG-INFO` & `django-passkeys-1.2.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.1b8
+Version: 1.2.1b9
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
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b8 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b9 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
```

### Comparing `django-passkeys-1.2.1b8/README.md` & `django-passkeys-1.2.1b9/README.md`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.2.1b9/django_passkeys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.1b8
+Version: 1.2.1b9
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
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b8 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.1b9 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
 Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
```

### Comparing `django-passkeys-1.2.1b8/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.2.1b9/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/FIDO2.py` & `django-passkeys-1.2.1b9/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/backend.py` & `django-passkeys-1.2.1b9/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/migrations/0001_initial.py` & `django-passkeys-1.2.1b9/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/models.py` & `django-passkeys-1.2.1b9/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.2.1b9/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.2.1b9/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.2.1b9/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.2.1b9/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.2.1b9/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/templates/PassKeys.html` & `django-passkeys-1.2.1b9/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/templates/check_passkeys.js` & `django-passkeys-1.2.1b9/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/templates/modal.html` & `django-passkeys-1.2.1b9/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/templates/passkeys.js` & `django-passkeys-1.2.1b9/passkeys/templates/passkeys.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
 
 function checkConditionalUI(form) {
     if (window.PublicKeyCredential && PublicKeyCredential.isConditionalMediationAvailable) {
         // Check if conditional mediation is available.
         PublicKeyCredential.isConditionalMediationAvailable().then((result) => {
             window.conditionalUI = result;
             if (window.conditionalUI) {
-                pk_login(form)
+                pk_login(form, true)
             }
         });
     }
 }
 
 var GetAssertReq = (getAssert) => {
     getAssert.publicKey.challenge = base64url.decode(getAssert.publicKey.challenge);
@@ -30,31 +30,32 @@
     }
 
     return getAssert
 }
 
 function authn(form) {
     window.conditionUIAbortController.abort();
-    pk_login(form);
+    pk_login(form, false);
 }
+s
 
-function pk_login(form) {
+function pk_login(form, conditional) {
     window.loginForm = form;
     fetch('{% url '
         passkeys: auth_begin ' %}', {
             method: 'GET',
         }).then(function(response) {
         if (response.ok) {
             return response.json().then(function(req) {
                 return GetAssertReq(req)
             });
         }
         throw new Error('No credential available to authenticate!');
     }).then(function(options) {
-        if (window.conditionalUI) {
+        if (conditionalUI) {
             options.mediation = 'conditional';
             options.signal = conditionUIAbortSignal;
         }
         console.log(options)
         return navigator.credentials.get(options);
     }).then(function(assertion) {
         pk = $("#passkeys")
```

### Comparing `django-passkeys-1.2.1b8/passkeys/urls.py` & `django-passkeys-1.2.1b9/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/passkeys/views.py` & `django-passkeys-1.2.1b9/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.1b8/setup.py` & `django-passkeys-1.2.1b9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.2.1b8',
+    version='1.2.1b9',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
```

