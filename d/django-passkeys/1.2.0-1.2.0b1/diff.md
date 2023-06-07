# Comparing `tmp/django-passkeys-1.2.0.tar.gz` & `tmp/django-passkeys-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-passkeys-1.2.0.tar", last modified: Wed Jun  7 16:54:02 2023, max compression
+gzip compressed data, was "django-passkeys-1.2.0b1.tar", last modified: Wed Jun  7 16:15:38 2023, max compression
```

## Comparing `django-passkeys-1.2.0.tar` & `django-passkeys-1.2.0b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.323593 django-passkeys-1.2.0/
--rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.0/LICENSE
--rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.0/MANIFEST.in
--rw-r--r--   0 mohamed    (501) admin       (80)     7139 2023-06-07 16:54:02.322819 django-passkeys-1.2.0/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)     5762 2023-06-07 16:52:58.000000 django-passkeys-1.2.0/README.md
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.302991 django-passkeys-1.2.0/django_passkeys.egg-info/
--rw-r--r--   0 mohamed    (501) admin       (80)     7139 2023-06-07 16:54:02.000000 django-passkeys-1.2.0/django_passkeys.egg-info/PKG-INFO
--rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 16:54:02.000000 django-passkeys-1.2.0/django_passkeys.egg-info/SOURCES.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 16:54:02.000000 django-passkeys-1.2.0/django_passkeys.egg-info/dependency_links.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.0/django_passkeys.egg-info/not-zip-safe
--rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 16:54:02.000000 django-passkeys-1.2.0/django_passkeys.egg-info/requires.txt
--rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 16:54:02.000000 django-passkeys-1.2.0/django_passkeys.egg-info/top_level.txt
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.307602 django-passkeys-1.2.0/passkeys/
--rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.0/passkeys/FIDO2.py
--rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.0/passkeys/backend.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.309899 django-passkeys-1.2.0/passkeys/migrations/
--rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/migrations/0001_initial.py
--rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/migrations/__init__.py
--rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/models.py
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.296326 django-passkeys-1.2.0/passkeys/static/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.296824 django-passkeys-1.2.0/passkeys/static/passkeys/
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.310461 django-passkeys-1.2.0/passkeys/static/passkeys/css/
--rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.311273 django-passkeys-1.2.0/passkeys/static/passkeys/imgs/
--rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.314217 django-passkeys-1.2.0/passkeys/static/passkeys/js/
--rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/static/passkeys/js/base64url.js
--rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/static/passkeys/js/helpers.js
-drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:54:02.319971 django-passkeys-1.2.0/passkeys/templates/
--rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.0/passkeys/templates/PassKeys.html
--rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/templates/PassKeys_base.html
--rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.0/passkeys/templates/check_passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.0/passkeys/templates/modal.html
--rw-r--r--   0 mohamed    (501) admin       (80)     2249 2023-06-07 15:58:05.000000 django-passkeys-1.2.0/passkeys/templates/passkeys.js
--rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.0/passkeys/urls.py
--rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.0/passkeys/views.py
--rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 16:54:02.323795 django-passkeys-1.2.0/setup.cfg
--rw-r--r--   0 mohamed    (501) admin       (80)     1811 2023-06-07 16:53:06.000000 django-passkeys-1.2.0/setup.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.081441 django-passkeys-1.2.0b1/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1075 2022-10-28 09:47:43.000000 django-passkeys-1.2.0b1/LICENSE
+-rw-r--r--   0 mohamed    (501) admin       (80)       74 2022-10-28 09:54:08.000000 django-passkeys-1.2.0b1/MANIFEST.in
+-rw-r--r--   0 mohamed    (501) admin       (80)     6928 2023-06-07 16:15:38.079360 django-passkeys-1.2.0b1/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)     5562 2023-06-07 16:14:51.000000 django-passkeys-1.2.0b1/README.md
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.063914 django-passkeys-1.2.0b1/django_passkeys.egg-info/
+-rw-r--r--   0 mohamed    (501) admin       (80)     6928 2023-06-07 16:15:38.000000 django-passkeys-1.2.0b1/django_passkeys.egg-info/PKG-INFO
+-rw-r--r--   0 mohamed    (501) admin       (80)      864 2023-06-07 16:15:38.000000 django-passkeys-1.2.0b1/django_passkeys.egg-info/SOURCES.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2023-06-07 16:15:38.000000 django-passkeys-1.2.0b1/django_passkeys.egg-info/dependency_links.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        1 2022-10-28 09:57:05.000000 django-passkeys-1.2.0b1/django_passkeys.egg-info/not-zip-safe
+-rw-r--r--   0 mohamed    (501) admin       (80)       47 2023-06-07 16:15:38.000000 django-passkeys-1.2.0b1/django_passkeys.egg-info/requires.txt
+-rw-r--r--   0 mohamed    (501) admin       (80)        9 2023-06-07 16:15:38.000000 django-passkeys-1.2.0b1/django_passkeys.egg-info/top_level.txt
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.068107 django-passkeys-1.2.0b1/passkeys/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5661 2023-06-07 15:50:35.000000 django-passkeys-1.2.0b1/passkeys/FIDO2.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       65 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      784 2023-06-07 15:50:35.000000 django-passkeys-1.2.0b1/passkeys/backend.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.069782 django-passkeys-1.2.0b1/passkeys/migrations/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1176 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/migrations/0001_initial.py
+-rw-r--r--   0 mohamed    (501) admin       (80)        0 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/migrations/__init__.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      599 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/models.py
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.056306 django-passkeys-1.2.0b1/passkeys/static/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.056711 django-passkeys-1.2.0b1/passkeys/static/passkeys/
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.070295 django-passkeys-1.2.0b1/passkeys/static/passkeys/css/
+-rw-r--r--   0 mohamed    (501) admin       (80)     1590 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/static/passkeys/css/bootstrap-toggle.min.css
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.071124 django-passkeys-1.2.0b1/passkeys/static/passkeys/imgs/
+-rw-r--r--   0 mohamed    (501) admin       (80)     8981 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.073459 django-passkeys-1.2.0b1/passkeys/static/passkeys/js/
+-rw-r--r--   0 mohamed    (501) admin       (80)     2684 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/static/passkeys/js/base64url.js
+-rw-r--r--   0 mohamed    (501) admin       (80)     4129 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/static/passkeys/js/bootstrap-toggle.min.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      687 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/static/passkeys/js/helpers.js
+drwxr-xr-x   0 mohamed    (501) admin       (80)        0 2023-06-07 16:15:38.077319 django-passkeys-1.2.0b1/passkeys/templates/
+-rw-r--r--   0 mohamed    (501) admin       (80)     5795 2023-06-07 15:50:35.000000 django-passkeys-1.2.0b1/passkeys/templates/PassKeys.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      128 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/templates/PassKeys_base.html
+-rw-r--r--   0 mohamed    (501) admin       (80)      724 2022-10-29 13:23:58.000000 django-passkeys-1.2.0b1/passkeys/templates/check_passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      807 2022-10-29 09:43:43.000000 django-passkeys-1.2.0b1/passkeys/templates/modal.html
+-rw-r--r--   0 mohamed    (501) admin       (80)     2249 2023-06-07 15:58:05.000000 django-passkeys-1.2.0b1/passkeys/templates/passkeys.js
+-rw-r--r--   0 mohamed    (501) admin       (80)      563 2022-10-29 13:32:38.000000 django-passkeys-1.2.0b1/passkeys/urls.py
+-rw-r--r--   0 mohamed    (501) admin       (80)      911 2022-10-29 13:31:50.000000 django-passkeys-1.2.0b1/passkeys/views.py
+-rw-r--r--   0 mohamed    (501) admin       (80)       38 2023-06-07 16:15:38.081704 django-passkeys-1.2.0b1/setup.cfg
+-rw-r--r--   0 mohamed    (501) admin       (80)     1813 2023-06-07 16:15:30.000000 django-passkeys-1.2.0b1/setup.py
```

### Comparing `django-passkeys-1.2.0/LICENSE` & `django-passkeys-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/PKG-INFO` & `django-passkeys-1.2.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.0
+Version: 1.2.0b1
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -147,21 +147,15 @@
 
 ## Using Conditional UI
 
 Conditional UI is a way for the browser to prompt the user to use the passkey to login to the system as shown in 
 
 ![conditionalUI.png](imgs%2FconditionalUI.png)
 
