# Comparing `tmp/visuallayer-0.0.12-py3.9-none-any.whl.zip` & `tmp/visuallayer-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 19386 bytes, number of entries: 19
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 06:40 visuallayer/__init__.py
--rw-r--r--  2.0 unx     4940 b- defN 23-Jun-07 06:40 visuallayer/sentry.py
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-07 06:40 visuallayer/datasets/__init__.py
--rw-r--r--  2.0 unx     4483 b- defN 23-Jun-07 06:40 visuallayer/datasets/clean_torchvision_oxford_iiit_pet.py
--rw-r--r--  2.0 unx      942 b- defN 23-Jun-07 06:40 visuallayer/datasets/dataset.py
--rw-r--r--  2.0 unx     2349 b- defN 23-Jun-07 06:40 visuallayer/datasets/image_folder.py
--rw-r--r--  2.0 unx     2765 b- defN 23-Jun-07 06:40 visuallayer/datasets/vl_cocodetection.py
--rw-r--r--  2.0 unx     3733 b- defN 23-Jun-07 06:40 visuallayer/datasets/vl_food101.py
--rw-r--r--  2.0 unx     1887 b- defN 23-Jun-07 06:40 visuallayer/datasets/vl_imagenet.py
--rw-r--r--  2.0 unx     3397 b- defN 23-Jun-07 06:40 visuallayer/datasets/vl_kitti.py
--rw-r--r--  2.0 unx     1139 b- defN 23-Jun-07 06:40 visuallayer/datasets/vl_parse_exclude_csv.py
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-07 06:40 visuallayer/datasets/zoo/__init__.py
--rw-r--r--  2.0 unx      644 b- defN 23-Jun-07 06:40 visuallayer/datasets/zoo/utils.py
--rw-r--r--  2.0 unx     6000 b- defN 23-Jun-07 06:40 visuallayer/datasets/zoo/vl_oxford_iiit.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-07 06:41 visuallayer-0.0.12.dist-info/LICENSE
--rw-r--r--  2.0 unx      864 b- defN 23-Jun-07 06:41 visuallayer-0.0.12.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 23-Jun-07 06:41 visuallayer-0.0.12.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-07 06:41 visuallayer-0.0.12.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1698 b- defN 23-Jun-07 06:41 visuallayer-0.0.12.dist-info/RECORD
-19 files, 46511 bytes uncompressed, 16560 bytes compressed:  64.4%
+Zip file size: 19191 bytes, number of entries: 19
+-rw-rw-r--  2.0 unx       91 b- defN 23-Jun-05 11:41 visuallayer/__init__.py
+-rw-rw-r--  2.0 unx     4940 b- defN 23-Jun-05 04:57 visuallayer/sentry.py
+-rw-rw-r--  2.0 unx       19 b- defN 23-Jun-05 11:52 visuallayer/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4483 b- defN 23-Jun-05 07:53 visuallayer/datasets/clean_torchvision_oxford_iiit_pet.py
+-rw-rw-r--  2.0 unx      942 b- defN 23-Jun-06 09:31 visuallayer/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2349 b- defN 23-Jun-05 05:02 visuallayer/datasets/image_folder.py
+-rw-rw-r--  2.0 unx     2765 b- defN 23-Jun-05 04:57 visuallayer/datasets/vl_cocodetection.py
+-rw-rw-r--  2.0 unx     3733 b- defN 23-Jun-05 04:57 visuallayer/datasets/vl_food101.py
+-rw-rw-r--  2.0 unx     1887 b- defN 23-May-31 05:01 visuallayer/datasets/vl_imagenet.py
+-rw-rw-r--  2.0 unx     3397 b- defN 23-Jun-05 04:57 visuallayer/datasets/vl_kitti.py
+-rw-rw-r--  2.0 unx     1139 b- defN 23-May-30 04:29 visuallayer/datasets/vl_parse_exclude_csv.py
+-rw-rw-r--  2.0 unx       82 b- defN 23-Jun-06 02:56 visuallayer/datasets/zoo/__init__.py
+-rw-rw-r--  2.0 unx      646 b- defN 23-Jun-07 03:50 visuallayer/datasets/zoo/utils.py
+-rw-rw-r--  2.0 unx     5413 b- defN 23-Jun-07 04:21 visuallayer/datasets/zoo/vl_oxford_iiit.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-07 05:33 visuallayer-0.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      821 b- defN 23-Jun-07 05:33 visuallayer-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 05:33 visuallayer-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jun-07 05:33 visuallayer-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1692 b- defN 23-Jun-07 05:33 visuallayer-0.0.2.dist-info/RECORD
+19 files, 45860 bytes uncompressed, 16375 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: visuallayer/datasets/zoo/utils.py
 Comment: 
 
 Filename: visuallayer/datasets/zoo/vl_oxford_iiit.py
 Comment: 
 
