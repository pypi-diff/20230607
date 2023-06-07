# Comparing `tmp/frankAllSkyCam-8.1.tar.gz` & `tmp/frankAllSkyCam-8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-8.1.tar", last modified: Wed Jun  7 19:17:52 2023, max compression
+gzip compressed data, was "frankAllSkyCam-8.2.tar", last modified: Wed Jun  7 21:14:45 2023, max compression
```

## Comparing `frankAllSkyCam-8.1.tar` & `frankAllSkyCam-8.2.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 19:17:52.315729 frankAllSkyCam-8.1/
--rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-07 19:17:52.315729 frankAllSkyCam-8.1/PKG-INFO
--rwxr--r--   0 pi        (1000) pi        (1000)     3200 2023-06-07 19:09:34.000000 frankAllSkyCam-8.1/README.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 19:17:52.315729 frankAllSkyCam-8.1/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-07 19:17:11.000000 frankAllSkyCam-8.1/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     5402 2023-06-07 19:05:59.000000 frankAllSkyCam-8.1/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3445 2023-06-07 19:06:39.000000 frankAllSkyCam-8.1/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/drawtext.py
--rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/exposurecalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/fileManager.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/getextdata.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/index.py
--rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/sqmexp.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/sqmreader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.000000 frankAllSkyCam-8.1/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 12:39:31.000000 frankAllSkyCam-8.1/frankAllSkyCam/watchDog.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 19:17:52.315729 frankAllSkyCam-8.1/frankAllSkyCam.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-07 19:17:52.000000 frankAllSkyCam-8.1/frankAllSkyCam.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      722 2023-06-07 19:17:52.000000 frankAllSkyCam-8.1/frankAllSkyCam.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-07 19:17:52.000000 frankAllSkyCam-8.1/frankAllSkyCam.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       18 2023-06-07 19:17:52.000000 frankAllSkyCam-8.1/frankAllSkyCam.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-07 19:17:52.000000 frankAllSkyCam-8.1/frankAllSkyCam.egg-info/top_level.txt
--rwxrw-rw-   0 pi        (1000) pi        (1000)       79 2023-06-07 19:17:52.319729 frankAllSkyCam-8.1/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-07 19:17:02.000000 frankAllSkyCam-8.1/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/
+-rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/PKG-INFO
+-rwxr--r--   0 pi        (1000) pi        (1000)     3200 2023-06-07 19:09:34.000000 frankAllSkyCam-8.2/README.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-07 21:14:12.000000 frankAllSkyCam-8.2/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     6068 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3877 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/drawtext.py
+-rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/exposurecalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/fileManager.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/getextdata.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/index.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1295 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/logos.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/sqmexp.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/sqmreader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.000000 frankAllSkyCam-8.2/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 21:13:55.000000 frankAllSkyCam-8.2/frankAllSkyCam/watchDog.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 21:14:45.642027 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      860 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      746 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       18 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       15 2023-06-07 21:14:45.000000 frankAllSkyCam-8.2/frankAllSkyCam.egg-info/top_level.txt
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       79 2023-06-07 21:14:45.646027 frankAllSkyCam-8.2/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-07 21:14:28.000000 frankAllSkyCam-8.2/setup.py
```

### Comparing `frankAllSkyCam-8.1/PKG-INFO` & `frankAllSkyCam-8.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: frankAllSkyCam
-Version: 8.1
+Version: 8.2
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.1.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.2.tar.gz
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
 Keywords: AllSkyCamera,Astronomy,AllSky
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `frankAllSkyCam-8.1/README.txt` & `frankAllSkyCam-8.2/README.txt`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/__main__.py` & `frankAllSkyCam-8.2/frankAllSkyCam/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import datetime
 from fractions import Fraction
 import time
 from pytz import timezone
 from importlib import resources  # Python 3.7+
 from configparser import ConfigParser
-from frankAllSkyCam import imageHeader, fileManager, drawtext, getextdata
+from frankAllSkyCam import imageHeader, fileManager, drawtext, getextdata, logos
 
 config = ConfigParser()
 configFileName = fileManager.getConfigFileName()
 config.read(configFileName)
 appPath = os.path.expanduser("~") + "/frankAllSkyCam/"
 
 time_zone = str(config['site']['time_zone'])
@@ -57,14 +57,23 @@
 et_y_pos       = int(config['extra_text']['et_y_pos'])
 et_font_size   = int(config['extra_text']['et_font_size'])
 et_font_colorR = int(config['extra_text']['et_font_colorR'])
 et_font_colorG = int(config['extra_text']['et_font_colorG'])
 et_font_colorB = int(config['extra_text']['et_font_colorB'])
 et_font_color = [et_font_colorR,et_font_colorG,et_font_colorB]
 
