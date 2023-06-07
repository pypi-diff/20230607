# Comparing `tmp/dynatrace_opentelemetry_core-1.265.2-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_core-1.267.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 279401 bytes, number of entries: 108
+Zip file size: 279418 bytes, number of entries: 108
 -rw-r--r--  2.0 unx     1706 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/__init__.py
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/_version.py
 -rw-r--r--  2.0 unx     1449 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/any_pb2.py
 -rw-r--r--  2.0 unx     2857 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/api_pb2.py
 -rw-r--r--  2.0 unx    46761 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor.py
 -rw-r--r--  2.0 unx     6819 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor_database.py
 -rw-r--r--  2.0 unx   116074 b- defN 20-Feb-02 00:00 dynatrace/_vendor/google/protobuf/descriptor_pb2.py
@@ -89,22 +89,22 @@
 -rw-r--r--  2.0 unx    12007 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_propagator/tags.py
 -rw-r--r--  2.0 unx    14942 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_propagator/textmap.py
 -rw-r--r--  2.0 unx    10475 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_propagator/textmapcodec.py
 -rw-r--r--  2.0 unx     3310 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_sampler/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_transport/__init__.py
 -rw-r--r--  2.0 unx     6841 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_transport/connection.py
 -rw-r--r--  2.0 unx     1224 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_transport/exceptions.py
--rw-r--r--  2.0 unx    10803 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_transport/pooling.py
+-rw-r--r--  2.0 unx    10865 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_transport/pooling.py
 -rw-r--r--  2.0 unx     2026 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_transport/response.py
 -rw-r--r--  2.0 unx     1150 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_transport/timeout.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/__init__.py
 -rw-r--r--  2.0 unx     3559 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/byteops.py
 -rw-r--r--  2.0 unx     2035 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/context.py
 -rw-r--r--  2.0 unx     6002 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/exceptions.py
 -rw-r--r--  2.0 unx     3287 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/hashes.py
 -rw-r--r--  2.0 unx     3307 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/meta.py
 -rw-r--r--  2.0 unx     1626 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/tracing/_util/tenant.py
-?rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.265.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.265.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.265.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx    11610 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.265.2.dist-info/RECORD
-108 files, 1019510 bytes uncompressed, 260111 bytes compressed:  74.5%
+?rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.267.3.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.267.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.267.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx    11610 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_core-1.267.3.dist-info/RECORD
+108 files, 1019572 bytes uncompressed, 260128 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -306,20 +306,20 @@
 
 Filename: dynatrace/opentelemetry/tracing/_util/meta.py
 Comment: 
 
 Filename: dynatrace/opentelemetry/tracing/_util/tenant.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.265.2.dist-info/METADATA
+Filename: dynatrace_opentelemetry_core-1.267.3.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.265.2.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_core-1.267.3.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.265.2.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_core-1.267.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_core-1.265.2.dist-info/RECORD
+Filename: dynatrace_opentelemetry_core-1.267.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/tracing/version.py

```diff
@@ -1,7 +1,7 @@
-__version__ = "1.265.2"
+__version__ = "1.267.3"
 
-FULL_VERSION = "1.265.2.20230407-042323"
-BUILD_DATE = "2023.04.07 04:23:23"
-SCM_REVISION = "cb2041ed0224672f649d4efdc1b97ae8e4b6ad3f"
+FULL_VERSION = "1.267.3.20230606-141409"
+BUILD_DATE = "2023.06.06 14:14:09"
+SCM_REVISION = "f529b54267cabe461bec612ee18d9a4c14f09af7"
 IS_DEV_VERSION = False
 IS_PACKAGE_MODE = True
```

## dynatrace/opentelemetry/tracing/_transport/pooling.py

```diff
@@ -175,15 +175,17 @@
             BaseSSLError,
             exceptions.SSLError,
         ) as ex:
             if isinstance(ex, BaseSSLError):
                 raise exceptions.SSLError(ex)
             if isinstance(ex, (socket.error, http.client.HTTPException)):
                 excls = exceptions.ProtocolError
-                if isinstance(ex, http.client.RemoteDisconnected):
+                if isinstance(
+                    ex, (http.client.RemoteDisconnected, ConnectionResetError)
+                ):
                     excls = exceptions.RemoteDisconnected
                 raise excls("Connection aborted", ex)
             raise
         finally:
             if not clean_exit:
                 conn = conn and conn.close()
                 release_conn = True
```

