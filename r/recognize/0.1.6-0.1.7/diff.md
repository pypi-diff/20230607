# Comparing `tmp/recognize-0.1.6.tar.gz` & `tmp/recognize-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognize-0.1.6.tar", max compression
+gzip compressed data, was "recognize-0.1.7.tar", max compression
```

## Comparing `recognize-0.1.6.tar` & `recognize-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.6/README.md
--rw-r--r--   0        0        0      436 2023-06-07 15:56:14.645202 recognize-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.6/recognize/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.6/recognize/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.6/recognize/commands/lib/__init__.py
--rw-r--r--   0        0        0     4380 2023-06-07 15:55:40.787734 recognize-0.1.6/recognize/commands/lib/client.py
--rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.6/recognize/commands/lib/entries.py
--rw-r--r--   0        0        0     1574 2023-06-07 14:04:50.724674 recognize-0.1.6/recognize/commands/lib/helpers.py
--rw-r--r--   0        0        0     3288 2023-06-07 14:12:08.572874 recognize-0.1.6/recognize/commands/search.py
--rw-r--r--   0        0        0     1723 2023-06-07 14:12:08.612866 recognize-0.1.6/recognize/commands/upload.py
--rw-r--r--   0        0        0      713 2023-06-07 15:55:18.465021 recognize-0.1.6/recognize/main.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 recognize-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:54:25.494041 recognize-0.1.7/README.md
+-rw-r--r--   0        0        0      436 2023-06-07 20:13:14.449781 recognize-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 10:51:05.501277 recognize-0.1.7/recognize/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:10:35.106880 recognize-0.1.7/recognize/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-03 22:21:58.098646 recognize-0.1.7/recognize/commands/lib/__init__.py
+-rw-r--r--   0        0        0     4453 2023-06-07 20:13:02.725616 recognize-0.1.7/recognize/commands/lib/client.py
+-rw-r--r--   0        0        0      175 2023-06-05 10:43:58.870449 recognize-0.1.7/recognize/commands/lib/entries.py
+-rw-r--r--   0        0        0     1574 2023-06-07 17:10:59.829887 recognize-0.1.7/recognize/commands/lib/helpers.py
+-rw-r--r--   0        0        0     3288 2023-06-07 17:10:59.830868 recognize-0.1.7/recognize/commands/search.py
+-rw-r--r--   0        0        0     1723 2023-06-07 17:10:59.831782 recognize-0.1.7/recognize/commands/upload.py
+-rw-r--r--   0        0        0      713 2023-06-07 17:10:59.832702 recognize-0.1.7/recognize/main.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 recognize-0.1.7/PKG-INFO
```

### Comparing `recognize-0.1.6/recognize/commands/lib/client.py` & `recognize-0.1.7/recognize/commands/lib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,20 @@
         }, files=files) as response, \
                 open(output_file, "wb") as output:
             self._process_response(output, response)
 
     async def upload_files(self, base_path, file_paths: Generator[str, None, None]) -> None:
         """Upload files concurrently to a given URL."""
         url = urljoin(self.url, f"upload/{base_path}")
-        st = speedtest.Speedtest()
-        upload_speed_mbps = st.upload() / 1e6  # Convert bits per second to Mbps
+
+        try:
+            st = speedtest.Speedtest()
+            upload_speed_mbps = st.upload() / 1e6  # Convert bits per second to Mbps
+        except:
+            upload_speed_mbps = 10
 
         semaphore = asyncio.Semaphore(max(1, int(upload_speed_mbps / 2)))
 
         tasks = [upload_file(semaphore, file_path, url, self.dev) for file_path in file_paths]
 
         with rich.progress.Progress(
                 "[progress.percentage]{task.percentage:>3.0f}%",
```

### Comparing `recognize-0.1.6/recognize/commands/lib/helpers.py` & `recognize-0.1.7/recognize/commands/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.6/recognize/commands/search.py` & `recognize-0.1.7/recognize/commands/search.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.6/recognize/commands/upload.py` & `recognize-0.1.7/recognize/commands/upload.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.6/recognize/main.py` & `recognize-0.1.7/recognize/main.py`

 * *Files identical despite different names*

### Comparing `recognize-0.1.6/PKG-INFO` & `recognize-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recognize
-Version: 0.1.6
+Version: 0.1.7
 Summary: CLI for ML Pipeline
 Author: Oscar King
 Author-email: oscarking.nl@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