+compass_filename = str(config['compass']['compass_filename'])
+compass_x_pos = int(config['compass']['compass_x_pos'])
+compass_y_pos = int(config['compass']['compass_y_pos'])
+compass_rot_angle = int(config['compass']['compass_rot_angle'])
+
+logo_filename = str(config['logo']['logo_filename'])
+logo_x_pos = int(config['logo']['logo_x_pos'])
+logo_y_pos = int(config['logo']['logo_y_pos'])
+
 sqm_le = config['sqm']['use_sqm_le']
 
 isFTP = str(config['ftp']['isFTP'])=='True'
 FTP_server = str(config['ftp']['FTP_server'])
 FTP_login = str(config['ftp']['FTP_login'])
 FTP_pass = str(config['ftp']['FTP_pass'])
 FTP_uploadFolder = str(config['ftp']['FTP_uploadFolder'])
@@ -125,14 +134,20 @@
           #extra_text needed
           extra_string = getextdata.getData()
           extra_text = [extra_string, et_font_size, et_font_color, et_x_pos, et_y_pos]
 
        # print watermark
        drawtext.printWatermark(s, jpg_file_name, font_size, font_color, sqm_le, rotation, text_positions, extra_text)
 
+       if logo_filename != "" or compass_filename != "":
+          print(logo_filename)
+          print(compass_filename)
+
+          logos.imagePaste(jpg_file_name, compass_filename, compass_x_pos, compass_y_pos, compass_rot_angle, logo_filename, logo_x_pos, logo_y_pos)
+
        #generate /update alive.txt to say we are still alive
        textcommand = "touch " + logFolder +  "/alive.txt"
        os.system(textcommand)
 
        pass
     except:
        print("ERROR: " + str(sys.exc_info()[0]))
```

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-8.2/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/config.py` & `frankAllSkyCam-8.2/frankAllSkyCam/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,14 +94,30 @@
 et_font_size = 18
 et_font_colorR = 0
 et_font_colorG = 255
 et_font_colorB = 255
 et_x_pos = 5
 et_y_pos = 80
 
+[compass]
+# relative path from frankAllSkyCam
+# if file not found, it will be skipped
+# set your coords according to your resolution
+compass_filename = compass.png
+compass_x_pos = 900
+compass_y_pos = 580
+compass_rot_angle = 20
+
+[logo]
+# relative path from frankAllSkyCam
+# if file not found, it will be skipped
+# set your coords according to your resolution
+logo_filename = logo.png
+logo_x_pos = 30
+logo_y_pos = 580
 
 [exposure]
 # max night exposure in seconds
 #  for urban sky, suggested value is 4
 #  for dark sky, suggested value is 55-60 (I found 55 secs ok for sqm 21,3).
 #  this value only limits the max exposure. The calculated or real SQM will drive exposure
 esp_secs =60
```

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/crontab.py` & `frankAllSkyCam-8.2/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-8.2/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/exposurecalc.py` & `frankAllSkyCam-8.2/frankAllSkyCam/exposurecalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-8.2/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/getextdata.py` & `frankAllSkyCam-8.2/frankAllSkyCam/getextdata.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-8.2/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/sqmreader.py` & `frankAllSkyCam-8.2/frankAllSkyCam/sqmreader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/startrail.py` & `frankAllSkyCam-8.2/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-8.2/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-8.2/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-8.2/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-8.2/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam.egg-info/PKG-INFO` & `frankAllSkyCam-8.2/frankAllSkyCam.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: frankAllSkyCam
-Version: 8.1
+Version: 8.2
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.1.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.2.tar.gz
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
 Keywords: AllSkyCamera,Astronomy,AllSky
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `frankAllSkyCam-8.1/frankAllSkyCam.egg-info/SOURCES.txt` & `frankAllSkyCam-8.2/frankAllSkyCam.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 frankAllSkyCam/crontab.py
 frankAllSkyCam/drawtext.py
 frankAllSkyCam/exposurecalc.py
 frankAllSkyCam/fileManager.py
 frankAllSkyCam/getextdata.py
 frankAllSkyCam/imageHeader.py
 frankAllSkyCam/index.py
+frankAllSkyCam/logos.py
 frankAllSkyCam/sqmexp.py
 frankAllSkyCam/sqmreader.py
 frankAllSkyCam/startrail.py
 frankAllSkyCam/suncalc2.py
 frankAllSkyCam/test_suncalc.py
 frankAllSkyCam/timelapse.py
 frankAllSkyCam/watchDog.py
```

### Comparing `frankAllSkyCam-8.1/setup.py` & `frankAllSkyCam-8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'frankAllSkyCam',
   packages = ['frankAllSkyCam'],
-  version = '8.1',
+  version = '8.2',
   license='MIT',
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',
   author = 'Francesco Sferlazza',
   author_email = 'sferlazza@gmail.com',
   url = 'https://github.com/sferlix/frankAllSkyCam',
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.1.tar.gz',
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/8.2.tar.gz',
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],
   install_requires=[
           'pytz',
           'numpy',
           'pandas',
       ],
   classifiers=[
```

