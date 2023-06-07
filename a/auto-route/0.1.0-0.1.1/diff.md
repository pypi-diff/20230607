# Comparing `tmp/auto_route-0.1.0.tar.gz` & `tmp/auto_route-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_route-0.1.0.tar", last modified: Wed Jun  7 00:01:01 2023, max compression
+gzip compressed data, was "auto_route-0.1.1.tar", last modified: Wed Jun  7 00:14:00 2023, max compression
```

## Comparing `auto_route-0.1.0.tar` & `auto_route-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:01:01.750017 auto_route-0.1.0/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:01:01.750017 auto_route-0.1.0/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4312 2023-05-13 16:21:56.000000 auto_route-0.1.0/README.md
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-06 23:59:56.000000 auto_route-0.1.0/README.rst
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:01:01.750017 auto_route-0.1.0/auto_route/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-05-12 18:05:03.000000 auto_route-0.1.0/auto_route/__init__.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     3701 2023-05-25 21:35:31.000000 auto_route-0.1.0/auto_route/auto_app.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-05-25 21:33:21.000000 auto_route-0.1.0/auto_route/auto_route.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-05-25 16:57:12.000000 auto_route-0.1.0/auto_route/cli_auto_route.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-05-23 23:28:52.000000 auto_route-0.1.0/auto_route/create_composed_class.py
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-05-25 16:57:12.000000 auto_route-0.1.0/auto_route/streamlit_demo.py
-drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:01:01.750017 auto_route-0.1.0/auto_route.egg-info/
--rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:01:01.000000 auto_route-0.1.0/auto_route.egg-info/PKG-INFO
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      363 2023-06-07 00:01:01.000000 auto_route-0.1.0/auto_route.egg-info/SOURCES.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:01:01.000000 auto_route-0.1.0/auto_route.egg-info/dependency_links.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       17 2023-06-07 00:01:01.000000 auto_route-0.1.0/auto_route.egg-info/requires.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       11 2023-06-07 00:01:01.000000 auto_route-0.1.0/auto_route.egg-info/top_level.txt
--rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:01:01.750017 auto_route-0.1.0/setup.cfg
--rw-rw-r--   0 ruben     (1000) ruben     (1000)      662 2023-06-07 00:00:04.000000 auto_route-0.1.0/setup.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:14:00.455490 auto_route-0.1.1/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:14:00.455490 auto_route-0.1.1/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4582 2023-06-06 23:59:56.000000 auto_route-0.1.1/README.rst
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:14:00.455490 auto_route-0.1.1/auto_app/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:09:47.000000 auto_route-0.1.1/auto_app/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     3701 2023-05-25 21:35:31.000000 auto_route-0.1.1/auto_app/auto_app.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     1608 2023-05-25 16:57:12.000000 auto_route-0.1.1/auto_app/cli_auto_route.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      779 2023-05-25 16:57:12.000000 auto_route-0.1.1/auto_app/streamlit_demo.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:14:00.455490 auto_route-0.1.1/auto_route/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        0 2023-05-12 18:05:03.000000 auto_route-0.1.1/auto_route/__init__.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     7067 2023-05-25 21:33:21.000000 auto_route-0.1.1/auto_route/auto_route.py
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     2657 2023-05-23 23:28:52.000000 auto_route-0.1.1/auto_route/create_composed_class.py
+drwxrwxr-x   0 ruben     (1000) ruben     (1000)        0 2023-06-07 00:14:00.455490 auto_route-0.1.1/auto_route.egg-info/
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)     4980 2023-06-07 00:14:00.000000 auto_route-0.1.1/auto_route.egg-info/PKG-INFO
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      368 2023-06-07 00:14:00.000000 auto_route-0.1.1/auto_route.egg-info/SOURCES.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)        1 2023-06-07 00:14:00.000000 auto_route-0.1.1/auto_route.egg-info/dependency_links.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       17 2023-06-07 00:14:00.000000 auto_route-0.1.1/auto_route.egg-info/requires.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       20 2023-06-07 00:14:00.000000 auto_route-0.1.1/auto_route.egg-info/top_level.txt
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)       38 2023-06-07 00:14:00.455490 auto_route-0.1.1/setup.cfg
+-rw-rw-r--   0 ruben     (1000) ruben     (1000)      674 2023-06-07 00:13:56.000000 auto_route-0.1.1/setup.py
```

### Comparing `auto_route-0.1.0/PKG-INFO` & `auto_route-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto_route
-Version: 0.1.0
+Version: 0.1.1
 Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
 Home-page: http://github.com/yourname/auto_route
 Author: Ruben Fernandez
 Author-email: ruben@carbonyl.org
 Description-Content-Type: text/x-rst
 
 Contributing to the AutoRoute Project
