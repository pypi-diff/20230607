# Comparing `tmp/django-all-in-one-accessibility-1.1.tar.gz` & `tmp/django-all-in-one-accessibility-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-all-in-one-accessibility-1.1.tar", last modified: Wed Jun  7 11:54:57 2023, max compression
+gzip compressed data, was "django-all-in-one-accessibility-1.2.tar", last modified: Wed Jun  7 12:02:59 2023, max compression
```

## Comparing `django-all-in-one-accessibility-1.1.tar` & `django-all-in-one-accessibility-1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.284154 django-all-in-one-accessibility-1.1/
--rw-rw-rw-   0        0        0     3989 2023-06-07 11:54:57.284154 django-all-in-one-accessibility-1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2868 2023-06-07 11:25:43.000000 django-all-in-one-accessibility-1.1/README.rst
--rw-rw-rw-   0        0        0     2874 2023-06-07 09:42:07.000000 django-all-in-one-accessibility-1.1/Readme.md
-drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.263211 django-all-in-one-accessibility-1.1/accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/__init__.py
--rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.1/accessibility/admin.py
--rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/apps.py
--rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.1/accessibility/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.265206 django-all-in-one-accessibility-1.1/accessibility/migrations/
--rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.1/accessibility/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/migrations/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.1/accessibility/models.py
--rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/tests.py
--rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.1/accessibility/urls.py
--rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.1/accessibility/views.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.280166 django-all-in-one-accessibility-1.1/aioa_accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/__init__.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/asgi.py
--rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/settings.py
--rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/urls.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.284154 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/
--rw-rw-rw-   0        0        0     3989 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-06-07 11:54:49.000000 django-all-in-one-accessibility-1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1032 2023-06-07 11:54:57.285152 django-all-in-one-accessibility-1.1/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.175747 django-all-in-one-accessibility-1.2/
+-rw-rw-rw-   0        0        0     3991 2023-06-07 12:02:59.175747 django-all-in-one-accessibility-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2868 2023-06-07 11:25:43.000000 django-all-in-one-accessibility-1.2/README.rst
+-rw-rw-rw-   0        0        0     2876 2023-06-07 12:02:46.000000 django-all-in-one-accessibility-1.2/Readme.md
+drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.148577 django-all-in-one-accessibility-1.2/accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.2/accessibility/admin.py
+-rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/apps.py
+-rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.2/accessibility/context_processors.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.150570 django-all-in-one-accessibility-1.2/accessibility/migrations/
+-rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.2/accessibility/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.2/accessibility/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.2/accessibility/tests.py
+-rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.2/accessibility/urls.py
+-rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.2/accessibility/views.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.165770 django-all-in-one-accessibility-1.2/aioa_accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/asgi.py
+-rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/settings.py
+-rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/urls.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.2/aioa_accessibility/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-07 12:02:59.174747 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/
+-rw-rw-rw-   0        0        0     3991 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-06-07 12:02:59.000000 django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-06-07 12:01:08.000000 django-all-in-one-accessibility-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1032 2023-06-07 12:02:59.176743 django-all-in-one-accessibility-1.2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.2/setup.py
```

### Comparing `django-all-in-one-accessibility-1.1/PKG-INFO` & `django-all-in-one-accessibility-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.1
+Version: 1.2
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,42 +32,42 @@
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
 
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.0`
+-   Run `pip install django-all-in-one-accessibility==1.2`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
 
 ## Usage
 
 ### Settings.INSTALLED_APPS
-Just add accessibility in to your setting.INSTALLED_APPS:
+Just add `accessibility` in to your setting.INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'accessibility',
 ]
 ```
 
 ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your setting.TEMPLATES:
