# Comparing `tmp/cdspyreadme-1.5.tar.gz` & `tmp/cdspyreadme-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdspyreadme-1.5.tar", last modified: Fri Mar 17 17:04:14 2023, max compression
+gzip compressed data, was "cdspyreadme-1.5.1.tar", last modified: Wed Jun  7 09:08:00 2023, max compression
```

## Comparing `cdspyreadme-1.5.tar` & `cdspyreadme-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-03-17 17:04:14.686071 cdspyreadme-1.5/
--rw-r--r--   0 gilles.landais  (1382) gilles.landais  (1381)     1523 2021-02-25 08:29:36.000000 cdspyreadme-1.5/LICENSE.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     5133 2023-03-17 17:04:14.686071 cdspyreadme-1.5/PKG-INFO
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     4548 2022-03-21 17:27:54.000000 cdspyreadme-1.5/README.md
-drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-03-17 17:04:14.686071 cdspyreadme-1.5/cdspyreadme/
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)    18391 2021-06-11 07:12:14.000000 cdspyreadme-1.5/cdspyreadme/CDSColumn.py
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      213 2021-04-30 10:20:23.000000 cdspyreadme-1.5/cdspyreadme/MRT.template
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      993 2022-06-01 07:50:01.000000 cdspyreadme-1.5/cdspyreadme/ReadMe.template
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      234 2023-03-14 10:56:06.000000 cdspyreadme-1.5/cdspyreadme/__init__.py
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      339 2021-02-25 08:29:19.000000 cdspyreadme-1.5/cdspyreadme/bytebybyte.template
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)    31325 2023-03-14 10:56:06.000000 cdspyreadme-1.5/cdspyreadme/core.py
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     6940 2021-02-25 08:29:19.000000 cdspyreadme-1.5/cdspyreadme/core_test.py
-drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-03-17 17:04:14.686071 cdspyreadme-1.5/cdspyreadme.egg-info/
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     5133 2023-03-17 17:04:14.000000 cdspyreadme-1.5/cdspyreadme.egg-info/PKG-INFO
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      398 2023-03-17 17:04:14.000000 cdspyreadme-1.5/cdspyreadme.egg-info/SOURCES.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)        1 2023-03-17 17:04:14.000000 cdspyreadme-1.5/cdspyreadme.egg-info/dependency_links.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       27 2023-03-17 17:04:14.000000 cdspyreadme-1.5/cdspyreadme.egg-info/requires.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       12 2023-03-17 17:04:14.000000 cdspyreadme-1.5/cdspyreadme.egg-info/top_level.txt
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       67 2021-06-11 07:27:38.000000 cdspyreadme-1.5/pyproject.toml
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       38 2023-03-17 17:04:14.686071 cdspyreadme-1.5/setup.cfg
--rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     1091 2021-06-11 08:39:58.000000 cdspyreadme-1.5/setup.py
+drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/
+-rw-r--r--   0 gilles.landais  (1382) gilles.landais  (1381)     1523 2021-02-25 08:29:36.000000 cdspyreadme-1.5.1/LICENSE.txt
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     5135 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/PKG-INFO
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     4548 2022-03-21 17:27:54.000000 cdspyreadme-1.5.1/README.md
+drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/cdspyreadme/
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)    18391 2021-06-11 07:12:14.000000 cdspyreadme-1.5.1/cdspyreadme/CDSColumn.py
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      213 2021-04-30 10:20:23.000000 cdspyreadme-1.5.1/cdspyreadme/MRT.template
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      993 2022-06-01 07:50:01.000000 cdspyreadme-1.5.1/cdspyreadme/ReadMe.template
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      236 2023-06-07 08:59:15.000000 cdspyreadme-1.5.1/cdspyreadme/__init__.py
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      339 2021-02-25 08:29:19.000000 cdspyreadme-1.5.1/cdspyreadme/bytebybyte.template
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)    31325 2023-03-14 10:56:06.000000 cdspyreadme-1.5.1/cdspyreadme/core.py
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     6943 2023-06-07 08:57:54.000000 cdspyreadme-1.5.1/cdspyreadme/core_test.py
+drwxrwxr-x   0 gilles.landais  (1382) gilles.landais  (1381)        0 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/cdspyreadme.egg-info/
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     5135 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/PKG-INFO
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)      398 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/SOURCES.txt
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)        1 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/dependency_links.txt
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       27 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/requires.txt
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       12 2023-06-07 09:08:00.000000 cdspyreadme-1.5.1/cdspyreadme.egg-info/top_level.txt
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       67 2021-06-11 07:27:38.000000 cdspyreadme-1.5.1/pyproject.toml
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)       38 2023-06-07 09:08:00.784558 cdspyreadme-1.5.1/setup.cfg
+-rw-rw-r--   0 gilles.landais  (1382) gilles.landais  (1381)     1091 2021-06-11 08:39:58.000000 cdspyreadme-1.5.1/setup.py
```

### Comparing `cdspyreadme-1.5/LICENSE.txt` & `cdspyreadme-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5/PKG-INFO` & `cdspyreadme-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdspyreadme
-Version: 1.5
+Version: 1.5.1
 Summary: ReadMe generator package (cdspyreadme)
 Home-page: https://github.com/cds-astro/cds.pyreadme
 Author: Gilles Landais (CDS)
 License: UNKNOWN
 Keywords: astronomy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cdspyreadme-1.5/README.md` & `cdspyreadme-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5/cdspyreadme/CDSColumn.py` & `cdspyreadme-1.5.1/cdspyreadme/CDSColumn.py`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5/cdspyreadme/ReadMe.template` & `cdspyreadme-1.5.1/cdspyreadme/ReadMe.template`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5/cdspyreadme/core.py` & `cdspyreadme-1.5.1/cdspyreadme/core.py`

 * *Files identical despite different names*

### Comparing `cdspyreadme-1.5/cdspyreadme/core_test.py` & `cdspyreadme-1.5.1/cdspyreadme/core_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def __readme_file(suffix):
         return "ReadMe_{}".format(suffix)
 
     def test_numpy(self):
         """test numpy table"""
         tablemaker = CDSTablesMaker()
         ntab = np.array([(1.1, 1, 'test'), (2.2, 2, 'test2'), (3.3, 3, None), (None, -1, '')],
-                        dtype=[('mag', np.float), ('recno', np.int32), ('comment', np.str_, 10)])
+                        dtype=[('mag', np.float64), ('recno', np.int32), ('comment', np.str_, 10)])
         tablename = ReadMeCase.__result_file("numpy")
         tablemaker.addTable(ntab,
                             name=tablename,
                             description="test numpy table")
         tablemaker.writeCDSTables()
         self.assertTrue(self.__test_file(tablename, 3), "numpy file")
 
@@ -182,8 +182,8 @@
         col.description = "test"
         col.unit = "deg"
         print(tab)
         tablemaker.addTable(tab,
                             name=tablename,
                             description="test MRT generation")
         tablemaker.toMRT()
-        self.assertTrue(self.__test_file(tablename, 3), "MRT generation")
+        self.assertTrue(self.__test_file(tablename, 3), "MRT generation")
```

### Comparing `cdspyreadme-1.5/cdspyreadme.egg-info/PKG-INFO` & `cdspyreadme-1.5.1/cdspyreadme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdspyreadme
-Version: 1.5
+Version: 1.5.1
 Summary: ReadMe generator package (cdspyreadme)
 Home-page: https://github.com/cds-astro/cds.pyreadme
 Author: Gilles Landais (CDS)
 License: UNKNOWN
 Keywords: astronomy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cdspyreadme-1.5/setup.py` & `cdspyreadme-1.5.1/setup.py`

 * *Files identical despite different names*

