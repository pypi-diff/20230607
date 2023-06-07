# Comparing `tmp/com.castsoftware.uc.python.common-1.0.6.tar.gz` & `tmp/com.castsoftware.uc.python.common-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.python.common-1.0.6.tar", last modified: Thu Jun  1 18:19:38 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.python.common-1.0.7.tar", last modified: Wed Jun  7 19:23:10 2023, max compression
```

## Comparing `com.castsoftware.uc.python.common-1.0.6.tar` & `com.castsoftware.uc.python.common-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 18:19:38.006461 com.castsoftware.uc.python.common-1.0.6/
--rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      714 2023-06-01 18:19:37.996746 com.castsoftware.uc.python.common-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 18:19:37.883353 com.castsoftware.uc.python.common-1.0.6/cast_common/
--rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/abstractClass.py
--rw-rw-rw-   0        0        0    12884 2023-06-01 16:17:16.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/aipRestCall.py
--rw-rw-rw-   0        0        0    10826 2023-05-25 20:32:57.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/highlight.py
--rw-rw-rw-   0        0        0     5478 2023-05-18 15:25:57.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/hlRestCall.py
--rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/logger.py
--rw-rw-rw-   0        0        0     5264 2023-05-21 20:59:32.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/restAPI.py
--rw-rw-rw-   0        0        0     6953 2023-06-01 18:18:30.000000 com.castsoftware.uc.python.common-1.0.6/cast_common/util.py
-drwxrwxrwx   0        0        0        0 2023-06-01 18:19:37.981840 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/
--rw-rw-rw-   0        0        0      714 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-01 18:19:37.000000 com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      643 2023-05-31 20:37:12.000000 com.castsoftware.uc.python.common-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 18:19:38.006461 com.castsoftware.uc.python.common-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 19:23:10.661091 com.castsoftware.uc.python.common-1.0.7/
+-rw-rw-rw-   0        0        0    35823 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      714 2023-06-07 19:23:10.644834 com.castsoftware.uc.python.common-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 19:23:10.530756 com.castsoftware.uc.python.common-1.0.7/cast_common/
+-rw-rw-rw-   0        0        0     2036 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/abstractClass.py
+-rw-rw-rw-   0        0        0    13723 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/aipRestCall.py
+-rw-rw-rw-   0        0        0    10826 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/highlight.py
+-rw-rw-rw-   0        0        0     5625 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/hlRestCall.py
+-rw-rw-rw-   0        0        0     1688 2023-05-18 15:18:26.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/logger.py
+-rw-rw-rw-   0        0        0     5264 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/restAPI.py
+-rw-rw-rw-   0        0        0     7054 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/cast_common/util.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:23:10.596930 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/
+-rw-rw-rw-   0        0        0      714 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 19:23:10.000000 com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      643 2023-06-07 19:16:42.000000 com.castsoftware.uc.python.common-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-07 19:23:10.661091 com.castsoftware.uc.python.common-1.0.7/setup.cfg
```

### Comparing `com.castsoftware.uc.python.common-1.0.6/LICENSE` & `com.castsoftware.uc.python.common-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.6/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.6
+Version: 1.0.7
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.6/cast_common/abstractClass.py` & `com.castsoftware.uc.python.common-1.0.7/cast_common/abstractClass.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.6/cast_common/aipRestCall.py` & `com.castsoftware.uc.python.common-1.0.7/cast_common/aipRestCall.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,34 @@
         if status == codes.ok and len(json) > 0:
             cat = json[0]['applicationResults'][0]['result']['categories']
             for index, name in enumerate(cat):
                 rslt.loc[name['key']]=[[name['name']],[name['value']]]
 
         return rslt
 
+    # def get_rules(self,domain_id,snapshot_id,business_criteria,critical=True,non_critical=True,start_row=1,max_rows=10000):
+    #     rslt_df =  DataFrame()
+    #     critical_arg=non_critical_arg=''
+
+    #     if critical:
+    #        critical_arg=f'cc:{business_criteria}' 
+    #     if non_critical:
+    #        non_critical_arg=f'nc:{business_criteria}' 
+
+    #     rule_arg=critical_arg
+    #     if len(rule_arg) > 0:
+    #         rule_arg = rule_arg + ','
+    #     rule_arg=f'{rule_arg}{non_critical_arg}'
+
+    #     url = f'{domain_id}/applications/3/snapshots/{snapshot_id}/violations?rule-pattern={rule_arg}&startRow={start_row}&nbRows={max_rows}'
+    #     (status,json) = self.get(url)
+    #     if status == codes.ok and len(json) > 0:
+    #         rslt_df = DataFrame(json)
+    #     return rslt_df
+
     def get_rules(self,domain_id,snapshot_id,business_criteria,critical=True,non_critical=True,start_row=1,max_rows=10000):
         rslt_df =  DataFrame()
         critical_arg=non_critical_arg=''
 
         if critical:
            critical_arg=f'cc:{business_criteria}' 
         if non_critical:
@@ -181,15 +201,14 @@
         url = f'{domain_id}/applications/3/snapshots/{snapshot_id}/violations?rule-pattern={rule_arg}&startRow={start_row}&nbRows={max_rows}'
         (status,json) = self.get(url)
         if status == codes.ok and len(json) > 0:
             rslt_df = json_normalize(json,meta=['component','diagnosis','remedialAction','rulePattern'])
             #rslt_df = DataFrame(json)
         return rslt_df
 
