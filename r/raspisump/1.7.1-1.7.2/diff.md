# Comparing `tmp/raspisump-1.7.1.tar.gz` & `tmp/raspisump-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.7.1.tar", last modified: Wed May 24 13:49:48 2023, max compression
+gzip compressed data, was "raspisump-1.7.2.tar", last modified: Wed Jun  7 16:46:07 2023, max compression
```

## Comparing `raspisump-1.7.1.tar` & `raspisump-1.7.2.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.629063 raspisump-1.7.1/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.7.1/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      251 2023-05-23 17:49:34.000000 raspisump-1.7.1/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3948 2023-05-24 13:49:48.625729 raspisump-1.7.1/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3174 2023-05-23 17:49:34.000000 raspisump-1.7.1/README.md
--rw-r--r--   0 al        (1000) users      (984)       24 2023-05-24 13:48:02.000000 raspisump-1.7.1/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/bin/
--rw-r--r--   0 al        (1000) users      (984)      362 2023-05-23 17:49:34.000000 raspisump-1.7.1/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      905 2023-05-23 17:49:34.000000 raspisump-1.7.1/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      670 2023-05-23 17:49:34.000000 raspisump-1.7.1/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      537 2023-05-23 17:49:34.000000 raspisump-1.7.1/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      703 2023-05-23 17:49:34.000000 raspisump-1.7.1/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/csv/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/web/css/raspi.css
--rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/web/css/raspi.css~
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.619063 raspisump-1.7.1/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/web/images/logo.png
--rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.7.1/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.622396 raspisump-1.7.1/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.7.1/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.7.1/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.622396 raspisump-1.7.1/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.7.1/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    10745 2023-05-23 17:49:34.000000 raspisump-1.7.1/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133806 2023-05-23 17:49:34.000000 raspisump-1.7.1/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.625729 raspisump-1.7.1/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.7.1/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     4950 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     2068 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     2002 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     4644 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)      872 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2745 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     2053 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1490 2023-05-23 17:49:34.000000 raspisump-1.7.1/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-24 13:49:48.625729 raspisump-1.7.1/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3948 2023-05-24 13:49:48.000000 raspisump-1.7.1/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      765 2023-05-24 13:49:48.000000 raspisump-1.7.1/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-05-24 13:49:48.000000 raspisump-1.7.1/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       13 2023-05-24 13:49:48.000000 raspisump-1.7.1/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-05-24 13:49:48.000000 raspisump-1.7.1/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-05-24 13:49:48.629063 raspisump-1.7.1/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2302 2023-05-24 13:48:02.000000 raspisump-1.7.1/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.920452 raspisump-1.7.2/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-06-02 22:51:18.000000 raspisump-1.7.2/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      251 2023-06-02 22:51:18.000000 raspisump-1.7.2/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3948 2023-06-07 16:46:07.920452 raspisump-1.7.2/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3174 2023-06-02 22:51:18.000000 raspisump-1.7.2/README.md
+-rw-r--r--   0 al        (1000) users      (984)       24 2023-06-07 16:45:05.000000 raspisump-1.7.2/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-06-02 22:51:18.000000 raspisump-1.7.2/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      962 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      638 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      538 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      705 2023-06-07 16:45:05.000000 raspisump-1.7.2/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.910452 raspisump-1.7.2/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/csv/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5687 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      614 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/css/raspi.css
+-rw-r--r--   0 al        (1000) users      (984)      690 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/css/raspi.css~
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/images/logo.png
+-rwxr-xr-x   0 al        (1000) users      (984)      906 2023-06-02 22:51:18.000000 raspisump-1.7.2/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.913786 raspisump-1.7.2/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2023-06-02 22:51:18.000000 raspisump-1.7.2/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2023-06-02 22:51:18.000000 raspisump-1.7.2/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.917119 raspisump-1.7.2/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2023-06-02 22:51:18.000000 raspisump-1.7.2/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    10745 2023-06-02 22:51:18.000000 raspisump-1.7.2/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133806 2023-06-02 22:51:18.000000 raspisump-1.7.2/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.917119 raspisump-1.7.2/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-02 22:51:18.000000 raspisump-1.7.2/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     4680 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     2068 2023-06-02 22:51:18.000000 raspisump-1.7.2/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     1965 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     4190 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      844 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2799 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     2045 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1414 2023-06-07 16:45:05.000000 raspisump-1.7.2/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.920452 raspisump-1.7.2/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3948 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      808 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-06-07 16:46:07.000000 raspisump-1.7.2/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-06-07 16:46:07.920452 raspisump-1.7.2/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2303 2023-06-07 16:45:05.000000 raspisump-1.7.2/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-06-07 16:46:07.920452 raspisump-1.7.2/tests/
+-rw-r--r--   0 al        (1000) users      (984)     1346 2023-06-07 16:45:05.000000 raspisump-1.7.2/tests/tests_logging.py
+-rw-r--r--   0 al        (1000) users      (984)     2342 2023-06-07 16:45:05.000000 raspisump-1.7.2/tests/tests_sump.py
```

### Comparing `raspisump-1.7.1/LICENSE` & `raspisump-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/PKG-INFO` & `raspisump-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.7.1
+Version: 1.7.2
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.7.1/README.md` & `raspisump-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/bin/rsump.py` & `raspisump-1.7.2/bin/rsump.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,25 @@
 import time
 import os
 import configparser
 from raspisump import reading, log
 
 config = configparser.RawConfigParser()
 user = os.getlogin()
