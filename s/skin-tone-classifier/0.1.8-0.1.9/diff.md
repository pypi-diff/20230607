# Comparing `tmp/skin-tone-classifier-0.1.8.tar.gz` & `tmp/skin-tone-classifier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skin-tone-classifier-0.1.8.tar", last modified: Wed Sep 21 09:26:01 2022, max compression
+gzip compressed data, was "skin-tone-classifier-0.1.9.tar", last modified: Tue Jan 10 06:09:26 2023, max compression
```

## Comparing `skin-tone-classifier-0.1.8.tar` & `skin-tone-classifier-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 09:26:01.944083 skin-tone-classifier-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-21 09:25:49.000000 skin-tone-classifier-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8590 2022-09-21 09:26:01.944083 skin-tone-classifier-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7673 2022-09-21 09:25:49.000000 skin-tone-classifier-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-21 09:26:01.944083 skin-tone-classifier-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-09-21 09:25:49.000000 skin-tone-classifier-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 09:26:01.940082 skin-tone-classifier-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 09:26:01.944083 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8590 2022-09-21 09:26:01.000000 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      417 2022-09-21 09:26:01.000000 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 09:26:01.000000 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-21 09:26:01.000000 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 09:26:01.000000 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-09-21 09:26:01.000000 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-21 09:26:01.000000 skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 09:26:01.944083 skin-tone-classifier-0.1.8/src/stone/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 09:25:49.000000 skin-tone-classifier-0.1.8/src/stone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12465 2022-09-21 09:25:49.000000 skin-tone-classifier-0.1.8/src/stone/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-10 06:09:26.000000 skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:26.421605 skin-tone-classifier-0.1.9/src/stone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/src/stone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-01-10 06:09:16.000000 skin-tone-classifier-0.1.9/src/stone/__main__.py
```

### Comparing `skin-tone-classifier-0.1.8/LICENSE` & `skin-tone-classifier-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skin-tone-classifier-0.1.8/PKG-INFO` & `skin-tone-classifier-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skin-tone-classifier
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy-to-use library for skin tone classification
 Home-page: https://chenglongma.com/SkinToneClassifier/
 Author: Chenglong Ma
 Author-email: chenglong.m@outlook.com
 Project-URL: Documentation, https://chenglongma.com/SkinToneClassifier/
 Project-URL: Code, https://github.com/ChenglongMa/SkinToneClassifier
 Project-URL: Issue tracker, https://github.com/ChenglongMa/SkinToneClassifier/issues
@@ -69,17 +69,17 @@
 2. dominant colors.
     1. _The number of colors depends on settings (default is 2) and their sizes depend on their proportion._
 3. specified color categories and the target label is enclosed by a rectangle.
 4. you can find a summary text at the bottom.
 
 Furthermore, there will be a report file named `result.csv` which contains more detailed information, e.g.,
 
-|file|face_location|dominant_1|props_1|dominant_2|props_2|category| distance(0-100)|
-|-----|-----|-----|-----|-----|-----|-----|-----|
-|lena_std|84:153|#CB6268|0.51|#E1A299|0.49|#e7c1b8|17.37|
+| file     | face_location | dominant_1 | props_1 | dominant_2 | props_2 | category | PERLA | distance(0-100) |
+|----------|---------------|------------|---------|------------|---------|----------|-------|-----------------|
+| lena_std | 84:153        | #CB6268    | 0.51    | #E1A299    | 0.49    | #e7c1b8  | I     | 17.37           |
 
 ## Detailed Usage
 
 To see the usage and parameters, run:
 
 ```shell
 stone -h
```

### Comparing `skin-tone-classifier-0.1.8/README.md` & `skin-tone-classifier-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,17 @@
 2. dominant colors.
     1. _The number of colors depends on settings (default is 2) and their sizes depend on their proportion._
 3. specified color categories and the target label is enclosed by a rectangle.
 4. you can find a summary text at the bottom.
 
 Furthermore, there will be a report file named `result.csv` which contains more detailed information, e.g.,
 
