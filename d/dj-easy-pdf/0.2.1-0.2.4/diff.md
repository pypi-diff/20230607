# Comparing `tmp/dj-easy-pdf-0.2.1.tar.gz` & `tmp/dj-easy-pdf-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-easy-pdf-0.2.1.tar", last modified: Wed Jun 15 22:36:33 2022, max compression
+gzip compressed data, was "dj-easy-pdf-0.2.4.tar", last modified: Wed Jun  7 20:29:36 2023, max compression
```

## Comparing `dj-easy-pdf-0.2.1.tar` & `dj-easy-pdf-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2022-06-15 22:36:33.358243 dj-easy-pdf-0.2.1/
--rw-r--r--   0 william   (1000) william   (1000)      143 2022-06-15 21:37:19.000000 dj-easy-pdf-0.2.1/AUTHORS.rst
--rw-r--r--   0 william   (1000) william   (1000)     1094 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/LICENSE
--rw-r--r--   0 william   (1000) william   (1000)      169 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/MANIFEST.in
--rw-r--r--   0 william   (1000) william   (1000)     1149 2022-06-15 22:36:33.358243 dj-easy-pdf-0.2.1/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)      294 2022-06-15 22:35:42.000000 dj-easy-pdf-0.2.1/README.rst
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2022-06-15 22:36:33.358243 dj-easy-pdf-0.2.1/dj_easy_pdf.egg-info/
--rw-r--r--   0 william   (1000) william   (1000)     1149 2022-06-15 22:36:32.000000 dj-easy-pdf-0.2.1/dj_easy_pdf.egg-info/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)      445 2022-06-15 22:36:33.000000 dj-easy-pdf-0.2.1/dj_easy_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 william   (1000) william   (1000)        1 2022-06-15 22:36:32.000000 dj-easy-pdf-0.2.1/dj_easy_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 william   (1000) william   (1000)        1 2022-06-15 22:36:31.000000 dj-easy-pdf-0.2.1/dj_easy_pdf.egg-info/not-zip-safe
--rw-r--r--   0 william   (1000) william   (1000)       40 2022-06-15 22:36:33.000000 dj-easy-pdf-0.2.1/dj_easy_pdf.egg-info/requires.txt
--rw-r--r--   0 william   (1000) william   (1000)        9 2022-06-15 22:36:33.000000 dj-easy-pdf-0.2.1/dj_easy_pdf.egg-info/top_level.txt
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2022-06-15 22:36:33.358243 dj-easy-pdf-0.2.1/easy_pdf/
--rw-r--r--   0 william   (1000) william   (1000)       95 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/easy_pdf/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)      106 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/easy_pdf/apps.py
--rw-r--r--   0 william   (1000) william   (1000)      583 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/easy_pdf/exceptions.py
--rw-r--r--   0 william   (1000) william   (1000)       15 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/easy_pdf/models.py
--rw-r--r--   0 william   (1000) william   (1000)     5558 2022-06-15 21:53:53.000000 dj-easy-pdf-0.2.1/easy_pdf/rendering.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2022-06-15 22:36:33.358243 dj-easy-pdf-0.2.1/easy_pdf/templates/
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2022-06-15 22:36:33.358243 dj-easy-pdf-0.2.1/easy_pdf/templates/easy_pdf/
--rw-r--r--   0 william   (1000) william   (1000)     1606 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/easy_pdf/templates/easy_pdf/base.html
--rw-r--r--   0 william   (1000) william   (1000)     1213 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/easy_pdf/tests.py
--rw-r--r--   0 william   (1000) william   (1000)     2341 2022-06-15 21:31:40.000000 dj-easy-pdf-0.2.1/easy_pdf/views.py
--rw-r--r--   0 william   (1000) william   (1000)      306 2022-06-15 22:36:33.358243 dj-easy-pdf-0.2.1/setup.cfg
--rw-r--r--   0 william   (1000) william   (1000)     1593 2022-06-15 22:33:16.000000 dj-easy-pdf-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.763068 dj-easy-pdf-0.2.4/easy_pdf/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/easy_pdf/templates/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/templates/easy_pdf/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 20:29:36.771068 dj-easy-pdf-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/tests/tests.py
```

### Comparing `dj-easy-pdf-0.2.1/LICENSE` & `dj-easy-pdf-0.2.4/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2014 Filip Wasilewski <en@ig.ma>
+Copyright (c) 2022 William Otieno <jimmywilliamotieno@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `dj-easy-pdf-0.2.1/easy_pdf/exceptions.py` & `dj-easy-pdf-0.2.4/easy_pdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.1/easy_pdf/rendering.py` & `dj-easy-pdf-0.2.4/easy_pdf/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,9 +153,9 @@
     :param using: Optional Django template engine
     :rtype: :class:`django.http.HttpResponse`
     """
     try:
         pdf = render_to_pdf(template, context, using=using, encoding=encoding, **kwargs)
         return make_response(pdf, filename)
     except PDFRenderingError as e:
-        logger.exception(e.message)
-        return HttpResponse(e.message)
+        logger.exception(e)
+        return HttpResponse(e)
```

### Comparing `dj-easy-pdf-0.2.1/easy_pdf/templates/easy_pdf/base.html` & `dj-easy-pdf-0.2.4/easy_pdf/templates/easy_pdf/base.html`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.1/easy_pdf/tests.py` & `dj-easy-pdf-0.2.4/easy_pdf/tests.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.1/easy_pdf/views.py` & `dj-easy-pdf-0.2.4/easy_pdf/views.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.1/setup.py` & `dj-easy-pdf-0.2.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.2.1"
+version = "0.2.4"
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel upload")
     print("You probably want to also tag the version now:")
     print("  git tag -a %s -m 'version %s'" % (version, version))
     print("  git push --tags")
     sys.exit()
@@ -37,15 +37,15 @@
         "django>=3.2",
         "xhtml2pdf>=0.2",
         "reportlab>=3"
     ],
     zip_safe=False,
     keywords="dj-easy-pdf",
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
```

