# Comparing `tmp/django-erp-framework-1.5.0.tar.gz` & `tmp/django-erp-framework-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-erp-framework-1.5.0.tar", last modified: Sun May 28 14:45:13 2023, max compression
+gzip compressed data, was "django-erp-framework-1.5.2.tar", last modified: Wed Jun  7 09:56:04 2023, max compression
```

## Comparing `django-erp-framework-1.5.0.tar` & `django-erp-framework-1.5.2.tar`

### file list

```diff
@@ -1,64 +1,60 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/
--rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-1.5.0/LICENSE
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-1.5.0/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4978 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3335 2023-05-26 08:27:01.000000 django-erp-framework-1.5.0/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.695144 django-erp-framework-1.5.0/django_erp_framework.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4978 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1721 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      204 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-05-28 14:45:13.000000 django-erp-framework-1.5.0/django_erp_framework.egg-info/top_level.txt
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.699144 django-erp-framework-1.5.0/erp_framework/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       97 2023-05-28 14:24:57.000000 django-erp-framework-1.5.0/erp_framework/__init__.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.699144 django-erp-framework-1.5.0/erp_framework/activity/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8413 2023-05-28 13:28:51.000000 django-erp-framework-1.5.0/erp_framework/activity/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.699144 django-erp-framework-1.5.0/erp_framework/activity/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/0002_auto_20200711_1253.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/0003_alter_myactivity_options.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/activity/models.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/admin/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-10 22:04:15.000000 django-erp-framework-1.5.0/erp_framework/admin/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    47051 2023-05-28 14:00:46.000000 django-erp-framework-1.5.0/erp_framework/admin/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/admin/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7520 2023-05-28 13:58:30.000000 django-erp-framework-1.5.0/erp_framework/admin/base.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      474 2023-05-08 22:07:29.000000 django-erp-framework-1.5.0/erp_framework/admin/forms.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      611 2023-05-08 22:03:29.000000 django-erp-framework-1.5.0/erp_framework/admin/helpers.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/admin/jazzmin_integration/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-14 13:33:44.000000 django-erp-framework-1.5.0/erp_framework/admin/jazzmin_integration/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      126 2023-05-14 13:33:44.000000 django-erp-framework-1.5.0/erp_framework/admin/jazzmin_integration/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      277 2023-05-28 13:58:30.000000 django-erp-framework-1.5.0/erp_framework/apps.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/base/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/base/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2342 2023-05-28 13:58:30.000000 django-erp-framework-1.5.0/erp_framework/base/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7619 2023-05-28 14:00:04.000000 django-erp-framework-1.5.0/erp_framework/base/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    12628 2023-05-28 14:00:04.000000 django-erp-framework-1.5.0/erp_framework/base/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      813 2023-05-28 14:15:31.000000 django-erp-framework-1.5.0/erp_framework/checks.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/contrib/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/contrib/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     3517 2023-05-14 14:42:52.000000 django-erp-framework-1.5.0/erp_framework/doc_types.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-08 18:31:35.000000 django-erp-framework-1.5.0/erp_framework/reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1051 2023-05-26 08:16:22.000000 django-erp-framework-1.5.0/erp_framework/reporting/admin.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1698 2023-05-26 08:17:43.000000 django-erp-framework-1.5.0/erp_framework/reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/reporting/forms.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.703143 django-erp-framework-1.5.0/erp_framework/reporting/migrations/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4526 2023-05-28 12:38:42.000000 django-erp-framework-1.5.0/erp_framework/reporting/migrations/0001_initial.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-25 21:59:15.000000 django-erp-framework-1.5.0/erp_framework/reporting/migrations/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1890 2023-05-26 08:17:43.000000 django-erp-framework-1.5.0/erp_framework/reporting/models.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     4205 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/reporting/printing.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7009 2023-05-26 08:16:22.000000 django-erp-framework-1.5.0/erp_framework/reporting/registry.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/erp_framework/reporting/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/reporting/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2782 2023-05-23 14:48:31.000000 django-erp-framework-1.5.0/erp_framework/reporting/templatetags/erp_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    13893 2023-05-28 14:37:56.000000 django-erp-framework-1.5.0/erp_framework/reporting/views.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      456 2023-05-28 13:28:51.000000 django-erp-framework-1.5.0/erp_framework/sites.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/erp_framework/utils/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/utils/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     2143 2023-05-06 11:19:07.000000 django-erp-framework-1.5.0/erp_framework/utils/views.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1781 2023-05-28 14:45:13.707144 django-erp-framework-1.5.0/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-1.5.0/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)    34523 2019-12-11 20:34:36.000000 django-erp-framework-1.5.2/LICENSE
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      177 2019-12-25 18:25:30.000000 django-erp-framework-1.5.2/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4978 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3335 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.407911 django-erp-framework-1.5.2/django_erp_framework.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4978 2023-06-07 09:56:04.000000 django-erp-framework-1.5.2/django_erp_framework.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1631 2023-06-07 09:56:04.000000 django-erp-framework-1.5.2/django_erp_framework.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-06-07 09:56:04.000000 django-erp-framework-1.5.2/django_erp_framework.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      204 2023-06-07 09:56:04.000000 django-erp-framework-1.5.2/django_erp_framework.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       28 2023-06-07 09:56:04.000000 django-erp-framework-1.5.2/django_erp_framework.egg-info/top_level.txt
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.407911 django-erp-framework-1.5.2/erp_framework/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       97 2023-06-07 09:55:59.000000 django-erp-framework-1.5.2/erp_framework/__init__.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/activity/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       68 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/activity/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8611 2023-06-02 11:44:48.000000 django-erp-framework-1.5.2/erp_framework/activity/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      191 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/activity/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/activity/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      792 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/activity/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      383 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/activity/migrations/0002_auto_20200711_1253.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      399 2023-05-07 12:35:32.000000 django-erp-framework-1.5.2/erp_framework/activity/migrations/0003_alter_myactivity_options.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/activity/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      260 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/activity/models.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/admin/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/admin/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    40902 2023-06-02 11:52:07.000000 django-erp-framework-1.5.2/erp_framework/admin/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      135 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/admin/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     5442 2023-06-06 10:48:57.000000 django-erp-framework-1.5.2/erp_framework/admin/base.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      611 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/admin/helpers.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/admin/jazzmin_integration/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/admin/jazzmin_integration/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      126 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/admin/jazzmin_integration/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      277 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/apps.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/base/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/base/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3971 2023-06-06 10:28:57.000000 django-erp-framework-1.5.2/erp_framework/base/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8082 2023-06-01 15:46:04.000000 django-erp-framework-1.5.2/erp_framework/base/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9675 2023-06-02 11:35:20.000000 django-erp-framework-1.5.2/erp_framework/base/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      813 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/checks.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/contrib/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/contrib/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3517 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/doc_types.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1051 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/reporting/admin.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1709 2023-06-03 10:41:07.000000 django-erp-framework-1.5.2/erp_framework/reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1067 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/reporting/forms.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/reporting/migrations/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4526 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/reporting/migrations/0001_initial.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        0 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/reporting/migrations/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1890 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/reporting/models.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3808 2023-06-01 13:01:47.000000 django-erp-framework-1.5.2/erp_framework/reporting/printing.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     8741 2023-06-03 10:41:07.000000 django-erp-framework-1.5.2/erp_framework/reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/erp_framework/reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-28 14:50:10.000000 django-erp-framework-1.5.2/erp_framework/reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     3737 2023-06-03 10:41:09.000000 django-erp-framework-1.5.2/erp_framework/reporting/templatetags/erp_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7839 2023-06-06 10:06:24.000000 django-erp-framework-1.5.2/erp_framework/reporting/views.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      473 2023-06-03 08:57:01.000000 django-erp-framework-1.5.2/erp_framework/sites.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1781 2023-06-07 09:56:04.411911 django-erp-framework-1.5.2/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-erp-framework-1.5.2/setup.py
```

### Comparing `django-erp-framework-1.5.0/LICENSE` & `django-erp-framework-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/PKG-INFO` & `django-erp-framework-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 1.5.0
+Version: 1.5.2
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/RamezIssac/django-erp-framework
 Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
