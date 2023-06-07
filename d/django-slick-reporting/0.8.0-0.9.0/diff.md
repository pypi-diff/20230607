# Comparing `tmp/django-slick-reporting-0.8.0.tar.gz` & `tmp/django-slick-reporting-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-slick-reporting-0.8.0.tar", last modified: Sun May 28 11:13:17 2023, max compression
+gzip compressed data, was "django-slick-reporting-0.9.0.tar", last modified: Wed Jun  7 08:55:44 2023, max compression
```

## Comparing `django-slick-reporting-0.8.0.tar` & `django-slick-reporting-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/
--rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-0.8.0/LICENSE.md
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-0.8.0/MANIFEST.in
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9291 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7604 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/README.rst
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.148920 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9291 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/PKG-INFO
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1200 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/SOURCES.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/SOURCES.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/dependency_links.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/dependency_links.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/requires.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/requires.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-05-28 11:13:17.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/top_level.txt
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-0.8.0/django_slick_reporting.egg-info/top_level.txt.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/setup.cfg
--rw-rw-r--   0 ramez     (1000) ramez     (1000)       37 2019-12-25 18:25:30.000000 django-slick-reporting-0.8.0/setup.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1688 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/app_settings.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      207 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/apps.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/decorators.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    16896 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/fields.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     8247 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/form_factory.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    38156 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/generator.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1565 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/helpers.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1693 2023-05-15 07:49:20.000000 django-slick-reporting-0.8.0/slick_reporting/registry.py
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.144920 django-slick-reporting-0.8.0/slick_reporting/static/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     7123 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    19417 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/main.js
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.144920 django-slick-reporting-0.8.0/slick_reporting/templates/
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     1937 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/base.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)     9397 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/simple_report.html
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/table.html
-drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-05-28 11:13:17.152920 django-slick-reporting-0.8.0/slick_reporting/templatetags/
--rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-0.8.0/slick_reporting/templatetags/__init__.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2022-07-07 07:19:02.000000 django-slick-reporting-0.8.0/slick_reporting/templatetags/slick_reporting_tags.py
--rw-rw-r--   0 ramez     (1000) ramez     (1000)    14341 2023-05-28 11:12:25.000000 django-slick-reporting-0.8.0/slick_reporting/views.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/
+-rw-r--r--   0 ramez     (1000) ramez     (1000)     1518 2020-04-23 10:03:51.000000 django-slick-reporting-0.9.0/LICENSE.md
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      152 2020-06-07 07:01:50.000000 django-slick-reporting-0.9.0/MANIFEST.in
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9292 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7605 2023-06-05 12:49:44.000000 django-slick-reporting-0.9.0/README.rst
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.696882 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     9292 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/PKG-INFO
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1285 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/SOURCES.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1003 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/SOURCES.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/dependency_links.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/dependency_links.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       71 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/requires.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       66 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/requires.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2023-06-07 08:55:44.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/top_level.txt
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       22 2021-07-15 08:55:50.000000 django-slick-reporting-0.9.0/django_slick_reporting.egg-info/top_level.txt.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1675 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/setup.cfg
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)       38 2023-06-05 11:59:25.000000 django-slick-reporting-0.9.0/setup.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      104 2023-06-07 08:55:39.000000 django-slick-reporting-0.9.0/slick_reporting/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1638 2023-06-06 12:54:30.000000 django-slick-reporting-0.9.0/slick_reporting/app_settings.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      214 2023-06-06 12:41:34.000000 django-slick-reporting-0.9.0/slick_reporting/apps.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      722 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/decorators.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    17166 2023-06-06 12:41:34.000000 django-slick-reporting-0.9.0/slick_reporting/fields.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      198 2023-06-06 12:40:41.000000 django-slick-reporting-0.9.0/slick_reporting/form_factory.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    11412 2023-06-06 12:36:51.000000 django-slick-reporting-0.9.0/slick_reporting/forms.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    38650 2023-06-06 12:41:56.000000 django-slick-reporting-0.9.0/slick_reporting/generator.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1565 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/helpers.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1693 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/registry.py
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.696882 django-slick-reporting-0.9.0/slick_reporting/static/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     7123 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    19417 2023-05-30 09:54:31.000000 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1697 2020-12-11 18:31:17.000000 django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/main.js
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.696882 django-slick-reporting-0.9.0/slick_reporting/templates/
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     1624 2023-06-04 13:48:28.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/base.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     2382 2023-06-04 14:00:22.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/js_resources.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)     4841 2023-06-04 14:16:10.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/simple_report.html
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      448 2020-07-24 10:59:05.000000 django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/table.html
+drwxrwxr-x   0 ramez     (1000) ramez     (1000)        0 2023-06-07 08:55:44.700882 django-slick-reporting-0.9.0/slick_reporting/templatetags/
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)        1 2019-11-14 16:41:29.000000 django-slick-reporting-0.9.0/slick_reporting/templatetags/__init__.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)      780 2023-06-05 11:59:25.000000 django-slick-reporting-0.9.0/slick_reporting/templatetags/slick_reporting_tags.py
+-rw-rw-r--   0 ramez     (1000) ramez     (1000)    18181 2023-06-06 12:42:49.000000 django-slick-reporting-0.9.0/slick_reporting/views.py
```

### Comparing `django-slick-reporting-0.8.0/LICENSE.md` & `django-slick-reporting-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/PKG-INFO` & `django-slick-reporting-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.8.0
+Version: 0.9.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
@@ -85,40 +85,44 @@
 So you have a model that contains data, let's call it `MySalesItems`
 
 You can simply use a code like this
 
 .. code-block:: python
 
     # in your urls.py
-    path('path-to-report', TotalProductSales.as_view())
+    path("path-to-report", TotalProductSales.as_view())
 
 
     # in views.py
     from django.db.models import Sum
-    from slick_reporting.views import SlickReportView
+    from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
-    class TotalProductSales(SlickReportView):
 
-        report_model = MySalesItems
-        date_field = 'date_placed'
-        group_by = 'product'
-        columns = ['title',
-                    SlickReportField.create(Sum, 'quantity') ,
-                    SlickReportField.create(Sum, 'value', name='sum__value') ]
-
-        chart_settings = [{
-            'type': 'column',
-            'data_source': ['sum__value'],
-            'plot_total': False,
-            'title_source': 'title',
-            'title': _('Detailed Columns'),
+    class TotalProductSales(ReportView):
 
-        }, ]
+        report_model = MySalesItems
+        date_field = "date_placed"
+        group_by = "product"
+        columns = [
+            "title",
+            SlickReportField.create(Sum, "quantity"),
+            SlickReportField.create(Sum, "value", name="sum__value"),
+        ]
+
+        chart_settings = [
+            {
+                "type": "column",
+                "data_source": ["sum__value"],
+                "plot_total": False,
+                "title_source": "title",
+                "title": _("Detailed Columns"),
+            },
+        ]
 
 
 To get something like this
 
 .. image:: https://i.ibb.co/SvxTM23/Selection-294.png
     :target: https://i.ibb.co/SvxTM23/Selection-294.png
     :alt: Shipped in View Page
@@ -126,27 +130,30 @@
 
 You can do a monthly time series :
 
 
 .. code-block:: python
 
     # in views.py