-config.read('/home/' + user + '/raspi-sump/raspisump.conf')
-reading_interval = config.getint('pit', 'reading_interval')
+config.read("/home/" + user + "/raspi-sump/raspisump.conf")
+reading_interval = config.getint("pit", "reading_interval")
 
 if reading_interval == 0:
     try:
         reading.water_depth()
     except RuntimeError:
-        print("ERROR -- Cannot Access gpio pins.  Make sure user is part of the gpio group.")
-        log.log_event("error_log", "GPIO ERROR -- Cannot Access gpio pins.  Make sure user is part of the gpio group.")
+        print(
+            "ERROR -- Cannot Access gpio pins.  Make sure user is part of the gpio group."
+        )
+        log.log_event(
+            "error_log",
+            "GPIO ERROR -- Cannot Access gpio pins.  Make sure user is part of the gpio group.",
+        )
 else:
     while True:
         reading.water_depth()
         time.sleep(reading_interval)
```

### Comparing `raspisump-1.7.1/bin/rsumpchart.py` & `raspisump-1.7.2/bin/rsumpchart.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 
 import time
 import os
 from raspisump import todaychart
 
 user = os.getlogin()
 
+
 def main():
     """Initiate todaychart.py module to graph sump pit activity."""
-    csv_file = "/home/" + user + "/raspi-sump/csv/waterlevel-{}.csv".format(
-        time.strftime("%Y%m%d")
-    )
-    filename = "/home/" + user + "/raspi-sump/charts/today.png"
+    csv_file = f"/home/{user}/raspi-sump/csv/waterlevel-{time.strftime('%Y%m%d')}.csv"
+    filename = f"/home/{user}/raspi-sump/charts/today.png"
     todaychart.graph(csv_file, filename)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `raspisump-1.7.1/bin/rsumpmonitor.py` & `raspisump-1.7.2/bin/rsumpmonitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 from raspisump import checkpid
 
 
 def main():
-    '''run checkpid.py module to restart Raspi-Sump if the rsump.py process is
-    stopped or has spawned multiple processes.'''
-    process = '/usr/local/bin/rsump.py'
+    """run checkpid.py module to restart Raspi-Sump if the rsump.py process is
+    stopped or has spawned multiple processes."""
+    process = "/usr/local/bin/rsump.py"
     checkpid.check_pid(process)
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `raspisump-1.7.1/bin/rsumpwebchart.py` & `raspisump-1.7.2/bin/rsumpwebchart.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,19 +9,21 @@
 
 import time
 import os
 from raspisump import webchart
 
 user = os.getlogin()
 
+
 def main():