-|file|face_location|dominant_1|props_1|dominant_2|props_2|category| distance(0-100)|
-|-----|-----|-----|-----|-----|-----|-----|-----|
-|lena_std|84:153|#CB6268|0.51|#E1A299|0.49|#e7c1b8|17.37|
+| file     | face_location | dominant_1 | props_1 | dominant_2 | props_2 | category | PERLA | distance(0-100) |
+|----------|---------------|------------|---------|------------|---------|----------|-------|-----------------|
+| lena_std | 84:153        | #CB6268    | 0.51    | #E1A299    | 0.49    | #e7c1b8  | I     | 17.37           |
 
 ## Detailed Usage
 
 To see the usage and parameters, run:
 
 ```shell
 stone -h
```

### Comparing `skin-tone-classifier-0.1.8/setup.py` & `skin-tone-classifier-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 
 with open('README.md') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name='skin-tone-classifier',
     version=VERSION,
@@ -27,19 +27,19 @@
     },
     entry_points={
         'console_scripts': [
             'stone = stone.__main__:main'
         ],
     },
     install_requires=[
-        "opencv-python~=4.6.0.66",
-        "imutils~=0.5.4",
-        "numpy~=1.21.5",
-        "colormath~=3.0.0",
-        "tqdm~=4.64.0"
+        "opencv-python>=4.6.0.66",
+        "imutils>=0.5.4",
+        "numpy>=1.21.5",
+        "colormath>=3.0.0",
+        "tqdm>=4.64.0"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Topic :: Scientific/Engineering :: Image Processing",
```

### Comparing `skin-tone-classifier-0.1.8/src/skin_tone_classifier.egg-info/PKG-INFO` & `skin-tone-classifier-0.1.9/src/skin_tone_classifier.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skin-tone-classifier
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy-to-use library for skin tone classification
 Home-page: https://chenglongma.com/SkinToneClassifier/
 Author: Chenglong Ma
 Author-email: chenglong.m@outlook.com
 Project-URL: Documentation, https://chenglongma.com/SkinToneClassifier/
 Project-URL: Code, https://github.com/ChenglongMa/SkinToneClassifier
 Project-URL: Issue tracker, https://github.com/ChenglongMa/SkinToneClassifier/issues
@@ -69,17 +69,17 @@
 2. dominant colors.
     1. _The number of colors depends on settings (default is 2) and their sizes depend on their proportion._
 3. specified color categories and the target label is enclosed by a rectangle.
 4. you can find a summary text at the bottom.
 
 Furthermore, there will be a report file named `result.csv` which contains more detailed information, e.g.,
 
-|file|face_location|dominant_1|props_1|dominant_2|props_2|category| distance(0-100)|
-|-----|-----|-----|-----|-----|-----|-----|-----|
-|lena_std|84:153|#CB6268|0.51|#E1A299|0.49|#e7c1b8|17.37|
+| file     | face_location | dominant_1 | props_1 | dominant_2 | props_2 | category | PERLA | distance(0-100) |
+|----------|---------------|------------|---------|------------|---------|----------|-------|-----------------|
+| lena_std | 84:153        | #CB6268    | 0.51    | #E1A299    | 0.49    | #e7c1b8  | I     | 17.37           |
 
 ## Detailed Usage
 
 To see the usage and parameters, run:
 
 ```shell
 stone -h
```

### Comparing `skin-tone-classifier-0.1.8/src/stone/__main__.py` & `skin-tone-classifier-0.1.9/src/stone/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import argparse
 import glob
 import logging
 import os
+import re
 from datetime import datetime
 
 import cv2
 import imutils
 import numpy as np
 from colormath.color_conversions import convert_color
 from colormath.color_diff import delta_e_cie2000
 from colormath.color_objects import sRGBColor, LabColor
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 from pathlib import Path
 
 
+def sort_file(filename: Path):
+    nums = re.findall(r'\d+', filename.stem)
+    return int(nums[0]) if nums else filename
+
+
 def detect_faces(image, scaleFactor=1.1, minNeighbors=5, minSize=(30, 30)):
     image = image.copy()
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
     gray = cv2.equalizeHist(gray)
 
     cascade = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_default.xml')
     rects = cascade.detectMultiScale(gray, scaleFactor=scaleFactor, minNeighbors=minNeighbors, minSize=minSize, flags=cv2.CASCADE_SCALE_IMAGE)
@@ -73,39 +79,40 @@
     counts = counts[order]
 
     props = counts / counts.sum()
 
     return colors, props
 
 
-def skin_label(colors, props, labels):
-    lab_labels = [convert_color(sRGBColor.new_from_rgb_hex(lbl), LabColor) for lbl in labels]
+def skin_label(colors, props, categories, cate_labels):
+    lab_labels = [convert_color(sRGBColor.new_from_rgb_hex(lbl), LabColor) for lbl in categories]
     lab_colors = [convert_color(sRGBColor(rgb_r=r, rgb_g=g, rgb_b=b, is_upscaled=True), LabColor) for b, g, r in colors]
     distances = [np.sum([delta_e_cie2000(c, label) * p for c, p in zip(lab_colors, props)]) for label in lab_labels]
     label_id = np.argmin(distances)
     distance: float = distances[label_id]
-    category_hex = labels[label_id]
+    category_hex = categories[label_id]
+    PERLA = cate_labels[label_id]
     LOG.info(f'Classified color category: {category_hex}, distance: {distance}')
-    return label_id, category_hex, distance
+    return label_id, category_hex, PERLA, distance
 
 
-def classify(image, n_dominant_colors, labels, report_image, debug=False):
+def classify(image, n_dominant_colors, categories, cate_labels, report_image, debug=False):
     image = image.copy()
     image = detect_skin(image)
 
     colors, props = dominant_colors(image, n_clusters=n_dominant_colors)
 
     # Generate readable strings
     hex_colors = ['#%02X%02X%02X' % tuple(np.around([r, g, b]).astype(int)) for b, g, r in colors]
     prop_strs = ['%.2f' % p for p in props]
     res = list(np.hstack(list(zip(hex_colors, prop_strs))))
     LOG.info(f'Dominant color(s) with proportion: {res}')
-    label_id, category_hex, distance = skin_label(colors, props, labels)
+    label_id, category_hex, PERLA, distance = skin_label(colors, props, categories, cate_labels)
     distance = round(distance, 2)
-    res.extend([category_hex, distance])
+    res.extend([category_hex, PERLA, distance])
 
     debug_img = None
     if debug:
         color_bars = []
         color_w = 100
         total_height = 0
         for index, color in enumerate(colors):
@@ -117,24 +124,24 @@
         padding_height = report_image.shape[0] - total_height
         if padding_height > 0:
             padding = create_bar(padding_height, color_w, (255, 255, 255))
             color_bars.append(padding)
         color_bars = np.vstack(color_bars)
 
         label_bars = []
-        label_h = report_image.shape[0] // len(labels)
+        label_h = report_image.shape[0] // len(categories)
         label_w = color_w
         label_bgrs = []
-        for index, label_hex in enumerate(labels):
+        for label_hex in categories:
             hex_val = label_hex.lstrip('#')
             lr, lg, lb = [int(hex_val[i:i + 2], 16) for i in (0, 2, 4)]
             label_bgrs.append([lb, lg, lr])
             label_bar = create_bar(label_h, label_w, [lb, lg, lr])
             label_bars.append(label_bar)
-        padding_height = report_image.shape[0] - label_h * len(labels)
+        padding_height = report_image.shape[0] - label_h * len(categories)
         if padding_height > 0:
             padding = create_bar(padding_height, label_w, (255, 255, 255))
             label_bars.append(padding)
         label_bars = np.vstack(label_bars)
 
         debug_img = np.hstack([report_image, color_bars, label_bars])
 
@@ -192,16 +199,19 @@
                         help='Image filename(s) to process;\n'
                              'supports multiple values separated by space, e.g., "a.jpg b.png";\n'
                              'supports directory or file name(s), e.g., "./path/to/images/ a.jpg";\n'
                              'The app will search all images in current directory in default.')
 
     default_categories = ["#373028", "#422811", "#513b2e", "#6f503c", "#81654f", "#9d7a54", "#bea07e", "#e5c8a6", "#e7c1b8", "#f3dad6", "#fbf2f3"]
 
