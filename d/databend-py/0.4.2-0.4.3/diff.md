# Comparing `tmp/databend_py-0.4.2-py3-none-any.whl.zip` & `tmp/databend_py-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 17796 bytes, number of entries: 18
--rw-r--r--  2.0 unx      227 b- defN 23-May-17 12:48 databend_py/__init__.py
--rw-r--r--  2.0 unx    12673 b- defN 23-May-17 12:48 databend_py/client.py
--rw-r--r--  2.0 unx     6927 b- defN 23-May-13 23:39 databend_py/connection.py
+Zip file size: 18837 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      158 b- defN 23-May-25 07:52 databend_py/__init__.py
+-rw-r--r--  2.0 unx     9756 b- defN 23-Jun-07 04:03 databend_py/client.py
+-rw-r--r--  2.0 unx     7348 b- defN 23-Jun-05 06:20 databend_py/connection.py
 -rw-r--r--  2.0 unx      909 b- defN 22-Nov-07 03:45 databend_py/context.py
 -rw-r--r--  2.0 unx      931 b- defN 23-Jan-12 08:08 databend_py/datetypes.py
 -rw-r--r--  2.0 unx      184 b- defN 22-Nov-16 02:52 databend_py/defines.py
--rw-r--r--  2.0 unx      884 b- defN 23-May-13 23:39 databend_py/errors.py
+-rw-r--r--  2.0 unx     1184 b- defN 23-May-22 07:09 databend_py/errors.py
 -rw-r--r--  2.0 unx      206 b- defN 22-Nov-07 03:45 databend_py/log.py
--rw-r--r--  2.0 unx     2117 b- defN 23-May-17 12:48 databend_py/result.py
+-rw-r--r--  2.0 unx     2291 b- defN 23-Jun-05 06:20 databend_py/result.py
 -rw-r--r--  2.0 unx     1133 b- defN 23-May-13 23:39 databend_py/retry.py
+-rw-r--r--  2.0 unx     4838 b- defN 23-Jun-07 04:03 databend_py/uploader.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-07 03:45 databend_py/util/__init__.py
 -rw-r--r--  2.0 unx     1452 b- defN 22-Nov-07 03:45 databend_py/util/escape.py
 -rw-r--r--  2.0 unx     2254 b- defN 22-Nov-12 09:37 databend_py/util/helper.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3531 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1437 b- defN 23-May-17 12:48 databend_py-0.4.2.dist-info/RECORD
-18 files, 46326 bytes uncompressed, 15454 bytes compressed:  66.6%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-07 04:15 databend_py-0.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3531 b- defN 23-Jun-07 04:15 databend_py-0.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 04:15 databend_py-0.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-07 04:15 databend_py-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1517 b- defN 23-Jun-07 04:15 databend_py-0.4.3.dist-info/RECORD
+19 files, 49153 bytes uncompressed, 16373 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -24,32 +24,35 @@
 
 Filename: databend_py/result.py
 Comment: 
 
 Filename: databend_py/retry.py
 Comment: 
 
+Filename: databend_py/uploader.py
+Comment: 
+
 Filename: databend_py/util/__init__.py
 Comment: 
 
 Filename: databend_py/util/escape.py
 Comment: 
 
 Filename: databend_py/util/helper.py
 Comment: 
 
-Filename: databend_py-0.4.2.dist-info/LICENSE
+Filename: databend_py-0.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: databend_py-0.4.2.dist-info/METADATA
+Filename: databend_py-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: databend_py-0.4.2.dist-info/WHEEL
+Filename: databend_py-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: databend_py-0.4.2.dist-info/top_level.txt
+Filename: databend_py-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: databend_py-0.4.2.dist-info/RECORD
+Filename: databend_py-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databend_py/__init__.py

```diff
@@ -1,8 +1,5 @@
 from .client import Client
 from .connection import Connection
 from .datetypes import DatabendDataType
 
-VERSION = (0, 4, 2)
-__version__ = '.'.join(str(x) for x in VERSION)
-
 __all__ = ['Client', 'Connection', 'DatabendDataType']
```

## databend_py/client.py