-    '''Pass variables to webchart.py'''
-    year = time.strftime('%Y')
-    month = time.strftime('%m')
-    today = time.strftime('%Y%m%d')
-    homedir = '/home/' + user + "/raspi-sump/"
+    """Pass variables to webchart.py"""
+    year = time.strftime("%Y")
+    month = time.strftime("%m")
+    today = time.strftime("%Y%m%d")
+    homedir = "/home/" + user + "/raspi-sump/"
     webchart.create_folders(year, month, homedir)
     webchart.create_chart(homedir)
     webchart.copy_chart(year, month, today, homedir)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `raspisump-1.7.1/conf/raspisump.conf` & `raspisump-1.7.2/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/conf/web/css/raspi.css` & `raspisump-1.7.2/conf/web/css/raspi.css`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/conf/web/css/raspi.css~` & `raspisump-1.7.2/conf/web/css/raspi.css~`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/conf/web/images/logo.png` & `raspisump-1.7.2/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/conf/web/index.html` & `raspisump-1.7.2/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/docs/install.md` & `raspisump-1.7.2/docs/install.md`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/docs/install.pdf` & `raspisump-1.7.2/docs/install.pdf`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/raspisump/alerts.py` & `raspisump-1.7.2/raspisump/alerts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''Send SMTP email alerts in case of sump pump failure.'''
+"""Send SMTP email alerts in case of sump pump failure."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
@@ -16,139 +16,137 @@
 from collections import deque
 import csv
 from raspisump import log
 
 
 config = configparser.RawConfigParser()
 user = os.getlogin()
-config.read('/home/' + user + '/raspi-sump/raspisump.conf')
+config.read("/home/" + user + "/raspi-sump/raspisump.conf")
 
-configs = {'email_to': config.get('email', 'email_to'),
-           'email_from': config.get('email', 'email_from'),
-           'smtp_authentication': config.getint(
-               'email', 'smtp_authentication'),
-           'smtp_tls': config.getint('email', 'smtp_tls'),
-           'smtp_server': config.get('email', 'smtp_server'),
-           'username': config.get('email', 'username'),
-           'password': config.get('email', 'password'),
-           'unit': config.get('pit', 'unit')}
+configs = {
+    "email_to": config.get("email", "email_to"),
+    "email_from": config.get("email", "email_from"),
+    "smtp_authentication": config.getint("email", "smtp_authentication"),
+    "smtp_tls": config.getint("email", "smtp_tls"),
+    "smtp_server": config.get("email", "smtp_server"),
+    "username": config.get("email", "username"),
+    "password": config.get("email", "password"),
+    "unit": config.get("pit", "unit"),
+}
 # If item in raspisump.conf add to configs dict above.  If not then provide
 # a default value
 try:
-    configs['alert_interval'] = config.getint('email', 'alert_interval')
+    configs["alert_interval"] = config.getint("email", "alert_interval")
 except configparser.NoOptionError:
-    configs['alert_interval'] = 5
+    configs["alert_interval"] = 5
 
 try:
-    configs['alert_when'] = config.get('pit', 'alert_when')
+    configs["alert_when"] = config.get("pit", "alert_when")
 except configparser.NoOptionError:
-    configs['alert_when'] = 'high'
+    configs["alert_when"] = "high"
 
 
 def current_time():
-    '''Return the current time as reported by the OS.'''
-    return time.strftime('%I:%M%P %Z')
+    """Return the current time as reported by the OS."""
+    return time.strftime("%I:%M%P %Z")
 
 
 def host_name():
-    '''Return the Raspberry Pi's Hostname'''
+    """Return the Raspberry Pi's Hostname"""
     return platform.node()
 
 
 def unit_types():
-    '''Determine  if inches or centimeters'''
+    """Determine  if inches or centimeters"""
 
-    unit = configs['unit']
+    unit = configs["unit"]
 
-    if unit == 'imperial':
-        return 'inches'
-    if unit == 'metric':
-        return 'centimeters'
+    if unit == "imperial":
+        return "inches"
+    if unit == "metric":
+        return "centimeters"
 
 
 def email_content(water_depth):
-    '''Build the contents of email body which will be sent as an alert'''
+    """Build the contents of email body which will be sent as an alert"""
 
     time_of_day = current_time()
     unit_type = unit_types()
     hostname = host_name()
-    email_contents = {'subject_high': 'Subject: Sump Pump Alert!',
-                      'subject_low': 'Subject: Low Water Level Alert!',
-                      'message_high': 'Critical! The sump pit water level is',
-                      'message_low': 'Warning! The waterlevel is down to'
-                      }
-
-    if configs['alert_when'] == 'high':
-        subject = email_contents['subject_high']
-        message = email_contents['message_high']
+    email_contents = {
+        "subject_high": "Subject: Sump Pump Alert!",
+        "subject_low": "Subject: Low Water Level Alert!",
+        "message_high": "Critical! The sump pit water level is",
+        "message_low": "Warning! The waterlevel is down to",
+    }
+
+    if configs["alert_when"] == "high":
+        subject = email_contents["subject_high"]
+        message = email_contents["message_high"]
     else:
-        subject = email_contents['subject_low']
-        message = email_contents['message_low']
+        subject = email_contents["subject_low"]
+        message = email_contents["message_low"]
 
-    return "\r\n".join((
-        "From: {}".format(configs['email_from']),
-        "To: {}".format(configs['email_to']),
-        "{}".format(subject),
-        "",
-        "{} - {} - {} {} {}.".format(hostname,
-                                     time_of_day,
-                                     message,
-                                     str(water_depth), unit_type),
-        "Next alert in {} minutes".format(configs['alert_interval']),
-        )
+    return "\r\n".join(
+        (
+            f"From: {configs['email_from']}",
+            f"To: {configs['email_to']}",
+            f"{subject}",
+            "",
+            f"{hostname} - {time_of_day} - {message} {str(water_depth)} {unit_type}.",
+            f"Next alert in {configs['alert_interval']} minutes",
         )
+    )
 
 
 def smtp_alerts(water_depth):
-    '''Send email alert if water level greater than critical distance.'''
-    recipients = configs['email_to'].split(', ')
+    """Send email alert if water level greater than critical distance."""
+    recipients = configs["email_to"].split(", ")
     email_body = email_content(water_depth)
-    server = smtplib.SMTP(configs['smtp_server'])
+    server = smtplib.SMTP(configs["smtp_server"])
 
     # Check if smtp server uses TLS
-    if configs['smtp_tls'] == 1:
+    if configs["smtp_tls"] == 1:
         server.starttls()
     else:
         pass
     # Check if smtp server uses authentication
-    if configs['smtp_authentication'] == 1:
-        username = configs['username']
-        password = configs['password']
+    if configs["smtp_authentication"] == 1:
+        username = configs["username"]
+        password = configs["password"]
         server.login(username, password)
     else:
         pass
 
-    server.sendmail(configs['email_from'], recipients, email_body)
+    server.sendmail(configs["email_from"], recipients, email_body)
     server.quit()
 
 
 def determine_if_alert(water_depth):
-    '''Determine if an alert is required.  Only send if last alert has been
+    """Determine if an alert is required.  Only send if last alert has been
     sent more than the amount of time identified in the raspisump.conf file.
-    Entry in conf file is alert_interval under the [email] section.'''
+    Entry in conf file is alert_interval under the [email] section."""
 
-    alert_interval = configs['alert_interval']
+    alert_interval = configs["alert_interval"]
 
-    alert_log = '/home/' + user + '/raspi-sump/logs/alert_log'
+    alert_log = "/home/" + user + "/raspi-sump/logs/alert_log"
 
     if not os.path.isfile(alert_log):
         smtp_alerts(water_depth)
-        log.log_event('alert_log', 'Email SMS Alert Sent')
+        log.log_event("alert_log", "Email SMS Alert Sent")
 
     else:
-        with open(alert_log, 'rt') as f:
+        with open(alert_log, "rt") as f:
             last_row = deque(csv.reader(f), 1)[0]
             last_alert_sent = last_row[0]
-            current_time = time.strftime('%Y-%m-%d %H:%M:%S')
-            last_alert_time = datetime.strptime(
-                last_alert_sent, '%Y-%m-%d %H:%M:%S'
-            )
-            time_now = datetime.strptime(current_time, '%Y-%m-%d %H:%M:%S')
-            delta = (time_now - last_alert_time)
+            current_time = time.strftime("%Y-%m-%d %H:%M:%S")
+            last_alert_time = datetime.strptime(last_alert_sent, "%Y-%m-%d %H:%M:%S")
+            time_now = datetime.strptime(current_time, "%Y-%m-%d %H:%M:%S")
+            delta = time_now - last_alert_time
             minutes_passed = delta.seconds / 60
 
         if minutes_passed >= alert_interval:
             smtp_alerts(water_depth)
-            log.log_event('alert_log', 'Email SMS Alert Sent')
+            log.log_event("alert_log", "Email SMS Alert Sent")
 
         else:
             pass
```

