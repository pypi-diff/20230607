# Comparing `tmp/InternetSpeedLogger-1.2.0.tar.gz` & `tmp/InternetSpeedLogger-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternetSpeedLogger-1.2.0.tar", last modified: Sun Jun  4 08:40:49 2023, max compression
+gzip compressed data, was "InternetSpeedLogger-1.3.0.tar", last modified: Wed Jun  7 09:35:22 2023, max compression
```

## Comparing `InternetSpeedLogger-1.2.0.tar` & `InternetSpeedLogger-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.930216 InternetSpeedLogger-1.2.0/
--rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.2.0/LICENSE
--rw-r--r--   0 andreas   (1000) apache      (48)     5809 2023-06-04 08:40:49.930216 InternetSpeedLogger-1.2.0/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)     3889 2023-06-03 13:09:41.000000 InternetSpeedLogger-1.2.0/README.md
--rw-r--r--   0 andreas   (1000) apache      (48)      936 2023-06-04 08:33:54.000000 InternetSpeedLogger-1.2.0/pyproject.toml
--rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-04 08:40:49.931216 InternetSpeedLogger-1.2.0/setup.cfg
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.920216 InternetSpeedLogger-1.2.0/src/
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.925216 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/
--rw-r--r--   0 andreas   (1000) apache      (48)     5711 2023-06-04 08:33:35.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/InternetSpeedLogger.py
--rw-r--r--   0 andreas   (1000) apache      (48)       47 2023-06-03 16:58:12.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/__init__.py
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 08:40:49.929216 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/
--rw-r--r--   0 andreas   (1000) apache      (48)     5809 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/entry_points.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       14 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-04 08:40:49.000000 InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 09:35:22.195748 InternetSpeedLogger-1.3.0/
+-rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-02 15:28:30.000000 InternetSpeedLogger-1.3.0/LICENSE
+-rw-r--r--   0 andreas   (1000) apache      (48)     7761 2023-06-07 09:35:22.192748 InternetSpeedLogger-1.3.0/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)     5841 2023-06-07 09:30:31.000000 InternetSpeedLogger-1.3.0/README.md
+-rw-r--r--   0 andreas   (1000) apache      (48)      968 2023-06-07 09:00:08.000000 InternetSpeedLogger-1.3.0/pyproject.toml
+-rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-07 09:35:22.195748 InternetSpeedLogger-1.3.0/setup.cfg
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 09:35:22.174748 InternetSpeedLogger-1.3.0/src/
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 09:35:22.179748 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger/
+-rw-r--r--   0 andreas   (1000) apache      (48)     6145 2023-06-07 09:00:00.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger/InternetSpeedLogger.py
+-rw-r--r--   0 andreas   (1000) apache      (48)       47 2023-06-03 16:58:12.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger/__init__.py
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 09:35:22.190748 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/
+-rw-r--r--   0 andreas   (1000) apache      (48)     7761 2023-06-07 09:35:22.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)      399 2023-06-07 09:35:22.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-07 09:35:22.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       85 2023-06-07 09:35:22.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/entry_points.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       32 2023-06-07 09:35:22.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       20 2023-06-07 09:35:22.000000 InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/top_level.txt
```

### Comparing `InternetSpeedLogger-1.2.0/LICENSE` & `InternetSpeedLogger-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `InternetSpeedLogger-1.2.0/PKG-INFO` & `InternetSpeedLogger-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,15 +62,15 @@
 InternetSpeedLogger
 ```
 
 Type `InternetSpeedLogger --help` to get detailed execution information:
 
 ```
 usage: InternetSpeedLogger [-h] [--version] [-i INTERVAL] [-d DURATION]
-                           [-l LOG_FILE]
+                           [-l LOG_FILE] [-no]
 
 A Python script that continuously monitors and logs your internet
 speed. It tests both download and upload speeds at regular intervals
 and records the data in a CSV file for easy analysis and tracking.
 Ideal for auditing your network performance or ISP reliability over
 time.
             
@@ -83,25 +83,60 @@
                         interval is not shorter than the time needed for
                         testing. (default: 60)
   -d DURATION, --duration DURATION
                         Duration of the entire test runs. The script will
                         automatically end after this duration. Set to <= 0 for
                         infinite. (default: 0)
   -l LOG_FILE, --log_file LOG_FILE
-                        Filename for the log-file. NOTE: ".csv" will be
-                        automatically appended to the filename!
+                        Filename for the log-file. NOTE: A similar filename
+                        will be chosen if a file with this name already
+                        exists.
+  -no, --no_overwrite   Set this flag to automatically select a similar log-
+                        filename, so a potentially already existing file will
+                        not be overwritten.
 
 Default location of the log-file:
     A .csv-file will be created, which will contain all logged information.
     Default Filename: "YYYY-MM-DD_HH:MM:SS_internet_speeds.csv"
-    Default Location: typically "/home/<username>" on Linux
-                      typically "C:\Users\<username>" on Windows
-                      typically "/Users/<username>" on macOS
+    Default Location: <tmp_dir>/InternetSpeedLogger/
+        <tmp_dir> on Windows: C:\TEMP, C:\TMP, \TEMP, or \TMP, in that order
+        <tmp_dir> on all other: /tmp, /var/tmp, or /usr/tmp, in that order
 ```
 