```

### Comparing `django-erp-framework-1.5.0/README.rst` & `django-erp-framework-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/django_erp_framework.egg-info/PKG-INFO` & `django-erp-framework-1.5.2/django_erp_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-erp-framework
-Version: 1.5.0
+Version: 1.5.2
 Summary: A light-weight effective Django based framework to create diverse business applications
 Home-page: https://github.com/RamezIssac/django-erp-framework
 Author: Ramez Issac
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/RA/
 Project-URL: Documentation, https://django-erp-framework.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/RA
```

### Comparing `django-erp-framework-1.5.0/django_erp_framework.egg-info/SOURCES.txt` & `django-erp-framework-1.5.2/django_erp_framework.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 erp_framework/activity/migrations/0002_auto_20200711_1253.py
 erp_framework/activity/migrations/0003_alter_myactivity_options.py
 erp_framework/activity/migrations/__init__.py
 erp_framework/admin/__init__.py
 erp_framework/admin/admin.py
 erp_framework/admin/apps.py
 erp_framework/admin/base.py
-erp_framework/admin/forms.py
 erp_framework/admin/helpers.py
 erp_framework/admin/jazzmin_integration/__init__.py
 erp_framework/admin/jazzmin_integration/apps.py
 erp_framework/base/__init__.py
 erp_framework/base/app_settings.py
 erp_framework/base/helpers.py
 erp_framework/base/models.py
@@ -41,10 +40,8 @@
 erp_framework/reporting/models.py
 erp_framework/reporting/printing.py
 erp_framework/reporting/registry.py
 erp_framework/reporting/views.py
 erp_framework/reporting/migrations/0001_initial.py
 erp_framework/reporting/migrations/__init__.py
 erp_framework/reporting/templatetags/__init__.py
-erp_framework/reporting/templatetags/erp_reporting_tags.py
-erp_framework/utils/__init__.py
-erp_framework/utils/views.py
+erp_framework/reporting/templatetags/erp_reporting_tags.py
```

### Comparing `django-erp-framework-1.5.0/erp_framework/activity/admin.py` & `django-erp-framework-1.5.2/erp_framework/activity/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,181 +11,182 @@
 from erp_framework.activity.models import MyActivity
 from erp_framework.admin.admin import RaThemeMixin
 from erp_framework.sites import erp_admin_site
 from erp_framework.base import app_settings
 from erp_framework.base.helpers import RaPermissionWidgetExclude
 
 action_names = {
-    ADDITION: 'Addition',
-    CHANGE: 'Change',
-    DELETION: 'Deletion',
+    ADDITION: "Addition",
+    CHANGE: "Change",
+    DELETION: "Deletion",
 }
 
 
-def translate_list(l, func=_):
-    """
-    Translate strings in list, used originally to translate report_columns
-    :param l: list of data
-    :param func: translation function
-    :return: translated list
-    """
-    t = []
-    for i in l:
-        t.append(func(i))
-    return t
-
-
 class FilterBase(admin.SimpleListFilter):
     def queryset(self, request, queryset):
         if self.value():
             dictionary = dict(((self.parameter_name, self.value()),))
             return queryset.filter(**dictionary)
 
 
 class ActionFilter(FilterBase):
-    title = _('Action')
-    parameter_name = 'action_flag'
+    title = _("Action")
+    parameter_name = "action_flag"
 
     def lookups(self, request, model_admin):
         vals = ()
         for x in action_names.items():
-            verbose = x[1] if x[1] != 'Change' else 'Update'
+            verbose = x[1] if x[1] != "Change" else "Update"
             vals += ((x[0], _(verbose)),)
         return vals
 
 
 class UserFilter(FilterBase):
     """Use this filter to only show current users, who appear in the log."""
-    title = _('User')
-    parameter_name = 'user_id'
+
+    title = _("User")
+    parameter_name = "user_id"
 
     def lookups(self, request, model_admin):
-        return tuple((u.id, u.username)
-                     for u in User.objects.filter(pk__in=LogEntry.objects.values_list('user_id').distinct())
-                     )
+        return tuple(
+            (u.id, u.username)
+            for u in User.objects.filter(
+                pk__in=LogEntry.objects.values_list("user_id").distinct()
+            )
+        )
 
 
 class AdminFilter(UserFilter):
     """Use this filter to only show current Superusers."""
-    title = 'admin'
+
+    title = "admin"
 
     def lookups(self, request, model_admin):
         return tuple((u.id, u.username) for u in User.objects.filter(is_superuser=True))
 
 
 class StaffFilter(UserFilter):
     """Use this filter to only show current Staff members."""
-    title = 'staff'
+
+    title = "staff"
 
     def lookups(self, request, model_admin):
         return tuple((u.id, u.username) for u in User.objects.filter(is_staff=True))
 
 
 class RAContentTypeFilter(admin.SimpleListFilter):
     """Use this filter to only Appropriate content types."""
-    title = _('Content Type')
-    parameter_name = 'content_type'
+
+    title = _("Content Type")
+    parameter_name = "content_type"
 
     def lookups(self, request, model_admin):
         vals = ()
         val_list = []
         cs = ContentType.objects.filter(logentry__action_flag__in=[1, 2, 3]).distinct()
         exclude_function = RaPermissionWidgetExclude()
         for c in cs:
             model = c.model_class()
             if model:
                 if not exclude_function(model):
-                    val_list.append({
-                        'name': capfirst(str(model._meta.verbose_name_plural)),
-                        'value': ((c.pk, capfirst(str(model._meta.verbose_name_plural))),)
-                    })
-        ordered_list = dictsort(val_list, 'name')
+                    val_list.append(
+                        {
+                            "name": capfirst(str(model._meta.verbose_name_plural)),
+                            "value": (
+                                (c.pk, capfirst(str(model._meta.verbose_name_plural))),
+                            ),
+                        }
+                    )
+        ordered_list = dictsort(val_list, "name")
         for o in ordered_list:
-            vals += o['value']
+            vals += o["value"]
         return vals
 
     def queryset(self, request, queryset):
         if self.value():
             queryset = queryset.filter(content_type_id=self.value())
         return queryset
         # return tuple((u.id, u.username) for u in User.objects.filter(is_staff=True))
 
 
 class LogEntryAdmin(RaThemeMixin, admin.ModelAdmin):
-    date_hierarchy = 'action_time'
+    date_hierarchy = "action_time"
     actions = None
     list_display_links = None
     # readonly_fields = LogEntry._meta.get_all_field_names()
     readonly_fields = [f.name for f in LogEntry._meta.get_fields()]
 
     list_filter = [
         UserFilter,
         ActionFilter,
         RAContentTypeFilter,
         # 'content_type',
         # 'user',
     ]
 
-    search_fields = [
-        'object_repr',
-        'change_message'
-    ]
+    search_fields = ["object_repr", "change_message"]
 
     list_display = [
-        'action_time',
-        'get_user',
-        'action_description',
-        'get_contenttype',
-        'object_link',
+        "action_time",
+        "get_user",
+        "action_description",
+        "get_contenttype",
+        "object_link",
         # 'action_flag',
-        'get_change_message',
-        'review'
+        "get_change_message",
+        "review",
     ]
 
     def has_module_permission(self, request):
         return True
 
     def has_add_permission(self, request):
         return False
 
     def has_change_permission(self, request, obj=None):