```diff
@@ -1,17 +1,13 @@
-import csv
 import json
-import os
 import re
-import requests
-import time
-import uuid
 from urllib.parse import urlparse, parse_qs, unquote
 
 from .connection import Connection
+from .uploader import DataUploader
 from .result import QueryResult
 from .util.escape import escape_params
 from .util.helper import asbool, Helper
 
 
 class Client(object):
     """
@@ -21,14 +17,15 @@
 
     def __init__(self, *args, **kwargs):
         self.settings = (kwargs.pop('settings', None) or {}).copy()
         self.connection = Connection(*args, **kwargs)
         self.query_result_cls = QueryResult
         self.helper = Helper
         self._debug = asbool(self.settings.get('debug', False))
+        self._uploader = DataUploader(self, self.settings, debug=self._debug, compress=self.settings.get('compress', False))
 
     def __enter__(self):
         return self
 
     def disconnect(self):
         self.disconnect_connection()
 
@@ -130,20 +127,16 @@
         if len(match.group().split(' ')) < 2:
             raise Exception("Not standard insert statement")
         table_name = match[1]
 
         batch_size = query.count(',') + 1
         if params is not None:
             tuple_ls = [tuple(params[i:i + batch_size]) for i in range(0, len(params), batch_size)]
-            filename = self._generate_csv(tuple_ls)
-            with open(filename, "rb") as f:
-                self._sync_csv_file_into_table(f, filename, table_name, "CSV")
             insert_rows = len(tuple_ls)
-            os.remove(filename)
-
+            self._uploader.upload_to_table(table_name, tuple_ls)
         return insert_rows
 
     def _process_ordinary_query(self, query, params=None, with_column_types=False,
                                 query_id=None):
         if params is not None:
             query = self._substitute_params(
                 query, params, self.connection.context
@@ -203,16 +196,20 @@
             elif name == 'secure':
                 kwargs[name] = asbool(value)
             elif name == 'copy_purge':
                 kwargs[name] = asbool(value)
                 settings[name] = asbool(value)
             elif name == 'debug':
                 settings[name] = asbool(value)
+            elif name == 'compress':
+                settings[name] = asbool(value)
             elif name in timeouts:
                 kwargs[name] = float(value)
+            elif name == 'persist_cookies':
+                kwargs[name] = asbool(value)
             else:
                 settings[name] = value  # settings={'copy_purge':False}
         secure = kwargs.get("secure", False)
         kwargs['secure'] = secure
 
         host = parsed_url.hostname
 
@@ -230,101 +227,26 @@
             kwargs['password'] = unquote(parsed_url.password)
 
         if settings:
             kwargs['settings'] = settings
 
         return cls(host, **kwargs)
 
-    def _generate_csv(self, bindings):
-        file_name = f'/tmp/{uuid.uuid4()}.csv'
-        with open(file_name, "w+") as csvfile:
-            spamwriter = csv.writer(csvfile, delimiter=',', quoting=csv.QUOTE_MINIMAL)
-            spamwriter.writerows(bindings)
-
-        return file_name
-
-    def stage_csv_file(self, file_descriptor, file_name):
-        stage_path = "@~/%s" % file_name
-        start_presign_time = time.time()
-        _, row = self.execute('presign upload %s' % stage_path)
-        if self._debug:
-            print("upload: presign file:%s duration:%ss" % (file_name, time.time() - start_presign_time))
-
-        presigned_url = row[0][2]
-        headers = json.loads(row[0][1])
-        start_upload_time = time.time()
-        try:
-            resp = requests.put(presigned_url, headers=headers, data=file_descriptor)
-            resp.raise_for_status()
-        finally:
-            if self._debug:
-                print("upload: put file:%s duration:%ss" % (file_name, time.time() - start_upload_time))
-        return stage_path
-
-    def _sync_csv_file_into_table(self, file_descriptor, file_name, table, file_type):
-        start = time.time()
-        stage_path = self.stage_csv_file(file_descriptor, file_name)
-        copy_options = self._generate_copy_options()
-        _, _ = self.execute(
-            f"COPY INTO {table} FROM {stage_path} FILE_FORMAT = (type = {file_type} RECORD_DELIMITER = '\r\n')\
-             PURGE = {copy_options['PURGE']} FORCE = {copy_options['FORCE']}\
-              SIZE_LIMIT={copy_options['SIZE_LIMIT']} ON_ERROR = {copy_options['ON_ERROR']}")
-        if self._debug:
-            print("upload: copy %s duration:%ss" % (file_name, int(time.time() - start)))
-
-    def upload(self, file_descriptor, file_name, table_name, file_type=None):
+    def insert(self, database_name, table_name, data):
         """
-        upload the file to database.table according to the file
-        filename: the filename
+        insert the data into database.table according to the file
+        database_name: the target database
         table_name: the table which write into
-        file_type: the file type, default CSV
+        data: the data which write into, it's a list of tuple
         """
-        if not file_type:
-            if len(file_name.split(".")) > 0:
-                file_type = file_name.split(".")[1].upper()
-            else:
-                file_type = "CSV"
-        self._sync_csv_file_into_table(file_descriptor, file_name, table_name, file_type)
+        # TODO: escape the database & table name
+        self._uploader.upload_to_table("%s.%s" % (database_name, table_name), data)
 
-    def upload_to_stage(self, file_descriptor, stage_path=None, file_name=None):
+    def upload_to_stage(self, stage_dir, file_name, data):
         """
         upload the file to user stage
-        :param stage_path: target stage path
-        :param file_descriptor: open file handler
-        :param file_name:
+        :param stage_dir: target stage directory
+        :param file_name: the target file name which placed into the stage_dir
+        :param data: the data value or file handler
         :return:
         """
-        if stage_path is None:
-            stage_path = "~"
-        if file_name is None:
-            file_name = f'{uuid.uuid4()}'
-        stage_path = f"@{stage_path}/{file_name}"
-        _, row = self.execute('presign upload %s' % stage_path)
-        presigned_url = row[0][2]
-        headers = json.loads(row[0][1])
-        resp = requests.put(presigned_url, headers=headers, data=file_descriptor)
-        resp.raise_for_status()
-        return stage_path
-
-    def _generate_copy_options(self):
-        # copy options docs: https://databend.rs/doc/sql-commands/dml/dml-copy-into-table#copyoptions
-        copy_options = {}
-        if "copy_purge" in self.settings:
-            copy_options["PURGE"] = self.settings["copy_purge"]
-        else:
-            copy_options["PURGE"] = False
-
-        if "force" in self.settings:
-            copy_options["FORCE"] = self.settings["force"]
-        else:
-            copy_options["FORCE"] = False
-
-        if "size_limit" in self.settings:
-            copy_options["SIZE_LIMIT"] = self.settings["size_limit"]
-        else:
-            copy_options["SIZE_LIMIT"] = 0
-        if "on_error" in self.settings:
-            copy_options["ON_ERROR"] = self.settings["on_error"]
-
-        else:
-            copy_options["ON_ERROR"] = "abort"
-        return copy_options
+        return self._uploader.upload_to_stage(stage_dir, file_name, data)
```

