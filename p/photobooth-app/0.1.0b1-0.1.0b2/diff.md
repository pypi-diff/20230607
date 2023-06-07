# Comparing `tmp/photobooth_app-0.1.0b1.tar.gz` & `tmp/photobooth_app-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photobooth_app-0.1.0b1.tar", max compression
+gzip compressed data, was "photobooth_app-0.1.0b2.tar", max compression
```

## Comparing `photobooth_app-0.1.0b1.tar` & `photobooth_app-0.1.0b2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     1105 2023-04-16 19:41:18.851253 photobooth_app-0.1.0b1/LICENSE.md
--rw-r--r--   0        0        0       34 2023-05-10 07:23:57.824936 photobooth_app-0.1.0b1/photobooth/__init__.py
--rw-r--r--   0        0        0     3726 2023-06-07 05:57:52.602534 photobooth_app-0.1.0b1/photobooth/__main__.py
--rw-r--r--   0        0        0    17065 2023-06-02 20:24:52.671100 photobooth_app-0.1.0b1/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2023-06-06 16:03:56.915894 photobooth_app-0.1.0b1/photobooth/application.py
--rw-r--r--   0        0        0     1427 2023-06-02 20:24:52.280427 photobooth_app-0.1.0b1/photobooth/containers.py
--rw-r--r--   0        0        0       37 2023-05-10 07:23:57.826935 photobooth_app-0.1.0b1/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2023-06-02 20:24:52.474620 photobooth_app-0.1.0b1/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2023-06-02 20:24:52.482670 photobooth_app-0.1.0b1/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2023-06-07 04:57:30.382728 photobooth_app-0.1.0b1/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2023-06-05 19:13:20.930204 photobooth_app-0.1.0b1/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2023-06-02 20:24:52.183447 photobooth_app-0.1.0b1/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2023-06-02 20:21:06.997514 photobooth_app-0.1.0b1/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1135 2023-06-02 20:24:52.226025 photobooth_app-0.1.0b1/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2023-06-02 20:24:52.667666 photobooth_app-0.1.0b1/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1478 2023-06-02 20:24:52.238638 photobooth_app-0.1.0b1/photobooth/routers/system.py
--rw-r--r--   0        0        0       37 2023-05-10 07:23:57.830933 photobooth_app-0.1.0b1/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-02 20:24:52.297677 photobooth_app-0.1.0b1/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      463 2023-06-02 20:21:06.993993 photobooth_app-0.1.0b1/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2023-06-02 20:21:06.993993 photobooth_app-0.1.0b1/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2023-06-07 05:38:27.581313 photobooth_app-0.1.0b1/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       37 2023-05-10 07:23:57.831939 photobooth_app-0.1.0b1/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2023-06-02 20:24:52.390055 photobooth_app-0.1.0b1/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0    11560 2023-06-02 20:21:06.992475 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2023-06-02 20:21:06.992984 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2023-06-06 15:59:52.014297 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2023-06-06 15:59:52.021124 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2023-06-06 15:59:52.027134 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2023-06-06 15:59:52.040572 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2023-06-06 15:59:52.051238 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0    43739 2023-06-06 15:59:56.690038 photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0     2618 2023-06-02 20:24:52.676149 photobooth_app-0.1.0b1/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    10505 2023-06-02 20:24:52.555326 photobooth_app-0.1.0b1/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16264 2023-06-02 20:23:56.441667 photobooth_app-0.1.0b1/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2023-06-02 20:24:52.362713 photobooth_app-0.1.0b1/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2023-06-02 20:24:52.433553 photobooth_app-0.1.0b1/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2023-06-07 05:11:57.354210 photobooth_app-0.1.0b1/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2023-06-02 20:24:52.893474 photobooth_app-0.1.0b1/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7597 2023-06-02 20:24:52.554325 photobooth_app-0.1.0b1/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0      527 2023-05-17 05:00:20.775209 photobooth_app-0.1.0b1/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3263 2023-06-04 06:50:54.801038 photobooth_app-0.1.0b1/photobooth/services/containers.py
--rw-r--r--   0        0        0     4202 2023-06-02 20:24:52.542987 photobooth_app-0.1.0b1/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2011 2023-06-04 06:54:16.991936 photobooth_app-0.1.0b1/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2023-06-05 19:13:00.192653 photobooth_app-0.1.0b1/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0       37 2023-05-10 07:23:57.839933 photobooth_app-0.1.0b1/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-02 20:21:07.003058 photobooth_app-0.1.0b1/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     6010 2023-06-02 20:21:07.004067 photobooth_app-0.1.0b1/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0     1934 2023-06-02 20:21:07.004067 photobooth_app-0.1.0b1/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0    10102 2023-06-02 20:21:07.004067 photobooth_app-0.1.0b1/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8753 2023-06-02 20:21:07.005067 photobooth_app-0.1.0b1/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     3019 2023-06-07 05:43:55.945504 photobooth_app-0.1.0b1/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5647 2023-06-02 20:24:52.874966 photobooth_app-0.1.0b1/photobooth/services/wledservice.py
--rw-r--r--   0        0        0       93 2023-06-02 20:21:07.005578 photobooth_app-0.1.0b1/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2023-06-02 20:21:07.006586 photobooth_app-0.1.0b1/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      474 2023-05-10 07:23:57.847934 photobooth_app-0.1.0b1/photobooth/utils/helper.py
--rw-r--r--   0        0        0      918 2023-05-10 07:23:57.847934 photobooth_app-0.1.0b1/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      646 2023-05-10 07:23:57.847934 photobooth_app-0.1.0b1/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11560 2023-05-10 07:23:57.848938 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2023-05-10 07:23:57.850938 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2023-05-10 07:23:57.851935 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2023-05-10 07:23:57.853933 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2023-05-10 07:23:57.855939 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2023-05-10 07:23:57.856937 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2023-05-10 07:23:57.858934 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2023-05-10 07:23:57.860934 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2023-05-10 07:23:57.861934 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2023-05-10 07:23:57.862933 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2023-05-10 07:23:57.864933 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2023-05-10 07:23:57.865936 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2023-05-10 07:23:57.867935 photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      144 2023-06-02 20:21:07.009105 photobooth_app-0.1.0b1/photobooth/web_spa/css/31.363e41a9.css
--rw-r--r--   0        0        0       88 2023-06-02 20:21:07.009105 photobooth_app-0.1.0b1/photobooth/web_spa/css/706.42cb67d0.css
--rw-r--r--   0        0        0      163 2023-06-02 20:21:07.009105 photobooth_app-0.1.0b1/photobooth/web_spa/css/71.0be6c807.css
--rw-r--r--   0        0        0      359 2023-06-02 15:50:59.543694 photobooth_app-0.1.0b1/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2023-06-02 20:21:07.011622 photobooth_app-0.1.0b1/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    64483 2023-06-02 15:50:59.543694 photobooth_app-0.1.0b1/photobooth/web_spa/favicon.ico-todo
--rw-r--r--   0        0        0   164912 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0    20436 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0     5336 2023-06-02 15:50:59.543694 photobooth_app-0.1.0b1/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0      905 2023-06-02 20:21:07.011622 photobooth_app-0.1.0b1/photobooth/web_spa/index.html
--rw-r--r--   0        0        0     9915 2023-06-02 20:21:07.011622 photobooth_app-0.1.0b1/photobooth/web_spa/js/31.51d7e662.js
--rw-r--r--   0        0        0     2918 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1217 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3034 2023-06-02 15:50:59.543694 photobooth_app-0.1.0b1/photobooth/web_spa/js/645.2ddc3ded.js
--rw-r--r--   0        0        0     5660 2023-06-02 20:21:07.012621 photobooth_app-0.1.0b1/photobooth/web_spa/js/692.cf3b55d3.js
--rw-r--r--   0        0        0     3924 2023-06-02 20:21:07.013130 photobooth_app-0.1.0b1/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9305 2023-06-02 20:21:07.013130 photobooth_app-0.1.0b1/photobooth/web_spa/js/706.f32434a0.js
--rw-r--r--   0        0        0     5357 2023-06-02 20:21:07.014138 photobooth_app-0.1.0b1/photobooth/web_spa/js/71.3aaf5d7d.js
--rw-r--r--   0        0        0     1581 2023-06-02 15:50:59.541687 photobooth_app-0.1.0b1/photobooth/web_spa/js/770.b7df615e.js
--rw-r--r--   0        0        0      778 2023-06-02 15:50:59.543694 photobooth_app-0.1.0b1/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2023-06-02 15:50:59.543694 photobooth_app-0.1.0b1/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0    12590 2023-06-02 20:21:07.014138 photobooth_app-0.1.0b1/photobooth/web_spa/js/app.ed0492eb.js
--rw-r--r--   0        0        0  1417500 2023-06-02 20:21:07.019174 photobooth_app-0.1.0b1/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0     3957 2023-06-07 15:42:03.506267 photobooth_app-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     5333 2023-06-07 05:43:16.458848 photobooth_app-0.1.0b1/README.md
--rw-r--r--   0        0        0     6850 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/LICENSE.md
+-rw-r--r--   0        0        0     5663 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/README.md
+-rw-r--r--   0        0        0       33 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/__init__.py
+-rw-r--r--   0        0        0     3726 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/__main__.py
+-rw-r--r--   0        0        0    17065 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3322 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2326 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/config.py
+-rw-r--r--   0        0        0      593 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/home.py
+-rw-r--r--   0        0        0      770 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/log.py
+-rw-r--r--   0        0        0     2133 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3390 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1135 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0      463 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0    11560 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2023-06-07 18:35:13.872542 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2023-06-07 18:35:13.876542 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2023-06-07 18:35:13.880543 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2023-06-07 18:35:13.884543 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2023-06-07 18:35:13.900544 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0    43739 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0     2618 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    10505 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16264 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7597 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0      506 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     3263 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/containers.py
+-rw-r--r--   0        0        0     4202 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2011 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0       36 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     6853 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     6010 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0     1934 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0    10102 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8753 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     4068 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5647 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0       93 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2023-06-07 18:35:13.916545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2023-06-07 18:35:13.916545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2023-06-07 18:35:13.916545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2023-06-07 18:35:13.920545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2023-06-07 18:35:13.920545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2023-06-07 18:35:13.920545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2023-06-07 18:35:13.924545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2023-06-07 18:35:13.924545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2023-06-07 18:35:13.924545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      144 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/31.363e41a9.css
+-rw-r--r--   0        0        0       88 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/706.42cb67d0.css
+-rw-r--r--   0        0        0      163 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/71.0be6c807.css
+-rw-r--r--   0        0        0      359 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    64483 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/favicon.ico-todo
+-rw-r--r--   0        0        0    20436 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     5336 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0      905 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0     9915 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/31.51d7e662.js
+-rw-r--r--   0        0        0     2918 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/391.70a80bd8.js
+-rw-r--r--   0        0        0     1217 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3034 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/645.2ddc3ded.js
+-rw-r--r--   0        0        0     5660 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/692.cf3b55d3.js
+-rw-r--r--   0        0        0     3924 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9305 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/706.f32434a0.js
+-rw-r--r--   0        0        0     5357 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/71.3aaf5d7d.js
+-rw-r--r--   0        0        0     1581 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/770.b7df615e.js
+-rw-r--r--   0        0        0      778 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0    12590 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/app.ed0492eb.js
+-rw-r--r--   0        0        0  1417500 2023-06-07 18:35:13.940546 photobooth_app-0.1.0b2/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0     3957 2023-06-07 18:35:13.944547 photobooth_app-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b2/PKG-INFO
```

### Comparing `photobooth_app-0.1.0b1/LICENSE.md` & `photobooth_app-0.1.0b2/LICENSE.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022-2023 Michael G (me@mgrl.de)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022-2023 Michael G (me@mgrl.de)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `photobooth_app-0.1.0b1/photobooth/__main__.py` & `photobooth_app-0.1.0b2/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/appconfig.py` & `photobooth_app-0.1.0b2/photobooth/appconfig.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/application.py` & `photobooth_app-0.1.0b2/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/containers.py` & `photobooth_app-0.1.0b2/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0b2/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/config.py` & `photobooth_app-0.1.0b2/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/home.py` & `photobooth_app-0.1.0b2/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/log.py` & `photobooth_app-0.1.0b2/photobooth/routers/log.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0b2/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0b2/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/processing.py` & `photobooth_app-0.1.0b2/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/sse.py` & `photobooth_app-0.1.0b2/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/routers/system.py` & `photobooth_app-0.1.0b2/photobooth/routers/system.py`

 * *Files 15% similar despite different names*