-        return True and request.method != 'POST'
+        return True and request.method != "POST"
 
     def has_delete_permission(self, request, obj=None):
         return False
 
     def get_user(self, obj):
         return obj.user
 
-    get_user.short_description = _('User')
-    get_user.admin_order_field = 'user'
+    get_user.short_description = _("User")
+    get_user.admin_order_field = "user"
 
     def get_change_message(self, obj):
         return truncatewords(obj.get_change_message(), 23)
 
-    get_change_message.short_description = _('Comment')
+    get_change_message.short_description = _("Comment")
 
     def object_link(self, obj):
         ct = obj.content_type
         repr_ = escape(obj.object_repr)
         try:
-            href = reverse('%s:%s_%s_change' % (app_settings.ERP_FRAMEWORK_SITE_NAME, ct.app_label, ct.model),
-                           args=[obj.object_id])
-            link = u'<a href="%s">%s</a>' % (href, repr_)
+            href = reverse(
+                "%s:%s_%s_change"
+                % (app_settings.ERP_FRAMEWORK_SITE_NAME, ct.app_label, ct.model),
+                args=[obj.object_id],
+            )
+            link = '<a href="%s">%s</a>' % (href, repr_)
         except NoReverseMatch:
             link = repr_
         return mark_safe(link) if obj.action_flag != DELETION else repr_
 
     object_link.allow_tags = True
-    object_link.admin_order_field = 'object_repr'
-    object_link.short_description = _('Slug/Name')
+    object_link.admin_order_field = "object_repr"
+    object_link.short_description = _("Slug/Name")
 
     def get_queryset(self, request):
-        queryset = super(LogEntryAdmin, self).get_queryset(request) \
-            .prefetch_related('content_type')
+        queryset = (
+            super(LogEntryAdmin, self)
+            .get_queryset(request)
+            .prefetch_related("content_type")
+        )
         if not request.user.is_superuser:
             queryset = queryset.filter(user__id=request.user.pk)
         return queryset
 
     def get_list_filter(self, request):
         filters = super(LogEntryAdmin, self).get_list_filter(request)
         if not request.user.is_superuser:
@@ -194,56 +195,73 @@
 
     def action_description(self, obj):
         verbose = action_names[obj.action_flag]
         # verbose = 'Update' if verbose == 'Change' else verbose
 
         return _(verbose)
 
-    action_description.short_description = _('Action')
-    action_description.admin_order_field = 'action_flag'
+    action_description.short_description = _("Action")
+    action_description.admin_order_field = "action_flag"
 
     def get_contenttype(self, obj):
         return capfirst(obj.content_type)
 
-    get_contenttype.short_description = _('Content Type')
-    get_contenttype.admin_order_field = 'content_type__model'
+    get_contenttype.short_description = _("Content Type")
+    get_contenttype.admin_order_field = "content_type__model"
 
     def review(self, obj):
         if obj.action_flag == 2:
             try:
-                url = reverse('%s:%s_%s_history' % (app_settings.ERP_FRAMEWORK_SITE_NAME, obj.content_type.app_label,
-                                                    obj.content_type.model), args=(obj.object_id,))
+                url = reverse(
+                    "%s:%s_%s_history"
+                    % (
+                        app_settings.ERP_FRAMEWORK_SITE_NAME,
+                        obj.content_type.app_label,
+                        obj.content_type.model,
+                    ),
+                    args=(obj.object_id,),
+                )
             except NoReverseMatch:
-                url = ''
+                url = ""
             link = """<a href="%s" class="legitRipple" data-popup="tooltip" title="%s">
                 <i class="fas fa-history text-indigo-800"></i>
-                <span class="legitRipple-ripple"></span></a>""" % (url, _('History'))
+                <span class="legitRipple-ripple"></span></a>""" % (
+                url,
+                _("History"),
+            )
             return mark_safe(link)
         elif obj.action_flag == 3:
-            url = reverse('%s:%s_%s_recover' % (app_settings.ERP_FRAMEWORK_SITE_NAME, obj.content_type.app_label,
-                                                obj.content_type.model), args=(obj.object_id,))
+            url = reverse(
+                "%s:%s_%s_recover"
+                % (
+                    app_settings.ERP_FRAMEWORK_SITE_NAME,
+                    obj.content_type.app_label,
+                    obj.content_type.model,
+                ),
+                args=(obj.object_id,),
+            )
             link = """<a href="%s" class="legitRipple" data-popup="tooltip" title="%s">
                     <i class="fas fa-undo text-indigo-800"></i>
-                    <span class="legitRipple-ripple"></span></a>""" % (url, _('Recover'))
+                    <span class="legitRipple-ripple"></span></a>""" % (
+                url,
+                _("Recover"),
+            )
             return mark_safe(link)
 
-        return ''
+        return ""
 
-    review.short_description = _('review')
+    review.short_description = _("review")
 
     def changelist_view(self, request, extra_context=None):
-        extra_context = {
-            'has_detached_sidebar': True
-        }
+        extra_context = {"has_detached_sidebar": True}
         return super(LogEntryAdmin, self).changelist_view(request, extra_context)
 
 
 class MyActivityAdmin(LogEntryAdmin):
     list_filter = [
-
         ActionFilter,
         RAContentTypeFilter,
     ]
 
     def get_queryset(self, request):
         qs = super(MyActivityAdmin, self).get_queryset(request)
         qs = qs.filter(user_id=request.user.pk)
```

### Comparing `django-erp-framework-1.5.0/erp_framework/activity/migrations/0001_initial.py` & `django-erp-framework-1.5.2/erp_framework/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/admin/admin.py` & `django-erp-framework-1.5.2/erp_framework/admin/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,27 +88,27 @@
             % ("admin", self.model._meta.app_label, self.model._meta.model_name),
             args=(quote(obj.pk),),
             current_app=self.admin_site.name,
         )
 
         # todo change the str obj
         view_link = (
-                '<a href="%s" data-popup="tooltip" name="%s %s" data-placement="bottom"> '
-                '<i class="fas fa-chart-line"></i> </a>'
-                % (url, capfirst(_("Statistics for")), str(obj))
+            '<a href="%s" data-popup="tooltip" name="%s %s" data-placement="bottom"> '
+            '<i class="fas fa-chart-line"></i> </a>'
+            % (url, capfirst(_("Statistics for")), str(obj))
         )
         return mark_safe(view_link)
 
     get_stats_icon.short_description = _("Stats")
 
     def get_view_fields(self, request, obj=None):
         return (
-                self.view_fields
-                or [x for x in flatten_list(self.fields)]
-                or self.get_fields(request, obj)
+            self.view_fields
+            or [x for x in flatten_list(self.fields)]
+            or self.get_fields(request, obj)
         )
 
     def get_view_title(self, request, obj=None):
         return _("View %s") % str(obj)
         # return self.get_title(request, obj)
 
     def get_urls(self):
@@ -142,18 +142,18 @@
             )
 
         model = self.model
         opts = model._meta
 
         obj = self.get_object(request, unquote(object_id), to_field)
 
-        if not self.has_view_permission(request, obj):
+        if not self.has_view_permission(request, obj):  # pragma: no cover
             raise PermissionDenied
 
-        if obj is None:
+        if obj is None:  # pragma: no cover
             return self._get_obj_does_not_exist_redirect(request, opts, object_id)
 
         data = []
         view_fields = self.get_view_fields(request, obj)
         for field_name in view_fields:
             # field = self.get_field(request, obj, field_name)
             field = model._meta.get_field(field_name)