```

### Comparing `auto_route-0.1.0/README.md` & `auto_route-0.1.1/auto_route.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,116 @@
-# Contributing to the AutoRoute Project
+Metadata-Version: 2.1
+Name: auto-route
+Version: 0.1.1
+Summary: Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
+Home-page: http://github.com/yourname/auto_route
+Author: Ruben Fernandez
+Author-email: ruben@carbonyl.org
+Description-Content-Type: text/x-rst
+
+Contributing to the AutoRoute Project
+=====================================
+
+Introduction
+------------
+
+Thank you for your interest in contributing to the AutoRoute project!
+Our goal is to simplify and automate the creation of SaaS/PaaS
+solutions. We’re excited to welcome you to our community.
+
+Here’s a guide on how you can contribute:
+
+Getting Started
+---------------
+
+**Understanding the Project:** Familiarize yourself with the project’s
+features, design philosophy, and architecture. Spend some time exploring
+the codebase and reading the existing documentation (md and docstrings).
+
+-  `Components_Breakdown.md <Components_Breakdown.md>`__
+-  `Proposal.md <Proposal.md>`__
+-  `Part 1 - Creating FastAPI Application and Auto-generating Class
+   Method
+   Endpoints.md <1%20-%20Creating%20FastAPI%20Application%20and%20Auto-generating%20Class%20Method%20Endpoints.md>`__
+-  `Part 2 - Generating OpenAPI Specification and Interactive
+   Documentation for
+   FastAPI.md <2%20-%20Generating%20OpenAPI%20Specification%20and%20Interactive%20Documentation%20for%20FastAPI.md>`__
+-  `Part 3 - Exploring the Generated Python Client Library and
+   Customizing Its
+   Configuration.md <3%20-%20Exploring%20the%20Generated%20Python%20Client%20Library%20and%20Customizing%20Its%20Configuration.md>`__
+-  `Part 4 - FastAPI Application and Generated Client Library: Complete
+   Guide for
+   Beginners.md <4%20-%20FastAPI%20Application%20and%20Generated%20Client%20Library%3A%20Complete%20Guide%20for%20Beginners.md>`__
+-  `Dockerfile_example.md <Dockerfile_example.md>`__
+-  `how_to_improve_microservice.md <how_to_improve_microservice.md>`__
+
+**Quick Guide:**
+
+::
+
+   @auto_route
+   def get_customer_id():
+       return "customer_id"
+
+1.  *@auto_route:*
+
+    1. The **naming conversion** for functions using this wrapper is
+       ``http-method_tag_*detail`` :
+
+       1. *where* http_method is in
+          ``[get, post, put, delete, patch, options, head, trace]``
+       2. the **tag** is the name of the class that the function is in,
+          e.g. ``customer``
+       3. the **detail** is the name of the function, in the example
+          above, the detail would be ``id``
+       4. e.g.  ## Areas of Contribution
+
+2.  **Documentation:** Clear, comprehensive documentation is crucial for
+    any successful open-source project. Help us improve our
+    documentation by creating tutorials, adding usage examples, and
+    improving descriptions of features and configurations.
+
+3.  **Continuous Integration/Continuous Deployment (CI/CD):** We’re
+    always aiming to improve our automated testing and deployment
+    processes. If you have experience with CI/CD platforms like GitHub
+    Actions, Travis CI, or Jenkins, your expertise could be incredibly
+    valuable.
+
+4.  **Automated Testing:** Robust testing is a core part of our
+    commitment to code quality. Help us achieve this by writing unit
+    tests and improving our code coverage.
+
+5.  **Code Quality Checks:** We’re committed to maintaining a clean and
+    readable codebase. Contribute by improving our linting processes,
+    static code analysis, and enforcing our code style guidelines.
+
+6.  **Debugging AI Models:** This is an exciting part of our project. If
+    you have ideas on how to include more common issues and security
+    checks, or ways to extend our debugging with user-defined checks, we
+    would love to hear from you.
+
+7.  **Payment Integrations:** We currently support Stripe, but we aim to
+    provide more flexibility for our users. Help us integrate other
+    payment providers like PayPal, Square, or even cryptocurrencies.
+
+8.  **Configuration Options:** We want to make our project as flexible
+    as possible. Your contributions could help us support different
+    deployment options, database backends, and more.
+
+9.  **API Wrappers:** We currently provide wrappers for Google
+    applications. Help us extend our reach by adding wrappers for other
+    popular APIs, such as social media APIs or other cloud service APIs.
+
+10. **Multi-Language Support:** We already support over 50 languages
+    thanks to openapi.json and the OpenAPI SDK generator. Help us extend
+    our reach by translating our documentation or other parts of our
+    project into other languages.
+
+Community
+---------
+
+Finally, we encourage all contributors to participate in our community.
+Join our forum or chat room, sign up for our mailing list, and help us
+build a friendly, active community around our project.
 