-    from slick_reporting.views import SlickReportView
+    from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
-    class MonthlyProductSales(SlickReportView):
+
+    class MonthlyProductSales(ReportView):
         report_model = MySalesItems
-        date_field = 'date_placed'
-        group_by = 'product'
-        columns = ['name', 'sku']
+        date_field = "date_placed"
+        group_by = "product"
+        columns = ["name", "sku"]
 
         # Analogy for time series
-        time_series_pattern = 'monthly'
-        time_series_columns = [SlickReportField.create(Sum, 'quantity', name='sum__quantity') ]
+        time_series_pattern = "monthly"
+        time_series_columns = [
+            SlickReportField.create(Sum, "quantity", name="sum__quantity")
+        ]
 
 
 This would return a table looking something like this:
 
 +--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
 | Product Name | SKU                  | Total Quantity  | Total Quantity | Total Quantity in ... | Total Quantity in December 20 |
 |              |                      | in Jan 20       | in Feb 20      |                       |                               |
@@ -161,26 +168,25 @@
 *This example code assumes your "MySalesItems" model contains the fields `product` as foreign key,  `quantity` as number , and `date_placed` as a date field. It also assumes your `Product` model has an SKU field.. Change those to better suit your structure.*
 
 
 --
 
 **On a low level**
 
-You can interact with the `ReportGenerator` using same syntax as used with the `SlickReportView` .
+You can interact with the `ReportGenerator` using same syntax as used with the `ReportView` .
 
 .. code-block:: python
 
     from slick_reporting.generator import ReportGenerator
-    from . models import MySalesModel
+    from .models import MySalesModel
 
