# Comparing `tmp/photobooth_app-0.1.0b2.tar.gz` & `tmp/photobooth_app-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photobooth_app-0.1.0b2.tar", max compression
+gzip compressed data, was "photobooth_app-0.1.0b3.tar", max compression
```

## Comparing `photobooth_app-0.1.0b2.tar` & `photobooth_app-0.1.0b3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
--rw-r--r--   0        0        0     1084 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/LICENSE.md
--rw-r--r--   0        0        0     5663 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/README.md
--rw-r--r--   0        0        0       33 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/__init__.py
--rw-r--r--   0        0        0     3726 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/__main__.py
--rw-r--r--   0        0        0    17065 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/application.py
--rw-r--r--   0        0        0     1427 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/containers.py
--rw-r--r--   0        0        0       36 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1135 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      463 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0    11560 2023-06-07 18:35:13.868542 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2023-06-07 18:35:13.872542 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2023-06-07 18:35:13.876542 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2023-06-07 18:35:13.880543 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2023-06-07 18:35:13.884543 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2023-06-07 18:35:13.900544 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0    43739 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0     2618 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    10505 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16264 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7597 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0      506 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3263 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/containers.py
--rw-r--r--   0        0        0     4202 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2011 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0       36 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     6010 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0     1934 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0    10102 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8753 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     4068 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5647 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/services/wledservice.py
--rw-r--r--   0        0        0       93 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2023-06-07 18:35:13.912545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2023-06-07 18:35:13.916545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2023-06-07 18:35:13.916545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2023-06-07 18:35:13.916545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2023-06-07 18:35:13.920545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2023-06-07 18:35:13.920545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2023-06-07 18:35:13.920545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2023-06-07 18:35:13.924545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2023-06-07 18:35:13.924545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2023-06-07 18:35:13.924545 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      144 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/31.363e41a9.css
--rw-r--r--   0        0        0       88 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/706.42cb67d0.css
--rw-r--r--   0        0        0      163 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/71.0be6c807.css
--rw-r--r--   0        0        0      359 2023-06-07 18:35:13.928546 photobooth_app-0.1.0b2/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    64483 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/favicon.ico-todo
--rw-r--r--   0        0        0    20436 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     5336 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0      905 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/index.html
--rw-r--r--   0        0        0     9915 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/31.51d7e662.js
--rw-r--r--   0        0        0     2918 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1217 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3034 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/645.2ddc3ded.js
--rw-r--r--   0        0        0     5660 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/692.cf3b55d3.js
--rw-r--r--   0        0        0     3924 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9305 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/706.f32434a0.js
--rw-r--r--   0        0        0     5357 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/71.3aaf5d7d.js
--rw-r--r--   0        0        0     1581 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/770.b7df615e.js
--rw-r--r--   0        0        0      778 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0    12590 2023-06-07 18:35:13.932546 photobooth_app-0.1.0b2/photobooth/web_spa/js/app.ed0492eb.js
--rw-r--r--   0        0        0  1417500 2023-06-07 18:35:13.940546 photobooth_app-0.1.0b2/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0     3957 2023-06-07 18:35:13.944547 photobooth_app-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/LICENSE.md
+-rw-r--r--   0        0        0     6586 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/README.md
+-rw-r--r--   0        0        0       33 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/__init__.py
+-rw-r--r--   0        0        0     3726 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/__main__.py
+-rw-r--r--   0        0        0    17065 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3322 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2326 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/config.py
+-rw-r--r--   0        0        0      593 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/home.py
+-rw-r--r--   0        0        0      770 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/log.py
+-rw-r--r--   0        0        0     2133 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3390 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1135 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3121 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0      463 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2023-06-07 20:03:38.737789 photobooth_app-0.1.0b3/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0    11560 2023-06-07 20:03:38.741789 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2023-06-07 20:03:38.741789 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2023-06-07 20:03:38.745789 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2023-06-07 20:03:38.749790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2023-06-07 20:03:38.753790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2023-06-07 20:03:38.765790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0    43739 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0     2618 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    10517 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16264 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7597 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0      506 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     3263 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/containers.py
+-rw-r--r--   0        0        0     4202 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2011 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0       36 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     6853 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     6010 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0     1934 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0    10102 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8753 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     4068 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5647 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0       93 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2023-06-07 20:03:38.773790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2023-06-07 20:03:38.777790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2023-06-07 20:03:38.777790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2023-06-07 20:03:38.777790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2023-06-07 20:03:38.781790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2023-06-07 20:03:38.785790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      144 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/31.363e41a9.css
+-rw-r--r--   0        0        0       88 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/706.42cb67d0.css
+-rw-r--r--   0        0        0      163 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/71.0be6c807.css
+-rw-r--r--   0        0        0      359 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    64483 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/favicon.ico-todo
+-rw-r--r--   0        0        0    20436 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     5336 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0      905 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0     9915 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/31.51d7e662.js
+-rw-r--r--   0        0        0     2918 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/391.70a80bd8.js
+-rw-r--r--   0        0        0     1217 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3034 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/645.2ddc3ded.js
+-rw-r--r--   0        0        0     5660 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/692.cf3b55d3.js
+-rw-r--r--   0        0        0     3924 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9305 2023-06-07 20:03:38.789790 photobooth_app-0.1.0b3/photobooth/web_spa/js/706.f32434a0.js
+-rw-r--r--   0        0        0     5357 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/71.3aaf5d7d.js
+-rw-r--r--   0        0        0     1581 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/770.b7df615e.js
+-rw-r--r--   0        0        0      778 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0    12590 2023-06-07 20:03:38.793790 photobooth_app-0.1.0b3/photobooth/web_spa/js/app.ed0492eb.js
+-rw-r--r--   0        0        0  1417500 2023-06-07 20:03:38.797790 photobooth_app-0.1.0b3/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0     3966 2023-06-07 20:03:38.797790 photobooth_app-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     8075 1970-01-01 00:00:00.000000 photobooth_app-0.1.0b3/PKG-INFO
```

### Comparing `photobooth_app-0.1.0b2/LICENSE.md` & `photobooth_app-0.1.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/README.md` & `photobooth_app-0.1.0b3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -67,27 +67,57 @@
 On a fresh Raspberry Pi OS 64bit, run following commands:
 
 ```sh
 sudo apt-get update
 sudo apt-get upgrade # system should be up to date
 
 # install some system dependencies
-sudo apt-get -y install libturbojpeg0 python3-pip libgl1 python3-picamera2
+sudo apt-get -y install libturbojpeg0 python3-pip libgl1 python3-picamera2 libgphoto2-dev
 
 # add user to input group for keyboard events
 usermod --append --groups tty,input {USERNAME}
 
 # install app
 pip install photobooth-app
+
+# create data folder
+mkdir ~/photobooth-data
+cd ~/photobooth-data
+
+# start app
+photobooth
 ```
 
