# Comparing `tmp/pm-td-ameritrade-api-0.1.2.tar.gz` & `tmp/pm-td-ameritrade-api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm-td-ameritrade-api-0.1.2.tar", last modified: Wed Jun  7 20:23:32 2023, max compression
+gzip compressed data, was "pm-td-ameritrade-api-0.1.3.tar", last modified: Wed Jun  7 20:29:41 2023, max compression
```

## Comparing `pm-td-ameritrade-api-0.1.2.tar` & `pm-td-ameritrade-api-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:23:32.092008 pm-td-ameritrade-api-0.1.2/
--rw-rw-rw-   0        0        0     3851 2023-06-07 15:32:53.000000 pm-td-ameritrade-api-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     9601 2023-06-07 20:23:32.092008 pm-td-ameritrade-api-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8915 2023-06-07 20:00:57.000000 pm-td-ameritrade-api-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 20:23:32.079362 pm-td-ameritrade-api-0.1.2/pm_td_ameritrade_api.egg-info/
--rw-rw-rw-   0        0        0     9601 2023-06-07 20:23:32.000000 pm-td-ameritrade-api-0.1.2/pm_td_ameritrade_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-07 20:23:32.000000 pm-td-ameritrade-api-0.1.2/pm_td_ameritrade_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:23:32.000000 pm-td-ameritrade-api-0.1.2/pm_td_ameritrade_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-06-07 20:23:32.000000 pm-td-ameritrade-api-0.1.2/pm_td_ameritrade_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:23:32.000000 pm-td-ameritrade-api-0.1.2/pm_td_ameritrade_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 20:23:32.092008 pm-td-ameritrade-api-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1355 2023-06-07 20:13:08.000000 pm-td-ameritrade-api-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 20:29:41.036464 pm-td-ameritrade-api-0.1.3/
+-rw-rw-rw-   0        0        0     3851 2023-06-07 15:32:53.000000 pm-td-ameritrade-api-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     9601 2023-06-07 20:29:41.036464 pm-td-ameritrade-api-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8915 2023-06-07 20:00:57.000000 pm-td-ameritrade-api-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 20:29:41.024459 pm-td-ameritrade-api-0.1.3/pm_td_ameritrade_api.egg-info/
+-rw-rw-rw-   0        0        0     9601 2023-06-07 20:29:40.000000 pm-td-ameritrade-api-0.1.3/pm_td_ameritrade_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-07 20:29:40.000000 pm-td-ameritrade-api-0.1.3/pm_td_ameritrade_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:29:40.000000 pm-td-ameritrade-api-0.1.3/pm_td_ameritrade_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-06-07 20:29:40.000000 pm-td-ameritrade-api-0.1.3/pm_td_ameritrade_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 20:29:40.000000 pm-td-ameritrade-api-0.1.3/pm_td_ameritrade_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 20:29:41.036464 pm-td-ameritrade-api-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1355 2023-06-07 20:27:43.000000 pm-td-ameritrade-api-0.1.3/setup.py
```

### Comparing `pm-td-ameritrade-api-0.1.2/LICENSE` & `pm-td-ameritrade-api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pm-td-ameritrade-api-0.1.2/PKG-INFO` & `pm-td-ameritrade-api-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm-td-ameritrade-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python client lirbary for the TD Ameritrade API.
 Home-page: https://github.com/primalmachina/pm-td-ameritrade-api
 Author: Zach Fortier
 Author-email: primalmachinaz@gmail.com
 Keywords: finance,td ameritrade,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `pm-td-ameritrade-api-0.1.2/README.md` & `pm-td-ameritrade-api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pm-td-ameritrade-api-0.1.2/pm_td_ameritrade_api.egg-info/PKG-INFO` & `pm-td-ameritrade-api-0.1.3/pm_td_ameritrade_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm-td-ameritrade-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python client lirbary for the TD Ameritrade API.
 Home-page: https://github.com/primalmachina/pm-td-ameritrade-api
 Author: Zach Fortier
 Author-email: primalmachinaz@gmail.com
 Keywords: finance,td ameritrade,api
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Financial and Insurance Industry
```

### Comparing `pm-td-ameritrade-api-0.1.2/setup.py` & `pm-td-ameritrade-api-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(file="README.md", mode="r") as fh:
     long_description = fh.read()
 
 setup(
     name="pm-td-ameritrade-api",
     author="Zach Fortier",
     author_email="primalmachinaz@gmail.com",
-    version="0.1.2",
+    version="0.1.3",
     description="A python client lirbary for the TD Ameritrade API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/primalmachina/pm-td-ameritrade-api",
     install_requires=[
         "aiofiles>=0.7.0",
         "pydantic>=1.10.2",
```

