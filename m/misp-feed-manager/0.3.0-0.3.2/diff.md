# Comparing `tmp/misp-feed-manager-0.3.0.tar.gz` & `tmp/misp-feed-manager-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "misp-feed-manager-0.3.0.tar", last modified: Fri Jun  2 09:13:14 2023, max compression
+gzip compressed data, was "misp-feed-manager-0.3.2.tar", last modified: Wed Jun  7 08:30:34 2023, max compression
```

## Comparing `misp-feed-manager-0.3.0.tar` & `misp-feed-manager-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4436 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/bin/consume_feed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/bin/generate_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/src/feed_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14623 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/src/feed_manager/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-02 09:13:14.000000 misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:13:14.507787 misp-feed-manager-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-02 09:13:01.000000 misp-feed-manager-0.3.0/tests/test_translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:30:34.207516 misp-feed-manager-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-07 08:30:34.207516 misp-feed-manager-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:30:34.203516 misp-feed-manager-0.3.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4436 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/bin/consume_feed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4932 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/bin/generate_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 08:30:34.207516 misp-feed-manager-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:30:34.203516 misp-feed-manager-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:30:34.203516 misp-feed-manager-0.3.2/src/feed_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/src/feed_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/src/feed_manager/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14623 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/src/feed_manager/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/src/feed_manager/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/src/feed_manager/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:30:34.207516 misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-07 08:30:34.000000 misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-07 08:30:34.000000 misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:30:34.000000 misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 08:30:34.000000 misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 08:30:34.000000 misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:30:34.207516 misp-feed-manager-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-07 08:30:21.000000 misp-feed-manager-0.3.2/tests/test_translator.py
```

### Comparing `misp-feed-manager-0.3.0/LICENSE` & `misp-feed-manager-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/PKG-INFO` & `misp-feed-manager-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misp-feed-manager
-Version: 0.3.0
+Version: 0.3.2
 Summary: Set of utilities to manage MISP feeds
 Home-page: https://github.com/vmware-labs/feed-manager-for-misp/
 Author: Stefano Ortolani
 Project-URL: Bug Tracker, https://github.com/vmware-labs/feed-manager-for-misp/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `misp-feed-manager-0.3.0/README.md` & `misp-feed-manager-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/bin/consume_feed.py` & `misp-feed-manager-0.3.2/bin/consume_feed.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/bin/generate_feed.py` & `misp-feed-manager-0.3.2/bin/generate_feed.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/pyproject.toml` & `misp-feed-manager-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/setup.cfg` & `misp-feed-manager-0.3.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = misp-feed-manager
-version = 0.3.0
+version = 0.3.2
 author = Stefano Ortolani
 description = Set of utilities to manage MISP feeds
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/vmware-labs/feed-manager-for-misp/
 project_urls = 
 	Bug Tracker = https://github.com/vmware-labs/feed-manager-for-misp/issues
```

### Comparing `misp-feed-manager-0.3.0/src/feed_manager/__init__.py` & `misp-feed-manager-0.3.2/src/feed_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/src/feed_manager/consumer.py` & `misp-feed-manager-0.3.2/src/feed_manager/consumer.py`

 * *Files 15% similar despite different names*

```diff
@@ -265,14 +265,19 @@
 
     def __init__(self, storage_layer):
         """Constructor."""
         self._logger = logging.getLogger(__name__)
         self._storage_layer = storage_layer
 
     @classmethod
+    def _round_timestamp_to_day(cls, timestamp: int) -> int:
+        """Round timestamp at day granularity level."""
+        return timestamp - (timestamp % (3600 * 24))
+
+    @classmethod
     def _infer_parser_class(cls, event_data: Dict) -> Type[BaseFeedParserSubType]:
         """Return the parser class able to read the feed."""
         objects_data = event_data["Event"].get("Object", [])
         attributes_data = event_data["Event"].get("Attribute", [])
         for object_data in objects_data:
             if object_data["name"] in ObjectFactory.TELEMETRY_OBJECT_NAMES:
                 return TelemetryFeedParser