-Start the app and browse to <http://localhost:8000>.
+Browse to <http://localhost:8000> and see if the app is working properly.
+
+#### Photobooth command not found
+
+If there is a warning as following during pip installation and photobooth can't start check the PATH variable
+
+```text
+WARNING: The script photobooth is installed in '/home/pi/.local/bin' which is not on PATH.
+Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+```
+
+See following is fine, might just need a restart after installation because the path .local/bin did not exist before.
+
+```sh  # ~/.profile
+# set PATH so it includes user's private bin if it exists
+if [ -d "$HOME/.local/bin" ] ; then
+    PATH="$HOME/.local/bin:$PATH"
+fi
+```
+
+#### Install development versions
+
+Stable releases are published at pypi registry.
+To test the latest development version install directly from git:
 
 ```sh
-photobooth # photobooth should be available globally. if file is not found check PATH
+pip install git+https://github.com/mgrl/photobooth-app.git@dev
 ```
 
 ### Integrate Photobooth-Project and this Photobooth-App
 
 Following commands have to be set in photobooth project to use this app as streamingserver.
 Replace <http://photobooth> by the actual hostname or localhost if on same server.
```

### Comparing `photobooth_app-0.1.0b2/photobooth/__main__.py` & `photobooth_app-0.1.0b3/photobooth/__main__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/appconfig.py` & `photobooth_app-0.1.0b3/photobooth/appconfig.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/application.py` & `photobooth_app-0.1.0b3/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/containers.py` & `photobooth_app-0.1.0b3/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0b3/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/config.py` & `photobooth_app-0.1.0b3/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/home.py` & `photobooth_app-0.1.0b3/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/log.py` & `photobooth_app-0.1.0b3/photobooth/routers/log.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0b3/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0b3/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/processing.py` & `photobooth_app-0.1.0b3/photobooth/routers/processing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/sse.py` & `photobooth_app-0.1.0b3/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/routers/system.py` & `photobooth_app-0.1.0b3/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0b3/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0b3/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0b3/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/gphoto2.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import time
 from threading import Condition, Event
 
 try:
     import gphoto2 as gp
 except Exception as import_exc:
-    raise OSError("gphoto2 not supported on windows platform") from import_exc
+    raise RuntimeError("gphoto2 import error; check gphoto2 installation") from import_exc
 
 from pymitter import EventEmitter
 
 from photobooth.services.backends.abstractbackend import AbstractBackend, BackendStats
 from photobooth.utils.stoppablethread import StoppableThread
 
 from ...appconfig import AppConfig
