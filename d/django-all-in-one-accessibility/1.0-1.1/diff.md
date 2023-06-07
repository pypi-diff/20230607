# Comparing `tmp/django-all-in-one-accessibility-1.0.tar.gz` & `tmp/django-all-in-one-accessibility-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-all-in-one-accessibility-1.0.tar", last modified: Wed Jun  7 05:59:41 2023, max compression
+gzip compressed data, was "django-all-in-one-accessibility-1.1.tar", last modified: Wed Jun  7 11:54:57 2023, max compression
```

## Comparing `django-all-in-one-accessibility-1.0.tar` & `django-all-in-one-accessibility-1.1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 05:59:41.806290 django-all-in-one-accessibility-1.0/
--rw-rw-rw-   0        0        0     1282 2023-06-07 05:59:41.806290 django-all-in-one-accessibility-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      800 2023-06-07 05:38:32.000000 django-all-in-one-accessibility-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-07 05:59:41.797346 django-all-in-one-accessibility-1.0/accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.0/accessibility/__init__.py
--rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.0/accessibility/admin.py
--rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.0/accessibility/apps.py
--rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.0/accessibility/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:59:41.798562 django-all-in-one-accessibility-1.0/accessibility/migrations/
--rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.0/accessibility/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.0/accessibility/migrations/__init__.py
--rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.0/accessibility/models.py
--rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.0/accessibility/tests.py
--rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.0/accessibility/urls.py
--rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.0/accessibility/views.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:59:41.802297 django-all-in-one-accessibility-1.0/aioa_accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.0/aioa_accessibility/__init__.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.0/aioa_accessibility/asgi.py
--rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.0/aioa_accessibility/settings.py
--rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.0/aioa_accessibility/urls.py
--rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.0/aioa_accessibility/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-06-07 05:59:41.806290 django-all-in-one-accessibility-1.0/django_all_in_one_accessibility.egg-info/
--rw-rw-rw-   0        0        0     1282 2023-06-07 05:59:41.000000 django-all-in-one-accessibility-1.0/django_all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      738 2023-06-07 05:59:41.000000 django-all-in-one-accessibility-1.0/django_all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 05:59:41.000000 django-all-in-one-accessibility-1.0/django_all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 05:59:41.000000 django-all-in-one-accessibility-1.0/django_all_in_one_accessibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-07 05:59:41.000000 django-all-in-one-accessibility-1.0/django_all_in_one_accessibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      508 2023-06-07 05:58:24.000000 django-all-in-one-accessibility-1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1032 2023-06-07 05:59:41.809285 django-all-in-one-accessibility-1.0/setup.cfg
--rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.284154 django-all-in-one-accessibility-1.1/
+-rw-rw-rw-   0        0        0     3989 2023-06-07 11:54:57.284154 django-all-in-one-accessibility-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2868 2023-06-07 11:25:43.000000 django-all-in-one-accessibility-1.1/README.rst
+-rw-rw-rw-   0        0        0     2874 2023-06-07 09:42:07.000000 django-all-in-one-accessibility-1.1/Readme.md
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.263211 django-all-in-one-accessibility-1.1/accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-06-06 10:53:45.000000 django-all-in-one-accessibility-1.1/accessibility/admin.py
+-rw-rw-rw-   0        0        0      106 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/apps.py
+-rw-rw-rw-   0        0        0      527 2023-06-06 10:58:34.000000 django-all-in-one-accessibility-1.1/accessibility/context_processors.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.265206 django-all-in-one-accessibility-1.1/accessibility/migrations/
+-rw-rw-rw-   0        0        0     2019 2023-06-06 10:39:45.000000 django-all-in-one-accessibility-1.1/accessibility/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1922 2023-06-06 10:38:52.000000 django-all-in-one-accessibility-1.1/accessibility/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-06 10:32:03.000000 django-all-in-one-accessibility-1.1/accessibility/tests.py
+-rw-rw-rw-   0        0        0      162 2023-06-06 10:33:50.000000 django-all-in-one-accessibility-1.1/accessibility/urls.py
+-rw-rw-rw-   0        0        0      239 2023-06-06 10:34:08.000000 django-all-in-one-accessibility-1.1/accessibility/views.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.280166 django-all-in-one-accessibility-1.1/aioa_accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/__init__.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/asgi.py
+-rw-rw-rw-   0        0        0     3349 2023-06-06 10:43:35.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/settings.py
+-rw-rw-rw-   0        0        0      834 2023-06-06 10:32:54.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/urls.py
+-rw-rw-rw-   0        0        0      429 2023-06-06 10:30:59.000000 django-all-in-one-accessibility-1.1/aioa_accessibility/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:57.284154 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/
+-rw-rw-rw-   0        0        0     3989 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-06-07 11:54:57.000000 django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-06-07 11:54:49.000000 django-all-in-one-accessibility-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1032 2023-06-07 11:54:57.285152 django-all-in-one-accessibility-1.1/setup.cfg
+-rw-rw-rw-   0        0        0       37 2023-06-07 04:23:51.000000 django-all-in-one-accessibility-1.1/setup.py
```

### Comparing `django-all-in-one-accessibility-1.0/accessibility/admin.py` & `django-all-in-one-accessibility-1.1/accessibility/admin.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.0/accessibility/context_processors.py` & `django-all-in-one-accessibility-1.1/accessibility/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.0/accessibility/migrations/0001_initial.py` & `django-all-in-one-accessibility-1.1/accessibility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.0/accessibility/models.py` & `django-all-in-one-accessibility-1.1/accessibility/models.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.0/aioa_accessibility/settings.py` & `django-all-in-one-accessibility-1.1/aioa_accessibility/settings.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.0/aioa_accessibility/urls.py` & `django-all-in-one-accessibility-1.1/aioa_accessibility/urls.py`

 * *Files identical despite different names*

### Comparing `django-all-in-one-accessibility-1.0/django_all_in_one_accessibility.egg-info/SOURCES.txt` & `django-all-in-one-accessibility-1.1/django_all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 README.rst
+Readme.md
 pyproject.toml
 setup.cfg
 setup.py
 accessibility/__init__.py
 accessibility/admin.py
 accessibility/apps.py
 accessibility/context_processors.py
```

### Comparing `django-all-in-one-accessibility-1.0/setup.cfg` & `django-all-in-one-accessibility-1.1/setup.cfg`

 * *Files identical despite different names*

