# Comparing `tmp/cosmian_py_ggml-0.2.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/cosmian_py_ggml-0.3.0-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 272221 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:20 cosmian_py_ggml.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-31 13:20 cosmian_py_ggml/
--rw-r--r--  2.0 unx     1315 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx     1064 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      592 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/RECORD
--rw-r--r--  2.0 unx      165 b- defN 23-May-31 13:20 cosmian_py_ggml-0.2.0.dist-info/WHEEL
--rwxr-xr-x  2.0 unx   684448 b- defN 23-May-31 13:20 cosmian_py_ggml/libggml-gptneox.so
--rw-r--r--  2.0 unx     5334 b- defN 23-May-31 13:20 cosmian_py_ggml/gpt_neox.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-31 13:20 cosmian_py_ggml/__init__.py
-10 files, 692918 bytes uncompressed, 270817 bytes compressed:  60.9%
+Zip file size: 272230 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-07 09:55 cosmian_py_ggml-0.3.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-07 09:55 cosmian_py_ggml.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-07 09:55 cosmian_py_ggml/
+-rw-r--r--  2.0 unx     1315 b- defN 23-Jun-07 09:55 cosmian_py_ggml-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx     1064 b- defN 23-Jun-07 09:55 cosmian_py_ggml-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      592 b- defN 23-Jun-07 09:55 cosmian_py_ggml-0.3.0.dist-info/RECORD
+-rw-r--r--  2.0 unx      165 b- defN 23-Jun-07 09:55 cosmian_py_ggml-0.3.0.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx   684448 b- defN 23-Jun-07 09:55 cosmian_py_ggml/libggml-gptneox.so
+-rw-r--r--  2.0 unx     5358 b- defN 23-Jun-07 09:55 cosmian_py_ggml/gpt_neox.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 09:55 cosmian_py_ggml/__init__.py
+10 files, 692942 bytes uncompressed, 270826 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -1,26 +1,26 @@
-Filename: cosmian_py_ggml.libs/
+Filename: cosmian_py_ggml-0.3.0.dist-info/
 Comment: 
 
-Filename: cosmian_py_ggml-0.2.0.dist-info/
+Filename: cosmian_py_ggml.libs/
 Comment: 
 
 Filename: cosmian_py_ggml/
 Comment: 
 
-Filename: cosmian_py_ggml-0.2.0.dist-info/METADATA
+Filename: cosmian_py_ggml-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_py_ggml-0.2.0.dist-info/LICENSE
+Filename: cosmian_py_ggml-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: cosmian_py_ggml-0.2.0.dist-info/RECORD
+Filename: cosmian_py_ggml-0.3.0.dist-info/RECORD
 Comment: 
 
-Filename: cosmian_py_ggml-0.2.0.dist-info/WHEEL
+Filename: cosmian_py_ggml-0.3.0.dist-info/WHEEL
 Comment: 
 
 Filename: cosmian_py_ggml/libggml-gptneox.so
 Comment: 
 
 Filename: cosmian_py_ggml/gpt_neox.py
 Comment:
```

## cosmian_py_ggml/gpt_neox.py

```diff
@@ -143,15 +143,15 @@
     if stream_callback:
         thread_stop_event = threading.Event()
 
         # Define a thread to handle streaming of generated tokens
         def stream_thread():
             len = 0
             while True:
-                time.sleep(1)
+                time.sleep(0.5)
                 tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
                 curr_len = tokens.index(0)
                 if curr_len > len:
                     stream_callback(tokens[len:curr_len])
                     len = curr_len
 
                 if thread_stop_event.is_set():
@@ -173,12 +173,13 @@
         top_k,
         top_p,
         temp,
     )
 
     # Stop the stream_thread if it was started
     if thread_stop_event is not None:
+        time.sleep(1)
         thread_stop_event.set()
 
     # Retrieve the generated tokens and return them
     output_tokens = [output_tokens_arr[i] for i in range(output_tokens_len)]
     return output_tokens[: output_tokens.index(0) + 1]
```

## Comparing `cosmian_py_ggml-0.2.0.dist-info/METADATA` & `cosmian_py_ggml-0.3.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmian-py-ggml
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python bindings for GGML
 License: MIT
 Author: Hugo Rosenkranz-Costa
 Author-email: hugo.rosenkranz@cosmian.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `cosmian_py_ggml-0.2.0.dist-info/LICENSE` & `cosmian_py_ggml-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cosmian_py_ggml-0.2.0.dist-info/RECORD` & `cosmian_py_ggml-0.3.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-cosmian_py_ggml-0.2.0.dist-info/METADATA,sha256=mRPEMa2a57KswBmtrIt9xXZpjV6nkcvtHrzm6lYJzpo,1315
-cosmian_py_ggml-0.2.0.dist-info/LICENSE,sha256=Z0wEwlIqJt-ulg5-OWzUBniisSSS6B_bRz_PWVktGMQ,1064
-cosmian_py_ggml-0.2.0.dist-info/RECORD,,
-cosmian_py_ggml-0.2.0.dist-info/WHEEL,sha256=Pakn5EYkUcLl97jUMw4FC8DAw0ZnXzfAMJoDBnx1DlE,165
+cosmian_py_ggml-0.3.0.dist-info/METADATA,sha256=bJClE-D1H7REUTPvlKDLAuFuitaZNUHeeDtqV8733WE,1315
+cosmian_py_ggml-0.3.0.dist-info/LICENSE,sha256=Z0wEwlIqJt-ulg5-OWzUBniisSSS6B_bRz_PWVktGMQ,1064
+cosmian_py_ggml-0.3.0.dist-info/RECORD,,
+cosmian_py_ggml-0.3.0.dist-info/WHEEL,sha256=Pakn5EYkUcLl97jUMw4FC8DAw0ZnXzfAMJoDBnx1DlE,165
 cosmian_py_ggml/libggml-gptneox.so,sha256=napTu31o_22zS0n7BERtq5seurw1L3_ufMS_Doidvts,684448
-cosmian_py_ggml/gpt_neox.py,sha256=yY73qGYJ8i19I34hx6DmPfpnihnT2YbpJ6PZxt7WI_s,5334
+cosmian_py_ggml/gpt_neox.py,sha256=m_v5gVWWvY-IvCOI14o1aNscHKDPb8R7dSX0RuEQSsk,5358
 cosmian_py_ggml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
```

