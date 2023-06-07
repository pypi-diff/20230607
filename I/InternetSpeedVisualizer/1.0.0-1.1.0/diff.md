# Comparing `tmp/InternetSpeedVisualizer-1.0.0.tar.gz` & `tmp/InternetSpeedVisualizer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InternetSpeedVisualizer-1.0.0.tar", last modified: Sun Jun  4 15:29:05 2023, max compression
+gzip compressed data, was "InternetSpeedVisualizer-1.1.0.tar", last modified: Wed Jun  7 10:45:52 2023, max compression
```

## Comparing `InternetSpeedVisualizer-1.0.0.tar` & `InternetSpeedVisualizer-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 15:29:05.313742 InternetSpeedVisualizer-1.0.0/
--rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-04 14:40:05.000000 InternetSpeedVisualizer-1.0.0/LICENSE
--rw-r--r--   0 andreas   (1000) apache      (48)     5760 2023-06-04 15:29:05.312742 InternetSpeedVisualizer-1.0.0/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)     3725 2023-06-04 15:27:55.000000 InternetSpeedVisualizer-1.0.0/README.md
--rw-r--r--   0 andreas   (1000) apache      (48)     1079 2023-06-04 14:47:23.000000 InternetSpeedVisualizer-1.0.0/pyproject.toml
--rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-04 15:29:05.313742 InternetSpeedVisualizer-1.0.0/setup.cfg
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 15:29:05.301742 InternetSpeedVisualizer-1.0.0/src/
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 15:29:05.307742 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer/
--rw-r--r--   0 andreas   (1000) apache      (48)     6506 2023-06-04 15:22:25.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer/InternetSpeedVisualizer.py
--rw-r--r--   0 andreas   (1000) apache      (48)       55 2023-06-04 14:44:50.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer/__init__.py
-drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-04 15:29:05.312742 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/
--rw-r--r--   0 andreas   (1000) apache      (48)     5760 2023-06-04 15:29:05.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/PKG-INFO
--rw-r--r--   0 andreas   (1000) apache      (48)      435 2023-06-04 15:29:05.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/SOURCES.txt
--rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-04 15:29:05.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/dependency_links.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       97 2023-06-04 15:29:05.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/entry_points.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       18 2023-06-04 15:29:05.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/requires.txt
--rw-r--r--   0 andreas   (1000) apache      (48)       24 2023-06-04 15:29:05.000000 InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/top_level.txt
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 10:45:52.625630 InternetSpeedVisualizer-1.1.0/
+-rw-r--r--   0 andreas   (1000) apache      (48)     1071 2023-06-04 14:40:05.000000 InternetSpeedVisualizer-1.1.0/LICENSE
+-rw-r--r--   0 andreas   (1000) apache      (48)     7030 2023-06-07 10:45:52.623630 InternetSpeedVisualizer-1.1.0/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)     4995 2023-06-07 10:35:20.000000 InternetSpeedVisualizer-1.1.0/README.md
+-rw-r--r--   0 andreas   (1000) apache      (48)     1079 2023-06-07 10:37:01.000000 InternetSpeedVisualizer-1.1.0/pyproject.toml
+-rw-r--r--   0 andreas   (1000) apache      (48)       38 2023-06-07 10:45:52.625630 InternetSpeedVisualizer-1.1.0/setup.cfg
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 10:45:52.613630 InternetSpeedVisualizer-1.1.0/src/
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 10:45:52.617630 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer/
+-rw-r--r--   0 andreas   (1000) apache      (48)     8604 2023-06-07 10:37:06.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer/InternetSpeedVisualizer.py
+-rw-r--r--   0 andreas   (1000) apache      (48)       55 2023-06-04 14:44:50.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer/__init__.py
+drwxr-xr-x   0 andreas   (1000) apache      (48)        0 2023-06-07 10:45:52.622630 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/
+-rw-r--r--   0 andreas   (1000) apache      (48)     7030 2023-06-07 10:45:52.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/PKG-INFO
+-rw-r--r--   0 andreas   (1000) apache      (48)      435 2023-06-07 10:45:52.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)        1 2023-06-07 10:45:52.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       97 2023-06-07 10:45:52.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/entry_points.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       18 2023-06-07 10:45:52.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/requires.txt
+-rw-r--r--   0 andreas   (1000) apache      (48)       24 2023-06-07 10:45:52.000000 InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/top_level.txt
```

### Comparing `InternetSpeedVisualizer-1.0.0/LICENSE` & `InternetSpeedVisualizer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `InternetSpeedVisualizer-1.0.0/PKG-INFO` & `InternetSpeedVisualizer-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedVisualizer
-Version: 1.0.0
+Version: 1.1.0
 Summary: InternetSpeedVisualizer is a powerful tool designed to help you visualize and analyze your Internet speed data, collected using the InternetSpeedLogger. 
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,45 +33,45 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # InternetSpeedVisualizer
 
-## 🚀 Powerful Python Tool for Analyzing Internet Connection Speed
+## Powerful Python Tool for Analyzing Internet Connection Speed
 
 InternetSpeedVisualizer is a tool designed to help you visualize and analyze
 your Internet speed data, which you can collect using the
 [InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger).
 
-## 📥 Installation
+## Installation
 
 Installation is as simple as running a pip command:
 
 ```bash
 pip install InternetSpeedVisualizer
 ```
 
-## 🏁 Usage
+## Usage
 
 Once InternetSpeedVisualizer is installed using pip, you can easily execute the
 script from anywhere:
 
 ```bash
 InternetSpeedVisualizer
 ```
 
 To access detailed execution information, simply type
 `InternetSpeedVisualizer --help`:
 
 ```
 usage: InternetSpeedVisualizer [-h] [--version] -i INPUT [-o OUTPUT]
                                [--width WIDTH] [--height HEIGHT]
