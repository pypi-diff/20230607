# Comparing `tmp/strawberry_django_plus-2.6.1.tar.gz` & `tmp/strawberry_django_plus-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.6.1.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.6.2.tar", max compression
```

## Comparing `strawberry_django_plus-2.6.1.tar` & `strawberry_django_plus-2.6.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1094 2023-06-05 15:02:15.404553 strawberry_django_plus-2.6.1/LICENSE
--rw-r--r--   0        0        0     3299 2023-06-05 15:02:15.404553 strawberry_django_plus-2.6.1/README.md
--rw-r--r--   0        0        0     4309 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     3001 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5562 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1657 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-05 15:02:15.408553 strawberry_django_plus-2.6.1/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6304 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0      896 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14825 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26108 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27526 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47691 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2357 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    18702 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10297 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13069 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-06-05 15:02:15.412553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13142 2023-06-05 15:02:15.416553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-06-05 15:02:15.416553 strawberry_django_plus-2.6.1/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/LICENSE
+-rw-r--r--   0        0        0     3299 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/README.md
+-rw-r--r--   0        0        0     4309 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3001 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5562 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1657 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:15:24.256543 strawberry_django_plus-2.6.2/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6304 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0      896 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14825 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26108 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27526 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47691 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2357 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    18673 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10297 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13223 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13142 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-06-07 16:15:24.260543 strawberry_django_plus-2.6.2/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.6.2/PKG-INFO
```

### Comparing `strawberry_django_plus-2.6.1/LICENSE` & `strawberry_django_plus-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/README.md` & `strawberry_django_plus-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/pyproject.toml` & `strawberry_django_plus-2.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.6.1"
+version = "2.6.2"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -55,15 +55,15 @@
 django-guardian = "^2.4.0"
 mkdocs = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^9.0.9"
 mkdocs-minify-plugin = "^0.6.2"
 pymdown-extensions = ">=9.5,<11.0"
 Markdown = "^3.3.7"
-ruff = "^0.0.270"
+ruff = "^0.0.271"
 debugpy = "^1.6.7"
 
 
 [tool.poetry.extras]
 enum = ["django-choices-field"]
 debug-toolbar = ["django-debug-toolbar"]
```

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "2.6.1"  # x-release-please-version
+__version__ = "2.6.2"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/field.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.6.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/type.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             prefetch_related=store and store.prefetch_related,
             disable_optimization=getattr(attr, "disable_optimization", False),
             extensions=getattr(attr, "extensions", ()),
         )
     elif isinstance(attr, StrawberryResolver):
         field = StrawberryDjangoField(base_resolver=attr)
     elif callable(attr):
-        field = cast(StrawberryDjangoField, StrawberryDjangoField()(attr))
+        field = StrawberryDjangoField()(attr)
     else:
         field = StrawberryDjangoField(default=attr)
 
     field.python_name = name
     # store origin django type for further usage
     field.origin_django_type = django_type
```

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/types.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,27 +213,31 @@
 
     def merge_selections(f1: SelectedField, f2: SelectedField) -> SelectedField:
         if not f1.selections:
             return f2
         if not f2.selections:
             return f1
 
-        f1_selections = {s.name: s for s in cast(List[SelectedField], f1.selections)}
-        f2_selections = {s.name: s for s in cast(List[SelectedField], f2.selections)}
+        f1_selections = {s.name: s for s in f1.selections if isinstance(s, SelectedField)}
+        f2_selections = {s.name: s for s in f2.selections if isinstance(s, SelectedField)}
 
-        selections: Dict[str, SelectedField] = {}
+        selections: dict[str, SelectedField] = {}
         for f_name in set(f1_selections) - set(f2_selections):
             selections[f_name] = f1_selections[f_name]
         for f_name in set(f2_selections) - set(f1_selections):
             selections[f_name] = f2_selections[f_name]
         for f_name in set(f2_selections) & set(f1_selections):
             selections[f_name] = f1_selections[f_name]
             selections[f_name] = merge_selections(f1_selections[f_name], f2_selections[f_name])
 
-        f1.selections = list(selections.values())
+        f1.selections = list(selections.values()) + [
+            s
+            for s in (f1.selections + f2.selections)
+            if isinstance(s, (FragmentSpread, InlineFragment))
+        ]
         return f1
 
     for s in selection.selections:
         if isinstance(s, SelectedField):
             # @include(if: <bool>)
             include = s.directives.get("include")
             if include and not include["if"]:
```

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.6.2/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.6.1/PKG-INFO` & `strawberry_django_plus-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.6.1
+Version: 2.6.2
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

