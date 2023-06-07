# Comparing `tmp/progscheduler-2.3.2.tar.gz` & `tmp/progscheduler-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progscheduler-2.3.2.tar", last modified: Mon Apr  3 16:55:21 2023, max compression
+gzip compressed data, was "progscheduler-2.3.3.tar", last modified: Wed Jun  7 21:17:37 2023, max compression
```

## Comparing `progscheduler-2.3.2.tar` & `progscheduler-2.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:21.510499 progscheduler-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-03 16:55:08.000000 progscheduler-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-04-03 16:55:21.510499 progscheduler-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-04-03 16:55:08.000000 progscheduler-2.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:21.506499 progscheduler-2.3.2/progscheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:21.506499 progscheduler-2.3.2/progscheduler/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/settings/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/settings/generic_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/settings/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/settings/specific_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:21.506499 progscheduler-2.3.2/progscheduler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/utils/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:21.510499 progscheduler-2.3.2/progscheduler/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/version/progsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-03 16:55:08.000000 progscheduler-2.3.2/progscheduler/version/progsettings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:55:21.506499 progscheduler-2.3.2/progscheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-04-03 16:55:21.000000 progscheduler-2.3.2/progscheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-03 16:55:21.000000 progscheduler-2.3.2/progscheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:55:21.000000 progscheduler-2.3.2/progscheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-03 16:55:21.000000 progscheduler-2.3.2/progscheduler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-03 16:55:21.000000 progscheduler-2.3.2/progscheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 16:55:21.000000 progscheduler-2.3.2/progscheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 16:55:21.510499 progscheduler-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-03 16:55:08.000000 progscheduler-2.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-07 21:17:24.000000 progscheduler-2.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-07 21:17:37.588670 progscheduler-2.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-07 21:17:24.000000 progscheduler-2.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/generic_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/specific_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/version/progsettings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:17:37.588670 progscheduler-2.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-07 21:17:24.000000 progscheduler-2.3.3/setup.py
```

### Comparing `progscheduler-2.3.2/LICENSE` & `progscheduler-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/PKG-INFO` & `progscheduler-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progscheduler
-Version: 2.3.2
+Version: 2.3.3
 Summary: A simple automated task to schedule files to open in specific days of the week or every day at startup or at specific time of the day.
 Home-page: https://github.com/zaytiri/program-scheduler
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/program-scheduler
 Project-URL: Changelog, https://github.com/zaytiri/program-scheduler/blob/main/CHANGELOG.md
 Keywords: program,schedule,scheduler,startup,days,open,files,folders
 Classifier: Environment :: Console
```

### Comparing `progscheduler-2.3.2/README.md` & `progscheduler-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler/app.py` & `progscheduler-2.3.3/progscheduler/app.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler/scheduler.py` & `progscheduler-2.3.3/progscheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler/settings/commands.py` & `progscheduler-2.3.3/progscheduler/settings/commands.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler/settings/generic_arguments.py` & `progscheduler-2.3.3/progscheduler/settings/generic_arguments.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler/settings/manager.py` & `progscheduler-2.3.3/progscheduler/settings/manager.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler/settings/specific_arguments.py` & `progscheduler-2.3.3/progscheduler/settings/specific_arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     @staticmethod
     def __validate_dates(user_list, current_dates):
         for date in user_list:
             validate_date = Date(date=date, date_separator='/')
             try:
                 if validate_date.lesser_than_today():
-                    show('\'' + date + '\': is an old date. It will be ignored.', to_exit=True)
+                    show('\'' + date + '\': is an old date. Cannot be added.', to_exit=True)
                 current_dates.append(validate_date.converted_date)
             except ValueError:
                 throw('\'' + date + '\': date not valid.')
 
     def __validate_exclude_include_dates(self, file, user_arguments):
         include_dates = self.__get_dates_list(file, user_arguments, self.include.name)
         exclude_dates = self.__get_dates_list(file, user_arguments, self.exclude.name)
@@ -196,19 +196,20 @@
 
         if self.include.name not in user_arguments and self.exclude.name not in user_arguments:
             return dates
 
         if self.alias.name in user_arguments and user_arguments.alias in file:
             try:
                 file_list = file[user_arguments.alias][name]
+                reduced_file_list = []
                 for old_date in file_list:
                     validate_date = Date(date=old_date, date_separator='/')
-                    if validate_date.lesser_than_today():
-                        file_list.pop(file_list.index(old_date))
-                self.__validate_dates(file[user_arguments.alias][name], dates)
+                    if validate_date.greater_than_today():
+                        reduced_file_list.append(file_list.index(old_date))
+                self.__validate_dates(reduced_file_list, dates)
             except KeyError:
                 pass
 
         if name in user_arguments:
             args = convert_to_dict(user_arguments)
             self.__validate_dates(args[name], dates)
```

### Comparing `progscheduler-2.3.2/progscheduler/utils/date.py` & `progscheduler-2.3.3/progscheduler/utils/date.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler/utils/directory.py` & `progscheduler-2.3.3/progscheduler/utils/directory.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/progscheduler.egg-info/PKG-INFO` & `progscheduler-2.3.3/progscheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progscheduler
-Version: 2.3.2
+Version: 2.3.3
 Summary: A simple automated task to schedule files to open in specific days of the week or every day at startup or at specific time of the day.
 Home-page: https://github.com/zaytiri/program-scheduler
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/program-scheduler
 Project-URL: Changelog, https://github.com/zaytiri/program-scheduler/blob/main/CHANGELOG.md
 Keywords: program,schedule,scheduler,startup,days,open,files,folders
 Classifier: Environment :: Console
```

### Comparing `progscheduler-2.3.2/progscheduler.egg-info/SOURCES.txt` & `progscheduler-2.3.3/progscheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.2/setup.py` & `progscheduler-2.3.3/setup.py`

 * *Files identical despite different names*

