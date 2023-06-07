# Comparing `tmp/dolibs-0.1.6.tar.gz` & `tmp/dolibs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibs-0.1.6.tar", last modified: Wed Jun  7 14:37:33 2023, max compression
+gzip compressed data, was "dolibs-0.1.7.tar", last modified: Wed Jun  7 14:46:26 2023, max compression
```

## Comparing `dolibs-0.1.6.tar` & `dolibs-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:37:33.736788 dolibs-0.1.6/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-07 14:37:33.736666 dolibs-0.1.6/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     1152 2023-05-03 10:26:07.000000 dolibs-0.1.6/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:37:33.735769 dolibs-0.1.6/dolibs/
--rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.6/dolibs/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4602 2023-06-07 14:34:54.000000 dolibs-0.1.6/dolibs/dewpoint.py
--rw-r--r--   0 leandro    (501) staff       (20)     4591 2023-05-03 09:47:15.000000 dolibs-0.1.6/dolibs/skintemp.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:37:33.736466 dolibs-0.1.6/dolibs.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-07 14:37:33.000000 dolibs-0.1.6/dolibs.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      224 2023-06-07 14:37:33.000000 dolibs-0.1.6/dolibs.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-07 14:37:33.000000 dolibs-0.1.6/dolibs.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       71 2023-06-07 14:37:33.000000 dolibs-0.1.6/dolibs.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)        7 2023-06-07 14:37:33.000000 dolibs-0.1.6/dolibs.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-07 14:37:33.736839 dolibs-0.1.6/setup.cfg
--rw-r--r--   0 leandro    (501) staff       (20)      599 2023-06-07 14:37:22.000000 dolibs-0.1.6/setup.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:46:26.781478 dolibs-0.1.7/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-07 14:46:26.781351 dolibs-0.1.7/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     1152 2023-05-03 10:26:07.000000 dolibs-0.1.7/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:46:26.780469 dolibs-0.1.7/dolibs/
+-rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.7/dolibs/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4596 2023-06-07 14:46:07.000000 dolibs-0.1.7/dolibs/dewpoint.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4591 2023-05-03 09:47:15.000000 dolibs-0.1.7/dolibs/skintemp.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-07 14:46:26.781168 dolibs-0.1.7/dolibs.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      224 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       71 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        7 2023-06-07 14:46:26.000000 dolibs-0.1.7/dolibs.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-07 14:46:26.781528 dolibs-0.1.7/setup.cfg
+-rw-r--r--   0 leandro    (501) staff       (20)      599 2023-06-07 14:46:23.000000 dolibs-0.1.7/setup.py
```

### Comparing `dolibs-0.1.6/README.md` & `dolibs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dolibs-0.1.6/dolibs/dewpoint.py` & `dolibs-0.1.7/dolibs/dewpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     print(connect_str)
     engine = db.create_engine(connect_str,future=True)
     connection = engine.connect()
     metadata = db.MetaData()
     try:
      
 
-        sql = db.text("delete from postgis.dp_temperature where id_acquisizione in (select id_acquisizione from postgis.acquisizioni inner join postgis.imgtypes using (id_imgtype) where imgtype = 'DEWPOINTTEMP' and dtime between '"+dtime_from+"'::timestamp and '"+dtime_to+"'::timestamp)")
+        sql = db.text("delete from postgis.dp_temperature where id_acquisizione in (select id_acquisizione from postgis.acquisizioni inner join postgis.imgtypes using (id_imgtype) where imgtype = 'DPTEMP' and dtime between '"+dtime_from+"'::timestamp and '"+dtime_to+"'::timestamp)")
 
         connection.execute(sql)
         
         connection.commit() 
 
         connection.close()
         return retval
```

### Comparing `dolibs-0.1.6/dolibs/skintemp.py` & `dolibs-0.1.7/dolibs/skintemp.py`

 * *Files identical despite different names*

### Comparing `dolibs-0.1.6/setup.py` & `dolibs-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='dolibs',
     packages=find_packages(include=['dolibs']),
-    version='0.1.6',
+    version='0.1.7',
     url='https://github.com/n3tmaster/ERA5_procedures',
     description='Library for importing ERA5 Copernicus data into Drought Observatory platform',
     author='Leandro Rocchi - CNR',
     author_email='leandro.rocchi@cnr.it',
     license='MIT',
     install_requires=['cdsapi','scipy','netcdf4','rioxarray','numpy','xarray','sqlalchemy','psycopg2-binary'],
     setup_requires=['pytest-runner'],
```