+Just add `accessibility.context_processors.admin_AIOA` in your setting.TEMPLATES:
 ```python
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [],
         'APP_DIRS': True,
         'OPTIONS': {
@@ -76,15 +76,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-Just add this tag in your base.html footer(your main template of django website) '<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>':
+Just add this tag in your base.html footer(your main template of django website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.1
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.2
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -23,30 +23,30 @@
 interface which handles UI and design related adjustments. All in One
 Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
 watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.0` - Add
+Installation - Run `pip install django-all-in-one-accessibility==1.2` - Add
 `accessibility` in `settings.INSTALLED_APPS` - Add
 `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
 context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
-### Settings.INSTALLED_APPS Just add accessibility in to your
+### Settings.INSTALLED_APPS Just add `accessibility` in to your
 setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
 'django.contrib.auth', 'django.contrib.contenttypes',
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your
+Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
-website) '
-': ```python
+website) `
+`: ```python
   ``` ### Migrate Migrate your app Restart your app with this command ```python
 python manage.py migrate ``` ### Restart Restart your app server with this
 command and check the admin panel the model is ready to use ```python python
 manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.1/README.rst` & `django-all-in-one-accessibility-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/Readme.md` & `django-all-in-one-accessibility-1.2/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,42 +8,42 @@
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
 
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.0`
+-   Run `pip install django-all-in-one-accessibility==1.2`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
 
 ## Usage
 
 ### Settings.INSTALLED_APPS
-Just add accessibility in to your setting.INSTALLED_APPS:
+Just add `accessibility` in to your setting.INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'accessibility',
 ]
 ```
 
 ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your setting.TEMPLATES:
+Just add `accessibility.context_processors.admin_AIOA` in your setting.TEMPLATES:
 ```python
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [],
         'APP_DIRS': True,
         'OPTIONS': {
@@ -52,15 +52,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-Just add this tag in your base.html footer(your main template of django website) '<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>':
+Just add this tag in your base.html footer(your main template of django website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -8,30 +8,30 @@
 accessibility interface which handles UI and design related adjustments. All in
 One Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
 watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.0` - Add
+Installation - Run `pip install django-all-in-one-accessibility==1.2` - Add
 `accessibility` in `settings.INSTALLED_APPS` - Add
 `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
 context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
-### Settings.INSTALLED_APPS Just add accessibility in to your
+### Settings.INSTALLED_APPS Just add `accessibility` in to your
 setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
 'django.contrib.auth', 'django.contrib.contenttypes',
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your
+Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
-website) '
-': ```python
+website) `
+`: ```python
   ``` ### Migrate Migrate your app Restart your app with this command ```python
 python manage.py migrate ``` ### Restart Restart your app server with this
 command and check the admin panel the model is ready to use ```python python
 manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.1/accessibility/admin.py` & `django-all-in-one-accessibility-1.2/accessibility/admin.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/accessibility/context_processors.py` & `django-all-in-one-accessibility-1.2/accessibility/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/accessibility/migrations/0001_initial.py` & `django-all-in-one-accessibility-1.2/accessibility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/accessibility/models.py` & `django-all-in-one-accessibility-1.2/accessibility/models.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/aioa_accessibility/settings.py` & `django-all-in-one-accessibility-1.2/aioa_accessibility/settings.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/aioa_accessibility/urls.py` & `django-all-in-one-accessibility-1.2/aioa_accessibility/urls.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/PKG-INFO` & `django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-all-in-one-accessibility
-Version: 1.1
+Version: 1.2
 Summary: All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: Skynet Technologies USA LLC <developer3@skynettechnologies.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,42 +32,42 @@
 It uses the accessibility interface which handles UI and design related adjustments. All in One Accessibility app enhances your Django website accessibility to people with hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive & learning impairments, seizure and epileptic, and ADHD problems. It uses the accessibility interface which handles UI and design related adjustments.
 
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget .
 
 ---
 
 ## Installation