-                               [-d MAX_DOWNLOAD] [-u MAX_UPLOAD]
-                               [--interactive]
+                               [-d <min>;<max>] [-u <min>;<max>]
+                               [--interactive] [-no]
 
 InternetSpeedVisualizer is a powerful tool designed to help you visualize and
 analyze your Internet speed data, collected using the InternetSpeedVisualizer.
             
 
 options:
   -h, --help            show this help message and exit
@@ -79,23 +79,58 @@
   -i INPUT, --input INPUT
                         Path to the .csv-log-file generated by
                         InternetSpeedVisualizer.
   -o OUTPUT, --output OUTPUT
                         Path to the line-graph-image that should be created.
   --width WIDTH         Width in inch of the output image. (default: 20)
   --height HEIGHT       Height in inch of the output image. (default: 10)
-  -d MAX_DOWNLOAD, --max_download MAX_DOWNLOAD
-                        Maximum download speed promised by the ISP. (default:
-                        250)
-  -u MAX_UPLOAD, --max_upload MAX_UPLOAD
-                        Maximum upload speed promised by the ISP. (default:
-                        40)
+  -d <min>;<max>, --download <min>;<max>
+                        Download speed promised by the ISP. (default:
+                        "180;250")
+  -u <min>;<max>, --upload <min>;<max>
+                        Upload speed promised by the ISP. (default: "35;40")
   --interactive         Show an interactive line-graph. (default: False)
+  -no, --no_overwrite   Set this flag to automatically select a similar
+                        output-filename, so a potentially already existing
+                        file will not be overwritten.
+
+Passing only minimum download speed:
+    --download "200;"
+Passing only maximum download speed:
+    --download ";250"
+Passing only minimum upload speed:
+    --upload "30;"
+Passing only maximum upload speed:
+    --upload ";40"
 ```
 
+## Sample output
+
+Given a sample .csv-file names `internet_speeds.csv`, the following command
+generates the following image:
+
+```
+InternetSpeedVisualizer -i internet_speeds.csv -o internet_speeds.png -d "180;250" -u "30;40"
+```
+
+![Internet Speed Visualizer Preview](images/internet_speeds.png)
+
+## Companion Tool: InternetSpeedLogger
+
+InternetSpeedVisualizer is designed to work in harmony with
+[InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger).
+This companion tool allows you to continuously log your internet speed at
+defined intervals.
+
+By saving the data in a CSV file,
+[InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger)
+provides you with a historical log of your internet speeds. This data can then
+be visualized using InternetSpeedVisualizer, enabling you to understand trends
+and fluctuations in your internet speed over time.
+
 ## 👏 Contribution
 
 We warmly welcome and highly appreciate contributions to the
 InternetSpeedVisualizer project! Your creative ideas and diligent work can make
 a real difference in its development and enhance the user experience.
 
 Multiple ways to contribute:
```

### Comparing `InternetSpeedVisualizer-1.0.0/README.md` & `InternetSpeedVisualizer-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # InternetSpeedVisualizer
 
