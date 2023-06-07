# Comparing `tmp/FuncsForSPO-5.1.3.tar.gz` & `tmp/FuncsForSPO-5.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FuncsForSPO-5.1.3.tar", last modified: Tue Jun  6 21:55:04 2023, max compression
+gzip compressed data, was "FuncsForSPO-5.1.5.tar", last modified: Wed Jun  7 19:24:08 2023, max compression
```

## Comparing `FuncsForSPO-5.1.3.tar` & `FuncsForSPO-5.1.5.tar`

### file list

```diff
@@ -1,71 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.194774 FuncsForSPO-5.1.3/
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.835671 FuncsForSPO-5.1.3/FuncsForSPO/
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.893951 FuncsForSPO-5.1.3/FuncsForSPO/femails/
--rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.3/FuncsForSPO/femails/__init__.py
--rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.3/FuncsForSPO/femails/femails.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.905167 FuncsForSPO-5.1.3/FuncsForSPO/fexceptions/
--rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fexceptions/__init__.py
--rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.3/FuncsForSPO/fexceptions/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.914652 FuncsForSPO-5.1.3/FuncsForSPO/fftp/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fftp/__init__.py
--rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.3/FuncsForSPO/fftp/fftp.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.921673 FuncsForSPO-5.1.3/FuncsForSPO/flanguage/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.3/FuncsForSPO/flanguage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.925741 FuncsForSPO-5.1.3/FuncsForSPO/flanguage/translator/
--rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.3/FuncsForSPO/flanguage/translator/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.3/FuncsForSPO/flanguage/translator/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.937043 FuncsForSPO-5.1.3/FuncsForSPO/fopenpyxl/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fopenpyxl/__init__.py
--rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.942044 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/
--rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.964466 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/
--rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/__init__.py
--rw-rw-rw-   0        0        0     4310 2023-06-06 21:54:39.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
--rw-rw-rw-   0        0        0     3545 2023-06-05 13:10:09.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/base.py
--rw-rw-rw-   0        0        0     1132 2023-06-02 20:13:34.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.980955 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fcompress/
--rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fcompress/__compress_online.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fcompress/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fcompress/compress.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.998533 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/
--rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
--rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
--rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.004052 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fimgpdf/
--rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.019865 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/focr/
--rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/focr/__init__.py
--rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/focr/__ocr_online.py
--rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpdf/focr/orc.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.029609 FuncsForSPO-5.1.3/FuncsForSPO/fpysimplegui/
--rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpysimplegui/__init__.py
--rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpysimplegui/functions_for_sg.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.039724 FuncsForSPO-5.1.3/FuncsForSPO/fpython/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpython/__init__.py
--rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.3/FuncsForSPO/fpython/functions_for_py.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.050721 FuncsForSPO-5.1.3/FuncsForSPO/fregex/
--rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fregex/__init__.py
--rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.3/FuncsForSPO/fregex/functions_re.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.058959 FuncsForSPO-5.1.3/FuncsForSPO/fselenium/
--rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fselenium/__init__.py
--rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.1.3/FuncsForSPO/fselenium/functions_selenium.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.071907 FuncsForSPO-5.1.3/FuncsForSPO/fsqlite/
--rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.3/FuncsForSPO/fsqlite/__init__.py
--rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.3/FuncsForSPO/fsqlite/sqlite_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.079707 FuncsForSPO-5.1.3/FuncsForSPO/fwinotify/
--rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.3/FuncsForSPO/fwinotify/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.3/FuncsForSPO/fwinotify/fwinotify.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:04.088183 FuncsForSPO-5.1.3/FuncsForSPO/utils/
--rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.3/FuncsForSPO/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 21:55:03.883423 FuncsForSPO-5.1.3/FuncsForSPO.egg-info/
--rw-rw-rw-   0        0        0     8026 2023-06-06 21:55:03.000000 FuncsForSPO-5.1.3/FuncsForSPO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1646 2023-06-06 21:55:03.000000 FuncsForSPO-5.1.3/FuncsForSPO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 21:55:03.000000 FuncsForSPO-5.1.3/FuncsForSPO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-06 21:55:03.000000 FuncsForSPO-5.1.3/FuncsForSPO.egg-info/requires.txt
--rw-rw-rw-   0        0        0      432 2023-06-06 21:55:03.000000 FuncsForSPO-5.1.3/FuncsForSPO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.3/LICENSE
--rw-rw-rw-   0        0        0     8026 2023-06-06 21:55:04.190208 FuncsForSPO-5.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 21:55:04.195781 FuncsForSPO-5.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2421 2023-06-06 21:54:59.000000 FuncsForSPO-5.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.918992 FuncsForSPO-5.1.5/
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.459373 FuncsForSPO-5.1.5/FuncsForSPO/
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.529987 FuncsForSPO-5.1.5/FuncsForSPO/femails/
+-rw-rw-rw-   0        0        0       86 2022-10-17 17:23:21.000000 FuncsForSPO-5.1.5/FuncsForSPO/femails/__init__.py
+-rw-rw-rw-   0        0        0     7124 2023-03-30 20:56:34.000000 FuncsForSPO-5.1.5/FuncsForSPO/femails/femails.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.546845 FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/
+-rw-rw-rw-   0        0        0       18 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-12-18 16:11:53.000000 FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.562395 FuncsForSPO-5.1.5/FuncsForSPO/fftp/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fftp/__init__.py
+-rw-rw-rw-   0        0        0     6205 2022-12-16 20:50:05.000000 FuncsForSPO-5.1.5/FuncsForSPO/fftp/fftp.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.569930 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.575483 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/
+-rw-rw-rw-   0        0        0        0 2023-06-05 14:56:28.000000 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-05 14:56:55.000000 FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.587874 FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/__init__.py
+-rw-rw-rw-   0        0        0    11048 2022-08-16 17:53:19.000000 FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.595445 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.662770 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/
+-rw-rw-rw-   0        0        0      195 2023-06-02 20:07:25.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/__init__.py
+-rw-rw-rw-   0        0        0     6389 2023-06-07 19:18:22.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
+-rw-rw-rw-   0        0        0     3699 2023-06-07 19:14:16.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/base.py
+-rw-rw-rw-   0        0        0     1134 2023-06-07 11:25:27.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+-rw-rw-rw-   0        0        0     2019 2023-06-07 16:48:53.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.685747 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/
+-rw-rw-rw-   0        0        0     9145 2023-06-06 21:38:19.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/__compress_online.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/__init__.py
+-rw-rw-rw-   0        0        0     1640 2023-06-06 21:39:15.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/compress.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.709742 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/
+-rw-rw-rw-   0        0        0     7094 2023-02-23 17:58:00.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
+-rw-rw-rw-   0        0        0      226 2022-11-17 11:12:39.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
+-rw-rw-rw-   0        0        0     1577 2022-11-30 15:19:23.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.715820 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fimgpdf/
+-rw-rw-rw-   0        0        0    12539 2023-02-23 17:58:26.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.734546 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/
+-rw-rw-rw-   0        0        0      129 2022-11-17 11:12:22.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/__init__.py
+-rw-rw-rw-   0        0        0     9646 2023-06-06 20:32:25.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/__ocr_online.py
+-rw-rw-rw-   0        0        0     5303 2023-06-06 20:31:18.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/orc.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.744243 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/pdfutils/
+-rw-rw-rw-   0        0        0       18 2023-06-02 20:07:40.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/pdfutils/__init__.py
+-rw-rw-rw-   0        0        0     1217 2023-06-07 11:50:52.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpdf/pdfutils/pdfutils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.755365 FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/
+-rw-rw-rw-   0        0        0       83 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/__init__.py
+-rw-rw-rw-   0        0        0     4708 2023-01-20 11:52:18.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/functions_for_sg.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.766652 FuncsForSPO-5.1.5/FuncsForSPO/fpython/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpython/__init__.py
+-rw-rw-rw-   0        0        0    67096 2023-06-03 13:16:56.000000 FuncsForSPO-5.1.5/FuncsForSPO/fpython/functions_for_py.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.778837 FuncsForSPO-5.1.5/FuncsForSPO/fregex/
+-rw-rw-rw-   0        0        0       24 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fregex/__init__.py
+-rw-rw-rw-   0        0        0    10406 2023-01-30 14:08:06.000000 FuncsForSPO-5.1.5/FuncsForSPO/fregex/functions_re.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.789803 FuncsForSPO-5.1.5/FuncsForSPO/fselenium/
+-rw-rw-rw-   0        0        0       27 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fselenium/__init__.py
+-rw-rw-rw-   0        0        0    39083 2023-06-06 21:05:50.000000 FuncsForSPO-5.1.5/FuncsForSPO/fselenium/functions_selenium.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.803208 FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/
+-rw-rw-rw-   0        0        0       25 2022-08-09 00:49:14.000000 FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/__init__.py
+-rw-rw-rw-   0        0        0     1610 2022-12-18 16:12:26.000000 FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/sqlite_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.812749 FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/
+-rw-rw-rw-   0        0        0       16 2022-09-12 21:24:16.000000 FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-09-12 21:21:52.000000 FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/fwinotify.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.841307 FuncsForSPO-5.1.5/FuncsForSPO/utils/
+-rw-rw-rw-   0        0        0   114869 2023-03-31 19:29:18.000000 FuncsForSPO-5.1.5/FuncsForSPO/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 19:24:08.514114 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/
+-rw-rw-rw-   0        0        0     8026 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1770 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      194 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      458 2023-06-07 19:24:08.000000 FuncsForSPO-5.1.5/FuncsForSPO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1074 2022-12-02 16:50:42.000000 FuncsForSPO-5.1.5/LICENSE
+-rw-rw-rw-   0        0        0     8026 2023-06-07 19:24:08.913440 FuncsForSPO-5.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7607 2023-01-21 19:11:53.000000 FuncsForSPO-5.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 19:24:08.919992 FuncsForSPO-5.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2506 2023-06-07 19:24:03.000000 FuncsForSPO-5.1.5/setup.py
```

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/femails/femails.py` & `FuncsForSPO-5.1.5/FuncsForSPO/femails/femails.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fexceptions/exceptions.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fexceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fftp/fftp.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fftp/fftp.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/flanguage/translator/translator.py` & `FuncsForSPO-5.1.5/FuncsForSPO/flanguage/translator/translator.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fopenpyxl/openpyxl_funcs.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fopenpyxl/openpyxl_funcs.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     e recupera um arquivo txt com a resposta do GPT
 """
 from FuncsForSPO.fpdf.fanalyser.base import *
 
 class ErroPDFAIException(Exception):
     pass
 
-class GPTPDF(BotMain):    
+class GPTPDFV1(BotMain):    
     def __init__(self, file_pdf: str, credentials:tuple, prompt:str, headless: bool=True) -> str:
         self.PDF_PATH = os.path.abspath(file_pdf)
         self.PROMPT = prompt
         self.HEADLESS = headless
         self.CREDENTIALS = credentials
         super().__init__(self.HEADLESS)
     
@@ -44,21 +44,21 @@
                 except (NoSuchElementException, TimeoutException):
                     break
 
 
             espera_elemento_disponivel_e_clica(self.WDW10, (By.CSS_SELECTOR, 'button:last-of-type span'))
             espera_elemento(self.WDW, (By.CSS_SELECTOR, 'input[type="file"]'), in_dom=True)
             self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.PDF_PATH)
-            espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'div[class*="flex justify-between"]>button'))
+            espera_elemento_disponivel_e_clica(self.WDW330, (By.CSS_SELECTOR, 'div[class*="flex justify-between"]>button'))
 
 
             while True:
                 try:
-                    espera_input_limpa_e_envia_send_keys(self.WDW30, 'é de suma importância que você coloque no inicio da sua resposta: "IA" e me responda em português. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]'))
-                    espera_elemento_disponivel_e_clica(self.WDW30, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]~button'))
+                    espera_input_limpa_e_envia_send_keys(self.WDW330, 'é de suma importância que você coloque no inicio da sua resposta: "IA" e me responda em português. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]'))
+                    espera_elemento_disponivel_e_clica(self.WDW330, (By.CSS_SELECTOR, 'textarea[placeholder*="Send"]~button'))
                     break
                 except ElementClickInterceptedException:
                     try:
                         self.DRIVER.execute_script("arguments[0].remove();", self.DRIVER.find_element(By.CSS_SELECTOR, '#__NEXT_DATA__~ins'))
                     except Exception:
                         pass
             
@@ -72,17 +72,56 @@
                 else:
                     faz_log(f'Resposta até agora: "{text}"')
                     tentativas -= 1
                     sleep(5)
                     continue
             self.DRIVER.get('https://pdf.ai/documents')
             espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, 'a[href="/auth/account"]~button'))
+
+            self.DRIVER.get('https://github.com/settings/sessions')
+            self.DRIVER.get('https://github.com/settings/sessions')
+            self.DRIVER.get('https://github.com/settings/sessions')
+            sessions = espera_e_retorna_conteudo_dos_atributos_dos_elementos_text(self.WDW, 'href', (By.CSS_SELECTOR, 'a[href*="/settings/sessions/"]'))
+            for session in sessions:
+                self.DRIVER.get(session)
+                try:
+                    espera_elemento_disponivel_e_clica(self.WDW, (By.CSS_SELECTOR, '#settings-frame div > form > button'))
+                except (NoSuchElementException, TimeoutException):
+                    pass
             sleep(2)
             self.DRIVER.quit()
             if tentativas == 0:
                 raise ErroPDFAIException('Muitas tentativas, tente uma nova solicitação')
             return text
         except Exception as e:
             faz_log(repr(e), 'c*')
             faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
             self.DRIVER.quit()
             raise ErroPDFAIException
+
+
+class GPTPDFV2(BotMain):    
+    def __init__(self, file_pdf: str, prompt:str, headless: bool=True) -> str:
+        self.PDF_PATH = os.path.abspath(file_pdf)
+        self.PROMPT = prompt
+        self.HEADLESS = headless
+        super().__init__(self.HEADLESS)
+    
+    def run(self):
+        try:
+            self.DRIVER.get('https://askyourpdf.com/')
+            espera_elemento(self.WDW, (By.CSS_SELECTOR, 'input[type="file"]'), in_dom=True)
+            self.DRIVER.find_element(By.CSS_SELECTOR, 'input[type="file"]').send_keys(self.PDF_PATH)
+
+            espera_input_limpa_e_envia_send_keys(self.WDW130, 'Adicione "AI RESPONSE" no final da sua resposta. '+self.PROMPT, (By.CSS_SELECTOR, 'textarea[placeholder="Write your question"]'))
+            espera_elemento_disponivel_e_clica(self.WDW130, (By.CSS_SELECTOR, 'button[class*="ant-btn-default"]'))
+            faz_log('Esperando a resposta')
+            while True:
+                text = espera_e_retorna_elemento_text(self.WDW, (By.CSS_SELECTOR, 'div[style="padding: 5px;"]>div:last-of-type>div:last-of-type span'))
+                if 'AI RES' in text:
+                    break
+            return text
+        except Exception as e:
+            faz_log(repr(e), 'c*')
+            faz_log(self.DRIVER.get_screenshot_as_base64(), 'i*')
+            self.DRIVER.quit()
+            raise ErroPDFAIException
```

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/base.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,46 +26,48 @@
         if headless == True:
             self._options.add_argument('--headless')
             self._options.add_experimental_option("excludeSwitches", ["enable-logging", "enable-automation"])
             self._options.add_experimental_option('useAutomationExtension', False)
             self.user_agent = cria_user_agent()
             # faz_log(self.user_agent)
             # self._options.add_argument(f"--user-agent={self.user_agent}")
