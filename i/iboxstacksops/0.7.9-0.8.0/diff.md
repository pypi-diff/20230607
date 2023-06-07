# Comparing `tmp/iboxstacksops-0.7.9.tar.gz` & `tmp/iboxstacksops-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iboxstacksops-0.7.9.tar", last modified: Fri May 19 17:18:19 2023, max compression
+gzip compressed data, was "iboxstacksops-0.8.0.tar", last modified: Wed Jun  7 11:25:09 2023, max compression
```

## Comparing `iboxstacksops-0.7.9.tar` & `iboxstacksops-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-19 17:18:19.184569 iboxstacksops-0.7.9/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-19 17:18:19.184569 iboxstacksops-0.7.9/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.7.9/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-19 17:18:19.172569 iboxstacksops-0.7.9/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-19 17:18:19.172569 iboxstacksops-0.7.9/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-19 17:18:19.176569 iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-05-19 17:18:18.000000 iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-05-19 17:18:18.000000 iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-05-19 17:18:18.000000 iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-05-19 17:18:18.000000 iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-05-19 17:18:18.000000 iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-19 17:18:19.184569 iboxstacksops-0.7.9/iboxstacksops/
--rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.7.9/iboxstacksops/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.7.9/iboxstacksops/actions.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.7.9/iboxstacksops/aws.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4096 2023-05-18 19:50:43.000000 iboxstacksops-0.7.9/iboxstacksops/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5507 2023-05-19 17:15:37.000000 iboxstacksops-0.7.9/iboxstacksops/changeset.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4204 2023-05-18 19:47:19.000000 iboxstacksops-0.7.9/iboxstacksops/commands.py
--rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.7.9/iboxstacksops/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.7.9/iboxstacksops/dashboard.py
--rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.7.9/iboxstacksops/events.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.7.9/iboxstacksops/i_region.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6390 2023-05-18 19:46:59.000000 iboxstacksops-0.7.9/iboxstacksops/i_stack.py
--rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.7.9/iboxstacksops/msg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1354 2023-05-18 19:52:27.000000 iboxstacksops-0.7.9/iboxstacksops/outputs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     8720 2023-05-18 19:52:16.000000 iboxstacksops-0.7.9/iboxstacksops/parameters.py
--rw-r--r--   0 mello     (1000) mello     (1000)    17319 2023-05-11 13:23:25.000000 iboxstacksops-0.7.9/iboxstacksops/parser.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.7.9/iboxstacksops/replica.py
--rw-r--r--   0 mello     (1000) mello     (1000)    10010 2023-04-27 12:45:52.000000 iboxstacksops-0.7.9/iboxstacksops/resolve.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.7.9/iboxstacksops/resources.py
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.7.9/iboxstacksops/route53.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.7.9/iboxstacksops/ssm.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.7.9/iboxstacksops/stacks.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1090 2023-03-28 16:37:37.000000 iboxstacksops-0.7.9/iboxstacksops/table.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.7.9/iboxstacksops/tags.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.7.9/iboxstacksops/template.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.7.9/iboxstacksops/tools.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-05-19 17:18:19.184569 iboxstacksops-0.7.9/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.7.9/scripts/ibox_stacksops.py
--rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-05-19 17:18:19.184569 iboxstacksops-0.7.9/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-05-19 17:17:49.000000 iboxstacksops-0.7.9/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      286 2021-04-21 12:16:09.000000 iboxstacksops-0.8.0/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.936640 iboxstacksops-0.8.0/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.936640 iboxstacksops-0.8.0/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.944640 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      909 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       55 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       14 2023-06-07 11:25:09.000000 iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/iboxstacksops/
+-rw-r--r--   0 mello     (1000) mello     (1000)       23 2021-09-05 11:44:37.000000 iboxstacksops-0.8.0/iboxstacksops/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8495 2023-03-29 09:24:36.000000 iboxstacksops-0.8.0/iboxstacksops/actions.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1847 2022-11-16 10:26:23.000000 iboxstacksops-0.8.0/iboxstacksops/aws.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4096 2023-05-18 19:50:43.000000 iboxstacksops-0.8.0/iboxstacksops/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5507 2023-05-19 17:15:37.000000 iboxstacksops-0.8.0/iboxstacksops/changeset.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4204 2023-05-18 19:47:19.000000 iboxstacksops-0.8.0/iboxstacksops/commands.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      808 2022-11-15 15:15:16.000000 iboxstacksops-0.8.0/iboxstacksops/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    36013 2023-03-13 12:56:53.000000 iboxstacksops-0.8.0/iboxstacksops/dashboard.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     4490 2022-12-15 09:44:09.000000 iboxstacksops-0.8.0/iboxstacksops/events.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2022-11-15 15:16:19.000000 iboxstacksops-0.8.0/iboxstacksops/i_region.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6390 2023-05-18 19:46:59.000000 iboxstacksops-0.8.0/iboxstacksops/i_stack.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      574 2022-11-16 13:40:57.000000 iboxstacksops-0.8.0/iboxstacksops/msg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1354 2023-05-18 19:52:27.000000 iboxstacksops-0.8.0/iboxstacksops/outputs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     8720 2023-05-18 19:52:16.000000 iboxstacksops-0.8.0/iboxstacksops/parameters.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    17398 2023-06-07 11:12:24.000000 iboxstacksops-0.8.0/iboxstacksops/parser.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-11-15 15:15:39.000000 iboxstacksops-0.8.0/iboxstacksops/replica.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    10015 2023-06-06 21:51:44.000000 iboxstacksops-0.8.0/iboxstacksops/resolve.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2732 2022-12-29 16:17:06.000000 iboxstacksops-0.8.0/iboxstacksops/resources.py
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5165 2021-10-28 09:48:25.000000 iboxstacksops-0.8.0/iboxstacksops/route53.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3177 2022-11-15 15:15:59.000000 iboxstacksops-0.8.0/iboxstacksops/ssm.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3267 2023-01-09 10:55:50.000000 iboxstacksops-0.8.0/iboxstacksops/stacks.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1563 2023-06-07 11:11:32.000000 iboxstacksops-0.8.0/iboxstacksops/table.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2836 2023-04-27 16:30:50.000000 iboxstacksops-0.8.0/iboxstacksops/tags.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2569 2022-11-15 15:16:25.000000 iboxstacksops-0.8.0/iboxstacksops/template.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3210 2023-03-29 07:47:33.000000 iboxstacksops-0.8.0/iboxstacksops/tools.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)      501 2022-11-16 09:52:19.000000 iboxstacksops-0.8.0/scripts/ibox_stacksops.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       61 2023-06-07 11:25:09.956641 iboxstacksops-0.8.0/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      971 2023-06-07 11:22:43.000000 iboxstacksops-0.8.0/setup.py
```

### Comparing `iboxstacksops-0.7.9/PKG-INFO` & `iboxstacksops-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.9
+Version: 0.8.0
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/PKG-INFO` & `iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iboxstacksops
-Version: 0.7.9
+Version: 0.8.0
 Summary: AWS Infrastructure in a Box - Stacks management program
 Home-page: https://github.com/mello7tre/AwsIBoxStackOps
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBoxStackOps
         Aws Infrastucture in a Box - Stacks management program.
