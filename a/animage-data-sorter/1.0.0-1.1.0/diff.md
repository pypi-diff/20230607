# Comparing `tmp/animage-data_sorter-1.0.0.tar.gz` & `tmp/animage-data_sorter-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\animage-data_sorter-1.0.0.tar", last modified: Wed May 31 06:58:01 2023, max compression
+gzip compressed data, was "dist\animage-data_sorter-1.1.0.tar", last modified: Wed Jun  7 06:25:49 2023, max compression
```

## Comparing `animage-data_sorter-1.0.0.tar` & `animage-data_sorter-1.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/
--rw-rw-rw-   0        0        0     1363 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/animage_data_sorter.egg-info/
--rw-rw-rw-   0        0        0     1363 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/animage_data_sorter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1347 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/animage_data_sorter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/animage_data_sorter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/animage_data_sorter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/data_sorter/
--rw-rw-rw-   0        0        0      628 2023-05-31 06:43:16.000000 animage-data_sorter-1.0.0/data_sorter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/data_sorter/old/
--rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageASLUtility.py
--rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDCMUtility.py
--rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorter.py
--rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterGEeASL7.py
--rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterGEpCASL13.py
--rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterMISC.py
--rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterPhilips13.py
--rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemens4.py
--rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemens5.py
--rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemensPASL.py
--rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
--rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterUtility.py
--rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.0.0/data_sorter/old/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/data_sorter/restructure/
--rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.0.0/data_sorter/restructure/__init__.py
--rw-rw-rw-   0        0        0    36865 2023-05-31 06:33:34.000000 animage-data_sorter-1.0.0/data_sorter/restructure/_dicom.py
--rw-rw-rw-   0        0        0     9885 2023-05-16 02:58:30.000000 animage-data_sorter-1.0.0/data_sorter/restructure/_dicom_util.py
--rw-rw-rw-   0        0        0     3833 2023-05-16 01:45:10.000000 animage-data_sorter-1.0.0/data_sorter/restructure/_type.py
--rw-rw-rw-   0        0        0     4279 2023-05-29 05:21:20.000000 animage-data_sorter-1.0.0/data_sorter/restructure/data_sorter_base.py
--rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.0.0/data_sorter/restructure/dcm2nifti.py
--rw-rw-rw-   0        0        0     3515 2023-05-17 05:44:59.000000 animage-data_sorter-1.0.0/data_sorter/restructure/errors.py
--rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.0.0/data_sorter/restructure/ge_3d_pcasl.py
--rw-rw-rw-   0        0        0     8516 2023-05-29 05:23:17.000000 animage-data_sorter-1.0.0/data_sorter/restructure/ge_easl.py
--rw-rw-rw-   0        0        0     9418 2023-05-17 06:20:12.000000 animage-data_sorter-1.0.0/data_sorter/restructure/noASL_MRI.py
--rw-rw-rw-   0        0        0     4431 2023-05-30 02:25:25.000000 animage-data_sorter-1.0.0/data_sorter/restructure/philips_3d_pcasl.py
--rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.0.0/data_sorter/restructure/siemens_3d_pasl.py
--rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.0.0/data_sorter/restructure/siemens_3d_pcasl.py
--rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.0.0/data_sorter/restructure/siemens_3d_pcasl_old.py
--rw-rw-rw-   0        0        0     4421 2023-05-16 01:48:06.000000 animage-data_sorter-1.0.0/data_sorter/restructure/uih_3d_pasl.py
--rw-rw-rw-   0        0        0       42 2023-05-31 06:58:01.000000 animage-data_sorter-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-05-31 06:54:05.000000 animage-data_sorter-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:25:49.000000 animage-data_sorter-1.1.0/
+-rw-rw-rw-   0        0        0     1363 2023-06-07 06:25:49.000000 animage-data_sorter-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-05-11 05:19:09.000000 animage-data_sorter-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 06:25:48.000000 animage-data_sorter-1.1.0/animage_data_sorter.egg-info/
+-rw-rw-rw-   0        0        0     1363 2023-06-07 06:25:48.000000 animage-data_sorter-1.1.0/animage_data_sorter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2023-06-07 06:25:48.000000 animage-data_sorter-1.1.0/animage_data_sorter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 06:25:48.000000 animage-data_sorter-1.1.0/animage_data_sorter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-07 06:25:48.000000 animage-data_sorter-1.1.0/animage_data_sorter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 06:25:48.000000 animage-data_sorter-1.1.0/data_sorter/
+-rw-rw-rw-   0        0        0      630 2023-05-31 06:58:45.000000 animage-data_sorter-1.1.0/data_sorter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:25:49.000000 animage-data_sorter-1.1.0/data_sorter/old/
+-rw-rw-rw-   0        0        0    23325 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageASLUtility.py
+-rw-rw-rw-   0        0        0     7768 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDCMUtility.py
+-rw-rw-rw-   0        0        0    26840 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorter.py
+-rw-rw-rw-   0        0        0     9852 2023-02-08 06:54:39.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterGEeASL7.py
+-rw-rw-rw-   0        0        0     9373 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterGEpCASL13.py
+-rw-rw-rw-   0        0        0     4348 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterMISC.py
+-rw-rw-rw-   0        0        0     5901 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterPhilips13.py
+-rw-rw-rw-   0        0        0    13115 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemens4.py
+-rw-rw-rw-   0        0        0    12711 2022-11-17 03:53:33.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemens5.py
+-rw-rw-rw-   0        0        0    12032 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemensPASL.py
+-rw-rw-rw-   0        0        0    21838 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemens_UCLA.py
+-rw-rw-rw-   0        0        0    11395 2022-11-03 04:01:31.000000 animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterUtility.py
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:57:47.000000 animage-data_sorter-1.1.0/data_sorter/old/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 06:25:49.000000 animage-data_sorter-1.1.0/data_sorter/restructure/
+-rw-rw-rw-   0        0        0     5204 2023-05-16 02:45:03.000000 animage-data_sorter-1.1.0/data_sorter/restructure/__init__.py
+-rw-rw-rw-   0        0        0    36871 2023-06-07 06:19:04.000000 animage-data_sorter-1.1.0/data_sorter/restructure/_dicom.py
+-rw-rw-rw-   0        0        0     9885 2023-05-16 02:58:30.000000 animage-data_sorter-1.1.0/data_sorter/restructure/_dicom_util.py
+-rw-rw-rw-   0        0        0     3833 2023-05-16 01:45:10.000000 animage-data_sorter-1.1.0/data_sorter/restructure/_type.py
+-rw-rw-rw-   0        0        0     4279 2023-05-29 05:21:20.000000 animage-data_sorter-1.1.0/data_sorter/restructure/data_sorter_base.py
+-rw-rw-rw-   0        0        0     7621 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.0/data_sorter/restructure/dcm2nifti.py
+-rw-rw-rw-   0        0        0     3515 2023-05-17 05:44:59.000000 animage-data_sorter-1.1.0/data_sorter/restructure/errors.py
+-rw-rw-rw-   0        0        0     5737 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.0/data_sorter/restructure/ge_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8516 2023-05-29 05:23:17.000000 animage-data_sorter-1.1.0/data_sorter/restructure/ge_easl.py
+-rw-rw-rw-   0        0        0    10501 2023-06-02 03:26:56.000000 animage-data_sorter-1.1.0/data_sorter/restructure/noASL_MRI.py
+-rw-rw-rw-   0        0        0     4431 2023-05-30 02:25:25.000000 animage-data_sorter-1.1.0/data_sorter/restructure/philips_3d_pcasl.py
+-rw-rw-rw-   0        0        0     6769 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.0/data_sorter/restructure/siemens_3d_pasl.py
+-rw-rw-rw-   0        0        0     7951 2023-05-31 02:53:56.000000 animage-data_sorter-1.1.0/data_sorter/restructure/siemens_3d_pcasl.py
+-rw-rw-rw-   0        0        0     8366 2023-05-16 01:42:26.000000 animage-data_sorter-1.1.0/data_sorter/restructure/siemens_3d_pcasl_old.py
+-rw-rw-rw-   0        0        0     4421 2023-05-16 01:48:06.000000 animage-data_sorter-1.1.0/data_sorter/restructure/uih_3d_pasl.py
+-rw-rw-rw-   0        0        0       42 2023-06-07 06:25:49.000000 animage-data_sorter-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      602 2023-06-07 06:20:03.000000 animage-data_sorter-1.1.0/setup.py
```

### Comparing `animage-data_sorter-1.0.0/PKG-INFO` & `animage-data_sorter-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data_sorter
-Version: 1.0.0
+Version: 1.1.0
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.0.0/README.md` & `animage-data_sorter-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/animage_data_sorter.egg-info/PKG-INFO` & `animage-data_sorter-1.1.0/animage_data_sorter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animage-data-sorter
-Version: 1.0.0
+Version: 1.1.0
 Summary: dicom sort
 Home-page: https://gitee.com/AnImage-Beijing/data_sorter
 Author: zhaomy
 Author-email: zhaomy@an-image.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `animage-data_sorter-1.0.0/animage_data_sorter.egg-info/SOURCES.txt` & `animage-data_sorter-1.1.0/animage_data_sorter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/__init__.py` & `animage-data_sorter-1.1.0/data_sorter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 from .old.AnImageDataSorter import ImageDataSort as ImageDataSort1
 from .restructure import ImageDataSort as ImageDataSort2
 
 def ImageDataSort(raw_folder, output_path, delay_time, delay_rep, label_dur, pasl_extra_factor, is_restructure=False,
                   calc_c_cbf=False):
     if is_restructure:
         return ImageDataSort2(raw_folder, output_path, delay_time, delay_rep, label_dur, pasl_extra_factor, calc_c_cbf=calc_c_cbf)
```

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageASLUtility.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageASLUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDCMUtility.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDCMUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorter.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorter.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterGEeASL7.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterGEeASL7.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterGEpCASL13.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterGEpCASL13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterMISC.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterMISC.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterPhilips13.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterPhilips13.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemens4.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemens4.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemens5.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemens5.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemensPASL.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemensPASL.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterSiemens_UCLA.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterSiemens_UCLA.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/old/AnImageDataSorterUtility.py` & `animage-data_sorter-1.1.0/data_sorter/old/AnImageDataSorterUtility.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/__init__.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/__init__.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/_dicom.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/_dicom.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         self.SeriesNumber = self.get_key((0x0020, 0x0011), dataset, '')
 
         # 设备信息
         self.Manufacturer = MANUFACTURER.str2MANUFACTURER(self.get_key((0x0008, 0x0070), dataset))
         self.ManufacturerModelName = self.get_key((0x0008, 0x1090), dataset, UnKnown)
         self.Modality = MODALITY.str2MODALITY(self.get_key((0x0008, 0x0060), dataset))
         self.InstitutionName = self.get_key((0x0008, 0x0080), dataset, '')