-            self._options.add_argument("--disable-web-security")
-            self._options.add_argument("--allow-running-insecure-content")
-            self._options.add_argument("--start-maximized")
-            self._options.add_argument("--no-sandbox")
-            self._options.add_argument('--disable-gpu')
-            self._options.add_argument('--disable-software-rasterizer')
+            # self._options.add_argument("--disable-web-security")
+            # self._options.add_argument("--allow-running-insecure-content")
+            # self._options.add_argument("--start-maximized")
+            # self._options.add_argument("--no-sandbox")
+            # self._options.add_argument('--disable-gpu')
+            # self._options.add_argument('--disable-software-rasterizer')
             self._options.add_argument('--incognito')
             self._options.add_argument("--window-size=1920,1080")
         else:
             self._options.add_experimental_option("excludeSwitches", ["enable-logging", "enable-automation"])
             self._options.add_experimental_option('useAutomationExtension', False)
             self.user_agent = cria_user_agent()
             # faz_log(self.user_agent)
-            self._options.add_argument(f"--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36")
-            self._options.add_argument("--disable-web-security")
-            self._options.add_argument("--allow-running-insecure-content")
-            self._options.add_argument("--start-maximized")
-            self._options.add_argument("--no-sandbox")
-            self._options.add_argument('--disable-gpu')
-            self._options.add_argument('--disable-software-rasterizer')
-            self._options.add_argument('--incognito')
+            # self._options.add_argument(f"--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36")
+            # self._options.add_argument("--disable-web-security")
+            # self._options.add_argument("--allow-running-insecure-content")
+            # self._options.add_argument("--start-maximized")
+            # self._options.add_argument("--no-sandbox")
+            # self._options.add_argument('--disable-gpu')
+            # self._options.add_argument('--disable-software-rasterizer')
+            # self._options.add_argument('--incognito')
             self._options.add_argument("--window-size=1920,1080")
             self._options.add_argument('--kiosk-printing')
 
         
         self.__service = Service(ChromeDriverManager().install())
         
         # create DRIVER
         self.DRIVER = Chrome(service=self.__service, options=self._options)
 
         self.WDW3 = WebDriverWait(self.DRIVER, timeout=3)
         self.WDW5 = WebDriverWait(self.DRIVER, timeout=5)
         self.WDW7 = WebDriverWait(self.DRIVER, timeout=7)
         self.WDW10 = WebDriverWait(self.DRIVER, timeout=10)
         self.WDW30 = WebDriverWait(self.DRIVER, timeout=30)