-## 🚀 Powerful Python Tool for Analyzing Internet Connection Speed
+## Powerful Python Tool for Analyzing Internet Connection Speed
 
 InternetSpeedVisualizer is a tool designed to help you visualize and analyze
 your Internet speed data, which you can collect using the
 [InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger).
 
-## 📥 Installation
+## Installation
 
 Installation is as simple as running a pip command:
 
 ```bash
 pip install InternetSpeedVisualizer
 ```
 
-## 🏁 Usage
+## Usage
 
 Once InternetSpeedVisualizer is installed using pip, you can easily execute the
 script from anywhere:
 
 ```bash
 InternetSpeedVisualizer
 ```
 
 To access detailed execution information, simply type
 `InternetSpeedVisualizer --help`:
 
 ```
 usage: InternetSpeedVisualizer [-h] [--version] -i INPUT [-o OUTPUT]
                                [--width WIDTH] [--height HEIGHT]
-                               [-d MAX_DOWNLOAD] [-u MAX_UPLOAD]
-                               [--interactive]
+                               [-d <min>;<max>] [-u <min>;<max>]
+                               [--interactive] [-no]
 
 InternetSpeedVisualizer is a powerful tool designed to help you visualize and
 analyze your Internet speed data, collected using the InternetSpeedVisualizer.
             
 
 options:
   -h, --help            show this help message and exit
@@ -42,23 +42,58 @@
   -i INPUT, --input INPUT
                         Path to the .csv-log-file generated by
                         InternetSpeedVisualizer.
   -o OUTPUT, --output OUTPUT
                         Path to the line-graph-image that should be created.
   --width WIDTH         Width in inch of the output image. (default: 20)
   --height HEIGHT       Height in inch of the output image. (default: 10)
-  -d MAX_DOWNLOAD, --max_download MAX_DOWNLOAD
-                        Maximum download speed promised by the ISP. (default:
-                        250)
-  -u MAX_UPLOAD, --max_upload MAX_UPLOAD
-                        Maximum upload speed promised by the ISP. (default:
-                        40)
+  -d <min>;<max>, --download <min>;<max>
+                        Download speed promised by the ISP. (default:
+                        "180;250")
+  -u <min>;<max>, --upload <min>;<max>
+                        Upload speed promised by the ISP. (default: "35;40")
   --interactive         Show an interactive line-graph. (default: False)
+  -no, --no_overwrite   Set this flag to automatically select a similar
+                        output-filename, so a potentially already existing
+                        file will not be overwritten.
+
+Passing only minimum download speed:
+    --download "200;"
+Passing only maximum download speed:
+    --download ";250"
+Passing only minimum upload speed:
+    --upload "30;"
+Passing only maximum upload speed:
+    --upload ";40"
 ```
 
+## Sample output
+
+Given a sample .csv-file names `internet_speeds.csv`, the following command
+generates the following image:
+
+```
+InternetSpeedVisualizer -i internet_speeds.csv -o internet_speeds.png -d "180;250" -u "30;40"
+```
+
+![Internet Speed Visualizer Preview](images/internet_speeds.png)
+
+## Companion Tool: InternetSpeedLogger
+
+InternetSpeedVisualizer is designed to work in harmony with
+[InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger).
+This companion tool allows you to continuously log your internet speed at
+defined intervals.
+
+By saving the data in a CSV file,
+[InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger)
+provides you with a historical log of your internet speeds. This data can then
+be visualized using InternetSpeedVisualizer, enabling you to understand trends
+and fluctuations in your internet speed over time.
+
 ## 👏 Contribution
 
 We warmly welcome and highly appreciate contributions to the
 InternetSpeedVisualizer project! Your creative ideas and diligent work can make
 a real difference in its development and enhance the user experience.
 
 Multiple ways to contribute:
```

### Comparing `InternetSpeedVisualizer-1.0.0/pyproject.toml` & `InternetSpeedVisualizer-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "InternetSpeedVisualizer"
-version = "1.0.0"
+version = "1.1.0"
 dependencies = [
     "matplotlib",
     "pandas"
 ]
 authors = [
   { name="Andreas Menzel", email="mail@andreas-menzel.com" },
 ]