-        self.ProtocolName = self.get_key((0x0018, 0x1030), dataset)
+        self.ProtocolName = self.get_key((0x0018, 0x1030), dataset, '')
 
         # 序列名
         self.PulseSequenceName = self.get_key((0x0018, 0x9005), dataset, '')
         self.SamplesPerPixel = self.get_key((0x0028, 0x0002), dataset, 1)
         if self.SamplesPerPixel != 1:
             # 不是原始的灰度图像忽略即可
             raise PhotometricRGBError()
@@ -701,15 +701,15 @@
             except InvalidDicomError:
                 logger.debug(f'忽略文件：{abs_fn}')
                 continue
             except PhotometricRGBError:
                 logger.debug(f'忽略彩色图像：{abs_fn}')
                 continue
             except Exception as e:
-                logger.warning(f'{e}：{abs_fn}')
+                logger.exception(f'{e}：{abs_fn}')
                 continue
             if ds_tags.StudyInstanceUID not in study_list:
                 study_list[ds_tags.StudyInstanceUID] = {}
             if ds_tags.SeriesInstanceUID not in study_list[ds_tags.StudyInstanceUID]:
                 study_list[ds_tags.StudyInstanceUID][ds_tags.SeriesInstanceUID] = SeriesModel(ds_tags, ds)
             study_list[ds_tags.StudyInstanceUID][ds_tags.SeriesInstanceUID].append(ds_tags)
