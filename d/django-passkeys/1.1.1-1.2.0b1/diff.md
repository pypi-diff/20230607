# Comparing `tmp/django-passkeys-1.1.1.tar.gz` & `tmp/django-passkeys-1.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-passkeys-1.1.1.tar", last modified: Wed May 24 14:33:34 2023, max compression
+gzip compressed data, was "django-passkeys-1.2.0b1.tar", last modified: Wed Jun  7 16:15:38 2023, max compression
```

## Comparing `django-passkeys-1.1.1.tar` & `django-passkeys-1.2.0b1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       74 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/MANIFEST.in
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6551 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5174 2023-05-23 14:13:48.000000 django-passkeys-1.1.1/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/django_passkeys.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6551 2023-05-24 14:33:34.000000 django-passkeys-1.1.1/django_passkeys.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      864 2023-05-24 14:33:34.000000 django-passkeys-1.1.1/django_passkeys.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-24 14:33:34.000000 django-passkeys-1.1.1/django_passkeys.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-04-09 09:42:26.000000 django-passkeys-1.1.1/django_passkeys.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       47 2023-05-24 14:33:34.000000 django-passkeys-1.1.1/django_passkeys.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        9 2023-05-24 14:33:34.000000 django-passkeys-1.1.1/django_passkeys.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/passkeys/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5661 2023-05-23 13:57:16.000000 django-passkeys-1.1.1/passkeys/FIDO2.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       65 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      784 2023-05-24 14:33:10.000000 django-passkeys-1.1.1/passkeys/backend.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/passkeys/migrations/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1176 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/migrations/0001_initial.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/migrations/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      599 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/models.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.924010 django-passkeys-1.1.1/passkeys/static/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.924010 django-passkeys-1.1.1/passkeys/static/passkeys/
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/passkeys/static/passkeys/css/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1590 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/static/passkeys/css/bootstrap-toggle.min.css
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/passkeys/static/passkeys/imgs/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     8981 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/passkeys/static/passkeys/js/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     2684 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/static/passkeys/js/base64url.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4129 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/static/passkeys/js/bootstrap-toggle.min.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      687 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/static/passkeys/js/helpers.js
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/passkeys/templates/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     5795 2023-05-23 13:57:16.000000 django-passkeys-1.1.1/passkeys/templates/PassKeys.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      128 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/templates/PassKeys_base.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      724 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/templates/check_passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      807 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/templates/modal.html
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1769 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/templates/passkeys.js
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      563 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      911 2023-04-09 08:41:37.000000 django-passkeys-1.1.1/passkeys/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-24 14:33:34.928010 django-passkeys-1.1.1/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1811 2023-05-24 14:33:28.000000 django-passkeys-1.1.1/setup.py
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

### Comparing `django-passkeys-1.1.1/LICENSE` & `django-passkeys-1.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/PKG-INFO` & `django-passkeys-1.2.0b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.1.1
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
@@ -72,15 +72,15 @@
 4. Add the following settings to your file
 
    ```python
     AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
     FIDO_SERVER_ID="localhost"      # Server rp id for FIDO2, it the full domain of your project
     FIDO_SERVER_NAME="TestApp"
     import passkeys
-    KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
+    KEY_ATTACHMENT = None | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
    ```
    **Note**: Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be a callable to support multi-tenants web applications, the `request` is passed to the called function.
 5. Add passkeys to urls.py
    ```python 
 
    urls_patterns= [
    '...',
@@ -119,14 +119,15 @@
 ```
 `cross_platform`: means that the user used a key from another platform so there is no key local to the device used to login e.g used an Android phone on Mac OS X or iPad.
 If the user didn't use a passkey then it will be set to False
 ```python
 {'passkey':False}
 ```
 
+
 # Check if the user can be enrolled for a platform authenticator
 
 If you want to check if the user can be enrolled to use a platform authenticator, you can do the following in your main page.
 
 ```html
 <div id="pk" class="alert alert-info" style="display: none">Your device supports passkeys, <a href="{%url 'passkeys:enroll'%}">Enroll</a> </div>
 <script type="text/javascript">
@@ -140,14 +141,27 @@
 ```
 check_passkey function paramters are as follows 
 * `platform_authenticator`: if the service requires only a platform authenticator (e.g TouchID, Windows Hello or Android SafetyNet)
 * `success_func`: function to call if a platform authenticator is found or if the user didn't login by a passkey
 * `fail_func`: function to call if no platform authenticator is found (optional).
 
 
