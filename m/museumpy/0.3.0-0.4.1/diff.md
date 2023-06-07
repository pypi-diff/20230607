# Comparing `tmp/museumpy-0.3.0.tar.gz` & `tmp/museumpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "museumpy-0.3.0.tar", last modified: Wed Oct 27 15:03:10 2021, max compression
+gzip compressed data, was "museumpy-0.4.1.tar", last modified: Wed Jun  7 13:27:58 2023, max compression
```

## Comparing `museumpy-0.3.0.tar` & `museumpy-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 15:03:10.128970 museumpy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2021-10-27 15:02:52.000000 museumpy-0.3.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     6948 2021-10-27 15:03:10.128970 museumpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4728 2021-10-27 15:02:52.000000 museumpy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 15:03:10.128970 museumpy-0.3.0/museumpy/
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2021-10-27 15:02:52.000000 museumpy-0.3.0/museumpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5412 2021-10-27 15:02:52.000000 museumpy-0.3.0/museumpy/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2021-10-27 15:02:52.000000 museumpy-0.3.0/museumpy/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2021-10-27 15:02:52.000000 museumpy-0.3.0/museumpy/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-10-27 15:02:52.000000 museumpy-0.3.0/museumpy/xmlparse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 15:03:10.128970 museumpy-0.3.0/museumpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6948 2021-10-27 15:03:09.000000 museumpy-0.3.0/museumpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-10-27 15:03:09.000000 museumpy-0.3.0/museumpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 15:03:09.000000 museumpy-0.3.0/museumpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-10-27 15:03:09.000000 museumpy-0.3.0/museumpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-10-27 15:03:09.000000 museumpy-0.3.0/museumpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      158 2021-10-27 15:03:10.128970 museumpy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2021-10-27 15:02:52.000000 museumpy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:27:58.883726 museumpy-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 13:27:48.000000 museumpy-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-07 13:27:58.883726 museumpy-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-06-07 13:27:48.000000 museumpy-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:27:58.883726 museumpy-0.4.1/museumpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-07 13:27:48.000000 museumpy-0.4.1/museumpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-06-07 13:27:48.000000 museumpy-0.4.1/museumpy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 13:27:48.000000 museumpy-0.4.1/museumpy/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-06-07 13:27:48.000000 museumpy-0.4.1/museumpy/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-07 13:27:48.000000 museumpy-0.4.1/museumpy/xmlparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:27:58.883726 museumpy-0.4.1/museumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-07 13:27:58.000000 museumpy-0.4.1/museumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 13:27:58.000000 museumpy-0.4.1/museumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:27:58.000000 museumpy-0.4.1/museumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 13:27:58.000000 museumpy-0.4.1/museumpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 13:27:58.000000 museumpy-0.4.1/museumpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-07 13:27:58.883726 museumpy-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-07 13:27:48.000000 museumpy-0.4.1/setup.py
```

### Comparing `museumpy-0.3.0/LICENSE.md` & `museumpy-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `museumpy-0.3.0/PKG-INFO` & `museumpy-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: museumpy
-Version: 0.3.0
+Version: 0.4.1
 Summary: Client for MuseumPlus
 Home-page: https://github.com/metaodi/museumpy
 Author: Stefan Oderbolz
 Author-email: odi@metaodi.ch
 Maintainer: Stefan Oderbolz
 Maintainer-email: odi@metaodi.ch
 License: MIT
-Download-URL: https://github.com/metaodi/museumpy/archive/v0.3.0.zip
+Download-URL: https://github.com/metaodi/museumpy/archive/v0.4.1.zip
 Description: # museumpy
         
         **museum**py is a client for python to get data from [Zetcom MuseumPlus](https://www.zetcom.com/en/museumplus-en/) instances.
         
         ## Table of Contents
         
         * [Installation](#installation)
```

### Comparing `museumpy-0.3.0/README.md` & `museumpy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `museumpy-0.3.0/museumpy/__init__.py` & `museumpy-0.4.1/museumpy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.3.0'
+__version__ = '0.4.1'
 __all__ = ['client', 'errors', 'response', 'xmlparse']
 
 from .errors import MuseumpyError  # noqa
 from .client import MuseumPlusClient
 
 def fulltext_search(base_url, query, **kwargs):  # noqa
     search_params = ['query', 'module', 'limit', 'offset']
@@ -12,19 +12,32 @@
     # assume all others kwargs are for the client
     client_kwargs = {k: v for k, v in kwargs.items() if k not in search_params}
     client_kwargs['base_url'] = base_url
 
     c = MuseumPlusClient(**client_kwargs)
     return c.search(**search_kwargs)
 
