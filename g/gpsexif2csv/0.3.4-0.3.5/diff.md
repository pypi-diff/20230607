# Comparing `tmp/gpsexif2csv-0.3.4.tar.gz` & `tmp/gpsexif2csv-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpsexif2csv-0.3.4.tar", max compression
+gzip compressed data, was "gpsexif2csv-0.3.5.tar", max compression
```

## Comparing `gpsexif2csv-0.3.4.tar` & `gpsexif2csv-0.3.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-03-21 16:57:10.719000 gpsexif2csv-0.3.4/gpsexif2csv/__init__.py
--rw-r--r--   0        0        0     3917 2023-03-21 16:57:10.720790 gpsexif2csv-0.3.4/gpsexif2csv/main.py
--rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 gpsexif2csv-0.3.4/LICENSE
--rw-r--r--   0        0        0      524 2023-03-21 17:21:55.812575 gpsexif2csv-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      727 2023-03-21 17:10:32.256950 gpsexif2csv-0.3.4/README.md
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 gpsexif2csv-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-21 16:57:10.719000 gpsexif2csv-0.3.5/gpsexif2csv/__init__.py
+-rw-r--r--   0        0        0     3886 2023-06-07 21:16:06.101865 gpsexif2csv-0.3.5/gpsexif2csv/main.py
+-rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 gpsexif2csv-0.3.5/LICENSE
+-rw-r--r--   0        0        0      524 2023-06-07 21:18:46.588456 gpsexif2csv-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      727 2023-03-21 17:10:32.256950 gpsexif2csv-0.3.5/README.md
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 gpsexif2csv-0.3.5/PKG-INFO
```

### Comparing `gpsexif2csv-0.3.4/gpsexif2csv/main.py` & `gpsexif2csv-0.3.5/gpsexif2csv/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                     gps_latitude = -gps_latitude
                 logger.debug(f"gps_info['GPSLongitude']: {gps_info['GPSLongitude']}")
                 gps_longitude = convert_to_degrees(gps_info['GPSLongitude'])
                 gps_longitude_ref = gps_info['GPSLongitudeRef']
                 if gps_longitude_ref == 'W':
                     gps_longitude = -gps_longitude
                 image_path = Path(image)
-                path = str(image_path.parent.name) + '/' + str(image_path.name)
+                path = str(image_path.resolve())
                 writer.writerow(
                     {'Path': path, 'Latitude': gps_latitude, 'Longitude': gps_longitude})
                 total += 1
         print(f"Processed {total} things.")
 
 # main function to find all JPEG images in a directory and its subdirectories and write the point geometry file
 @app.command()
```

### Comparing `gpsexif2csv-0.3.4/LICENSE` & `gpsexif2csv-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpsexif2csv-0.3.4/pyproject.toml` & `gpsexif2csv-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpsexif2csv"
-version = "0.3.4"
+version = "0.3.5"
 description = "Extract EXIF GPS data into CSV"
 authors = ["João Fauvel <jmmfauvel@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `gpsexif2csv-0.3.4/README.md` & `gpsexif2csv-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `gpsexif2csv-0.3.4/PKG-INFO` & `gpsexif2csv-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpsexif2csv
-Version: 0.3.4
+Version: 0.3.5
 Summary: Extract EXIF GPS data into CSV
 License: GPL-3.0-or-later
 Author: João Fauvel
 Author-email: jmmfauvel@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