@@ -237,15 +237,15 @@
     formfield_overrides = {
         # DateTimeField: {'widget': AdminSplitDateTime},
         # DecimalField: {'widget': NumberInput},
         # ForeignKey: {'widget': RaBootstrapForeignKeyWidget},
         TextField: {"widget": AdminTextareaWidget(attrs={"rows": 2})}
     }
 
-    # Ra New Attributes
+    # ERP New Attributes
     # ------------------
     description = None  # Description of the model to be displayed in hte changelist filter under the name
     enable_next_serial = True  # Enable the default slug to be a serial number
     enable_view_view = True  # If False there is no "DetailView ie Stats view"
     print_template = None
     no_records_message = _("No Data")
 
@@ -275,16 +275,16 @@
                 ),
                 args=(quote(pk),),
                 current_app=self.admin_site.name,
             )
             if not main_url:
                 main_url = url
             view_link = (
-                    '<a href="%s" data-popup="tooltip" name="%s" data-placement="bottom">'
-                    ' <i class="fas fa-edit"></i> </a>' % (url, capfirst(_("change")))
+                '<a href="%s" data-popup="tooltip" name="%s" data-placement="bottom">'
+                ' <i class="fas fa-edit"></i> </a>' % (url, capfirst(_("change")))
             )
             links.append(view_link)
             links = "<span class='go-to-change-form'>%s</span>" % "".join(links) + ""
             obj_link_title = "<a href='%s'>%s</a>" % (main_url, obj.name)
             return mark_safe("%s %s" % (obj_link_title, links))
 
         return obj.name
@@ -301,101 +301,14 @@
         )
 
     get_history_link.short_description = _("History")
 
     get_enhanced_obj_title.short_description = _("name")
     get_enhanced_obj_title.admin_order_field = "name"
 
-    # Permissions
-    # def has_view_permission(self, request, obj=None):
-    #     if not self.enable_view_view:
-    #         return False
-    #     opts = self.opts
-    #     codename = get_permission_codename('view', opts)
-    #     return request.user.has_perm("%s.%s" % (opts.app_label, codename))
-    #
-    # def view_view(self, request, object_id, form_url='', extra_context=None):
-    #     extra_context = extra_context or {}
-    #     extra_context['has_add_permission'] = self.has_add_permission(request)
-    #     '''
-    #         Code copied from ChangeForm
-    #     '''
-    #
-    #     to_field = request.POST.get(TO_FIELD_VAR, request.GET.get(TO_FIELD_VAR))
-    #     if to_field and not self.to_field_allowed(request, to_field):
-    #         raise DisallowedModelAdminToField("The field %s cannot be referenced." % to_field)
-    #
-    #     model = self.model
-    #     opts = model._meta
-    #     add = object_id is None
-    #
-    #     if add:
-    #         if not self.has_add_permission(request):
-    #             raise PermissionDenied
-    #         obj = None
-    #
-    #     else:
-    #         obj = self.get_object(request, unquote(object_id), to_field)
-    #
-    #         if not self.has_view_permission(request, obj):
-    #             raise PermissionDenied
-    #
-    #         if obj is None:
-    #             raise Http404(_('%(name)s object with primary key %(key)r does not exist.') % {
-    #                 'name': str(opts.verbose_name), 'key': escape(object_id)})
-    #
-    #             # if request.method == 'POST' and "_saveasnew" in request.POST:
-    #             #     return self.add_view(request, form_url=reverse('admin:%s_%s_add' % (
-    #             #         opts.app_label, opts.model_name), current_app=self.admin_site.name))
-    #     context = dict(self.admin_site.each_context(request),
-    #                    name=obj,
-    #                    app_label=opts.app_label,
-    #                    object_id=object_id,
-    #                    original=obj,
-    #                    is_popup=(IS_POPUP_VAR in request.POST or
-    #                              IS_POPUP_VAR in request.GET),
-    #                    to_field=to_field,
-    #                    # media=media,
-    #                    preserved_filters=self.get_preserved_filters(request),
-    #                    )
-    #
-    #     context.update(extra_context or {})
-    #
-    #     opts = self.model._meta
-    #     app_label = opts.app_label
-    #     preserved_filters = self.get_preserved_filters(request)
-    #     form_url = add_preserved_filters({'preserved_filters': preserved_filters, 'opts': opts}, form_url)
-    #     view_on_site_url = self.get_view_on_site_url(obj)
-    #     context.update({
-    #         'add': add,
-    #         'change': not add,
-    #         'has_add_permission': self.has_add_permission(request),
-    #         'has_change_permission': self.has_change_permission(request, obj),
-    #         'has_delete_permission': self.has_delete_permission(request, obj),
-    #         'has_file_field': True,
-    #         'has_absolute_url': view_on_site_url is not None,
-    #         'absolute_url': view_on_site_url,
-    #         'form_url': form_url,
-    #         'opts': opts,
-    #         'content_type_id': get_content_type_for_model(self.model).pk,
-    #         'save_as': self.save_as,
-    #         'save_on_top': self.save_on_top,
-    #         'to_field_var': TO_FIELD_VAR,
-    #         'is_popup_var': IS_POPUP_VAR,
-    #         'app_label': app_label,
-    #     })
-    #
-    #     request.current_app = self.admin_site.name
-    #     return TemplateResponse(request, self.view_template or [
-    #         "erp_framework/%s/%s/view.html" % (opts.app_label, opts.model_name),
-    #         "erp_framework/%s/view.html" % opts.app_label,
-    #         'erp_framework/view.html',
-    #         f"{app_settings.ERP_FRAMEWORK_THEME}/view.html",
-    #     ], context)
-
     @csrf_protect_m
     def changelist_view(self, request, extra_context=None):
         extra_context = extra_context or {}
         extra_context["description"] = self.description
         return super(EntityAdmin, self).changelist_view(request, extra_context)
 
     def save_model(self, request, obj, form, change):
@@ -588,17 +501,17 @@
                 new_object = self.save_form(request, form, change=not add)
             else:
                 new_object = form.instance
             formsets, inline_instances = self._create_formsets(
                 request, new_object, change=not add
             )
             if (
-                    all_valid(formsets)
-                    and form_validated
-                    and self.whole_changeform_validation(request, form, formsets, not add)
+                all_valid(formsets)
+                and form_validated
+                and self.whole_changeform_validation(request, form, formsets, not add)
             ):
                 self.pre_save(form, formsets, change=not add)
                 self.save_model(request, new_object, form, not add)
                 self.save_related(request, form, formsets, not add)
                 self.post_save(request, new_object, form, formsets, not add)
                 changeform_saved.send(self.model, instance=new_object, created=add)
 
@@ -669,17 +582,17 @@
             "errors": helpers.AdminErrorList(form, formsets),
             "preserved_filters": self.get_preserved_filters(request),
         }
 
         # Hide the "Save" and "Save and continue" buttons if "Save as New" was
         # previously chosen to prevent the interface from getting confusing.
         if (
-                request.method == "POST"
-                and not form_validated
-                and "_saveasnew" in request.POST
+            request.method == "POST"
+            and not form_validated
+            and "_saveasnew" in request.POST
         ):
             context["show_save"] = False
             context["show_save_and_continue"] = False
             # Use the change template instead of the add template.
             add = False
 
         context.update(extra_context or {})