-
     def get_action_plan(self,domain_id,snapshot_id):
         business_criteria = ['Robustness','Efficiency','Security','Transferability','Changeability']
     
         catagory = ''
         tech_criteria = ''
         rslt_df =  DataFrame()
         ap_summary_df =  DataFrame()
```

### Comparing `com.castsoftware.uc.python.common-1.0.6/cast_common/highlight.py` & `com.castsoftware.uc.python.common-1.0.7/cast_common/highlight.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.6/cast_common/hlRestCall.py` & `com.castsoftware.uc.python.common-1.0.7/cast_common/hlRestCall.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,18 +116,23 @@
                     load_df_element(tp,lic_df,'version')
                     load_df_element(tp,lic_df,'languages')
                     load_df_element(tp,lic_df,'release')
                     load_df_element(tp,lic_df,'origin')
                     load_df_element(tp,lic_df,'lastVersion')
                     lic=concat([lic,lic_df],ignore_index=True)
 
-            if 'component' in cves.columns:
+            if not cves.empty and 'component' in cves.columns:
                 cves=cves[['component','version','languages','release','origin','lastVersion','cve', 'description', 'cweId', 'cweLabel', 'criticity', 'cpe']]
-            if 'component' in lic.columns:
+            else:
+                cves=None
+                
+            if not lic.empty and  'component' in lic.columns:
                 lic=lic[['component','version','languages','release','origin','lastVersion','license','compliance']] 
+            else:
+                lic=None
 
         return lic,cves,len(third_party)
     
     def create_an_app(self, url, instance_id, app_name):
         url = f'{url}/domains/{instance_id}/applications/'
         payload =[{"name": app_name,"domains": [{"id": instance_id}]}]
```

### Comparing `com.castsoftware.uc.python.common-1.0.6/cast_common/logger.py` & `com.castsoftware.uc.python.common-1.0.7/cast_common/logger.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.6/cast_common/restAPI.py` & `com.castsoftware.uc.python.common-1.0.7/cast_common/restAPI.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.python.common-1.0.6/cast_common/util.py` & `com.castsoftware.uc.python.common-1.0.7/cast_common/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pandas import DataFrame,json_normalize,concat,ExcelWriter
 from os import mkdir
 from os.path import exists,abspath,join
 from subprocess import Popen,PIPE,STDOUT
+from pandas.api.types import is_numeric_dtype
 import sys
 
 
 def get_between(txt,tag_start,tag_end,start_at=0):
     text = txt[start_at:]
     
     start = text[start_at:].find(f"{tag_start}")+len(f"{tag_start}")
@@ -173,48 +174,56 @@
         if output == True and len(line.strip(' ')) > 0:
             print(line)
         ret.append(line)
     stdout, stderr = process.communicate()
     return process.returncode,ret
     
 
-def format_table(writer, data, sheet_name,width=None):
+def format_table(writer, data, sheet_name,width=None,total_line=False):
     
-    data.to_excel(writer, index=False, sheet_name=sheet_name, startrow=1,header=False,float_format = "%0.2f")
+    data.to_excel(writer, index=False, sheet_name=sheet_name, startrow=1,header=False)
 
     workbook = writer.book
     worksheet = writer.sheets[sheet_name]
     rows = len(data)
     cols = len(data.columns)-1
+
     columns=[]
+    first=True
     for col_num, value in enumerate(data.columns.values):
-        columns.append({'header': value})
+        json = {'header': value}
+        if first:
+            first=False
+            if total_line:
+                json['total_string']='Totals'
+        else: 
+            if is_numeric_dtype(data[value]) and data[value].dtype != 'bool':
+                if total_line:
+                    json['total_function']='sum'
+
+        columns.append(json)
 
     table_options={
+                'total_row':total_line,
                 'columns':columns,
                 'header_row':True,
                 'autofilter':True,
                 'banded_rows':True
                 }
     worksheet.add_table(0, 0, rows, cols,table_options)
-    
-    header_format = workbook.add_format({'text_wrap':True,
-                                        'align': 'center'})
 
     col_width = 10
     if width == None:
         width = []
         for i in range(1,len(data.columns)+1):
            width.append(col_width)
-    for col_num, value in enumerate(data.columns.values):
-        worksheet.write(0, col_num, value, header_format)
-        w=width[col_num]
-        worksheet.set_column(col_num, col_num, w)
+
     return worksheet
 
+
 def convert_LOC(total:int):
     unit = ''
     if 1000 <= total <= 1000000:
         unit = 'KLoc'
         total = int(total/1000)
     elif total > 1000000:
         unit = 'MLoc'
```

### Comparing `com.castsoftware.uc.python.common-1.0.6/com.castsoftware.uc.python.common.egg-info/PKG-INFO` & `com.castsoftware.uc.python.common-1.0.7/com.castsoftware.uc.python.common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.python.common
-Version: 1.0.6
+Version: 1.0.7
 Summary: A set of common classes and methods for use with python projects
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.python.common
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.python.common/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10.6
```

### Comparing `com.castsoftware.uc.python.common-1.0.6/pyproject.toml` & `com.castsoftware.uc.python.common-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name='com.castsoftware.uc.python.common'
 description="A set of common classes and methods for use with python projects"
 
-version='1.0.6' #prod version
+version='1.0.7' #prod version
 
 dependencies = ['pandas','requests','XlsxWriter']
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
```