```

### Comparing `InternetSpeedVisualizer-1.0.0/src/InternetSpeedVisualizer.egg-info/PKG-INFO` & `InternetSpeedVisualizer-1.1.0/src/InternetSpeedVisualizer.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: InternetSpeedVisualizer
-Version: 1.0.0
+Version: 1.1.0
 Summary: InternetSpeedVisualizer is a powerful tool designed to help you visualize and analyze your Internet speed data, collected using the InternetSpeedLogger. 
 Author-email: Andreas Menzel <mail@andreas-menzel.com>
 License: MIT License
         
         Copyright (c) 2023 Andreas Menzel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -33,45 +33,45 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # InternetSpeedVisualizer
 
-## 🚀 Powerful Python Tool for Analyzing Internet Connection Speed
+## Powerful Python Tool for Analyzing Internet Connection Speed
 
 InternetSpeedVisualizer is a tool designed to help you visualize and analyze
 your Internet speed data, which you can collect using the
 [InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger).
 
-## 📥 Installation
+## Installation
 
 Installation is as simple as running a pip command:
 
 ```bash
 pip install InternetSpeedVisualizer
 ```
 
-## 🏁 Usage
+## Usage
 
 Once InternetSpeedVisualizer is installed using pip, you can easily execute the
 script from anywhere:
 
 ```bash
 InternetSpeedVisualizer
 ```
 
 To access detailed execution information, simply type
 `InternetSpeedVisualizer --help`:
 
 ```
 usage: InternetSpeedVisualizer [-h] [--version] -i INPUT [-o OUTPUT]
                                [--width WIDTH] [--height HEIGHT]
-                               [-d MAX_DOWNLOAD] [-u MAX_UPLOAD]
-                               [--interactive]
+                               [-d <min>;<max>] [-u <min>;<max>]
+                               [--interactive] [-no]
 
 InternetSpeedVisualizer is a powerful tool designed to help you visualize and
 analyze your Internet speed data, collected using the InternetSpeedVisualizer.
             
 
 options:
   -h, --help            show this help message and exit
@@ -79,23 +79,58 @@
   -i INPUT, --input INPUT
                         Path to the .csv-log-file generated by
                         InternetSpeedVisualizer.
   -o OUTPUT, --output OUTPUT
                         Path to the line-graph-image that should be created.
   --width WIDTH         Width in inch of the output image. (default: 20)
   --height HEIGHT       Height in inch of the output image. (default: 10)
-  -d MAX_DOWNLOAD, --max_download MAX_DOWNLOAD
-                        Maximum download speed promised by the ISP. (default:
-                        250)
-  -u MAX_UPLOAD, --max_upload MAX_UPLOAD
-                        Maximum upload speed promised by the ISP. (default:
-                        40)
+  -d <min>;<max>, --download <min>;<max>
+                        Download speed promised by the ISP. (default:
+                        "180;250")
+  -u <min>;<max>, --upload <min>;<max>
+                        Upload speed promised by the ISP. (default: "35;40")
   --interactive         Show an interactive line-graph. (default: False)
+  -no, --no_overwrite   Set this flag to automatically select a similar
+                        output-filename, so a potentially already existing
+                        file will not be overwritten.
+
+Passing only minimum download speed:
+    --download "200;"
+Passing only maximum download speed:
+    --download ";250"
+Passing only minimum upload speed:
+    --upload "30;"
+Passing only maximum upload speed:
+    --upload ";40"
 ```
 
+## Sample output
+
+Given a sample .csv-file names `internet_speeds.csv`, the following command
+generates the following image:
+
+```
+InternetSpeedVisualizer -i internet_speeds.csv -o internet_speeds.png -d "180;250" -u "30;40"
+```
+
+![Internet Speed Visualizer Preview](images/internet_speeds.png)
+
+## Companion Tool: InternetSpeedLogger
+
+InternetSpeedVisualizer is designed to work in harmony with
+[InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger).
+This companion tool allows you to continuously log your internet speed at
+defined intervals.
+
+By saving the data in a CSV file,
+[InternetSpeedLogger](https://github.com/Andreas-Menzel/InternetSpeedLogger)
+provides you with a historical log of your internet speeds. This data can then
+be visualized using InternetSpeedVisualizer, enabling you to understand trends
+and fluctuations in your internet speed over time.
+
 ## 👏 Contribution
 
 We warmly welcome and highly appreciate contributions to the
 InternetSpeedVisualizer project! Your creative ideas and diligent work can make
 a real difference in its development and enhance the user experience.
 
 Multiple ways to contribute:
```