+        self.WDW130 = WebDriverWait(self.DRIVER, timeout=130)
+        self.WDW330 = WebDriverWait(self.DRIVER, timeout=330)
         self.WDW = self.WDW7
 
         self.DRIVER.maximize_window()
         return self.DRIVER
```

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fanalyser/pdfanalyser.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 	:param file_pdf: A string representing the path to the PDF file.
 	:param prompt: A string representing a prompt to start the analysis.
 	:param credentials: A tuple containing the username and password.
 	:param headless: A boolean indicating if the browser should run in headless mode. Default is True.
 	:return: A string with the analysis result.
 	"""
     # CREDENTIALS EXEMPLE -> (username, password)
-    app = GPTPDF(file_pdf=file_pdf, credentials=credentials, prompt=prompt, headless=headless)
+    app = GPTPDFV1(file_pdf=file_pdf, credentials=credentials, prompt=prompt, headless=headless)
     text = app.run()
     return text
 
 
 # file_pdf='initial_9232.pdf', prompt='analise e me fale em portugues esse pdf', headless=True, credentials=('githubpaycon', 'bolarede792')
```

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fcompress/__compress_online.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/__compress_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fcompress/compress.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fcompress/compress.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/focr/__ocr_online.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/__ocr_online.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpdf/focr/orc.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpdf/focr/orc.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpysimplegui/functions_for_sg.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpysimplegui/functions_for_sg.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fpython/functions_for_py.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fpython/functions_for_py.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fregex/functions_re.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fregex/functions_re.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fselenium/functions_selenium.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fselenium/functions_selenium.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fsqlite/sqlite_functions.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fsqlite/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/fwinotify/fwinotify.py` & `FuncsForSPO-5.1.5/FuncsForSPO/fwinotify/fwinotify.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO/utils/utils.py` & `FuncsForSPO-5.1.5/FuncsForSPO/utils/utils.py`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO.egg-info/PKG-INFO` & `FuncsForSPO-5.1.5/FuncsForSPO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.3
+Version: 5.1.5
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.3/FuncsForSPO.egg-info/SOURCES.txt` & `FuncsForSPO-5.1.5/FuncsForSPO.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,28 @@
 FuncsForSPO/flanguage/translator/translator.py
 FuncsForSPO/fopenpyxl/__init__.py
 FuncsForSPO/fopenpyxl/openpyxl_funcs.py
 FuncsForSPO/fpdf/__init__.py
 FuncsForSPO/fpdf/fanalyser/__init__.py
 FuncsForSPO/fpdf/fanalyser/__pdfanalyser.py
 FuncsForSPO/fpdf/fanalyser/base.py
-FuncsForSPO/fpdf/fanalyser/pdfanalyser.py
+FuncsForSPO/fpdf/fanalyser/pdfanalyser_v1.py
+FuncsForSPO/fpdf/fanalyser/pdfanalyser_v2.py
 FuncsForSPO/fpdf/fcompress/__compress_online.py
 FuncsForSPO/fpdf/fcompress/__init__.py
 FuncsForSPO/fpdf/fcompress/compress.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__html_to_pdf.py
 FuncsForSPO/fpdf/fhtml_to_pdf/__init__.py
 FuncsForSPO/fpdf/fhtml_to_pdf/html_to_pdf.py
 FuncsForSPO/fpdf/fimgpdf/img_to_pdf.py
 FuncsForSPO/fpdf/focr/__init__.py
 FuncsForSPO/fpdf/focr/__ocr_online.py
 FuncsForSPO/fpdf/focr/orc.py
+FuncsForSPO/fpdf/pdfutils/__init__.py
+FuncsForSPO/fpdf/pdfutils/pdfutils.py
 FuncsForSPO/fpysimplegui/__init__.py
 FuncsForSPO/fpysimplegui/functions_for_sg.py
 FuncsForSPO/fpython/__init__.py
 FuncsForSPO/fpython/functions_for_py.py
 FuncsForSPO/fregex/__init__.py
 FuncsForSPO/fregex/functions_re.py
 FuncsForSPO/fselenium/__init__.py
```