```

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0b3/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/containers.py` & `photobooth_app-0.1.0b3/photobooth/services/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/informationservice.py` & `photobooth_app-0.1.0b3/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0b3/photobooth/services/keyboardservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0b3/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0b3/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0b3/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0b3/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0b3/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/processingservice.py` & `photobooth_app-0.1.0b3/photobooth/services/processingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/systemservice.py` & `photobooth_app-0.1.0b3/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/services/wledservice.py` & `photobooth_app-0.1.0b3/photobooth/services/wledservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0b3/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0b3/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0b3/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0b3/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/favicon.ico-todo` & `photobooth_app-0.1.0b3/photobooth/web_spa/favicon.ico-todo`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0b3/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0b3/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/index.html` & `photobooth_app-0.1.0b3/photobooth/web_spa/index.html`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/31.51d7e662.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/31.51d7e662.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/391.70a80bd8.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/645.2ddc3ded.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/645.2ddc3ded.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/692.cf3b55d3.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/692.cf3b55d3.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/706.f32434a0.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/706.f32434a0.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/71.3aaf5d7d.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/71.3aaf5d7d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/770.b7df615e.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/770.b7df615e.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/app.ed0492eb.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/app.ed0492eb.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0b3/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0b2/pyproject.toml` & `photobooth_app-0.1.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 686f 746f 626f 6f74 682d 6170  = "photobooth-ap
 00000020: 7022 0d0a 7265 7175 6972 6573 2d70 7974  p"..requires-pyt
 00000030: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 00000040: 3132 220d 0a76 6572 7369 6f6e 203d 2022  12"..version = "
-00000050: 302e 312e 3062 3222 0d0a 6465 7363 7269  0.1.0b2"..descri
+00000050: 302e 312e 3062 3322 0d0a 6465 7363 7269  0.1.0b3"..descri
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
-000004a0: 3062 3222 0d0a 6465 7363 7269 7074 696f  0b2"..descriptio
+000004a0: 3062 3322 0d0a 6465 7363 7269 7074 696f  0b3"..descriptio
 000004b0: 6e20 3d20 2250 686f 746f 626f 6f74 6820  n = "Photobooth 
 000004c0: 6170 7020 7772 6974 7465 6e20 696e 2050  app written in P
 000004d0: 7974 686f 6e20 7375 7070 6f72 7469 6e67  ython supporting
 000004e0: 2044 534c 522c 2070 6963 616d 6572 6132   DSLR, picamera2
 000004f0: 2c20 7765 6263 616d 6572 6173 220d 0a61  , webcameras"..a
 00000500: 7574 686f 7273 203d 205b 224d 6963 6861  uthors = ["Micha
 00000510: 656c 2047 203c 6d65 406d 6772 6c2e 6465  el G <me@mgrl.de
@@ -103,146 +103,146 @@
 00000660: 735d 0d0a 7068 6f74 6f62 6f6f 7468 203d  s]..photobooth =
 00000670: 2022 7068 6f74 6f62 6f6f 7468 2e5f 5f6d   "photobooth.__m
 00000680: 6169 6e5f 5f3a 6d61 696e 220d 0a0d 0a0d  ain__:main".....
 00000690: 0a5b 746f 6f6c 2e70 6f65 7472 792e 6465  .[tool.poetry.de
 000006a0: 7065 6e64 656e 6369 6573 5d0d 0a70 7974  pendencies]..pyt
 000006b0: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 000006c0: 3132 220d 0a66 6173 7461 7069 203d 2022  12"..fastapi = "
-000006d0: 5e30 2e39 352e 3222 0d0a 6f70 656e 6376  ^0.95.2"..opencv
-000006e0: 2d70 7974 686f 6e20 3d20 225e 342e 372e  -python = "^4.7.
-000006f0: 302e 3732 220d 0a70 6965 7869 6620 3d20  0.72"..piexif = 
-00000700: 225e 312e 312e 3322 0d0a 7069 6c6c 6f77  "^1.1.3"..pillow
-00000710: 203d 2022 5e39 2e35 2e30 220d 0a70 7375   = "^9.5.0"..psu
-00000720: 7469 6c20 3d20 225e 352e 392e 3522 0d0a  til = "^5.9.5"..
-00000730: 7079 6461 6e74 6963 203d 2022 5e31 2e31  pydantic = "^1.1
-00000740: 302e 3822 0d0a 7079 6d69 7474 6572 203d  0.8"..pymitter =
-00000750: 2022 5e30 2e34 2e30 220d 0a70 7974 7572   "^0.4.0"..pytur
-00000760: 626f 6a70 6567 203d 2022 5e31 2e37 2e31  bojpeg = "^1.7.1
-00000770: 220d 0a72 6571 7565 7374 7320 3d20 225e  "..requests = "^
-00000780: 322e 3331 2e30 220d 0a73 7365 2d73 7461  2.31.0"..sse-sta
-00000790: 726c 6574 7465 203d 2022 5e31 2e36 2e31  rlette = "^1.6.1
-000007a0: 220d 0a75 7669 636f 726e 203d 2022 5e30  "..uvicorn = "^0
-000007b0: 2e32 322e 3022 0d0a 7079 7468 6f6e 2d64  .22.0"..python-d
-000007c0: 6f74 656e 7620 3d20 225e 312e 302e 3022  otenv = "^1.0.0"
-000007d0: 0d0a 7079 7365 7269 616c 203d 2022 5e33  ..pyserial = "^3
-000007e0: 2e35 220d 0a6a 736f 6e72 6566 203d 2022  .5"..jsonref = "
-000007f0: 5e31 2e31 2e30 220d 0a64 6570 656e 6465  ^1.1.0"..depende
-00000800: 6e63 792d 696e 6a65 6374 6f72 203d 2022  ncy-injector = "
-00000810: 5e34 2e34 312e 3022 0d0a 7069 6c67 7261  ^4.41.0"..pilgra
-00000820: 6d32 203d 2022 5e32 2e30 2e32 220d 0a76  m2 = "^2.0.2"..v
-00000830: 346c 3270 7920 3d20 7b76 6572 7369 6f6e  4l2py = {version
-00000840: 203d 2022 5e30 2e36 2e32 222c 2070 6c61   = "^0.6.2", pla
-00000850: 7466 6f72 6d20 3d20 226c 696e 7578 227d  tform = "linux"}
-00000860: 0d0a 6770 696f 7a65 726f 203d 207b 7665  ..gpiozero = {ve
-00000870: 7273 696f 6e20 3d20 225e 312e 362e 3222  rsion = "^1.6.2"
-00000880: 2c20 706c 6174 666f 726d 203d 2022 6c69  , platform = "li
-00000890: 6e75 7822 7d0d 0a67 7068 6f74 6f32 203d  nux"}..gphoto2 =
-000008a0: 207b 7665 7273 696f 6e20 3d20 225e 322e   {version = "^2.
-000008b0: 332e 3422 2c20 706c 6174 666f 726d 203d  3.4", platform =
-000008c0: 2022 6c69 6e75 7822 7d0d 0a70 7974 686f   "linux"}..pytho
-000008d0: 6e2d 7374 6174 656d 6163 6869 6e65 203d  n-statemachine =
-000008e0: 2022 5e32 2e30 2e30 220d 0a23 206b 6579   "^2.0.0"..# key
-000008f0: 626f 6172 6420 6973 2075 6e6d 6169 6e74  board is unmaint
-00000900: 6169 6e65 6420 6275 7420 6c61 7465 7374  ained but latest
-00000910: 206d 6173 7465 7220 7665 7273 696f 6e20   master version 
-00000920: 6e65 6564 6564 2074 6f20 7375 7070 6f72  needed to suppor
-00000930: 7420 6e6f 6e2d 7375 646f 206b 6579 626f  t non-sudo keybo
-00000940: 6172 6420 6163 6365 7373 2e0d 0a23 2069  ard access...# i
-00000950: 6e63 6c75 6465 206b 6579 626f 6172 6420  nclude keyboard 
-00000960: 6173 2076 656e 646f 7220 7375 6270 6163  as vendor subpac
-00000970: 6b61 6765 2072 6967 6874 206e 6f77 2075  kage right now u
-00000980: 6e74 696c 2062 6574 7465 7220 736f 6c75  ntil better solu
-00000990: 7469 6f6e 2066 6f75 6e64 2e20 6469 7265  tion found. dire
-000009a0: 6374 2072 6566 6572 656e 6365 7320 6172  ct references ar
-000009b0: 6520 6e6f 7420 616c 6c6f 7765 6420 6f6e  e not allowed on
-000009c0: 2070 7970 692e 0d0a 2320 6874 7470 733a   pypi...# https:
-000009d0: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6f70  //github.com/bop
-000009e0: 7072 6568 2f6b 6579 626f 6172 642f 6973  preh/keyboard/is
-000009f0: 7375 6573 2f34 3230 2369 7373 7565 636f  sues/420#issueco
-00000a00: 6d6d 656e 742d 3133 3634 3130 3039 3735  mment-1364100975
-00000a10: 0d0a 2320 6b65 7962 6f61 7264 203d 207b  ..# keyboard = {
-00000a20: 6769 7420 3d20 2268 7474 7073 3a2f 2f67  git = "https://g
-00000a30: 6974 6875 622e 636f 6d2f 626f 7070 7265  ithub.com/boppre
-00000a40: 682f 6b65 7962 6f61 7264 222c 2072 6576  h/keyboard", rev
-00000a50: 3d22 6432 3332 6465 3039 6264 6135 3065  ="d232de09bda50e
-00000a60: 6362 3532 3131 6562 6363 3539 6238 3562  cb5211ebcc59b85b
-00000a70: 6336 6461 3661 6161 3234 227d 0d0a 0d0a  c6da6aaa24"}....
-00000a80: 0d0a 5b74 6f6f 6c2e 706f 6574 7279 2e67  ..[tool.poetry.g
-00000a90: 726f 7570 2e64 6576 2e64 6570 656e 6465  roup.dev.depende
-00000aa0: 6e63 6965 735d 0d0a 7079 7465 7374 203d  ncies]..pytest =
-00000ab0: 2022 5e37 2e32 2e30 220d 0a70 7974 6573   "^7.2.0"..pytes
-00000ac0: 742d 6265 6e63 686d 6172 6b20 3d20 225e  t-benchmark = "^
-00000ad0: 342e 302e 3022 0d0a 7079 7465 7374 2d63  4.0.0"..pytest-c
-00000ae0: 6f76 203d 2022 5e34 2e30 2e30 220d 0a72  ov = "^4.0.0"..r
-00000af0: 7566 6620 3d20 225e 302e 302e 3237 3022  uff = "^0.0.270"
-00000b00: 0d0a 6874 7470 782d 7373 6520 3d20 225e  ..httpx-sse = "^
-00000b10: 302e 332e 3122 0d0a 6874 7470 7820 3d20  0.3.1"..httpx = 
-00000b20: 225e 302e 3234 2e31 220d 0a73 696d 706c  "^0.24.1"..simpl
-00000b30: 656a 7065 6720 3d20 225e 312e 362e 3622  ejpeg = "^1.6.6"
-00000b40: 0d0a 636f 7665 7261 6765 203d 207b 6578  ..coverage = {ex
-00000b50: 7472 6173 203d 205b 2274 6f6d 6c22 5d2c  tras = ["toml"],
-00000b60: 2076 6572 7369 6f6e 203d 2022 5e37 2e32   version = "^7.2
-00000b70: 2e37 227d 0d0a 0d0a 5b62 7569 6c64 2d73  .7"}....[build-s
-00000b80: 7973 7465 6d5d 0d0a 7265 7175 6972 6573  ystem]..requires
-00000b90: 203d 205b 2270 6f65 7472 792d 636f 7265   = ["poetry-core
-00000ba0: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
-00000bb0: 6420 3d20 2270 6f65 7472 792e 636f 7265  d = "poetry.core
-00000bc0: 2e6d 6173 6f6e 7279 2e61 7069 220d 0a0d  .masonry.api"...
-00000bd0: 0a0d 0a5b 746f 6f6c 2e70 7974 6573 742e  ...[tool.pytest.
-00000be0: 696e 695f 6f70 7469 6f6e 735d 0d0a 6c6f  ini_options]..lo
-00000bf0: 675f 636c 6920 3d20 7472 7565 0d0a 6c6f  g_cli = true..lo
-00000c00: 675f 636c 695f 6c65 7665 6c20 3d20 2244  g_cli_level = "D
-00000c10: 4542 5547 220d 0a6c 6f67 5f63 6c69 5f66  EBUG"..log_cli_f
-00000c20: 6f72 6d61 7420 3d20 2225 2861 7363 7469  ormat = "%(ascti
-00000c30: 6d65 2973 205b 2528 6c65 7665 6c6e 616d  me)s [%(levelnam
-00000c40: 6529 3873 5d20 2528 6d65 7373 6167 6529  e)8s] %(message)
-00000c50: 7320 2825 2866 696c 656e 616d 6529 733a  s (%(filename)s:
-00000c60: 2528 6c69 6e65 6e6f 2973 2922 0d0a 6c6f  %(lineno)s)"..lo
-00000c70: 675f 636c 695f 6461 7465 5f66 6f72 6d61  g_cli_date_forma
-00000c80: 7420 3d20 2225 592d 256d 2d25 6420 2548  t = "%Y-%m-%d %H
-00000c90: 3a25 4d3a 2553 220d 0a0d 0a5b 746f 6f6c  :%M:%S"....[tool
-00000ca0: 2e63 6f76 6572 6167 652e 7275 6e5d 0d0a  .coverage.run]..
-00000cb0: 2320 6469 7361 626c 6520 636f 756c 646e  # disable couldn
-00000cc0: 742d 7061 7273 653a 2068 7474 7073 3a2f  t-parse: https:/
-00000cd0: 2f67 6974 6875 622e 636f 6d2f 6e65 6462  /github.com/nedb
-00000ce0: 6174 2f63 6f76 6572 6167 6570 792f 6973  at/coveragepy/is
-00000cf0: 7375 6573 2f31 3339 320d 0a64 6973 6162  sues/1392..disab
-00000d00: 6c65 5f77 6172 6e69 6e67 7320 3d20 5b22  le_warnings = ["
-00000d10: 636f 756c 646e 742d 7061 7273 6522 5d0d  couldnt-parse"].
-00000d20: 0a6f 6d69 7420 3d20 5b0d 0a20 2020 2022  .omit = [..    "
-00000d30: 696e 7374 616c 6c2e 7079 222c 0d0a 2020  install.py",..  
-00000d40: 2020 2274 6573 745f 2a2e 7079 222c 0d0a    "test_*.py",..
-00000d50: 2020 2020 222e 2f74 6573 7473 2f2a 220d      "./tests/*".
-00000d60: 0a20 2020 205d 0d0a 7061 7261 6c6c 656c  .    ]..parallel
-00000d70: 203d 2074 7275 650d 0a63 6f6e 6375 7272   = true..concurr
-00000d80: 656e 6379 203d 205b 2274 6872 6561 6422  ency = ["thread"
-00000d90: 2c22 6d75 6c74 6970 726f 6365 7373 696e  ,"multiprocessin
-00000da0: 6722 5d0d 0a0d 0a5b 746f 6f6c 2e62 6c61  g"]....[tool.bla
-00000db0: 636b 5d0d 0a6c 696e 652d 6c65 6e67 7468  ck]..line-length
-00000dc0: 203d 2031 3230 0d0a 0d0a 5b74 6f6f 6c2e   = 120....[tool.
-00000dd0: 7275 6666 5d0d 0a6c 696e 652d 6c65 6e67  ruff]..line-leng
-00000de0: 7468 203d 2031 3230 0d0a 7365 6c65 6374  th = 120..select
-00000df0: 203d 205b 0d0a 2020 2245 222c 2020 2023   = [..  "E",   #
-00000e00: 2070 7963 6f64 6573 7479 6c65 0d0a 2020   pycodestyle..  
-00000e10: 2257 222c 2020 2023 2070 7963 6f64 6573  "W",   # pycodes
-00000e20: 7479 6c65 0d0a 2020 2246 222c 2020 2023  tyle..  "F",   #
-00000e30: 2070 7966 6c61 6b65 730d 0a20 2022 4222   pyflakes..  "B"
-00000e40: 2c20 2020 2320 6275 6762 6561 720d 0a20  ,   # bugbear.. 
-00000e50: 2022 5550 222c 2020 2320 7079 7570 6772   "UP",  # pyupgr
-00000e60: 6164 650d 0a20 2022 4922 2c20 2020 2320  ade..  "I",   # 
-00000e70: 6973 6f72 740d 0a20 2023 2244 222c 2020  isort..  #"D",  
-00000e80: 2023 2070 7964 6f63 7374 796c 6520 2020   # pydocstyle   
-00000e90: 2320 6164 6420 6c61 7465 720d 0a5d 0d0a  # add later..]..
-00000ea0: 6967 6e6f 7265 203d 205b 0d0a 2020 2242  ignore = [..  "B
-00000eb0: 3030 3822 2023 7573 6564 2066 6f72 2044  008" #used for D
-00000ec0: 4920 696e 6a65 6374 696f 6e0d 0a20 205d  I injection..  ]
-00000ed0: 0d0a 6578 7465 6e64 2d65 7863 6c75 6465  ..extend-exclude
-00000ee0: 203d 205b 222e 2f73 6372 6970 7473 222c   = ["./scripts",
-00000ef0: 2022 696e 7374 616c 6c2e 7079 225d 0d0a   "install.py"]..
-00000f00: 0d0a 5b74 6f6f 6c2e 7275 6666 2e70 6572  ..[tool.ruff.per
-00000f10: 2d66 696c 652d 6967 6e6f 7265 735d 0d0a  -file-ignores]..
-00000f20: 2270 686f 746f 626f 6f74 682f 6170 7063  "photobooth/appc
-00000f30: 6f6e 6669 672e 7079 2220 3d20 5b22 4535  onfig.py" = ["E5
-00000f40: 3031 225d 0d0a 0d0a 5b74 6f6f 6c2e 7275  01"]....[tool.ru
-00000f50: 6666 2e70 7964 6f63 7374 796c 655d 0d0a  ff.pydocstyle]..
-00000f60: 636f 6e76 656e 7469 6f6e 203d 2022 676f  convention = "go
-00000f70: 6f67 6c65 22                             ogle"
+000006d0: 3e3d 302e 3935 2e32 2c3c 302e 3937 2e30  >=0.95.2,<0.97.0
+000006e0: 220d 0a6f 7065 6e63 762d 7079 7468 6f6e  "..opencv-python
+000006f0: 203d 2022 5e34 2e37 2e30 2e37 3222 0d0a   = "^4.7.0.72"..
+00000700: 7069 6578 6966 203d 2022 5e31 2e31 2e33  piexif = "^1.1.3
+00000710: 220d 0a70 696c 6c6f 7720 3d20 225e 392e  "..pillow = "^9.
+00000720: 352e 3022 0d0a 7073 7574 696c 203d 2022  5.0"..psutil = "
+00000730: 5e35 2e39 2e35 220d 0a70 7964 616e 7469  ^5.9.5"..pydanti
+00000740: 6320 3d20 225e 312e 3130 2e38 220d 0a70  c = "^1.10.8"..p
+00000750: 796d 6974 7465 7220 3d20 225e 302e 342e  ymitter = "^0.4.
+00000760: 3022 0d0a 7079 7475 7262 6f6a 7065 6720  0"..pyturbojpeg 
+00000770: 3d20 225e 312e 372e 3122 0d0a 7265 7175  = "^1.7.1"..requ
+00000780: 6573 7473 203d 2022 5e32 2e33 312e 3022  ests = "^2.31.0"
+00000790: 0d0a 7373 652d 7374 6172 6c65 7474 6520  ..sse-starlette 
+000007a0: 3d20 225e 312e 362e 3122 0d0a 7576 6963  = "^1.6.1"..uvic
+000007b0: 6f72 6e20 3d20 225e 302e 3232 2e30 220d  orn = "^0.22.0".
+000007c0: 0a70 7974 686f 6e2d 646f 7465 6e76 203d  .python-dotenv =
+000007d0: 2022 5e31 2e30 2e30 220d 0a70 7973 6572   "^1.0.0"..pyser
+000007e0: 6961 6c20 3d20 225e 332e 3522 0d0a 6a73  ial = "^3.5"..js
+000007f0: 6f6e 7265 6620 3d20 225e 312e 312e 3022  onref = "^1.1.0"
+00000800: 0d0a 6465 7065 6e64 656e 6379 2d69 6e6a  ..dependency-inj
+00000810: 6563 746f 7220 3d20 225e 342e 3431 2e30  ector = "^4.41.0
+00000820: 220d 0a70 696c 6772 616d 3220 3d20 225e  "..pilgram2 = "^
+00000830: 322e 302e 3222 0d0a 7634 6c32 7079 203d  2.0.2"..v4l2py =
+00000840: 207b 7665 7273 696f 6e20 3d20 225e 302e   {version = "^0.
+00000850: 362e 3222 2c20 706c 6174 666f 726d 203d  6.2", platform =
+00000860: 2022 6c69 6e75 7822 7d0d 0a67 7069 6f7a   "linux"}..gpioz
+00000870: 6572 6f20 3d20 7b76 6572 7369 6f6e 203d  ero = {version =
+00000880: 2022 5e31 2e36 2e32 222c 2070 6c61 7466   "^1.6.2", platf
+00000890: 6f72 6d20 3d20 226c 696e 7578 227d 0d0a  orm = "linux"}..
+000008a0: 6770 686f 746f 3220 3d20 7b76 6572 7369  gphoto2 = {versi
+000008b0: 6f6e 203d 2022 5e32 2e33 2e34 222c 2070  on = "^2.3.4", p
+000008c0: 6c61 7466 6f72 6d20 3d20 226c 696e 7578  latform = "linux
+000008d0: 227d 0d0a 7079 7468 6f6e 2d73 7461 7465  "}..python-state
+000008e0: 6d61 6368 696e 6520 3d20 225e 322e 302e  machine = "^2.0.
+000008f0: 3022 0d0a 2320 6b65 7962 6f61 7264 2069  0"..# keyboard i
+00000900: 7320 756e 6d61 696e 7461 696e 6564 2062  s unmaintained b
+00000910: 7574 206c 6174 6573 7420 6d61 7374 6572  ut latest master
+00000920: 2076 6572 7369 6f6e 206e 6565 6465 6420   version needed 
+00000930: 746f 2073 7570 706f 7274 206e 6f6e 2d73  to support non-s
+00000940: 7564 6f20 6b65 7962 6f61 7264 2061 6363  udo keyboard acc
+00000950: 6573 732e 0d0a 2320 696e 636c 7564 6520  ess...# include 
+00000960: 6b65 7962 6f61 7264 2061 7320 7665 6e64  keyboard as vend
+00000970: 6f72 2073 7562 7061 636b 6167 6520 7269  or subpackage ri
+00000980: 6768 7420 6e6f 7720 756e 7469 6c20 6265  ght now until be
+00000990: 7474 6572 2073 6f6c 7574 696f 6e20 666f  tter solution fo
+000009a0: 756e 642e 2064 6972 6563 7420 7265 6665  und. direct refe
+000009b0: 7265 6e63 6573 2061 7265 206e 6f74 2061  rences are not a
+000009c0: 6c6c 6f77 6564 206f 6e20 7079 7069 2e0d  llowed on pypi..
+000009d0: 0a23 2068 7474 7073 3a2f 2f67 6974 6875  .# https://githu
+000009e0: 622e 636f 6d2f 626f 7070 7265 682f 6b65  b.com/boppreh/ke
+000009f0: 7962 6f61 7264 2f69 7373 7565 732f 3432  yboard/issues/42
+00000a00: 3023 6973 7375 6563 6f6d 6d65 6e74 2d31  0#issuecomment-1
+00000a10: 3336 3431 3030 3937 350d 0a23 206b 6579  364100975..# key
+00000a20: 626f 6172 6420 3d20 7b67 6974 203d 2022  board = {git = "
+00000a30: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000a40: 6f6d 2f62 6f70 7072 6568 2f6b 6579 626f  om/boppreh/keybo
+00000a50: 6172 6422 2c20 7265 763d 2264 3233 3264  ard", rev="d232d
+00000a60: 6530 3962 6461 3530 6563 6235 3231 3165  e09bda50ecb5211e
+00000a70: 6263 6335 3962 3835 6263 3664 6136 6161  bcc59b85bc6da6aa
+00000a80: 6132 3422 7d0d 0a0d 0a0d 0a5b 746f 6f6c  a24"}......[tool
+00000a90: 2e70 6f65 7472 792e 6772 6f75 702e 6465  .poetry.group.de
+00000aa0: 762e 6465 7065 6e64 656e 6369 6573 5d0d  v.dependencies].
+00000ab0: 0a70 7974 6573 7420 3d20 225e 372e 322e  .pytest = "^7.2.
+00000ac0: 3022 0d0a 7079 7465 7374 2d62 656e 6368  0"..pytest-bench
+00000ad0: 6d61 726b 203d 2022 5e34 2e30 2e30 220d  mark = "^4.0.0".
+00000ae0: 0a70 7974 6573 742d 636f 7620 3d20 225e  .pytest-cov = "^
+00000af0: 342e 302e 3022 0d0a 7275 6666 203d 2022  4.0.0"..ruff = "
+00000b00: 5e30 2e30 2e32 3730 220d 0a68 7474 7078  ^0.0.270"..httpx
+00000b10: 2d73 7365 203d 2022 5e30 2e33 2e31 220d  -sse = "^0.3.1".
+00000b20: 0a68 7474 7078 203d 2022 5e30 2e32 342e  .httpx = "^0.24.
+00000b30: 3122 0d0a 7369 6d70 6c65 6a70 6567 203d  1"..simplejpeg =
+00000b40: 2022 5e31 2e36 2e36 220d 0a63 6f76 6572   "^1.6.6"..cover
+00000b50: 6167 6520 3d20 7b65 7874 7261 7320 3d20  age = {extras = 
+00000b60: 5b22 746f 6d6c 225d 2c20 7665 7273 696f  ["toml"], versio
+00000b70: 6e20 3d20 225e 372e 322e 3722 7d0d 0a0d  n = "^7.2.7"}...
+00000b80: 0a5b 6275 696c 642d 7379 7374 656d 5d0d  .[build-system].
+00000b90: 0a72 6571 7569 7265 7320 3d20 5b22 706f  .requires = ["po
+00000ba0: 6574 7279 2d63 6f72 6522 5d0d 0a62 7569  etry-core"]..bui
+00000bb0: 6c64 2d62 6163 6b65 6e64 203d 2022 706f  ld-backend = "po
+00000bc0: 6574 7279 2e63 6f72 652e 6d61 736f 6e72  etry.core.masonr
+00000bd0: 792e 6170 6922 0d0a 0d0a 0d0a 5b74 6f6f  y.api"......[too
+00000be0: 6c2e 7079 7465 7374 2e69 6e69 5f6f 7074  l.pytest.ini_opt
+00000bf0: 696f 6e73 5d0d 0a6c 6f67 5f63 6c69 203d  ions]..log_cli =
+00000c00: 2074 7275 650d 0a6c 6f67 5f63 6c69 5f6c   true..log_cli_l
+00000c10: 6576 656c 203d 2022 4445 4255 4722 0d0a  evel = "DEBUG"..
+00000c20: 6c6f 675f 636c 695f 666f 726d 6174 203d  log_cli_format =
+00000c30: 2022 2528 6173 6374 696d 6529 7320 5b25   "%(asctime)s [%
+00000c40: 286c 6576 656c 6e61 6d65 2938 735d 2025  (levelname)8s] %
+00000c50: 286d 6573 7361 6765 2973 2028 2528 6669  (message)s (%(fi
+00000c60: 6c65 6e61 6d65 2973 3a25 286c 696e 656e  lename)s:%(linen
+00000c70: 6f29 7329 220d 0a6c 6f67 5f63 6c69 5f64  o)s)"..log_cli_d
+00000c80: 6174 655f 666f 726d 6174 203d 2022 2559  ate_format = "%Y
+00000c90: 2d25 6d2d 2564 2025 483a 254d 3a25 5322  -%m-%d %H:%M:%S"
+00000ca0: 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665 7261  ....[tool.covera
+00000cb0: 6765 2e72 756e 5d0d 0a23 2064 6973 6162  ge.run]..# disab
+00000cc0: 6c65 2063 6f75 6c64 6e74 2d70 6172 7365  le couldnt-parse
+00000cd0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00000ce0: 2e63 6f6d 2f6e 6564 6261 742f 636f 7665  .com/nedbat/cove
+00000cf0: 7261 6765 7079 2f69 7373 7565 732f 3133  ragepy/issues/13
+00000d00: 3932 0d0a 6469 7361 626c 655f 7761 726e  92..disable_warn
+00000d10: 696e 6773 203d 205b 2263 6f75 6c64 6e74  ings = ["couldnt
+00000d20: 2d70 6172 7365 225d 0d0a 6f6d 6974 203d  -parse"]..omit =
+00000d30: 205b 0d0a 2020 2020 2269 6e73 7461 6c6c   [..    "install
+00000d40: 2e70 7922 2c0d 0a20 2020 2022 7465 7374  .py",..    "test
+00000d50: 5f2a 2e70 7922 2c0d 0a20 2020 2022 2e2f  _*.py",..    "./
+00000d60: 7465 7374 732f 2a22 0d0a 2020 2020 5d0d  tests/*"..    ].
+00000d70: 0a70 6172 616c 6c65 6c20 3d20 7472 7565  .parallel = true
+00000d80: 0d0a 636f 6e63 7572 7265 6e63 7920 3d20  ..concurrency = 
+00000d90: 5b22 7468 7265 6164 222c 226d 756c 7469  ["thread","multi
+00000da0: 7072 6f63 6573 7369 6e67 225d 0d0a 0d0a  processing"]....
+00000db0: 5b74 6f6f 6c2e 626c 6163 6b5d 0d0a 6c69  [tool.black]..li
+00000dc0: 6e65 2d6c 656e 6774 6820 3d20 3132 300d  ne-length = 120.
+00000dd0: 0a0d 0a5b 746f 6f6c 2e72 7566 665d 0d0a  ...[tool.ruff]..
+00000de0: 6c69 6e65 2d6c 656e 6774 6820 3d20 3132  line-length = 12
+00000df0: 300d 0a73 656c 6563 7420 3d20 5b0d 0a20  0..select = [.. 
+00000e00: 2022 4522 2c20 2020 2320 7079 636f 6465   "E",   # pycode
+00000e10: 7374 796c 650d 0a20 2022 5722 2c20 2020  style..  "W",   
+00000e20: 2320 7079 636f 6465 7374 796c 650d 0a20  # pycodestyle.. 
+00000e30: 2022 4622 2c20 2020 2320 7079 666c 616b   "F",   # pyflak
+00000e40: 6573 0d0a 2020 2242 222c 2020 2023 2062  es..  "B",   # b
+00000e50: 7567 6265 6172 0d0a 2020 2255 5022 2c20  ugbear..  "UP", 
+00000e60: 2023 2070 7975 7067 7261 6465 0d0a 2020   # pyupgrade..  
+00000e70: 2249 222c 2020 2023 2069 736f 7274 0d0a  "I",   # isort..
+00000e80: 2020 2322 4422 2c20 2020 2320 7079 646f    #"D",   # pydo
+00000e90: 6373 7479 6c65 2020 2023 2061 6464 206c  cstyle   # add l
+00000ea0: 6174 6572 0d0a 5d0d 0a69 676e 6f72 6520  ater..]..ignore 
+00000eb0: 3d20 5b0d 0a20 2022 4230 3038 2220 2375  = [..  "B008" #u
+00000ec0: 7365 6420 666f 7220 4449 2069 6e6a 6563  sed for DI injec
+00000ed0: 7469 6f6e 0d0a 2020 5d0d 0a65 7874 656e  tion..  ]..exten
+00000ee0: 642d 6578 636c 7564 6520 3d20 5b22 2e2f  d-exclude = ["./
+00000ef0: 7363 7269 7074 7322 2c20 2269 6e73 7461  scripts", "insta
+00000f00: 6c6c 2e70 7922 5d0d 0a0d 0a5b 746f 6f6c  ll.py"]....[tool
+00000f10: 2e72 7566 662e 7065 722d 6669 6c65 2d69  .ruff.per-file-i
+00000f20: 676e 6f72 6573 5d0d 0a22 7068 6f74 6f62  gnores].."photob
+00000f30: 6f6f 7468 2f61 7070 636f 6e66 6967 2e70  ooth/appconfig.p
+00000f40: 7922 203d 205b 2245 3530 3122 5d0d 0a0d  y" = ["E501"]...
+00000f50: 0a5b 746f 6f6c 2e72 7566 662e 7079 646f  .[tool.ruff.pydo
+00000f60: 6373 7479 6c65 5d0d 0a63 6f6e 7665 6e74  cstyle]..convent
+00000f70: 696f 6e20 3d20 2267 6f6f 676c 6522       ion = "google"
```

