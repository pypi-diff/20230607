# Comparing `tmp/dmodel-0.0.5.tar.gz` & `tmp/dmodel-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmodel-0.0.5.tar", max compression
+gzip compressed data, was "dmodel-0.0.6.tar", max compression
```

## Comparing `dmodel-0.0.5.tar` & `dmodel-0.0.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      179 2023-06-03 03:40:49.031993 dmodel-0.0.5/dmodel/__init__.py
--rw-r--r--   0        0        0     2058 2023-06-01 15:45:38.497909 dmodel-0.0.5/dmodel/context.py
--rw-r--r--   0        0        0     3821 2023-06-01 17:09:16.404736 dmodel-0.0.5/dmodel/descriptors.py
--rw-r--r--   0        0        0      405 2023-05-31 04:15:24.383229 dmodel-0.0.5/dmodel/enums.py
--rw-r--r--   0        0        0     7577 2023-06-01 17:19:39.711949 dmodel-0.0.5/dmodel/form.py
--rw-r--r--   0        0        0       24 2023-06-03 03:40:49.033773 dmodel-0.0.5/dmodel/functions/__init__.py
--rw-r--r--   0        0        0      231 2023-06-03 03:40:49.758590 dmodel-0.0.5/dmodel/functions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1777 2023-06-03 11:57:03.655619 dmodel-0.0.5/dmodel/functions/__pycache__/iteration.cpython-39.pyc
--rw-r--r--   0        0        0      973 2023-06-03 11:57:03.031529 dmodel-0.0.5/dmodel/functions/iteration.py
--rw-r--r--   0        0        0     8801 2023-06-06 03:03:57.201311 dmodel-0.0.5/dmodel/model.py
--rw-r--r--   0        0        0      109 2023-05-31 04:24:50.902840 dmodel-0.0.5/dmodel/models/__init__.py
--rw-r--r--   0        0        0      297 2023-05-31 04:24:51.214456 dmodel-0.0.5/dmodel/models/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1154 2023-06-01 16:09:11.419206 dmodel-0.0.5/dmodel/models/__pycache__/facility.cpython-39.pyc
--rw-r--r--   0        0        0     2278 2023-06-03 12:13:17.812328 dmodel-0.0.5/dmodel/models/__pycache__/person.cpython-39.pyc
--rw-r--r--   0        0        0     4268 2023-06-03 12:13:17.815083 dmodel-0.0.5/dmodel/models/__pycache__/profile.cpython-39.pyc
--rw-r--r--   0        0        0     1778 2023-06-06 03:00:23.585737 dmodel-0.0.5/dmodel/models/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     3037 2023-06-06 03:00:23.587602 dmodel-0.0.5/dmodel/models/__pycache__/visit.cpython-39.pyc
--rw-r--r--   0        0        0      738 2023-06-01 16:09:10.856266 dmodel-0.0.5/dmodel/models/facility.py
--rw-r--r--   0        0        0     1562 2023-06-03 12:13:17.303958 dmodel-0.0.5/dmodel/models/person.py
--rw-r--r--   0        0        0     3252 2023-06-03 12:13:17.301387 dmodel-0.0.5/dmodel/models/profile.py
--rw-r--r--   0        0        0     1190 2023-06-06 03:00:23.151340 dmodel-0.0.5/dmodel/models/user.py
--rw-r--r--   0        0        0     2398 2023-06-06 03:00:23.147772 dmodel-0.0.5/dmodel/models/visit.py
--rw-r--r--   0        0        0      662 2023-05-31 04:18:41.392670 dmodel-0.0.5/dmodel/regex.py
--rw-r--r--   0        0        0      450 2023-06-01 17:08:30.423818 dmodel-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      812 2023-06-06 03:04:27.282232 dmodel-0.0.5/setup.py
--rw-r--r--   0        0        0      609 2023-06-06 03:04:27.282419 dmodel-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      179 2023-06-03 03:40:49.031993 dmodel-0.0.6/dmodel/__init__.py
+-rw-r--r--   0        0        0     2058 2023-06-01 15:45:38.497909 dmodel-0.0.6/dmodel/context.py
+-rw-r--r--   0        0        0     3821 2023-06-01 17:09:16.404736 dmodel-0.0.6/dmodel/descriptors.py
+-rw-r--r--   0        0        0      405 2023-05-31 04:15:24.383229 dmodel-0.0.6/dmodel/enums.py
+-rw-r--r--   0        0        0     7854 2023-06-07 04:08:17.161906 dmodel-0.0.6/dmodel/form.py
+-rw-r--r--   0        0        0       24 2023-06-03 03:40:49.033773 dmodel-0.0.6/dmodel/functions/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-03 03:40:49.758590 dmodel-0.0.6/dmodel/functions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1777 2023-06-03 11:57:03.655619 dmodel-0.0.6/dmodel/functions/__pycache__/iteration.cpython-39.pyc
+-rw-r--r--   0        0        0      973 2023-06-03 11:57:03.031529 dmodel-0.0.6/dmodel/functions/iteration.py
+-rw-r--r--   0        0        0     8801 2023-06-06 03:03:57.201311 dmodel-0.0.6/dmodel/model.py
+-rw-r--r--   0        0        0      109 2023-05-31 04:24:50.902840 dmodel-0.0.6/dmodel/models/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-31 04:24:51.214456 dmodel-0.0.6/dmodel/models/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1154 2023-06-01 16:09:11.419206 dmodel-0.0.6/dmodel/models/__pycache__/facility.cpython-39.pyc
+-rw-r--r--   0        0        0     2278 2023-06-03 12:13:17.812328 dmodel-0.0.6/dmodel/models/__pycache__/person.cpython-39.pyc
+-rw-r--r--   0        0        0     4268 2023-06-03 12:13:17.815083 dmodel-0.0.6/dmodel/models/__pycache__/profile.cpython-39.pyc
+-rw-r--r--   0        0        0     1778 2023-06-06 03:00:23.585737 dmodel-0.0.6/dmodel/models/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     3037 2023-06-06 03:00:23.587602 dmodel-0.0.6/dmodel/models/__pycache__/visit.cpython-39.pyc
+-rw-r--r--   0        0        0      738 2023-06-01 16:09:10.856266 dmodel-0.0.6/dmodel/models/facility.py
+-rw-r--r--   0        0        0     1562 2023-06-03 12:13:17.303958 dmodel-0.0.6/dmodel/models/person.py
+-rw-r--r--   0        0        0     3252 2023-06-03 12:13:17.301387 dmodel-0.0.6/dmodel/models/profile.py
+-rw-r--r--   0        0        0     1190 2023-06-06 03:00:23.151340 dmodel-0.0.6/dmodel/models/user.py
+-rw-r--r--   0        0        0     2398 2023-06-06 03:00:23.147772 dmodel-0.0.6/dmodel/models/visit.py
+-rw-r--r--   0        0        0      662 2023-05-31 04:18:41.392670 dmodel-0.0.6/dmodel/regex.py
+-rw-r--r--   0        0        0      450 2023-06-07 04:05:18.179170 dmodel-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      812 2023-06-07 04:08:20.950796 dmodel-0.0.6/setup.py
+-rw-r--r--   0        0        0      609 2023-06-07 04:08:20.950979 dmodel-0.0.6/PKG-INFO
```

### Comparing `dmodel-0.0.5/dmodel/context.py` & `dmodel-0.0.6/dmodel/context.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/descriptors.py` & `dmodel-0.0.6/dmodel/descriptors.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/form.py` & `dmodel-0.0.6/dmodel/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__all__ = ['FormField', 'HTMLForm']
+__all__ = ['FormField', 'HTMLForm', 'HTMXForm']
 
 from abc import ABC
 from typing import Any, Union
 from dataclasses import dataclass
 from dhint import *
 from .descriptors import *
 