--   Run `pip install django-all-in-one-accessibility==1.0`
+-   Run `pip install django-all-in-one-accessibility==1.2`
 -   Add `accessibility` in `settings.INSTALLED_APPS`
 -   Add `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES context_processors`
 -   Add `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`put this line in your base.html footer
 -   Run `python manage.py migrate`
 -   Run `python manage.py runserver` for Restart your application server
 
 ---
 
 ## Usage
 
 ### Settings.INSTALLED_APPS
-Just add accessibility in to your setting.INSTALLED_APPS:
+Just add `accessibility` in to your setting.INSTALLED_APPS:
 
 ```python
 INSTALLED_APPS = [
     'django.contrib.admin',
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'accessibility',
 ]
 ```
 
 ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your setting.TEMPLATES:
+Just add `accessibility.context_processors.admin_AIOA` in your setting.TEMPLATES:
 ```python
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [],
         'APP_DIRS': True,
         'OPTIONS': {
@@ -76,15 +76,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-Just add this tag in your base.html footer(your main template of django website) '<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>':
+Just add this tag in your base.html footer(your main template of django website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.1
+Metadata-Version: 2.1 Name: django-all-in-one-accessibility Version: 1.2
 Summary: All in One Accessibility widget makes it easy for users to customize
 their experience in a single click tap or press of a button Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 Skynet Technologies USA LLC
 skynettechnologies.com> Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
@@ -23,30 +23,30 @@
 interface which handles UI and design related adjustments. All in One
 Accessibility app enhances your Django website accessibility to people with
 hearing or vision impairments, motor impaired, color blind, dyslexia, cognitive
 & learning impairments, seizure and epileptic, and ADHD problems. It uses the
 accessibility interface which handles UI and design related adjustments.
 [`django-all-in-one-accessibility-introduction`](https://www.youtube.com/
 watch?v=PPQMWSzroAA) - introduction of All in One Accessibility widget . --- ##
-Installation - Run `pip install django-all-in-one-accessibility==1.0` - Add
+Installation - Run `pip install django-all-in-one-accessibility==1.2` - Add
 `accessibility` in `settings.INSTALLED_APPS` - Add
 `accessibility.context_processors.admin_AIOA` in `settings.TEMPLATES
 context_processors` - Add `
 `put this line in your base.html footer - Run `python manage.py migrate` - Run
 `python manage.py runserver` for Restart your application server --- ## Usage
-### Settings.INSTALLED_APPS Just add accessibility in to your
+### Settings.INSTALLED_APPS Just add `accessibility` in to your
 setting.INSTALLED_APPS: ```python INSTALLED_APPS = [ 'django.contrib.admin',
 'django.contrib.auth', 'django.contrib.contenttypes',
 'django.contrib.sessions', 'django.contrib.messages',
 'django.contrib.staticfiles', 'accessibility', ] ``` ### Settings.TEMPLATES
-Just add 'accessibility.context_processors.admin_AIOA' in your
+Just add `accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'accessibility.context_processors.admin_AIOA', ], }, }, ] ``` ### Base.html
 Just add this tag in your base.html footer(your main template of django
-website) '
-': ```python
+website) `
+`: ```python
   ``` ### Migrate Migrate your app Restart your app with this command ```python
 python manage.py migrate ``` ### Restart Restart your app server with this
 command and check the admin panel the model is ready to use ```python python
 manage.py runserver ```
```

### Comparing `django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/SOURCES.txt` & `django-all-in-one-accessibility-1.2/django_all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.1/pyproject.toml` & `django-all-in-one-accessibility-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-all-in-one-accessibility"
-version = "1.1"
+version = "1.2"
 authors = [
   { name="Skynet Technologies USA LLC", email="developer3@skynettechnologies.com" },
 ]
 description = "All in One Accessibility widget makes it easy for users to customize their experience in a single click tap or press of a button"
 readme = "Readme.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `django-all-in-one-accessibility-1.1/setup.cfg` & `django-all-in-one-accessibility-1.2/setup.cfg`

 * *Files identical despite different names*

