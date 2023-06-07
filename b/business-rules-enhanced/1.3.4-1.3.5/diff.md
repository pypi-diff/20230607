# Comparing `tmp/business-rules-enhanced-1.3.4.tar.gz` & `tmp/business-rules-enhanced-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "business-rules-enhanced-1.3.4.tar", last modified: Thu Apr 13 15:03:40 2023, max compression
+gzip compressed data, was "business-rules-enhanced-1.3.5.tar", last modified: Wed Jun  7 10:21:05 2023, max compression
```

## Comparing `business-rules-enhanced-1.3.4.tar` & `business-rules-enhanced-1.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/business_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    58425 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/six.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/business_rules/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-13 15:03:40.000000 business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 15:03:40.900611 business-rules-enhanced-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-13 15:03:12.000000 business-rules-enhanced-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58368 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/business_rules/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 10:21:05.000000 business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:21:05.688345 business-rules-enhanced-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 10:20:40.000000 business-rules-enhanced-1.3.5/setup.py
```

### Comparing `business-rules-enhanced-1.3.4/LICENSE` & `business-rules-enhanced-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.4/PKG-INFO` & `business-rules-enhanced-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.4
+Version: 1.3.5
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.4/README.md` & `business-rules-enhanced-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.4/business_rules/actions.py` & `business-rules-enhanced-1.3.5/business_rules/actions.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.4/business_rules/engine.py` & `business-rules-enhanced-1.3.5/business_rules/engine.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.4/business_rules/operators.py` & `business-rules-enhanced-1.3.5/business_rules/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas
 import sys
 
 from .six import string_types, integer_types
 
 from .fields import (FIELD_DATAFRAME, FIELD_TEXT, FIELD_NUMERIC, FIELD_NO_INPUT,
                      FIELD_SELECT, FIELD_SELECT_MULTIPLE)
-from .utils import fn_name_to_pretty_label, float_to_decimal, vectorized_is_valid, vectorized_compare_dates, \
+from .utils import flatten_list, fn_name_to_pretty_label, float_to_decimal, vectorized_is_valid, vectorized_compare_dates, \
     vectorized_is_complete_date, vectorized_len, vectorized_get_dict_key, vectorized_is_in, vectorized_case_insensitive_is_in, \
     vectorized_apply_regex, apply_regex
 from decimal import Decimal, Inexact, Context
 import operator
 import numpy as np
 import pandas as pd
 
@@ -854,20 +854,17 @@
         target = self.replace_prefix(other_value.get("target"))
         results = vectorized_is_complete_date(self.value[target])
         return pd.Series(results)
 
     @type_operator(FIELD_DATAFRAME)
     def is_unique_set(self, other_value):
         target = self.replace_prefix(other_value.get("target"))
-        value = other_value.get("comparator")
-        if isinstance(value, list):
-            value.append(target)
-            target_data = value
-        else:
-            target_data = [value, target]
+        comparator = other_value.get("comparator")
+        values = [target, comparator]
+        target_data = flatten_list(values)
         target_names = []
         for target_name in target_data:
             target_name = self.replace_prefix(target_name)
             if target_name in self.value.columns:
                 target_names.append(target_name)
         counts = self.value[target_names].groupby(target_names)[target].transform('size')
         results = np.where(counts <= 1, True, False)
```

### Comparing `business-rules-enhanced-1.3.4/business_rules/six.py` & `business-rules-enhanced-1.3.5/business_rules/six.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.4/business_rules/utils.py` & `business-rules-enhanced-1.3.5/business_rules/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,21 @@
 
 def apply_regex(regex: str, val: str):
     result = re.findall(regex, val)
     if result:
         return result[0]
     else:
         return None
+    
+def flatten_list(l):
+    for item in l:
+        if isinstance(item, list):
+            yield from flatten_list(item)
+        else:
+            yield item
 
 vectorized_apply_regex = np.vectorize(apply_regex)
 vectorized_is_complete_date = np.vectorize(is_complete_date)
 vectorized_compare_dates = np.vectorize(compare_dates)
 vectorized_is_valid = np.vectorize(is_valid_date)
 vectorized_get_dict_key = np.vectorize(get_dict_key_val)
 vectorized_is_in = np.vectorize(is_in)
```

### Comparing `business-rules-enhanced-1.3.4/business_rules/variables.py` & `business-rules-enhanced-1.3.5/business_rules/variables.py`

 * *Files identical despite different names*

### Comparing `business-rules-enhanced-1.3.4/business_rules_enhanced.egg-info/PKG-INFO` & `business-rules-enhanced-1.3.5/business_rules_enhanced.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: business-rules-enhanced
-Version: 1.3.4
+Version: 1.3.5
 Summary: Fork of Venmo-Business-Rules: Python DSL for setting up business intelligence rules that can be configured without code  History -------  1.0.1 +++++ released 2016-3-16  - Fixes a packaging bug preventing 1.0.0 from being installed on some platforms.  1.0.0 +++++ released 2016-3-16  - Removes caching layer on rule decorator 
 Home-page: https://github.com/cdisc-org/business-rules
 Author: cdisc-org
 Author-email: UNKNOWN
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `business-rules-enhanced-1.3.4/setup.py` & `business-rules-enhanced-1.3.5/setup.py`

 * *Files identical despite different names*

