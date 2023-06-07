# Comparing `tmp/pypeman-0.5.2.tar.gz` & `tmp/pypeman-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypeman-0.5.2.tar", last modified: Thu Jun  1 14:28:20 2023, max compression
+gzip compressed data, was "pypeman-0.5.3.tar", last modified: Wed Jun  7 12:56:44 2023, max compression
```

## Comparing `pypeman-0.5.2.tar` & `pypeman-0.5.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    11358 2023-06-01 14:13:10.000000 pypeman-0.5.2/LICENSE
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       41 2023-06-01 14:13:10.000000 pypeman-0.5.2/MANIFEST.in
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-06-01 14:28:20.554592 pypeman-0.5.2/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1928 2023-06-01 14:13:10.000000 pypeman-0.5.2/README.rst
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       68 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    34065 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/channels.py
--rwxrwxr-x   0 quentin   (1000) quentin   (1000)    12351 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/commands.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2443 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/conf.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman/contrib/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3606 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/csv.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2178 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/ctx.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     8624 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/ftp.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6612 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/hl7.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    10070 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/http.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      803 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/time.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      971 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/contrib/xml.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2126 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/debug.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1451 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/default_settings.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3437 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/endpoints.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      189 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/errors.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1395 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/events.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2577 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/graph.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman/helpers/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/__init__.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      421 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/aio_compat.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3247 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/cli.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      235 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/itertools.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1894 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/lazyload.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      663 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/logging.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3005 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/reloader.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1216 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/sleeper.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      315 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/helpers/tempfile.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1335 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/map_item.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     6369 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/message.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    16408 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/msgstore.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    27977 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/nodes.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3713 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/persistence.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3946 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/pjt_templates.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3008 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/plugin_mgr.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)    19018 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/remoteadmin.py
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3790 2023-06-01 14:13:10.000000 pypeman-0.5.2/pypeman/test.py
-drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-01 14:28:20.554592 pypeman-0.5.2/pypeman.egg-info/
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/PKG-INFO
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     1056 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/SOURCES.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/dependency_links.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)       49 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/entry_points.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      175 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/requires.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)        8 2023-06-01 14:28:20.000000 pypeman-0.5.2/pypeman.egg-info/top_level.txt
--rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2023-06-01 14:28:20.558592 pypeman-0.5.2/setup.cfg
--rw-rw-r--   0 quentin   (1000) quentin   (1000)     2216 2023-06-01 14:13:10.000000 pypeman-0.5.2/setup.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-07 12:56:44.404276 pypeman-0.5.3/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    11358 2023-06-07 12:24:15.000000 pypeman-0.5.3/LICENSE
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       41 2023-06-07 12:24:15.000000 pypeman-0.5.3/MANIFEST.in
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-06-07 12:56:44.404276 pypeman-0.5.3/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1928 2023-06-07 12:24:15.000000 pypeman-0.5.3/README.rst
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-07 12:56:44.400276 pypeman-0.5.3/pypeman/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       68 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    34088 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/channels.py
+-rwxrwxr-x   0 quentin   (1000) quentin   (1000)    12351 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/commands.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2443 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/conf.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-07 12:56:44.404276 pypeman-0.5.3/pypeman/contrib/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3606 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/csv.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2178 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/ctx.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     8624 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/ftp.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6750 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/hl7.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    10401 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/http.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      803 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/time.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      971 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/contrib/xml.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2126 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/debug.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1451 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/default_settings.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3433 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/endpoints.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      189 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/errors.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1395 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/events.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2577 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/graph.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-07 12:56:44.404276 pypeman-0.5.3/pypeman/helpers/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        0 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/__init__.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      421 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/aio_compat.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3247 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/cli.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      235 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/itertools.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1894 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/lazyload.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      663 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/logging.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3005 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/reloader.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1216 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/sleeper.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      315 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/helpers/tempfile.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1335 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/map_item.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     6369 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/message.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    16408 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/msgstore.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    27977 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/nodes.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3713 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/persistence.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3946 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/pjt_templates.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3008 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/plugin_mgr.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)    19018 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/remoteadmin.py
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3790 2023-06-07 12:24:15.000000 pypeman-0.5.3/pypeman/test.py
+drwxrwxr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-07 12:56:44.400276 pypeman-0.5.3/pypeman.egg-info/
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     3077 2023-06-07 12:56:44.000000 pypeman-0.5.3/pypeman.egg-info/PKG-INFO
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     1056 2023-06-07 12:56:44.000000 pypeman-0.5.3/pypeman.egg-info/SOURCES.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        1 2023-06-07 12:56:44.000000 pypeman-0.5.3/pypeman.egg-info/dependency_links.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)       49 2023-06-07 12:56:44.000000 pypeman-0.5.3/pypeman.egg-info/entry_points.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      175 2023-06-07 12:56:44.000000 pypeman-0.5.3/pypeman.egg-info/requires.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)        8 2023-06-07 12:56:44.000000 pypeman-0.5.3/pypeman.egg-info/top_level.txt
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)      279 2023-06-07 12:56:44.404276 pypeman-0.5.3/setup.cfg
+-rw-rw-r--   0 quentin   (1000) quentin   (1000)     2216 2023-06-07 12:24:15.000000 pypeman-0.5.3/setup.py
```

### Comparing `pypeman-0.5.2/LICENSE` & `pypeman-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/PKG-INFO` & `pypeman-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.2
+Version: 0.5.3
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pypeman-0.5.2/README.rst` & `pypeman-0.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/channels.py` & `pypeman-0.5.3/pypeman/channels.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,26 +383,27 @@
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
                 await self.message_store.change_message_state(msg_store_id, message.Message.PROCESSED)
                 if self.drop_nodes and not has_callback:
                     await self.drop_nodes[0].handle(msg.copy())
                 if self.raise_dropped:
                     raise