```

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/_dicom_util.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/_dicom_util.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/_type.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/_type.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/data_sorter_base.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/data_sorter_base.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/dcm2nifti.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/dcm2nifti.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/errors.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/errors.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/ge_3d_pcasl.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/ge_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/ge_easl.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/ge_easl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/noASL_MRI.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/noASL_MRI.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+import numpy
+import numpy as np
 import pydicom
 
 from log import logger
 
 from ._dicom import SeriesModel, DicomRequiredTags
 from ._dicom_util import write_dicom_series
 from .data_sorter_base import DataSorterBase
@@ -112,34 +114,35 @@
         self.series_list = self.DWI_list + self.ADC_list
 
     def validate_series(self):
         if len(self.DWI_list) < 1:
             raise MissingSequenceError('DWI')
         elif len(self.DWI_list) > 1:
             logger.warning(f'发现{len(self.DWI_list)}组DWI数据')
+        else:
+            self.DWI = self.DWI_list[0]
 
         if len(self.ADC_list) < 1:
-            raise MissingSequenceError('ADC')
+            logger.warning(f'未发现ADC序列')
+            self.ADC: SeriesModel = None
+            # raise MissingSequenceError('ADC')
         elif len(self.ADC_list) > 1:
             logger.warning(f'发现{len(self.DWI_list)}组ADC数据')
+        else:
+            self.ADC = self.ADC_list[0]
 
-        self.DWI = self.DWI_list[0]
-        self.ADC = self.ADC_list[0]
+        if self.ADC is not None and self.DWI.SliceNumber != self.ADC.SliceNumber:
+            raise SpaceIsDifferentError('DWI', 'ADC')
+        if self.ADC is not None and (self.DWI.Repetition != 2 or self.ADC.Repetition != 1):
+            raise SliceLessError(self.ADC.SliceNumber)
 
     def Sorter(self):
         super(DataSorterDWI, self).Sorter()
-
         self.validate_series()
 
-        if self.DWI.SliceNumber != self.ADC.SliceNumber:
-            raise SpaceIsDifferentError('DWI', 'ADC')
-
-        if self.DWI.Repetition != 2 or self.ADC.Repetition != 1:
-            raise SliceLessError(self.ADC.SliceNumber)
-
         # DWI需要包含B0与B1000
         # 标准dicom中的B值(弥散系数)标签信息
         second_slice_number = 1 if self.DWI.is_second_arrangement_mode else self.DWI.SliceNumber
 
         def get_tag(dcm_obj: Union[DicomRequiredTags, pydicom.Dataset], key, default=None):
             if isinstance(dcm_obj, DicomRequiredTags):
                 return dcm_obj.get_tag(key, default=default)
@@ -188,19 +191,35 @@
                            os.path.join(self.output_root, 'dwi', f'b{first_b_value}'))
         cur_series_number += 1
         write_dicom_series(DWI_img[...,1], self.DWI, f'dwi-b{second_b_value}', cur_series_number,
                                os.path.join(self.output_root, 'dwi', f'b{second_b_value}'))
 
         cur_series_number += 1
         rescale_type = '10^-6 mm^2/s'
-        # ADC， 确定单位
-        rescale_type_1 = self.ADC.get_tag((0x0028, 0x1054), '')
-        rescale_type_2 = self.ADC.get_tag((0x2005, 0x140B), '')
-        if rescale_type_1 != '':
-            rescale_type = rescale_type_1
-        elif rescale_type_2 != '':
-            rescale_type = rescale_type_2
-
-        rescale = 1000 if rescale_type == '10^-3 mm^2/s' else 1
-        ADC_img = self.ADC.load(rescale)
-        write_dicom_series(ADC_img[...,0], self.DWI, f'dwi-adc', cur_series_number,
-                           os.path.join(self.output_root, 'dwi', f'adc'))
+        if self.ADC is not None:
+            # ADC， 确定单位
+            rescale_type_1 = self.ADC.get_tag((0x0028, 0x1054), '')
+            rescale_type_2 = self.ADC.get_tag((0x2005, 0x140B), '')
+            if rescale_type_1 != '':
+                rescale_type = rescale_type_1
+            elif rescale_type_2 != '':
+                rescale_type = rescale_type_2
+
+            rescale = 1000 if rescale_type == '10^-3 mm^2/s' else 1
+            ADC_img = self.ADC.load(rescale)[...,0]
+            write_dicom_series(ADC_img, self.DWI, 'dwi-adc', cur_series_number,
+                               os.path.join(self.output_root, 'dwi', 'adc'))
+
+        else:
+            logger.debug(f'开始计算ADC')
+            # 使second_b_value等于较大B值的那个图像
+            first_b0_idx, second_b1_idx = 0, 1
+            if first_b_value > second_b_value:
+                first_b_value, second_b_value = second_b_value, first_b_value
+                first_b0_idx, second_b1_idx = second_b1_idx, first_b0_idx
+            ADC_img = np.log(DWI_img[...,first_b0_idx] / DWI_img[...,second_b1_idx]) / (second_b_value - first_b_value)
+            ADC_img[np.isinf(ADC_img) | np.isnan(ADC_img)] = 0
+            ADC_img *= 10**6
+            ADC_img[ADC_img < 0] = -256
+
+            write_dicom_series(ADC_img, self.DWI, 'dwi-adc', cur_series_number,
+                               os.path.join(self.output_root, 'dwi', 'adc'))
```

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/philips_3d_pcasl.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/philips_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/siemens_3d_pasl.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/siemens_3d_pasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/siemens_3d_pcasl.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/siemens_3d_pcasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/siemens_3d_pcasl_old.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/siemens_3d_pcasl_old.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/data_sorter/restructure/uih_3d_pasl.py` & `animage-data_sorter-1.1.0/data_sorter/restructure/uih_3d_pasl.py`

 * *Files identical despite different names*

### Comparing `animage-data_sorter-1.0.0/setup.py` & `animage-data_sorter-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="animage-data_sorter",
-  version="1.0.0",
+  version="1.1.0",
   author="zhaomy",
   author_email="zhaomy@an-image.cn",
   description="dicom sort",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://gitee.com/AnImage-Beijing/data_sorter",
   packages=setuptools.find_packages(),
```