## databend_py/connection.py

```diff
@@ -2,19 +2,18 @@
 import os
 import base64
 import time
 from requests.auth import HTTPBasicAuth
 
 import environs
 import requests
-from mysql.connector.errors import Error
 from . import log
 from . import defines
 from .context import Context
-from databend_py.errors import WarehouseTimeoutException
+from databend_py.errors import WarehouseTimeoutException, UnexpectedException, ServerException
 from databend_py.retry import retry
 
 headers = {'Content-Type': 'application/json', 'Accept': 'application/json', 'X-DATABEND-ROUTE': 'warehouse'}
 
 
 class ServerInfo(object):
     def __init__(self, name, version_major, version_minor, version_patch,
@@ -49,50 +48,54 @@
 
 
 def get_error(response):
     if response['error'] is None:
         return None
 
     # Wrap errno into msg, for result check
-    return Error(msg=response['error']['message'],
-                 errno=response['error']['code'])
+    return ServerException(
+        response['error']['message'],
+        response['error']['code'])
 
 
 class Connection(object):
     # Databend http handler doc: https://databend.rs/doc/reference/api/rest
 
     # Call connect(**driver)
     # driver is a dict contains:
     # {
     #   'user': 'root',
     #   'host': '127.0.0.1',
     #   'port': 3307,
     #   'database': 'default'
     # }
     def __init__(self, host, port=None, user=defines.DEFAULT_USER, password=defines.DEFAULT_PASSWORD,
-                 database=defines.DEFAULT_DATABASE, secure=False, copy_purge=False, session_settings=None):
+                 database=defines.DEFAULT_DATABASE, secure=False, copy_purge=False, session_settings=None, persist_cookies=False):
         self.host = host
         self.port = port
         self.user = user
         self.password = password
         self.database = database
         self.secure = secure
         self.copy_purge = copy_purge
         self.session_max_idle_time = defines.DEFAULT_SESSION_IDLE_TIME
         self.client_session = session_settings
         self.additional_headers = dict()
         self.query_option = None
         self.context = Context()
+        self.requests_session = requests.Session()
         self.schema = 'http'
         if self.secure:
             self.schema = 'https'
         e = environs.Env()
         if os.getenv("ADDITIONAL_HEADERS") is not None:
             print(os.getenv("ADDITIONAL_HEADERS"))
             self.additional_headers = e.dict("ADDITIONAL_HEADERS")
+        self.persist_cookies = persist_cookies
+        self.cookies = None
 
     def default_session(self):
         return {"database": self.database}
 
     def make_headers(self):
         if "Authorization" not in self.additional_headers:
             return {
@@ -108,23 +111,27 @@
         return '{}:{}'.format(self.host, self.port)
 
     def disconnect(self):
         self.client_session = dict()
 
     @retry(times=5, exceptions=WarehouseTimeoutException)
     def do_query(self, url, query_sql):
-        response = requests.post(url,
+        response = self.requests_session.post(url,
                                  data=json.dumps(query_sql),
                                  headers=self.make_headers(),
                                  auth=HTTPBasicAuth(self.user, self.password),
                                  verify=True)
-        resp_dict = json.loads(response.content)
+        try:
+            resp_dict = json.loads(response.content)
+        except json.decoder.JSONDecodeError:
+            raise UnexpectedException("failed to parse response: %s" % response.content)
         if resp_dict and resp_dict.get('error') and "no endpoint" in resp_dict.get('error'):
             raise WarehouseTimeoutException
-
+        if self.persist_cookies:
+            self.cookies = response.cookies
         return resp_dict
 
     def query(self, statement):
         url = self.format_url()
         log.logger.debug(f"http sql: {statement}")
         query_sql = {'sql': statement, "string_fields": True}
         if self.client_session is not None and len(self.client_session) != 0:
@@ -153,15 +160,15 @@
         return f"{self.schema}://{self.host}:{self.port}/v1/query/"
 
     def reset_session(self):
         self.client_session = dict()
 
     def next_page(self, next_uri):
         url = "{}://{}:{}{}".format(self.schema, self.host, self.port, next_uri)
-        return requests.get(url=url, headers=self.make_headers())
+        return self.requests_session.get(url=url, headers=self.make_headers(), cookies=self.cookies)
 
     # return a list of response util empty next_uri
     def query_with_session(self, statement):
         response_list = list()
         response = self.query(statement)
         log.logger.debug(f"response content: {response}")
         response_list.append(response)
```