+                return msg
             except Rejected as exc:
                 self.logger.info("%s REJECT msg %s", str(self), str(msg))
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
                 await self.message_store.change_message_state(msg_store_id, message.Message.REJECTED)
                 if self.reject_nodes and not has_callback:
                     await self.reject_nodes[0].handle(msg.copy())
                 raise
             except Exception as exc:
                 msg.chan_exc = exc
                 msg.chan_exc_traceback = traceback.format_exc()
-                self.logger.exception('Error while processing message %s (chan %s)', str(msg), str(self))
+                self.logger.error('Error while processing message %s (chan %s)', str(msg), str(self))
                 await self.message_store.change_message_state(msg_store_id, message.Message.ERROR)
                 if self.fail_nodes and not has_callback:
                     await self.fail_nodes[0].handle(msg.copy())
                 raise
             finally:
                 self.status = BaseChannel.WAITING
                 self.processed_msgs += 1
```

### Comparing `pypeman-0.5.2/pypeman/commands.py` & `pypeman-0.5.3/pypeman/commands.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/conf.py` & `pypeman-0.5.3/pypeman/conf.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/contrib/csv.py` & `pypeman-0.5.3/pypeman/contrib/csv.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/contrib/ctx.py` & `pypeman-0.5.3/pypeman/contrib/ctx.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/contrib/ftp.py` & `pypeman-0.5.3/pypeman/contrib/ftp.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/contrib/hl7.py` & `pypeman-0.5.3/pypeman/contrib/hl7.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,17 @@
         await super().start()
         self.mllp_endpoint.set_handler(handler=self.handle_hl7_message)
 
     async def handle_hl7_message(self, hl7_message):
         content = hl7_message.decode(self.encoding)
         msg = message.Message(content_type='text/hl7', payload=content, meta={})
         try:
-            result = await self.handle(msg)
-            return result.payload.encode(self.encoding)
+            await self.handle(msg)
+            ack = hl7.parse(content, encoding=self.encoding)
+            return str(ack.create_ack('AA')).encode(self.encoding)
         except channels.Dropped:
             ack = hl7.parse(content, encoding=self.encoding)
             return str(ack.create_ack('AA')).encode(self.encoding)
         except channels.Rejected:
             ack = hl7.parse(content, encoding=self.encoding)
             return str(ack.create_ack('AR')).encode(self.encoding)
         except Exception:
@@ -165,19 +166,20 @@
             ack = hl7.parse(content, encoding=self.encoding)
             return str(ack.create_ack('AE')).encode(self.encoding)
 
 
 class HL7ToPython(nodes.BaseNode):
     """ Convert hl7 payload to python struct."""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, encoding="utf-8", **kwargs):
+        self.encoding = encoding
         super().__init__(*args, **kwargs)
 
     def process(self, msg):
-        msg.payload = hl7.parse(msg.payload)
+        msg.payload = hl7.parse(msg.payload, encoding=self.encoding)
         msg.content_type = 'application/python'
         return msg
 
 
 class PythonToHL7(nodes.BaseNode):
     """ Convert python payload to HL7. Must be HL7 structure."""
```

### Comparing `pypeman-0.5.2/pypeman/contrib/http.py` & `pypeman-0.5.3/pypeman/contrib/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,16 @@
             'get_params': dict(request.query),
             })
 
         msg = message.Message(content_type='http_request', payload=content, meta=meta)
         try:
             result = await self.handle(msg)
             encoding = self.encoding or 'utf-8'
-            return web.Response(body=result.payload.encode(encoding), status=result.meta.get('status', 200))
+            return web.Response(
+                body=str(result.payload).encode(encoding), status=result.meta.get('status', 200))
 
         except channels.Dropped:
             return web.Response(body="Dropped".encode('utf-8'), status=200)
         except Exception as exc:
             logger.exception(
                 "HttpChannel %s raise an error, cannot send 200 speed response, will return 503",
                 str(self))
@@ -174,32 +175,39 @@
         url_dict = msg.meta
         if self.payload_in_url_dict:
             url_dict = dict(url_dict)
             try:
                 for key, val in msg.payload.items():
                     url_dict['payload.' + key] = val
             except AttributeError:
