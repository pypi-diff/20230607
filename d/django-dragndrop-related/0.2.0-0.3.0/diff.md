# Comparing `tmp/django-dragndrop-related-0.2.0.tar.gz` & `tmp/django-dragndrop-related-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dragndrop-related-0.2.0.tar", last modified: Fri May  5 09:25:23 2023, max compression
+gzip compressed data, was "django-dragndrop-related-0.3.0.tar", last modified: Wed Jun  7 18:01:48 2023, max compression
```

## Comparing `django-dragndrop-related-0.2.0.tar` & `django-dragndrop-related-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,44 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.954630 django-dragndrop-related-0.2.0/
--rw-r--r--   0 james      (501) staff       (20)     1070 2022-06-14 13:19:32.000000 django-dragndrop-related-0.2.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      107 2022-06-14 13:32:35.000000 django-dragndrop-related-0.2.0/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     7431 2023-05-05 09:25:23.955267 django-dragndrop-related-0.2.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     6430 2023-05-05 09:20:18.000000 django-dragndrop-related-0.2.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.942214 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     7431 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      847 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2022-06-14 13:36:24.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)      159 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       34 2023-05-05 09:25:23.000000 django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.942880 django-dragndrop-related-0.2.0/dragndrop_related/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:56:04.000000 django-dragndrop-related-0.2.0/dragndrop_related/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.935554 django-dragndrop-related-0.2.0/dragndrop_related/templates/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.935682 django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.943671 django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/dragndrop_related/
--rw-r--r--   0 james      (501) staff       (20)     2612 2023-05-05 09:14:23.000000 django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/dragndrop_related/change_form.html
--rw-r--r--   0 james      (501) staff       (20)     7915 2023-05-05 09:15:48.000000 django-dragndrop-related-0.2.0/dragndrop_related/views.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.948601 django-dragndrop-related-0.2.0/example_project/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/asgi.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.951617 django-dragndrop-related-0.2.0/example_project/gallery/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/gallery/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      387 2022-06-14 14:19:59.000000 django-dragndrop-related-0.2.0/example_project/gallery/admin.py
--rw-r--r--   0 james      (501) staff       (20)      146 2022-06-14 13:49:16.000000 django-dragndrop-related-0.2.0/example_project/gallery/apps.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-05 09:25:23.954321 django-dragndrop-related-0.2.0/example_project/gallery/migrations/
--rw-r--r--   0 james      (501) staff       (20)     1005 2022-06-14 14:22:18.000000 django-dragndrop-related-0.2.0/example_project/gallery/migrations/0001_initial.py
--rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/gallery/migrations/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      423 2022-06-14 14:00:13.000000 django-dragndrop-related-0.2.0/example_project/gallery/models.py
--rwxr-xr-x   0 james      (501) staff       (20)      671 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/manage.py
--rw-r--r--   0 james      (501) staff       (20)     3533 2022-06-14 14:05:30.000000 django-dragndrop-related-0.2.0/example_project/settings.py
--rw-r--r--   0 james      (501) staff       (20)      960 2022-06-14 14:06:49.000000 django-dragndrop-related-0.2.0/example_project/urls.py
--rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.2.0/example_project/wsgi.py
--rw-r--r--   0 james      (501) staff       (20)      115 2023-05-05 09:25:23.956952 django-dragndrop-related-0.2.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     2002 2023-05-05 09:23:58.000000 django-dragndrop-related-0.2.0/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.968204 django-dragndrop-related-0.3.0/
+-rw-r--r--   0 james      (501) staff       (20)     1070 2022-06-14 13:19:32.000000 django-dragndrop-related-0.3.0/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      107 2022-06-14 13:32:35.000000 django-dragndrop-related-0.3.0/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     8361 2023-06-07 18:01:48.968418 django-dragndrop-related-0.3.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     7360 2023-06-07 16:26:07.000000 django-dragndrop-related-0.3.0/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.953615 django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     8361 2023-06-07 18:01:48.000000 django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1080 2023-06-07 18:01:48.000000 django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 18:01:48.000000 django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2022-06-14 13:36:24.000000 django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)      189 2023-06-07 18:01:48.000000 django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       34 2023-06-07 18:01:48.000000 django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.954469 django-dragndrop-related-0.3.0/dragndrop_related/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:56:04.000000 django-dragndrop-related-0.3.0/dragndrop_related/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.946716 django-dragndrop-related-0.3.0/dragndrop_related/templates/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.946834 django-dragndrop-related-0.3.0/dragndrop_related/templates/admin/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.955234 django-dragndrop-related-0.3.0/dragndrop_related/templates/admin/dragndrop_related/
+-rw-r--r--   0 james      (501) staff       (20)     2739 2023-06-07 16:09:35.000000 django-dragndrop-related-0.3.0/dragndrop_related/templates/admin/dragndrop_related/change_form.html
+-rw-r--r--   0 james      (501) staff       (20)     9230 2023-06-07 17:59:01.000000 django-dragndrop-related-0.3.0/dragndrop_related/views.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.960160 django-dragndrop-related-0.3.0/example_project/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.3.0/example_project/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.3.0/example_project/asgi.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.963827 django-dragndrop-related-0.3.0/example_project/gallery/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.3.0/example_project/gallery/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      387 2022-06-14 14:19:59.000000 django-dragndrop-related-0.3.0/example_project/gallery/admin.py
+-rw-r--r--   0 james      (501) staff       (20)      146 2022-06-14 13:49:16.000000 django-dragndrop-related-0.3.0/example_project/gallery/apps.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.965422 django-dragndrop-related-0.3.0/example_project/gallery/migrations/
+-rw-r--r--   0 james      (501) staff       (20)     1005 2022-06-14 14:22:18.000000 django-dragndrop-related-0.3.0/example_project/gallery/migrations/0001_initial.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-06-14 13:34:34.000000 django-dragndrop-related-0.3.0/example_project/gallery/migrations/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      423 2022-06-14 14:00:13.000000 django-dragndrop-related-0.3.0/example_project/gallery/models.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.967005 django-dragndrop-related-0.3.0/example_project/library/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-06-07 17:26:23.000000 django-dragndrop-related-0.3.0/example_project/library/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      468 2023-06-07 17:37:27.000000 django-dragndrop-related-0.3.0/example_project/library/admin.py
+-rw-r--r--   0 james      (501) staff       (20)      146 2023-06-07 17:34:33.000000 django-dragndrop-related-0.3.0/example_project/library/apps.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 18:01:48.967973 django-dragndrop-related-0.3.0/example_project/library/migrations/
+-rw-r--r--   0 james      (501) staff       (20)     1140 2023-06-07 17:35:23.000000 django-dragndrop-related-0.3.0/example_project/library/migrations/0001_initial.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-06-07 17:35:23.000000 django-dragndrop-related-0.3.0/example_project/library/migrations/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      571 2023-06-07 17:33:43.000000 django-dragndrop-related-0.3.0/example_project/library/models.py
+-rwxr-xr-x   0 james      (501) staff       (20)      671 2022-06-14 13:34:34.000000 django-dragndrop-related-0.3.0/example_project/manage.py
+-rw-r--r--   0 james      (501) staff       (20)     3583 2023-06-07 17:34:53.000000 django-dragndrop-related-0.3.0/example_project/settings.py
+-rw-r--r--   0 james      (501) staff       (20)      960 2022-06-14 14:06:49.000000 django-dragndrop-related-0.3.0/example_project/urls.py
+-rw-r--r--   0 james      (501) staff       (20)      407 2022-06-14 13:34:34.000000 django-dragndrop-related-0.3.0/example_project/wsgi.py
+-rw-r--r--   0 james      (501) staff       (20)      115 2023-06-07 18:01:48.969283 django-dragndrop-related-0.3.0/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     2062 2023-06-07 17:44:42.000000 django-dragndrop-related-0.3.0/setup.py
```

### Comparing `django-dragndrop-related-0.2.0/LICENSE` & `django-dragndrop-related-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.2.0/PKG-INFO` & `django-dragndrop-related-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dragndrop-related
-Version: 0.2.0
+Version: 0.3.0
 Summary: Drag-and-drop multiple uploading of related images/files for
 Home-page: http://github.com/BigglesZX/django-dragndrop-related
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -35,23 +35,23 @@
 
 The example project shown uses [django-admin-thumbnails](https://pypi.org/project/django-admin-thumbnails/) to show `ImageField` preview thumbnails.
 
 ## Rationale
 
 One of the most common requests I get from clients when working on Django projects is to support some kind of drag-and-drop upload to save them the tedium of working with multiple file upload fields. I finally put some effort into solving this problem and came up with this library, which essentially provides for the creation of related models via AJAX POST request.
 
-It assumes some simplicity on the part of the related model – e.g. that only an `ImageField` is required to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
+It assumes some simplicity on the part of the related model – e.g. that a valid instance only requires a single `ImageField` or `FileField` to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
 
 I decided not to try to support drag-and-drop uploads when _creating_ parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
 
 ## Compatibility
 
 This library has been tested on Django 3.2 and 4.0 on Python 3.8, though I expect it to be fairly compatible with other versions. For now, the package is marked as requiring Python 3.6 or higher.
 
-**Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket, but be aware it's not being developed intensively at this stage.**
+**Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket and I'll review it, but be aware it's not being developed intensively at this stage.**
 
 ## Installation
 
 ```
 $ pip install django-dragndrop-related
 ```
 
@@ -172,14 +172,25 @@
 
 class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
     # ...
 
     related_model_order_field_name = 'order'
 ```
 
+4. The Dropzone.js library supports an `acceptFiles` configuration option which restricts the types of files that can be selected or dropped in. If the field on your related child model is an `ImageField`, an `acceptFiles` value of `image/*` will be passed to Dropzone.js. For a `FileField` no restriction is specified by default. You can override the value of `acceptFiles` passed to Dropzone.js by specifying the `dropzone_accepted_files` property on the class that inherits from `DragAndDropRelatedImageMixin`, e.g.
+
+```python
+class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
+    # ...
+
+    dropzone_accepted_files = 'application/pdf'
+```
+
+See Mozilla's [documentation for the `file` input type](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file#unique_file_type_specifiers) for more information about how these types can be specified.
+
 ## Development
 
 If working locally on the package you can install the development tools via `pip`:
 
 ```shell
 $ pip install -e .[dev]
 ```
```

### Comparing `django-dragndrop-related-0.2.0/README.md` & `django-dragndrop-related-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
 The example project shown uses [django-admin-thumbnails](https://pypi.org/project/django-admin-thumbnails/) to show `ImageField` preview thumbnails.
 
 ## Rationale
 
 One of the most common requests I get from clients when working on Django projects is to support some kind of drag-and-drop upload to save them the tedium of working with multiple file upload fields. I finally put some effort into solving this problem and came up with this library, which essentially provides for the creation of related models via AJAX POST request.
 
-It assumes some simplicity on the part of the related model – e.g. that only an `ImageField` is required to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
+It assumes some simplicity on the part of the related model – e.g. that a valid instance only requires a single `ImageField` or `FileField` to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
 
 I decided not to try to support drag-and-drop uploads when _creating_ parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
 
 ## Compatibility
 
 This library has been tested on Django 3.2 and 4.0 on Python 3.8, though I expect it to be fairly compatible with other versions. For now, the package is marked as requiring Python 3.6 or higher.
 
-**Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket, but be aware it's not being developed intensively at this stage.**
+**Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket and I'll review it, but be aware it's not being developed intensively at this stage.**
 
 ## Installation
 
 ```
 $ pip install django-dragndrop-related
 ```
 
@@ -145,14 +145,25 @@
 
 class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
     # ...
 
     related_model_order_field_name = 'order'
 ```
 
+4. The Dropzone.js library supports an `acceptFiles` configuration option which restricts the types of files that can be selected or dropped in. If the field on your related child model is an `ImageField`, an `acceptFiles` value of `image/*` will be passed to Dropzone.js. For a `FileField` no restriction is specified by default. You can override the value of `acceptFiles` passed to Dropzone.js by specifying the `dropzone_accepted_files` property on the class that inherits from `DragAndDropRelatedImageMixin`, e.g.
+
+```python
+class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
+    # ...
+
+    dropzone_accepted_files = 'application/pdf'
+```
+
+See Mozilla's [documentation for the `file` input type](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file#unique_file_type_specifiers) for more information about how these types can be specified.
+
 ## Development
 
 If working locally on the package you can install the development tools via `pip`:
 
 ```shell
 $ pip install -e .[dev]
 ```
```

### Comparing `django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/PKG-INFO` & `django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dragndrop-related
-Version: 0.2.0
+Version: 0.3.0
 Summary: Drag-and-drop multiple uploading of related images/files for
 Home-page: http://github.com/BigglesZX/django-dragndrop-related
 Author: James Tiplady
 Maintainer: James Tiplady
 License: MIT
 Keywords: django
 Platform: OS Independent
@@ -35,23 +35,23 @@
 
 The example project shown uses [django-admin-thumbnails](https://pypi.org/project/django-admin-thumbnails/) to show `ImageField` preview thumbnails.
 
 ## Rationale
 
 One of the most common requests I get from clients when working on Django projects is to support some kind of drag-and-drop upload to save them the tedium of working with multiple file upload fields. I finally put some effort into solving this problem and came up with this library, which essentially provides for the creation of related models via AJAX POST request.
 
-It assumes some simplicity on the part of the related model – e.g. that only an `ImageField` is required to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
+It assumes some simplicity on the part of the related model – e.g. that a valid instance only requires a single `ImageField` or `FileField` to be populated – and uses [Dropzone.js](https://www.dropzone.dev/js/) to accept uploads and fire off POST requests to an endpoint which creates new child models using the related manager of the parent model.
 
 I decided not to try to support drag-and-drop uploads when _creating_ parent model instances, since the uploads would need to be stashed somewhere temporarily then associated with the new model when it was saved. Instead this library operates only on existing model instances and requires the user to reload the page once they're done dropping files, so that Django's admin/inline UI can display the newly created child models for editing. This is acceptable in my use-cases but may not be in yours.
 
 ## Compatibility
 
 This library has been tested on Django 3.2 and 4.0 on Python 3.8, though I expect it to be fairly compatible with other versions. For now, the package is marked as requiring Python 3.6 or higher.
 
-**Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket, but be aware it's not being developed intensively at this stage.**
+**Please note that this library is an early beta release, mostly published so that I can share code between my own projects. It works well for my specific use-case but your mileage may vary. If you have issues with the library please open a ticket and I'll review it, but be aware it's not being developed intensively at this stage.**
 
 ## Installation
 
 ```
 $ pip install django-dragndrop-related
 ```
 
@@ -172,14 +172,25 @@
 
 class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
     # ...
 
     related_model_order_field_name = 'order'
 ```
 
+4. The Dropzone.js library supports an `acceptFiles` configuration option which restricts the types of files that can be selected or dropped in. If the field on your related child model is an `ImageField`, an `acceptFiles` value of `image/*` will be passed to Dropzone.js. For a `FileField` no restriction is specified by default. You can override the value of `acceptFiles` passed to Dropzone.js by specifying the `dropzone_accepted_files` property on the class that inherits from `DragAndDropRelatedImageMixin`, e.g.
+
+```python
+class AlbumAdmin(DragAndDropRelatedImageMixin, admin.ModelAdmin):
+    # ...
+
+    dropzone_accepted_files = 'application/pdf'
+```
+
+See Mozilla's [documentation for the `file` input type](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/file#unique_file_type_specifiers) for more information about how these types can be specified.
+
 ## Development
 
 If working locally on the package you can install the development tools via `pip`:
 
 ```shell
 $ pip install -e .[dev]
 ```
```

### Comparing `django-dragndrop-related-0.2.0/django_dragndrop_related.egg-info/SOURCES.txt` & `django-dragndrop-related-0.3.0/django_dragndrop_related.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,8 +19,14 @@
 example_project/urls.py
 example_project/wsgi.py
 example_project/gallery/__init__.py
 example_project/gallery/admin.py
 example_project/gallery/apps.py
 example_project/gallery/models.py
 example_project/gallery/migrations/0001_initial.py
-example_project/gallery/migrations/__init__.py
+example_project/gallery/migrations/__init__.py
+example_project/library/__init__.py
+example_project/library/admin.py
+example_project/library/apps.py
+example_project/library/models.py
+example_project/library/migrations/0001_initial.py
+example_project/library/migrations/__init__.py
```

### Comparing `django-dragndrop-related-0.2.0/dragndrop_related/templates/admin/dragndrop_related/change_form.html` & `django-dragndrop-related-0.3.0/dragndrop_related/templates/admin/dragndrop_related/change_form.html`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,17 @@
                             <li class="success">
                                 Your {{ related_model_name }} was uploaded successfully. When you're finished uploading, <button type="button" class="button" onClick="window.location.reload();">reload</button> the page or <input class="button" type="submit" value="save and continue editing" name="_continue"> to see the new {{ related_model_name_plural }} reflected above and to make further edits.
                             </li>
                         </ul>
                     </div>
                     <script>
                         var myDropzone = new Dropzone("div#dropzone", {
-                            acceptedFiles: "image/*",
+                            {% if dropzone_accepted_files %}
+                                acceptedFiles: "{{ dropzone_accepted_files }}",
+                            {% endif %}
                             headers: { "X-CSRFToken": "{{ csrf_token }}" },
                             init: function() {
                                 this.on("success", function() {
                                     document.getElementById("dropzone-success").style.display = 'block';
                                 });
                             },
                             paramName: "{{ related_model_field_name }}",
```

### Comparing `django-dragndrop-related-0.2.0/dragndrop_related/views.py` & `django-dragndrop-related-0.3.0/dragndrop_related/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django import forms
 from django.contrib.auth.mixins import PermissionRequiredMixin
-from django.db import transaction
+from django.db import models, transaction
 from django.db.models import Max
 from django.http import (HttpResponse, HttpResponseBadRequest,
                          HttpResponseRedirect)
 from django.urls import re_path, reverse
 from django.views.generic import DetailView
 from django.views.generic.edit import FormMixin, ProcessFormView
 
@@ -25,22 +25,34 @@
         info = self.model._meta.app_label, self.model._meta.model_name
         urlpattern = 'admin:{0}_{1}_change'.format(*info)
         return HttpResponseRedirect(
             reverse(urlpattern, kwargs={'object_id': self.object.pk}))
 
     def get_form_class(self):
         ''' Construct a dynamic form class with a field named using the
-            `related_model_field_name` kwarg passed in from the `ModelAdmin`
+            `related_model_field_name` kwarg passed in from the `ModelAdmin`,
+            and with a type appropriate to the underlying field on the related
+            model
 
             source: https://stackoverflow.com/a/27505090/258794
         '''
 
-        related_model_field_name = self.kwargs['related_model_field_name']
+        related_manager_field_name = \
+            self.kwargs['related_manager_field_name']
+        related_model_field_name = \
+            self.kwargs['related_model_field_name']
+        related_model = \
+            getattr(self.object, related_manager_field_name).field.model
+        related_model_field_class = \
+            related_model._meta.get_field(related_model_field_name)
+
         form_fields = {}
-        form_fields[related_model_field_name] = forms.ImageField()
+        form_fields[related_model_field_name] = \
+            forms.ImageField() if isinstance(related_model_field_class, models.ImageField) else forms.FileField()  # noqa: E501
+
         return type('DragAndDropForm', (forms.Form,), form_fields)
 
     def get_permission_required(self):
         ''' Ensure the user has `change` permission for the model '''
 
         info = self.model._meta.app_label, self.model._meta.model_name
         return ('{0}.change_{1}'.format(*info), )
@@ -109,36 +121,56 @@
 
     ''' Path to template from which the custom admin `change_form` template
         should inherit
     '''
     change_form_template_parent = 'admin/change_form.html'
 
     ''' Name of the reverse relation on the associated model to which images
-        will be added
+        or files will be added
     '''
     related_manager_field_name = 'images'
 
-    ''' Name of the field on the *related* model where images will be saved '''
+    ''' Name of the field on the *related* model where images or files will
+        be saved
+    '''
     related_model_field_name = 'image'
 
     ''' Name of the ordering field on the *related* model, which will be used
         to ensure a valid order is set on new instances
 
         Defaults to `None` to skip this feature; override in in the descendant
         class to make use of this
     '''
     related_model_order_field_name = None
 
+    ''' Customise the `acceptedFiles` option passed to the Dropzone library in
+        the `add` or `change` templates
+
+        Defaults to `None` to use a sensible default based on the type of the
+        field on the related model
+    '''
+    dropzone_accepted_files = None
+
     def get_related_model_info(self):
         ''' Access the related model according to the value of
             `related_manager_field_name` and build a dict of useful info
         '''
 
         related_model = \
             getattr(self.model, self.related_manager_field_name).field.model
+
+        related_model_field_class = \
+            related_model._meta.get_field(self.related_model_field_name)
+        if self.dropzone_accepted_files:
+            dropzone_accepted_files = self.dropzone_accepted_files
+        elif isinstance(related_model_field_class, models.ImageField):
+            dropzone_accepted_files = 'image/*'
+        else:
+            dropzone_accepted_files = None
+
         return {
             'related_model':
                 related_model,
             'related_model_name':
                 related_model._meta.verbose_name,
             'related_model_name_plural':
                 related_model._meta.verbose_name_plural,
@@ -146,14 +178,16 @@
                 self.related_manager_field_name,
             'related_model_field_name':
                 self.related_model_field_name,
             'related_model_order_field_name':
                 self.related_model_order_field_name,
             'change_form_template_parent':
                 self.change_form_template_parent,
+            'dropzone_accepted_files':
+                dropzone_accepted_files,
         }
 
     def add_view(self, request, form_url='', extra_context=None):
         ''' Add our helpful related model info to the `add` view context '''
 
         extra_context = extra_context or {}
         extra_context = {**extra_context, **self.get_related_model_info()}
```

### Comparing `django-dragndrop-related-0.2.0/example_project/gallery/migrations/0001_initial.py` & `django-dragndrop-related-0.3.0/example_project/gallery/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.2.0/example_project/manage.py` & `django-dragndrop-related-0.3.0/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.2.0/example_project/settings.py` & `django-dragndrop-related-0.3.0/example_project/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
     'django_cleanup.apps.CleanupConfig',
     'dragndrop_related',
     'example_project.gallery.apps.GalleryConfig',
+    'example_project.library.apps.LibraryConfig',
 ]
 
 MIDDLEWARE = [
     'django.middleware.security.SecurityMiddleware',
     'django.contrib.sessions.middleware.SessionMiddleware',
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
```

### Comparing `django-dragndrop-related-0.2.0/example_project/urls.py` & `django-dragndrop-related-0.3.0/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django-dragndrop-related-0.2.0/setup.py` & `django-dragndrop-related-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     7. $ python setup.py register sdist
     8. $ twine upload dist/*
 '''
 
 from setuptools import setup, find_packages  # noqa: E402
 
 
-VERSION = '.'.join(('0', '2', '0'))
+VERSION = '.'.join(('0', '3', '0'))
 
 DESCRIPTION = '''Drag-and-drop multiple uploading of related images/files for
               Django admin, using Dropzone.js'''
 
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Environment :: Web Environment',
@@ -53,14 +53,16 @@
     install_requires=['Django>=3.2'],
     extras_require={
         'dev': [
             'Django>=3.2',
             'django-admin-thumbnails>=0.2.6',
             'django-cleanup>=6.0.0',
             'flake8>=3.7.7',
+            'ipdb>=0.13.13',
+            'ipython>=8.12.2',
             'Pillow>=9.1.1',
             'setuptools>=41.0.0',
             'twine>=1.13.0',
             'wheel>=0.33.1',
         ]
     },
     classifiers=CLASSIFIERS
```

