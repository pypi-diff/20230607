# Comparing `tmp/frankAllSkyCam-7.8.tar.gz` & `tmp/frankAllSkyCam-7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frankAllSkyCam-7.8.tar", last modified: Mon Jun  5 20:14:52 2023, max compression
+gzip compressed data, was "frankAllSkyCam-7.9.tar", last modified: Wed Jun  7 12:46:05 2023, max compression
```

## Comparing `frankAllSkyCam-7.8.tar` & `frankAllSkyCam-7.9.tar`

### file list

```diff
@@ -1,25 +1,23 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 20:14:52.987187 frankAllSkyCam-7.8/
--rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-06-05 20:14:52.987187 frankAllSkyCam-7.8/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-05 20:14:52.987187 frankAllSkyCam-7.8/frankAllSkyCam/
--rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-05 20:14:18.983678 frankAllSkyCam-7.8/frankAllSkyCam/__init__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     5310 2023-06-05 20:12:48.497031 frankAllSkyCam-7.8/frankAllSkyCam/__main__.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/allskycamdelete.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3389 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/config.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/crontab.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/drawtext.py
--rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/exposurecalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/fileManager.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/getextdata.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-05 20:12:48.493031 frankAllSkyCam-7.8/frankAllSkyCam/imageHeader.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-05 20:12:48.497031 frankAllSkyCam-7.8/frankAllSkyCam/index.py
--rwxr--r--   0 pi        (1000) pi        (1000)     1068 2023-06-05 20:12:48.497031 frankAllSkyCam-7.8/frankAllSkyCam/shelly_temp.py
--rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-05 20:12:48.497031 frankAllSkyCam-7.8/frankAllSkyCam/sqmexp.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-05 20:12:48.497031 frankAllSkyCam-7.8/frankAllSkyCam/sqmreader.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-05 20:12:48.497031 frankAllSkyCam-7.8/frankAllSkyCam/startrail.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-05 20:12:48.501031 frankAllSkyCam-7.8/frankAllSkyCam/suncalc2.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)      941 2023-06-05 20:12:48.501031 frankAllSkyCam-7.8/frankAllSkyCam/test_sqm.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.501031 frankAllSkyCam-7.8/frankAllSkyCam/test_suncalc.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-05 20:12:48.501031 frankAllSkyCam-7.8/frankAllSkyCam/timelapse.py
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-05 20:12:48.501031 frankAllSkyCam-7.8/frankAllSkyCam/watchDog.py
--rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-7.8/setup.cfg
--rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-05 20:14:08.471832 frankAllSkyCam-7.8/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 12:46:05.336249 frankAllSkyCam-7.9/
+-rw-r--r--   0 pi        (1000) pi        (1000)      899 2023-06-07 12:46:05.336249 frankAllSkyCam-7.9/PKG-INFO
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-07 12:46:05.336249 frankAllSkyCam-7.9/frankAllSkyCam/
+-rwxrwxrw-   0 pi        (1000) pi        (1000)       71 2023-06-07 12:42:20.509821 frankAllSkyCam-7.9/frankAllSkyCam/__init__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     5427 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/__main__.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1033 2023-06-07 12:39:31.298876 frankAllSkyCam-7.9/frankAllSkyCam/allskycamdelete.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3421 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/config.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     3491 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/crontab.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2431 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/drawtext.py
+-rw-r-xr--   0 pi        (1000) pi        (1000)     1156 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/exposurecalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3758 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/fileManager.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2823 2023-06-07 12:39:31.302876 frankAllSkyCam-7.9/frankAllSkyCam/getextdata.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     9426 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/imageHeader.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)      503 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/index.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      233 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/sqmexp.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)    16497 2023-06-07 12:39:31.306876 frankAllSkyCam-7.9/frankAllSkyCam/sqmreader.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     3082 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/startrail.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     6939 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/suncalc2.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)     2271 2023-06-05 20:12:48.501031 frankAllSkyCam-7.9/frankAllSkyCam/test_suncalc.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     4433 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/timelapse.py
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1593 2023-06-07 12:39:31.310876 frankAllSkyCam-7.9/frankAllSkyCam/watchDog.py
+-rwxrw-rw-   0 pi        (1000) pi        (1000)       65 2023-04-26 18:08:27.179909 frankAllSkyCam-7.9/setup.cfg
+-rwxrwxrw-   0 pi        (1000) pi        (1000)     1067 2023-06-07 12:41:14.390249 frankAllSkyCam-7.9/setup.py
```

### Comparing `frankAllSkyCam-7.8/PKG-INFO` & `frankAllSkyCam-7.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: frankAllSkyCam
-Version: 7.8
+Version: 7.9
 Summary: AllSkyCamera with Raspberry Pi and Pi HQ Camera 
 Home-page: https://github.com/sferlix/frankAllSkyCam
 Author: Francesco Sferlazza
 Author-email: sferlazza@gmail.com
 License: MIT
-Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.8.tar.gz
+Download-URL: https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.9.tar.gz
 Description: UNKNOWN
 Keywords: AllSkyCamera,Astronomy,AllSky
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/__main__.py` & `frankAllSkyCam-7.9/frankAllSkyCam/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 outputFolder = appPath + str(config['system']['otuputFolder'])
 outputLocalWebFile = str(config['system']['outputLocalWebFile'])
 horiz = str(config['resolution']['horiz'])
 vert = str(config['resolution']['vert'])
 rotation = int(config['resolution']['picture_rotation'])
 picture_rotation = str(config['resolution']['picture_rotation'])
 
-additional_params = str(config['libcamera']['additional_params'])
+additional_night_params = str(config['libcamera']['additional_night_params'])
+additional_day_params = str(config['libcamera']['additional_day_params'])
+
 
 font_size   = int(config['font']['font_size'])
 font_colorR = int(config['font']['font_colorR'])
 font_colorG = int(config['font']['font_colorG'])
 font_colorB = int(config['font']['font_colorB'])
 font_color = [font_colorR,font_colorG,font_colorB]
 
@@ -98,17 +100,17 @@
 
     command = "libcamera-still -n -o " + jpg_file_name
     command += " --width " + str(horiz)
     command += " --height "+ str(vert)
     command += " --immediate "
     if exposure >0:
        command +=" --shutter " + str(int(exposure)) + " "
-       command += additional_params
+       command += additional_night_params
     else:
-       command += " --metering average "
+       command += additional_day_params + " --metering average "
 
     try:
        # ensure no libcamera is operating
        killcmd = "ps -ef|grep libcamera | grep -v color|awk '{print $2}'|xargs kill -9 1> /dev/null 2>&1"
        os.system(killcmd)
        print(killcmd)
```

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/allskycamdelete.py` & `frankAllSkyCam-7.9/frankAllSkyCam/allskycamdelete.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/config.py` & `frankAllSkyCam-7.9/frankAllSkyCam/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
 vert = 600
 picture_rotation = 0
 
 [libcamera]
 # may personalize the libcamara params.
 # please DO NOT set --shutter, --immediate
 # parameters will be used only when exposure > 0
-additional_params = --gain 14 --awbgains 2.2,1.6 --contrast 1.5
+additional_night_params = --gain 14 --awbgains 2.2,1.6 --contrast 1.5
+additional_day_params = 
 
 
 [timelapse]
 # if True, timelapse from sunset to sunrise will be generated  Otherwise, not.
 nightTL = True
 
 # if True, 24h timelapse from 9am to 9am next day will be generated. Otherwise, not.
```

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/crontab.py` & `frankAllSkyCam-7.9/frankAllSkyCam/crontab.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/drawtext.py` & `frankAllSkyCam-7.9/frankAllSkyCam/drawtext.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/exposurecalc.py` & `frankAllSkyCam-7.9/frankAllSkyCam/exposurecalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/fileManager.py` & `frankAllSkyCam-7.9/frankAllSkyCam/fileManager.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/getextdata.py` & `frankAllSkyCam-7.9/frankAllSkyCam/getextdata.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/imageHeader.py` & `frankAllSkyCam-7.9/frankAllSkyCam/imageHeader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/sqmreader.py` & `frankAllSkyCam-7.9/frankAllSkyCam/sqmreader.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/startrail.py` & `frankAllSkyCam-7.9/frankAllSkyCam/startrail.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/suncalc2.py` & `frankAllSkyCam-7.9/frankAllSkyCam/suncalc2.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/test_suncalc.py` & `frankAllSkyCam-7.9/frankAllSkyCam/test_suncalc.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/timelapse.py` & `frankAllSkyCam-7.9/frankAllSkyCam/timelapse.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/frankAllSkyCam/watchDog.py` & `frankAllSkyCam-7.9/frankAllSkyCam/watchDog.py`

 * *Files identical despite different names*

### Comparing `frankAllSkyCam-7.8/setup.py` & `frankAllSkyCam-7.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'frankAllSkyCam',
   packages = ['frankAllSkyCam'],
-  version = '7.8',
+  version = '7.9',
   license='MIT',
   description = 'AllSkyCamera with Raspberry Pi and Pi HQ Camera ',
   author = 'Francesco Sferlazza',
   author_email = 'sferlazza@gmail.com',
   url = 'https://github.com/sferlix/frankAllSkyCam',
-  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.8.tar.gz',
+  download_url = 'https://github.com/sferlix/frankAllSkyCam/archive/refs/tags/7.9.tar.gz',
   keywords = ['AllSkyCamera', 'Astronomy', 'AllSky'],
   install_requires=[
           'pytz',
           'numpy',
           'pandas',
       ],
   classifiers=[
```