## databend_py/errors.py

```diff
@@ -13,18 +13,28 @@
 class ServerException(Error):
     def __init__(self, message, code=None):
         self.message = message
         self.code = code
         super(ServerException, self).__init__(message)
 
     def __str__(self):
-        return 'Code: {}\n{}'.format(self.code, self.message)
+        return 'Code: {} {}'.format(self.code, self.message)
 
 
 class WarehouseTimeoutException(Error):
     def __init__(self, message, code=None):
         self.message = message
         self.code = code
         super(WarehouseTimeoutException, self).__init__(message)
 
     def __str__(self):
-        return 'Provision warehouse timeout: \n{}'.format(self.message)
+        return 'Provision warehouse timeout: {}'.format(self.message)
+
+
+class UnexpectedException(Error):
+    def __init__(self, message):
+        self.message = message
+        super(UnexpectedException, self).__init__(message)
+
+    def __str__(self):
+        message = ' ' + self.message if self.message is not None else ''
+        return 'Unexpected: {}'.format(message)
```

## databend_py/result.py

```diff
@@ -16,36 +16,41 @@
         self.column_data_dict_list = []
         self.columns_with_types = []
         self.column_type_dic = {}
         self.type_convert = DatabendDataType.type_convert_fn
 
         super(QueryResult, self).__init__()
 
-    def store(self, raw_data: dict):
+    def store_data(self, raw_data: dict):
         fields = raw_data.get("schema")
         column_name_ls = []
         datas = raw_data.get("data")
         for field in fields:
-            inner_type = self.extract_type(field["type"])
-            column_type = (field['name'], inner_type)
-            self.column_type_dic[field['name']] = inner_type
             column_name_ls.append(field['name'])
-            self.columns_with_types.append(column_type)
 
         for data in datas:
             self.column_data_dict_list.append(dict(zip(column_name_ls, data)))
 
+    def store_columns(self, raw_data: dict):
+        fields = raw_data.get("schema")
+        for field in fields:
+            inner_type = self.extract_type(field["type"])
+            column_type = (field['name'], inner_type)
+            self.column_type_dic[field['name']] = inner_type
+            self.columns_with_types.append(column_type)
+
     def get_result(self):
         """
         :return: stored query result.
         """
         data = []
-        self.store(self.first_data)
+        self.store_data(self.first_data)
+        self.store_columns(self.first_data)
         for d in self.data_generator:
-            self.store(d)
+            self.store_data(d)
 
         for read_data in self.column_data_dict_list:
             tmp_list = []
             for c, d in read_data.items():
                 if d == 'NULL':
                     tmp_list.append(d)
                 else:
```