```

### Comparing `iboxstacksops-0.7.9/build/lib/iboxstacksops.egg-info/SOURCES.txt` & `iboxstacksops-0.8.0/build/lib/iboxstacksops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/actions.py` & `iboxstacksops-0.8.0/iboxstacksops/actions.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/aws.py` & `iboxstacksops-0.8.0/iboxstacksops/aws.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/cfg.py` & `iboxstacksops-0.8.0/iboxstacksops/cfg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/changeset.py` & `iboxstacksops-0.8.0/iboxstacksops/changeset.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/commands.py` & `iboxstacksops-0.8.0/iboxstacksops/commands.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/common.py` & `iboxstacksops-0.8.0/iboxstacksops/common.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/dashboard.py` & `iboxstacksops-0.8.0/iboxstacksops/dashboard.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/events.py` & `iboxstacksops-0.8.0/iboxstacksops/events.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/i_region.py` & `iboxstacksops-0.8.0/iboxstacksops/i_region.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/i_stack.py` & `iboxstacksops-0.8.0/iboxstacksops/i_stack.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/msg.py` & `iboxstacksops-0.8.0/iboxstacksops/msg.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/outputs.py` & `iboxstacksops-0.8.0/iboxstacksops/outputs.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/parameters.py` & `iboxstacksops-0.8.0/iboxstacksops/parameters.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/parser.py` & `iboxstacksops-0.8.0/iboxstacksops/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     )
 
 
 def get_show_parser(subparser, parents=[]):
     parser = subparser.add_parser("show", parents=parents, help="Show Stacks table")
 
     parser.add_argument(
-        "-F", "--fields", nargs="+", type=str, default=cfg.SHOW_TABLE_FIELDS
+        "-F", "--fields", nargs="+", type=str, default=cfg.SHOW_TABLE_FIELDS,
+        help="Can use syntax 'Name=DisplayName' to use custom table heading",
     )
     parser.add_argument(
         "-O", "--output", type=str, default="text", choices=["text", "html", "bare"]
     )
 
     return parser
```

### Comparing `iboxstacksops-0.7.9/iboxstacksops/replica.py` & `iboxstacksops-0.8.0/iboxstacksops/replica.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/resolve.py` & `iboxstacksops-0.8.0/iboxstacksops/resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 if not _awsnovalue(r_value):
                     r_root.append(r_value)
 
             return r_root
 
         elif isinstance(value, (int, str, float)):
 
-            return value
+            return str(value)
 
     def _resolve_sub(name, value):
         if isinstance(value, list):
             sub_string = value[0]
             sub_data = value[1]
         else:
             sub_string = value
```

### Comparing `iboxstacksops-0.7.9/iboxstacksops/resources.py` & `iboxstacksops-0.8.0/iboxstacksops/resources.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/route53.py` & `iboxstacksops-0.8.0/iboxstacksops/route53.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/ssm.py` & `iboxstacksops-0.8.0/iboxstacksops/ssm.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/stacks.py` & `iboxstacksops-0.8.0/iboxstacksops/stacks.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/tags.py` & `iboxstacksops-0.8.0/iboxstacksops/tags.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/template.py` & `iboxstacksops-0.8.0/iboxstacksops/template.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/iboxstacksops/tools.py` & `iboxstacksops-0.8.0/iboxstacksops/tools.py`

 * *Files identical despite different names*

### Comparing `iboxstacksops-0.7.9/setup.py` & `iboxstacksops-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="iboxstacksops",
-    version="0.7.9",
+    version="0.8.0",
     author="Mello",
     author_email="mello+python@ankot.org",
     description="AWS Infrastructure in a Box - Stacks management program",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mello7tre/AwsIBoxStackOps",
     packages=["iboxstacksops",],
```