```diff
@@ -33,12 +33,22 @@
         appcontainer.init_resources()
     elif action == "service" and param == "restart":
         system_service.util_systemd_control("restart")
     elif action == "service" and param == "stop":
         system_service.util_systemd_control("stop")
     elif action == "service" and param == "start":
         system_service.util_systemd_control("start")
+    elif action == "service" and param == "install":
+        try:
+            system_service.install_service()
+        except Exception as exc:
+            raise HTTPException(500, f"service install failed: {exc}") from exc
+    elif action == "service" and param == "uninstall":
+        try:
+            system_service.uninstall_service()
+        except Exception as exc:
+            raise HTTPException(500, f"service uninstall failed: {exc}") from exc
 
     else:
         raise HTTPException(500, f"invalid request action={action}, param={param}")
 
     return f"action={action}, param={param}"
```

### Comparing `photobooth_app-0.1.0b1/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0b2/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/gphoto2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0b2/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/containers.py` & `photobooth_app-0.1.0b2/photobooth/services/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/informationservice.py` & `photobooth_app-0.1.0b2/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0b2/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0b2/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0b2/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0b2/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0b2/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0b2/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/processingservice.py` & `photobooth_app-0.1.0b2/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/services/wledservice.py` & `photobooth_app-0.1.0b2/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0b2/photobooth/utils/repeatedtimer.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-"""
-Repeat Timer in separate thread for tasks to be executed in intervals
-"""
-from threading import Timer
-
-
-class RepeatedTimer:
-    """_summary_"""
-
-    def __init__(self, interval: float, function, *args, **kwargs):
-        self._timer = None
-        self.interval: float = interval
-        self.function = function
-        self.args = args
-        self.kwargs = kwargs
-        self.is_running = False
-        # self.start()
-
-    def _run(self):
-        """_summary_"""
-        self.is_running = False
-        self.start()
-        self.function(*self.args, **self.kwargs)
-
-    def start(self):
-        """_summary_"""
-        if not self.is_running:
-            self._timer = Timer(self.interval, self._run)
-            self._timer.start()
-            self.is_running = True
-
-    def stop(self):
-        """_summary_"""
-        self._timer.cancel()
-        self.is_running = False
+"""
+Repeat Timer in separate thread for tasks to be executed in intervals
+"""
+from threading import Timer
+
+
+class RepeatedTimer:
+    """_summary_"""
+
+    def __init__(self, interval: float, function, *args, **kwargs):
+        self._timer = None
+        self.interval: float = interval
+        self.function = function
+        self.args = args
+        self.kwargs = kwargs
+        self.is_running = False
+        # self.start()
+
+    def _run(self):
+        """_summary_"""
+        self.is_running = False
+        self.start()
+        self.function(*self.args, **self.kwargs)
+
+    def start(self):
+        """_summary_"""
+        if not self.is_running:
+            self._timer = Timer(self.interval, self._run)
+            self._timer.start()
+            self.is_running = True
+
+    def stop(self):
+        """_summary_"""
+        self._timer.cancel()
+        self.is_running = False
```

### Comparing `photobooth_app-0.1.0b1/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0b2/photobooth/utils/stoppablethread.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-"""_summary_
-"""
-import threading
-
-
-class StoppableThread(threading.Thread):
-    """Thread class with a stop() method. The thread itself has to check
-    regularly for the stopped() condition."""
-
-    def __init__(self, *args, **kwargs):
-        """_summary_"""
-        super().__init__(*args, **kwargs)
-        self._stop_event = threading.Event()
-
-    def stop(self):
-        """_summary_"""
-        self._stop_event.set()
-
-    def stopped(self):
-        """check in run loop. break loop if stopped() returns True
-
-        Returns:
-            _type_: _description_
-        """
-        return self._stop_event.is_set()
+"""_summary_
+"""
+import threading
+
+
+class StoppableThread(threading.Thread):
+    """Thread class with a stop() method. The thread itself has to check
+    regularly for the stopped() condition."""
+
+    def __init__(self, *args, **kwargs):
+        """_summary_"""
+        super().__init__(*args, **kwargs)
+        self._stop_event = threading.Event()
+
+    def stop(self):
+        """_summary_"""
+        self._stop_event.set()
+
+    def stopped(self):
+        """check in run loop. break loop if stopped() returns True
+
+        Returns:
+            _type_: _description_
+        """
+        return self._stop_event.is_set()
```

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0b2/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/favicon.ico-todo` & `photobooth_app-0.1.0b2/photobooth/web_spa/favicon.ico-todo`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0b2/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/index.html` & `photobooth_app-0.1.0b2/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/31.51d7e662.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/31.51d7e662.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/391.70a80bd8.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/645.2ddc3ded.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/645.2ddc3ded.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/692.cf3b55d3.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/692.cf3b55d3.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/706.f32434a0.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/706.f32434a0.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/71.3aaf5d7d.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/71.3aaf5d7d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/770.b7df615e.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/770.b7df615e.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/app.ed0492eb.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/app.ed0492eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0b2/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b1/pyproject.toml` & `photobooth_app-0.1.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 686f 746f 626f 6f74 682d 6170  = "photobooth-ap
 00000020: 7022 0d0a 7265 7175 6972 6573 2d70 7974  p"..requires-pyt
 00000030: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 00000040: 3132 220d 0a76 6572 7369 6f6e 203d 2022  12"..version = "
-00000050: 302e 312e 3062 3122 0d0a 6465 7363 7269  0.1.0b1"..descri
+00000050: 302e 312e 3062 3222 0d0a 6465 7363 7269  0.1.0b2"..descri
 00000060: 7074 696f 6e20 3d20 2250 686f 746f 626f  ption = "Photobo
 00000070: 6f74 6820 6170 7020 7772 6974 7465 6e20  oth app written 
 00000080: 696e 2050 7974 686f 6e20 7375 7070 6f72  in Python suppor
 00000090: 7469 6e67 2044 534c 522c 2070 6963 616d  ting DSLR, picam
 000000a0: 6572 6132 2c20 7765 6263 616d 6572 6173  era2, webcameras
 000000b0: 220d 0a61 7574 686f 7273 203d 205b 7b20  "..authors = [{ 
 000000c0: 6e61 6d65 203d 2022 4d69 6368 6165 6c20  name = "Michael 
@@ -68,15 +68,15 @@
 00000430: 656e 7461 7469 6f6e 203d 2022 6874 7470  entation = "http
 00000440: 733a 2f2f 6d67 726c 2e67 6974 6875 622e  s://mgrl.github.
 00000450: 696f 2f70 686f 746f 626f 6f74 682d 646f  io/photobooth-do
 00000460: 6373 220d 0a0d 0a0d 0a5b 746f 6f6c 2e70  cs"......[tool.p
 00000470: 6f65 7472 795d 0d0a 6e61 6d65 203d 2022  oetry]..name = "
 00000480: 7068 6f74 6f62 6f6f 7468 2d61 7070 220d  photobooth-app".
 00000490: 0a76 6572 7369 6f6e 203d 2022 302e 312e  .version = "0.1.
-000004a0: 3062 3122 0d0a 6465 7363 7269 7074 696f  0b1"..descriptio
+000004a0: 3062 3222 0d0a 6465 7363 7269 7074 696f  0b2"..descriptio
 000004b0: 6e20 3d20 2250 686f 746f 626f 6f74 6820  n = "Photobooth 
 000004c0: 6170 7020 7772 6974 7465 6e20 696e 2050  app written in P
 000004d0: 7974 686f 6e20 7375 7070 6f72 7469 6e67  ython supporting
 000004e0: 2044 534c 522c 2070 6963 616d 6572 6132   DSLR, picamera2
 000004f0: 2c20 7765 6263 616d 6572 6173 220d 0a61  , webcameras"..a
 00000500: 7574 686f 7273 203d 205b 224d 6963 6861  uthors = ["Micha
 00000510: 656c 2047 203c 6d65 406d 6772 6c2e 6465  el G <me@mgrl.de
```

### Comparing `photobooth_app-0.1.0b1/README.md` & `photobooth_app-0.1.0b2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 ![rpi, linux and windows platform supported](https://img.shields.io/badge/platform-rpi%20%7C%20linux%20%7C%20windows-lightgrey)
 [![ruff](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml)
 [![pytest](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml)
 [![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/dev/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
 
 The photobooth app is written in Python 🐍 and coming along with a modern Vue frontend.
 
----
-
-**[Features](#heart_eyes-features)** - **[Supported Cameras](#camera-supported-cameras)** - **[Installation](#wrench-installation)** - **[Troubleshooting](#interrobang-troubleshooting)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)**
+**[Features](#-features)** - **[Supported Cameras](#-supported-cameras)** - **[Installation](#-installation)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)**
 
 ## 😍 Features
 
 - 📹 camera live preview with shortest delay as possible, permanent video live view in background
 - ⚡️ optimized for speed, live stream hardware accelerated on rpi, cpu load < 20%
 - 🫶 several camera backends supported for high quality stills and livestream
 - 💡 WLED support signaling photo countdown and feedback to the user when the photo is actually taken
@@ -35,21 +33,21 @@
 
 The booth is made from 3d printed parts, [see the documentation ✍ over here](https://github.com/mgrl/photobooth-3d).
 The camera support is mostly ready to use, the frontend is not production ready yet.
 Use [photobooth project](https://photoboothproject.github.io/) as frontend.
 
 ## 💅 Screenshots
 
-![frontpage](misc/screenshots/frontpage.png)
-![gallery list](misc/screenshots/gallery_list.png)
-![gallery detail](misc/screenshots/gallery_detail.png)
-![admin center page dashboard](misc/screenshots/admin_dashboard.png)
-![admin center page config tab backends](misc/screenshots/admin_config_backends.png)
-![admin center page config tab userinterface](misc/screenshots/admin_config_ui.png)
-![admin center page status](misc/screenshots/admin_status.png)
+![frontpage](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/frontpage.png)
+![gallery list](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_list.png)
+![gallery detail](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_detail.png)
+![admin center page dashboard](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_dashboard.png)
+![admin center page config tab backends](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_backends.png)
+![admin center page config tab userinterface](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_ui.png)
+![admin center page status](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_status.png)
 
 ## 🔧 Installation
 
 ### Prerequisites
 
 - Python 3.9 or later
 - Camera, can be one or two (first camera for stills, second camera for live view)
```

### Comparing `photobooth_app-0.1.0b1/PKG-INFO` & `photobooth_app-0.1.0b2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
 Home-page: https://github.com/mgrl/photobooth-app
 License: MIT
 Author: Michael G
 Author-email: me@mgrl.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -42,17 +42,15 @@
 ![rpi, linux and windows platform supported](https://img.shields.io/badge/platform-rpi%20%7C%20linux%20%7C%20windows-lightgrey)
 [![ruff](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/ruff.yml)
 [![pytest](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml/badge.svg)](https://github.com/mgrl/photobooth-app/actions/workflows/pytests.yml)
 [![codecov](https://codecov.io/gh/mgrl/photobooth-app/branch/dev/graph/badge.svg?token=SBB5DGX17V)](https://codecov.io/gh/mgrl/photobooth-app)
 
 The photobooth app is written in Python 🐍 and coming along with a modern Vue frontend.
 
----
-
-**[Features](#heart_eyes-features)** - **[Supported Cameras](#camera-supported-cameras)** - **[Installation](#wrench-installation)** - **[Troubleshooting](#interrobang-troubleshooting)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)**
+**[Features](#-features)** - **[Supported Cameras](#-supported-cameras)** - **[Installation](#-installation)** - **[Documentation](https://mgrl.github.io/photobooth-docs/)**
 
 ## 😍 Features
 
 - 📹 camera live preview with shortest delay as possible, permanent video live view in background
 - ⚡️ optimized for speed, live stream hardware accelerated on rpi, cpu load < 20%
 - 🫶 several camera backends supported for high quality stills and livestream
 - 💡 WLED support signaling photo countdown and feedback to the user when the photo is actually taken
@@ -73,21 +71,21 @@
 
 The booth is made from 3d printed parts, [see the documentation ✍ over here](https://github.com/mgrl/photobooth-3d).
 The camera support is mostly ready to use, the frontend is not production ready yet.
 Use [photobooth project](https://photoboothproject.github.io/) as frontend.
 
 ## 💅 Screenshots
 
-![frontpage](misc/screenshots/frontpage.png)
-![gallery list](misc/screenshots/gallery_list.png)
-![gallery detail](misc/screenshots/gallery_detail.png)
-![admin center page dashboard](misc/screenshots/admin_dashboard.png)
-![admin center page config tab backends](misc/screenshots/admin_config_backends.png)
-![admin center page config tab userinterface](misc/screenshots/admin_config_ui.png)
-![admin center page status](misc/screenshots/admin_status.png)
+![frontpage](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/frontpage.png)
+![gallery list](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_list.png)
+![gallery detail](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/gallery_detail.png)
+![admin center page dashboard](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_dashboard.png)
+![admin center page config tab backends](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_backends.png)
+![admin center page config tab userinterface](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_config_ui.png)
+![admin center page status](https://raw.githubusercontent.com/mgrl/photobooth-app/main/misc/screenshots/admin_status.png)
 
 ## 🔧 Installation
 
 ### Prerequisites
 
 - Python 3.9 or later
 - Camera, can be one or two (first camera for stills, second camera for live view)
```