+    default_labels = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'[:len(default_categories)]
     parser.add_argument('-c', '--categories', nargs='+', default=default_categories, metavar='COLOR',
                         help='Skin tone categories; supports RGB hex value leading by # or RGB values separated by comma(,).')
+    parser.add_argument('-l', '--labels', nargs='+', default=default_labels, metavar='LABEL',
+                        help='Category labels; default values are uppercase alphabet list; separated by comma(,).')
     parser.add_argument('-d', '--debug', action='store_true', help='Whether to output processed images, used for debugging and verification.')
     parser.add_argument('-o', '--output', default='./', metavar='DIRECTORY',
                         help='The path of output file, defaults to current directory.')
 
     parser.add_argument('--n_colors', type=int, metavar='N',
                         help='CONFIG: the number of dominant colors to be extracted, defaults to 2.', default=2)
     parser.add_argument('--new_width', type=int, metavar='WIDTH',
@@ -225,40 +235,44 @@
         if os.path.isdir(name):
             filenames.extend([glob.glob(os.path.join(name, i)) for i in valid_images])
         if os.path.isfile(name):
             filenames.append([name])
 
     filenames = [Path(f) for fs in filenames for f in fs]
     assert len(filenames) > 0, 'No valid images in the specified path.'
+    # Sort filenames by (first) number extracted from the filename string
+    filenames.sort(key=sort_file)
     is_single_file = len(filenames) == 1
 
     debug: bool = args.debug
     categories: list[str] = args.categories
+    cate_labels = args.labels
     for idx, ct in enumerate(categories):
         if not ct.startswith('#') and len(ct.split(',')) == 3:
             r, g, b = ct.split(',')
             categories[idx] = '#%02X%02X%02X' % (int(r), int(g), int(b))
     n_dominant_colors = args.n_colors
     min_size = args.min_size[:2]
     output_dir = args.output
     os.makedirs(output_dir, exist_ok=True)
 
     # Start - open file
     f = open(os.path.join(args.output, './result.csv'), 'w', encoding='UTF8')
-    header = 'file,face_location,' + ','.join([f'dominant_{i + 1},props_{i + 1}' for i in range(n_dominant_colors)]) + ',category, distance(0-100)\n'
+    header = 'file,face_location,' + ','.join(
+        [f'dominant_{i + 1},props_{i + 1}' for i in range(n_dominant_colors)]) + ',category,PERLA,distance(0-100)\n'
     f.write(header)
 
     # Start - processing images
     with logging_redirect_tqdm():
         for filename in tqdm(filenames):
             basename, extension = filename.stem, filename.suffix
 
             LOG.info(f'\n----- Processing {basename} -----')
             ori_image = cv2.imread(str(filename.resolve()), cv2.IMREAD_UNCHANGED)
-            if not ori_image:
+            if ori_image is None:
                 LOG.warning(f'{filename}.{extension} is not found or is not a valid image.')
                 continue
 
             resized_image = imutils.resize(ori_image, width=args.new_width)
             final_image = resized_image.copy()
             faces = detect_faces(resized_image, args.scale, args.min_nbrs, min_size)
 
@@ -266,20 +280,20 @@
             if len(faces) > 0:
                 LOG.info(f'Found {len(faces)} face(s)')
                 for idx, (x1, y1, x2, y2) in enumerate(faces):
                     LOG.info(f'Face {idx + 1} location: {x1}:{x2}')
                     face = resized_image[y1:y2, x1:x2]
                     if debug:
                         final_image = draw_rects(resized_image, [x1, y1, x2, y2])
-                    res, _debug_img = classify(face, n_dominant_colors, categories, final_image, debug)
+                    res, _debug_img = classify(face, n_dominant_colors, categories, cate_labels, final_image, debug)
                     writerow(f, [basename, f'{x1}:{x2}'] + res)
                     debug_imgs.append(_debug_img)
             else:
                 LOG.info(f'Found 0 face, will detect global skin area instead')
-                res, _debug_img = classify(resized_image, n_dominant_colors, categories, final_image, debug)
+                res, _debug_img = classify(resized_image, n_dominant_colors, categories, cate_labels, final_image, debug)
                 writerow(f, [basename, 'NA'] + res)
                 debug_imgs.append(_debug_img)
 
             if debug:
                 debug_dir = os.path.join(output_dir, './debug')
                 os.makedirs(debug_dir, exist_ok=True)
                 for idx, img in enumerate(debug_imgs):
```