+## Sample Data
+
+Below is a small sample of the data that will be logged in the CSV file by
+InternetSpeedLogger:
+
+| Timestamp         | Download (bps)    | Upload (bps)       | Datetime            | Download (Mbps) | Upload (Mbps) |
+|-------------------|-------------------|--------------------|---------------------|-----------------|---------------|
+| 1686061579.679576 | 89643494.95465901 | 35883256.43988523  | 2023-06-06 16:26:19 | 90              | 36            |
+| 1686061662.23925  | 89641818.67603663 | 36233910.883253716 | 2023-06-06 16:27:42 | 90              | 36            |
+| 1686061721.562057 | 87986931.8695042  | 37110387.93753454  | 2023-06-06 16:28:41 | 88              | 37            |
+| 1686061781.628893 | 91452820.98341656 | 37945852.74793821  | 2023-06-06 16:29:41 | 91              | 38            |
+| 1686061841.479557 | 91453448.72492264 | 38497589.18734731  | 2023-06-06 16:30:41 | 91              | 38            |
+
+Each row represents a single speed test with timestamp of when the test took
+place, the download and upload speeds in bps and Mbps, and the formatted
+datetime.
+
+## Visualizing Data
+
+Once you have accumulated a decent amount of data, you might want to visualize
+it. Check out the
+[InternetSpeedVisualizer](https://github.com/Andreas-Menzel/InternetSpeedVisualizer)
+repository. This companion tool provides a suite of visualization options,
+allowing you to uncover insights about your Internet speed over time.
+
+![Internet Speed Visualizer Preview](images/InternetSpeed.png)
+
+Follow the instructions in its README to get started. Your data logging with
+InternetSpeedLogger can now be taken to the next level with this visualization
+tool!
+
 ## Contribution
 
 We warmly welcome contributions to the InternetSpeedLogger project! Your ideas
 and work can make a real difference to its development.
 
 There are many ways to contribute:
```

### Comparing `InternetSpeedLogger-1.2.0/pyproject.toml` & `InternetSpeedLogger-1.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "InternetSpeedLogger"
-version = "1.2.0"
+version = "1.3.0"
 dependencies = [
+    "matplotlib",
+    "pandas",
     "speedtest_cli"
 ]
 authors = [
   { name="Andreas Menzel", email="mail@andreas-menzel.com" },
 ]
 description = "A Python script that continuously monitors and logs your internet speed."
 readme = "README.md"
```

### Comparing `InternetSpeedLogger-1.2.0/src/InternetSpeedLogger/InternetSpeedLogger.py` & `InternetSpeedLogger-1.3.0/src/InternetSpeedLogger/InternetSpeedLogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # InternetSpeedLogger
 #
 # A Python script that continuously monitors and logs your internet speed. It
 # tests both download and upload speeds at regular intervals and records the
 # data in a CSV file for easy analysis and tracking. Ideal for auditing your
 # network performance or ISP reliability over time.
 #
-# https://github.com/Andreas-Menzel/InternetSpeedLogger
+# https://github.com/Andreas-Menzel/InternetSpeedLogger/
 # https://pypi.org/project/InternetSpeedLogger/
 # ------------------------------------------------------------------------------
 # @author: Andreas Menzel
 # @license: MIT License
 # ------------------------------------------------------------------------------
 
 import argparse
@@ -21,15 +21,15 @@
 from pathlib import Path
 from signal import signal, SIGINT
 from speedtest import Speedtest
 from tempfile import gettempdir
 from time import sleep
 
 
-script_version = '1.2.0'
+script_version = '1.3.0'
 
 
 def argparse_check_positive(value):
     ivalue = int(value)
     if ivalue <= 0:
         raise argparse.ArgumentTypeError(
             "%s is an invalid positive int value" % value)
@@ -64,14 +64,17 @@
     parser.add_argument('-d', '--duration',
                         help='Duration of the entire test runs. The script will automatically end after this duration. Set to <= 0 for infinite. (default: %(default)s)',
                         type=int,
                         default=0)
     parser.add_argument('-l', '--log_file',
                         help='Filename for the log-file. NOTE: A similar filename will be chosen if a file with this name already exists.',
                         default='')
+    parser.add_argument('-no', '--no_overwrite',
+                        help='Set this flag to automatically select a similar log-filename, so a potentially already existing file will not be overwritten.',
+                        action='store_true')
     return parser.parse_args()
 
 
 def main():
     args = setupArgumentParser()
 
     st = Speedtest()
@@ -84,29 +87,32 @@
             csv_file = Path(f'{args.log_file}.csv')
     else:
         # Set to default/fallback location.
         csv_file = Path(
             f'{Path(gettempdir(), "InternetSpeedLogger", datetimeString)}_internet_speeds.csv')
 
     # Make sure that the log-file is unique and does not exist yet.
-    if csv_file.exists():
-        csv_file = Path(csv_file.parent, f'{csv_file.stem}_{datetimeString}{csv_file.suffix}')
-    if csv_file.exists():
-        counter = 2
-        new_csv_file = csv_file
-        while new_csv_file.exists():
-            new_csv_file = Path(csv_file.parent, f'{csv_file.stem}_{counter}{csv_file.suffix}')
-            counter = counter + 1
-        csv_file = new_csv_file
+    if args.no_overwrite or args.log_file == '':
+        if csv_file.exists():
+            csv_file = Path(csv_file.parent,
+                            f'{csv_file.stem}_{datetimeString}{csv_file.suffix}')
+        if csv_file.exists():
+            counter = 2
+            new_csv_file = csv_file
+            while new_csv_file.exists():
+                new_csv_file = Path(
+                    csv_file.parent, f'{csv_file.stem}_{counter}{csv_file.suffix}')
+                counter = counter + 1
+            csv_file = new_csv_file
 
     print(f"""\
 InternetSpeedLogger (version {script_version})
 
 Testing interval: {args.interval} s
-Testing duration: {args.duration} s
+Testing duration: {str(args.duration) + ' s' if args.duration > 0 else 'infinite'}
 Log-file: "{csv_file.absolute()}"\
     """)
 
     csv_file.parent.mkdir(parents=True, exist_ok=True)
     with open(csv_file, mode='w') as file:
         writer = csv.writer(file)
         writer.writerow(['Timestamp', 'Download (bps)', 'Upload (bps)',
```

### Comparing `InternetSpeedLogger-1.2.0/src/InternetSpeedLogger.egg-info/PKG-INFO` & `InternetSpeedLogger-1.3.0/src/InternetSpeedLogger.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedLogger
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python script that continuously monitors and logs your internet speed.
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -62,15 +62,15 @@
 InternetSpeedLogger
 ```
 
 Type `InternetSpeedLogger --help` to get detailed execution information:
 
 ```
 usage: InternetSpeedLogger [-h] [--version] [-i INTERVAL] [-d DURATION]
-                           [-l LOG_FILE]
+                           [-l LOG_FILE] [-no]
 
 A Python script that continuously monitors and logs your internet
 speed. It tests both download and upload speeds at regular intervals
 and records the data in a CSV file for easy analysis and tracking.
 Ideal for auditing your network performance or ISP reliability over
 time.
             
@@ -83,25 +83,60 @@
                         interval is not shorter than the time needed for
                         testing. (default: 60)
   -d DURATION, --duration DURATION
                         Duration of the entire test runs. The script will
                         automatically end after this duration. Set to <= 0 for
                         infinite. (default: 0)
   -l LOG_FILE, --log_file LOG_FILE
-                        Filename for the log-file. NOTE: ".csv" will be
-                        automatically appended to the filename!
+                        Filename for the log-file. NOTE: A similar filename
+                        will be chosen if a file with this name already
+                        exists.
+  -no, --no_overwrite   Set this flag to automatically select a similar log-
+                        filename, so a potentially already existing file will
+                        not be overwritten.
 
 Default location of the log-file:
     A .csv-file will be created, which will contain all logged information.
     Default Filename: "YYYY-MM-DD_HH:MM:SS_internet_speeds.csv"
-    Default Location: typically "/home/<username>" on Linux
-                      typically "C:\Users\<username>" on Windows
-                      typically "/Users/<username>" on macOS
+    Default Location: <tmp_dir>/InternetSpeedLogger/
+        <tmp_dir> on Windows: C:\TEMP, C:\TMP, \TEMP, or \TMP, in that order
+        <tmp_dir> on all other: /tmp, /var/tmp, or /usr/tmp, in that order
 ```
 
+## Sample Data
+
+Below is a small sample of the data that will be logged in the CSV file by
+InternetSpeedLogger:
+
+| Timestamp         | Download (bps)    | Upload (bps)       | Datetime            | Download (Mbps) | Upload (Mbps) |
+|-------------------|-------------------|--------------------|---------------------|-----------------|---------------|
+| 1686061579.679576 | 89643494.95465901 | 35883256.43988523  | 2023-06-06 16:26:19 | 90              | 36            |
+| 1686061662.23925  | 89641818.67603663 | 36233910.883253716 | 2023-06-06 16:27:42 | 90              | 36            |
+| 1686061721.562057 | 87986931.8695042  | 37110387.93753454  | 2023-06-06 16:28:41 | 88              | 37            |
+| 1686061781.628893 | 91452820.98341656 | 37945852.74793821  | 2023-06-06 16:29:41 | 91              | 38            |
+| 1686061841.479557 | 91453448.72492264 | 38497589.18734731  | 2023-06-06 16:30:41 | 91              | 38            |
+
+Each row represents a single speed test with timestamp of when the test took
+place, the download and upload speeds in bps and Mbps, and the formatted
+datetime.
+
+## Visualizing Data
+
+Once you have accumulated a decent amount of data, you might want to visualize
+it. Check out the
+[InternetSpeedVisualizer](https://github.com/Andreas-Menzel/InternetSpeedVisualizer)
+repository. This companion tool provides a suite of visualization options,
+allowing you to uncover insights about your Internet speed over time.
+
+![Internet Speed Visualizer Preview](images/InternetSpeed.png)
+
+Follow the instructions in its README to get started. Your data logging with
+InternetSpeedLogger can now be taken to the next level with this visualization
+tool!
+
 ## Contribution
 
 We warmly welcome contributions to the InternetSpeedLogger project! Your ideas
 and work can make a real difference to its development.
 
 There are many ways to contribute:
```