@@ -687,16 +600,16 @@
         return self.render_change_form(
             request, context, add=add, change=not add, obj=obj, form_url=form_url
         )
 
     def get_actions(self, request):
         actions = super(EntityAdmin, self).get_actions(request)
         if not (
-                app_settings.ERP_FRAMEWORK_ENABLE_ADMIN_DELETE_ALL
-                and request.user.is_superuser
+            app_settings.ERP_FRAMEWORK_ENABLE_ADMIN_DELETE_ALL
+            and request.user.is_superuser
         ):
             if "delete_selected" in actions:
                 del actions["delete_selected"]
         return actions
 
     def get_list_display(self, request):
         list_display = super(EntityAdmin, self).get_list_display(request)
@@ -823,16 +736,15 @@
 
         elif type(self.permission_override_model) is ModelBase:
             return self.permission_override_model._meta.model_name
 
         else:
             raise ImproperlyConfigured(
                 "self.permission_override_model can be True, False , str or ModelBase"
-                " .Got %s instead "
-                % type(self.permission_override_model)
+                " .Got %s instead " % type(self.permission_override_model)
             )
 
     def has_add_permission(self, request, obj=None):
         if self.opts.auto_created:
             # We're checking the rights to an auto-created intermediate model,
             # which doesn't have its own individual permissions. The user needs
             # to have the change permission for the related model in order to
@@ -909,15 +821,15 @@
         )
         form_field = app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
             self, db_field, form_field, request, **kwargs
         )
         return form_field
 
 
-class RaGenericTabularInline(GenericTabularInline):
+class ERPFrameworkGenericTabularInline(GenericTabularInline):
     """
     Implementation of teh needed methods for Generic Tabular inline with RA
     """
 
     extra = 1
     exclude = (
         "slug",
@@ -957,17 +869,15 @@
                     )
                     formfield.widget = RelatedFieldWidgetWrapper(
                         formfield.widget,
                         db_field.remote_field,
                         self.admin_site,
                         **wrapper_kwargs,
                     )
-        form_field = super(RaGenericTabularInline, self).formfield_for_dbfield(
-            db_field, request, **kwargs
-        )
+        form_field = super().formfield_for_dbfield(db_field, request, **kwargs)
         form_field = app_settings.ERP_ADMIN_DEFAULT_FORMFIELD_FOR_DBFIELD_FUNC(
             self, db_field, form_field, request, **kwargs
         )
         return form_field
 
 
 class PrepopulatedAdmin(object):
@@ -1108,16 +1018,16 @@
                 )
             else:
                 initial_data = self.get_formset_initial(
                     inline, inline_queryset, request, obj, change
                 )
                 # Not here is a necessity, in case you find unuseful revise again
                 if (
-                        inline.__class__ in self.prepopulated_inlines
-                        or not self.prepopulated_inlines
+                    inline.__class__ in self.prepopulated_inlines
+                    or not self.prepopulated_inlines
                 ):
                     FormSet.extra = len(initial_data)
                 if initial_data:
                     formset_params.update({"initial": initial_data})
             formsets.append(FormSet(**formset_params))
             inline_instances.append(inline)
         return formsets, inline_instances
@@ -1143,68 +1053,7 @@
                 formset_form.instance.notes = form.instance.notes
             for copy_item in self.copy_to_inlines:
                 formset_form.instance.__setattr__(
                     copy_item, form.instance.__getattribute__(copy_item)
                 )
 
         formset.save()
-
-# class RaUserAdmin(RaThemeMixin, UserTabularPermissionsMixin, UserAdmin):
-#     enable_view_view = False
-#     date_hierarchy = None
-#     fields = None
-#     list_display_links = ["username"]
-#     change_user_password_template = (
-#         f"{app_settings.ERP_FRAMEWORK_THEME}/auth/user/change_password.html"
-#     )
-#     list_display = ("username", "is_superuser", "last_login", "is_active")
-#
-#     save_on_top = True
-#
-#     fieldsets = (
-#         (None, {"fields": ("username", "password")}),
-#         (_("Personal info"), {"fields": (("first_name", "last_name", "email"),)}),
-#         (
-#             _("Permissions"),
-#             {"fields": (("is_active", "is_superuser"), "groups", "user_permissions")},
-#         ),
-#         # (_('Important dates'), {'fields': (('last_login', 'date_joined'),)}),
-#     )
-#     list_filter = ("is_superuser", "is_active", "groups")
-#     form = CustomUserChangeForm
-#
-#     def get_actions(self, request):
-#         actions = super(RaUserAdmin, self).get_actions(request)
-#         if "delete_selected" in actions:
-#             del actions["delete_selected"]
-#         return actions
-#
-#     def has_delete_permission(self, request, obj=None):
-#         return False
-#
-#     def save_model(self, request, obj, form, change):
-#         obj.is_staff = True
-#         super(RaUserAdmin, self).save_model(request, obj, form, change)
-#
-#     def get_inline_instances(self, request, obj=None):
-#         if obj is None:
-#             return []
-#         return super(RaUserAdmin, self).get_inline_instances(request, obj)
-#
-#     def changelist_view(self, request, extra_context=None):
-#         extra_context = {"has_detached_sidebar": True}
-#         return super(RaUserAdmin, self).changelist_view(request, extra_context)
-#
-#
-# class RaGroupAdmin(RaThemeMixin, GroupTabularPermissionsMixin, GroupAdmin):
-#     enable_view_view = False
-#     date_hierarchy = None
-#     fields = None
-#     list_display_links = ["name"]
-#     list_display = ["name"]
-#
-#     save_on_top = True
-#
-#
-#
-# erp_admin_site.register(Group, RaGroupAdmin)
-# erp_admin_site.register(User, RaUserAdmin)
```

### Comparing `django-erp-framework-1.5.0/erp_framework/admin/base.py` & `django-erp-framework-1.5.2/erp_framework/admin/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,87 @@
 from __future__ import unicode_literals
 
 import logging
-from functools import update_wrapper
+from typing import Any
 
 from django.apps import apps
 from django.contrib.admin import AdminSite
 from django.http import JsonResponse
 from django.shortcuts import render
 from django.template.response import TemplateResponse
 from django.urls import re_path as url, include
-from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 
 from erp_framework.admin.helpers import get_each_context
 from erp_framework.base import app_settings
 
-# from erp_framework.top_search.views import TopSearchView
-
 logger = logging.getLogger(__name__)
-CACHE_DURATION = 0
-
-MSG_ADDED_SUCCESSFULLY = _('The %(name)s "%(obj)s" was added successfully.')
-MSG_CHANGED_SUCCESSFULLY = _('The %(name)s "%(obj)s" was changed successfully.')
-MSG_YOU_MAY_ADD = _("You may add another %(name)s below")
-MSG_YOU_MAY_CHANGE = _("You may change it again below.")
-
-
-def get_report_list_class(request, base_model):
-    from erp_framework.base.app_settings import RA_REPORT_LIST_MAP
-    from erp_framework.reporting.views import ReportList
-
-    klass = RA_REPORT_LIST_MAP.get(base_model, False)
-    if klass:
-        klass = import_string(klass)
-        if callable(klass):
-            return klass(request, base_model=base_model)
-    else:
-        klass = ReportList
-
-    return klass.as_view()(request, base_model=base_model)
-
-
-def get_report_view(request, base_model, report_slug):
-    from erp_framework.reporting.registry import report_registry
-
-    klass = report_registry.get(base_model, report_slug)
-    return klass.as_view()(request)
 
 
 class ERPFrameworkAdminSiteBase(AdminSite):
     site_title = app_settings.ERP_ADMIN_SITE_TITLE
     site_header = app_settings.ERP_ADMIN_SITE_HEADER
     index_title = app_settings.ERP_ADMIN_INDEX_TITLE
 