### Comparing `photobooth_app-0.1.0b2/PKG-INFO` & `photobooth_app-0.1.0b3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
 Home-page: https://github.com/mgrl/photobooth-app
 License: MIT
 Author: Michael G
 Author-email: me@mgrl.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dependency-injector (>=4.41.0,<5.0.0)
-Requires-Dist: fastapi (>=0.95.2,<0.96.0)
+Requires-Dist: fastapi (>=0.95.2,<0.97.0)
 Requires-Dist: gphoto2 (>=2.3.4,<3.0.0) ; sys_platform == "linux"
 Requires-Dist: gpiozero (>=1.6.2,<2.0.0) ; sys_platform == "linux"
 Requires-Dist: jsonref (>=1.1.0,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
 Requires-Dist: pilgram2 (>=2.0.2,<3.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
@@ -105,27 +105,57 @@
 On a fresh Raspberry Pi OS 64bit, run following commands:
 
 ```sh
 sudo apt-get update
 sudo apt-get upgrade # system should be up to date
 
 # install some system dependencies
-sudo apt-get -y install libturbojpeg0 python3-pip libgl1 python3-picamera2
+sudo apt-get -y install libturbojpeg0 python3-pip libgl1 python3-picamera2 libgphoto2-dev
 
 # add user to input group for keyboard events
 usermod --append --groups tty,input {USERNAME}
 
 # install app
 pip install photobooth-app
+
+# create data folder
+mkdir ~/photobooth-data
+cd ~/photobooth-data
+
+# start app
+photobooth
 ```
 
-Start the app and browse to <http://localhost:8000>.
+Browse to <http://localhost:8000> and see if the app is working properly.
+
+#### Photobooth command not found
+
+If there is a warning as following during pip installation and photobooth can't start check the PATH variable
+
+```text
+WARNING: The script photobooth is installed in '/home/pi/.local/bin' which is not on PATH.
+Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+```
+
+See following is fine, might just need a restart after installation because the path .local/bin did not exist before.
+
+```sh  # ~/.profile
+# set PATH so it includes user's private bin if it exists
+if [ -d "$HOME/.local/bin" ] ; then
+    PATH="$HOME/.local/bin:$PATH"
+fi
+```
+
+#### Install development versions
+
+Stable releases are published at pypi registry.
+To test the latest development version install directly from git:
 
 ```sh
-photobooth # photobooth should be available globally. if file is not found check PATH
+pip install git+https://github.com/mgrl/photobooth-app.git@dev
 ```
 
 ### Integrate Photobooth-Project and this Photobooth-App
 
 Following commands have to be set in photobooth project to use this app as streamingserver.
 Replace <http://photobooth> by the actual hostname or localhost if on same server.
```

