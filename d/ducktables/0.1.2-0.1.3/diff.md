# Comparing `tmp/ducktables-0.1.2.tar.gz` & `tmp/ducktables-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ducktables-0.1.2.tar", last modified: Fri May 26 22:17:44 2023, max compression
+gzip compressed data, was "ducktables-0.1.3.tar", last modified: Wed Jun  7 20:25:06 2023, max compression
```

## Comparing `ducktables-0.1.2.tar` & `ducktables-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/
--rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-26 22:17:44.984170 ducktables-0.1.2/PKG-INFO
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/ducktables/
--rw-rw-r--   0 mark      (4000) mark      (4000)        3 2023-05-26 22:15:50.000000 ducktables-0.1.2/ducktables/__init__.py
--rw-rw-r--   0 mark      (4000) mark      (4000)     3922 2023-05-19 16:52:49.000000 ducktables-0.1.2/ducktables/aws.py
--rw-rw-r--   0 mark      (4000) mark      (4000)      358 2023-05-23 17:02:10.000000 ducktables-0.1.2/ducktables/github.py
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/ducktables/google/
--rw-rw-r--   0 mark      (4000) mark      (4000)     3918 2023-05-19 19:34:59.000000 ducktables-0.1.2/ducktables/google/__init__.py
--rw-rw-r--   0 mark      (4000) mark      (4000)     3479 2023-05-19 19:34:59.000000 ducktables-0.1.2/ducktables/google/analytics.py
--rw-rw-r--   0 mark      (4000) mark      (4000)     1039 2023-05-19 16:52:49.000000 ducktables-0.1.2/ducktables/openai.py
-drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-05-26 22:17:44.984170 ducktables-0.1.2/ducktables.egg-info/
--rw-rw-r--   0 mark      (4000) mark      (4000)      210 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (4000) mark      (4000)      321 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)      267 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/requires.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)       11 2023-05-26 22:17:44.000000 ducktables-0.1.2/ducktables.egg-info/top_level.txt
--rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-05-26 22:17:44.984170 ducktables-0.1.2/setup.cfg
--rw-rw-r--   0 mark      (4000) mark      (4000)      252 2023-05-26 22:16:08.000000 ducktables-0.1.2/setup.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.162996 ducktables-0.1.3/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     7625 2023-06-07 20:25:06.158996 ducktables-0.1.3/PKG-INFO
+-rw-rw-r--   0 mark      (4000) mark      (4000)     6364 2023-06-07 20:22:38.000000 ducktables-0.1.3/README.md
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.158996 ducktables-0.1.3/ducktables/
+-rw-rw-r--   0 mark      (4000) mark      (4000)        3 2023-05-26 22:15:50.000000 ducktables-0.1.3/ducktables/__init__.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3915 2023-06-07 20:22:38.000000 ducktables-0.1.3/ducktables/aws.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)      358 2023-05-23 17:02:10.000000 ducktables-0.1.3/ducktables/github.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.158996 ducktables-0.1.3/ducktables/google/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3917 2023-06-07 20:22:38.000000 ducktables-0.1.3/ducktables/google/__init__.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     3479 2023-05-19 19:34:59.000000 ducktables-0.1.3/ducktables/google/analytics.py
+-rw-rw-r--   0 mark      (4000) mark      (4000)     1044 2023-06-07 20:22:38.000000 ducktables-0.1.3/ducktables/openai.py
+drwxrwxr-x   0 mark      (4000) mark      (4000)        0 2023-06-07 20:25:06.158996 ducktables-0.1.3/ducktables.egg-info/
+-rw-rw-r--   0 mark      (4000) mark      (4000)     7625 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (4000) mark      (4000)      331 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)        1 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)      267 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/requires.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)       11 2023-06-07 20:25:06.000000 ducktables-0.1.3/ducktables.egg-info/top_level.txt
+-rw-rw-r--   0 mark      (4000) mark      (4000)       38 2023-06-07 20:25:06.162996 ducktables-0.1.3/setup.cfg
+-rw-rw-r--   0 mark      (4000) mark      (4000)      543 2023-06-07 20:24:40.000000 ducktables-0.1.3/setup.py
```

### Comparing `ducktables-0.1.2/ducktables/aws.py` & `ducktables-0.1.3/ducktables/aws.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 
 import boto3
 
 
 def ec2_instances():
     """
     SQL Usage:
-    SELECT * FROM python_table('aws', 'ec2_instances',
-      {
+    SELECT * FROM pytable('aws:ec2_instances',
+      columns = {
         'instance_id': 'VARCHAR',
         'name': 'VARCHAR',
         'instance_type': 'VARCHAR',
         'state': 'VARCHAR',
         'key_pair': 'VARCHAR',
         'platform': 'VARCHAR',
         'architecture': 'VARCHAR',
         'vpc_id': 'VARCHAR',
         'subnet_id': 'VARCHAR',
         'public_dns': 'VARCHAR',
         'public_ip': 'VARCHAR',
         'private_dns': 'VARCHAR',
         'private_ip': 'VARCHAR'
-        }, []);
+        });
     """
     def response_to_rows(response):
         for resv in response['Reservations']:
             resv_id = resv['ReservationId']
             instances = resv['Instances']
             for i in instances:
                 instance_name = None