-    index_template = app_settings.ERP_ADMIN_INDEX_TEMPLATE
-    app_index_template = app_settings.ERP_FRAMEWORK_APP_INDEX_TEMPLATE
-    login_template = app_settings.ERP_FRAMEWORK_LOGIN_TEMPLATE
-    logout_template = app_settings.ERP_FRAMEWORK_LOGGED_OUT_TEMPLATE
+    # index_template = app_settings.ERP_ADMIN_INDEX_TEMPLATE
+    # app_index_template = app_settings.ERP_FRAMEWORK_APP_INDEX_TEMPLATE
+    # login_template = app_settings.ERP_FRAMEWORK_LOGIN_TEMPLATE
+    # logout_template = app_settings.ERP_FRAMEWORK_LOGGED_OUT_TEMPLATE
+
+    admin_base_site_template = None
+
+    def __getattribute__(self, name: str) -> Any:
+        output = super().__getattribute__(name)
+        if (
+            name
+            in [
+                "index_template",
+                "login_template",
+                "logout_template",
+                "app_index_template",
+            ]
+            and output is None
+        ):
+            return app_settings.get_template(name, self.name)
+        return output
 
-    def get_urls(self):
-        # from erp_framework.utils.views import access_denied
-        def wrap(view, cacheable=False):
-            def wrapper(*args, **kwargs):
-                return self.admin_view(view, cacheable)(*args, **kwargs)
-
-            return update_wrapper(wrapper, view)
+    def has_permission(self, request):
+        return app_settings.admin_site_access_permission(request)
 
+    def get_urls(self):
         urls = super(ERPFrameworkAdminSiteBase, self).get_urls()
         help_center = [url(r"^i18n/", include("django.conf.urls.i18n"))]
 
         settings_update = [
             url(r"^manifest/$", self.manifest_view, name="manifest"),
             url(r"^sw.js$", self.service_worker_view, name="service-worker"),
         ]
 
         urlpatterns = [
-            url(
-                r"^reports/(?P<base_model>[\w-]+)/$",
-                get_report_list_class,
-                name="report_list",
-            ),
+            # url(
+            #     r"^reports/(?P<base_model>[\w-]+)/$",
+            #     get_report_list_class,
+            #     name="report_list",
+            # ),
             url(
                 r"^reports/(?P<base_model>[\w-]+)/(?P<report_slug>[\w-]+)/$",
-                get_report_view,
+                self.get_report_view,
                 name="report",
             ),
-            # new from sites
-            # path('top-search/', TopSearchView.as_view(), name='top-search'),
-            # path('access-denied/', access_denied, name='access-denied'),
         ]
 
         return help_center + settings_update + urlpatterns + urls
 
+    def get_report_view(self, request, base_model, report_slug):
+        request.current_app = self.name
+        from erp_framework.reporting.registry import report_registry
+
+        klass = report_registry.get(base_model, report_slug, admin_site=self.name)
+        return klass.as_view()(request)
+
     def service_worker_view(self, request):
         return render(
             request,
             f"erp_framework/service-worker.js.html",
             content_type="application/javascript",
         )
 
@@ -123,40 +109,17 @@
             "start_url": "../?launcher=true",
             "display": "standalone",
             "theme_color": "#000066",
             "background_color": "#fff",
         }
         return JsonResponse(json, status=200)
 
-    def __init__(self, name="admin"):
-        super(ERPFrameworkAdminSiteBase, self).__init__(name)
-
-        self._registry_names = {}  # holds model name -> ModelAdmin instances
-        #                  l-> Model
-        self._registered_models_CT = []
-
-    def _fill_registry_names(self):
-        """
-        Fills the `self._registry_names`
-        """
-        for model in self._registry.keys():
-            try:
-                model_name = model.get_class_name().lower()
-            except AttributeError:
-                model_name = model._meta.model_name.lower()
-            self._registry_names[model_name] = {
-                "admin": self._registry[model],
-                "model": model,
-            }
-
     def app_index(self, request, app_label, extra_context=None):
         app_name = apps.get_app_config(app_label).verbose_name
         context = self.each_context(request)
-        # app_list = context["app_list"]
-        # current_app_list = get_from_list(False, app_list, "app_label", app_label)
         context.update(
             dict(
                 title=_("%(app)s administration") % {"app": app_name},
                 # current_app_list=[app_dict],
                 # current_app_list=[current_app_list],
                 app_label=app_label,
                 app_name=app_name,
@@ -169,41 +132,31 @@
             request,
             self.app_index_template
             or ["admin/%s/app_index.html" % app_label, "admin/app_index.html"],
             context,
         )
 
     def index(self, request, extra_context=None):
-        extra_context = extra_context or {}
-        extra_context["opts"] = {"app_name": "home"}
-        extra_context["is_index"] = True
-        extra_context["sidebar_status"] = "expanded"
-        context = dict(self.each_context(request), name=self.index_title)
-        context.update(extra_context or {})
+        app_list = self.get_app_list(request)
+        context = {
+            **self.each_context(request),
+            "title": app_settings.ERP_ADMIN_INDEX_TITLE,
+            "subtitle": None,
+            "app_list": app_list,
+            **(extra_context or {}),
+        }
 
         request.current_app = self.name
-        context["title"] = app_settings.ERP_ADMIN_INDEX_TITLE
 
         return TemplateResponse(
             request, self.index_template or "admin/index.html", context
         )
 
     def each_context(self, request):
         context = super(ERPFrameworkAdminSiteBase, self).each_context(request)
-        context["ERP_FRAMEWORK_SITE_NAME"] = app_settings.ERP_FRAMEWORK_SITE_NAME
+        context[
+            "admin_base_site_template"
+        ] = self.admin_base_site_template or app_settings.get_admin_base_template(
+            self.name
+        )
         context.update(get_each_context(request, self))
         return context
-
-    def get_admin_by_model_name(self, model_name):
-        """
-        Get the model admin of a model by its name
-        :param model_name:
-        :return: ModalAdmin Instance or None
-        """
-        if not self._registry_names:
-            self._fill_registry_names()
-        return self._registry_names.get(model_name, None)
-
-    def login(self, request, extra_context=None):
-        extra_context = extra_context or {}
-        # extra_context["SHOW_LANGUAGE_SELECTOR"] = True
-        return super(ERPFrameworkAdminSiteBase, self).login(request, extra_context)
```

### Comparing `django-erp-framework-1.5.0/erp_framework/admin/helpers.py` & `django-erp-framework-1.5.2/erp_framework/admin/helpers.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/base/app_settings.py` & `django-erp-framework-1.5.2/erp_framework/base/app_settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,14 +13,21 @@
     # only you need to add a help text or something
     "admin_default_formfield_for_dbfield": (
         "erp_framework.base.helpers.default_formfield_for_dbfield"
     ),
     "admin_site_class": "erp_framework.admin.admin.ERPFrameworkAdminSite",
     "admin_site_namespace": "erp_framework",
     "enable_delete_all": False,
+    "admin_site_access_permission": "erp_framework.base.helpers.admin_site_access_permission",
+    "report_access_function": "erp_framework.base.helpers.report_access_function",
+    "admin_base_site_template": "admin/base.html",
+    "report_base_template": "erp_framework/base_site.html",
+    "reports_list_view_class": "",  # todo
+    "reports_root_view_class": "",  # todo
+    "sites": {},
 }
 
 USER_FRAMEWORK_SETTINGS = getattr(settings, "ERP_FRAMEWORK_SETTINGS", {})
 
 ERP_FRAMEWORK_SETTINGS.update(USER_FRAMEWORK_SETTINGS)
 
 """
@@ -67,7 +74,51 @@
 ERP_FRAMEWORK_LOGGED_OUT_TEMPLATE = ERP_FRAMEWORK_SETTINGS.get(
     "logout_template", "admin/logout.html"
 )
 
 ERP_FRAMEWORK_ENABLE_ADMIN_DELETE_ALL = ERP_FRAMEWORK_SETTINGS.get(
     "enable_delete_all", False
 )
+
+
+admin_site_access_permission = get_callable(
+    ERP_FRAMEWORK_SETTINGS.get(
+        "admin_site_access_permission",
+        "erp_framework.base.helpers.admin_site_access_permission",
+    )
+)
+
+report_access_function = get_callable(
+    ERP_FRAMEWORK_SETTINGS.get(
+        "report_access_function", "erp_framework.base.helpers.report_access_function"
+    )
+)
+
+report_base_template = ERP_FRAMEWORK_SETTINGS.get(
+    "report_base_template", "erp_framework/base_site.html"
+)
+
+admin_base_site_template = ERP_FRAMEWORK_SETTINGS.get(
+    "admin_base_site_template", "erp_framework/base_site.html"
+)
+
+
+def get_admin_base_template(site=None):
+    admin_base_site_template = ERP_FRAMEWORK_SETTINGS.get(
+        "admin_base_site_template", "erp_framework/base_site.html"
+    )
+
+    if site:
+        # breakpoint()
+        admin_base_site_template = (
+            ERP_FRAMEWORK_SETTINGS["sites"]
+            .get(site, {})
+            .get("admin_base_site_template", admin_base_site_template)
+        )
+    return admin_base_site_template
+
+
+def get_template(name, site=None):
+    template = ERP_FRAMEWORK_SETTINGS.get(name, "")
+    if site:
+        template = ERP_FRAMEWORK_SETTINGS["sites"].get(site, {}).get(name, template)
+    return template
```

### Comparing `django-erp-framework-1.5.0/erp_framework/base/helpers.py` & `django-erp-framework-1.5.2/erp_framework/base/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from collections.abc import Iterable
 
 from django.apps import apps
+from django.conf import settings
 from django.db.models import Max
 
 logger = logging.getLogger(__name__)
 
 get_model = apps.get_model
 
 
@@ -219,7 +220,24 @@
 
 def flatten_list(items):
     for x in items:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from flatten_list(x)
         else:
             yield x
+
+
+def admin_site_access_permission(request):
+    if settings.DEBUG:
+        return True
+    return request.user.is_active and request.user.is_staff
+
+
+def report_access_function(request, permission, report):
+    from erp_framework.reporting.registry import report_registry
+
+    if settings.DEBUG:
+        return True
+
+    return report_registry.has_perm(
+        request.user, report.get_report_code(), permission=permission
+    )
```

### Comparing `django-erp-framework-1.5.0/erp_framework/base/models.py` & `django-erp-framework-1.5.2/erp_framework/base/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -84,31 +84,14 @@
         return the class name, usable when a erp_framework model is mimicking (ie:proxying)
         another model.
         This method is used is get_doc_type_* functions,
         This method is made to avoid to repeat registered type to make adjustments
         """
         return cls.__name__
 
