# Comparing `tmp/sackeylib-0.0.8.tar.gz` & `tmp/sackeylib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sackeylib-0.0.8.tar", last modified: Wed Dec 29 12:51:12 2021, max compression
+gzip compressed data, was "dist\sackeylib-0.0.9.tar", last modified: Wed Dec 29 12:57:42 2021, max compression
```

## Comparing `sackeylib-0.0.8.tar` & `sackeylib-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2021-12-29 12:51:12.990064 sackeylib-0.0.8/
--rw-rw-rw-   0        0        0      244 2021-12-29 12:51:12.989066 sackeylib-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-12-29 12:51:12.977100 sackeylib-0.0.8/sackeylib/
--rw-rw-rw-   0        0        0        0 2021-12-07 08:37:01.000000 sackeylib-0.0.8/sackeylib/__init__.py
--rw-rw-rw-   0        0        0    10382 2021-12-29 12:49:04.000000 sackeylib-0.0.8/sackeylib/sackey_lib.py
-drwxrwxrwx   0        0        0        0 2021-12-29 12:51:12.987072 sackeylib-0.0.8/sackeylib.egg-info/
--rw-rw-rw-   0        0        0      244 2021-12-29 12:51:12.000000 sackeylib-0.0.8/sackeylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2021-12-29 12:51:12.000000 sackeylib-0.0.8/sackeylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-29 12:51:12.000000 sackeylib-0.0.8/sackeylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-12-22 14:36:29.000000 sackeylib-0.0.8/sackeylib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2021-12-29 12:51:12.000000 sackeylib-0.0.8/sackeylib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-29 12:51:12.990064 sackeylib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      287 2021-12-29 12:51:09.000000 sackeylib-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-12-29 12:57:42.106655 sackeylib-0.0.9/
+-rw-rw-rw-   0        0        0      244 2021-12-29 12:57:42.105657 sackeylib-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2021-12-29 12:57:42.092693 sackeylib-0.0.9/sackeylib/
+-rw-rw-rw-   0        0        0        0 2021-12-07 08:37:01.000000 sackeylib-0.0.9/sackeylib/__init__.py
+-rw-rw-rw-   0        0        0    10447 2021-12-29 12:57:24.000000 sackeylib-0.0.9/sackeylib/sackey_lib.py
+drwxrwxrwx   0        0        0        0 2021-12-29 12:57:42.103664 sackeylib-0.0.9/sackeylib.egg-info/
+-rw-rw-rw-   0        0        0      244 2021-12-29 12:57:41.000000 sackeylib-0.0.9/sackeylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2021-12-29 12:57:41.000000 sackeylib-0.0.9/sackeylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-12-29 12:57:41.000000 sackeylib-0.0.9/sackeylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-12-22 14:36:29.000000 sackeylib-0.0.9/sackeylib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2021-12-29 12:57:41.000000 sackeylib-0.0.9/sackeylib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2021-12-29 12:57:42.106655 sackeylib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      287 2021-12-29 12:57:39.000000 sackeylib-0.0.9/setup.py
```

### Comparing `sackeylib-0.0.8/sackeylib/sackey_lib.py` & `sackeylib-0.0.9/sackeylib/sackey_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
 
 def print_var(var,i=0):
     """
     打印一个变量
     """
     print("**" * 20 + str(i))
+    print('打印变量:',var_name(var))
     print(var.__str__)
     print(var)
     print(type(var))
     print("###" * 20)
 
 def print_error(tips=""):
     tips += "输入有误，请重新输入:"
@@ -342,9 +343,10 @@
         except Exception as es:
             print(es.__str__())
             print_function(item)
 
 
 
 if __name__ == "__main__":
-    print_msg()
+    a = {"12":12312}
+    print_var(a)
```

