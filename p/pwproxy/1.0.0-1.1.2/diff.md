# Comparing `tmp/pwproxy-1.0.0.tar.gz` & `tmp/pwproxy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwproxy-1.0.0.tar", last modified: Sun May  7 03:22:58 2023, max compression
+gzip compressed data, was "pwproxy-1.1.2.tar", last modified: Wed Jun  7 15:28:00 2023, max compression
```

## Comparing `pwproxy-1.0.0.tar` & `pwproxy-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,10 @@
-drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.959820 pwproxy-1.0.0/
--rw-r--r--   0 gaochuang   (501) staff       (20)    11357 2023-05-07 03:21:17.000000 pwproxy-1.0.0/LICENSE
--rw-r--r--   0 gaochuang   (501) staff       (20)     1134 2023-05-07 03:22:58.959682 pwproxy-1.0.0/PKG-INFO
--rw-r--r--   0 gaochuang   (501) staff       (20)      895 2023-05-07 03:21:17.000000 pwproxy-1.0.0/README.md
--rw-r--r--   0 gaochuang   (501) staff       (20)      545 2023-05-07 03:21:17.000000 pwproxy-1.0.0/pyproject.toml
--rw-r--r--   0 gaochuang   (501) staff       (20)       38 2023-05-07 03:22:58.959859 pwproxy-1.0.0/setup.cfg
-drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.957527 pwproxy-1.0.0/src/
--rw-r--r--   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/__init__.py
-drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.958098 pwproxy-1.0.0/src/pwproxy/
--rw-r--r--   0 gaochuang   (501) staff       (20)      544 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/pwproxy/__init__.py
--rw-r--r--   0 gaochuang   (501) staff       (20)      990 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/pwproxy/function.py
--rw-r--r--   0 gaochuang   (501) staff       (20)     2106 2023-05-07 03:21:17.000000 pwproxy-1.0.0/src/pwproxy/run.py
-drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.958792 pwproxy-1.0.0/src/pwproxy.egg-info/
--rw-r--r--   0 gaochuang   (501) staff       (20)     1134 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/PKG-INFO
--rw-r--r--   0 gaochuang   (501) staff       (20)      364 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/SOURCES.txt
--rw-r--r--   0 gaochuang   (501) staff       (20)        1 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/dependency_links.txt
--rw-r--r--   0 gaochuang   (501) staff       (20)       24 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/requires.txt
--rw-r--r--   0 gaochuang   (501) staff       (20)        8 2023-05-07 03:22:58.000000 pwproxy-1.0.0/src/pwproxy.egg-info/top_level.txt
-drwxr-xr-x   0 gaochuang   (501) staff       (20)        0 2023-05-07 03:22:58.959458 pwproxy-1.0.0/test/
--rw-r--r--   0 gaochuang   (501) staff       (20)      352 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_1.py
--rw-r--r--   0 gaochuang   (501) staff       (20)      617 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_2.py
--rw-r--r--   0 gaochuang   (501) staff       (20)      326 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_3.py
--rw-r--r--   0 gaochuang   (501) staff       (20)      336 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_4.py
--rw-r--r--   0 gaochuang   (501) staff       (20)      447 2023-05-07 03:21:17.000000 pwproxy-1.0.0/test/test_5.py
+-rw-r--r--   0        0        0      895 2023-06-07 15:27:51.973580 pwproxy-1.1.2/README.md
+-rw-r--r--   0        0        0      623 2023-06-07 15:28:00.425601 pwproxy-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      675 2023-06-07 15:27:51.973580 pwproxy-1.1.2/src/pwproxy/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-07 15:27:51.973580 pwproxy-1.1.2/src/pwproxy/cli.py
+-rw-r--r--   0        0        0      990 2023-06-07 15:27:51.973580 pwproxy-1.1.2/src/pwproxy/function.py
+-rw-r--r--   0        0        0     1827 2023-06-07 15:27:51.973580 pwproxy-1.1.2/src/pwproxy/run.py
+-rw-r--r--   0        0        0      653 2023-06-07 15:27:51.973580 pwproxy-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0      326 2023-06-07 15:27:51.973580 pwproxy-1.1.2/tests/demo.py
+-rw-r--r--   0        0        0     1344 2023-06-07 15:27:51.973580 pwproxy-1.1.2/tests/test_run.py
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 pwproxy-1.1.2/PKG-INFO
```

### Comparing `pwproxy-1.0.0/PKG-INFO` & `pwproxy-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: pwproxy
-Version: 1.0.0
-Author-email: gc <895091550@qq.com>
-Keywords: playwright,mitmproxy,intercept request,modify response
+Version: 1.1.2
+Summary: Implement the core functions of mitmproxy based on playwright: request interception, response tampering
+Author-Email: gaochuang <895091550@qq.com>
+License: MIT
 Requires-Python: >=3.10
+Requires-Dist: playwright>=1.33.0
+Requires-Dist: pandas>=2.0.1
+Requires-Dist: click>=8.1.3
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # pwproxy
 
 <hr>
 
 > 基于playwright实现mitmproxy的核心功能:请求拦截,响应篡改<br>
```

### Comparing `pwproxy-1.0.0/README.md` & `pwproxy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pwproxy-1.0.0/src/pwproxy/function.py` & `pwproxy-1.1.2/src/pwproxy/function.py`

 * *Files identical despite different names*