-                self.channel.logger.exception(
+                self.channel.logger.error(
                     "Payload must be a python dict if used to generate url. "
                     "This can be fixed using JsonToPython node before your "
                     "RequestNode")
                 raise
-        return self.url % url_dict
+        try:
+            request_url = self.url % url_dict
+        except Exception as exc:
+            logger.error("cannot create url %r with args %r", self.url, repr(url_dict))
+            raise exc
+        return request_url
 
     async def handle_request(self, msg):
         """ generate url and handle request """
         url = self.generate_request_url(msg)
         loop = self.channel.loop
         conn = None
         ssl_context = None
         if self.client_cert:
             if self.verify:
                 ssl_context = ssl.create_default_context()
             else:
                 ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+                ssl_context.check_hostname = False
+                ssl_context.verify_mode = ssl.CERT_NONE
             try:
                 ssl_context.load_cert_chain(self.client_cert[0], self.client_cert[1])
             except FileNotFoundError:
                 logger.error("loading certs %s failed", self.client_cert)
                 raise
             conn = aiohttp.TCPConnector(ssl=ssl_context, loop=loop)
         else:
@@ -243,25 +251,26 @@
                         method=method,
                         url=url,
                         auth=basic_auth,
                         headers=headers,
                         params=get_params,
                         data=data
                         )
-            if self.binary:
-                resp_content = await resp.read()
-            else:
-                resp_content = str(await resp.text())
-            if self.json:
-                try:
-                    resp_content = json.loads(resp_content)
-                except Exception as exc:
-                    logger.error(
-                        "cannot json parse response from url %s (response=%r)",
-                        url, resp_content)
-                    raise exc
-            return resp_content
+        return resp
 
     async def process(self, msg):
         """ handles request """
-        msg.payload = await self.handle_request(msg)
+        resp = await self.handle_request(msg)
+        msg.meta["status_code"] = resp.status
+        if self.binary:
+            resp_content = await resp.read()
+        else:
+            resp_content = str(await resp.text())
+        if self.json:
+            try:
+                resp_content = json.loads(resp_content)
+            except Exception:
+                logger.exception(
+                    "cannot json parse response from url %s (response=%r)",
+                    self.generate_request_url(msg), resp_content)
+        msg.payload = resp_content
         return msg
```

### Comparing `pypeman-0.5.2/pypeman/contrib/time.py` & `pypeman-0.5.3/pypeman/contrib/time.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/contrib/xml.py` & `pypeman-0.5.3/pypeman/contrib/xml.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/debug.py` & `pypeman-0.5.3/pypeman/debug.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/default_settings.py` & `pypeman-0.5.3/pypeman/default_settings.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/endpoints.py` & `pypeman-0.5.3/pypeman/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 try:
                     host, port = sock.split(":")
                     port = int(port)
                     if not host:
                         raise
                     bind_param = (host, port)
                 except Exception:
-                    logger.exception('error on sock params in socket endpoint')
+                    logger.error('error on sock params in socket endpoint')
                     raise
                 sock_obj = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 sock_obj.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             else:
                 bind_param = sock.split(":", 1)[1]
                 sock_obj = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
             if reuse_port:
```

### Comparing `pypeman-0.5.2/pypeman/events.py` & `pypeman-0.5.3/pypeman/events.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/graph.py` & `pypeman-0.5.3/pypeman/graph.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/helpers/cli.py` & `pypeman-0.5.3/pypeman/helpers/cli.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/helpers/lazyload.py` & `pypeman-0.5.3/pypeman/helpers/lazyload.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/helpers/logging.py` & `pypeman-0.5.3/pypeman/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/helpers/reloader.py` & `pypeman-0.5.3/pypeman/helpers/reloader.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/helpers/sleeper.py` & `pypeman-0.5.3/pypeman/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/map_item.py` & `pypeman-0.5.3/pypeman/map_item.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/message.py` & `pypeman-0.5.3/pypeman/message.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/msgstore.py` & `pypeman-0.5.3/pypeman/msgstore.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/nodes.py` & `pypeman-0.5.3/pypeman/nodes.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/persistence.py` & `pypeman-0.5.3/pypeman/persistence.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/pjt_templates.py` & `pypeman-0.5.3/pypeman/pjt_templates.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/plugin_mgr.py` & `pypeman-0.5.3/pypeman/plugin_mgr.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/remoteadmin.py` & `pypeman-0.5.3/pypeman/remoteadmin.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman/test.py` & `pypeman-0.5.3/pypeman/test.py`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/pypeman.egg-info/PKG-INFO` & `pypeman-0.5.3/pypeman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypeman
-Version: 0.5.2
+Version: 0.5.3
 Summary: Minimalistic but pragmatic ESB / ETL / EAI in Python
 Home-page: https://github.com/mhcomm/pypeman
 Author: Jeremie Pardou
 Author-email: jeremie@jeremiez.net
 License: Apache Software License
 Keywords: esb etl eai pipeline data processing asyncio http ftp hl7
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pypeman-0.5.2/pypeman.egg-info/SOURCES.txt` & `pypeman-0.5.3/pypeman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypeman-0.5.2/setup.py` & `pypeman-0.5.3/setup.py`

 * *Files identical despite different names*