-Filename: visuallayer-0.0.12.dist-info/LICENSE
+Filename: visuallayer-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: visuallayer-0.0.12.dist-info/METADATA
+Filename: visuallayer-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: visuallayer-0.0.12.dist-info/WHEEL
+Filename: visuallayer-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: visuallayer-0.0.12.dist-info/top_level.txt
+Filename: visuallayer-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: visuallayer-0.0.12.dist-info/RECORD
+Filename: visuallayer-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## visuallayer/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = '0.0.12'
+__version__ = '0.0.1'
 from .datasets import *
 from .sentry import init_sentry
 init_sentry()
```

## visuallayer/datasets/zoo/utils.py

```diff
@@ -14,10 +14,10 @@
 def list_datasets():
     names = get_dataset_names()
     print("Listing all datasets in zoo.")
     return names
 
 
 def get_dataset_names():
-    datasets = [VLOxfordIIITPet]
+    datasets = [VLOxfordIIITPet()]
     datasets_names = [dataset.name for dataset in datasets]
     return datasets_names
```

## visuallayer/datasets/zoo/vl_oxford_iiit.py

```diff
@@ -17,18 +17,14 @@
     homepage_url: str = "https://www.robots.ox.ac.uk/~vgg/data/pets/"
     license: str = (
         "Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)"
     )
     description: str = "A modified version of the original Oxford IIIT Pets Dataset removing dataset issues."
     num_images: int = 7349
 
-    # Hack: Download the dataset in the current dir
-    def __post_init__(self):
-        OxfordIIITPet(root="./", download=True)
-
     @property
     def num_images_with_issues(self) -> int:
         df = pd.read_csv(self.filelist_csv_url)
         return len(df["filename"].unique())
 
     @property
     def info(self) -> None:
@@ -111,31 +107,20 @@
             )
 
     def export_issues(self, filename: str) -> None:
         df = pd.read_csv(self.issue_count_csv_url)
         df.to_csv(filename, index=False)
 
     def explore(self):
-        import base64
-
         def to_img_tag(path):
             if isinstance(path, str):
-                with open(path, 'rb') as f:
-                    image_data = f.read()
-                    base64_image = base64.b64encode(image_data).decode('utf-8')
-                return '<img src="data:image/png;base64,' + base64_image + '" width="150" >'
+                return '<img src="' + path + '" width="150" >'
             else:
                 return path  # Return the original value if it's not a string
 
