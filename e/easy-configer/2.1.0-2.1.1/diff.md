# Comparing `tmp/easy_configer-2.1.0.tar.gz` & `tmp/easy_configer-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_configer-2.1.0.tar", last modified: Tue Jun  6 09:32:55 2023, max compression
+gzip compressed data, was "easy_configer-2.1.1.tar", last modified: Wed Jun  7 06:10:23 2023, max compression
```

## Comparing `easy_configer-2.1.0.tar` & `easy_configer-2.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.953714 easy_configer-2.1.0/
--rw-rw-rw-   0        0        0    17635 2023-06-06 09:32:55.953714 easy_configer-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    13903 2023-04-21 05:47:34.000000 easy_configer-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.941154 easy_configer-2.1.0/easy_configer/
--rw-rw-rw-   0        0        0     1456 2023-04-21 05:47:25.000000 easy_configer-2.1.0/easy_configer/Argparser.py
--rw-rw-rw-   0        0        0     9359 2023-06-06 09:06:37.000000 easy_configer-2.1.0/easy_configer/Configer.py
--rw-rw-rw-   0        0        0     2023 2023-06-01 10:10:43.000000 easy_configer-2.1.0/easy_configer/IO_Converter.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.949722 easy_configer-2.1.0/easy_configer/utils/
--rw-rw-rw-   0        0        0      807 2023-04-21 05:47:25.000000 easy_configer-2.1.0/easy_configer/utils/Flag.py
--rw-rw-rw-   0        0        0     4189 2023-06-06 09:28:09.000000 easy_configer-2.1.0/easy_configer/utils/Type_Convertor.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.947165 easy_configer-2.1.0/easy_configer.egg-info/
--rw-rw-rw-   0        0        0    17635 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-06 09:32:55.000000 easy_configer-2.1.0/easy_configer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 09:32:55.954713 easy_configer-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1057 2023-06-06 09:32:08.000000 easy_configer-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:32:55.951721 easy_configer-2.1.0/test/
--rw-rw-rw-   0        0        0     3033 2023-04-21 05:47:25.000000 easy_configer-2.1.0/test/test_Configer.py
--rw-rw-rw-   0        0        0     1294 2023-04-21 05:47:25.000000 easy_configer-2.1.0/test/test_IO_Converter.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:10:23.088237 easy_configer-2.1.1/
+-rw-rw-rw-   0        0        0    17635 2023-06-07 06:10:23.088237 easy_configer-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13903 2023-06-07 00:47:17.000000 easy_configer-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:10:23.075271 easy_configer-2.1.1/easy_configer/
+-rw-rw-rw-   0        0        0     1456 2023-06-07 00:47:17.000000 easy_configer-2.1.1/easy_configer/Argparser.py
+-rw-rw-rw-   0        0        0     9359 2023-06-06 09:06:37.000000 easy_configer-2.1.1/easy_configer/Configer.py
+-rw-rw-rw-   0        0        0     2023 2023-06-07 00:47:17.000000 easy_configer-2.1.1/easy_configer/IO_Converter.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:10:23.083251 easy_configer-2.1.1/easy_configer/utils/
+-rw-rw-rw-   0        0        0      807 2023-06-07 00:47:17.000000 easy_configer-2.1.1/easy_configer/utils/Flag.py
+-rw-rw-rw-   0        0        0     4783 2023-06-07 06:07:37.000000 easy_configer-2.1.1/easy_configer/utils/Type_Convertor.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:10:23.080258 easy_configer-2.1.1/easy_configer.egg-info/
+-rw-rw-rw-   0        0        0    17635 2023-06-07 06:10:23.000000 easy_configer-2.1.1/easy_configer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-06-07 06:10:23.000000 easy_configer-2.1.1/easy_configer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:10:23.000000 easy_configer-2.1.1/easy_configer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-06-07 06:10:23.000000 easy_configer-2.1.1/easy_configer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:10:23.089234 easy_configer-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1057 2023-06-07 06:09:20.000000 easy_configer-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:10:23.086243 easy_configer-2.1.1/test/
+-rw-rw-rw-   0        0        0     3033 2023-04-21 05:47:25.000000 easy_configer-2.1.1/test/test_Configer.py
+-rw-rw-rw-   0        0        0     1294 2023-04-21 05:47:25.000000 easy_configer-2.1.1/test/test_IO_Converter.py
```

### Comparing `easy_configer-2.1.0/PKG-INFO` & `easy_configer-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_configer
-Version: 2.1.0
+Version: 2.1.1
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Description: # Project description
         #### easy_configer version : 2.0.1