-    @classmethod
-    def get_model_name(cls):
-        """
-        A convenience method to get the base model name, needed in templates
-        :return:
-        """
-
-        return cls._meta.model_name.lower()
-
-    @classmethod
-    def get_verbose_name_plural(cls):
-        """
-        A convenience method to get the base model verbose name, needed in templates
-        :return:
-        """
-        return cls._meta.verbose_name_plural
-
 
 class EntityModel(ERPMixin, RAModel):
     """
     The Main base for ERP framework `static` models
     Example: Client , Expense etc..
     """
 
@@ -181,72 +164,14 @@
             if not self.lastmod_user_id and self.owner_id:
                 self.lastmod_user_id = self.owner_id
 
         self.lastmod = now()
 
         super(EntityModel, self).save(*args, **kwargs)
 
-    @classmethod
-    def _get_doc_type_plus_list(cls):
-        """
-
-        Returns List of Identified doctype that a plus effect on the entity
-        """
-        return []
-        # return ["fb"] + registry.get_model_doc_type_map(cls.get_class_name()).get(
-        #     "plus_list", []
-        # )
-
-    @classmethod
-    def _get_doc_type_minus_list(cls):
-        """Returns List of Identified doctype that a minus effect on the entity"""
-        return []
-        # return registry.get_model_doc_type_map(cls.get_class_name()).get(
-        #     "minus_list", []
-        # )
-
-    @classmethod
-    def get_doc_type_neuter_list(cls):
-        """Returns List of Identified doctype that have a neuttral effect on the entity"""
-
-        return []
-
-    #
-    # @classmethod
-    # def get_doc_type_full_map(cls):
-    #     from .registry import model_doc_type_full_map
-    #
-    #     doc_types_unfiltered = model_doc_type_full_map.get(cls.get_class_name(), [])
-    #     doc_typed_filtered = []
-    #     for type in doc_types_unfiltered:
-    #         if not type.get('hidden', False):
-    #             doc_typed_filtered.append(type)
-    #
-    #     return doc_typed_filtered
-
-    # @classmethod
-    # def get_doc_types(cls):
-    #     """
-    #     Return a list of the doc_types supported by the current model , Must implemented when needed by children
-    #     @return:
-    #     """
-    #     return cls._get_doc_type_plus_list() + cls._get_doc_type_minus_list() + cls.get_doc_type_neuter_list()
-
-    @classmethod
-    def get_report_list_url(cls):
-        """
-        Return the url for the report list for this model
-        :return: a string url
-        """
-        # todo consider deleting
-        return reverse(
-            "%s:report_list" % app_settings.ERP_FRAMEWORK_SITE_NAME,
-            args=(cls.get_class_name().lower(),),
-        )
-
 
 class TransactionModel(EntityModel):
     name = None
 
     slug = models.SlugField(
         _("Slug"), max_length=50, db_index=True, validators=[], blank=True
     )
@@ -364,51 +289,23 @@
     lastmod_user = models.ForeignKey(
         User,
         related_name="%(app_label)s_%(class)s_lastmod_related",
         verbose_name=_("Last modification by"),
         on_delete=models.DO_NOTHING,
     )
 
-    @classmethod
-    def get_doc_type_plus_list(cls):
-        """
-
-        Returns List of Identified doctype that a plus effect on the entity
-        """
-        return []
-
-    @classmethod
-    def get_doc_type_minus_list(cls):
-        """Returns List of Identified doctype that a minus effect on the entity"""
-
-        return []
-
     class Meta:
         abstract = True
         default_permissions = ()
 
 
 class QuanValueReport(BaseReportModel):
     quantity = models.DecimalField(
         _("quantity"), max_digits=19, decimal_places=2, default=0
     )
     price = models.DecimalField(_("price"), max_digits=19, decimal_places=2, default=0)
     discount = models.DecimalField(
         _("discount"), max_digits=19, decimal_places=2, default=0
     )
 
-    @classmethod
-    def get_doc_type_plus_list(cls):
-        """
-
-        Returns List of Identified doctype that a plus effect on the entity
-        """
-        return []
-
-    @classmethod
-    def get_doc_type_minus_list(cls):
-        """Returns List of Identified doctype that a minus effect on the entity"""
-
-        return []
-
     class Meta:
         abstract = True
```

### Comparing `django-erp-framework-1.5.0/erp_framework/checks.py` & `django-erp-framework-1.5.2/erp_framework/checks.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/doc_types.py` & `django-erp-framework-1.5.2/erp_framework/doc_types.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/reporting/admin.py` & `django-erp-framework-1.5.2/erp_framework/reporting/admin.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/reporting/apps.py` & `django-erp-framework-1.5.2/erp_framework/reporting/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 from django import apps
 from django.db import ProgrammingError, OperationalError