@@ -289,14 +294,31 @@
         return event_uuids
 
     def _get_events_since(self, date_object: datetime.datetime) -> List[Dict]:
         """Return list of event data objects."""
         event_uuids = self._get_event_uuids_since(date_object.timestamp())
         return [self._storage_layer.load_event(x) for x in event_uuids]
 
+    def _get_event_uuids_on(self, timestamp: float = None) -> List[str]:
+        """Read the manifest and return the event uuid matching the filter."""
+        event_uuids = []
+        target_timestamp = self._round_timestamp_to_day(int(timestamp))
+        for event_uuid, event_data in self._storage_layer.load_manifest().items():
+            if (
+                not timestamp
+                or self._round_timestamp_to_day(event_data["timestamp"]) == target_timestamp
+            ):
+                event_uuids.append(event_uuid)
+        return event_uuids
+
+    def _get_events_on(self, date_object: datetime.datetime) -> List[Dict]:
+        """Return list of event data objects."""
+        event_uuids = self._get_event_uuids_on(date_object.timestamp())
+        return [self._storage_layer.load_event(x) for x in event_uuids]
+
     @classmethod
     def _get_tag_galaxy(cls, tag_name: str) -> Optional[str]:
         """Get the galaxy if the tag is a MISP galaxy cluster."""
         try:
             category = tag_name.split("=")[0]
             tag_type, tag_galaxy = category.split(":")
             return tag_galaxy if tag_type == "misp-galaxy" else None
@@ -331,7 +353,26 @@
                 with parser_class(event_data) as parser:
                     for indicator in parser:
                         if self._filter_indicator(indicator, attribute_type, galaxy_name):
                             ret.append(indicator)
             except EmptyFeedException:
                 self._logger.warning("The feed '%s' is empty", event_data["Event"]["info"])
         return ret
+
+    def get_items_on(
+        self,
+        date_objects: List[datetime.datetime],
+        attribute_type: Optional[str] = None,
+        galaxy_name: Optional[str] = None,
+    ) -> List[Dict]:
+        """Return the items contained in the feed."""
+        ret = []
+        for date_object in date_objects:
+            for event_data in self._get_events_on(date_object):
+                parser_class = self._infer_parser_class(event_data)
+                with parser_class(event_data) as parser:
+                    for indicator in parser:
+                        if self._filter_indicator(indicator, attribute_type, galaxy_name):
+                            ret.append(indicator)
+        if not ret:
+            self._logger.warning("The feed is empty")
+        return ret
```

### Comparing `misp-feed-manager-0.3.0/src/feed_manager/generator.py` & `misp-feed-manager-0.3.2/src/feed_manager/generator.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/src/feed_manager/storage.py` & `misp-feed-manager-0.3.2/src/feed_manager/storage.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/src/feed_manager/translator.py` & `misp-feed-manager-0.3.2/src/feed_manager/translator.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/PKG-INFO` & `misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misp-feed-manager
-Version: 0.3.0
+Version: 0.3.2
 Summary: Set of utilities to manage MISP feeds
 Home-page: https://github.com/vmware-labs/feed-manager-for-misp/
 Author: Stefano Ortolani
 Project-URL: Bug Tracker, https://github.com/vmware-labs/feed-manager-for-misp/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `misp-feed-manager-0.3.0/src/misp_feed_manager.egg-info/SOURCES.txt` & `misp-feed-manager-0.3.2/src/misp_feed_manager.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,10 +12,11 @@
 src/feed_manager/storage.py
 src/feed_manager/translator.py
 src/misp_feed_manager.egg-info/PKG-INFO
 src/misp_feed_manager.egg-info/SOURCES.txt
 src/misp_feed_manager.egg-info/dependency_links.txt
 src/misp_feed_manager.egg-info/requires.txt
 src/misp_feed_manager.egg-info/top_level.txt
+tests/test_consumer.py
 tests/test_generator.py
 tests/test_storage.py
 tests/test_translator.py
```

### Comparing `misp-feed-manager-0.3.0/tests/test_generator.py` & `misp-feed-manager-0.3.2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/tests/test_storage.py` & `misp-feed-manager-0.3.2/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `misp-feed-manager-0.3.0/tests/test_translator.py` & `misp-feed-manager-0.3.2/tests/test_translator.py`

 * *Files identical despite different names*