+
 def search(base_url, field, value, **kwargs):  # noqa
     search_params = ['field', 'value', 'module', 'limit', 'offset']
     search_kwargs = {k: v for k, v in kwargs.items() if k in search_params}
     search_kwargs['field'] = field
     search_kwargs['value'] = value
 
     # assume all others kwargs are for the client
     client_kwargs = {k: v for k, v in kwargs.items() if k not in search_params}
     client_kwargs['base_url'] = base_url
 
     c = MuseumPlusClient(**client_kwargs)
     return c.search(**search_kwargs)
+
+
+def exports(base_url, **kwargs):
+    exports_params = ['module']
+    export_kwargs = {k: v for k, v in kwargs.items() if k in exports_params}
+
+    # assume all others kwargs are for the client
+    client_kwargs = {k: v for k, v in kwargs.items() if k not in exports_params}
+    client_kwargs['base_url'] = base_url
+
+    c = MuseumPlusClient(**client_kwargs)
+    return c.exports(**export_kwargs)
```

### Comparing `museumpy-0.3.0/museumpy/errors.py` & `museumpy-0.4.1/museumpy/errors.py`

 * *Files identical despite different names*

### Comparing `museumpy-0.3.0/museumpy/response.py` & `museumpy-0.4.1/museumpy/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from . import xmlparse
 from . import errors
 
 ZETCOM_NS = "http://www.zetcom.com/ria/ws/module"
+EXPORT_NS = "http://www.zetcom.com/ria/ws/module/export"
 
 
 class SearchResponse(object):
     def __init__(self, data_loader, limit=100, offset=0, map_function=None):
         self.data_loader = data_loader
         self.xmlparser = xmlparse.XMLParser()
         self.records = []
@@ -147,7 +148,58 @@
 
     def _load_new_data(self):
         self.offset = self.offset + self.limit
         if self.offset >= self.count:
             raise errors.NoMoreRecordsError("There are no more records")
         xml = self.data_loader.load(limit=self.limit, offset=self.offset)
         self._parse_content(xml)
+
+
+class ExportResponse(object):
+    def __init__(self, data_loader):
+        self.data_loader = data_loader
+        self.xmlparser = xmlparse.XMLParser()
+        self.exports = []
+        xml = data_loader.load()
+        self._parse_content(xml)
+
+    def _parse_content(self, xml):
+        self._extract_exports(xml)
+
+    def _extract_exports(self, xml):
+        xml_recs = self.xmlparser.findall(xml, f'.//{{{EXPORT_NS}}}export')  # noqa
+        for xml_rec in xml_recs:
+            export = self._map_xml(xml_rec)
+            export['raw'] = self.xmlparser.todict(xml_rec, xml_attribs=True)
+            self.exports.append(export)
+
+    def _map_xml(self, xml_rec):
+        def xml_text(xpath):
+            return self.xmlparser.find(xml_rec, xpath).text
+
+        export = {
+            'id': xml_rec.attrib['id'],
+            'extension': xml_text(f".//{{{EXPORT_NS}}}extension"),
+            'label': xml_text(f".//{{{EXPORT_NS}}}label"),
+        }
+        return export
+
+    def __repr__(self):
+        try:
+            return (
+                'ExportResponse('
+                'count=%r)'
+                ) % (
+                   len(self.exports)
+                )
+        except AttributeError:
+            return 'ExportResponse(empty)'
+
+    def __len__(self):
+        return len(self.exports)
+
+    def __iter__(self):
+        for export in self.exports:
+            yield export
+
+    def __getitem__(self, key):
+        return self.exports[key]
```

### Comparing `museumpy-0.3.0/museumpy/xmlparse.py` & `museumpy-0.4.1/museumpy/xmlparse.py`

 * *Files identical despite different names*

### Comparing `museumpy-0.3.0/museumpy.egg-info/PKG-INFO` & `museumpy-0.4.1/museumpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: museumpy
-Version: 0.3.0
+Version: 0.4.1
 Summary: Client for MuseumPlus
 Home-page: https://github.com/metaodi/museumpy
 Author: Stefan Oderbolz
 Author-email: odi@metaodi.ch
 Maintainer: Stefan Oderbolz
 Maintainer-email: odi@metaodi.ch
 License: MIT
-Download-URL: https://github.com/metaodi/museumpy/archive/v0.3.0.zip
+Download-URL: https://github.com/metaodi/museumpy/archive/v0.4.1.zip
 Description: # museumpy
         
         **museum**py is a client for python to get data from [Zetcom MuseumPlus](https://www.zetcom.com/en/museumplus-en/) instances.
         
         ## Table of Contents
         
         * [Installation](#installation)
```

### Comparing `museumpy-0.3.0/setup.py` & `museumpy-0.4.1/setup.py`

 * *Files identical despite different names*