@@ -124,30 +124,36 @@
             return self.textarea_field(value)
         return ''
 
 
 @dataclass
 class HTMLForm:
     model: Union[BaseDetaModel, type[BaseDetaModel]]
+    action: str
+    method: str
     delete: bool = False
     search: bool = False
     
+    @property
+    def _action(self):
+        return f'action="{self.action}"'
+    
     def form(self, form_fields):
         if self.search:
             method = 'get'
             name = f'Search{self.model.class_name()}'
         else:
             method = 'post'
             if self.delete:
                 name = f'Delete{self.model.class_name()}'
             elif isdataclass_instance(self.model):
                 name = f'Update{self.model.class_name()}'
             else:
                 name = f'New{self.model.class_name()}'
-        return f'{self.title}<form id="{name}" method="{method}">' \
+        return f'{self.title}<form id="{name}" method="{method}" {self._action}>' \
                f'{"".join([self.container(item) for item in form_fields])}{self.button}</form>'
     
     @property
     def title(self):
         if self.search:
             return f'<h2>Buscar {self.model.singular()}</h2>'
         elif self.delete:
@@ -190,7 +196,14 @@
                 form_fields = [FormField(item).render(defaults.get(item.public_name, '')) for item in
                                self.model.descriptors().values() if not item in self.model.no_form_descriptors()]
             else:
                 form_fields = [FormField(item).render(item.get_default()) for item in
                                self.model.descriptors().values() if not item in self.model.no_form_descriptors()]
         return self.form(form_fields)
 
+
+@dataclass
+class HTMXForm(HTMLForm):
+    
+    @property
+    def _action(self):
+        return f'data-hx-{self.method}="{self.action}"'
```

### Comparing `dmodel-0.0.5/dmodel/functions/__pycache__/iteration.cpython-39.pyc` & `dmodel-0.0.6/dmodel/functions/__pycache__/iteration.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/functions/iteration.py` & `dmodel-0.0.6/dmodel/functions/iteration.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/model.py` & `dmodel-0.0.6/dmodel/model.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/__pycache__/facility.cpython-39.pyc` & `dmodel-0.0.6/dmodel/models/__pycache__/facility.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/__pycache__/person.cpython-39.pyc` & `dmodel-0.0.6/dmodel/models/__pycache__/person.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/__pycache__/profile.cpython-39.pyc` & `dmodel-0.0.6/dmodel/models/__pycache__/profile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/__pycache__/user.cpython-39.pyc` & `dmodel-0.0.6/dmodel/models/__pycache__/user.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/__pycache__/visit.cpython-39.pyc` & `dmodel-0.0.6/dmodel/models/__pycache__/visit.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/facility.py` & `dmodel-0.0.6/dmodel/models/facility.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/person.py` & `dmodel-0.0.6/dmodel/models/person.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/profile.py` & `dmodel-0.0.6/dmodel/models/profile.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/user.py` & `dmodel-0.0.6/dmodel/models/user.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/models/visit.py` & `dmodel-0.0.6/dmodel/models/visit.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/dmodel/regex.py` & `dmodel-0.0.6/dmodel/regex.py`

 * *Files identical despite different names*

### Comparing `dmodel-0.0.5/setup.py` & `dmodel-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'python-multipart>=0.0.6,<0.0.7',
  'smartjs>=0.1.6,<0.2.0',
  'typing-extensions>=4.6.2,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dmodel',
-    'version': '0.0.5',
+    'version': '0.0.6',
     'description': 'models for deta space',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dmodel-0.0.5/PKG-INFO` & `dmodel-0.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmodel
-Version: 0.0.5
+Version: 0.0.6
 Summary: models for deta space
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