-        # def to_img_tag(path):
-        #     if isinstance(path, str):
-        #         return '<img src="' + path + '" width="150" >'
-        #     else:
-        #         return path  # Return the original value if it's not a string
-
         df = pd.read_csv(self.filelist_csv_url)
         df["filename_preview"] = df["filename"]
         df["prototype_preview"] = df["prototype"]
         df = df.loc[
             :,
             [
                 "filename",
```

## Comparing `visuallayer-0.0.12.dist-info/LICENSE` & `visuallayer-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visuallayer-0.0.12.dist-info/METADATA` & `visuallayer-0.0.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: visuallayer
-Version: 0.0.12
+Version: 0.0.2
 Summary: Open, Clean Datasets for Computer Vision.
 Home-page: https://github.com/visual-layer/vl-datasets
 Author: Visual Layer
 Author-email: info@visual-layer.com
 License: Apache-2.0
 Keywords: machine learning,computer vision,data-centric
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: pandas
 Requires-Dist: sentry-sdk
 Requires-Dist: scipy
-Requires-Dist: itables
 
 Coming soon.
-
```

## Comparing `visuallayer-0.0.12.dist-info/RECORD` & `visuallayer-0.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-visuallayer/__init__.py,sha256=yaaUjAesEsqTpywcRuC67igyhRX1oe3sR8Vl7CrcEs8,92
+visuallayer/__init__.py,sha256=ED_jsdf3kqSiifRC_8zkYY2KYLFCdgo8EY_HZwSzong,91
 visuallayer/sentry.py,sha256=AAmaO2kO8xyh9crTiq6YDnfHSJxyjorioI-Sdk2K7lc,4940
 visuallayer/datasets/__init__.py,sha256=A1TkIulArINdCJtTM1jED6HDemnZ3AlURsyVxENP2ug,19
 visuallayer/datasets/clean_torchvision_oxford_iiit_pet.py,sha256=yUwBGTFyy9FI6ct7C3hx-V9nOfywrjCasEM4TtqAT2k,4483
 visuallayer/datasets/dataset.py,sha256=Oe3eCCk5VhKn2siPXC8W6zk_cVHKMAaeXzEERhFC-ro,942
 visuallayer/datasets/image_folder.py,sha256=yT_W1RRsrxVfV2XlCniiKfaUka5k_Ly6s4X39fpP1Oc,2349
 visuallayer/datasets/vl_cocodetection.py,sha256=xwGDWoT2DRMnlnQwu3igiDUVXGNjfjfWR1tTaEpskz0,2765
 visuallayer/datasets/vl_food101.py,sha256=7bVDgxZed1FVnPDlB5BFl2mFCJwheVHLjkXodD3c08k,3733
 visuallayer/datasets/vl_imagenet.py,sha256=li6jc5qcEYHx6f4iFXGuwGycqOw_RKn5V4Zfc2REwhs,1887
 visuallayer/datasets/vl_kitti.py,sha256=aEVqgh3Akw98qmMAk-rZrMK7IZ__wOCLOeunr-FXHvM,3397
 visuallayer/datasets/vl_parse_exclude_csv.py,sha256=kUR0KlJgbJ6Elo-nvRDu9a3UOhcPfS_wr2stx8ZJg84,1139
 visuallayer/datasets/zoo/__init__.py,sha256=vRb7pVKdPoKsCpm1UzStXLtQDkk5mZ_Pxi8HxfHW-qo,82
-visuallayer/datasets/zoo/utils.py,sha256=Ndr8djNk7hgre02-LhUuUG8qJR7BQsEwOrclemTOPUE,644
-visuallayer/datasets/zoo/vl_oxford_iiit.py,sha256=rc-DZ8dkrPaju8z9B4QX8iY1Iw2TLbJIPY98Nj4QlX4,6000
-visuallayer-0.0.12.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-visuallayer-0.0.12.dist-info/METADATA,sha256=o4_SrGgkm9Fc38kocJuoVbsZno_oaUBnfDG9Doj47bw,864
-visuallayer-0.0.12.dist-info/WHEEL,sha256=YT1wPceIeW2Q5XD-ypzUqEKq0BMVsXhboTN8eU2aMIk,108
-visuallayer-0.0.12.dist-info/top_level.txt,sha256=hxebilWiIk5JiZslpQz8-F1__45rw-otTI9GwhE9Zw0,12
-visuallayer-0.0.12.dist-info/RECORD,,
+visuallayer/datasets/zoo/utils.py,sha256=gkYJPckZyC2DMTreu7IP9drxj1ye2duovRHurOpM4GQ,646
+visuallayer/datasets/zoo/vl_oxford_iiit.py,sha256=2Ba7rMEngftzhv-jXM6LDcmkWCVhfKFXqZ5Y5fQcORI,5413
+visuallayer-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+visuallayer-0.0.2.dist-info/METADATA,sha256=5G0tMasuMKpA9MgJ1xMr8YCCy8aA6LXf0Ymp6MkImvA,821
+visuallayer-0.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+visuallayer-0.0.2.dist-info/top_level.txt,sha256=hxebilWiIk5JiZslpQz8-F1__45rw-otTI9GwhE9Zw0,12
+visuallayer-0.0.2.dist-info/RECORD,,
```