### Comparing `raspisump-1.7.1/raspisump/checkpid.py` & `raspisump-1.7.2/raspisump/checkpid.py`

 * *Files identical despite different names*

### Comparing `raspisump-1.7.1/raspisump/emailtest.py` & `raspisump-1.7.2/raspisump/emailtest.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,30 +25,29 @@
     "smtp_server": config.get("email", "smtp_server"),
     "username": config.get("email", "username"),
     "password": config.get("email", "password"),
 }
 
 
 def test_email_content():
-
     """Build the contents of test email body."""
 
     time_of_day = alerts.current_time()
     hostname = alerts.host_name()
 
     subject = "Subject: Raspi-Sump Email Test"
     message = "Raspi-Sump Test Email"
 
     return "\r\n".join(
         (
-            "From: {}".format(configs["email_from"]),
-            "To: {}".format(configs["email_to"]),
-            "{}".format(subject),
+            f"From: {configs['email_from']}",
+            f"To: {configs['email_to']}",
+            f"{subject}",
             "",
-            "{} - {} - {}.".format(hostname, time_of_day, message),
+            f"{hostname} - {time_of_day} - {message}.",
         )
     )
 
 
 def test_email():
     """Send test email only."""
     recipients = configs["email_to"].split(", ")
```

### Comparing `raspisump-1.7.1/raspisump/heartbeat.py` & `raspisump-1.7.2/raspisump/heartbeat.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''Send Heartbeat alert to test that email notifications are working.'''
+"""Send Heartbeat alert to test that email notifications are working."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
@@ -15,116 +15,110 @@
 from collections import deque
 import csv
 from raspisump import log, alerts
 
 
 config = configparser.RawConfigParser()
 user = os.getlogin()
-config.read('/home/' + user + '/raspi-sump/raspisump.conf')
+config.read("/home/" + user + "/raspi-sump/raspisump.conf")
 
-configs = {'email_to': config.get('email', 'email_to'),
-           'email_from': config.get('email', 'email_from'),
-           'smtp_authentication': config.getint(
-           'email', 'smtp_authentication'),
-           'smtp_tls': config.getint('email', 'smtp_tls'),
-           'smtp_server': config.get('email', 'smtp_server'),
-           'username': config.get('email', 'username'),
-           'password': config.get('email', 'password')
-           }
+configs = {
+    "email_to": config.get("email", "email_to"),
+    "email_from": config.get("email", "email_from"),
+    "smtp_authentication": config.getint("email", "smtp_authentication"),
+    "smtp_tls": config.getint("email", "smtp_tls"),
+    "smtp_server": config.get("email", "smtp_server"),
+    "username": config.get("email", "username"),
+    "password": config.get("email", "password"),
+}
 
 try:
-    configs['heartbeat_interval'] = config.getint('email',
-                                                  'heartbeat_interval')
+    configs["heartbeat_interval"] = config.getint("email", "heartbeat_interval")
 except configparser.NoOptionError:
-    configs['heartbeat_interval'] = 10080
+    configs["heartbeat_interval"] = 10080
 
 
 def get_last_alert_time():
-    '''Retrieve the last alert time string from logfile'''
-    heartbeat_log = '/home/' + user + '/raspi-sump/logs/heartbeat_log'
-    with open(heartbeat_log, 'rt') as f:
+    """Retrieve the last alert time string from logfile"""
+    heartbeat_log = "/home/" + user + "/raspi-sump/logs/heartbeat_log"
+    with open(heartbeat_log, "rt") as f:
         last_row = deque(csv.reader(f), 1)[0]
         return last_row[0]
 
 
 def heartbeat_email_content():
-    '''Build the contents of email body which will be sent as an alert'''
-    heartbeat_interval_time = configs['heartbeat_interval']
-    current_time = time.strftime('%Y-%m-%d %H:%M:%S')
-    last_alert = datetime.strptime(current_time, '%Y-%m-%d %H:%M:%S')
+    """Build the contents of email body which will be sent as an alert"""
+    heartbeat_interval_time = configs["heartbeat_interval"]
+    current_time = time.strftime("%Y-%m-%d %H:%M:%S")
+    last_alert = datetime.strptime(current_time, "%Y-%m-%d %H:%M:%S")
     future_date = last_alert + timedelta(minutes=heartbeat_interval_time + 1)
 
-    weekday = future_date.strftime('%A')[0:3]
-    month = future_date.strftime('%B')
-    hour = future_date.strftime('%I')
-    minute = future_date.strftime('%M')
-    am_pm = future_date.strftime('%p').lower()
+    weekday = future_date.strftime("%A")[0:3]
+    month = future_date.strftime("%B")
+    hour = future_date.strftime("%I")
+    minute = future_date.strftime("%M")
+    am_pm = future_date.strftime("%p").lower()
 
     time_of_day = alerts.current_time()
     hostname = alerts.host_name()
-    subject = 'Subject: Raspi-Sump Heartbeat Notification'
-    message = 'Raspi-Sump Email Notifications Working'
+    subject = "Subject: Raspi-Sump Heartbeat Notification"
+    message = "Raspi-Sump Email Notifications Working"
 
-    return "\r\n".join((
-        "From: {}".format(configs['email_from']),
-        "To: {}".format(configs['email_to']),
-        "{}".format(subject),
-        "",
-        "{} - {} - {}.".format(hostname, time_of_day, message),
-        "Next heartbeat: {} {} {} at {}:{} {}".format(weekday,
-                                                      month,
-                                                      future_date.day,
-                                                      hour,
-                                                      minute,
-                                                      am_pm),
-        )
+    return "\r\n".join(
+        (
+            f"From: {configs['email_from']}",
+            f"To: {configs['email_to']}",
+            f"{subject}",
+            "",
+            f"{hostname} - {time_of_day} - {message}.",
+            f"Next heartbeat: {weekday} {month} {future_date.day} at {hour}:{minute} {am_pm}",
         )
+    )
 
 
 def heartbeat_alerts():
-    '''Send heartbeat email alert if water level greater
-    than critical distance.'''
-    recipients = configs['email_to'].split(', ')
+    """Send heartbeat email alert if water level greater
+    than critical distance."""
+    recipients = configs["email_to"].split(", ")
     email_body = heartbeat_email_content()
-    server = smtplib.SMTP(configs['smtp_server'])
+    server = smtplib.SMTP(configs["smtp_server"])
 
     # Check if smtp server uses TLS
-    if configs['smtp_tls'] == 1:
+    if configs["smtp_tls"] == 1:
         server.starttls()
     else:
         pass
     # Check if smtp server uses authentication
-    if configs['smtp_authentication'] == 1:
-        username = configs['username']
-        password = configs['password']
+    if configs["smtp_authentication"] == 1:
+        username = configs["username"]
+        password = configs["password"]
         server.login(username, password)
     else:
         pass
 
-    server.sendmail(configs['email_from'], recipients, email_body)
+    server.sendmail(configs["email_from"], recipients, email_body)
     server.quit()
 
 
 def determine_if_heartbeat():
-    '''Determine if a heartbeat notification is required and if so, send
-    the notification.'''
+    """Determine if a heartbeat notification is required and if so, send
+    the notification."""
 
-    heartbeat_log = '/home/' + user + '/raspi-sump/logs/heartbeat_log'
+    heartbeat_log = "/home/" + user + "/raspi-sump/logs/heartbeat_log"
     if not os.path.isfile(heartbeat_log):
         heartbeat_alerts()
         log.log_event("heartbeat_log", "Heartbeat Email Sent")
 
     else:
-        heartbeat_interval_time = configs['heartbeat_interval']
+        heartbeat_interval_time = configs["heartbeat_interval"]
         last_email_sent = get_last_alert_time()
-        current_time = time.strftime('%Y-%m-%d %H:%M:%S')
-        last_heartbeat_time = datetime.strptime(last_email_sent,
-                                                '%Y-%m-%d %H:%M:%S')
-        time_now = datetime.strptime(current_time, '%Y-%m-%d %H:%M:%S')
-        delta = (time_now - last_heartbeat_time)
+        current_time = time.strftime("%Y-%m-%d %H:%M:%S")
+        last_heartbeat_time = datetime.strptime(last_email_sent, "%Y-%m-%d %H:%M:%S")
+        time_now = datetime.strptime(current_time, "%Y-%m-%d %H:%M:%S")
+        delta = time_now - last_heartbeat_time
         minutes_passed = int((delta).total_seconds() / 60)
 
         if minutes_passed >= heartbeat_interval_time:
             heartbeat_alerts()
             log.log_event("heartbeat_log", "Heartbeat Email Sent")
         else:
             pass
```

### Comparing `raspisump-1.7.1/raspisump/log.py` & `raspisump-1.7.2/raspisump/log.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-'''Log waterlevel readings, restarts and alerts.'''
+"""Log waterlevel readings, restarts and alerts."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
 # https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
 import os
 
 user = os.getlogin()
 
-def log_event(logfile, notification):
-    _logfile = "/home/" + user + "/raspi-sump/logs/{}".format(logfile)
-    with open(_logfile, 'a') as f:
-        f.write(time.strftime("%Y-%m-%d %H:%M:%S,")),
-        f.write(notification + "\n"),
 
+def log_event(logfile, notification):
+    _logfile = f"/home/{user}/raspi-sump/logs/{logfile}"
+    with open(_logfile, "a") as f:
+        f.write(f"{time.strftime('%Y-%m-%d %H:%M:%S,')}")
+        f.write(f"{notification}\n")
 
-def log_reading(water_depth):
-    '''Log time and water depth reading.'''
-    filename = "/home/" + user + "/raspi-sump/csv/waterlevel-{}.csv".format(
-        time.strftime("%Y%m%d"))
-    with open(filename, 'a') as f:
-        f.write(time.strftime("%H:%M:%S,")),
-        f.write(str(water_depth) + "\n"),
 
+def log_reading(logfile, water_depth):
+    """Log time and water depth reading."""
+    filename = f"/home/{user}/raspi-sump/csv/{logfile}-{time.strftime('%Y%m%d')}.csv"
+    with open(filename, "a") as f:
+        f.write(f"{time.strftime('%H:%M:%S,')}")
+        f.write(f"{water_depth}\n")
```

### Comparing `raspisump-1.7.1/raspisump/reading.py` & `raspisump-1.7.2/raspisump/reading.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,34 +54,38 @@
     unit = configs["unit"]
 
     value = sensor.Measurement(trig_pin, echo_pin, temperature, unit)
 
     try:
         raw_distance = value.raw_distance(sample_wait=0.3)
     except SystemError:
-        log.log_event("error_log",
-                      "ERROR - Signal not received. Possible cable or sensor problem.")
+        log.log_event(
+            "error_log",
+            "ERROR - Signal not received. Possible cable or sensor problem.",
+        )
         exit(0)
 
     return round(value.depth(raw_distance, pit_depth), 1)
 
 
 def water_depth():
     """Determine the depth of the water, log result and generate alert
     if needed.
     """
 
     critical_water_level = configs["critical_water_level"]
     water_depth = water_reading()
     if water_depth < 0.0:
         water_depth = 0.0
-        log.log_reading(water_depth)
-        log.log_event("error_log",
-                      "ERROR - Negative reading adjusted to 0.0. Possible degrading sensor.")
-    log.log_reading(water_depth)
+        log.log_reading("waterlevel", water_depth)
+        log.log_event(
+            "error_log",
+            "ERROR - Negative reading adjusted to 0.0. Possible degrading sensor.",
+        )
+    log.log_reading("waterlevel", water_depth)
 
     if water_depth > critical_water_level and configs["alert_when"] == "high":
         alerts.determine_if_alert(water_depth)
     elif water_depth < critical_water_level and configs["alert_when"] == "low":
         alerts.determine_if_alert(water_depth)
     else:
         pass
```

### Comparing `raspisump-1.7.1/raspisump/todaychart.py` & `raspisump-1.7.2/raspisump/todaychart.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         x=date,
         y=value,
         ls="solid",
         linewidth=2,
         color="#" + configs["line_color"],
         fmt=":",
     )
-    title = "Sump Pit Water Level {}".format(time.strftime("%Y-%m-%d %H:%M"))
+    title = f"Sump Pit Water Level {time.strftime('%Y-%m-%d %H:%M')}"
     title_set = plt.title(title)
     title_set.set_y(1.09)
     plt.subplots_adjust(top=0.86)
 
     if unit == "imperial":
         plt.ylabel("inches")
     if unit == "metric":
```

### Comparing `raspisump-1.7.1/raspisump/webchart.py` & `raspisump-1.7.2/raspisump/webchart.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 import subprocess
 import time
 from raspisump import todaychart
 
 
 def create_folders(year, month, homedir):
     """Check if folders exist in charts folder and create them if they don't"""
-    if not os.path.isdir("{}charts/{}/".format(homedir, year)):
-        _year = "mkdir {}charts/{}".format(homedir, year)
+    if not os.path.isdir(f"{homedir}charts/{year}/"):
+        _year = f"mkdir {homedir}charts/{year}"
         create_year = _year.split(" ")
         subprocess.call(create_year)
 
-    if not os.path.isdir("{}charts/{}/{}/".format(homedir, year, month)):
-        _month = "mkdir {}charts/{}/{}".format(homedir, year, month)
+    if not os.path.isdir(f"{homedir}charts/{year}/{month}/"):
+        _month = f"mkdir {homedir}charts/{year}/{month}"
         create_month = _month.split(" ")
         subprocess.call(create_month)
 
 
 def create_chart(homedir):
     """Create a chart of sump pit activity and save to web folder"""
-    csv_file = "{}csv/waterlevel-{}.csv".format(homedir, time.strftime("%Y%m%d"))
-    filename = "{}charts/today.png".format(homedir)
+    csv_file = f"{homedir}csv/waterlevel-{time.strftime('%Y%m%d')}.csv"
+    filename = f"{homedir}charts/today.png"
     todaychart.graph(csv_file, filename)
 
 
 def copy_chart(year, month, today, homedir):
     """Copy today.png to year/month/day folder for web viewing"""
-    copy_cmd = "cp {}charts/today.png {}charts/{}/{}/{}.png".format(
-        homedir, homedir, year, month, today
+    copy_cmd = (
+        f"cp {homedir}charts/today.png {homedir}charts/{year}/{month}/{today}.png"
     )
     copy_file = copy_cmd.split(" ")
     subprocess.call(copy_file)
```

### Comparing `raspisump-1.7.1/raspisump.egg-info/PKG-INFO` & `raspisump-1.7.2/raspisump.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.7.1
+Version: 1.7.2
 Summary: A sump pit monitoring system for Raspberry Pi
 Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `raspisump-1.7.1/raspisump.egg-info/SOURCES.txt` & `raspisump-1.7.2/raspisump.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -31,8 +31,10 @@
 raspisump/reading.py
 raspisump/todaychart.py
 raspisump/webchart.py
 raspisump.egg-info/PKG-INFO
 raspisump.egg-info/SOURCES.txt
 raspisump.egg-info/dependency_links.txt
 raspisump.egg-info/requires.txt
-raspisump.egg-info/top_level.txt
+raspisump.egg-info/top_level.txt
+tests/tests_logging.py
+tests/tests_sump.py
```

### Comparing `raspisump-1.7.1/setup.py` & `raspisump-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.7.1"
+version = "1.7.2"
 user = os.getlogin()
 
 homedir = "/home/" + user + "/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
@@ -27,15 +27,15 @@
     (homedir + "docs", ["docs/install.md"]),
     (homedir + "cron", ["cron/README.md"]),
     (homedir + "cron", ["cron/picrontab"]),
     (homedir + "web", ["conf/web/index.html"]),
     (homedir + "web/images", ["conf/web/images/logo.png"]),
     (homedir + "web/css", ["conf/web/css/index.html"]),
     (homedir + "web/css", ["conf/web/css/raspi.css"]),
-    (homedir, ["VERSION"])
+    (homedir, ["VERSION"]),
 ]
 
 setup(
     name="raspisump",
     version=version,
     description="A sump pit monitoring system for Raspberry Pi",
     long_description_content_type="text/markdown",
```