-from django.db.models.signals import post_migrate
 
 
 def autodiscover():
-    import os
-    import sys
-    import copy
-    from django.utils.module_loading import module_has_submodule
-
     from importlib import import_module
     from django.apps import apps
 
     mods = [
         (app_config.name, app_config.module) for app_config in apps.get_app_configs()
     ]
 
@@ -28,24 +22,28 @@
                 raise e
 
 
 def sync_reports():
     from .models import Report
     from .registry import report_registry
 
-    reports = report_registry.get_all_reports()
+    reports = report_registry.get_all_reports(all_sites=True)
 
     try:
         reports_in_db = list(Report.objects.all().values_list("code", flat=True))
     except (ProgrammingError, OperationalError):
         # Before first migrations
         return
 
     for report_klass in reports:
-        code = f"{report_klass.get_base_model_name()}.{report_klass.get_report_slug()}"
+        try:
+            base_model_name = report_klass.get_base_model_name()
+        except AttributeError:
+            base_model_name = report_klass.__module__.split(".")[0]
+        code = f"{base_model_name}.{report_klass.get_report_slug()}"
         c, created = Report.objects.update_or_create(
             code=code,
         )
         c.deleted = False
         c.save()
         try:
             reports_in_db.remove(code)
```

### Comparing `django-erp-framework-1.5.0/erp_framework/reporting/forms.py` & `django-erp-framework-1.5.2/erp_framework/reporting/forms.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/reporting/migrations/0001_initial.py` & `django-erp-framework-1.5.2/erp_framework/reporting/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/reporting/models.py` & `django-erp-framework-1.5.2/erp_framework/reporting/models.py`

 * *Files identical despite different names*

### Comparing `django-erp-framework-1.5.0/erp_framework/reporting/printing.py` & `django-erp-framework-1.5.2/erp_framework/reporting/printing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,28 @@
 # from __future__ import unicode_literals
 import logging
 
 import csv
 from django.http import HttpResponse
 from django.shortcuts import render
 
-from erp_framework.utils.views import re_time_series
-from erp_framework.base import app_settings
 
 logger = logging.getLogger(__name__)
 
 
 def regroup_data(obj_list, header_report, key):
     values = {}
     for line in obj_list:
         key_value = line[key]
         if key_value not in values:
             values[key_value] = []
         values[key_value].append(line)
     return values
 
 
-# def is_time_series(name):
-#     is_time_field = re_time_series.findall(name)
-#     return is_time_field or False
-
-#
-# def is_partial_text_in_list(text, lst):
-#     check = False
-#     for item in lst:
-#         if text in item:
-#             check = True
-#             break
-#     return check
-#
-
-
 class HTMLPrintingClass(object):
     def __init__(
         self,
         request,
         form_settings,
         response,
         header_report=None,
```

### Comparing `django-erp-framework-1.5.0/erp_framework/reporting/templatetags/erp_reporting_tags.py` & `django-erp-framework-1.5.2/erp_framework/reporting/templatetags/erp_reporting_tags.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,64 +8,99 @@
 
 from erp_framework.base import app_settings
 
 register = template.Library()
 
 
 @register.simple_tag(takes_context=True)
-def render_reports_menu(context, template_name="erp_framework/reports_menu.html"):
+def get_report_url(context, report):
+    request = context.get("request", None)
+    return report.get_url(request=request)
+
+
+@register.simple_tag(takes_context=True)
+def render_reports_menu(context, template_name="reporting/flat_menu.html", flat=True):
     request = context["request"]
-    is_in_reports = False
-    active_base_model = ""
-    if request.path.startswith("/reports/"):
-        is_in_reports = True
-        active_base_model = [x for x in request.path.split("/") if x][1]
+    base_models = []
+    reports = []
 
     from erp_framework.reporting.registry import report_registry
 
-    base_models = report_registry.get_base_models_with_reports()
-    if base_models:
-        output = render_to_string(
-            template_name,
-            {
-                "base_models_reports_tuple": base_models,
-                "is_report": context.get("is_report", False),
-                "base_model": context.get("base_model", False),
-                "report_slug": context.get("report_slug", False),
-                "current_base_model_name": context.get(
-                    "current_base_model_name", False
-                ),
-            },
-            request,
-        )
-        return mark_safe(output)
-    return ""
+    try:
+        current_app = request.current_app
+    except:
+        current_app = None
+
+    if flat:
+        reports = report_registry.get_all_reports(admin_site=current_app)
+    else:
+        base_models = report_registry.get_base_models_with_reports()
+    # if base_models:
+    output = render_to_string(
+        template_name,
+        {
+            "reports": reports,
+            "base_models_reports_tuple": base_models,
+            "is_report": context.get("is_report", False),
+            "base_model": context.get("base_model", False),
+            "report_slug": context.get("report_slug", False),
+            "CURRENT_REPORT": context.get("CURRENT_REPORT", None),
+        },
+        request,
+    )
+    return mark_safe(output)
+
+
+@register.simple_tag(takes_context=True)
+def is_active_report(
+    context,
+    report,
+):
+    current_report = context.get("CURRENT_REPORT", None)
+
+    return current_report == report.__class__
 
 
 @register.simple_tag(takes_context=True)
 def get_report(context, base_model, report_slug):
     from erp_framework.reporting.registry import report_registry
 
-    return report_registry.get(namespace=base_model, report_slug=report_slug)
+    request = context["request"]
+    try:
+        current_app = request.current_app
+    except AttributeError:
+        current_app = app_settings.ERP_FRAMEWORK_SITE_NAME
 
+    return report_registry.get(
+        namespace=base_model, report_slug=report_slug, admin_site=current_app
+    )
 
-@register.simple_tag()
-def get_model_verbose_name_plural(model):
-    return capfirst(model._meta.verbose_name_plural)
 
+@register.simple_tag
+def get_widget(report, template_name="", **kwargs):
+    kwargs["report"] = report
+    if not report:
+        raise ValueError(
+            "report argument is empty. Are you sure you're using the correct report name"
+        )
+    # if not report.chart_settings:
+    kwargs.setdefault("display_chart", bool(report.chart_settings))
+    kwargs.setdefault("display_table", True)
 
-@register.simple_tag(takes_context=True)
-def get_report_active_class(context, base_model, css_class=None):
-    css_class = css_class or "active"
-    current_base_model_name = context["current_base_model_name"]
-    return (
-        css_class
-        if current_base_model_name == base_model._meta.model_name.lower()
-        else ""
-    )
+    kwargs.setdefault("display_chart_selector", kwargs["display_chart"])
+    kwargs.setdefault("display_title", True)
+
+    passed_title = kwargs.get("title", None)
+    kwargs["title"] = passed_title or report.get_report_title()
+
+    kwargs.setdefault("extra_params", "")
+
+    template = get_template(template_name or "erp_framework/widget_template.html")
+
+    return template.render(context=kwargs)
 
 
 @register.simple_tag
 def get_html_panel(report, template_name="", **kwargs):
     kwargs["report"] = report
     if not report:
         raise ValueError(
@@ -77,7 +112,12 @@
     kwargs.setdefault("data_display_chart_selector", kwargs["no_chart"])
     kwargs.setdefault("title", report.get_report_title())
 
     template = get_template(
         template_name or "erp_framework/report_widget_template.html"
     )
     return template.render(context=kwargs)
+
+
+@register.simple_tag
+def get_erp_settings():
+    return app_settings.ERP_FRAMEWORK_SETTINGS
```

### Comparing `django-erp-framework-1.5.0/setup.cfg` & `django-erp-framework-1.5.2/setup.cfg`

 * *Files identical despite different names*