-    report = ReportGenerator(report_model=MySalesModel,
-                            group_by='product',
-                            columns=['title', '__total__']
+    report = ReportGenerator(
+        report_model=MySalesModel, group_by="product", columns=["title", "__total__"]
     )
-    report.get_report_data() #-> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
+    report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
 
 
 This is just a scratch, for more please visit the documentation 
 
 Batteries Included
 ------------------
```

### Comparing `django-slick-reporting-0.8.0/README.rst` & `django-slick-reporting-0.9.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -47,40 +47,44 @@
 So you have a model that contains data, let's call it `MySalesItems`
 
 You can simply use a code like this
 
 .. code-block:: python
 
     # in your urls.py
-    path('path-to-report', TotalProductSales.as_view())
+    path("path-to-report", TotalProductSales.as_view())
 
 
     # in views.py
     from django.db.models import Sum
-    from slick_reporting.views import SlickReportView
+    from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
-    class TotalProductSales(SlickReportView):
 
-        report_model = MySalesItems
-        date_field = 'date_placed'
-        group_by = 'product'
-        columns = ['title',
-                    SlickReportField.create(Sum, 'quantity') ,
-                    SlickReportField.create(Sum, 'value', name='sum__value') ]
-
-        chart_settings = [{
-            'type': 'column',
-            'data_source': ['sum__value'],
-            'plot_total': False,
-            'title_source': 'title',
-            'title': _('Detailed Columns'),
+    class TotalProductSales(ReportView):
 
-        }, ]
+        report_model = MySalesItems
+        date_field = "date_placed"
+        group_by = "product"
+        columns = [
+            "title",
+            SlickReportField.create(Sum, "quantity"),
+            SlickReportField.create(Sum, "value", name="sum__value"),
+        ]
+
+        chart_settings = [
+            {
+                "type": "column",
+                "data_source": ["sum__value"],
+                "plot_total": False,
+                "title_source": "title",
+                "title": _("Detailed Columns"),
+            },
+        ]
 
 
 To get something like this
 
 .. image:: https://i.ibb.co/SvxTM23/Selection-294.png
     :target: https://i.ibb.co/SvxTM23/Selection-294.png
     :alt: Shipped in View Page
@@ -88,27 +92,30 @@
 
 You can do a monthly time series :
 
 
 .. code-block:: python
 
     # in views.py
-    from slick_reporting.views import SlickReportView
+    from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
-    class MonthlyProductSales(SlickReportView):
+
+    class MonthlyProductSales(ReportView):
         report_model = MySalesItems
-        date_field = 'date_placed'
-        group_by = 'product'
-        columns = ['name', 'sku']
+        date_field = "date_placed"
+        group_by = "product"
+        columns = ["name", "sku"]
 
         # Analogy for time series
-        time_series_pattern = 'monthly'
-        time_series_columns = [SlickReportField.create(Sum, 'quantity', name='sum__quantity') ]
+        time_series_pattern = "monthly"
+        time_series_columns = [
+            SlickReportField.create(Sum, "quantity", name="sum__quantity")
+        ]
 
 
 This would return a table looking something like this:
 
 +--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
 | Product Name | SKU                  | Total Quantity  | Total Quantity | Total Quantity in ... | Total Quantity in December 20 |
 |              |                      | in Jan 20       | in Feb 20      |                       |                               |
@@ -123,26 +130,25 @@
 *This example code assumes your "MySalesItems" model contains the fields `product` as foreign key,  `quantity` as number , and `date_placed` as a date field. It also assumes your `Product` model has an SKU field.. Change those to better suit your structure.*
 
 
 --
 
 **On a low level**
 
-You can interact with the `ReportGenerator` using same syntax as used with the `SlickReportView` .
+You can interact with the `ReportGenerator` using same syntax as used with the `ReportView` .
 
 .. code-block:: python
 
     from slick_reporting.generator import ReportGenerator
-    from . models import MySalesModel
+    from .models import MySalesModel
 
-    report = ReportGenerator(report_model=MySalesModel,
-                            group_by='product',
-                            columns=['title', '__total__']
+    report = ReportGenerator(
+        report_model=MySalesModel, group_by="product", columns=["title", "__total__"]
     )
-    report.get_report_data() #-> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
+    report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
 
 
 This is just a scratch, for more please visit the documentation 
 
 Batteries Included
 ------------------
```

### Comparing `django-slick-reporting-0.8.0/django_slick_reporting.egg-info/PKG-INFO` & `django-slick-reporting-0.9.0/django_slick_reporting.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slick-reporting
-Version: 0.8.0
+Version: 0.9.0
 Summary: A one-stop report and analytics generation and computation with batteries included
 Home-page: https://django-slick-reporting.com/
 Author: Ra Systems
 Author-email: ramez@rasystems.io
 Project-URL: Travis CI, https://travis-ci.org/ra-systems/django-slick-reporting/
 Project-URL: Documentation, https://django-slick-reporting.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ra-systems/django-slick-reporting
@@ -85,40 +85,44 @@
 So you have a model that contains data, let's call it `MySalesItems`
 
 You can simply use a code like this
 
 .. code-block:: python
 
     # in your urls.py
-    path('path-to-report', TotalProductSales.as_view())
+    path("path-to-report", TotalProductSales.as_view())
 
 
     # in views.py
     from django.db.models import Sum
-    from slick_reporting.views import SlickReportView
+    from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
-    class TotalProductSales(SlickReportView):
 
-        report_model = MySalesItems
-        date_field = 'date_placed'
-        group_by = 'product'
-        columns = ['title',
-                    SlickReportField.create(Sum, 'quantity') ,
-                    SlickReportField.create(Sum, 'value', name='sum__value') ]
-
-        chart_settings = [{
-            'type': 'column',
-            'data_source': ['sum__value'],
-            'plot_total': False,
-            'title_source': 'title',
-            'title': _('Detailed Columns'),
+    class TotalProductSales(ReportView):
 
-        }, ]
+        report_model = MySalesItems
+        date_field = "date_placed"
+        group_by = "product"
+        columns = [
+            "title",
+            SlickReportField.create(Sum, "quantity"),
+            SlickReportField.create(Sum, "value", name="sum__value"),
+        ]
+
+        chart_settings = [
+            {
+                "type": "column",
+                "data_source": ["sum__value"],
+                "plot_total": False,
+                "title_source": "title",
+                "title": _("Detailed Columns"),
+            },
+        ]
 
 
 To get something like this
 
 .. image:: https://i.ibb.co/SvxTM23/Selection-294.png
     :target: https://i.ibb.co/SvxTM23/Selection-294.png
     :alt: Shipped in View Page
@@ -126,27 +130,30 @@
 
 You can do a monthly time series :
 
 
 .. code-block:: python
 
     # in views.py
-    from slick_reporting.views import SlickReportView
+    from slick_reporting.views import ReportView
     from slick_reporting.fields import SlickReportField
     from .models import MySalesItems
 
-    class MonthlyProductSales(SlickReportView):
+
+    class MonthlyProductSales(ReportView):
         report_model = MySalesItems
-        date_field = 'date_placed'
-        group_by = 'product'
-        columns = ['name', 'sku']
+        date_field = "date_placed"
+        group_by = "product"
+        columns = ["name", "sku"]
 
         # Analogy for time series
-        time_series_pattern = 'monthly'
-        time_series_columns = [SlickReportField.create(Sum, 'quantity', name='sum__quantity') ]
+        time_series_pattern = "monthly"
+        time_series_columns = [
+            SlickReportField.create(Sum, "quantity", name="sum__quantity")
+        ]
 
 
 This would return a table looking something like this:
 
 +--------------+----------------------+-----------------+----------------+-----------------------+-------------------------------+
 | Product Name | SKU                  | Total Quantity  | Total Quantity | Total Quantity in ... | Total Quantity in December 20 |
 |              |                      | in Jan 20       | in Feb 20      |                       |                               |
@@ -161,26 +168,25 @@
 *This example code assumes your "MySalesItems" model contains the fields `product` as foreign key,  `quantity` as number , and `date_placed` as a date field. It also assumes your `Product` model has an SKU field.. Change those to better suit your structure.*
 
 
 --
 
 **On a low level**
 
-You can interact with the `ReportGenerator` using same syntax as used with the `SlickReportView` .
+You can interact with the `ReportGenerator` using same syntax as used with the `ReportView` .
 
 .. code-block:: python
 
     from slick_reporting.generator import ReportGenerator
-    from . models import MySalesModel
+    from .models import MySalesModel
 
-    report = ReportGenerator(report_model=MySalesModel,
-                            group_by='product',
-                            columns=['title', '__total__']
+    report = ReportGenerator(
+        report_model=MySalesModel, group_by="product", columns=["title", "__total__"]
     )
-    report.get_report_data() #-> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
+    report.get_report_data()  # -> [{'title':'Product 1', '__total__: 56}, {'title':'Product 2', '__total__: 43}, ]
 
 
 This is just a scratch, for more please visit the documentation 
 
 Batteries Included
 ------------------
```

### Comparing `django-slick-reporting-0.8.0/django_slick_reporting.egg-info/SOURCES.txt` & `django-slick-reporting-0.9.0/django_slick_reporting.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 django_slick_reporting.egg-info/top_level.txt.py
 slick_reporting/__init__.py
 slick_reporting/app_settings.py
 slick_reporting/apps.py
 slick_reporting/decorators.py
 slick_reporting/fields.py
 slick_reporting/form_factory.py
+slick_reporting/forms.py
 slick_reporting/generator.py
 slick_reporting/helpers.py
 slick_reporting/registry.py
 slick_reporting/views.py
 slick_reporting/static/slick_reporting/erp_framework.chartsjs.js
 slick_reporting/static/slick_reporting/erp_framework.highchart.js
 slick_reporting/static/slick_reporting/main.js
 slick_reporting/templates/slick_reporting/base.html
+slick_reporting/templates/slick_reporting/js_resources.html
 slick_reporting/templates/slick_reporting/simple_report.html
 slick_reporting/templates/slick_reporting/table.html
 slick_reporting/templatetags/__init__.py
 slick_reporting/templatetags/slick_reporting_tags.py
```

### Comparing `django-slick-reporting-0.8.0/setup.cfg` & `django-slick-reporting-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/slick_reporting/app_settings.py` & `django-slick-reporting-0.9.0/slick_reporting/app_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import pytz
 from django.conf import settings
 from django.utils.functional import lazy
 
 import datetime
 
-from django.utils.timezone import now
 
 
 def get_first_of_this_year():
     d = datetime.datetime.today()
     return datetime.datetime(d.year, 1, 1, 0, 0)
```

### Comparing `django-slick-reporting-0.8.0/slick_reporting/decorators.py` & `django-slick-reporting-0.9.0/slick_reporting/decorators.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/slick_reporting/fields.py` & `django-slick-reporting-0.9.0/slick_reporting/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import uuid
-
 from django.db.models import Sum
 from django.template.defaultfilters import date as date_filter
 from django.utils.translation import gettext_lazy as _
 
 from .helpers import get_calculation_annotation
 from .registry import field_registry
 
@@ -35,14 +33,19 @@
     type = "number"
     """Just a string describing what this computation field return, usually passed to frontend"""
 
     is_summable = True
     """Indicate if this computation can be summed over. Useful to be passed to frontend or whenever needed"""
 
     report_model = None
+    """The model on which the computation would occur"""
+
+    queryset = None
+    """The queryset on which the computation would occur"""
+
     group_by = None
     plus_side_q = None
     minus_side_q = None
 
     base_kwargs_filters = None
     base_q_filters = None
 
@@ -71,15 +74,14 @@
         :param field: The field on which the computation would occur
         :param name: a name to refer to this field else where
         :param verbose_name: Verbose name
         :param is_summable:
         :return:
         """
         if not name:
-            identifier = str(uuid.uuid4()).split("-")[-1]
             name = name or f"{method.name.lower()}__{field}"
             assert name not in cls._field_registry.get_all_report_fields_names()
 
         verbose_name = verbose_name or f"{method.name} {field}"
         report_klass = type(
             f"ReportField_{name}",
             (cls,),
@@ -94,23 +96,30 @@
         return report_klass
 
     def __init__(
         self,
         plus_side_q=None,
         minus_side_q=None,
         report_model=None,
-        qs=None,
+        queryset=None,
         calculation_field=None,
         calculation_method=None,
         date_field="",
         group_by=None,
     ):
         super(SlickReportField, self).__init__()
         self.date_field = date_field
         self.report_model = self.report_model or report_model
+        self.queryset = self.queryset or queryset
+        self.queryset = (
+            self.report_model._default_manager.all()
+            if self.queryset is None
+            else self.queryset
+        )
+
         self.calculation_field = (
             calculation_field if calculation_field else self.calculation_field
         )
         self.calculation_method = (
             calculation_method if calculation_method else self.calculation_method
         )
         self.plus_side_q = self.plus_side_q or plus_side_q
@@ -197,15 +206,15 @@
                 queryset = self.apply_q_minus_filter(queryset)
 
             credit_results = self.apply_aggregation(queryset, group_by)
 
         return debit_results, credit_results
 
     def get_queryset(self):
-        queryset = self.report_model.objects
+        queryset = self.queryset
         if self.base_q_filters:
             queryset = queryset.filter(*self.base_q_filters)
         if self.base_kwargs_filters:
             queryset = queryset.filter(**self.base_kwargs_filters)
         return queryset.order_by()
 
     def get_annotation_name(self):
```

### Comparing `django-slick-reporting-0.8.0/slick_reporting/generator.py` & `django-slick-reporting-0.9.0/slick_reporting/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals
-
 import datetime
 import logging
 from dataclasses import dataclass
 from inspect import isclass
 
 from django.core.exceptions import ImproperlyConfigured, FieldDoesNotExist
 from django.db.models import Q, ForeignKey
@@ -37,143 +35,145 @@
             data_source=self.data_source,
             title_source=self.title_source,
             plot_total=self.plot_total,
             engine=self.engine,
         )
 
 
-class ReportGenerator(object):
-    """
-    The main class responsible generating the report and managing the flow
-    """
-
-    field_registry_class = field_registry
-    """You can have a custom computation field locator! It only needs a `get_field_by_name(string)` 
-    and returns a ReportField`"""
-
+class ReportGeneratorAPI:
     report_model = None
     """The main model where data is """
 
+    queryset = None
+    """If set, the report will use this queryset instead of the report_model"""
+
     """
     Class to generate a Json Object containing report data.
     """
-    date_field = None
+    date_field = ""
     """Main date field to use whenever date filter is needed"""
 
+    start_date_field_name = None
+    """If set, the report will use this field to filter the start date, default to date_field"""
+
+    end_date_field_name = None
+    """If set, the report will use this field to filter the end date, default to date_field"""
+
     print_flag = None
-    list_display_links = []
 
     group_by = None
     """The field to use for grouping, if not set then the report is expected to be a sub version of the report model"""
 
     columns = None
     """A list of column names.
     Columns names can be 
-    
+
     1. A Computation Field
-    
-    2. If group_by is set, then any field on teh group_by model
-    
+
+    2. If group_by is set, then any field on the group_by model
+
     3. If group_by is not set, then any field name on the report_model / queryset
-     
+
     4. A callable on the generator
-      
+
     5. Special __time_series__, and __crosstab__ 
        Those can be use to control the position of the time series inside the columns, defaults it's appended at the end
-       
+
        Example:
        columns = ['product_id', '__time_series__', 'col_b']
        Same is true with __crosstab__ 
-    
+
     You can customize aspects of the column by adding it as a tuple like this 
         ('field_name', dict(verbose_name=_('My Enhanced Verbose_name'))
-        
-         
+
+
      """
 
     time_series_pattern = ""
     """
     If set the Report will compute a time series.
-    
+
     Possible options are: daily, weekly, semimonthly, monthly, quarterly, semiannually, annually and custom.
-    
+
     if `custom` is set, you'd need to override  `get_custom_time_series_dates`
     """
     time_series_columns = None
     """
     a list of Calculation Field names which will be included in the series calculation.
      Example: ['__total__', '__total_quantity__'] with compute those 2 fields for all the series
-     
+
     """
 
     time_series_custom_dates = None
     """
     Used with `time_series_pattern` set to 'custom'
     It's a list of tuple, each tuple represent start date & end date
     Example: [ (start_date_1, end_date_1), (start_date_2, end_date_2), ....]
     """
 
-    crosstab_model = None
+    crosstab_model = None  # deprecated
+
+    crosstab_field = None
     """
     If set, a cross tab over this model selected ids (via `crosstab_ids`)  
     """
+
     crosstab_columns = None
     """The computation fields which will be computed for each crosstab-ed ids """
 
     crosstab_ids = None
     """A list is the ids to create a crosstab report on"""
 
     crosstab_compute_remainder = True
     """Include an an extra crosstab_columns for the outer group ( ie: all expects those `crosstab_ids`) """
 
-    show_empty_records = True
-    """
-    If group_by is set, this option control if the report result will include all objects regardless of appearing in the report_model/qs.
-    If set False, only those objects which are found in the report_model/qs
-    Example: Say you group by client
-    show_empty_records = True will get the computation fields for all clients in the Client model (including those who 
-    didnt make a transaction.
-    
-    show_empty_records = False will get the computation fields for all clients in the Client model (including those who 
-    didnt make a transaction.
-     
-    """
-
     limit_records = None
-    """Serves are a main limit to  the returned data of teh report_model.
+    """Serves are a main limit to  the returned data of the report_model.
     Can be beneficial if the results may be huge.
     """
     swap_sign = False
 
+
+class ReportGenerator(ReportGeneratorAPI, object):
+    """
+    The main class responsible generating the report and managing the flow
+    """
+
+    field_registry_class = field_registry
+    """You can have a custom computation field locator! It only needs a `get_field_by_name(string)` 
+    and returns a ReportField`"""
+
     def __init__(
         self,
         report_model=None,
         main_queryset=None,
         start_date=None,
         end_date=None,
         date_field=None,
         q_filters=None,
         kwargs_filters=None,
         group_by=None,
         columns=None,
         time_series_pattern=None,
         time_series_columns=None,
         time_series_custom_dates=None,
-        crosstab_model=None,
+        crosstab_field=None,
         crosstab_columns=None,
         crosstab_ids=None,
         crosstab_compute_remainder=None,
         swap_sign=False,
         show_empty_records=None,
         print_flag=False,
         doc_type_plus_list=None,
         doc_type_minus_list=None,
         limit_records=False,
         format_row_func=None,
         container_class=None,
+        start_date_field_name=None,
+        end_date_field_name=None,
     ):
         """
 
         :param report_model: Main model containing the data
         :param main_queryset: Default to report_model.objects
         :param start_date:
         :param end_date:
@@ -197,65 +197,82 @@
         :param limit_records:
         """
         from .app_settings import (
             SLICK_REPORTING_DEFAULT_START_DATE,
             SLICK_REPORTING_DEFAULT_END_DATE,
         )
 
-        super(ReportGenerator, self).__init__()
+        super().__init__()
 
         self.report_model = self.report_model or report_model
-        if not self.report_model:
+        if self.queryset is None:
+            self.queryset = main_queryset
+
+        if not self.report_model and self.queryset is None:
             raise ImproperlyConfigured(
-                "report_model must be set on a class level or via init"
+                "report_model or queryset must be set on a class level or via init"
             )
 
+        main_queryset = (
+            self.report_model.objects if self.queryset is None else self.queryset
+        )
+
         self.start_date = start_date or datetime.datetime.combine(
             SLICK_REPORTING_DEFAULT_START_DATE.date(),
             SLICK_REPORTING_DEFAULT_START_DATE.time(),
         )
 
         self.end_date = end_date or datetime.datetime.combine(
             SLICK_REPORTING_DEFAULT_END_DATE.date(),
             SLICK_REPORTING_DEFAULT_END_DATE.time(),
         )
         self.date_field = self.date_field or date_field
 
+        self.start_date_field_name = (
+            self.start_date_field_name or start_date_field_name or self.date_field
+        )
+        self.end_date_field_name = (
+            self.end_date_field_name or end_date_field_name or self.date_field
+        )
+
         self.q_filters = q_filters or []
         self.kwargs_filters = kwargs_filters or {}
+        self.crosstab_field = self.crosstab_field or crosstab_field
 
-        self.crosstab_model = self.crosstab_model or crosstab_model
         self.crosstab_columns = crosstab_columns or self.crosstab_columns or []
         self.crosstab_ids = self.crosstab_ids or crosstab_ids or []
         self.crosstab_compute_remainder = (
             self.crosstab_compute_remainder
             if crosstab_compute_remainder is None
             else crosstab_compute_remainder
         )
 
         self.format_row = format_row_func or self._default_format_row
 
-        main_queryset = main_queryset or self.report_model.objects
-        main_queryset = main_queryset.order_by()
+        main_queryset = (
+            self.report_model.objects if main_queryset is None else main_queryset
+        )
+        # todo revise & move somewhere nicer, List Report need to override the resetting of order
+        main_queryset = self._remove_order(main_queryset)
 
         self.columns = columns or self.columns or []
         self.group_by = group_by or self.group_by
 
         self.time_series_pattern = self.time_series_pattern or time_series_pattern
         self.time_series_columns = self.time_series_columns or time_series_columns
         self.time_series_custom_dates = (
             self.time_series_custom_dates or time_series_custom_dates
         )
         self.container_class = container_class
 
-        if not self.date_field and (
-            self.time_series_pattern or self.crosstab_model or self.group_by
-        ):
+        if not (
+            self.date_field or (self.start_date_field_name and self.end_date_field_name)
+        ) and (self.time_series_pattern or self.crosstab_field or self.group_by):
             raise ImproperlyConfigured(
-                "date_field must be set on a class level or via init"
+                f"date_field or [start_date_field_name and end_date_field_name] must be set for {self}"
             )
 
         self._prepared_results = {}
         self.report_fields_classes = {}
 
         self._report_fields_dependencies = {
             "time_series": {},
@@ -294,79 +311,74 @@
         self.doc_type_minus_list = (
             list(doc_type_minus_list) if doc_type_minus_list else doc_types[1]
         )
 
         self.swap_sign = self.swap_sign or swap_sign
         self.limit_records = self.limit_records or limit_records
 
-        # passed to the report fields
-        # self.date_field = date_field or self.date_field
-
         # in case of a group by, do we show a grouped by model data regardless of their appearance in the results
         # a client who didn't make a transaction during the date period.
         self.show_empty_records = False  # show_empty_records if show_empty_records else self.show_empty_records
         # Looks like this options is harder then what i thought as it interfere with the usual filtering of the report
 
         # Preparing actions
         self._parse()
         if self.group_by:
-            if self.show_empty_records:
-                pass
-                # group_by_filter = self.kwargs_filters.get(self.group_by, '')
-                # qs = self.group_by_field.related_model.objects
-                # if group_by_filter:
-                #     lookup = 'pk__in' if isinstance(group_by_filter, Iterable) else 'pk'
-                #     qs = qs.filter(**{lookup: group_by_filter})
-                # self.main_queryset = qs.values()
-
+            self.main_queryset = self._apply_queryset_options(main_queryset)
+            if type(self.group_by_field) is ForeignKey:
+                ids = self.main_queryset.values_list(
+                    self.group_by_field_attname
+                ).distinct()
+                # uses the same logic that is in Django's query.py when fields is empty in values() call
+                concrete_fields = [
+                    f.name
+                    for f in self.group_by_field.related_model._meta.concrete_fields
+                ]
+                # add database columns that are not already in concrete_fields
+                final_fields = concrete_fields + list(
+                    set(self.get_database_columns()) - set(concrete_fields)
+                )
+                self.main_queryset = self.group_by_field.related_model.objects.filter(
+                    **{f"{self.group_by_field.target_field.name}__in": ids}
+                ).values(*final_fields)
             else:
-                self.main_queryset = self._apply_queryset_options(main_queryset)
-                if type(self.group_by_field) is ForeignKey:
-                    ids = self.main_queryset.values_list(
-                        self.group_by_field_attname
-                    ).distinct()
-                    # uses the same logic that is in Django's query.py when fields is empty in values() call
-                    concrete_fields = [
-                        f.name
-                        for f in self.group_by_field.related_model._meta.concrete_fields
-                    ]
-                    # add database columns that are not already in concrete_fields
-                    final_fields = concrete_fields + list(
-                        set(self.get_database_columns()) - set(concrete_fields)
-                    )
-                    self.main_queryset = (
-                        self.group_by_field.related_model.objects.filter(
-                            pk__in=ids
-                        ).values(*final_fields)
-                    )
-                else:
-                    self.main_queryset = self.main_queryset.distinct().values(
-                        self.group_by_field_attname
-                    )
+                self.main_queryset = self.main_queryset.distinct().values(
+                    self.group_by_field_attname
+                )
         else:
             if self.time_series_pattern:
                 self.main_queryset = [{}]
             else:
                 self.main_queryset = self._apply_queryset_options(
                     main_queryset, self.get_database_columns()
                 )
         self._prepare_report_dependencies()
 
+    def _remove_order(self, main_queryset):
+        """
+        Remove order_by from the main queryset
+        :param main_queryset:
+        :return:
+        """
+        # if main_queryset.query.order_by:
+        main_queryset = main_queryset.order_by()
+        return main_queryset
+
     def _apply_queryset_options(self, query, fields=None):
         """
         Apply the filters to the main queryset which will computed results be mapped to
         :param query:
         :param fields:
         :return:
         """
         filters = {}
         if self.date_field:
             filters = {
-                f"{self.date_field}__gt": self.start_date,
-                f"{self.date_field}__lte": self.end_date,
+                f"{self.start_date_field_name}__gt": self.start_date,
+                f"{self.end_date_field_name}__lte": self.end_date,
             }
         filters.update(self.kwargs_filters)
 
         if filters:
             query = query.filter(**filters)
         if fields:
             return query.values(*fields)
@@ -374,18 +386,25 @@
 
     def _construct_crosstab_filter(self, col_data):
         """
         In charge of adding the needed crosstab filter, specific to the case of is_remainder or not
         :param col_data:
         :return:
         """
+        if "__" in col_data["crosstab_field"]:
+            column_name = col_data["crosstab_field"]
+        else:
+            field = get_field_from_query_text(
+                col_data["crosstab_field"], self.report_model
+            )
+            column_name = field.column
         if col_data["is_remainder"]:
-            filters = [~Q(**{f"{col_data['model']}_id__in": self.crosstab_ids})]
+            filters = [~Q(**{f"{column_name}__in": self.crosstab_ids})]
         else:
-            filters = [Q(**{f"{col_data['model']}_id": col_data["id"]})]
+            filters = [Q(**{f"{column_name}": col_data["id"]})]
         return filters
 
     def _prepare_report_dependencies(self):
         from .fields import SlickReportField
 
         all_columns = (
             ("normal", self._parsed_columns),
@@ -432,14 +451,15 @@
 
                 report_class = klass(
                     self.doc_type_plus_list,
                     self.doc_type_minus_list,
                     group_by=self.group_by,
                     report_model=self.report_model,
                     date_field=self.date_field,
+                    queryset=self.queryset,
                 )
 
                 q_filters = None
                 date_filter = {
                     f"{self.date_field}__gte": col_data.get(
                         "start_date", self.start_date
                     ),
@@ -541,18 +561,17 @@
     @classmethod
     def check_columns(cls, columns, group_by, report_model, container_class=None):
         """
         Check and parse the columns, throw errors in case an item in the columns cant not identified
         :param columns: List of columns
         :param group_by: group by field if any
         :param report_model: the report model
-        :param container_class: a class to search for custom columns attribute in, typically the SlickReportView
+        :param container_class: a class to search for custom columns attribute in, typically the ReportView
         :return: List of dict, each dict contains relevant data to the respective field in `columns`
         """
-        group_by_field = ""
         group_by_model = None
         if group_by:
             try:
                 group_by_field = [
                     x
                     for x in report_model._meta.get_fields()
                     if x.name == group_by.split("__")[0]
@@ -681,15 +700,15 @@
             time_series_columns = self.get_time_series_parsed_columns()
             try:
                 index = self.columns.index("__time_series__")
                 columns[index:index] = time_series_columns
             except ValueError:
                 columns += time_series_columns
 
-        if self.crosstab_model:
+        if self.crosstab_field:
             crosstab_columns = self.get_crosstab_parsed_columns()
 
             try:
                 index = self.columns.index("__crosstab__")
                 columns[index:index] = crosstab_columns
             except ValueError:
                 columns += crosstab_columns
@@ -818,19 +837,19 @@
                     magic_field_class = col
 
                 output_cols.append(
                     {
                         "name": f"{magic_field_class.name}CT{id}",
                         "original_name": magic_field_class.name,
                         "verbose_name": self.get_crosstab_field_verbose_name(
-                            magic_field_class, self.crosstab_model, id
+                            magic_field_class, self.crosstab_field, id
                         ),
                         "ref": magic_field_class,
                         "id": id,
-                        "model": self.crosstab_model,
+                        "crosstab_field": self.crosstab_field,
                         "is_remainder": counter == ids_length
                         if self.crosstab_compute_remainder
                         else False,
                         "source": "magic_field" if magic_field_class else "",
                         "is_summable": magic_field_class.is_summable,
                     }
                 )
@@ -856,15 +875,15 @@
         crosstab_columns = self.get_crosstab_parsed_columns()
         metadata = {
             "time_series_pattern": self.time_series_pattern,
             "time_series_column_names": [x["name"] for x in time_series_columns],
             "time_series_column_verbose_names": [
                 x["verbose_name"] for x in time_series_columns
             ],
-            "crosstab_model": self.crosstab_model or "",
+            "crosstab_model": self.crosstab_field or "",
             "crosstab_column_names": [x["name"] for x in crosstab_columns],
             "crosstab_column_verbose_names": [
                 x["verbose_name"] for x in crosstab_columns
             ],
         }
         return metadata
 
@@ -1007,7 +1026,10 @@
 
                 else:
                     if col_data.get("type", "") == "choice":
                         data[name] = getattr(obj, f"get_{name}_display", "")()
                     else:
                         data[name] = getattr(obj, name, "")
         return data
+
+    def _remove_order(self, main_queryset):
+        return main_queryset
```

### Comparing `django-slick-reporting-0.8.0/slick_reporting/helpers.py` & `django-slick-reporting-0.9.0/slick_reporting/helpers.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/slick_reporting/registry.py` & `django-slick-reporting-0.9.0/slick_reporting/registry.py`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js` & `django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.chartsjs.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js` & `django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/erp_framework.highchart.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/slick_reporting/static/slick_reporting/main.js` & `django-slick-reporting-0.9.0/slick_reporting/static/slick_reporting/main.js`

 * *Files identical despite different names*

### Comparing `django-slick-reporting-0.8.0/slick_reporting/templates/slick_reporting/base.html` & `django-slick-reporting-0.9.0/slick_reporting/templates/slick_reporting/base.html`

 * *Files 18% similar despite different names*

```diff
@@ -8,47 +8,36 @@
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
 
     <!-- Bootstrap CSS -->
     <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
           integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
 
-    <link rel="stylesheet" type="text/css"
-          href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"/>
     <title>Django Slick Reporting</title>
 </head>
 <body>
 <div class="container">
     <div class="py-5 ">
         {% block content %}
 
         {% endblock %}
     </div>
 </div>
 <!-- Optional JavaScript -->
-<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"
-        integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1"
-        crossorigin="anonymous"></script>
-<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"
-        integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM"
-        crossorigin="anonymous"></script>
+{#<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js"#}
+{#        integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1"#}
+{#        crossorigin="anonymous"></script>#}
+{#<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js"#}
+{#        integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM"#}
+{#        crossorigin="anonymous"></script>#}
 
 {#Date picker #}
-<script type="text/javascript" src="https://cdn.jsdelivr.net/momentjs/latest/moment.min.js"></script>
-<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/daterangepicker/daterangepicker.min.js"></script>
-<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/daterangepicker/daterangepicker.css"/>
-
-{#select2#}
-
-
-
-
-{# datatable #}
-<script type="text/javascript" src="https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.js"></script>
-    <link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/v/bs4/dt-1.10.20/datatables.min.css"/>
-
+{#<script type="text/javascript" src="https://cdn.jsdelivr.net/momentjs/latest/moment.min.js"></script>#}
+{#<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/daterangepicker/daterangepicker.min.js"></script>#}
+{#<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/daterangepicker/daterangepicker.css"/>#}
 
+{% include "slick_reporting/js_resources.html" %}
 
 {% block extrajs %}
 {% endblock %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,11 +1,17 @@
  {% load static %} {% load crispy_forms_tags %}
 
 
 
-
 {% block content %} {% endblock %}
- {#Date picker #}
-
- {#select2#} {# datatable #}
-
- {% block extrajs %} {% endblock %}
+ {#
+} {# integrity="sha384-
+UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1"#} {#
+crossorigin="anonymous">
+#} {#
+} {# integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/
+nJGzIxFDsf4x0xIM+B07jRM"#} {# crossorigin="anonymous">
+#} {#Date picker #} {#
+#} {#
+#} {#
+#} {% include "slick_reporting/js_resources.html" %} {% block extrajs %} {%
+endblock %}
```

### Comparing `django-slick-reporting-0.8.0/slick_reporting/templatetags/slick_reporting_tags.py` & `django-slick-reporting-0.9.0/slick_reporting/templatetags/slick_reporting_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 from django.utils.safestring import mark_safe
 
 register = template.Library()
 
 
 @register.simple_tag
 def get_data(row, column):
-    return row[column['name']]
+    return row[column["name"]]
 
 
 def jsonify(object):
     def date_handler(obj):
-        if hasattr(obj, 'isoformat'):
+        if hasattr(obj, "isoformat"):
             return obj.isoformat()
         elif isinstance(obj, Promise):
             return force_str(obj)
 
     if isinstance(object, QuerySet):
-        return serialize('json', object)
+        return serialize("json", object)
 
     return mark_safe(json.dumps(object, use_decimal=True, default=date_handler))
 
 
-register.filter('jsonify', jsonify)
+register.filter("jsonify", jsonify)
```

### Comparing `django-slick-reporting-0.8.0/slick_reporting/views.py` & `django-slick-reporting-0.9.0/slick_reporting/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,45 @@
-import datetime
 import csv
+import datetime
+import warnings
 
 import simplejson as json
 from django import forms
 from django.conf import settings
+from django.db.models import Q
 from django.forms import modelform_factory
-from django.http import HttpResponse, StreamingHttpResponse
+from django.http import HttpResponse, StreamingHttpResponse, JsonResponse
 from django.utils.encoding import force_str
 from django.utils.functional import Promise
 from django.views.generic import FormView
 
 from .app_settings import (
     SLICK_REPORTING_DEFAULT_END_DATE,
     SLICK_REPORTING_DEFAULT_START_DATE,
-    SLICK_REPORTING_DEFAULT_CHARTS_ENGINE,
 )
-from .form_factory import (
+from .forms import (
     report_form_factory,
     get_crispy_helper,
     default_formfield_callback,
+    OrderByForm,
+)
+from .generator import (
+    ReportGenerator,
+    ListViewReportGenerator,
+    ReportGeneratorAPI,
+    Chart,  # noqa # needed for easier importing in other apps
 )
-from .generator import ReportGenerator, ListViewReportGenerator, Chart
+
+
+def dictsort(value, arg, desc=False):
+    """
+    Takes a list of dicts, returns that list sorted by the property given in
+    the argument.
+    """
+    return sorted(value, key=lambda x: x[arg], reverse=desc)
 
 
 class ExportToCSV(object):
     def get_filename(self):
         return self.report_title
 
     def get_response(self):
@@ -73,58 +88,77 @@
                 "Content-Disposition": 'attachment; filename="{filename}.csv"'.format(
                     filename=self.get_filename()
                 )
             },
         )
 
 
-class SlickReportViewBase(FormView):
-    group_by = None
-    columns = None
+class ReportViewBase(ReportGeneratorAPI, FormView):
+    report_slug = None
 
     report_title = ""
-    time_series_pattern = ""
-    time_series_columns = None
 
-    date_field = None
-
-    swap_sign = False
+    report_title_context_key = "title"
 
     report_generator_class = ReportGenerator
 
-    report_model = None
-
     base_model = None
-    limit_records = None
-
-    queryset = None
 
     chart_settings = None
 
-    crosstab_model = None
-    crosstab_ids = None
-    crosstab_columns = None
-    crosstab_compute_remainder = True
     excluded_fields = None
-    report_title_context_key = "title"
 
     time_series_selector = False
     time_series_selector_choices = None
     time_series_selector_default = None
     time_series_selector_allow_empty = False
 
     csv_export_class = ExportToStreamingCSV
 
-    """
-    A list of chart settings objects instructing front end on how to plot the data.
-    
-    """
+    with_type = False
+    doc_type_field_name = "doc_type"
+    doc_type_plus_list = None
+    doc_type_minus_list = None
+
+    default_order_by = ""
 
     template_name = "slick_reporting/simple_report.html"
 
+    @staticmethod
+    def form_filter_func(fkeys_dict):
+        # todo revise
+        return fkeys_dict
+
+    def order_results(self, data):
+        """
+        order the results based on GET parameter or default_order_by
+        :param data: List of Dict to be ordered
+        :return: Ordered data
+        """
+        order_field, asc = OrderByForm(self.request.GET).get_order_by(
+            self.default_order_by
+        )
+        if order_field:
+            data = dictsort(data, order_field, asc)
+        return data
+
+    def get_doc_types_q_filters(self):
+        if self.doc_type_plus_list or self.doc_type_minus_list:
+            return (
+                [Q(**{f"{self.doc_type_field_name}__in": self.doc_type_plus_list})]
+                if self.doc_type_plus_list
+                else []
+            ), (
+                [Q(**{f"{self.doc_type_field_name}__in": self.doc_type_minus_list})]
+                if self.doc_type_minus_list
+                else []
+            )
+
+        return [], []
+
     def get(self, request, *args, **kwargs):
         form_class = self.get_form_class()
         self.form = self.get_form(form_class)
         if self.form.is_valid():
             report_data = self.get_report_results()
 
             export_option = request.GET.get("_export", "")
@@ -136,25 +170,29 @@
 
             if request.headers.get("x-requested-with") == "XMLHttpRequest":
                 return self.ajax_render_to_response(report_data)
 
             return self.render_to_response(
                 self.get_context_data(report_data=report_data)
             )
+        else:
+            return self.form_invalid(self.form)
 
-        return self.render_to_response(self.get_context_data())
+        # return self.render_to_response(self.get_context_data())
 
     def export_csv(self, report_data):
         return self.csv_export_class(
             self.request, report_data, self.report_title
         ).get_response()
 
     @classmethod
     def get_report_model(cls):
-        return cls.report_model or cls.queryset.model
+        if cls.queryset is not None:
+            return cls.queryset.model
+        return cls.report_model
 
     def ajax_render_to_response(self, report_data):
         return HttpResponse(
             self.serialize_to_json(report_data), content_type="application/json"
         )
 
     def serialize_to_json(self, response_data):
@@ -179,17 +217,18 @@
     def get_form_class(self):
         """
         Automatically instantiate a form based on details provided
         :return:
         """
         return self.form_class or report_form_factory(
             self.get_report_model(),
-            crosstab_model=self.crosstab_model,
+            crosstab_model=self.crosstab_field,
             display_compute_remainder=self.crosstab_compute_remainder,
             excluded_fields=self.excluded_fields,
+            fkeys_filter_func=self.form_filter_func,
             initial=self.get_form_initial(),
             show_time_series_selector=self.time_series_selector,
             time_series_selector_choices=self.time_series_selector_choices,
             time_series_selector_default=self.time_series_selector_default,
             time_series_selector_allow_empty=self.time_series_selector_allow_empty,
         )
 
@@ -216,48 +255,55 @@
                     "data": self.request.GET,
                 }
             )
         return kwargs
 
     def get_report_generator(self, queryset, for_print):
         q_filters, kw_filters = self.form.get_filters()
-        if self.crosstab_model:
+        if self.crosstab_field:
             self.crosstab_ids = self.form.get_crosstab_ids()
 
         crosstab_compute_remainder = (
             self.form.get_crosstab_compute_remainder()
             if self.request.GET or self.request.POST
             else self.crosstab_compute_remainder
         )
 
         time_series_pattern = self.time_series_pattern
         if self.time_series_selector:
-            time_series_pattern = self.form.cleaned_data["time_series_pattern"]
+            time_series_pattern = self.form.get_time_series_pattern()
+
+        doc_type_plus_list, doc_type_minus_list = [], []
+
+        if self.with_type:
+            doc_type_plus_list, doc_type_minus_list = self.get_doc_types_q_filters()
 
         return self.report_generator_class(
             self.get_report_model(),
-            start_date=self.form.cleaned_data["start_date"],
-            end_date=self.form.cleaned_data["end_date"],
+            start_date=self.form.get_start_date(),
+            end_date=self.form.get_end_date(),
             q_filters=q_filters,
             kwargs_filters=kw_filters,
             date_field=self.date_field,
             main_queryset=queryset,
             print_flag=for_print,
             limit_records=self.limit_records,
             swap_sign=self.swap_sign,
             columns=self.columns,
             group_by=self.group_by,
             time_series_pattern=time_series_pattern,
             time_series_columns=self.time_series_columns,
-            crosstab_model=self.crosstab_model,
+            crosstab_field=self.crosstab_field,
             crosstab_ids=self.crosstab_ids,
             crosstab_columns=self.crosstab_columns,
             crosstab_compute_remainder=crosstab_compute_remainder,
             format_row_func=self.format_row,
             container_class=self,
+            doc_type_plus_list=doc_type_plus_list,
+            doc_type_minus_list=doc_type_minus_list,
         )
 
     def format_row(self, row_obj):
         """
         A hook to format each row . This method gets called on each row in the results. <ust return the object
         :param row_obj: a dict representing a single row in the results
         :return: A dict representing a single row in the results
@@ -279,14 +325,15 @@
         :return: JsonResponse
         """
 
         queryset = self.get_queryset()
         report_generator = self.get_report_generator(queryset, for_print)
         data = report_generator.get_report_data()
         data = self.filter_results(data, for_print)
+        data = self.order_results(data)
 
         return report_generator.get_full_response(
             data=data,
             report_slug=self.get_report_slug(),
             chart_settings=self.chart_settings,
             default_chart_title=self.report_title,
         )
@@ -303,78 +350,100 @@
         """
         Ensure the sane settings are passed to the front end.
         """
         return generator.get_chart_settings(
             self.chart_settings or [], self.report_title
         )
 
-    def get_queryset(self):
-        return self.queryset or self.report_model.objects
+    @classmethod
+    def get_queryset(cls):
+        if cls.queryset is None:
+            return cls.get_report_model()._default_manager.all()
+        return cls.queryset
 
     def filter_results(self, data, for_print=False):
         """
         Hook to Filter results based on computed data (like eliminate __balance__ = 0, etc)
+        return None to remove the row from the results
         :param data: List of objects
         :param for_print: is print request
         :return: filtered data
         """
         return data
 
     @classmethod
     def get_report_slug(cls):
-        return cls.__name__.lower()
+        return cls.report_slug or cls.__name__.lower()
 
     @staticmethod
     def get_form_initial():
         # todo revise why not actually displaying datetime on screen
         return {
             "start_date": SLICK_REPORTING_DEFAULT_START_DATE,
             "end_date": SLICK_REPORTING_DEFAULT_END_DATE,
         }
 
     def get_form_crispy_helper(self):
-        return self.form.get_crispy_helper()
+        """
+        A hook retuning crispy helper for the form
+        :return:
+        """
+        if hasattr(self, "form"):
+            return self.form.get_crispy_helper()
+        return None
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context[self.report_title_context_key] = self.report_title
         context["crispy_helper"] = self.get_form_crispy_helper()
 
         if not (self.request.POST or self.request.GET):
             # initialize empty form with initials if the no data is in the get or the post
             context["form"] = self.get_form_class()()
         return context
 
+    def form_invalid(self, form):
+        if self.request.META.get("HTTP_X_REQUESTED_WITH") == "XMLHttpRequest":
+            return JsonResponse(form.errors, status=400)
+        return super().form_invalid(form)
+
 
-class SlickReportView(SlickReportViewBase):
+class ReportView(ReportViewBase):
     def __init_subclass__(cls) -> None:
         # date_field = getattr(cls, 'date_field', '')
         # if not date_field:
         #     raise TypeError(f'`date_field` is not set on {cls}')
         # cls.report_generator_class.check_columns([cls.date_field], False, cls.get_report_model())
 
-        # sanity check, raises error if the columns or date fields is not mapped
-
-        cls.report_generator_class.check_columns(
-            cls.columns, cls.group_by, cls.get_report_model(), container_class=cls
-        )
+        # sanity check, raises error if the columns or date fields is not set
+        if cls.columns:
+            cls.report_generator_class.check_columns(
+                cls.columns,
+                cls.group_by,
+                cls.get_report_model(),
+                container_class=cls,
+            )
 
         super().__init_subclass__()
 
-    @staticmethod
-    def check_chart_settings(chart_settings=None):
-        # todo check on chart settings
-        return
-
 
-class SlickReportingListView(SlickReportViewBase):
+class SlickReportingListViewMixin:
     report_generator_class = ListViewReportGenerator
     filters = None
 
+    def get_queryset(self):
+        qs = self.queryset or self.report_model.objects
+        if self.default_order_by:
+            qs.order_by(self.default_order_by)
+        return qs
+
     def get_form_filters(self, form):
+        if self.form_class:
+            return form.get_filters()
+
         kw_filters = {}
 
         for name, field in form.base_fields.items():
             if type(field) is forms.ModelMultipleChoiceField:
                 value = form.cleaned_data[name]
                 if value:
                     kw_filters[f"{name}__in"] = form.cleaned_data[name]
@@ -409,19 +478,24 @@
             limit_records=self.limit_records,
             columns=self.columns,
             format_row_func=self.format_row,
             container_class=self,
         )
 
     def get_form_class(self):
-        return modelform_factory(
-            self.get_report_model(),
-            fields=self.filters,
-            formfield_callback=default_formfield_callback,
-        )
+        if self.form_class:
+            return self.form_class
+
+        elif self.filters:
+            return modelform_factory(
+                self.get_report_model(),
+                fields=self.filters,
+                formfield_callback=default_formfield_callback,
+            )
+        return forms.Form
 
     def get_report_results(self, for_print=False):
         """
         Gets the reports Data, and, its meta data used by datatables.net and highcharts
         :return: JsonResponse
         """
 
@@ -432,7 +506,52 @@
 
         return report_generator.get_full_response(
             data=data,
             report_slug=self.get_report_slug(),
             chart_settings=self.chart_settings,
             default_chart_title=self.report_title,
         )
+
+
+class SlickReportingListView(SlickReportingListViewMixin, ReportViewBase):
+    def __init_subclass__(cls) -> None:
+        warnings.warn(
+            "slick_reporting.view.SlickReportingListView is"
+            "deprecated in favor of slick_reporting.view.ListReportView",
+            Warning,
+            stacklevel=2,
+        )
+        super().__init_subclass__()
+
+
+class ListReportView(SlickReportingListViewMixin, ReportViewBase):
+    pass
+
+
+class SlickReportViewBase(ReportViewBase):
+    """
+    Deprecated in favor of slick_reporting.view.ReportViewBase
+    """
+
+    def __init_subclass__(cls) -> None:
+        warnings.warn(
+            "slick_reporting.view.SlickReportView and slick_reporting.view.SlickReportViewBase are "
+            "deprecated in favor of slick_reporting.view.ReportView and slick_reporting.view.BaseReportView",
+            Warning,
+            stacklevel=2,
+        )
+
+        super().__init_subclass__()
+
+
+class SlickReportView(ReportView):
+    def __init_subclass__(cls) -> None:
+        warnings.warn(
+            "slick_reporting.view.SlickReportView and slick_reporting.view.SlickReportViewBase are "
+            "deprecated in favor of slick_reporting.view.ReportView and slick_reporting.view.BaseReportView",
+            Warning,
+            stacklevel=2,
+        )
+
+        # cls.report_generator_class.check_columns(
+        #     cls.columns, cls.group_by, cls.get_report_model(), container_class=cls
+        # )
```