@@ -59,28 +59,28 @@
         token = response.get('NextToken')
         
         
 
 def s3_buckets():
     """
     SQL Usage:
-    SELECT * FROM python_table('aws', 's3_buckets', {'name': 'VARCHAR', 'creation_date': 'VARCHAR'}, []);
+    SELECT * FROM pytable('aws:s3_buckets', columns={'name': 'VARCHAR', 'creation_date': 'VARCHAR'});
     """
     client = boto3.client('s3')
     response = client.list_buckets()
     for bucket in response['Buckets']:
         yield (bucket['Name'], bucket['CreationDate'].strftime('%m/%d/%Y'))
     
 
 def s3_objects(bucket, prefix = None):
     """
     SQL Usage:
-    SELECT * FROM python_table('aws', 's3_objects',
-      { 'key': 'VARCHAR', 'last_modified': 'VARCHAR', 'size': 'INT', 'storage_class': 'VARCHAR'},
-      ['bucket-name', 'foo/bar/prefix']);
+    SELECT * FROM pytable('aws:s3_objects', 'bucket-name', 'foo/bar/prefix',
+      columns = { 'key': 'VARCHAR', 'last_modified': 'VARCHAR', 'size': 'INT', 'storage_class': 'VARCHAR'}
+    );
 
     Note that the final prefix argument is optional, and you don't need to specify it in
     your SQL query. To list all objects:
     SELECT * FROM python_table('aws', 's3_objects',
       { 'key': 'VARCHAR', 'last_modified': 'VARCHAR', 'size': 'INT', 'storage_class': 'VARCHAR'},
       ['bucket-name']);
     """
```

### Comparing `ducktables-0.1.2/ducktables/google/__init__.py` & `ducktables-0.1.3/ducktables/google/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return key_file_path
     
 
 def sheet(sheets_url_or_key, cell_range, key_file_path = None):
     """
     SQL Usage:
     SELECT *
-    FROM pytable('google_:sheet', '1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgvE2upms', 'Class Data!A2:F31',
+    FROM pytable('google:sheet', '1BxiMVs0XRA5nFMdKvBdBZjgmUUqptlbs74OgvE2upms', 'Class Data!A2:F31',
          columns = {
              'name': 'VARCHAR', 'gender': 'VARCHAR', 'class_level': 'VARCHAR',
              'state': 'VARCHAR', 'major': 'VARCHAR', 'extracurricular': 'VARCHAR'}
     );
     """
     key_file_path = _key_path(key_file_path)
```

### Comparing `ducktables-0.1.2/ducktables/google/analytics.py` & `ducktables-0.1.3/ducktables/google/analytics.py`

 * *Files identical despite different names*

### Comparing `ducktables-0.1.2/ducktables/openai.py` & `ducktables-0.1.3/ducktables/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 openai.organization = os.getenv("OPENAI_ORG_ID")
 openai.api_key = os.getenv("OPENAI_API_KEY")
 
 def prompt(input_phrase, num_responses = 5):
     """
     SQL Usage:
-    SELECT * FROM pytable('chatgpt', 'prompt',
-      {'index': 'INT','message': 'VARCHAR', 'message_role': 'VARCHAR', 'finish_reason': 'VARCHAR'},
-      ['Write a limerick poem about how much you love SQL', 2]);
+    SELECT * FROM pytable('chatgpt:prompt', 'Write a limerick poem about how much you love SQL', 2,
+      columns = {'index': 'INT','message': 'VARCHAR', 'message_role': 'VARCHAR', 'finish_reason': 'VARCHAR'},
+    );
     """
     completion = openai.ChatCompletion.create(
         model="gpt-3.5-turbo",
         # Complains when getting int like things so we explicitly cast
         n = int(num_responses),
         messages=[
             {"role": "user", "content": input_phrase}
```