-Starting version v1.2. you can use Conditional UI by adding the following to your login page
-
-1. Add `webauthn` to autocomplete of the username field as shown below.
-```html
-<input name="username" placeholder="username" autocomplete="username webauthn">
-```
-add the following to the page js.
+Starting version 1.2. you can use Conditional UI by adding the following to your login page
 
 ```js
 window.onload = checkConditionalUI('loginForm');
 ```
 where `loginForm` is name of your login form.
 
 ## Security contact information
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.0b1 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
-Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
-:: Web Environment Classifier: Framework :: Django Classifier: Framework ::
-Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework ::
-Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework ::
-Django :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework ::
-Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
-Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python Classifier:
+Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
+Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
+2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
+2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
+3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django ::
+4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django ::
+4.2 Classifier: Intended Audience :: Developers Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE # django-
 passkeys [![PyPI version](https://badge.fury.io/py/django-passkeys.svg)](https:
@@ -70,17 +70,15 @@
  ``` check_passkey function paramters are as follows *
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
 (optional). ## Using Conditional UI Conditional UI is a way for the browser to
 prompt the user to use the passkey to login to the system as shown in !
-[conditionalUI.png](imgs%2FconditionalUI.png) Starting version v1.2. you can
-use Conditional UI by adding the following to your login page 1. Add `webauthn`
-to autocomplete of the username field as shown below. ```html [username
-] ``` add the following to the page js. ```js window.onload =
+[conditionalUI.png](imgs%2FconditionalUI.png) Starting version 1.2. you can use
+Conditional UI by adding the following to your login page ```js window.onload =
 checkConditionalUI('loginForm'); ``` where `loginForm` is name of your login
 form. ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
 (https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
 [gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.2.0/README.md` & `django-passkeys-1.2.0b1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -112,21 +112,15 @@
 
 ## Using Conditional UI
 
 Conditional UI is a way for the browser to prompt the user to use the passkey to login to the system as shown in 
 
 ![conditionalUI.png](imgs%2FconditionalUI.png)
 
-Starting version v1.2. you can use Conditional UI by adding the following to your login page
-
-1. Add `webauthn` to autocomplete of the username field as shown below.
-```html
-<input name="username" placeholder="username" autocomplete="username webauthn">
-```
-add the following to the page js.
+Starting version 1.2. you can use Conditional UI by adding the following to your login page
 
 ```js
 window.onload = checkConditionalUI('loginForm');
 ```
 where `loginForm` is name of your login form.
 
 ## Security contact information
```

#### html2text {}

```diff
@@ -53,17 +53,15 @@
  ``` check_passkey function paramters are as follows *
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
 (optional). ## Using Conditional UI Conditional UI is a way for the browser to
 prompt the user to use the passkey to login to the system as shown in !
-[conditionalUI.png](imgs%2FconditionalUI.png) Starting version v1.2. you can
-use Conditional UI by adding the following to your login page 1. Add `webauthn`
-to autocomplete of the username field as shown below. ```html [username
-] ``` add the following to the page js. ```js window.onload =
+[conditionalUI.png](imgs%2FconditionalUI.png) Starting version 1.2. you can use
+Conditional UI by adding the following to your login page ```js window.onload =
 checkConditionalUI('loginForm'); ``` where `loginForm` is name of your login
 form. ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
 (https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
 [gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.2.0/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.2.0b1/django_passkeys.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.2.0
+Version: 1.2.0b1
 Summary: A Django Authentication Backend for Passkeys
 Home-page: https://github.com/mkalioby/django-passkeys
 Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -147,21 +147,15 @@
 
 ## Using Conditional UI
 
 Conditional UI is a way for the browser to prompt the user to use the passkey to login to the system as shown in 
 
 ![conditionalUI.png](imgs%2FconditionalUI.png)
 
-Starting version v1.2. you can use Conditional UI by adding the following to your login page
-
-1. Add `webauthn` to autocomplete of the username field as shown below.
-```html
-<input name="username" placeholder="username" autocomplete="username webauthn">
-```
-add the following to the page js.
+Starting version 1.2. you can use Conditional UI by adding the following to your login page
 
 ```js
 window.onload = checkConditionalUI('loginForm');
 ```
 where `loginForm` is name of your login form.
 
 ## Security contact information
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.0 Summary: A Django
+Metadata-Version: 2.1 Name: django-passkeys Version: 1.2.0b1 Summary: A Django
 Authentication Backend for Passkeys Home-page: https://github.com/mkalioby/
 django-passkeys Download-URL: https://github.com/mkalioby/django-passkeys
 Author: Mohamed El-Kalioby Author-email: mkalioby@mkalioby.com License: MIT
-Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
-:: Web Environment Classifier: Framework :: Django Classifier: Framework ::
-Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework ::
-Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework ::
-Django :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework ::
-Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework ::
-Django :: 4.2 Classifier: Intended Audience :: Developers Classifier: Operating
-System :: OS Independent Classifier: Programming Language :: Python Classifier:
+Classifier: Development Status :: 4 - Beta Classifier: Environment :: Web
+Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
+2.0 Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django ::
+2.2 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django ::
+3.1 Classifier: Framework :: Django :: 3.2 Classifier: Framework :: Django ::
+4.0 Classifier: Framework :: Django :: 4.1 Classifier: Framework :: Django ::
+4.2 Classifier: Intended Audience :: Developers Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Requires-Python:
 >=3.7 Description-Content-Type: text/markdown License-File: LICENSE # django-
 passkeys [![PyPI version](https://badge.fury.io/py/django-passkeys.svg)](https:
@@ -70,17 +70,15 @@
  ``` check_passkey function paramters are as follows *
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
 (optional). ## Using Conditional UI Conditional UI is a way for the browser to
 prompt the user to use the passkey to login to the system as shown in !
-[conditionalUI.png](imgs%2FconditionalUI.png) Starting version v1.2. you can
-use Conditional UI by adding the following to your login page 1. Add `webauthn`
-to autocomplete of the username field as shown below. ```html [username
-] ``` add the following to the page js. ```js window.onload =
+[conditionalUI.png](imgs%2FconditionalUI.png) Starting version 1.2. you can use
+Conditional UI by adding the following to your login page ```js window.onload =
 checkConditionalUI('loginForm'); ``` where `loginForm` is name of your login
 form. ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
 (https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
 [gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.2.0/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.2.0b1/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/FIDO2.py` & `django-passkeys-1.2.0b1/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/backend.py` & `django-passkeys-1.2.0b1/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/migrations/0001_initial.py` & `django-passkeys-1.2.0b1/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/models.py` & `django-passkeys-1.2.0b1/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/templates/PassKeys.html` & `django-passkeys-1.2.0b1/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/templates/check_passkeys.js` & `django-passkeys-1.2.0b1/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/templates/modal.html` & `django-passkeys-1.2.0b1/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/templates/passkeys.js` & `django-passkeys-1.2.0b1/passkeys/templates/passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/urls.py` & `django-passkeys-1.2.0b1/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/passkeys/views.py` & `django-passkeys-1.2.0b1/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.2.0/setup.py` & `django-passkeys-1.2.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.2.0',
+    version='1.2.0b1',
     description='A Django Authentication Backend for Passkeys',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/django-passkeys',
     download_url='https://github.com/mkalioby/django-passkeys',
@@ -20,16 +20,16 @@
         'user-agents',
         'fido2 == 1.1.1',
       ],
     python_requires=">=3.7",
     include_package_data=True,
     zip_safe=False, # because we're including static files
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        #"Development Status :: 4 - Beta",
+        #"Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Framework :: Django :: 2.0",
         "Framework :: Django :: 2.1",
         "Framework :: Django :: 2.2",
         "Framework :: Django :: 3.0",
         "Framework :: Django :: 3.1",
```