## Comparing `dynatrace_opentelemetry_core-1.265.2.dist-info/METADATA` & `dynatrace_opentelemetry_core-1.267.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynatrace-opentelemetry-core
-Version: 1.265.2
+Version: 1.267.3
 Summary: Dynatrace OpenTelemetry core package
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `dynatrace_opentelemetry_core-1.265.2.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_core-1.267.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dynatrace_opentelemetry_core-1.265.2.dist-info/RECORD` & `dynatrace_opentelemetry_core-1.267.3.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 dynatrace/odin/proto/trace/v1/trace_pb2.py,sha256=6qFXDDS5U9_tshiqUjk0FTWHxMl9WOxcgE2yK6w10Aw,5585
 dynatrace/odin/semconv/_version.py,sha256=rvjjo5RBC86V0X6_1Q4um7329CS2s96rCFsLW9nfU7Q,39
 dynatrace/odin/semconv/v1/__init__.py,sha256=hWRbd7IEJZsM6Snn0kY4M10fb2IPwHY6DHjwDXJMpco,61795
 dynatrace/opentelemetry/tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/api.py,sha256=c7Rb1TkphWCUqKerxW5E310Smvj-VBqIfJsJlu5VEtk,1012
 dynatrace/opentelemetry/tracing/api.pyi,sha256=QkVFJRNMk2p5loY3VO5rCFHQxz8MacstxiWQzKY2DfY,1678
 dynatrace/opentelemetry/tracing/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dynatrace/opentelemetry/tracing/version.py,sha256=TcTUiM3basy7TJMvWF0uH3GW6fte-iY6rJDg-3aozyY,205
+dynatrace/opentelemetry/tracing/version.py,sha256=9qBz4EqG8q5NhA9RVNnfYnCV7NnFq9X4Qe_q-_7hD_Q,205
 dynatrace/opentelemetry/tracing/_config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_config/banner.py,sha256=HKXTTNkvvSy8j1Kwik_9kbjqve9RaivwNNSfbnn4H2U,3752
 dynatrace/opentelemetry/tracing/_config/configure.py,sha256=zC2p9ba7isZh-aOnfwd0Y9Fx5k2Njx0iagSzqt9ncgU,1780
 dynatrace/opentelemetry/tracing/_config/reader.py,sha256=52wMwG_9MbS97y0H4OeG4d7uWgBfyEfB6o4AkraVGKE,10949
 dynatrace/opentelemetry/tracing/_config/settings.py,sha256=SUiUyRfz5YJ0g3OBX51GAxjjprB5XPd3ISfzN1FUs68,18329
 dynatrace/opentelemetry/tracing/_export/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_export/exporter.py,sha256=PVj1EG2i_BUvyfcH_1KexngKSlP6qc3nz-_mnDtlH0Y,13769
@@ -88,21 +88,21 @@
 dynatrace/opentelemetry/tracing/_propagator/tags.py,sha256=g2aM7vS41mwGCw-2f49orrTwKDbfDfASojjivmjZMEE,12007
 dynatrace/opentelemetry/tracing/_propagator/textmap.py,sha256=UEpNLsxxfLAL7KplDTlpBfIrGTFaaKMM2zKg7dE3suQ,14942
 dynatrace/opentelemetry/tracing/_propagator/textmapcodec.py,sha256=SCmHmkazTnXllGwo62Hk3LUQ5rc-izWuATGJRI9jIkY,10475
 dynatrace/opentelemetry/tracing/_sampler/__init__.py,sha256=Zeu8s_Skzhly65rr6hKZ0PsQuii-ktLMuPyGgnPikog,3310
 dynatrace/opentelemetry/tracing/_transport/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_transport/connection.py,sha256=tSaXB4Fd_-cXBWnym5DeXA5ybHtgrE1dWfXUv41A3oQ,6841
 dynatrace/opentelemetry/tracing/_transport/exceptions.py,sha256=gmx9tKePRQWX0MtFzJsmsxiZ7Te4Ik-jxiBpx8SpIZM,1224
-dynatrace/opentelemetry/tracing/_transport/pooling.py,sha256=aFfKAAxw8q8beboqdvEQ_IvmLzUEOlM1Yw-zJafuS5o,10803
+dynatrace/opentelemetry/tracing/_transport/pooling.py,sha256=Z_JTH_sM9smn5vzEPp9CWE_QAo63VfRQ1j8IsBJBUvs,10865
 dynatrace/opentelemetry/tracing/_transport/response.py,sha256=zoBc57QTEOk5HSiKdovxQNncBHM93yoQR1qnp8dCwZk,2026
 dynatrace/opentelemetry/tracing/_transport/timeout.py,sha256=Xfdv8rAl-yGYQZYWK5aV1RA1q1HHJJKMAlii8jPKUVI,1150
 dynatrace/opentelemetry/tracing/_util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dynatrace/opentelemetry/tracing/_util/byteops.py,sha256=d9NPDsMmu338laXMgDjX4EIooSeEvgXkdneQLm9-Qhs,3559
 dynatrace/opentelemetry/tracing/_util/context.py,sha256=1QZpjw33kLAaSYT1CjlKuP-moRWGvCrC47O-ZtbTEYo,2035
 dynatrace/opentelemetry/tracing/_util/exceptions.py,sha256=XLYTvsqoNfhHeHheSFTizqQKaltYDqCuseGITDXz-aA,6002
 dynatrace/opentelemetry/tracing/_util/hashes.py,sha256=Ea7W7XVS1iOdp85qlaqK9ue3YLSJJvErkb4Ja646sqc,3287
 dynatrace/opentelemetry/tracing/_util/meta.py,sha256=BkkQp6X6JgkH6beoUJqSfNovZd3LAT8FGKo7s8mAjOA,3307
 dynatrace/opentelemetry/tracing/_util/tenant.py,sha256=tIuLrPLpD3rhcBzv3i7inj4LIP6mgeRWY72DLL_DKvU,1626
-dynatrace_opentelemetry_core-1.265.2.dist-info/METADATA,sha256=V9W1S3jXi4xSCYVwtLOkzAIhqrBe-wWxQhI_1PD3YwM,1153
-dynatrace_opentelemetry_core-1.265.2.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-dynatrace_opentelemetry_core-1.265.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
-dynatrace_opentelemetry_core-1.265.2.dist-info/RECORD,,
+dynatrace_opentelemetry_core-1.267.3.dist-info/METADATA,sha256=XzMCzotnNfm03xUzvvU4oMR40e9R_htUS-VE1FfW7WQ,1153
+dynatrace_opentelemetry_core-1.267.3.dist-info/WHEEL,sha256=KGYbc1zXlYddvwxnNty23BeaKzh7YuoSIvIMO4jEhvw,87
+dynatrace_opentelemetry_core-1.267.3.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
+dynatrace_opentelemetry_core-1.267.3.dist-info/RECORD,,
```