+## Using Conditional UI
+
+Conditional UI is a way for the browser to prompt the user to use the passkey to login to the system as shown in 
+
+![conditionalUI.png](imgs%2FconditionalUI.png)
+
+Starting version 1.2. you can use Conditional UI by adding the following to your login page
+
+```js
+window.onload = checkConditionalUI('loginForm');
+```
+where `loginForm` is name of your login form.
+
 ## Security contact information
 
 To report a security vulnerability, please use the
 [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure.
 
 # Contributors
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.1.1 Summary: A Django
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
@@ -31,15 +31,15 @@
 django-passkeys` Currently, it support Django 2.0+, Python 3.7+ # Usage 1. in
 your settings.py add the application to your installed apps ```python
 INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect Static Files
 `python manage.py collectstatic` 3. Run migrate `python manage.py migrate` 4.
 Add the following settings to your file ```python AUTHENTICATION_BACKENDS =
 ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
 FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
-project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = NONE |
+project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = None |
 passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` **Note**:
 Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be a callable to
 support multi-tenants web applications, the `request` is passed to the called
 function. 5. Add passkeys to urls.py ```python urls_patterns= [ '...', url
 (r'^passkeys/', include('passkeys.urls')), '....', ] ``` 6. To match the look
 and feel of your project, Passkeys includes `base.html` but it needs blocks
 named `head` & `content` to added its content to it. **Notes:** 1. You can
@@ -68,12 +68,17 @@
 platform authenticator, you can do the following in your main page. ```html
 Your device supports passkeys, Enroll
  ``` check_passkey function paramters are as follows *
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
-(optional). ## Security contact information To report a security vulnerability,
+(optional). ## Using Conditional UI Conditional UI is a way for the browser to
+prompt the user to use the passkey to login to the system as shown in !
+[conditionalUI.png](imgs%2FconditionalUI.png) Starting version 1.2. you can use
+Conditional UI by adding the following to your login page ```js window.onload =
+checkConditionalUI('loginForm'); ``` where `loginForm` is name of your login
+form. ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
 (https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
 [gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.1.1/README.md` & `django-passkeys-1.2.0b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 4. Add the following settings to your file
 
    ```python
     AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
     FIDO_SERVER_ID="localhost"      # Server rp id for FIDO2, it the full domain of your project
     FIDO_SERVER_NAME="TestApp"
     import passkeys
-    KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
+    KEY_ATTACHMENT = None | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
    ```
    **Note**: Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be a callable to support multi-tenants web applications, the `request` is passed to the called function.
 5. Add passkeys to urls.py
    ```python 
 
    urls_patterns= [
    '...',
@@ -84,14 +84,15 @@
 ```
 `cross_platform`: means that the user used a key from another platform so there is no key local to the device used to login e.g used an Android phone on Mac OS X or iPad.
 If the user didn't use a passkey then it will be set to False
 ```python
 {'passkey':False}
 ```
 
+
 # Check if the user can be enrolled for a platform authenticator
 
 If you want to check if the user can be enrolled to use a platform authenticator, you can do the following in your main page.
 
 ```html
 <div id="pk" class="alert alert-info" style="display: none">Your device supports passkeys, <a href="{%url 'passkeys:enroll'%}">Enroll</a> </div>
 <script type="text/javascript">
@@ -105,14 +106,27 @@
 ```
 check_passkey function paramters are as follows 
 * `platform_authenticator`: if the service requires only a platform authenticator (e.g TouchID, Windows Hello or Android SafetyNet)
 * `success_func`: function to call if a platform authenticator is found or if the user didn't login by a passkey
 * `fail_func`: function to call if no platform authenticator is found (optional).
 
 
+## Using Conditional UI
+
+Conditional UI is a way for the browser to prompt the user to use the passkey to login to the system as shown in 
+
+![conditionalUI.png](imgs%2FconditionalUI.png)
+
+Starting version 1.2. you can use Conditional UI by adding the following to your login page
+
+```js
+window.onload = checkConditionalUI('loginForm');
+```
+where `loginForm` is name of your login form.
+
 ## Security contact information
 
 To report a security vulnerability, please use the
 [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure.
 
 # Contributors
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 Usage 1. in your settings.py add the application to your installed apps
 ```python INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect
 Static Files `python manage.py collectstatic` 3. Run migrate `python manage.py
 migrate` 4. Add the following settings to your file ```python
 AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change
 your authentication backend FIDO_SERVER_ID="localhost" # Server rp id for
 FIDO2, it the full domain of your project FIDO_SERVER_NAME="TestApp" import
-passkeys KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM |
+passkeys KEY_ATTACHMENT = None | passkeys.Attachment.CROSS_PLATFORM |
 passkeys.Attachment.PLATFORM ``` **Note**: Starting v1.1, `FIDO_SERVER_ID` and/
 or `FIDO_SERVER_NAME` can be a callable to support multi-tenants web
 applications, the `request` is passed to the called function. 5. Add passkeys
 to urls.py ```python urls_patterns= [ '...', url(r'^passkeys/', include
 ('passkeys.urls')), '....', ] ``` 6. To match the look and feel of your
 project, Passkeys includes `base.html` but it needs blocks named `head` &
 `content` to added its content to it. **Notes:** 1. You can override
@@ -51,12 +51,17 @@
 platform authenticator, you can do the following in your main page. ```html
 Your device supports passkeys, Enroll
  ``` check_passkey function paramters are as follows *
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
-(optional). ## Security contact information To report a security vulnerability,
+(optional). ## Using Conditional UI Conditional UI is a way for the browser to
+prompt the user to use the passkey to login to the system as shown in !
+[conditionalUI.png](imgs%2FconditionalUI.png) Starting version 1.2. you can use
+Conditional UI by adding the following to your login page ```js window.onload =
+checkConditionalUI('loginForm'); ``` where `loginForm` is name of your login
+form. ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
 (https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
 [gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.1.1/django_passkeys.egg-info/PKG-INFO` & `django-passkeys-1.2.0b1/django_passkeys.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-passkeys
-Version: 1.1.1
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
@@ -72,15 +72,15 @@
 4. Add the following settings to your file
 
    ```python
     AUTHENTICATION_BACKENDS = ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
     FIDO_SERVER_ID="localhost"      # Server rp id for FIDO2, it the full domain of your project
     FIDO_SERVER_NAME="TestApp"
     import passkeys
-    KEY_ATTACHMENT = NONE | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
+    KEY_ATTACHMENT = None | passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM
    ```
    **Note**: Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be a callable to support multi-tenants web applications, the `request` is passed to the called function.
 5. Add passkeys to urls.py
    ```python 
 
    urls_patterns= [
    '...',
@@ -119,14 +119,15 @@
 ```
 `cross_platform`: means that the user used a key from another platform so there is no key local to the device used to login e.g used an Android phone on Mac OS X or iPad.
 If the user didn't use a passkey then it will be set to False
 ```python
 {'passkey':False}
 ```
 
+
 # Check if the user can be enrolled for a platform authenticator
 
 If you want to check if the user can be enrolled to use a platform authenticator, you can do the following in your main page.
 
 ```html
 <div id="pk" class="alert alert-info" style="display: none">Your device supports passkeys, <a href="{%url 'passkeys:enroll'%}">Enroll</a> </div>
 <script type="text/javascript">
@@ -140,14 +141,27 @@
 ```
 check_passkey function paramters are as follows 
 * `platform_authenticator`: if the service requires only a platform authenticator (e.g TouchID, Windows Hello or Android SafetyNet)
 * `success_func`: function to call if a platform authenticator is found or if the user didn't login by a passkey
 * `fail_func`: function to call if no platform authenticator is found (optional).
 
 
+## Using Conditional UI
+
+Conditional UI is a way for the browser to prompt the user to use the passkey to login to the system as shown in 
+
+![conditionalUI.png](imgs%2FconditionalUI.png)
+
+Starting version 1.2. you can use Conditional UI by adding the following to your login page
+
+```js
+window.onload = checkConditionalUI('loginForm');
+```
+where `loginForm` is name of your login form.
+
 ## Security contact information
 
 To report a security vulnerability, please use the
 [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure.
 
 # Contributors
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: django-passkeys Version: 1.1.1 Summary: A Django
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
@@ -31,15 +31,15 @@
 django-passkeys` Currently, it support Django 2.0+, Python 3.7+ # Usage 1. in
 your settings.py add the application to your installed apps ```python
 INSTALLED_APPS=( '......', 'passkeys', '......') ``` 2. Collect Static Files
 `python manage.py collectstatic` 3. Run migrate `python manage.py migrate` 4.
 Add the following settings to your file ```python AUTHENTICATION_BACKENDS =
 ['passkeys.backend.PasskeyModelBackend'] # Change your authentication backend
 FIDO_SERVER_ID="localhost" # Server rp id for FIDO2, it the full domain of your
-project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = NONE |
+project FIDO_SERVER_NAME="TestApp" import passkeys KEY_ATTACHMENT = None |
 passkeys.Attachment.CROSS_PLATFORM | passkeys.Attachment.PLATFORM ``` **Note**:
 Starting v1.1, `FIDO_SERVER_ID` and/or `FIDO_SERVER_NAME` can be a callable to
 support multi-tenants web applications, the `request` is passed to the called
 function. 5. Add passkeys to urls.py ```python urls_patterns= [ '...', url
 (r'^passkeys/', include('passkeys.urls')), '....', ] ``` 6. To match the look
 and feel of your project, Passkeys includes `base.html` but it needs blocks
 named `head` & `content` to added its content to it. **Notes:** 1. You can
@@ -68,12 +68,17 @@
 platform authenticator, you can do the following in your main page. ```html
 Your device supports passkeys, Enroll
  ``` check_passkey function paramters are as follows *
 `platform_authenticator`: if the service requires only a platform authenticator
 (e.g TouchID, Windows Hello or Android SafetyNet) * `success_func`: function to
 call if a platform authenticator is found or if the user didn't login by a
 passkey * `fail_func`: function to call if no platform authenticator is found
-(optional). ## Security contact information To report a security vulnerability,
+(optional). ## Using Conditional UI Conditional UI is a way for the browser to
+prompt the user to use the passkey to login to the system as shown in !
+[conditionalUI.png](imgs%2FconditionalUI.png) Starting version 1.2. you can use
+Conditional UI by adding the following to your login page ```js window.onload =
+checkConditionalUI('loginForm'); ``` where `loginForm` is name of your login
+form. ## Security contact information To report a security vulnerability,
 please use the [Tidelift security contact](https://tidelift.com/security).
 Tidelift will coordinate the fix and disclosure. # Contributors * [mahmoodnasr]
 (https://github.com/mahmoodnasr) * [jacopsd](https://github.com/jacopsd) *
 [gasparbrogueira](https://github.com/gasparbrogueira)
```

### Comparing `django-passkeys-1.1.1/django_passkeys.egg-info/SOURCES.txt` & `django-passkeys-1.2.0b1/django_passkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/FIDO2.py` & `django-passkeys-1.2.0b1/passkeys/FIDO2.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/backend.py` & `django-passkeys-1.2.0b1/passkeys/backend.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/migrations/0001_initial.py` & `django-passkeys-1.2.0b1/passkeys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/models.py` & `django-passkeys-1.2.0b1/passkeys/models.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/static/passkeys/css/bootstrap-toggle.min.css` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/css/bootstrap-toggle.min.css`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/imgs/FIDO-Passkey_Icon-White.png`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/static/passkeys/js/base64url.js` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/js/base64url.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/static/passkeys/js/bootstrap-toggle.min.js` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/js/bootstrap-toggle.min.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/static/passkeys/js/helpers.js` & `django-passkeys-1.2.0b1/passkeys/static/passkeys/js/helpers.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/templates/PassKeys.html` & `django-passkeys-1.2.0b1/passkeys/templates/PassKeys.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/templates/check_passkeys.js` & `django-passkeys-1.2.0b1/passkeys/templates/check_passkeys.js`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/templates/modal.html` & `django-passkeys-1.2.0b1/passkeys/templates/modal.html`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/templates/passkeys.js` & `django-passkeys-1.2.0b1/passkeys/templates/passkeys.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -2,37 +2,54 @@
     % load static %
 } <
 script type = "application/javascript"
 src = "{% static 'passkeys/js/base64url.js' %}" > < /script> <
     script type = "application/javascript"
 src = "{% static 'passkeys/js/helpers.js' %}" > < /script> <
     script type = "text/javascript" >
-    var GetAssertReq = (getAssert) => {
-        getAssert.publicKey.challenge = base64url.decode(getAssert.publicKey.challenge);
+    window.conditionalUI = false;
 
-        for (let allowCred of getAssert.publicKey.allowCredentials) {
-            allowCred.id = base64url.decode(allowCred.id);
-        }
+function checkConditionalUI(form) {
+    if (window.PublicKeyCredential && PublicKeyCredential.isConditionalMediationAvailable) {
+        // Check if conditional mediation is available.
+        PublicKeyCredential.isConditionalMediationAvailable().then((result) => {
+            window.conditionalUI = result;
+            if (window.conditionalUI) {
+                authn(form)
+            }
+        });
+    }
+}
+
+var GetAssertReq = (getAssert) => {
+    getAssert.publicKey.challenge = base64url.decode(getAssert.publicKey.challenge);
 
-        return getAssert
+    for (let allowCred of getAssert.publicKey.allowCredentials) {
+        allowCred.id = base64url.decode(allowCred.id);
     }
 
+    return getAssert
+}
+
 function authn(form) {
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
+        if (window.conditionalUI) {
+            options.mediation = 'conditional';
+        }
         console.log(options)
         return navigator.credentials.get(options);
     }).then(function(assertion) {
         pk = $("#passkeys")
         if (pk.length == 0) {
             console.error("Did you add the 'passkeys' hidden input field")
             return
```

### Comparing `django-passkeys-1.1.1/passkeys/urls.py` & `django-passkeys-1.2.0b1/passkeys/urls.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/passkeys/views.py` & `django-passkeys-1.2.0b1/passkeys/views.py`

 * *Files identical despite different names*

### Comparing `django-passkeys-1.1.1/setup.py` & `django-passkeys-1.2.0b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='django-passkeys',
-    version='1.1.1',
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