## Comparing `databend_py-0.4.2.dist-info/LICENSE` & `databend_py-0.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `databend_py-0.4.2.dist-info/METADATA` & `databend_py-0.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databend-py
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python driver with native interface for Databend
 Home-page: https://github.com/databendcloud/databend-py
 Author: Databend Cloud Team
 Author-email: hantmac@outlook.com
 License: Apache License
 Keywords: databend db database cloud analytics
 Classifier: Development Status :: 4 - Beta
```

## Comparing `databend_py-0.4.2.dist-info/RECORD` & `databend_py-0.4.3.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-databend_py/__init__.py,sha256=bgTD6P2OftE-qz5KI3x3q7KcZFKugu-Vp4fmxgTvtcM,227
-databend_py/client.py,sha256=mt7_9Z8F1dkuM_CwYjT37aoJsTWRFm-K2dhefZ-nmwI,12673
-databend_py/connection.py,sha256=90u06LUJS8216pWVqX2UcHAT24f7Dx_aOKlh_7fhPF4,6927
+databend_py/__init__.py,sha256=_v1TB3rTudKBJB9IKOLI5nKXsCqDZ4FCyNWEYoln1qs,158
+databend_py/client.py,sha256=WFh_qKraobzqqOTEI1BzPU2Yzqx7sCFhF7y7TMIlTk8,9756
+databend_py/connection.py,sha256=yGx9S7jm1mNnSMKsol34dQ0Sjg-HU8QcNWSW8Y9uXZI,7348
 databend_py/context.py,sha256=yPkJ_BN4LGODvKCOjNlDGqABwxAMQTQl7w1vIGRPBDg,909
 databend_py/datetypes.py,sha256=Yl5ZS_C5oPfyOcE2xTQNtxgPZnxnMKIc_lYSmEnFJdg,931
 databend_py/defines.py,sha256=eQOK22KSKfcBukcD4oHsmlgpXFms92ew0ORxWNnxxH0,184
-databend_py/errors.py,sha256=-4WBvTF0OvggCa9pJEWeU02BDX-IVDx6e5hGZWjH2GI,884
+databend_py/errors.py,sha256=asAU_I2YKnJbW10KFz3eHANLpwFOdpDYVshgeaE2lJI,1184
 databend_py/log.py,sha256=dMuMaWptI_nexWDZMtZaAnoEOluIfYWNdoR9OSAhgKM,206
-databend_py/result.py,sha256=Zx6f_bz7CS0HDOx-wpi5GY-HQwLRkenpobnw0bkzNqo,2117
+databend_py/result.py,sha256=wVSmABQhGqoeMh_mjY9CEfYxxVNCTwNjdivxT8-DRF4,2291
 databend_py/retry.py,sha256=c-kNYxqgnD30U23Xy-yHVeBp0wItsatkxql2O1rkWNE,1133
+databend_py/uploader.py,sha256=9Ms0W092Oz2poj1VtABl0YZk5YC-g-KbU-irwOchsrc,4838
 databend_py/util/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 databend_py/util/escape.py,sha256=DE7PaShERoOw285fkg3pu7T_oMU4_2dMkHbjXEqPcn4,1452
 databend_py/util/helper.py,sha256=0r1d3CeNtMLdTPN_v8yW-GjjpjHVneIJJKKGdTioOoE,2254
-databend_py-0.4.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-databend_py-0.4.2.dist-info/METADATA,sha256=fEZwHCIt0fwFaTwg6qKSvKdsXsG5R3jx2RkbkTY7rZM,3531
-databend_py-0.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-databend_py-0.4.2.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
-databend_py-0.4.2.dist-info/RECORD,,
+databend_py-0.4.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+databend_py-0.4.3.dist-info/METADATA,sha256=fwT8pF2bnPW3Go0tefDc2HI9OcmbCv7qitzKnGgBFgA,3531
+databend_py-0.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+databend_py-0.4.3.dist-info/top_level.txt,sha256=t0rUVwHfEpXcuMreSkL69rc5DWv6FmzB4AfEGcc4_7U,12
+databend_py-0.4.3.dist-info/RECORD,,
```