-## Introduction
-
-Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.
-
-Here's a guide on how you can contribute:
-
-## Getting Started
-
-**Understanding the Project:** Familiarize yourself with the project's features, design philosophy, and architecture. Spend some time exploring the codebase and reading the existing documentation (md and docstrings).
-
-* [Components_Breakdown.md](Components_Breakdown.md)
-* [Proposal.md](Proposal.md)
-* [Part 1 - Creating FastAPI Application and Auto-generating Class Method Endpoints.md](1%20-%20Creating%20FastAPI%20Application%20and%20Auto-generating%20Class%20Method%20Endpoints.md)
-* [Part 2 - Generating OpenAPI Specification and Interactive Documentation for FastAPI.md](2%20-%20Generating%20OpenAPI%20Specification%20and%20Interactive%20Documentation%20for%20FastAPI.md)
-* [Part 3 - Exploring the Generated Python Client Library and Customizing Its Configuration.md](3%20-%20Exploring%20the%20Generated%20Python%20Client%20Library%20and%20Customizing%20Its%20Configuration.md)
-* [Part 4 - FastAPI Application and Generated Client Library: Complete Guide for Beginners.md](4%20-%20FastAPI%20Application%20and%20Generated%20Client%20Library%3A%20Complete%20Guide%20for%20Beginners.md)
-* [Dockerfile_example.md](Dockerfile_example.md)
-* [how_to_improve_microservice.md](how_to_improve_microservice.md)
-
-**Quick Guide:** 
-
-```
-@auto_route
-def get_customer_id():
-    return "customer_id"
-```
-
-1. *@auto_route:*
-    1. The **naming conversion** for functions using this wrapper is ```http-method_tag_*detail``` : 
-       1. *where* http_method is in ```[get, post, put, delete, patch, options, head, trace]``` 
-       2. the **tag** is the name of the class that the function is in, e.g. ```customer```
-       3. the **detail** is the name of the function, in the example above, the detail would be ```id```
-       4. e.g. 
-## Areas of Contribution
-
-1. **Documentation:** Clear, comprehensive documentation is crucial for any successful open-source project. Help us improve our documentation by creating tutorials, adding usage examples, and improving descriptions of features and configurations.
-
-2. **Continuous Integration/Continuous Deployment (CI/CD):** We're always aiming to improve our automated testing and deployment processes. If you have experience with CI/CD platforms like GitHub Actions, Travis CI, or Jenkins, your expertise could be incredibly valuable.
-
-3. **Automated Testing:** Robust testing is a core part of our commitment to code quality. Help us achieve this by writing unit tests and improving our code coverage.
-
-4. **Code Quality Checks:** We're committed to maintaining a clean and readable codebase. Contribute by improving our linting processes, static code analysis, and enforcing our code style guidelines.
-
-5. **Debugging AI Models:** This is an exciting part of our project. If you have ideas on how to include more common issues and security checks, or ways to extend our debugging with user-defined checks, we would love to hear from you.
-
-6. **Payment Integrations:** We currently support Stripe, but we aim to provide more flexibility for our users. Help us integrate other payment providers like PayPal, Square, or even cryptocurrencies.
-
-7. **Configuration Options:** We want to make our project as flexible as possible. Your contributions could help us support different deployment options, database backends, and more.
-
-8. **API Wrappers:** We currently provide wrappers for Google applications. Help us extend our reach by adding wrappers for other popular APIs, such as social media APIs or other cloud service APIs.
-
-9. **Multi-Language Support:** We already support over 50 languages thanks to openapi.json and the OpenAPI SDK generator. Help us extend our reach by translating our documentation or other parts of our project into other languages.
-
-## Community
-
-Finally, we encourage all contributors to participate in our community. Join our forum or chat room, sign up for our mailing list, and help us build a friendly, active community around our project.
-
-Thank you for considering contributing to AutoRoute. We look forward to working with you!
+Thank you for considering contributing to AutoRoute. We look forward to
+working with you!
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auto_route-0.1.0/README.rst` & `auto_route-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.0/auto_route/auto_app.py` & `auto_route-0.1.1/auto_app/auto_app.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.0/auto_route/auto_route.py` & `auto_route-0.1.1/auto_route/auto_route.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.0/auto_route/cli_auto_route.py` & `auto_route-0.1.1/auto_app/cli_auto_route.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.0/auto_route/create_composed_class.py` & `auto_route-0.1.1/auto_route/create_composed_class.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.0/auto_route/streamlit_demo.py` & `auto_route-0.1.1/auto_app/streamlit_demo.py`

 * *Files identical despite different names*

### Comparing `auto_route-0.1.0/setup.py` & `auto_route-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto_route',
-    version='0.1.0',  # Semantic Versioning
-    packages=["auto_route"],
+    version='0.1.1',  # Semantic Versioning
+    packages=["auto_route", "auto_app"],
     author='Ruben Fernandez',
     author_email='ruben@carbonyl.org',
     description="Thank you for your interest in contributing to the AutoRoute project! Our goal is to simplify and "
                 "automate the creation of SaaS/PaaS solutions. We're excited to welcome you to our community.",
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='http://github.com/yourname/auto_route',
```