### Comparing `FuncsForSPO-5.1.3/LICENSE` & `FuncsForSPO-5.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/PKG-INFO` & `FuncsForSPO-5.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FuncsForSPO
-Version: 5.1.3
+Version: 5.1.5
 Summary: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Home-page: https://github.com/githubpaycon/FuncsForSPO
 Author: Gabriel Lopes de Souza
 Author-email: githubpaycon@gmail.com
 License: MIT License
 Keywords: Funções Para Melhorar Desenvolvimento de Robôs com Selenium
 Description-Content-Type: text/markdown
```

### Comparing `FuncsForSPO-5.1.3/README.md` & `FuncsForSPO-5.1.5/README.md`

 * *Files identical despite different names*

### Comparing `FuncsForSPO-5.1.3/setup.py` & `FuncsForSPO-5.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup
 
-version = '5.1.3'
+version = '5.1.5'
 
 with open("README.md", "r", encoding='utf-8') as fh:
     readme = fh.read()
     setup(
         name='FuncsForSPO',
         version=version,
         url='https://github.com/githubpaycon/FuncsForSPO',
@@ -26,14 +26,15 @@
             os.path.join('FuncsForSPO', 'fpdf'),
             os.path.join('FuncsForSPO', 'fpdf', 'focr'),
             os.path.join('FuncsForSPO', 'fpdf', 'focr'),
             os.path.join('FuncsForSPO', 'fpdf', 'fcompress'),
             os.path.join('FuncsForSPO', 'fpdf', 'fimgpdf'),
             os.path.join('FuncsForSPO', 'fpdf', 'fanalyser'),
             os.path.join('FuncsForSPO', 'fpdf', 'fhtml_to_pdf'),
+            os.path.join('FuncsForSPO', 'fpdf', 'pdfutils'),
             os.path.join('FuncsForSPO', 'fopenpyxl'),
             os.path.join('FuncsForSPO', 'fpysimplegui'),
             os.path.join('FuncsForSPO', 'fpython'),
             os.path.join('FuncsForSPO', 'fpython'),
             os.path.join('FuncsForSPO', 'fregex'),
             os.path.join('FuncsForSPO', 'fselenium'),
             os.path.join('FuncsForSPO', 'fsqlite'),
@@ -53,12 +54,13 @@
             'packaging',
             'PySimpleGUI',
             'macholib',
             'wget',
             'winotify',
             'pypdf',
             'pywin32',
+            'PyPDF2',
             'sqlalchemy',
             'rich==12.6.0',
             'pyinstaller==5.6.2',
         ],
         )
```