```

### Comparing `easy_configer-2.1.0/README.md` & `easy_configer-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easy_configer-2.1.0/easy_configer/Argparser.py` & `easy_configer-2.1.1/easy_configer/Argparser.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.1.0/easy_configer/Configer.py` & `easy_configer-2.1.1/easy_configer/Configer.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.1.0/easy_configer/IO_Converter.py` & `easy_configer-2.1.1/easy_configer/IO_Converter.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.1.0/easy_configer/utils/Flag.py` & `easy_configer-2.1.1/easy_configer/utils/Flag.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.1.0/easy_configer/utils/Type_Convertor.py` & `easy_configer-2.1.1/easy_configer/utils/Type_Convertor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from functools import partial
 import ast
 import re
 
+import warnings
+def warning_on_one_line(message, category, filename, lineno, file=None, line=None):
+    return "{}:{}: {}: {}\n".format(filename, lineno, category.__name__, message)
+warnings.formatwarning = warning_on_one_line
+
+
 class Type_Convertor(object):
     '''
         As the name implies, this helper class of Configer will convert the raw string of config file
         into variable of the corresponding type.
         
         Now, i have update the security policy to prevent loading the harmful code to your system ~
         feel free to use the default type converter. 
@@ -49,33 +55,41 @@
         '''    
         # force to add split character at the end of parsed string
         cfg_raw_str = cfg_raw_str + self.__split_chr if (not self.__split_chr in cfg_raw_str) else cfg_raw_str
         try:
             val_str, typ = cfg_raw_str.split(self.__split_chr)
         except:
             raise RuntimeError
-            
+        
         if typ in self.__customized_cnvtor.keys():
-            return self.__customized_cnvtor[typ](val_str)
+            args = ast.literal_eval(val_str)
+            # For init customized class, we provide args, kwargs or default init  
+            if isinstance(args, dict):
+                return self.__customized_cnvtor[typ](**args)
+            elif isinstance(args, list):
+                return self.__customized_cnvtor[typ](*args)
+            else:  # invalid type of args is considered as default init  
+                warnings.warn(f"You're initialized class '{typ}' with default arguments!")
+                return self.__customized_cnvtor[typ]()
+        
         # support 'None' placeholder and [], {} eval, instead of define '@type'
         elif (val_str == 'None') or (not typ):  
             return ast.literal_eval(val_str)
+        
         # type-validator : we use ast.literal_eval and it need to \
         else:  # strip '[', ']', '{', '}' notation before feeding into 'default' type-conveter
             stripped_val_str = re.sub(r"[\[\]\{\}]", "", val_str)
         return self.__default_cnvtor[typ](stripped_val_str)
     
-    # HACK : new cnvt_func can not consider arguments as non-str type
-    #  so, currently we use {'key':val} str to map to the registered class!
     def regist_cnvtor(self, type_name:str = None, cnvt_func:callable = None):
         '''
             type_name :
                 Name of registered function, namely the name of customized class.
             
             cnvt_func :
                 The function for converting the string object into the customized class instance.
         '''
         assert callable(cnvt_func), "The converter function should be callable."
         assert isinstance(type_name, str) and len(type_name) > 0, "The cnvt_name should be given"
         
-        func_wrap = lambda dict_str : cnvt_func( **ast.literal_eval(dict_str) )
+        func_wrap = lambda *args, **kwargs : cnvt_func(*args, **kwargs)
         self.__customized_cnvtor[type_name] = func_wrap
```

### Comparing `easy_configer-2.1.0/easy_configer.egg-info/PKG-INFO` & `easy_configer-2.1.1/easy_configer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-configer
-Version: 2.1.0
+Version: 2.1.1
 Summary: An easy way for configurating python program by the given config file or config str
 Home-page: https://github.com/HuangChiEn/easy_config
 Author: JosefHuang
 Author-email: a3285556aa@gmail.com
 License: MIT
 Description: # Project description
         #### easy_configer version : 2.0.1
```

### Comparing `easy_configer-2.1.0/setup.py` & `easy_configer-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # read the contents of your README file
 this_directory = abspath(dirname(__file__))
 with open(join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='easy_configer',
-    version='2.1.0',
+    version='2.1.1',
     description='An easy way for configurating python program by the given config file or config str',
     author='JosefHuang',
     author_email='a3285556aa@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/HuangChiEn/easy_config',
```

### Comparing `easy_configer-2.1.0/test/test_Configer.py` & `easy_configer-2.1.1/test/test_Configer.py`

 * *Files identical despite different names*

### Comparing `easy_configer-2.1.0/test/test_IO_Converter.py` & `easy_configer-2.1.1/test/test_IO_Converter.py`

 * *Files identical despite different names*

