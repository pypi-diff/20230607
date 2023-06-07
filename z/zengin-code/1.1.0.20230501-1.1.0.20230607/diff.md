# Comparing `tmp/zengin_code-1.1.0.20230501.tar.gz` & `tmp/zengin_code-1.1.0.20230607.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zengin_code-1.1.0.20230501.tar", last modified: Mon May  1 06:28:44 2023, max compression
+gzip compressed data, was "zengin_code-1.1.0.20230607.tar", last modified: Wed Jun  7 08:05:51 2023, max compression
```

## Comparing `zengin_code-1.1.0.20230501.tar` & `zengin_code-1.1.0.20230607.tar`

### file list

```diff
@@ -1,1413 +1,1413 @@
-drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-05-01 06:28:44.072435 zengin_code-1.1.0.20230501/
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1077 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/LICENSE.txt
--rw-r--r--   0 sho-kusano   (501) staff       (20)      270 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/MANIFEST.in
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2040 2023-05-01 06:28:44.072518 zengin_code-1.1.0.20230501/PKG-INFO
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1013 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/README.rst
--rw-r--r--   0 sho-kusano   (501) staff       (20)      244 2023-05-01 06:28:44.072803 zengin_code-1.1.0.20230501/setup.cfg
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2088 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/setup.py
-drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-05-01 06:28:43.800756 zengin_code-1.1.0.20230501/tests/
--rw-r--r--   0 sho-kusano   (501) staff       (20)        0 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/tests/__init__.py
--rw-r--r--   0 sho-kusano   (501) staff       (20)      590 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/tests/test_bank.py
--rw-r--r--   0 sho-kusano   (501) staff       (20)      176 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/tox.ini
-drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-05-01 06:28:43.802283 zengin_code-1.1.0.20230501/zengin_code/
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1107 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/zengin_code/__init__.py
--rw-r--r--   0 sho-kusano   (501) staff       (20)      687 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/zengin_code/bank.py
--rw-r--r--   0 sho-kusano   (501) staff       (20)      332 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230501/zengin_code/branch.py
-drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-05-01 06:28:43.799483 zengin_code-1.1.0.20230501/zengin_code/source-data/
-drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-05-01 06:28:43.805046 zengin_code-1.1.0.20230501/zengin_code/source-data/data/
--rw-r--r--   0 sho-kusano   (501) staff       (20)   216855 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/banks.json
-drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-05-01 06:28:44.072163 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/
--rw-r--r--   0 sho-kusano   (501) staff       (20)    69566 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0001.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)   104610 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0005.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    77946 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0009.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    45853 2023-01-16 00:11:02.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0010.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    15589 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0017.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8495 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0033.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2713 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0034.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      140 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0035.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11141 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0036.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3820 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0038.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1610 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0039.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3801 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0040.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1475 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0041.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2201 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0042.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1669 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0043.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      401 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0044.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    19812 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0116.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13453 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0117.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13480 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0118.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13769 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0119.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11526 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0120.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0121.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12148 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0122.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    15005 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0123.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7722 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0124.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    20195 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0125.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16745 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0126.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    20752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0128.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    17260 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0129.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    24063 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0130.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    20263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0131.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0133.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    24572 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0134.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10006 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0135.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    24370 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0137.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    28908 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0138.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    30163 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0140.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12928 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0141.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12243 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0142.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    20484 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0143.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    25533 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0144.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5218 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0145.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0146.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13848 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0147.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    23413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0149.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16236 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0150.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10599 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0151.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    21286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0152.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    21226 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0153.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    23573 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0154.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    17984 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0155.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    18335 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0157.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    23980 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0158.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    35765 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0159.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    19197 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0161.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    17965 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0162.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    15519 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0163.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9223 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0164.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8802 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0166.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    20666 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0167.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    22077 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0168.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    21098 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0169.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16580 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0170.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13460 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0172.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16508 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0173.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    19973 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0174.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0175.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    22509 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0177.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5850 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0178.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13718 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0179.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13596 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0180.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    27341 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0181.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0182.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12162 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0183.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13592 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0184.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    20654 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0185.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9024 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0187.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8509 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0188.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    23453 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0190.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5017 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0191.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6905 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0288.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4729 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0289.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    19219 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0294.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0295.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0297.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4116 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0300.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    37975 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0304.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      264 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0307.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0309.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16012 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0310.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0311.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0320.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0321.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1591 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0322.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0324.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0325.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4794 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0397.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3070 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0398.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      403 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0401.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0402.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0403.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1609 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0411.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0413.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0414.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      354 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0421.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      396 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0423.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0424.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0425.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0426.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0429.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0430.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      554 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0432.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0438.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0439.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0442.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0443.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0444.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0445.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0456.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0457.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0458.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0460.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0461.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0463.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0468.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0471.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2049 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0472.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0477.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0482.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0484.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0485.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0487.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      963 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0489.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0495.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0498.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    23900 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0501.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    19098 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0508.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10420 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0509.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9773 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0512.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7096 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0513.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7528 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0514.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12357 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0516.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11127 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0517.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16658 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0522.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11217 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0525.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13450 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0526.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4611 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0530.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9444 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0532.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7072 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0533.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8960 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0534.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4917 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0537.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5941 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0538.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14093 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0542.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    15557 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0543.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12090 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0544.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12990 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0546.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    18697 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0554.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4306 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0555.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14184 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0562.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4681 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0565.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8036 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0566.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14084 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0569.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7940 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0570.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13892 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0572.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12075 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0573.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14592 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0576.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9344 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0578.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5398 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0582.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4332 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0583.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2987 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0585.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9364 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0587.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5392 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0590.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7274 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0591.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8553 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0594.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6444 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0596.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11952 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0597.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0603.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0607.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0608.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0611.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0612.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0615.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0616.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      273 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0617.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0619.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0621.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0623.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0624.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0625.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0626.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0627.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0629.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0630.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0631.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0632.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0633.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1733 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1000.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10787 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1001.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3833 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1003.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2742 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1004.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3928 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1006.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3109 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1008.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      945 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1009.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1867 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1010.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1037 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1011.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1425 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1012.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1475 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1013.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2646 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1014.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1764 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1016.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4907 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1018.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5472 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1020.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3100 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1021.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2362 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1022.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2887 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1024.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4045 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1026.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2387 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1027.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3250 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1028.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1030.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2445 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1031.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2524 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1033.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2341 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1104.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5567 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1105.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2174 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1120.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1123.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1677 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1140.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1685 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1141.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1751 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1142.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1041 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1143.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3014 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1150.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      767 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1152.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2168 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1153.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1236 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1154.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1201 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1155.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1389 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1156.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3629 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1170.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1755 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1171.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1675 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1172.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2192 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1174.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1445 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1175.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2385 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1181.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2482 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1182.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2106 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1184.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1185.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2036 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1186.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1895 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1188.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      894 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1189.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3048 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1190.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3362 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1203.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4163 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1204.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2207 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1206.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2064 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1208.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1215 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1209.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1458 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1210.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7017 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1211.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3099 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1221.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2072 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1222.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1548 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1223.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1003 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1224.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1106 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1225.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1359 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1227.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8545 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1240.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3117 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1242.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13023 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1250.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6157 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1251.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4857 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1252.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6808 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1253.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6463 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1260.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3675 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1261.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3541 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1262.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1731 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1264.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2016 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1267.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8312 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1280.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6225 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1281.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6427 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1282.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7673 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1283.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3249 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1286.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4350 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1288.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1289.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2191 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1290.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8094 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1303.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1305.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7517 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1310.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4176 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1311.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6724 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1319.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9076 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1320.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1311 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1321.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3076 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1323.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1366 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1326.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3156 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1327.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1333.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3929 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1336.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10623 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1341.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11360 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1344.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2701 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1345.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1444 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1346.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1348.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4124 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1349.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11471 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1351.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3087 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1352.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6031 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1356.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4930 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1358.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11762 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1360.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2750 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1370.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2046 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1371.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3380 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1373.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1056 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1374.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      895 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1375.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1963 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1376.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1524 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1377.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      881 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1379.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      884 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1380.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2673 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1385.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4348 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1386.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5104 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1390.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3479 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1391.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2999 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1392.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2827 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1393.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2978 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1394.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2511 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1396.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3829 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1401.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2675 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1402.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      904 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1404.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1338 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1405.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      901 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1406.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1173 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1412.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      528 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1413.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4365 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1440.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3085 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1442.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2882 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1444.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1678 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1445.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2538 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1448.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5108 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1470.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1051 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1471.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1520 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1472.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      930 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1473.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1475.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7238 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1501.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5488 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1502.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11366 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1503.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4096 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1505.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6669 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1506.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2417 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1507.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1509.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4340 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1511.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3832 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1512.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6902 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1513.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2751 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1515.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3193 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1517.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11978 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1530.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4181 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1531.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2511 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1532.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6703 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1533.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1576 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1534.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1152 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1538.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1789 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1540.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2612 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1550.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4473 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1551.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13611 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1552.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6126 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1553.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9642 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1554.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2557 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1555.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4773 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1556.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4462 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1557.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5611 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1559.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10713 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1560.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6635 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1561.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5932 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1562.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3244 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1563.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1565.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2529 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1566.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      787 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1580.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3755 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1581.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2405 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1582.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1583.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      881 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1585.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4203 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1602.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2030 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1603.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1586 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1604.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12613 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1610.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    18054 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1611.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5013 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1620.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9544 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1630.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3850 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1633.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11899 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1635.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2748 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1636.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2419 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1643.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9011 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1645.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1656.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1879 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1666.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2428 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1667.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1696 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1668.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1031 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1671.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5624 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1674.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3651 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1680.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5902 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1685.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8797 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1686.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4933 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1687.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11586 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1688.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1689.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3374 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1691.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3407 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1692.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3519 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1694.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3915 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1695.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4492 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1696.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2440 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1701.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1954 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1702.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      966 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1703.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1607 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1710.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1269 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1711.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2678 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1712.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4327 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1732.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2187 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1734.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1735.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2594 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1738.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1295 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1740.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1589 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1741.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1240 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1742.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2211 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1743.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9711 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1750.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5702 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1752.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2898 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1756.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1165 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1758.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2643 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1780.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6749 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1781.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3578 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1789.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2203 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1801.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1803.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4245 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1830.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2177 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1833.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6458 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1860.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1310 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1862.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1358 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1864.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      734 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1866.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1724 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1880.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3575 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1881.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2009 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1901.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5619 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1903.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1828 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1908.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1737 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1909.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2654 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1910.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1123 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1913.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1281 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1917.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2146 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1920.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1060 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1930.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1419 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1931.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1199 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1932.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2351 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1933.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1679 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1942.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1951.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3142 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1952.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1954.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1470 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1955.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3250 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1960.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4142 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1962.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      613 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1968.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3639 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1980.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1201 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1981.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1060 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1982.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3190 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1985.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1986.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1990.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7731 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1991.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1938 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1993.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2390 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1996.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    11863 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2004.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1221 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2010.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3342 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2011.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1782 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2013.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      862 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2014.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      643 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2017.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1204 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2019.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1023 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2024.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1480 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2025.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3047 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2030.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2045.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2049.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2070 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2060.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1556 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2061.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1229 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2062.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      633 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2063.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2075.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1496 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2083.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1022 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2084.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      935 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2085.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2087.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2164 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2090.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2092.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1809 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2095.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1788 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2096.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10851 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2101.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      750 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2122.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1222 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2125.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1703 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2143.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2975 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2146.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4705 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2149.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2151.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2162.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1161 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2165.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1132 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2167.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1703 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2180.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2828 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2184.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1918 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2190.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1418 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2202.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2210.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2211.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      128 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2213.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2215.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      509 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2224.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      522 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2226.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      879 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2229.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2231.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2323 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2235.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2179 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2241.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      975 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2243.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5429 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2248.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3022 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2254.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      508 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2266.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      937 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2271.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2272.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      395 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2274.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2276.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2185 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2277.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      533 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2304.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2305.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3832 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2306.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2307.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      426 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2315.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      534 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2318.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2332.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2351.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2354.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      624 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2356.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1391 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2357.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      757 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2358.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1837 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2360.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      868 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2361.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2362.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1293 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2363.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      664 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2365.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2366.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4383 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2377.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2378.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6717 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2390.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2402.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1466 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2404.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      373 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2411.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2417.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2430.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2435.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2440.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1025 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2442.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2443.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2444.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2446.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2447.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1424 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2448.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1535 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2451.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      482 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2452.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2470.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2471.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2473.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2078 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2476.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      777 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2481.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2485.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      786 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2504.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1409 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2505.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      636 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2526.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2143 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2540.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2404 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2541.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1890 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2543.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      381 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2548.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1984 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2549.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2556.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2560.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      273 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2566.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4266 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2567.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2580.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      397 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2581.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1195 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2582.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2602.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      538 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2605.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3064 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2606.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2610.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2826 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2616.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      929 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2620.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2634.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      662 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2661.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1821 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2672.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2673.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2125 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2674.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4565 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2680.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3166 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2681.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1407 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2684.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2686.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1822 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2690.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1689 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2696.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      520 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2703.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2247 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2721.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      244 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2740.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2741.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2751.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2753.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1948 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2763.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5366 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2773.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1952 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2778.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2802.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1042 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2803.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2808.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      938 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2820.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2821.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      733 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2825.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      389 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2826.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      245 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2833.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1155 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2840.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2842.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2845.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4850 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2870.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2884.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3295 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2890.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2891.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2895.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2950.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4932 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2951.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8816 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2954.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    18089 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2963.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3433 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2965.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2847 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2966.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3311 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2968.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3166 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2970.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5415 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2972.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7271 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2978.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4945 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2984.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3190 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2987.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    10570 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2990.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1433 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2997.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2551 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3000.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      596 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3001.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3003.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3008.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3011.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      297 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3013.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3014.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3015.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      408 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3016.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3017.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3019.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3020.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3021.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3022.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3023.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3024.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3025.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3026.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      273 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3027.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      497 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3028.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3030.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3031.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3034.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      471 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3035.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3036.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3037.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      299 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3038.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      282 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3039.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3040.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3041.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      272 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3044.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3045.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3046.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3056.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3058.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      518 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3066.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2219 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3068.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      531 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3086.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3087.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3094.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3095.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3103.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3107.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      905 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3112.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3114.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      648 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3120.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3122.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3124.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3125.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3126.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3129.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1690 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3133.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1070 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3139.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      268 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3142.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      403 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3145.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3147.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3154.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      915 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3156.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3161.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3164.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3165.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3168.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      282 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3170.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      518 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3172.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3173.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      256 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3175.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      664 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3177.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3181.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      388 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3188.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1050 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3189.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      377 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3200.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3201.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1028 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3202.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3206.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3208.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1156 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3210.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3214.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      410 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3219.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3220.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3223.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3224.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3225.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3227.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3228.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      824 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3231.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3238.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      387 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3244.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      394 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3248.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3254.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      401 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3257.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3259.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3260.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      270 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3261.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      574 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3264.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3265.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3266.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3267.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3268.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3269.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3270.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3271.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3273.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3275.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3276.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3277.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3278.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3279.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3280.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3281.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3282.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      385 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3283.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3285.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3286.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3287.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3288.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3289.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3290.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      253 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3297.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      570 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3301.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3303.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3305.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      550 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3306.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1055 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3317.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3319.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3320.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3321.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3322.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      550 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3326.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3328.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3329.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3330.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3334.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3335.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3336.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3337.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3338.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3339.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3348.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3349.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3350.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      572 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3354.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3358.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3373.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1412 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3387.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      377 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3390.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1933 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3407.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      713 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3421.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      372 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3442.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1329 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3455.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      548 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3469.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3474.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3488.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2284 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3517.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3539.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      620 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3541.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3677 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3553.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1022 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3572.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      400 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3579.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1634 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3590.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      774 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3598.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2776 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3636.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      243 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3647.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      916 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3652.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      916 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3653.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      792 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3664.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1279 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3665.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      912 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3682.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2000 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3702.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      616 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3704.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      245 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3710.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3717.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4053 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3721.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1690 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3731.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1308 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3751.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      528 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3762.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      816 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3764.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3771.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3773.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      539 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3784.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3795.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      673 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3798.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      625 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3805.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2132 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3810.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2225 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3825.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3855.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1298 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3878.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      908 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3913.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3917.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3929.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3931.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2299 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3932.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3938.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1177 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3943.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3960.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      564 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3962.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3971.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1026 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3973.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      770 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3980.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3986.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3987.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1205 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3989.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      629 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4000.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1161 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4013.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4022.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1287 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4027.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4036.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8853 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4047.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4265 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4064.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1202 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4069.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2445 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4076.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2481 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4091.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      772 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4104.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1365 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4125.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1032 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4130.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      943 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4132.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1297 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4148.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5099 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4160.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2104 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4175.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1015 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4189.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5886 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4196.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      900 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4197.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1259 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4220.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1844 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4230.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1098 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4238.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3554 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4263.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4294.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4295.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      370 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4296.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1127 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4301.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      640 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4310.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      503 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4322.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      244 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4324.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2063 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4344.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1179 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4357.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4363.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4371.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      744 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4378.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4387.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      643 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4394.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1441 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4397.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1029 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4413.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      886 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4422.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      705 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4425.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1866 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4445.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      844 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4456.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      870 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4463.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1199 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4478.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1126 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4490.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1038 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4497.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1236 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4507.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      652 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4518.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1547 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4523.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      976 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4533.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4540.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4544.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1937 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4563.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      749 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4567.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      635 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4593.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      914 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4594.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      995 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4608.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      375 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4613.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      708 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4626.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      378 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4628.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1031 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4632.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1151 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4652.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1188 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4664.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1324 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4665.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2207 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4677.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6106 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4682.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      482 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4688.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4691.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1257 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4693.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      641 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4714.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4726.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      742 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4730.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5281 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4735.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1949 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4780.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      506 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4792.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      953 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4802.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1412 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4808.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4820.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4821.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4823.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1457 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4828.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      729 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4847.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1453 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4848.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1314 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4859.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1200 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4864.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      586 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4874.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2144 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4876.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1138 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4893.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      644 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4902.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1661 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4909.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1285 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4916.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1853 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4929.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      990 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4949.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1997 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4954.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      515 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4955.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1730 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4959.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4962.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2052 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4965.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2462 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4975.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      766 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4992.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4993.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      388 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4996.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1283 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5000.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5002.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5011.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2504 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5016.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1041 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5030.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      638 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5037.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      919 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5039.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      926 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5050.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      601 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5055.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1222 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5060.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1934 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5070.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1228 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5072.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1438 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5077.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1453 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5087.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1705 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5094.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5095.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1974 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5097.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1934 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5100.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      311 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5111.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6809 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5114.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5009 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5123.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1047 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5128.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5130.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5564 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5131.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2793 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5137.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1143 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5139.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1094 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5140.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3817 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5147.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1793 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5152.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      796 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5153.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2039 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5159.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      908 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5162.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      652 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5169.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      819 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5199.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1318 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5207.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1140 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5209.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      818 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5222.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      902 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5234.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      674 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5243.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      505 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5260.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1807 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5272.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5284.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      264 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5287.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      941 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5311.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5330.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1715 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5335.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1193 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5348.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1427 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5372.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2152 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5384.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2191 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5405.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5437.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      506 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5441.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5447.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2932 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5448.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5449.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5462.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      903 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5466.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      760 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5470.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5477.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      892 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5483.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      635 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5485.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5491.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      380 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5493.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3793 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5499.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5524.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      393 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5541.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5542.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      253 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5550.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      896 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5554.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5568.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1726 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5577.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      529 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5585.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3911 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5600.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1186 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5631.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3095 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5666.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5685.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      435 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5690.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5693.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      777 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5706.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1041 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5707.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1316 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5714.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5719.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      708 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5720.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3400 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5768.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      628 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5797.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5815.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      640 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5823.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      864 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5832.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5847.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5864.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      633 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5877.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      758 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5883.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      536 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5884.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      631 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5885.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      544 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5888.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      781 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5895.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5897.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1177 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5898.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5905.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5906.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1343 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5911.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1159 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5916.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      764 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5920.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1202 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5921.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      401 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5927.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      623 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5932.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5935.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1146 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5943.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1375 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5962.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5980.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      658 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5982.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5997.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6010.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      768 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6012.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      894 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6024.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1378 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6025.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      790 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6062.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      382 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6076.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      381 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6084.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1310 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6094.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      877 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6113.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6117.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6121.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6122.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6268 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6129.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4046 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6175.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1399 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6198.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6019 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6242.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3620 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6265.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2423 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6287.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3914 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6313.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1566 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6328.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      910 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6333.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1351 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6338.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1137 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6342.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14009 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6345.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2034 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6351.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2417 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6355.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1516 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6357.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6363.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2360 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6373.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3465 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6377.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1171 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6382.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      822 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6386.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1694 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6387.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3686 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6391.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7804 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6403.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      256 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6423.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6426.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3891 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6430.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      815 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6436.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6443.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2700 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6451.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1285 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6456.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2672 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6466.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1995 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6470.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3515 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6483.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      880 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6503.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1629 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6514.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6441 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6531.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4296 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6552.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2620 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6560.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3027 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6572.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4326 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6582.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6591.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1008 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6606.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1898 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6612.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1153 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6615.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2282 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6618.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6766 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6649.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3978 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6665.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1428 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6673.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2400 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6677.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      545 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6678.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1239 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6690.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      933 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6697.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3004 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6731.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      992 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6741.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1498 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6758.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      551 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6762.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      496 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6770.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7182 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6785.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      393 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6789.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6805.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      746 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6810.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      515 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6823.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1459 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6832.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1362 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6836.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6838.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      870 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6841.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      645 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6853.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1166 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6860.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1037 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6863.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5520 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6874.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1160 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6883.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      859 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6885.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1138 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6888.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6889.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2342 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6897.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6900.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6909.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      381 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6911.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2055 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6912.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1232 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6919.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1125 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6924.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6931.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      251 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6932.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6933.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6935.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2130 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6941.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1940 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6956.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2421 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6961.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3994 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6990.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1796 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6996.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      593 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7025.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7029.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      608 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7032.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1960 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7041.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1584 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7087.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3132 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7092.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2974 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7111.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3950 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7139.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1724 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7156.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3576 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7164.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      805 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7184.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7191.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3618 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7193.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1321 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7200.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8359 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7213.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      847 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7239.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2013 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7240.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1666 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7249.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2041 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7264.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7274.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     8151 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7288.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7316.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      492 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7326.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2841 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7338.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      890 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7353.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      949 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7362.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7363.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1114 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7373.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9622 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7387.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2219 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7532.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      684 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7541.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      876 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7543.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1442 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7550.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1004 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7559.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1666 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7565.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2212 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7576.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      761 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7591.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3583 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7601.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2187 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7625.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4369 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7641.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13243 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7708.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5045 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7755.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7768.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4344 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7794.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1786 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7825.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12534 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7837.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1638 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7847.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1010 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7859.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1975 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7868.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1149 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7889.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4162 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7909.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1845 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7913.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1019 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7916.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1782 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7938.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1268 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7981.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    13089 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7994.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      392 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8011.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8019.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1680 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8027.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2082 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8029.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7662 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8047.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1480 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8069.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8076.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      625 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8096.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      992 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8102.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      989 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8103.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1158 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8118.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    16034 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8134.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      998 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8143.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1433 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8153.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1664 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8166.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8181.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      768 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8197.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      884 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8200.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1027 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8223.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1161 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8231.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      852 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8234.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      522 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8242.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8252.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      266 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8257.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8261.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8263.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      620 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8268.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8288.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      253 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8296.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8300.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8301.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8305.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      247 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8312.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      989 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8323.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    12629 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8332.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      992 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8389.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8395.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1649 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8397.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2028 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8398.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2673 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8400.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      243 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8401.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4898 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8425.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1521 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8457.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1303 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8463.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8477.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1079 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8482.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8500.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8511.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1767 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8512.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      888 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8514.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      896 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8524.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8528.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8536.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      772 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8544.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1738 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8551.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8559.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      360 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8575.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     7501 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8582.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1298 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8589.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8592.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8593.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1926 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8610.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1027 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8621.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1607 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8626.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1406 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8632.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4186 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8633.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1240 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8635.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     4148 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8636.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1149 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8645.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      516 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8653.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      653 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8656.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8660.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8664.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      516 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8667.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1559 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8668.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      934 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8680.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1459 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8689.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8692.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      765 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8694.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1378 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8701.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1232 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8715.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1463 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8730.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8740.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     6758 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8762.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1363 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8766.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1045 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8771.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1839 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8794.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2148 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8813.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2308 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8829.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1782 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8857.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8893.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      363 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8905.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      541 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8906.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2892 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8916.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1979 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8926.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8934.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      881 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8941.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8949.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      862 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8964.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      857 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8982.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1173 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9010.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1318 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9017.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      647 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9043.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      652 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9048.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      510 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9069.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9070.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9072.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      406 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9103.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     5122 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9104.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      260 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9137.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9140.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9145.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1546 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9169.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9177.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1871 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9178.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9181.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2091 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9184.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      744 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9193.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      505 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9197.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      392 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9200.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      248 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9203.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      531 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9205.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9208.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1798 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9213.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      651 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9221.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2532 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9229.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9234.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      404 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9240.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      953 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9251.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      784 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9257.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1332 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9270.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1981 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9296.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1250 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9302.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1860 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9319.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      899 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9332.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9338.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1562 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9341.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9347.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      654 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9353.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1537 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9363.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     9515 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9375.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      887 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9450.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9451.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1150 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9452.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      649 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9453.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9456.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      374 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9457.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     3508 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9461.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9462.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9463.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9466.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      365 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9467.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9468.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9470.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9471.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      387 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9472.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      505 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9473.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      367 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9475.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1264 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9477.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      504 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9479.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9480.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      882 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9481.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      914 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9483.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1164 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9484.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9485.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      649 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9486.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      265 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9487.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      398 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9488.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)     1758 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9489.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      533 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9490.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9491.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9493.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      526 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9494.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9495.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9496.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)    14024 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9900.json
--rw-r--r--   0 sho-kusano   (501) staff       (20)       32 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/md5
--rw-r--r--   0 sho-kusano   (501) staff       (20)        8 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230501/zengin_code/source-data/data/updated_at
-drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-05-01 06:28:43.802944 zengin_code-1.1.0.20230501/zengin_code.egg-info/
--rw-r--r--   0 sho-kusano   (501) staff       (20)     2040 2023-05-01 06:28:43.000000 zengin_code-1.1.0.20230501/zengin_code.egg-info/PKG-INFO
--rw-r--r--   0 sho-kusano   (501) staff       (20)    66979 2023-05-01 06:28:43.000000 zengin_code-1.1.0.20230501/zengin_code.egg-info/SOURCES.txt
--rw-r--r--   0 sho-kusano   (501) staff       (20)        1 2023-05-01 06:28:43.000000 zengin_code-1.1.0.20230501/zengin_code.egg-info/dependency_links.txt
--rw-r--r--   0 sho-kusano   (501) staff       (20)        4 2023-05-01 06:28:43.000000 zengin_code-1.1.0.20230501/zengin_code.egg-info/requires.txt
--rw-r--r--   0 sho-kusano   (501) staff       (20)       12 2023-05-01 06:28:43.000000 zengin_code-1.1.0.20230501/zengin_code.egg-info/top_level.txt
+drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-06-07 08:05:51.122763 zengin_code-1.1.0.20230607/
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1077 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/LICENSE.txt
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      270 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/MANIFEST.in
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2040 2023-06-07 08:05:51.122848 zengin_code-1.1.0.20230607/PKG-INFO
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1013 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/README.rst
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      244 2023-06-07 08:05:51.123148 zengin_code-1.1.0.20230607/setup.cfg
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2088 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/setup.py
+drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-06-07 08:05:50.854752 zengin_code-1.1.0.20230607/tests/
+-rw-r--r--   0 sho-kusano   (501) staff       (20)        0 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/tests/__init__.py
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      590 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/tests/test_bank.py
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      176 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/tox.ini
+drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-06-07 08:05:50.855175 zengin_code-1.1.0.20230607/zengin_code/
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1107 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/zengin_code/__init__.py
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      687 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/zengin_code/bank.py
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      332 2023-01-15 23:57:10.000000 zengin_code-1.1.0.20230607/zengin_code/branch.py
+drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-06-07 08:05:50.853514 zengin_code-1.1.0.20230607/zengin_code/source-data/
+drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-06-07 08:05:50.857736 zengin_code-1.1.0.20230607/zengin_code/source-data/data/
+-rw-r--r--   0 sho-kusano   (501) staff       (20)   216855 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/banks.json
+drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-06-07 08:05:51.122527 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    69566 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0001.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)   104610 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0005.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    77946 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0009.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    45853 2023-01-16 00:11:02.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0010.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    15589 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0017.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8474 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0033.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2713 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0034.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      140 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0035.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11141 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0036.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3820 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0038.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1610 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0039.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3801 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0040.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1475 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0041.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2201 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0042.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1669 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0043.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      401 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0044.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    19812 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0116.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13453 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0117.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13480 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0118.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13769 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0119.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11526 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0120.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0121.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12148 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0122.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    15005 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0123.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7722 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0124.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    20195 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0125.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16745 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0126.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    20752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0128.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    17260 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0129.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    24063 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0130.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    20263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0131.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0133.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    24572 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0134.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10006 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0135.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    24370 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0137.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    28908 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0138.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    30163 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0140.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12928 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0141.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12243 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0142.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    20484 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0143.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    25533 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0144.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5218 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0145.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14284 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0146.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13848 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0147.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    23413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0149.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16095 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0150.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10599 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0151.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    21286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0152.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    21226 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0153.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    23573 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0154.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    17984 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0155.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    18335 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0157.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    23980 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0158.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    35765 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0159.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    19197 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0161.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    17965 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0162.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    15519 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0163.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9223 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0164.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8802 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0166.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    20666 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0167.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    22077 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0168.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    21098 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0169.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16580 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0170.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13460 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0172.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16508 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0173.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    19973 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0174.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0175.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    22509 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0177.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5850 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0178.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13718 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0179.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13596 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0180.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    27341 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0181.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0182.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12162 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0183.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13592 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0184.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    20654 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0185.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9024 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0187.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8509 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0188.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    23453 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0190.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5017 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0191.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6905 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0288.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4729 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0289.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    19219 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0294.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0295.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0297.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4116 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0300.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    38033 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0304.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0307.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0309.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16012 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0310.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0311.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0320.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0321.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1591 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0322.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0324.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0325.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4794 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0397.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3070 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0398.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      403 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0401.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0402.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0403.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1609 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0411.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0413.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0414.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      354 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0421.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      396 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0423.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0424.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0425.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0426.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0429.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0430.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      554 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0432.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0438.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0439.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0442.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0443.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0444.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0445.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0456.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0457.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0458.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0460.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0461.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0463.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0468.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0471.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2049 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0472.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0477.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0482.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0484.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0485.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0487.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      963 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0489.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0495.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0498.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    23900 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0501.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    19098 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0508.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10420 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0509.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9773 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0512.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7096 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0513.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7528 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0514.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12357 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0516.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11127 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0517.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16658 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0522.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11217 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0525.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13450 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0526.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4611 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0530.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9444 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0532.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7072 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0533.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8960 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0534.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4917 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0537.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5941 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0538.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14093 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0542.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    15557 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0543.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12222 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0544.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12990 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0546.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    18697 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0554.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4306 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0555.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14184 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0562.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4681 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0565.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8036 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0566.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14084 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0569.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7940 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0570.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13892 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0572.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12075 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0573.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14592 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0576.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9344 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0578.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5398 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0582.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4332 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0583.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2987 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0585.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9364 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0587.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5392 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0590.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7274 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0591.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8553 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0594.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6444 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0596.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11952 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0597.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0603.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0607.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0608.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0611.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0612.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0615.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0616.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      273 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0617.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0619.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0621.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0623.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0624.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      267 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0625.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0626.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0627.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0629.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0630.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0631.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0632.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0633.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1733 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1000.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10787 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1001.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3833 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1003.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2742 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1004.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3928 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1006.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3109 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1008.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      945 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1009.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1867 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1010.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1037 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1011.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1425 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1012.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1475 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1013.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2646 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1014.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1764 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1016.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4907 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1018.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5472 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1020.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3100 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1021.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2362 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1022.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2887 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1024.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4045 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1026.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2387 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1027.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3250 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1028.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1030.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2445 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1031.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2524 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1033.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2341 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1104.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5567 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1105.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2174 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1120.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1123.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1677 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1140.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1685 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1141.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1751 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1142.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1041 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1143.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3014 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1150.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      767 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1152.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2168 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1153.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1236 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1154.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1201 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1155.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1389 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1156.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3629 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1170.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1755 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1171.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1675 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1172.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2192 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1174.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1445 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1175.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2385 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1181.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2482 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1182.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2106 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1184.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1185.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2036 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1186.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1895 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1188.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      894 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1189.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3048 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1190.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3362 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1203.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4163 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1204.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2207 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1206.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2064 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1208.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1215 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1209.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1458 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1210.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7017 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1211.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3099 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1221.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2072 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1222.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1548 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1223.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1003 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1224.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1106 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1225.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1359 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1227.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8545 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1240.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3117 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1242.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13023 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1250.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6157 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1251.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4857 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1252.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6808 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1253.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6463 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1260.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3675 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1261.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3541 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1262.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1731 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1264.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2016 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1267.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8312 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1280.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6225 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1281.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6427 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1282.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7673 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1283.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3249 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1286.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4350 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1288.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1289.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2191 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1290.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8094 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1303.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1305.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7517 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1310.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4176 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1311.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6724 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1319.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9076 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1320.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1311 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1321.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3076 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1323.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1366 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1326.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3156 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1327.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1333.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3929 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1336.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10623 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1341.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11360 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1344.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2701 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1345.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1444 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1346.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1348.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4124 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1349.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11471 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1351.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3087 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1352.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6031 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1356.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4930 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1358.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11762 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1360.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2750 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1370.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2046 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1371.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3380 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1373.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1056 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1374.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      895 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1375.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1963 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1376.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1524 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1377.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      881 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1379.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      884 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1380.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2673 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1385.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4348 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1386.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5104 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1390.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3479 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1391.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2999 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1392.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2827 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1393.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2978 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1394.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2511 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1396.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3829 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1401.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2675 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1402.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      904 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1404.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1338 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1405.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      901 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1406.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1173 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1412.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      528 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1413.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4365 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1440.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3085 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1442.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2882 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1444.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1678 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1445.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2538 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1448.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5108 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1470.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1051 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1471.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1520 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1472.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      930 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1473.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1475.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7238 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1501.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5488 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1502.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11366 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1503.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4096 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1505.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6669 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1506.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2417 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1507.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1509.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4340 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1511.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3832 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1512.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6902 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1513.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2751 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1515.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3193 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1517.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11978 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1530.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4181 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1531.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2511 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1532.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6703 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1533.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1576 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1534.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1152 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1538.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1789 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1540.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2612 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1550.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4473 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1551.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13611 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1552.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6126 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1553.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9642 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1554.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2557 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1555.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4773 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1556.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4462 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1557.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5611 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1559.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10713 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1560.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6635 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1561.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5932 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1562.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3244 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1563.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1565.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2529 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1566.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      787 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1580.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3755 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1581.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2405 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1582.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1583.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      881 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1585.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4203 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1602.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2030 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1603.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1586 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1604.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12613 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1610.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    18054 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1611.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5013 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1620.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9544 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1630.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3850 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1633.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11899 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1635.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2748 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1636.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2419 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1643.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9011 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1645.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1656.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1879 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1666.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2428 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1667.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1696 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1668.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1031 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1671.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5624 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1674.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3651 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1680.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5902 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1685.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8797 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1686.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4933 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1687.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11586 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1688.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1689.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3374 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1691.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3407 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1692.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3519 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1694.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3915 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1695.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4492 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1696.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2440 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1701.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1954 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1702.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      966 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1703.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1607 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1710.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1269 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1711.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2521 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1712.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4327 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1732.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2187 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1734.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1735.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2594 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1738.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1295 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1740.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1589 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1741.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1240 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1742.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2211 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1743.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9711 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1750.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5702 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1752.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2898 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1756.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1165 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1758.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2643 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1780.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6749 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1781.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3578 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1789.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2203 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1801.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1803.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4245 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1830.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2177 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1833.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6334 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1860.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1310 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1862.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1358 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1864.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      734 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1866.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1724 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1880.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3575 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1881.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2009 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1901.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5619 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1903.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1828 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1908.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1737 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1909.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2654 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1910.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1123 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1913.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1414 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1917.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2146 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1920.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1060 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1930.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1419 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1931.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1199 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1932.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2351 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1933.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1679 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1942.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1951.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3142 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1952.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1954.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1470 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1955.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3250 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1960.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4142 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1962.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      613 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1968.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3639 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1980.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1201 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1981.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1060 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1982.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3190 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1985.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1986.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1990.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7731 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1991.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1938 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1993.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2390 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1996.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    11863 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2004.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1221 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2010.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3342 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2011.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1782 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2013.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      862 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2014.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      643 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2017.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1204 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2019.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1023 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2024.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1480 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2025.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3047 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2030.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2045.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2049.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2070 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2060.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1556 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2061.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1229 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2062.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      633 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2063.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2075.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1496 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2083.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1022 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2084.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      935 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2085.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2087.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2164 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2090.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2092.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1809 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2095.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1788 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2096.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10851 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2101.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      750 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2122.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1222 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2125.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1703 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2143.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2975 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2146.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4705 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2149.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2151.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2162.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1161 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2165.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1132 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2167.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1703 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2180.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2828 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2184.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1918 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2190.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1418 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2202.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2210.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2211.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      128 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2213.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2215.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      509 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2224.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      522 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2226.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      879 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2229.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2231.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2323 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2235.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2179 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2241.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      975 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2243.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5429 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2248.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3022 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2254.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      508 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2266.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      937 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2271.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2272.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      395 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2274.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2276.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2185 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2277.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      533 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2304.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2305.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3832 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2306.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2307.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      426 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2315.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      534 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2318.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2332.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2351.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2354.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      624 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2356.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1391 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2357.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      757 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2358.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1837 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2360.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      868 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2361.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1088 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2362.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1293 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2363.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      664 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2365.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2366.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4383 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2377.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2378.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6717 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2390.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2402.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1466 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2404.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      373 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2411.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2417.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2430.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2435.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2440.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1025 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2442.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2443.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2444.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2446.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2447.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1424 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2448.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1535 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2451.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      482 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2452.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2470.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2471.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2473.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2078 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2476.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      777 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2481.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2485.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      786 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2504.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1409 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2505.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      636 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2526.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2143 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2540.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2404 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2541.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1890 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2543.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      381 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2548.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1984 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2549.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2556.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2560.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      273 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2566.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4266 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2567.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2580.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      397 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2581.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1195 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2582.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2602.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      538 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2605.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3064 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2606.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2610.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2826 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2616.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      929 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2620.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2634.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      662 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2661.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1821 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2672.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2673.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2125 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2674.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4565 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2680.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3166 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2681.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1407 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2684.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2686.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1822 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2690.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1689 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2696.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      520 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2703.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2247 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2721.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      244 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2740.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2741.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2751.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2753.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1948 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2763.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5366 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2773.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1952 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2778.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2802.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1042 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2803.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2808.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      938 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2820.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2821.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      733 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2825.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      389 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2826.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      245 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2833.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1155 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2840.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2842.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2845.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4850 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2870.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2884.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3295 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2890.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2891.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2895.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2950.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4932 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2951.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8816 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2954.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    18089 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2963.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3433 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2965.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2847 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2966.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3311 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2968.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3166 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2970.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5415 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2972.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7271 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2978.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4945 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2984.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3190 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2987.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    10570 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2990.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1433 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2997.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2551 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3000.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      596 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3001.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3003.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3008.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3011.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      297 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3013.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3014.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3015.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      408 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3016.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3017.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3019.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3020.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3021.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3022.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3023.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3024.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3025.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3026.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      273 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3027.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      497 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3028.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3030.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3031.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3034.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      471 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3035.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3036.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3037.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      299 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3038.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      282 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3039.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3040.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3041.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      272 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3044.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3045.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3046.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3056.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3058.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      518 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3066.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2219 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3068.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      531 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3086.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3087.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3094.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3095.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3103.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3107.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      905 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3112.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3114.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      648 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3120.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3122.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3124.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3125.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3126.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3129.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1690 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3133.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1070 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3139.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      268 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3142.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      403 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3145.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3147.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3154.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      915 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3156.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3161.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3164.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3165.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3168.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      282 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3170.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      518 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3172.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3173.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      256 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3175.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      664 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3177.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3181.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      388 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3188.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1050 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3189.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      377 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3200.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3201.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1028 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3202.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3206.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3208.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1156 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3210.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3214.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      410 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3219.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3220.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3223.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3224.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      263 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3225.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3227.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3228.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      824 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3231.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3238.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      387 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3244.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      394 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3248.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3254.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      401 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3257.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3259.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3260.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      270 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3261.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      574 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3264.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3265.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3266.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3267.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3268.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3269.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3270.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3271.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3273.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3275.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3276.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3277.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3278.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3279.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3280.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3281.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3282.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      385 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3283.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3285.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3286.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3287.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3288.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3289.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3290.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      253 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3297.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      570 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3301.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3303.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3305.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      550 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3306.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1055 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3317.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3319.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3320.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3321.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3322.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      550 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3326.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3328.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3329.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3330.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3334.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3335.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3336.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3337.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3338.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3339.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3348.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3349.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3350.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      572 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3354.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3358.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3373.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1412 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3387.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      377 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3390.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1933 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3407.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      713 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3421.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      372 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3442.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1329 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3455.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      548 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3469.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3474.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3488.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2284 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3517.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3539.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      620 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3541.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3677 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3553.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1022 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3572.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      400 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3579.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1113 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3590.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      774 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3598.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2776 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3636.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      243 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3647.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      916 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3652.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      916 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3653.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      792 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3664.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1279 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3665.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      912 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3682.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2000 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3702.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      616 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3704.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      245 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3710.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3717.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4053 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3721.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1690 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3731.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1308 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3751.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      528 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3762.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      816 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3764.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3771.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3773.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      539 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3784.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3795.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      673 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3798.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      625 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3805.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2132 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3810.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2225 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3825.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3855.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1298 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3878.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      908 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3913.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3917.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3929.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      811 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3931.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2299 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3932.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3938.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1177 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3943.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3960.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      564 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3962.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3971.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1026 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3973.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      770 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3980.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3986.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3987.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1205 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3989.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      629 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4000.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1161 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4013.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4022.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1287 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4027.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4036.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8853 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4047.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4265 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4064.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1202 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4069.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2445 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4076.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2481 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4091.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      772 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4104.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1365 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4125.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1032 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4130.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      943 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4132.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1297 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4148.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5099 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4160.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2104 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4175.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1015 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4189.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5886 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4196.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      900 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4197.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1259 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4220.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1844 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4230.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1098 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4238.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3554 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4263.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4294.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4295.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      370 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4296.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1127 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4301.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      640 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4310.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      503 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4322.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      244 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4324.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2063 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4344.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1179 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4357.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      924 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4363.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4371.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      744 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4378.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4387.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      643 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4394.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1441 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4397.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1029 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4413.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      886 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4422.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      705 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4425.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1866 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4445.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      844 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4456.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      870 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4463.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1199 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4478.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1126 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4490.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1038 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4497.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1236 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4507.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      652 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4518.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1547 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4523.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      976 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4533.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4540.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1791 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4544.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1937 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4563.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      749 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4567.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      635 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4593.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      914 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4594.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      995 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4608.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      375 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4613.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      708 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4626.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      378 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4628.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1031 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4632.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1151 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4652.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1188 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4664.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1324 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4665.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2207 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4677.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6106 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4682.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      482 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4688.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4691.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1257 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4693.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      641 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4714.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4726.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      742 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4730.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5281 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4735.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1949 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4780.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      506 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4792.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      953 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4802.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1412 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4808.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4820.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4821.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4823.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1457 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4828.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      729 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4847.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1453 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4848.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1314 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4859.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1200 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4864.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      586 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4874.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2144 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4876.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1138 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4893.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      644 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4902.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1661 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4909.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1285 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4916.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1853 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4929.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      990 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4949.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1997 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4954.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      515 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4955.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1730 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4959.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4962.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2052 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4965.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2462 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4975.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      766 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4992.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4993.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      388 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4996.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1283 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5000.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5002.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5011.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2504 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5016.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1041 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5030.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      638 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5037.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      919 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5039.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      926 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5050.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      601 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5055.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1222 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5060.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1934 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5070.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1228 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5072.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1438 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5077.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1453 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5087.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1705 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5094.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5095.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1974 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5097.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1934 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5100.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      311 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5111.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6809 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5114.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5009 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5123.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1047 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5128.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5130.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5564 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5131.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2793 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5137.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1143 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5139.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1094 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5140.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3817 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5147.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1793 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5152.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      796 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5153.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2039 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5159.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      908 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5162.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      652 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5169.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      819 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5199.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1318 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5207.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1140 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5209.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      818 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5222.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      902 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5234.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      674 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5243.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      505 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5260.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1807 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5272.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5284.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      264 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5287.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      941 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5311.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5330.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1715 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5335.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1193 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5348.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1427 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5372.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2152 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5384.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2191 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5405.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5437.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      506 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5441.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5447.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2932 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5448.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5449.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5462.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      903 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5466.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      760 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5470.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2780 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5477.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      892 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5483.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      635 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5485.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5491.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      380 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5493.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3793 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5499.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5524.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      393 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5541.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5542.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      253 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5550.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      896 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5554.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5568.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1726 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5577.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      529 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5585.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3911 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5600.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1186 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5631.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3095 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5666.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5685.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      435 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5690.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5693.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      777 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5706.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      781 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5707.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1316 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5714.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5719.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      708 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5720.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3400 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5768.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      628 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5797.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5815.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      640 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5823.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      864 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5832.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5847.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1413 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5864.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      633 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5877.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      758 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5883.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      536 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5884.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      631 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5885.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      544 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5888.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      781 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5895.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5897.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1177 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5898.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5905.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5906.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1343 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5911.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1159 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5916.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      764 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5920.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1202 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5921.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      401 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5927.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      623 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5932.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5935.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1146 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5943.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1375 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5962.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5980.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      658 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5982.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      661 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5997.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6010.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      768 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6012.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      894 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6024.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1378 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6025.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      790 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6062.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      382 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6076.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      381 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6084.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1310 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6094.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      877 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6113.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6117.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6121.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6122.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5868 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6129.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4046 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6175.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1399 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6198.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6019 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6242.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3620 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6265.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2423 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6287.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3914 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6313.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1566 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6328.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      910 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6333.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1351 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6338.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1137 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6342.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14009 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6345.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2034 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6351.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2417 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6355.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1516 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6357.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6363.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2360 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6373.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3465 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6377.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1171 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6382.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      822 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6386.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1694 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6387.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3686 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6391.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7804 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6403.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      256 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6423.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6426.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3891 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6430.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      659 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6436.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      402 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6443.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2700 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6451.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1285 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6456.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2672 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6466.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1995 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6470.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3515 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6483.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      880 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6503.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1629 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6514.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6441 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6531.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4296 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6552.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2620 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6560.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3027 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6572.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4326 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6582.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6591.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1008 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6606.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1898 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6612.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1153 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6615.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2282 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6618.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6766 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6649.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3978 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6665.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1428 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6673.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2400 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6677.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      545 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6678.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1239 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6690.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      933 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6697.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3004 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6731.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      992 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6741.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1498 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6758.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      551 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6762.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      496 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6770.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7182 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6785.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      393 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6789.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6805.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      746 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6810.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      515 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6823.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1459 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6832.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1362 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6836.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6838.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      870 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6841.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      645 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6853.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1166 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6860.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1037 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6863.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5520 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6874.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1160 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6883.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      859 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6885.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1138 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6888.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6889.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2342 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6897.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6900.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6909.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      381 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6911.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2055 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6912.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1232 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6919.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1125 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6924.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6931.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      251 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6932.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6933.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      262 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6935.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2130 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6941.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1940 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6956.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2421 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6961.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3994 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6990.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1796 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6996.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      593 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7025.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7029.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      608 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7032.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1960 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7041.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1584 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7087.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3132 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7092.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2974 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7111.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3950 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7139.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1724 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7156.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3576 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7164.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      805 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7184.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      255 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7191.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3618 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7193.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1321 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7200.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8359 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7213.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      847 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7239.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2013 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7240.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1666 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7249.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2041 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7264.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7274.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     8151 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7288.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7316.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      492 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7326.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2841 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7338.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      890 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7353.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      949 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7362.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      925 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7363.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1114 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7373.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9622 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7387.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2219 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7532.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      684 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7541.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      876 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7543.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1442 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7550.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1004 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7559.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1666 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7565.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2212 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7576.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      761 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7591.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3583 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7601.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2187 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7625.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4369 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7641.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13243 2023-02-11 08:04:30.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7708.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5045 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7755.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7768.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4344 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7794.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1786 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7825.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12534 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7837.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1638 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7847.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1010 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7859.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1975 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7868.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1149 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7889.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4162 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7909.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1845 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7913.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1019 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7916.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1782 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7938.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1268 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7981.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    13089 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7994.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      392 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8011.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8019.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1680 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8027.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2082 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8029.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7662 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8047.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1480 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8069.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1384 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8076.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      625 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8096.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      992 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8102.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      989 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8103.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1158 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8118.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    16034 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8134.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      998 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8143.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1433 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8153.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1664 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8166.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8181.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      768 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8197.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      884 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8200.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1027 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8223.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1161 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8231.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      852 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8234.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      522 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8242.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8252.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      266 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8257.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8261.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8263.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      620 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8268.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      258 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8288.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      253 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8296.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8300.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8301.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8305.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      247 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8312.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      989 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8323.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    12629 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8332.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      992 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8389.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1139 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8395.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1649 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8397.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2028 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8398.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2673 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8400.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      243 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8401.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4898 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8425.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1521 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8457.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1303 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8463.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      637 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8477.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1079 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8482.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8500.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8511.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1767 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8512.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      888 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8514.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      896 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8524.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      261 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8528.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8536.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      772 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8544.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1738 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8551.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8559.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      360 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8575.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     7501 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8582.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1298 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8589.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      276 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8592.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      386 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8593.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1926 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8610.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1027 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8621.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1607 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8626.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1406 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8632.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4186 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8633.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1240 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8635.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     4148 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8636.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1149 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8645.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      516 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8653.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      653 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8656.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      752 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8660.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8664.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      516 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8667.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1559 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8668.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      934 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8680.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1459 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8689.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8692.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      765 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8694.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1378 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8701.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1232 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8715.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1463 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8730.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8740.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     6758 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8762.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1363 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8766.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1045 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8771.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1839 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8794.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2148 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8813.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2308 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8829.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1782 2023-04-03 23:15:38.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8857.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1286 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8893.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      363 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8905.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      541 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8906.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2632 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8916.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1979 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8926.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8934.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      881 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8941.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1513 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8949.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      862 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8964.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      857 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8982.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1173 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9010.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1318 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9017.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      647 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9043.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      652 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9048.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      510 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9069.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      873 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9070.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9072.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      406 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9103.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     5122 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9104.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      260 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9137.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9140.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9145.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1546 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9169.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9177.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1871 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9178.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9181.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2091 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9184.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      744 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9193.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      505 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9197.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      392 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9200.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      248 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9203.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      531 2023-03-09 01:22:11.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9205.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1317 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9208.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1798 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9213.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      651 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9221.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2532 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9229.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1617 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9234.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      404 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9240.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      953 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9251.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      784 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9257.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1332 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9270.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1981 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9296.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1250 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9302.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1860 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9319.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      899 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9332.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      254 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9338.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1562 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9341.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9347.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      654 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9353.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1537 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9363.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     9515 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9375.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      887 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9450.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9451.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1150 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9452.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      649 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9453.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9456.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      374 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9457.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     3508 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9461.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9462.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9463.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9466.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      365 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9467.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9468.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9470.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9471.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      387 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9472.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      505 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9473.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      367 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9475.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1264 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9477.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      504 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9479.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9480.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      882 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9481.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      914 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9483.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1164 2023-05-01 06:27:53.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9484.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      133 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9485.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      649 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9486.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      265 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9487.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      398 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9488.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     1758 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9489.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      533 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9490.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9491.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9493.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      526 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9494.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9495.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)      131 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9496.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    14024 2023-01-15 23:57:15.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9900.json
+-rw-r--r--   0 sho-kusano   (501) staff       (20)       32 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/md5
+-rw-r--r--   0 sho-kusano   (501) staff       (20)        8 2023-06-07 08:05:06.000000 zengin_code-1.1.0.20230607/zengin_code/source-data/data/updated_at
+drwxr-xr-x   0 sho-kusano   (501) staff       (20)        0 2023-06-07 08:05:50.856001 zengin_code-1.1.0.20230607/zengin_code.egg-info/
+-rw-r--r--   0 sho-kusano   (501) staff       (20)     2040 2023-06-07 08:05:50.000000 zengin_code-1.1.0.20230607/zengin_code.egg-info/PKG-INFO
+-rw-r--r--   0 sho-kusano   (501) staff       (20)    66979 2023-06-07 08:05:50.000000 zengin_code-1.1.0.20230607/zengin_code.egg-info/SOURCES.txt
+-rw-r--r--   0 sho-kusano   (501) staff       (20)        1 2023-06-07 08:05:50.000000 zengin_code-1.1.0.20230607/zengin_code.egg-info/dependency_links.txt
+-rw-r--r--   0 sho-kusano   (501) staff       (20)        4 2023-06-07 08:05:50.000000 zengin_code-1.1.0.20230607/zengin_code.egg-info/requires.txt
+-rw-r--r--   0 sho-kusano   (501) staff       (20)       12 2023-06-07 08:05:50.000000 zengin_code-1.1.0.20230607/zengin_code.egg-info/top_level.txt
```

### Comparing `zengin_code-1.1.0.20230501/LICENSE.txt` & `zengin_code-1.1.0.20230607/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/PKG-INFO` & `zengin_code-1.1.0.20230607/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zengin_code
-Version: 1.1.0.20230501
+Version: 1.1.0.20230607
 Summary: bank codes and branch codes for Japanese.
 Home-page: https://github.com/zengin-code/zengin-py
 Author: Zengin Code
 Author-email: zengin-code@zeny.io
 License: MIT
 Keywords: zengin,bank,japanese
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zengin_code-1.1.0.20230501/README.rst` & `zengin_code-1.1.0.20230607/README.rst`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/setup.py` & `zengin_code-1.1.0.20230607/setup.py`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/tests/test_bank.py` & `zengin_code-1.1.0.20230607/tests/test_bank.py`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/__init__.py` & `zengin_code-1.1.0.20230607/zengin_code/__init__.py`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/bank.py` & `zengin_code-1.1.0.20230607/zengin_code/bank.py`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/banks.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/banks.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0001.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0001.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0005.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0005.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0009.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0009.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0010.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0010.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0017.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0017.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0033.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0033.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9934426229508195%*

 * *Differences: {"'817'": "{'name': 'スペード', 'kana': 'スペ－ド', 'hira': 'すぺ－ど', 'roma': 'supe-do'}",*

 * * "'818'": "{'name': 'ハート', 'kana': 'ハ－ト', 'hira': 'は－と', 'roma': 'ha-to'}"}*

```diff
@@ -256,25 +256,25 @@
         "hira": "\u3042\u3093\u3069\u308d\u3081\u3060\u3056",
         "kana": "\u30a2\u30f3\u30c9\u30ed\u30e1\u30c0\u30b6",
         "name": "\u30a2\u30f3\u30c9\u30ed\u30e1\u30c0\u5ea7",
         "roma": "andoromedaza"
     },
     "817": {
         "code": "817",
-        "hira": "\u307b\u3046\u304a\u3046\u3056",
-        "kana": "\u30db\u30a6\u30aa\u30a6\u30b6",
-        "name": "\u307b\u3046\u304a\u3046\u5ea7",
-        "roma": "hououza"
+        "hira": "\u3059\u307a\uff0d\u3069",
+        "kana": "\u30b9\u30da\uff0d\u30c9",
+        "name": "\u30b9\u30da\u30fc\u30c9",
+        "roma": "supe-do"
     },
     "818": {
         "code": "818",
-        "hira": "\u3053\u3050\u307e\u3056",
-        "kana": "\u30b3\u30b0\u30de\u30b6",
-        "name": "\u3053\u3050\u307e\u5ea7",
-        "roma": "kogumaza"
+        "hira": "\u306f\uff0d\u3068",
+        "kana": "\u30cf\uff0d\u30c8",
+        "name": "\u30cf\u30fc\u30c8",
+        "roma": "ha-to"
     },
     "819": {
         "code": "819",
         "hira": "\u3042\u3044\u3059\u304f\u308a\uff0d\u3080",
         "kana": "\u30a2\u30a4\u30b9\u30af\u30ea\uff0d\u30e0",
         "name": "\u30a2\u30a4\u30b9\u30af\u30ea\u30fc\u30e0",
         "roma": "aisukuri-mu"
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0034.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0034.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0036.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0036.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0038.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0038.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0039.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0039.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0040.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0040.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0041.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0041.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0042.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0042.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0043.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0043.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0116.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0116.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0117.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0117.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0118.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0118.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0119.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0119.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0120.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0120.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0121.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0121.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0122.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0122.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0123.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0123.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0124.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0124.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0125.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0125.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0126.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0126.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0128.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0128.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0129.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0129.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0130.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0130.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0131.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0131.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0133.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0133.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0134.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0134.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0135.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0135.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0137.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0137.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0138.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0138.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9992610837438424%*

 * *Differences: {"'331'": "{'name': '保土ケ谷'}", "'332'": "{'name': '希望ケ丘'}", "'333'": "{'name': '鶴ケ峯'}"}*

```diff
@@ -160,29 +160,29 @@
         "name": "\u3044\u305a\u307f\u91ce",
         "roma": "izumino"
     },
     "331": {
         "code": "331",
         "hira": "\u307b\u3069\u304c\u3084",
         "kana": "\u30db\u30c9\u30ac\u30e4",
-        "name": "\u4fdd\u571f\u30f6\u8c37",
+        "name": "\u4fdd\u571f\u30b1\u8c37",
         "roma": "hodogaya"
     },
     "332": {
         "code": "332",
         "hira": "\u304d\u307c\u3046\u304c\u304a\u304b",
         "kana": "\u30ad\u30dc\u30a6\u30ac\u30aa\u30ab",
-        "name": "\u5e0c\u671b\u30f6\u4e18",
+        "name": "\u5e0c\u671b\u30b1\u4e18",
         "roma": "kibougaoka"
     },
     "333": {
         "code": "333",
         "hira": "\u3064\u308b\u304c\u307f\u306d",
         "kana": "\u30c4\u30eb\u30ac\u30df\u30cd",
-        "name": "\u9db4\u30f6\u5cef",
+        "name": "\u9db4\u30b1\u5cef",
         "roma": "tsurugamine"
     },
     "334": {
         "code": "334",
         "hira": "\u308f\u3060\u307e\u3061",
         "kana": "\u30ef\u30c0\u30de\u30c1",
         "name": "\u548c\u7530\u753a",
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0140.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0140.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0141.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0141.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0142.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0142.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0143.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0143.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0144.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0144.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0145.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0145.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0146.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0146.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998095238095238%*

 * *Differences: {"'503'": "{'name': '福井北部', 'kana': 'フクイホクブ', 'hira': 'ふくいほくぶ', 'roma': 'fukuihokubu'}"}*

```diff
@@ -690,18 +690,18 @@
         "hira": "\u3075\u304f\u3044",
         "kana": "\u30d5\u30af\u30a4",
         "name": "\u798f\u4e95",
         "roma": "fukui"
     },
     "503": {
         "code": "503",
-        "hira": "\u304b\u306a\u3065",
-        "kana": "\u30ab\u30ca\u30c5",
-        "name": "\u91d1\u6d25",
-        "roma": "kanadu"
+        "hira": "\u3075\u304f\u3044\u307b\u304f\u3076",
+        "kana": "\u30d5\u30af\u30a4\u30db\u30af\u30d6",
+        "name": "\u798f\u4e95\u5317\u90e8",
+        "roma": "fukuihokubu"
     },
     "504": {
         "code": "504",
         "hira": "\u305f\u3093\u306a\u3093",
         "kana": "\u30bf\u30f3\u30ca\u30f3",
         "name": "\u4e39\u5357",
         "roma": "tannan"
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0147.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0147.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0149.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0149.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0150.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0150.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {'delete': "['702']"}*

```diff
@@ -548,21 +548,14 @@
     "700": {
         "code": "700",
         "hira": "\u3057\u307f\u305a",
         "kana": "\u30b7\u30df\u30ba",
         "name": "\u6e05\u6c34",
         "roma": "shimizu"
     },
-    "702": {
-        "code": "702",
-        "hira": "\u3057\u307f\u305a\u3048\u304d",
-        "kana": "\u30b7\u30df\u30ba\u30a8\u30ad",
-        "name": "\u6e05\u6c34\u99c5",
-        "roma": "shimizueki"
-    },
     "704": {
         "code": "704",
         "hira": "\u3057\u307f\u305a\u307f\u307b",
         "kana": "\u30b7\u30df\u30ba\u30df\u30db",
         "name": "\u6e05\u6c34\u4e09\u4fdd",
         "roma": "shimizumiho"
     },
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0151.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0151.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0152.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0152.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0153.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0153.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0154.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0154.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0155.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0155.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0157.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0157.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0158.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0158.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0159.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0159.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0161.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0161.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0162.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0162.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0163.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0163.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0164.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0164.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0166.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0166.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0167.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0167.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0168.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0168.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0169.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0169.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0170.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0170.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0172.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0172.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0173.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0173.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0174.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0174.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0175.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0175.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0177.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0177.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0178.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0178.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0179.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0179.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0180.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0180.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0181.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0181.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0182.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0182.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0183.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0183.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0184.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0184.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0185.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0185.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0187.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0187.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0188.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0188.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0190.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0190.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0191.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0191.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0288.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0288.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0289.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0289.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0294.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0294.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0300.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0300.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0304.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0304.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981981981981982%*

 * *Differences: {"'233'": "{'name': '新宿２３３', 'kana': 'シンジユクニサンサン', 'hira': 'しんじゆくにさんさん', 'roma': "*

 * *          "'shinjiyukunisansan'}",*

 * * "'240'": "{'name': '町田２４０', 'kana': 'マチダニヨンゼロ', 'hira': 'まちだによんぜろ', 'roma': 'machidaniyonzero'}"}*

```diff
@@ -725,18 +725,18 @@
         "hira": "\u306a\u306f",
         "kana": "\u30ca\u30cf",
         "name": "\u90a3\u8987",
         "roma": "naha"
     },
     "233": {
         "code": "233",
-        "hira": "\u305b\u3044\u3058\u3088\u3046",
-        "kana": "\u30bb\u30a4\u30b8\u30e8\u30a6",
-        "name": "\u6210\u57ce",
-        "roma": "seijiyou"
+        "hira": "\u3057\u3093\u3058\u3086\u304f\u306b\u3055\u3093\u3055\u3093",
+        "kana": "\u30b7\u30f3\u30b8\u30e6\u30af\u30cb\u30b5\u30f3\u30b5\u30f3",
+        "name": "\u65b0\u5bbf\uff12\uff13\uff13",
+        "roma": "shinjiyukunisansan"
     },
     "236": {
         "code": "236",
         "hira": "\u3046\u3081\u3060\u306b\u3055\u3093\u308d\u304f",
         "kana": "\u30a6\u30e1\u30c0\u30cb\u30b5\u30f3\u30ed\u30af",
         "name": "\u6885\u7530\uff12\uff13\uff16",
         "roma": "umedanisanroku"
@@ -753,18 +753,18 @@
         "hira": "\u3064\u304f\u3070",
         "kana": "\u30c4\u30af\u30d0",
         "name": "\u3064\u304f\u3070",
         "roma": "tsukuba"
     },
     "240": {
         "code": "240",
-        "hira": "\u3057\u3093\u3086\u308a\u304c\u304a\u304b",
-        "kana": "\u30b7\u30f3\u30e6\u30ea\u30ac\u30aa\u30ab",
-        "name": "\u65b0\u767e\u5408\u30b1\u4e18",
-        "roma": "shinyurigaoka"
+        "hira": "\u307e\u3061\u3060\u306b\u3088\u3093\u305c\u308d",
+        "kana": "\u30de\u30c1\u30c0\u30cb\u30e8\u30f3\u30bc\u30ed",
+        "name": "\u753a\u7530\uff12\uff14\uff10",
+        "roma": "machidaniyonzero"
     },
     "241": {
         "code": "241",
         "hira": "\u3068\u3064\u304b",
         "kana": "\u30c8\u30c4\u30ab",
         "name": "\u6238\u585a",
         "roma": "totsuka"
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0310.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0310.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0322.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0322.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0397.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0397.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0398.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0398.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0411.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0411.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0432.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0432.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0472.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0472.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0489.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0489.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0501.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0501.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0508.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0508.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0509.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0509.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0512.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0512.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0513.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0513.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0514.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0514.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0516.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0516.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0517.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0517.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0522.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0522.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0525.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0525.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0526.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0526.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0530.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0530.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0532.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0532.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0533.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0533.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0534.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0534.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0537.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0537.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0538.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0538.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0542.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0542.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0543.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0543.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0544.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0544.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931034482758619%*

 * *Differences: {"'601'": "{'name': '桑名中央', 'kana': 'クワナチユウオウ', 'hira': 'くわなちゆうおう', 'roma': 'kuwanachiyuuou'}",*

 * * "'603'": "{'name': '四日市中央', 'kana': 'ヨツカイチチユウオウ', 'hira': 'よつかいちちゆうおう', 'roma': "*

 * *          "'yotsukaichichiyuuou'}",*

 * * "'604'": "{'name': '富田中央', 'kana': 'トミダチユウオウ', 'hira': 'とみだちゆうおう', 'roma': 'tomidachiyuuou'}"}*

```diff
@@ -473,39 +473,39 @@
         "hira": "\u3057\u305a\u304a\u304b",
         "kana": "\u30b7\u30ba\u30aa\u30ab",
         "name": "\u9759\u5ca1",
         "roma": "shizuoka"
     },
     "601": {
         "code": "601",
-        "hira": "\u304f\u308f\u306a",
-        "kana": "\u30af\u30ef\u30ca",
-        "name": "\u6851\u540d",
-        "roma": "kuwana"
+        "hira": "\u304f\u308f\u306a\u3061\u3086\u3046\u304a\u3046",
+        "kana": "\u30af\u30ef\u30ca\u30c1\u30e6\u30a6\u30aa\u30a6",
+        "name": "\u6851\u540d\u4e2d\u592e",
+        "roma": "kuwanachiyuuou"
     },
     "602": {
         "code": "602",
         "hira": "\u3042\u3052\u304d",
         "kana": "\u30a2\u30b2\u30ad",
         "name": "\u963f\u4e0b\u559c",
         "roma": "ageki"
     },
     "603": {
         "code": "603",
-        "hira": "\u3088\u3064\u304b\u3044\u3061",
-        "kana": "\u30e8\u30c4\u30ab\u30a4\u30c1",
-        "name": "\u56db\u65e5\u5e02",
-        "roma": "yotsukaichi"
+        "hira": "\u3088\u3064\u304b\u3044\u3061\u3061\u3086\u3046\u304a\u3046",
+        "kana": "\u30e8\u30c4\u30ab\u30a4\u30c1\u30c1\u30e6\u30a6\u30aa\u30a6",
+        "name": "\u56db\u65e5\u5e02\u4e2d\u592e",
+        "roma": "yotsukaichichiyuuou"
     },
     "604": {
         "code": "604",
-        "hira": "\u3068\u307f\u3060",
-        "kana": "\u30c8\u30df\u30c0",
-        "name": "\u5bcc\u7530",
-        "roma": "tomida"
+        "hira": "\u3068\u307f\u3060\u3061\u3086\u3046\u304a\u3046",
+        "kana": "\u30c8\u30df\u30c0\u30c1\u30e6\u30a6\u30aa\u30a6",
+        "name": "\u5bcc\u7530\u4e2d\u592e",
+        "roma": "tomidachiyuuou"
     },
     "605": {
         "code": "605",
         "hira": "\u3064",
         "kana": "\u30c4",
         "name": "\u6d25",
         "roma": "tsu"
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0546.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0546.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0554.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0554.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0555.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0555.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0562.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0562.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0565.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0565.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0566.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0566.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0569.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0569.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0570.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0570.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0572.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0572.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0573.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0573.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0576.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0576.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0578.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0578.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0582.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0582.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0583.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0583.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0585.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0585.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0587.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0587.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0590.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0590.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0591.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0591.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0594.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0594.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0596.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0596.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/0597.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/0597.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1000.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1000.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1001.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1001.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1003.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1003.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1004.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1004.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1006.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1006.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1008.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1008.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1009.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1009.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1010.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1010.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1011.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1011.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1012.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1012.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1013.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1013.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1014.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1014.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1016.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1016.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1018.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1018.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1020.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1020.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1021.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1021.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1022.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1022.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1024.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1024.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1026.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1026.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1027.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1027.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1028.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1028.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1030.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1030.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1031.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1031.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1033.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1033.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1104.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1104.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1105.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1105.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1120.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1120.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1123.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1123.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1140.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1140.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1141.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1141.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1142.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1142.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1143.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1143.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1150.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1150.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1152.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1152.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1153.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1153.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1154.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1154.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1155.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1155.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1156.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1156.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1170.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1170.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1171.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1171.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1172.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1172.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1174.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1174.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1175.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1175.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1181.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1181.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1182.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1182.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1184.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1184.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1185.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1185.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1186.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1186.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1188.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1188.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1189.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1189.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1190.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1190.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1203.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1203.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1204.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1204.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1206.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1206.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1208.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1208.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1209.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1209.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1210.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1210.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1211.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1211.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1221.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1221.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1222.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1222.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1223.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1223.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1224.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1224.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1225.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1225.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1227.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1227.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1240.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1240.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1242.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1242.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1250.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1250.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1251.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1251.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1252.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1252.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1253.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1253.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1260.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1260.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1261.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1261.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1262.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1262.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1264.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1264.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1267.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1267.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1280.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1280.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1281.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1281.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1282.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1282.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1283.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1283.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1286.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1286.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1288.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1288.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1289.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1289.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1290.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1290.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1303.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1303.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1305.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1305.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1310.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1310.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1311.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1311.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1319.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1319.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1320.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1320.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1321.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1321.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1323.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1323.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1326.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1326.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1327.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1327.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1333.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1333.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1336.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1336.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1341.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1341.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1344.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1344.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1345.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1345.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1346.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1346.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1348.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1348.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1349.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1349.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1351.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1351.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1352.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1352.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1356.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1356.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1358.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1358.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1360.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1360.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1370.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1370.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1371.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1371.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1373.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1373.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1374.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1374.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1375.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1375.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1376.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1376.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1377.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1377.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1379.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1379.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1380.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1380.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1385.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1385.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1386.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1386.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1390.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1390.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1391.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1391.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1392.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1392.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1393.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1393.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1394.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1394.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1396.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1396.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1401.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1401.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1402.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1402.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1404.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1404.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1405.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1405.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1406.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1406.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1412.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1412.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1413.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1413.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1440.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1440.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1442.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1442.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1444.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1444.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1445.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1445.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1448.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1448.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1470.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1470.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1471.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1471.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1472.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1472.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1473.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1473.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1475.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1475.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1501.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1501.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1502.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1502.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1503.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1503.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1505.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1505.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1506.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1506.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1507.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1507.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1509.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1509.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1511.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1511.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1512.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1512.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1513.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1513.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1515.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1515.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1517.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1517.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1530.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1530.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1531.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1531.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1532.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1532.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1533.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1533.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1534.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1534.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1538.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1538.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1540.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1540.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1550.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1550.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1551.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1551.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1552.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1552.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1553.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1553.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1554.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1554.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1555.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1555.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1556.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1556.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1557.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1557.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1559.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1559.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1560.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1560.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1561.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1561.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1562.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1562.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1563.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1563.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1565.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1565.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1566.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1566.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1580.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1580.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1581.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1581.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1582.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1582.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1583.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1583.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1585.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1585.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1602.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1602.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1603.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1603.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1604.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1604.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1610.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1610.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1611.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1611.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1620.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1620.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1630.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1630.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1633.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1633.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1635.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1635.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1636.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1636.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1643.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1643.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1645.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1645.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1656.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1656.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1666.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1666.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1667.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1667.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1668.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1668.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1671.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1671.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1674.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1674.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1680.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1680.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1685.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1685.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1686.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1686.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1687.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1687.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1688.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1688.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1689.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1689.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1691.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1691.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1692.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1692.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1694.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1694.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1695.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1695.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1696.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1696.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1701.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1701.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1702.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1702.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1703.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1703.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1710.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1710.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1711.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1711.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1712.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1712.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809523%*

 * *Differences: {'delete': "['117']"}*

```diff
@@ -121,21 +121,14 @@
     "116": {
         "code": "116",
         "hira": "\u304a\u3084\u307e",
         "kana": "\u30aa\u30e4\u30de",
         "name": "\u5c0f\u5c71",
         "roma": "oyama"
     },
-    "117": {
-        "code": "117",
-        "hira": "\u305f\u3044\u3057\u3084\u307f\u306a\u307f",
-        "kana": "\u30bf\u30a4\u30b7\u30e4\u30df\u30ca\u30df",
-        "name": "\u5927\u793e\u5357",
-        "roma": "taishiyaminami"
-    },
     "119": {
         "code": "119",
         "hira": "\u3072\u304c\u3057",
         "kana": "\u30d2\u30ac\u30b7",
         "name": "\u6771",
         "roma": "higashi"
     },
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1732.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1732.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1734.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1734.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1735.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1735.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1738.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1738.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1740.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1740.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1741.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1741.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1742.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1742.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1743.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1743.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1750.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1750.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1752.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1752.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1756.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1756.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1758.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1758.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1780.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1780.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1781.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1781.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1789.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1789.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1801.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1801.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1803.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1803.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1830.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1830.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1833.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1833.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1860.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1860.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795918367346939%*

 * *Differences: {'delete': "['043']"}*

```diff
@@ -149,21 +149,14 @@
     "042": {
         "code": "042",
         "hira": "\u307f\u3084\u306b\u3057",
         "kana": "\u30df\u30e4\u30cb\u30b7",
         "name": "\u5bae\u897f",
         "roma": "miyanishi"
     },
-    "043": {
-        "code": "043",
-        "hira": "\u3042\u305d\u3060",
-        "kana": "\u30a2\u30bd\u30c0",
-        "name": "\u671d\u751f\u7530",
-        "roma": "asoda"
-    },
     "044": {
         "code": "044",
         "hira": "\u304b\u308f\u3046\u3061",
         "kana": "\u30ab\u30ef\u30a6\u30c1",
         "name": "\u5ddd\u5185",
         "roma": "kawauchi"
     },
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1862.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1862.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1864.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1864.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1866.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1866.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1880.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1880.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1881.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1881.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1901.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1901.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1903.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1903.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1908.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1908.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1909.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1909.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1910.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1910.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1913.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1913.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1917.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2084.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5272727272727272%*

 * *Differences: {"'002'": "OrderedDict([('code', '002'), ('name', '小松'), ('kana', 'コマツ'), ('hira', 'こまつ'), "*

 * *          "('roma', 'komatsu')])",*

 * * "'003'": "{'name': '小国', 'kana': 'オグニ', 'hira': 'おぐに', 'roma': 'oguni'}",*

 * * "'004'": "{'name': '荒砥', 'kana': 'アラト', 'hira': 'あらと', 'roma': 'arato'}",*

 * * "'006'": "{'name': '寒河江', 'kana': 'サガエ', 'hira': 'さがえ', 'roma': 'sagae'}",*

 * * "'007'": "{'name': '左沢', 'kana': 'アテラザワ', 'hira': 'あてらざわ', 'roma': 'aterazawa'}",*

 * * "'008'": "{'name': '飯豊', 'kana': 'イイデ', 'hira': 'いいで', 'roma': 'iide'}",*

 * *  […]*

```diff
@@ -2,71 +2,57 @@
     "001": {
         "code": "001",
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
         "name": "\u672c\u5e97\u55b6\u696d\u90e8",
         "roma": "honten"
     },
+    "002": {
+        "code": "002",
+        "hira": "\u3053\u307e\u3064",
+        "kana": "\u30b3\u30de\u30c4",
+        "name": "\u5c0f\u677e",
+        "roma": "komatsu"
+    },
     "003": {
         "code": "003",
-        "hira": "\u305f\u3050\u3061",
-        "kana": "\u30bf\u30b0\u30c1",
-        "name": "\u7530\u53e3",
-        "roma": "taguchi"
+        "hira": "\u304a\u3050\u306b",
+        "kana": "\u30aa\u30b0\u30cb",
+        "name": "\u5c0f\u56fd",
+        "roma": "oguni"
     },
     "004": {
         "code": "004",
-        "hira": "\u304a\u304a\u304d",
-        "kana": "\u30aa\u30aa\u30ad",
-        "name": "\u5927\u6728",
-        "roma": "ooki"
-    },
-    "005": {
-        "code": "005",
-        "hira": "\u3058\u3088\u3046\u3058\u307e",
-        "kana": "\u30b8\u30e8\u30a6\u30b8\u30de",
-        "name": "\u57ce\u5cf6",
-        "roma": "jiyoujima"
+        "hira": "\u3042\u3089\u3068",
+        "kana": "\u30a2\u30e9\u30c8",
+        "name": "\u8352\u7825",
+        "roma": "arato"
     },
     "006": {
         "code": "006",
-        "hira": "\u3082\u308d\u3069\u307f",
-        "kana": "\u30e2\u30ed\u30c9\u30df",
-        "name": "\u8af8\u5bcc",
-        "roma": "morodomi"
+        "hira": "\u3055\u304c\u3048",
+        "kana": "\u30b5\u30ac\u30a8",
+        "name": "\u5bd2\u6cb3\u6c5f",
+        "roma": "sagae"
     },
     "007": {
         "code": "007",
-        "hira": "\u304d\u3080\u308d",
-        "kana": "\u30ad\u30e0\u30ed",
-        "name": "\u6728\u5ba4",
-        "roma": "kimuro"
+        "hira": "\u3042\u3066\u3089\u3056\u308f",
+        "kana": "\u30a2\u30c6\u30e9\u30b6\u30ef",
+        "name": "\u5de6\u6ca2",
+        "roma": "aterazawa"
     },
     "008": {
         "code": "008",
-        "hira": "\u304b\u308f\u3050\u3061",
-        "kana": "\u30ab\u30ef\u30b0\u30c1",
-        "name": "\u5ddd\u53e3",
-        "roma": "kawaguchi"
-    },
-    "009": {
-        "code": "009",
-        "hira": "\u307f\u3064\u307e\u305f",
-        "kana": "\u30df\u30c4\u30de\u30bf",
-        "name": "\u4e09\u53c8",
-        "roma": "mitsumata"
-    },
-    "010": {
-        "code": "010",
-        "hira": "\u307f\u3065\u307e",
-        "kana": "\u30df\u30c5\u30de",
-        "name": "\u30df\u30c5\u30de",
-        "roma": "miduma"
+        "hira": "\u3044\u3044\u3067",
+        "kana": "\u30a4\u30a4\u30c7",
+        "name": "\u98ef\u8c4a",
+        "roma": "iide"
     },
     "011": {
         "code": "011",
-        "hira": "\u3055\u3051\u307f",
-        "kana": "\u30b5\u30b1\u30df",
-        "name": "\u9152\u898b",
-        "roma": "sakemi"
+        "hira": "\u308a\u3088\u3046\u306a\u3093",
+        "kana": "\u30ea\u30e8\u30a6\u30ca\u30f3",
+        "name": "\u9675\u5357",
+        "roma": "riyounan"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1920.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1920.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1930.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1930.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1931.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1931.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1932.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1932.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1933.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1933.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1942.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1942.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1951.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1951.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1952.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1952.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1954.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1954.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1955.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1955.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1960.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1960.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1962.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1962.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1968.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1968.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1980.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1980.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1981.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1981.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1982.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1982.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1985.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1985.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1986.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1986.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1990.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1990.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1991.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1991.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1993.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1993.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/1996.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1996.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2004.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2004.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2010.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2010.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2011.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2011.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2013.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2013.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2014.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2014.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2017.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2017.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2019.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2019.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2024.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2024.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2025.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2025.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2030.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2030.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2060.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2060.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2061.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2061.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2062.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2062.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2063.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2063.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2075.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2075.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2083.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2083.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2084.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8660.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2318181818181818%*

 * *Differences: {"'001'": "{'name': '本店'}",*

 * * "'007'": "{'name': '中央', 'kana': 'チユウオウ', 'hira': 'ちゆうおう', 'roma': 'chiyuuou'}",*

 * * "'009'": "OrderedDict([('code', '009'), ('name', '南部'), ('kana', 'ナンブ'), ('hira', 'なんぶ'), "*

 * *          "('roma', 'nambu')])",*

 * * "'011'": "{'name': '北部', 'kana': 'ホクブ', 'hira': 'ほくぶ', 'roma': 'hokubu'}",*

 * * "'014'": "OrderedDict([('code', '014'), ('name', '東部'), ('kana', 'トウブ'), ('hira', 'とうぶ'), "*

 * *          "('roma', 'toubu')])",*

 * * "'017'": "OrderedDict([('code', '017'), ('name', '西部'), ('kana', 'セイブ'),  […]*

```diff
@@ -1,58 +1,44 @@
 {
     "001": {
         "code": "001",
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
-        "name": "\u672c\u5e97\u55b6\u696d\u90e8",
+        "name": "\u672c\u5e97",
         "roma": "honten"
     },
-    "002": {
-        "code": "002",
-        "hira": "\u3053\u307e\u3064",
-        "kana": "\u30b3\u30de\u30c4",
-        "name": "\u5c0f\u677e",
-        "roma": "komatsu"
-    },
-    "003": {
-        "code": "003",
-        "hira": "\u304a\u3050\u306b",
-        "kana": "\u30aa\u30b0\u30cb",
-        "name": "\u5c0f\u56fd",
-        "roma": "oguni"
-    },
-    "004": {
-        "code": "004",
-        "hira": "\u3042\u3089\u3068",
-        "kana": "\u30a2\u30e9\u30c8",
-        "name": "\u8352\u7825",
-        "roma": "arato"
-    },
-    "006": {
-        "code": "006",
-        "hira": "\u3055\u304c\u3048",
-        "kana": "\u30b5\u30ac\u30a8",
-        "name": "\u5bd2\u6cb3\u6c5f",
-        "roma": "sagae"
-    },
     "007": {
         "code": "007",
-        "hira": "\u3042\u3066\u3089\u3056\u308f",
-        "kana": "\u30a2\u30c6\u30e9\u30b6\u30ef",
-        "name": "\u5de6\u6ca2",
-        "roma": "aterazawa"
-    },
-    "008": {
-        "code": "008",
-        "hira": "\u3044\u3044\u3067",
-        "kana": "\u30a4\u30a4\u30c7",
-        "name": "\u98ef\u8c4a",
-        "roma": "iide"
+        "hira": "\u3061\u3086\u3046\u304a\u3046",
+        "kana": "\u30c1\u30e6\u30a6\u30aa\u30a6",
+        "name": "\u4e2d\u592e",
+        "roma": "chiyuuou"
+    },
+    "009": {
+        "code": "009",
+        "hira": "\u306a\u3093\u3076",
+        "kana": "\u30ca\u30f3\u30d6",
+        "name": "\u5357\u90e8",
+        "roma": "nambu"
     },
     "011": {
         "code": "011",
-        "hira": "\u308a\u3088\u3046\u306a\u3093",
-        "kana": "\u30ea\u30e8\u30a6\u30ca\u30f3",
-        "name": "\u9675\u5357",
-        "roma": "riyounan"
+        "hira": "\u307b\u304f\u3076",
+        "kana": "\u30db\u30af\u30d6",
+        "name": "\u5317\u90e8",
+        "roma": "hokubu"
+    },
+    "014": {
+        "code": "014",
+        "hira": "\u3068\u3046\u3076",
+        "kana": "\u30c8\u30a6\u30d6",
+        "name": "\u6771\u90e8",
+        "roma": "toubu"
+    },
+    "017": {
+        "code": "017",
+        "hira": "\u305b\u3044\u3076",
+        "kana": "\u30bb\u30a4\u30d6",
+        "name": "\u897f\u90e8",
+        "roma": "seibu"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2085.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2085.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2090.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2090.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2092.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2092.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2095.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2095.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2096.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2096.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2101.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2101.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2122.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2122.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2125.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2125.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2143.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2143.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2146.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2146.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2149.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2149.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2165.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2165.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2167.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2167.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2180.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2180.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2184.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2184.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2190.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2190.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2202.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2202.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2226.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2226.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2229.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2229.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2231.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2231.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2235.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2235.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2241.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2241.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2243.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2243.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2248.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2248.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2254.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2254.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2271.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2271.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2277.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2277.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2304.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2304.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2306.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2306.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2318.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2318.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2351.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2351.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2356.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2356.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2357.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2357.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2358.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2358.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2360.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2360.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2361.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2361.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2362.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2362.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2363.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2363.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2365.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2365.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2366.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2366.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2377.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2377.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2378.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2378.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2390.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2390.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2404.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2404.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2442.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2442.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2448.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2448.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2451.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2451.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2470.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2470.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2471.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2471.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2476.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2476.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2481.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2481.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2504.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2504.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2505.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2505.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2526.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2526.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2540.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2540.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2541.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2541.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2543.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2543.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2549.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2549.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2567.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2567.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2582.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2582.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2605.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2605.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2606.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2606.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2616.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2616.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2620.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2620.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2661.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2661.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2672.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2672.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2674.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2674.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2680.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2680.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2681.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2681.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2684.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2684.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2690.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2690.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2696.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2696.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2703.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2703.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2721.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2721.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2763.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2763.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2773.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2773.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2778.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2778.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2803.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2803.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2808.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2808.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2820.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2820.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2825.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2825.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2840.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2840.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2845.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2845.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2870.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2870.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2890.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2890.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2895.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2895.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2951.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2951.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2954.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2954.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2963.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2963.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2965.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2965.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2966.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2966.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2968.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2968.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2970.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2970.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2972.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2972.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2978.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2978.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2984.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2984.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2987.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2987.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2990.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2990.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/2997.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/2997.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3000.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3000.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3001.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3001.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3066.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3066.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3068.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3068.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3086.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3086.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3112.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3112.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3120.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3120.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3133.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3133.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3139.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3139.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3156.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3156.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3172.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3172.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3177.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3177.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3189.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3189.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3202.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3202.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3210.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3210.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3231.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3231.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3238.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3238.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3264.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3264.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3301.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3301.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3306.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3306.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3317.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3317.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3326.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3326.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3339.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3339.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3354.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3354.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3373.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3373.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3387.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3387.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3407.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3407.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3421.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3421.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3455.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3455.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3469.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3469.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3488.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3488.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3517.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3517.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3541.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3541.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3553.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3553.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3572.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3572.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3590.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6888.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.05%*

 * *Differences: {"'003'": "OrderedDict([('code', '003'), ('name', '赤野井'), ('kana', 'アカノイ'), ('hira', 'あかのい'), "*

 * *          "('roma', 'akanoi')])",*

 * * "'004'": "OrderedDict([('code', '004'), ('name', '明富'), ('kana', 'アケトミ'), ('hira', 'あけとみ'), "*

 * *          "('roma', 'aketomi')])",*

 * * "'006'": "OrderedDict([('code', '006'), ('name', '河西'), ('kana', 'カワニシ'), ('hira', 'かわにし'), "*

 * *          "('roma', 'kawanishi')])",*

 * * "'100'": "OrderedDict([('code', '100'), ('name', '守山'), ('kana', 'モリヤマ'), ('hira', 'もりやま'), "*

 * *          "('roma', 'mori […]*

```diff
@@ -2,85 +2,64 @@
     "001": {
         "code": "001",
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
         "name": "\u672c\u5e97",
         "roma": "honten"
     },
-    "002": {
-        "code": "002",
-        "hira": "\u305b\u3093\u307e\u3084",
-        "kana": "\u30bb\u30f3\u30de\u30e4",
-        "name": "\u5343\u53a9",
-        "roma": "semmaya"
-    },
-    "008": {
-        "code": "008",
-        "hira": "\u3075\u3058\u3055\u308f",
-        "kana": "\u30d5\u30b8\u30b5\u30ef",
-        "name": "\u85e4\u6ca2",
-        "roma": "fujisawa"
-    },
-    "016": {
-        "code": "016",
-        "hira": "\u3060\u3044\u3068\u3046",
-        "kana": "\u30c0\u30a4\u30c8\u30a6",
-        "name": "\u5927\u6771",
-        "roma": "daitou"
-    },
-    "021": {
-        "code": "021",
-        "hira": "\u3072\u304c\u3057\u3084\u307e",
-        "kana": "\u30d2\u30ac\u30b7\u30e4\u30de",
-        "name": "\u6771\u5c71",
-        "roma": "higashiyama"
-    },
-    "025": {
-        "code": "025",
-        "hira": "\u3080\u308d\u306d",
-        "kana": "\u30e0\u30ed\u30cd",
-        "name": "\u5ba4\u6839",
-        "roma": "murone"
-    },
-    "028": {
-        "code": "028",
-        "hira": "\u304b\u308f\u3055\u304d",
-        "kana": "\u30ab\u30ef\u30b5\u30ad",
-        "name": "\u5ddd\u5d0e\u51fa\u5f35\u6240",
-        "roma": "kawasaki"
-    },
-    "110": {
-        "code": "110",
-        "hira": "\u3052\u3093\u3073",
-        "kana": "\u30b2\u30f3\u30d3",
-        "name": "\u53b3\u7f8e\u51fa\u5f35\u6240",
-        "roma": "gembi"
-    },
-    "114": {
-        "code": "114",
-        "hira": "\u3044\u3061\u306e\u305b\u304d\u3061\u3086\u3046\u304a\u3046",
-        "kana": "\u30a4\u30c1\u30ce\u30bb\u30ad\u30c1\u30e6\u30a6\u30aa\u30a6",
-        "name": "\u4e00\u95a2\u4e2d\u592e",
-        "roma": "ichinosekichiyuuou"
-    },
-    "118": {
-        "code": "118",
-        "hira": "\u306f\u306a\u3044\u305a\u307f",
-        "kana": "\u30cf\u30ca\u30a4\u30ba\u30df",
-        "name": "\u82b1\u6cc9",
-        "roma": "hanaizumi"
-    },
-    "122": {
-        "code": "122",
-        "hira": "\u306a\u304c\u3044",
-        "kana": "\u30ca\u30ac\u30a4",
-        "name": "\u6c38\u4e95\u51fa\u5f35\u6240",
-        "roma": "nagai"
-    },
-    "124": {
-        "code": "124",
-        "hira": "\u3072\u3089\u3044\u305a\u307f",
-        "kana": "\u30d2\u30e9\u30a4\u30ba\u30df",
-        "name": "\u5e73\u6cc9",
-        "roma": "hiraizumi"
+    "003": {
+        "code": "003",
+        "hira": "\u3042\u304b\u306e\u3044",
+        "kana": "\u30a2\u30ab\u30ce\u30a4",
+        "name": "\u8d64\u91ce\u4e95",
+        "roma": "akanoi"
+    },
+    "004": {
+        "code": "004",
+        "hira": "\u3042\u3051\u3068\u307f",
+        "kana": "\u30a2\u30b1\u30c8\u30df",
+        "name": "\u660e\u5bcc",
+        "roma": "aketomi"
+    },
+    "006": {
+        "code": "006",
+        "hira": "\u304b\u308f\u306b\u3057",
+        "kana": "\u30ab\u30ef\u30cb\u30b7",
+        "name": "\u6cb3\u897f",
+        "roma": "kawanishi"
+    },
+    "100": {
+        "code": "100",
+        "hira": "\u3082\u308a\u3084\u307e",
+        "kana": "\u30e2\u30ea\u30e4\u30de",
+        "name": "\u5b88\u5c71",
+        "roma": "moriyama"
+    },
+    "120": {
+        "code": "120",
+        "hira": "\u3084\u3059",
+        "kana": "\u30e4\u30b9",
+        "name": "\u91ce\u6d32",
+        "roma": "yasu"
+    },
+    "121": {
+        "code": "121",
+        "hira": "\u304e\u304a\u3046",
+        "kana": "\u30ae\u30aa\u30a6",
+        "name": "\u7947\u738b",
+        "roma": "giou"
+    },
+    "123": {
+        "code": "123",
+        "hira": "\u307f\u304b\u307f",
+        "kana": "\u30df\u30ab\u30df",
+        "name": "\u4e09\u4e0a",
+        "roma": "mikami"
+    },
+    "130": {
+        "code": "130",
+        "hira": "\u3061\u3086\u3046\u305a",
+        "kana": "\u30c1\u30e6\u30a6\u30ba",
+        "name": "\u4e2d\u4e3b",
+        "roma": "chiyuuzu"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3598.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3598.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3636.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3636.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3652.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3652.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3653.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3653.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3664.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3664.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3665.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3665.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3682.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3682.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3702.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3702.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3704.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3704.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3721.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3721.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3731.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3731.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3751.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3751.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3762.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3762.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3764.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3764.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3784.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3784.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3798.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3798.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3805.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3805.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3810.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3810.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3825.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3825.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3855.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3855.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3878.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3878.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3913.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3913.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3931.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3931.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3932.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3932.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3943.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3943.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3960.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3960.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3962.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3962.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3973.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3973.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3980.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3980.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/3989.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3989.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4000.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4000.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4013.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4013.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4027.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4027.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4047.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4047.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4064.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4064.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4069.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4069.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4076.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4076.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4091.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4091.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4104.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4104.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4125.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4125.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4130.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4130.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4132.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4132.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4148.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4148.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4160.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4160.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4175.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4175.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4189.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4189.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4196.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4196.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4197.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4197.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4220.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4220.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4230.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4230.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4238.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4238.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4263.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4263.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4301.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4301.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4310.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4310.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4344.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4344.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4357.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4357.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4363.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4363.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4378.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4378.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4394.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4394.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4397.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4397.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4413.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4413.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4422.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4422.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4425.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4425.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4445.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4445.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4456.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4456.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4463.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4463.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4478.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4478.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4490.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4490.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4497.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4497.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4507.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4507.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4518.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4518.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4523.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4523.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4533.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4533.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4544.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4544.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4563.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4563.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4567.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4567.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4593.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4593.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4594.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4594.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4608.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4608.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4626.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4626.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4632.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4632.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4652.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4652.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4664.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4664.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4665.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4665.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4677.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4677.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4682.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4682.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4691.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4691.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4693.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4693.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4714.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4714.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4726.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4726.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4730.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4730.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4735.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4735.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4780.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4780.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4802.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4802.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4808.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4808.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4828.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4828.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4847.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4847.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4848.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4848.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4859.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4859.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4864.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4864.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4874.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4874.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4876.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4876.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4893.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4893.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4902.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4902.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4909.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4909.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4916.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4916.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4929.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4929.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4949.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4949.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4954.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4954.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4955.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4955.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4959.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4959.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4962.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4962.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4965.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4965.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4975.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4975.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/4992.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/4992.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5000.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5000.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5016.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5016.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5030.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5030.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5037.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5037.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5039.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5039.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5050.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5050.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5055.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5055.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5060.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5060.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5070.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5070.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5072.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5072.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5077.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5077.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5087.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5087.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5094.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5094.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5097.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5097.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5100.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5100.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5114.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5114.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5123.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5123.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5128.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5128.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5131.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5131.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5137.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5137.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5139.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5139.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5140.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5140.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5147.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5147.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5152.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5152.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5153.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5153.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5159.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5159.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5162.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5162.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5169.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5169.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5199.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5199.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5207.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5207.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5209.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5209.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5222.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5222.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5234.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5234.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5243.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5243.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5272.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5272.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5311.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5311.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5335.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5335.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5348.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5348.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5372.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5372.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5384.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5384.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5405.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5405.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5448.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5448.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5466.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5466.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5470.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5470.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5477.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5477.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5483.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5483.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5485.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5485.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5499.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5499.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5524.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5524.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5554.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5554.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5577.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5577.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5585.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5585.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5600.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5600.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5631.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5631.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5666.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5666.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5685.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5685.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5693.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5693.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5706.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5706.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5707.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9010.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.24615384615384617%*

 * *Differences: {"'001'": "{'name': '本所', 'kana': 'ホンシヨ', 'hira': 'ほんしよ', 'roma': 'honshiyo'}",*

 * * "'002'": "{'name': '松橋', 'kana': 'マツバセ', 'hira': 'まつばせ', 'roma': 'matsubase'}",*

 * * "'007'": "{'name': '下北', 'kana': 'シモキタ', 'hira': 'しもきた', 'roma': 'shimokita'}",*

 * * "'009'": "OrderedDict([('code', '009'), ('name', '富合'), ('kana', 'トミアイ'), ('hira', 'とみあい'), "*

 * *          "('roma', 'tomiai')])",*

 * * "'012'": "{'name': '小川町', 'kana': 'オガワマチ', 'hira': 'おがわまち', 'roma': 'ogawamachi'}",*

 * * "'017'": "OrderedDict([('code', '017'), ('name', '下東'), […]*

```diff
@@ -1,58 +1,65 @@
 {
     "001": {
         "code": "001",
-        "hira": "\u307b\u3093\u3066\u3093",
-        "kana": "\u30db\u30f3\u30c6\u30f3",
-        "name": "\u672c\u5e97",
-        "roma": "honten"
+        "hira": "\u307b\u3093\u3057\u3088",
+        "kana": "\u30db\u30f3\u30b7\u30e8",
+        "name": "\u672c\u6240",
+        "roma": "honshiyo"
     },
     "002": {
         "code": "002",
-        "hira": "\u3080\u3044\u304b\u307e\u3061",
-        "kana": "\u30e0\u30a4\u30ab\u30de\u30c1",
-        "name": "\u516d\u65e5\u753a",
-        "roma": "muikamachi"
-    },
-    "003": {
-        "code": "003",
-        "hira": "\u3044\u304b\u3056\u308f",
-        "kana": "\u30a4\u30ab\u30b6\u30ef",
-        "name": "\u4e94\u5341\u6ca2",
-        "roma": "ikazawa"
-    },
-    "004": {
-        "code": "004",
-        "hira": "\u3058\u3088\u3046\u306a\u3044",
-        "kana": "\u30b8\u30e8\u30a6\u30ca\u30a4",
-        "name": "\u57ce\u5185",
-        "roma": "jiyounai"
-    },
-    "005": {
-        "code": "005",
-        "hira": "\u304a\u304a\u307e\u304d",
-        "kana": "\u30aa\u30aa\u30de\u30ad",
-        "name": "\u5927\u5dfb",
-        "roma": "oomaki"
+        "hira": "\u307e\u3064\u3070\u305b",
+        "kana": "\u30de\u30c4\u30d0\u30bb",
+        "name": "\u677e\u6a4b",
+        "roma": "matsubase"
     },
     "007": {
         "code": "007",
-        "hira": "\u3046\u3089\u3055",
-        "kana": "\u30a6\u30e9\u30b5",
-        "name": "\u6d66\u4f50",
-        "roma": "urasa"
+        "hira": "\u3057\u3082\u304d\u305f",
+        "kana": "\u30b7\u30e2\u30ad\u30bf",
+        "name": "\u4e0b\u5317",
+        "roma": "shimokita"
+    },
+    "009": {
+        "code": "009",
+        "hira": "\u3068\u307f\u3042\u3044",
+        "kana": "\u30c8\u30df\u30a2\u30a4",
+        "name": "\u5bcc\u5408",
+        "roma": "tomiai"
     },
     "012": {
         "code": "012",
-        "hira": "\u3057\u304a\u3056\u308f",
-        "kana": "\u30b7\u30aa\u30b6\u30ef",
-        "name": "\u5869\u6ca2",
-        "roma": "shiozawa"
-    },
-    "015": {
-        "code": "015",
-        "hira": "\u3086\u3056\u308f",
-        "kana": "\u30e6\u30b6\u30ef",
-        "name": "\u6e6f\u6ca2",
-        "roma": "yuzawa"
+        "hira": "\u304a\u304c\u308f\u307e\u3061",
+        "kana": "\u30aa\u30ac\u30ef\u30de\u30c1",
+        "name": "\u5c0f\u5ddd\u753a",
+        "roma": "ogawamachi"
+    },
+    "017": {
+        "code": "017",
+        "hira": "\u3057\u3082\u3072\u304c\u3057",
+        "kana": "\u30b7\u30e2\u30d2\u30ac\u30b7",
+        "name": "\u4e0b\u6771",
+        "roma": "shimohigashi"
+    },
+    "023": {
+        "code": "023",
+        "hira": "\u3046\u3068",
+        "kana": "\u30a6\u30c8",
+        "name": "\u5b87\u571f",
+        "roma": "uto"
+    },
+    "030": {
+        "code": "030",
+        "hira": "\u307f\u3059\u307f",
+        "kana": "\u30df\u30b9\u30df",
+        "name": "\u4e09\u89d2",
+        "roma": "misumi"
+    },
+    "035": {
+        "code": "035",
+        "hira": "\u3057\u3089\u306c\u3072",
+        "kana": "\u30b7\u30e9\u30cc\u30d2",
+        "name": "\u4e0d\u77e5\u706b",
+        "roma": "shiranuhi"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5714.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5714.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5720.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5720.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5768.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5768.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5797.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5797.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5823.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5823.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5832.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5832.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5864.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5864.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5877.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5877.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5883.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5883.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5884.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5884.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5885.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5885.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5888.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5888.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5895.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5895.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5898.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5898.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5911.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5911.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5916.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5916.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5920.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5920.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5921.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5921.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5932.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5932.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5943.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5943.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5962.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5962.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5982.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5982.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/5997.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5997.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6012.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6012.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6024.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6024.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6025.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6025.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6062.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6062.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6094.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6094.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6113.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6113.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6129.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6129.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {'delete': "['004', '032', '076']"}*

```diff
@@ -9,21 +9,14 @@
     "003": {
         "code": "003",
         "hira": "\u3044\u308f\u306e\u3060",
         "kana": "\u30a4\u30ef\u30ce\u30c0",
         "name": "\u5ca9\u91ce\u7530",
         "roma": "iwanoda"
     },
-    "004": {
-        "code": "004",
-        "hira": "\u3068\u304d\u308f",
-        "kana": "\u30c8\u30ad\u30ef",
-        "name": "\u5e38\u78d0",
-        "roma": "tokiwa"
-    },
     "005": {
         "code": "005",
         "hira": "\u3055\u304e\u3084\u307e",
         "kana": "\u30b5\u30ae\u30e4\u30de",
         "name": "\u9dfa\u5c71",
         "roma": "sagiyama"
     },
@@ -100,21 +93,14 @@
     "031": {
         "code": "031",
         "hira": "\u304d\u305f\u306a\u304c\u3082\u308a",
         "kana": "\u30ad\u30bf\u30ca\u30ac\u30e2\u30ea",
         "name": "\u5317\u9577\u68ee",
         "roma": "kitanagamori"
     },
-    "032": {
-        "code": "032",
-        "hira": "\u306a\u304c\u3089\u306b\u3057",
-        "kana": "\u30ca\u30ac\u30e9\u30cb\u30b7",
-        "name": "\u9577\u826f\u897f",
-        "roma": "nagaranishi"
-    },
     "034": {
         "code": "034",
         "hira": "\u3057\u307e",
         "kana": "\u30b7\u30de",
         "name": "\u5cf6",
         "roma": "shima"
     },
@@ -303,21 +289,14 @@
     "075": {
         "code": "075",
         "hira": "\u305f\u304b\u3068\u307f",
         "kana": "\u30bf\u30ab\u30c8\u30df",
         "name": "\u9ad8\u5bcc",
         "roma": "takatomi"
     },
-    "076": {
-        "code": "076",
-        "hira": "\u304a\u304a\u3056\u304f\u3089",
-        "kana": "\u30aa\u30aa\u30b6\u30af\u30e9",
-        "name": "\u5927\u685c",
-        "roma": "oozakura"
-    },
     "077": {
         "code": "077",
         "hira": "\u3044\u3058\u3089",
         "kana": "\u30a4\u30b8\u30e9",
         "name": "\u4f0a\u81ea\u826f",
         "roma": "ijira"
     },
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6175.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6175.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6198.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6198.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6242.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6242.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6265.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6265.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6287.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6287.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6313.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6313.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6328.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6328.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6333.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6333.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6338.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6338.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6342.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6342.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6345.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6345.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6351.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6351.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6355.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6355.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6357.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6357.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6363.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6363.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6373.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6373.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6377.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6377.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6382.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6382.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6386.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6386.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6387.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6387.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6391.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6391.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6403.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6403.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6430.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6430.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6436.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6436.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'delete': "['064']"}*

```diff
@@ -29,16 +29,9 @@
     },
     "056": {
         "code": "056",
         "hira": "\u3072\u3089\u3070\u308a",
         "kana": "\u30d2\u30e9\u30d0\u30ea",
         "name": "\u5e73\u91dd",
         "roma": "hirabari"
-    },
-    "064": {
-        "code": "064",
-        "hira": "\u3046\u3048\u3060\u3048\u304d\u307e\u3048",
-        "kana": "\u30a6\u30a8\u30c0\u30a8\u30ad\u30de\u30a8",
-        "name": "\u690d\u7530\u99c5\u524d",
-        "roma": "uedaekimae"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6451.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6451.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6456.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6456.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6466.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6466.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6470.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6470.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6483.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6483.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6503.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6503.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6514.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6514.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6531.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6531.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6552.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6552.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6560.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6560.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6572.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6572.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6582.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6582.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6591.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6591.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6606.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6606.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6612.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6612.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6615.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6615.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6618.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6618.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6649.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6649.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6665.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6665.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6673.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6673.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6677.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6677.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6678.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6678.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6690.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6690.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6697.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6697.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6731.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6731.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6741.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6741.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6758.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6758.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6762.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6762.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6785.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6785.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6810.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6810.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6823.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6823.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6832.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6832.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6836.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6836.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6841.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6841.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6853.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6853.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6860.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6860.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6863.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6863.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6874.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6874.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6883.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6883.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6885.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6885.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6888.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8730.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2%*

 * *Differences: {"'001'": "{'name': '築城', 'kana': 'ツイキ', 'hira': 'ついき', 'roma': 'tsuiki'}",*

 * * "'004'": "{'name': '椎田', 'kana': 'シイダ', 'hira': 'しいだ', 'roma': 'shiida'}",*

 * * "'012'": "OrderedDict([('code', '012'), ('name', '豊前'), ('kana', 'ブゼン'), ('hira', 'ぶぜん'), "*

 * *          "('roma', 'buzen')])",*

 * * "'021'": "OrderedDict([('code', '021'), ('name', '築東'), ('kana', 'チクトウ'), ('hira', 'ちくとう'), "*

 * *          "('roma', 'chikutou')])",*

 * * "'100'": "{'name': '本店', 'kana': 'ホンテン', 'hira': 'ほんてん', 'roma': 'honten'}",*

 * * "'105'": "OrderedDict([( […]*

```diff
@@ -1,65 +1,79 @@
 {
     "001": {
         "code": "001",
-        "hira": "\u307b\u3093\u3066\u3093",
-        "kana": "\u30db\u30f3\u30c6\u30f3",
-        "name": "\u672c\u5e97",
-        "roma": "honten"
-    },
-    "003": {
-        "code": "003",
-        "hira": "\u3042\u304b\u306e\u3044",
-        "kana": "\u30a2\u30ab\u30ce\u30a4",
-        "name": "\u8d64\u91ce\u4e95",
-        "roma": "akanoi"
+        "hira": "\u3064\u3044\u304d",
+        "kana": "\u30c4\u30a4\u30ad",
+        "name": "\u7bc9\u57ce",
+        "roma": "tsuiki"
     },
     "004": {
         "code": "004",
-        "hira": "\u3042\u3051\u3068\u307f",
-        "kana": "\u30a2\u30b1\u30c8\u30df",
-        "name": "\u660e\u5bcc",
-        "roma": "aketomi"
-    },
-    "006": {
-        "code": "006",
-        "hira": "\u304b\u308f\u306b\u3057",
-        "kana": "\u30ab\u30ef\u30cb\u30b7",
-        "name": "\u6cb3\u897f",
-        "roma": "kawanishi"
+        "hira": "\u3057\u3044\u3060",
+        "kana": "\u30b7\u30a4\u30c0",
+        "name": "\u690e\u7530",
+        "roma": "shiida"
+    },
+    "012": {
+        "code": "012",
+        "hira": "\u3076\u305c\u3093",
+        "kana": "\u30d6\u30bc\u30f3",
+        "name": "\u8c4a\u524d",
+        "roma": "buzen"
+    },
+    "021": {
+        "code": "021",
+        "hira": "\u3061\u304f\u3068\u3046",
+        "kana": "\u30c1\u30af\u30c8\u30a6",
+        "name": "\u7bc9\u6771",
+        "roma": "chikutou"
     },
     "100": {
         "code": "100",
-        "hira": "\u3082\u308a\u3084\u307e",
-        "kana": "\u30e2\u30ea\u30e4\u30de",
-        "name": "\u5b88\u5c71",
-        "roma": "moriyama"
-    },
-    "120": {
-        "code": "120",
-        "hira": "\u3084\u3059",
-        "kana": "\u30e4\u30b9",
-        "name": "\u91ce\u6d32",
-        "roma": "yasu"
+        "hira": "\u307b\u3093\u3066\u3093",
+        "kana": "\u30db\u30f3\u30c6\u30f3",
+        "name": "\u672c\u5e97",
+        "roma": "honten"
+    },
+    "105": {
+        "code": "105",
+        "hira": "\u3086\u304f\u306f\u3057\u3061\u3086\u3046\u304a\u3046",
+        "kana": "\u30e6\u30af\u30cf\u30b7\u30c1\u30e6\u30a6\u30aa\u30a6",
+        "name": "\u884c\u6a4b\u4e2d\u592e",
+        "roma": "yukuhashichiyuuou"
+    },
+    "108": {
+        "code": "108",
+        "hira": "\u3086\u304f\u306f\u3057\u307f\u306a\u307f",
+        "kana": "\u30e6\u30af\u30cf\u30b7\u30df\u30ca\u30df",
+        "name": "\u884c\u6a4b\u5357",
+        "roma": "yukuhashiminami"
+    },
+    "111": {
+        "code": "111",
+        "hira": "\u304b\u3093\u3060",
+        "kana": "\u30ab\u30f3\u30c0",
+        "name": "\u82c5\u7530",
+        "roma": "kanda"
     },
     "121": {
         "code": "121",
-        "hira": "\u304e\u304a\u3046",
-        "kana": "\u30ae\u30aa\u30a6",
-        "name": "\u7947\u738b",
-        "roma": "giou"
-    },
-    "123": {
-        "code": "123",
-        "hira": "\u307f\u304b\u307f",
-        "kana": "\u30df\u30ab\u30df",
-        "name": "\u4e09\u4e0a",
-        "roma": "mikami"
-    },
-    "130": {
-        "code": "130",
-        "hira": "\u3061\u3086\u3046\u305a",
-        "kana": "\u30c1\u30e6\u30a6\u30ba",
-        "name": "\u4e2d\u4e3b",
-        "roma": "chiyuuzu"
+        "hira": "\u3068\u3088\u3064",
+        "kana": "\u30c8\u30e8\u30c4",
+        "name": "\u8c4a\u6d25",
+        "roma": "toyotsu"
+    },
+    "131": {
+        "code": "131",
+        "hira": "\u3055\u3044\u304c\u308f",
+        "kana": "\u30b5\u30a4\u30ac\u30ef",
+        "name": "\u7280\u5ddd",
+        "roma": "saigawa"
+    },
+    "141": {
+        "code": "141",
+        "hira": "\u304b\u3064\u3084\u307e",
+        "kana": "\u30ab\u30c4\u30e4\u30de",
+        "name": "\u52dd\u5c71",
+        "roma": "katsuyama"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6889.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6889.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6897.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6897.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6912.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6912.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6919.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6919.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6924.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6924.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6941.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6941.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6956.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6956.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6961.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6961.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6990.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6990.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/6996.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/6996.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7025.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7025.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7029.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7029.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7032.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7032.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7041.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7041.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7087.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7087.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7092.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7092.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7111.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7111.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7139.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7139.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7156.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7156.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7164.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7164.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7184.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7184.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7193.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7193.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7200.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7200.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7213.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7213.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7239.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7239.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7240.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7240.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7249.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7249.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7264.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7264.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7274.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7274.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7288.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7288.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7338.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7338.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7353.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7353.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7362.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7362.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7363.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7363.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7373.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7373.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7387.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7387.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7532.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7532.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7541.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7541.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7543.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7543.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7550.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7550.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7559.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7559.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7565.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7565.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7576.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7576.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7591.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7591.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7601.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7601.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7625.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7625.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7641.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7641.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7708.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7708.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7755.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7755.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7768.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7768.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7794.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7794.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7825.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7825.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7837.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7837.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7847.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7847.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7859.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7859.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7868.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7868.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7889.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7889.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7909.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7909.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7913.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7913.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7916.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7916.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7938.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7938.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7981.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7981.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/7994.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/7994.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8027.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8027.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8029.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8029.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8047.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8047.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8069.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8069.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8076.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8076.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8096.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8096.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8102.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8102.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8103.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8103.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8118.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8118.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8134.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8134.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8143.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8143.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8153.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8153.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8166.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8166.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8181.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8181.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8197.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8197.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8200.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8200.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8223.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8223.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8231.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8231.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8234.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8234.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8242.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8242.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8252.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8252.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8268.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8268.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8323.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8323.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8332.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8332.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8389.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8389.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8395.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8395.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8397.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8397.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8398.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8398.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8400.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8400.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8425.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8425.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8457.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8457.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8463.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8463.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8477.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8477.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8482.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8482.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8500.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8500.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8512.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8512.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8514.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8514.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8524.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8524.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8544.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8544.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8551.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8551.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8582.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8582.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8589.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8589.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8610.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8610.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8621.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8621.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8626.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8626.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8632.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8632.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8633.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8633.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8635.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8635.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8636.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8636.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8645.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8645.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8653.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8653.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8656.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8656.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8660.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9483.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.08333333333333333%*

 * *Differences: {"'002'": "OrderedDict([('code', '002'), ('name', '福山'), ('kana', 'フクヤマ'), ('hira', 'ふくやま'), "*

 * *          "('roma', 'fukuyama')])",*

 * * "'035'": "OrderedDict([('code', '035'), ('name', '広島西'), ('kana', 'ヒロシマニシ'), ('hira', 'ひろしまにし'), "*

 * *          "('roma', 'hiroshimanishi')])",*

 * * "'040'": "OrderedDict([('code', '040'), ('name', '地御前'), ('kana', 'ヂゴゼン'), ('hira', 'ぢごぜん'), "*

 * *          "('roma', 'digozen')])",*

 * * "'095'": "OrderedDict([('code', '095'), ('name', '江能'), ('kana', 'エノウ'), ('hira', 'えのう'), "*

 * *          "('ro […]*

```diff
@@ -2,43 +2,50 @@
     "001": {
         "code": "001",
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
         "name": "\u672c\u5e97",
         "roma": "honten"
     },
-    "007": {
-        "code": "007",
-        "hira": "\u3061\u3086\u3046\u304a\u3046",
-        "kana": "\u30c1\u30e6\u30a6\u30aa\u30a6",
-        "name": "\u4e2d\u592e",
-        "roma": "chiyuuou"
-    },
-    "009": {
-        "code": "009",
-        "hira": "\u306a\u3093\u3076",
-        "kana": "\u30ca\u30f3\u30d6",
-        "name": "\u5357\u90e8",
-        "roma": "nambu"
-    },
-    "011": {
-        "code": "011",
-        "hira": "\u307b\u304f\u3076",
-        "kana": "\u30db\u30af\u30d6",
-        "name": "\u5317\u90e8",
-        "roma": "hokubu"
-    },
-    "014": {
-        "code": "014",
-        "hira": "\u3068\u3046\u3076",
-        "kana": "\u30c8\u30a6\u30d6",
-        "name": "\u6771\u90e8",
-        "roma": "toubu"
-    },
-    "017": {
-        "code": "017",
-        "hira": "\u305b\u3044\u3076",
-        "kana": "\u30bb\u30a4\u30d6",
-        "name": "\u897f\u90e8",
-        "roma": "seibu"
+    "002": {
+        "code": "002",
+        "hira": "\u3075\u304f\u3084\u307e",
+        "kana": "\u30d5\u30af\u30e4\u30de",
+        "name": "\u798f\u5c71",
+        "roma": "fukuyama"
+    },
+    "035": {
+        "code": "035",
+        "hira": "\u3072\u308d\u3057\u307e\u306b\u3057",
+        "kana": "\u30d2\u30ed\u30b7\u30de\u30cb\u30b7",
+        "name": "\u5e83\u5cf6\u897f",
+        "roma": "hiroshimanishi"
+    },
+    "040": {
+        "code": "040",
+        "hira": "\u3062\u3054\u305c\u3093",
+        "kana": "\u30c2\u30b4\u30bc\u30f3",
+        "name": "\u5730\u5fa1\u524d",
+        "roma": "digozen"
+    },
+    "095": {
+        "code": "095",
+        "hira": "\u3048\u306e\u3046",
+        "kana": "\u30a8\u30ce\u30a6",
+        "name": "\u6c5f\u80fd",
+        "roma": "enou"
+    },
+    "125": {
+        "code": "125",
+        "hira": "\u304a\u3093\u3069",
+        "kana": "\u30aa\u30f3\u30c9",
+        "name": "\u97f3\u6238",
+        "roma": "ondo"
+    },
+    "225": {
+        "code": "225",
+        "hira": "\u304a\u306e\u307f\u3061",
+        "kana": "\u30aa\u30ce\u30df\u30c1",
+        "name": "\u5c3e\u9053",
+        "roma": "onomichi"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8667.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8667.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8668.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8668.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8680.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8680.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8689.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8689.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8692.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8692.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8694.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8694.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8701.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8701.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8715.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8715.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8730.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9213.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.11818181818181818%*

 * *Differences: {"'001'": "{'name': '日向', 'kana': 'ヒユウガ', 'hira': 'ひゆうが', 'roma': 'hiyuuga'}",*

 * * "'002'": "OrderedDict([('code', '002'), ('name', '岩脇'), ('kana', 'イワワキ'), ('hira', 'いわわき'), "*

 * *          "('roma', 'iwawaki')])",*

 * * "'003'": "OrderedDict([('code', '003'), ('name', '美々津'), ('kana', 'ミミツ'), ('hira', 'みみつ'), "*

 * *          "('roma', 'mimitsu')])",*

 * * "'004'": "{'name': '日知屋', 'kana': 'ヒチヤ', 'hira': 'ひちや', 'roma': 'hichiya'}",*

 * * "'005'": "OrderedDict([('code', '005'), ('name', '財光寺'), ('kana', 'ザイコウジ'), ('hira', 'ざいこうじ'),  […]*

```diff
@@ -1,79 +1,100 @@
 {
     "001": {
         "code": "001",
-        "hira": "\u3064\u3044\u304d",
-        "kana": "\u30c4\u30a4\u30ad",
-        "name": "\u7bc9\u57ce",
-        "roma": "tsuiki"
+        "hira": "\u3072\u3086\u3046\u304c",
+        "kana": "\u30d2\u30e6\u30a6\u30ac",
+        "name": "\u65e5\u5411",
+        "roma": "hiyuuga"
+    },
+    "002": {
+        "code": "002",
+        "hira": "\u3044\u308f\u308f\u304d",
+        "kana": "\u30a4\u30ef\u30ef\u30ad",
+        "name": "\u5ca9\u8107",
+        "roma": "iwawaki"
+    },
+    "003": {
+        "code": "003",
+        "hira": "\u307f\u307f\u3064",
+        "kana": "\u30df\u30df\u30c4",
+        "name": "\u7f8e\u3005\u6d25",
+        "roma": "mimitsu"
     },
     "004": {
         "code": "004",
-        "hira": "\u3057\u3044\u3060",
-        "kana": "\u30b7\u30a4\u30c0",
-        "name": "\u690e\u7530",
-        "roma": "shiida"
-    },
-    "012": {
-        "code": "012",
-        "hira": "\u3076\u305c\u3093",
-        "kana": "\u30d6\u30bc\u30f3",
-        "name": "\u8c4a\u524d",
-        "roma": "buzen"
-    },
-    "021": {
-        "code": "021",
-        "hira": "\u3061\u304f\u3068\u3046",
-        "kana": "\u30c1\u30af\u30c8\u30a6",
-        "name": "\u7bc9\u6771",
-        "roma": "chikutou"
+        "hira": "\u3072\u3061\u3084",
+        "kana": "\u30d2\u30c1\u30e4",
+        "name": "\u65e5\u77e5\u5c4b",
+        "roma": "hichiya"
+    },
+    "005": {
+        "code": "005",
+        "hira": "\u3056\u3044\u3053\u3046\u3058",
+        "kana": "\u30b6\u30a4\u30b3\u30a6\u30b8",
+        "name": "\u8ca1\u5149\u5bfa",
+        "roma": "zaikouji"
+    },
+    "006": {
+        "code": "006",
+        "hira": "\u3057\u304a\u307f",
+        "kana": "\u30b7\u30aa\u30df",
+        "name": "\u5869\u898b",
+        "roma": "shiomi"
+    },
+    "010": {
+        "code": "010",
+        "hira": "\u304b\u3069\u304c\u308f",
+        "kana": "\u30ab\u30c9\u30ac\u30ef",
+        "name": "\u9580\u5ddd",
+        "roma": "kadogawa"
+    },
+    "030": {
+        "code": "030",
+        "hira": "\u3068\u3046\u3054\u3046",
+        "kana": "\u30c8\u30a6\u30b4\u30a6",
+        "name": "\u6771\u90f7",
+        "roma": "tougou"
+    },
+    "040": {
+        "code": "040",
+        "hira": "\u306a\u3093\u3054\u3046",
+        "kana": "\u30ca\u30f3\u30b4\u30a6",
+        "name": "\u5357\u90f7",
+        "roma": "nangou"
+    },
+    "050": {
+        "code": "050",
+        "hira": "\u3055\u3044\u3054\u3046",
+        "kana": "\u30b5\u30a4\u30b4\u30a6",
+        "name": "\u897f\u90f7",
+        "roma": "saigou"
+    },
+    "060": {
+        "code": "060",
+        "hira": "\u304d\u305f\u3054\u3046",
+        "kana": "\u30ad\u30bf\u30b4\u30a6",
+        "name": "\u5317\u90f7",
+        "roma": "kitagou"
+    },
+    "070": {
+        "code": "070",
+        "hira": "\u3082\u308d\u3064\u304b",
+        "kana": "\u30e2\u30ed\u30c4\u30ab",
+        "name": "\u8af8\u585a",
+        "roma": "morotsuka"
+    },
+    "080": {
+        "code": "080",
+        "hira": "\u3057\u3044\u3070",
+        "kana": "\u30b7\u30a4\u30d0",
+        "name": "\u690e\u8449",
+        "roma": "shiiba"
     },
     "100": {
         "code": "100",
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
         "name": "\u672c\u5e97",
         "roma": "honten"
-    },
-    "105": {
-        "code": "105",
-        "hira": "\u3086\u304f\u306f\u3057\u3061\u3086\u3046\u304a\u3046",
-        "kana": "\u30e6\u30af\u30cf\u30b7\u30c1\u30e6\u30a6\u30aa\u30a6",
-        "name": "\u884c\u6a4b\u4e2d\u592e",
-        "roma": "yukuhashichiyuuou"
-    },
-    "108": {
-        "code": "108",
-        "hira": "\u3086\u304f\u306f\u3057\u307f\u306a\u307f",
-        "kana": "\u30e6\u30af\u30cf\u30b7\u30df\u30ca\u30df",
-        "name": "\u884c\u6a4b\u5357",
-        "roma": "yukuhashiminami"
-    },
-    "111": {
-        "code": "111",
-        "hira": "\u304b\u3093\u3060",
-        "kana": "\u30ab\u30f3\u30c0",
-        "name": "\u82c5\u7530",
-        "roma": "kanda"
-    },
-    "121": {
-        "code": "121",
-        "hira": "\u3068\u3088\u3064",
-        "kana": "\u30c8\u30e8\u30c4",
-        "name": "\u8c4a\u6d25",
-        "roma": "toyotsu"
-    },
-    "131": {
-        "code": "131",
-        "hira": "\u3055\u3044\u304c\u308f",
-        "kana": "\u30b5\u30a4\u30ac\u30ef",
-        "name": "\u7280\u5ddd",
-        "roma": "saigawa"
-    },
-    "141": {
-        "code": "141",
-        "hira": "\u304b\u3064\u3084\u307e",
-        "kana": "\u30ab\u30c4\u30e4\u30de",
-        "name": "\u52dd\u5c71",
-        "roma": "katsuyama"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8762.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8762.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8766.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8766.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8771.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8771.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8794.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8794.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8813.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8813.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8829.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8829.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8857.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8857.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8893.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8893.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8906.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8906.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8916.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8916.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9090909090909091%*

 * *Differences: {'delete': "['011', '012']"}*

```diff
@@ -30,28 +30,14 @@
     "009": {
         "code": "009",
         "hira": "\u306a\u3093\u3076",
         "kana": "\u30ca\u30f3\u30d6",
         "name": "\u5357\u90e8",
         "roma": "nambu"
     },
-    "011": {
-        "code": "011",
-        "hira": "\u304b\u308f\u3057\u308a",
-        "kana": "\u30ab\u30ef\u30b7\u30ea",
-        "name": "\u5ddd\u5c3b",
-        "roma": "kawashiri"
-    },
-    "012": {
-        "code": "012",
-        "hira": "\u308a\u304d\u3054\u3046",
-        "kana": "\u30ea\u30ad\u30b4\u30a6",
-        "name": "\u529b\u5408",
-        "roma": "rikigou"
-    },
     "013": {
         "code": "013",
         "hira": "\u304f\u307e\u306a\u3093",
         "kana": "\u30af\u30de\u30ca\u30f3",
         "name": "\u304f\u307e\u306a\u3093",
         "roma": "kumanan"
     },
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8926.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8926.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8941.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8941.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8949.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8949.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8964.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8964.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/8982.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/8982.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9010.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9270.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('100', OrderedDict([('code', '100'), ('name', '本所'), ('kana', 'ホンシヨ'), "*

 * *            "('hira', 'ほんしよ'), ('roma', 'honshiyo')])), ('101', OrderedDict([('code', '101'), "*

 * *            "('name', '串木野'), ('kana', 'クシキノ'), ('hira', 'くしきの'), ('roma', 'kushikino')])), "*

 * *            "('107', OrderedDict([('code', '107'), ('name', '市来'), ('kana', 'イチキ'), ('hira', "*

 * *            "'いちき'), ('roma', 'ichiki')])), ('109', OrderedDict([('code', '109'), ('name', '東市来'), "*

 * *            "('kana', 'ヒガシ […]*

```diff
@@ -1,65 +1,72 @@
 {
-    "001": {
-        "code": "001",
+    "100": {
+        "code": "100",
         "hira": "\u307b\u3093\u3057\u3088",
         "kana": "\u30db\u30f3\u30b7\u30e8",
         "name": "\u672c\u6240",
         "roma": "honshiyo"
     },
-    "002": {
-        "code": "002",
-        "hira": "\u307e\u3064\u3070\u305b",
-        "kana": "\u30de\u30c4\u30d0\u30bb",
-        "name": "\u677e\u6a4b",
-        "roma": "matsubase"
-    },
-    "007": {
-        "code": "007",
-        "hira": "\u3057\u3082\u304d\u305f",
-        "kana": "\u30b7\u30e2\u30ad\u30bf",
-        "name": "\u4e0b\u5317",
-        "roma": "shimokita"
-    },
-    "009": {
-        "code": "009",
-        "hira": "\u3068\u307f\u3042\u3044",
-        "kana": "\u30c8\u30df\u30a2\u30a4",
-        "name": "\u5bcc\u5408",
-        "roma": "tomiai"
-    },
-    "012": {
-        "code": "012",
-        "hira": "\u304a\u304c\u308f\u307e\u3061",
-        "kana": "\u30aa\u30ac\u30ef\u30de\u30c1",
-        "name": "\u5c0f\u5ddd\u753a",
-        "roma": "ogawamachi"
-    },
-    "017": {
-        "code": "017",
-        "hira": "\u3057\u3082\u3072\u304c\u3057",
-        "kana": "\u30b7\u30e2\u30d2\u30ac\u30b7",
-        "name": "\u4e0b\u6771",
-        "roma": "shimohigashi"
-    },
-    "023": {
-        "code": "023",
-        "hira": "\u3046\u3068",
-        "kana": "\u30a6\u30c8",
-        "name": "\u5b87\u571f",
-        "roma": "uto"
-    },
-    "030": {
-        "code": "030",
-        "hira": "\u307f\u3059\u307f",
-        "kana": "\u30df\u30b9\u30df",
-        "name": "\u4e09\u89d2",
-        "roma": "misumi"
-    },
-    "035": {
-        "code": "035",
-        "hira": "\u3057\u3089\u306c\u3072",
-        "kana": "\u30b7\u30e9\u30cc\u30d2",
-        "name": "\u4e0d\u77e5\u706b",
-        "roma": "shiranuhi"
+    "101": {
+        "code": "101",
+        "hira": "\u304f\u3057\u304d\u306e",
+        "kana": "\u30af\u30b7\u30ad\u30ce",
+        "name": "\u4e32\u6728\u91ce",
+        "roma": "kushikino"
+    },
+    "107": {
+        "code": "107",
+        "hira": "\u3044\u3061\u304d",
+        "kana": "\u30a4\u30c1\u30ad",
+        "name": "\u5e02\u6765",
+        "roma": "ichiki"
+    },
+    "109": {
+        "code": "109",
+        "hira": "\u3072\u304c\u3057\u3044\u3061\u304d",
+        "kana": "\u30d2\u30ac\u30b7\u30a4\u30c1\u30ad",
+        "name": "\u6771\u5e02\u6765",
+        "roma": "higashiichiki"
+    },
+    "113": {
+        "code": "113",
+        "hira": "\u3044\u3058\u3086\u3046\u3044\u3093",
+        "kana": "\u30a4\u30b8\u30e6\u30a6\u30a4\u30f3",
+        "name": "\u4f0a\u96c6\u9662",
+        "roma": "ijiyuuin"
+    },
+    "118": {
+        "code": "118",
+        "hira": "\u307e\u3064\u3082\u3068",
+        "kana": "\u30de\u30c4\u30e2\u30c8",
+        "name": "\u677e\u5143",
+        "roma": "matsumoto"
+    },
+    "122": {
+        "code": "122",
+        "hira": "\u3053\u304a\u308a\u3084\u307e",
+        "kana": "\u30b3\u30aa\u30ea\u30e4\u30de",
+        "name": "\u90e1\u5c71",
+        "roma": "kooriyama"
+    },
+    "124": {
+        "code": "124",
+        "hira": "\u3072\u3088\u3057",
+        "kana": "\u30d2\u30e8\u30b7",
+        "name": "\u65e5\u5409",
+        "roma": "hiyoshi"
+    },
+    "126": {
+        "code": "126",
+        "hira": "\u3075\u304d\u3042\u3052",
+        "kana": "\u30d5\u30ad\u30a2\u30b2",
+        "name": "\u5439\u4e0a",
+        "roma": "fukiage"
+    },
+    "128": {
+        "code": "128",
+        "hira": "\u304d\u3093\u307d\u3046",
+        "kana": "\u30ad\u30f3\u30dd\u30a6",
+        "name": "\u91d1\u5cf0",
+        "roma": "kimpou"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9017.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9017.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9043.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9043.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9048.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9048.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9070.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9070.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9104.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9104.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9169.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9169.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9178.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9178.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9184.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9184.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9193.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9193.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9205.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9205.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9208.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9208.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9213.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/1917.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25263157894736843%*

 * *Differences: {"'001'": "{'name': '本店営業部', 'kana': 'ホンテン', 'hira': 'ほんてん', 'roma': 'honten'}",*

 * * "'003'": "{'name': '田口', 'kana': 'タグチ', 'hira': 'たぐち', 'roma': 'taguchi'}",*

 * * "'004'": "{'name': '大木', 'kana': 'オオキ', 'hira': 'おおき', 'roma': 'ooki'}",*

 * * "'005'": "{'name': '城島', 'kana': 'ジヨウジマ', 'hira': 'じようじま', 'roma': 'jiyoujima'}",*

 * * "'006'": "{'name': '諸富', 'kana': 'モロドミ', 'hira': 'もろどみ', 'roma': 'morodomi'}",*

 * * "'007'": "OrderedDict([('code', '007'), ('name', '木室'), ('kana', 'キムロ'), ('hira', 'きむろ'), "*

 * *          "('roma', 'kim […]*

```diff
@@ -1,100 +1,79 @@
 {
     "001": {
         "code": "001",
-        "hira": "\u3072\u3086\u3046\u304c",
-        "kana": "\u30d2\u30e6\u30a6\u30ac",
-        "name": "\u65e5\u5411",
-        "roma": "hiyuuga"
-    },
-    "002": {
-        "code": "002",
-        "hira": "\u3044\u308f\u308f\u304d",
-        "kana": "\u30a4\u30ef\u30ef\u30ad",
-        "name": "\u5ca9\u8107",
-        "roma": "iwawaki"
+        "hira": "\u307b\u3093\u3066\u3093",
+        "kana": "\u30db\u30f3\u30c6\u30f3",
+        "name": "\u672c\u5e97\u55b6\u696d\u90e8",
+        "roma": "honten"
     },
     "003": {
         "code": "003",
-        "hira": "\u307f\u307f\u3064",
-        "kana": "\u30df\u30df\u30c4",
-        "name": "\u7f8e\u3005\u6d25",
-        "roma": "mimitsu"
+        "hira": "\u305f\u3050\u3061",
+        "kana": "\u30bf\u30b0\u30c1",
+        "name": "\u7530\u53e3",
+        "roma": "taguchi"
     },
     "004": {
         "code": "004",
-        "hira": "\u3072\u3061\u3084",
-        "kana": "\u30d2\u30c1\u30e4",
-        "name": "\u65e5\u77e5\u5c4b",
-        "roma": "hichiya"
+        "hira": "\u304a\u304a\u304d",
+        "kana": "\u30aa\u30aa\u30ad",
+        "name": "\u5927\u6728",
+        "roma": "ooki"
     },
     "005": {
         "code": "005",
-        "hira": "\u3056\u3044\u3053\u3046\u3058",
-        "kana": "\u30b6\u30a4\u30b3\u30a6\u30b8",
-        "name": "\u8ca1\u5149\u5bfa",
-        "roma": "zaikouji"
+        "hira": "\u3058\u3088\u3046\u3058\u307e",
+        "kana": "\u30b8\u30e8\u30a6\u30b8\u30de",
+        "name": "\u57ce\u5cf6",
+        "roma": "jiyoujima"
     },
     "006": {
         "code": "006",
-        "hira": "\u3057\u304a\u307f",
-        "kana": "\u30b7\u30aa\u30df",
-        "name": "\u5869\u898b",
-        "roma": "shiomi"
+        "hira": "\u3082\u308d\u3069\u307f",
+        "kana": "\u30e2\u30ed\u30c9\u30df",
+        "name": "\u8af8\u5bcc",
+        "roma": "morodomi"
+    },
+    "007": {
+        "code": "007",
+        "hira": "\u304d\u3080\u308d",
+        "kana": "\u30ad\u30e0\u30ed",
+        "name": "\u6728\u5ba4",
+        "roma": "kimuro"
+    },
+    "008": {
+        "code": "008",
+        "hira": "\u304b\u308f\u3050\u3061",
+        "kana": "\u30ab\u30ef\u30b0\u30c1",
+        "name": "\u5ddd\u53e3",
+        "roma": "kawaguchi"
+    },
+    "009": {
+        "code": "009",
+        "hira": "\u307f\u3064\u307e\u305f",
+        "kana": "\u30df\u30c4\u30de\u30bf",
+        "name": "\u4e09\u53c8",
+        "roma": "mitsumata"
     },
     "010": {
         "code": "010",
-        "hira": "\u304b\u3069\u304c\u308f",
-        "kana": "\u30ab\u30c9\u30ac\u30ef",
-        "name": "\u9580\u5ddd",
-        "roma": "kadogawa"
-    },
-    "030": {
-        "code": "030",
-        "hira": "\u3068\u3046\u3054\u3046",
-        "kana": "\u30c8\u30a6\u30b4\u30a6",
-        "name": "\u6771\u90f7",
-        "roma": "tougou"
-    },
-    "040": {
-        "code": "040",
-        "hira": "\u306a\u3093\u3054\u3046",
-        "kana": "\u30ca\u30f3\u30b4\u30a6",
-        "name": "\u5357\u90f7",
-        "roma": "nangou"
-    },
-    "050": {
-        "code": "050",
-        "hira": "\u3055\u3044\u3054\u3046",
-        "kana": "\u30b5\u30a4\u30b4\u30a6",
-        "name": "\u897f\u90f7",
-        "roma": "saigou"
-    },
-    "060": {
-        "code": "060",
-        "hira": "\u304d\u305f\u3054\u3046",
-        "kana": "\u30ad\u30bf\u30b4\u30a6",
-        "name": "\u5317\u90f7",
-        "roma": "kitagou"
-    },
-    "070": {
-        "code": "070",
-        "hira": "\u3082\u308d\u3064\u304b",
-        "kana": "\u30e2\u30ed\u30c4\u30ab",
-        "name": "\u8af8\u585a",
-        "roma": "morotsuka"
-    },
-    "080": {
-        "code": "080",
-        "hira": "\u3057\u3044\u3070",
-        "kana": "\u30b7\u30a4\u30d0",
-        "name": "\u690e\u8449",
-        "roma": "shiiba"
-    },
-    "100": {
-        "code": "100",
-        "hira": "\u307b\u3093\u3066\u3093",
-        "kana": "\u30db\u30f3\u30c6\u30f3",
-        "name": "\u672c\u5e97",
-        "roma": "honten"
+        "hira": "\u307f\u3065\u307e",
+        "kana": "\u30df\u30c5\u30de",
+        "name": "\u30df\u30c5\u30de",
+        "roma": "miduma"
+    },
+    "011": {
+        "code": "011",
+        "hira": "\u3055\u3051\u307f",
+        "kana": "\u30b5\u30b1\u30df",
+        "name": "\u9152\u898b",
+        "roma": "sakemi"
+    },
+    "012": {
+        "code": "012",
+        "hira": "\u3086\u3081\u3055\u304d",
+        "kana": "\u30e6\u30e1\u30b5\u30ad",
+        "name": "\u3086\u3081\u54b2",
+        "roma": "yumesaki"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9221.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9221.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9229.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9229.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9234.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9234.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9251.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9251.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9257.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9257.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9270.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9319.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2210526315789474%*

 * *Differences: {"'101'": "{'name': '加治木', 'kana': 'カジキ', 'hira': 'かじき', 'roma': 'kajiki'}",*

 * * "'105'": "OrderedDict([('code', '105'), ('name', '姶良町'), ('kana', 'アイラチヨウ'), ('hira', 'あいらちよう'), "*

 * *          "('roma', 'airachiyou')])",*

 * * "'111'": "OrderedDict([('code', '111'), ('name', '蒲生'), ('kana', 'カモウ'), ('hira', 'かもう'), "*

 * *          "('roma', 'kamou')])",*

 * * "'112'": "OrderedDict([('code', '112'), ('name', '溝辺'), ('kana', 'ミゾベ'), ('hira', 'みぞべ'), "*

 * *          "('roma', 'mizobe')])",*

 * * "'116'": "OrderedDict([('code', '116'), ('n […]*

```diff
@@ -4,69 +4,97 @@
         "hira": "\u307b\u3093\u3057\u3088",
         "kana": "\u30db\u30f3\u30b7\u30e8",
         "name": "\u672c\u6240",
         "roma": "honshiyo"
     },
     "101": {
         "code": "101",
-        "hira": "\u304f\u3057\u304d\u306e",
-        "kana": "\u30af\u30b7\u30ad\u30ce",
-        "name": "\u4e32\u6728\u91ce",
-        "roma": "kushikino"
-    },
-    "107": {
-        "code": "107",
-        "hira": "\u3044\u3061\u304d",
-        "kana": "\u30a4\u30c1\u30ad",
-        "name": "\u5e02\u6765",
-        "roma": "ichiki"
-    },
-    "109": {
-        "code": "109",
-        "hira": "\u3072\u304c\u3057\u3044\u3061\u304d",
-        "kana": "\u30d2\u30ac\u30b7\u30a4\u30c1\u30ad",
-        "name": "\u6771\u5e02\u6765",
-        "roma": "higashiichiki"
-    },
-    "113": {
-        "code": "113",
-        "hira": "\u3044\u3058\u3086\u3046\u3044\u3093",
-        "kana": "\u30a4\u30b8\u30e6\u30a6\u30a4\u30f3",
-        "name": "\u4f0a\u96c6\u9662",
-        "roma": "ijiyuuin"
+        "hira": "\u304b\u3058\u304d",
+        "kana": "\u30ab\u30b8\u30ad",
+        "name": "\u52a0\u6cbb\u6728",
+        "roma": "kajiki"
+    },
+    "105": {
+        "code": "105",
+        "hira": "\u3042\u3044\u3089\u3061\u3088\u3046",
+        "kana": "\u30a2\u30a4\u30e9\u30c1\u30e8\u30a6",
+        "name": "\u59f6\u826f\u753a",
+        "roma": "airachiyou"
+    },
+    "111": {
+        "code": "111",
+        "hira": "\u304b\u3082\u3046",
+        "kana": "\u30ab\u30e2\u30a6",
+        "name": "\u84b2\u751f",
+        "roma": "kamou"
+    },
+    "112": {
+        "code": "112",
+        "hira": "\u307f\u305e\u3079",
+        "kana": "\u30df\u30be\u30d9",
+        "name": "\u6e9d\u8fba",
+        "roma": "mizobe"
+    },
+    "116": {
+        "code": "116",
+        "hira": "\u3088\u3053\u304c\u308f",
+        "kana": "\u30e8\u30b3\u30ac\u30ef",
+        "name": "\u6a2a\u5ddd",
+        "roma": "yokogawa"
     },
     "118": {
         "code": "118",
-        "hira": "\u307e\u3064\u3082\u3068",
-        "kana": "\u30de\u30c4\u30e2\u30c8",
-        "name": "\u677e\u5143",
-        "roma": "matsumoto"
+        "hira": "\u304f\u308a\u306e",
+        "kana": "\u30af\u30ea\u30ce",
+        "name": "\u6817\u91ce",
+        "roma": "kurino"
+    },
+    "121": {
+        "code": "121",
+        "hira": "\u3088\u3057\u307e\u3064",
+        "kana": "\u30e8\u30b7\u30de\u30c4",
+        "name": "\u5409\u677e",
+        "roma": "yoshimatsu"
     },
     "122": {
         "code": "122",
-        "hira": "\u3053\u304a\u308a\u3084\u307e",
-        "kana": "\u30b3\u30aa\u30ea\u30e4\u30de",
-        "name": "\u90e1\u5c71",
-        "roma": "kooriyama"
-    },
-    "124": {
-        "code": "124",
-        "hira": "\u3072\u3088\u3057",
-        "kana": "\u30d2\u30e8\u30b7",
-        "name": "\u65e5\u5409",
-        "roma": "hiyoshi"
-    },
-    "126": {
-        "code": "126",
-        "hira": "\u3075\u304d\u3042\u3052",
-        "kana": "\u30d5\u30ad\u30a2\u30b2",
-        "name": "\u5439\u4e0a",
-        "roma": "fukiage"
+        "hira": "\u307e\u304d\u305e\u306e",
+        "kana": "\u30de\u30ad\u30be\u30ce",
+        "name": "\u7267\u5712",
+        "roma": "makizono"
+    },
+    "123": {
+        "code": "123",
+        "hira": "\u306f\u3084\u3068",
+        "kana": "\u30cf\u30e4\u30c8",
+        "name": "\u96bc\u4eba",
+        "roma": "hayato"
     },
     "128": {
         "code": "128",
-        "hira": "\u304d\u3093\u307d\u3046",
-        "kana": "\u30ad\u30f3\u30dd\u30a6",
-        "name": "\u91d1\u5cf0",
-        "roma": "kimpou"
+        "hira": "\u304d\u308a\u3057\u307e",
+        "kana": "\u30ad\u30ea\u30b7\u30de",
+        "name": "\u9727\u5cf6",
+        "roma": "kirishima"
+    },
+    "130": {
+        "code": "130",
+        "hira": "\u3053\u304f\u3076",
+        "kana": "\u30b3\u30af\u30d6",
+        "name": "\u56fd\u5206",
+        "roma": "kokubu"
+    },
+    "135": {
+        "code": "135",
+        "hira": "\u307e\u304d\u306e\u306f\u3089",
+        "kana": "\u30de\u30ad\u30ce\u30cf\u30e9",
+        "name": "\u7267\u4e4b\u539f",
+        "roma": "makinohara"
+    },
+    "140": {
+        "code": "140",
+        "hira": "\u304d\u308a\u3057\u307e\u3057\u3084\u304f\u3057\u3088",
+        "kana": "\u30ad\u30ea\u30b7\u30de\u30b7\u30e4\u30af\u30b7\u30e8",
+        "name": "\u9727\u5cf6\u5e02\u5f79\u6240",
+        "roma": "kirishimashiyakushiyo"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9296.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9296.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9302.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9302.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9319.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9484.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('001', OrderedDict([('code', '001'), ('name', '本店'), ('kana', 'ホンテン'), "*

 * *            "('hira', 'ほんてん'), ('roma', 'honten')])), ('175', OrderedDict([('code', '175'), "*

 * *            "('name', '柳井港'), ('kana', 'ヤナイミナト'), ('hira', 'やないみなと'), ('roma', 'yanaiminato')])), "*

 * *            "('315', OrderedDict([('code', '315'), ('name', '周南'), ('kana', 'シユウナン'), ('hira', "*

 * *            "'しゆうなん'), ('roma', 'shiyuunan')])), ('355', OrderedDict([('code', '355'), ('name', "*

 * *            "'吉佐'), ('k […]*

```diff
@@ -1,100 +1,65 @@
 {
-    "100": {
-        "code": "100",
-        "hira": "\u307b\u3093\u3057\u3088",
-        "kana": "\u30db\u30f3\u30b7\u30e8",
-        "name": "\u672c\u6240",
-        "roma": "honshiyo"
-    },
-    "101": {
-        "code": "101",
-        "hira": "\u304b\u3058\u304d",
-        "kana": "\u30ab\u30b8\u30ad",
-        "name": "\u52a0\u6cbb\u6728",
-        "roma": "kajiki"
-    },
-    "105": {
-        "code": "105",
-        "hira": "\u3042\u3044\u3089\u3061\u3088\u3046",
-        "kana": "\u30a2\u30a4\u30e9\u30c1\u30e8\u30a6",
-        "name": "\u59f6\u826f\u753a",
-        "roma": "airachiyou"
-    },
-    "111": {
-        "code": "111",
-        "hira": "\u304b\u3082\u3046",
-        "kana": "\u30ab\u30e2\u30a6",
-        "name": "\u84b2\u751f",
-        "roma": "kamou"
-    },
-    "112": {
-        "code": "112",
-        "hira": "\u307f\u305e\u3079",
-        "kana": "\u30df\u30be\u30d9",
-        "name": "\u6e9d\u8fba",
-        "roma": "mizobe"
-    },
-    "116": {
-        "code": "116",
-        "hira": "\u3088\u3053\u304c\u308f",
-        "kana": "\u30e8\u30b3\u30ac\u30ef",
-        "name": "\u6a2a\u5ddd",
-        "roma": "yokogawa"
-    },
-    "118": {
-        "code": "118",
-        "hira": "\u304f\u308a\u306e",
-        "kana": "\u30af\u30ea\u30ce",
-        "name": "\u6817\u91ce",
-        "roma": "kurino"
-    },
-    "121": {
-        "code": "121",
-        "hira": "\u3088\u3057\u307e\u3064",
-        "kana": "\u30e8\u30b7\u30de\u30c4",
-        "name": "\u5409\u677e",
-        "roma": "yoshimatsu"
-    },
-    "122": {
-        "code": "122",
-        "hira": "\u307e\u304d\u305e\u306e",
-        "kana": "\u30de\u30ad\u30be\u30ce",
-        "name": "\u7267\u5712",
-        "roma": "makizono"
-    },
-    "123": {
-        "code": "123",
-        "hira": "\u306f\u3084\u3068",
-        "kana": "\u30cf\u30e4\u30c8",
-        "name": "\u96bc\u4eba",
-        "roma": "hayato"
-    },
-    "128": {
-        "code": "128",
-        "hira": "\u304d\u308a\u3057\u307e",
-        "kana": "\u30ad\u30ea\u30b7\u30de",
-        "name": "\u9727\u5cf6",
-        "roma": "kirishima"
-    },
-    "130": {
-        "code": "130",
-        "hira": "\u3053\u304f\u3076",
-        "kana": "\u30b3\u30af\u30d6",
-        "name": "\u56fd\u5206",
-        "roma": "kokubu"
-    },
-    "135": {
-        "code": "135",
-        "hira": "\u307e\u304d\u306e\u306f\u3089",
-        "kana": "\u30de\u30ad\u30ce\u30cf\u30e9",
-        "name": "\u7267\u4e4b\u539f",
-        "roma": "makinohara"
-    },
-    "140": {
-        "code": "140",
-        "hira": "\u304d\u308a\u3057\u307e\u3057\u3084\u304f\u3057\u3088",
-        "kana": "\u30ad\u30ea\u30b7\u30de\u30b7\u30e4\u30af\u30b7\u30e8",
-        "name": "\u9727\u5cf6\u5e02\u5f79\u6240",
-        "roma": "kirishimashiyakushiyo"
+    "001": {
+        "code": "001",
+        "hira": "\u307b\u3093\u3066\u3093",
+        "kana": "\u30db\u30f3\u30c6\u30f3",
+        "name": "\u672c\u5e97",
+        "roma": "honten"
+    },
+    "175": {
+        "code": "175",
+        "hira": "\u3084\u306a\u3044\u307f\u306a\u3068",
+        "kana": "\u30e4\u30ca\u30a4\u30df\u30ca\u30c8",
+        "name": "\u67f3\u4e95\u6e2f",
+        "roma": "yanaiminato"
+    },
+    "315": {
+        "code": "315",
+        "hira": "\u3057\u3086\u3046\u306a\u3093",
+        "kana": "\u30b7\u30e6\u30a6\u30ca\u30f3",
+        "name": "\u5468\u5357",
+        "roma": "shiyuunan"
+    },
+    "355": {
+        "code": "355",
+        "hira": "\u304d\u3064\u3055",
+        "kana": "\u30ad\u30c4\u30b5",
+        "name": "\u5409\u4f50",
+        "roma": "kitsusa"
+    },
+    "390": {
+        "code": "390",
+        "hira": "\u304a\u304a\u307f",
+        "kana": "\u30aa\u30aa\u30df",
+        "name": "\u5927\u6d77",
+        "roma": "oomi"
+    },
+    "510": {
+        "code": "510",
+        "hira": "\u3046\u3079\u307f\u3055\u304d",
+        "kana": "\u30a6\u30d9\u30df\u30b5\u30ad",
+        "name": "\u5b87\u90e8\u5cac",
+        "roma": "ubemisaki"
+    },
+    "815": {
+        "code": "815",
+        "hira": "\u306a\u304c\u3068",
+        "kana": "\u30ca\u30ac\u30c8",
+        "name": "\u9577\u9580",
+        "roma": "nagato"
+    },
+    "930": {
+        "code": "930",
+        "hira": "\u306f\u304e",
+        "kana": "\u30cf\u30ae",
+        "name": "\u306f\u304e",
+        "roma": "hagi"
+    },
+    "955": {
+        "code": "955",
+        "hira": "\u304a\u304a\u3057\u307e",
+        "kana": "\u30aa\u30aa\u30b7\u30de",
+        "name": "\u5927\u5cf6",
+        "roma": "ooshima"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9332.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9332.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9341.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9341.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9353.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9353.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9363.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9363.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9375.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9375.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9450.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9450.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9452.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9452.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9453.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9453.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9461.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9461.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9477.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9477.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9481.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9481.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9483.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/5707.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.16363636363636364%*

 * *Differences: {"'002'": "{'name': '六日町', 'kana': 'ムイカマチ', 'hira': 'むいかまち', 'roma': 'muikamachi'}",*

 * * "'004'": "OrderedDict([('code', '004'), ('name', '城内'), ('kana', 'ジヨウナイ'), ('hira', 'じようない'), "*

 * *          "('roma', 'jiyounai')])",*

 * * "'007'": "OrderedDict([('code', '007'), ('name', '浦佐'), ('kana', 'ウラサ'), ('hira', 'うらさ'), "*

 * *          "('roma', 'urasa')])",*

 * * "'012'": "OrderedDict([('code', '012'), ('name', '塩沢'), ('kana', 'シオザワ'), ('hira', 'しおざわ'), "*

 * *          "('roma', 'shiozawa')])",*

 * * "'015'": "OrderedDict([('code', '015 […]*

```diff
@@ -4,48 +4,41 @@
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
         "name": "\u672c\u5e97",
         "roma": "honten"
     },
     "002": {
         "code": "002",
-        "hira": "\u3075\u304f\u3084\u307e",
-        "kana": "\u30d5\u30af\u30e4\u30de",
-        "name": "\u798f\u5c71",
-        "roma": "fukuyama"
-    },
-    "035": {
-        "code": "035",
-        "hira": "\u3072\u308d\u3057\u307e\u306b\u3057",
-        "kana": "\u30d2\u30ed\u30b7\u30de\u30cb\u30b7",
-        "name": "\u5e83\u5cf6\u897f",
-        "roma": "hiroshimanishi"
-    },
-    "040": {
-        "code": "040",
-        "hira": "\u3062\u3054\u305c\u3093",
-        "kana": "\u30c2\u30b4\u30bc\u30f3",
-        "name": "\u5730\u5fa1\u524d",
-        "roma": "digozen"
-    },
-    "095": {
-        "code": "095",
-        "hira": "\u3048\u306e\u3046",
-        "kana": "\u30a8\u30ce\u30a6",
-        "name": "\u6c5f\u80fd",
-        "roma": "enou"
-    },
-    "125": {
-        "code": "125",
-        "hira": "\u304a\u3093\u3069",
-        "kana": "\u30aa\u30f3\u30c9",
-        "name": "\u97f3\u6238",
-        "roma": "ondo"
-    },
-    "225": {
-        "code": "225",
-        "hira": "\u304a\u306e\u307f\u3061",
-        "kana": "\u30aa\u30ce\u30df\u30c1",
-        "name": "\u5c3e\u9053",
-        "roma": "onomichi"
+        "hira": "\u3080\u3044\u304b\u307e\u3061",
+        "kana": "\u30e0\u30a4\u30ab\u30de\u30c1",
+        "name": "\u516d\u65e5\u753a",
+        "roma": "muikamachi"
+    },
+    "004": {
+        "code": "004",
+        "hira": "\u3058\u3088\u3046\u306a\u3044",
+        "kana": "\u30b8\u30e8\u30a6\u30ca\u30a4",
+        "name": "\u57ce\u5185",
+        "roma": "jiyounai"
+    },
+    "007": {
+        "code": "007",
+        "hira": "\u3046\u3089\u3055",
+        "kana": "\u30a6\u30e9\u30b5",
+        "name": "\u6d66\u4f50",
+        "roma": "urasa"
+    },
+    "012": {
+        "code": "012",
+        "hira": "\u3057\u304a\u3056\u308f",
+        "kana": "\u30b7\u30aa\u30b6\u30ef",
+        "name": "\u5869\u6ca2",
+        "roma": "shiozawa"
+    },
+    "015": {
+        "code": "015",
+        "hira": "\u3086\u3056\u308f",
+        "kana": "\u30e6\u30b6\u30ef",
+        "name": "\u6e6f\u6ca2",
+        "roma": "yuzawa"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9484.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9489.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.05%*

 * *Differences: {"'002'": "OrderedDict([('code', '002'), ('name', '佐賀統括'), ('kana', 'サガトウカツ'), ('hira', 'さがとうかつ'), "*

 * *          "('roma', 'sagatoukatsu')])",*

 * * "'003'": "OrderedDict([('code', '003'), ('name', '有明'), ('kana', 'アリアケ'), ('hira', 'ありあけ'), "*

 * *          "('roma', 'ariake')])",*

 * * "'004'": "OrderedDict([('code', '004'), ('name', '長崎統括'), ('kana', 'ナガサキトウカツ'), ('hira', "*

 * *          "'ながさきとうかつ'), ('roma', 'nagasakitoukatsu')])",*

 * * "'005'": "OrderedDict([('code', '005'), ('name', '宮崎統括'), ('kana', 'ミヤザキトウカツ'), ('hira', "*

 * *  […]*

```diff
@@ -2,64 +2,85 @@
     "001": {
         "code": "001",
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
         "name": "\u672c\u5e97",
         "roma": "honten"
     },
-    "175": {
-        "code": "175",
-        "hira": "\u3084\u306a\u3044\u307f\u306a\u3068",
-        "kana": "\u30e4\u30ca\u30a4\u30df\u30ca\u30c8",
-        "name": "\u67f3\u4e95\u6e2f",
-        "roma": "yanaiminato"
-    },
-    "315": {
-        "code": "315",
-        "hira": "\u3057\u3086\u3046\u306a\u3093",
-        "kana": "\u30b7\u30e6\u30a6\u30ca\u30f3",
-        "name": "\u5468\u5357",
-        "roma": "shiyuunan"
-    },
-    "355": {
-        "code": "355",
-        "hira": "\u304d\u3064\u3055",
-        "kana": "\u30ad\u30c4\u30b5",
-        "name": "\u5409\u4f50",
-        "roma": "kitsusa"
-    },
-    "390": {
-        "code": "390",
-        "hira": "\u304a\u304a\u307f",
-        "kana": "\u30aa\u30aa\u30df",
-        "name": "\u5927\u6d77",
-        "roma": "oomi"
-    },
-    "510": {
-        "code": "510",
-        "hira": "\u3046\u3079\u307f\u3055\u304d",
-        "kana": "\u30a6\u30d9\u30df\u30b5\u30ad",
-        "name": "\u5b87\u90e8\u5cac",
-        "roma": "ubemisaki"
-    },
-    "815": {
-        "code": "815",
-        "hira": "\u306a\u304c\u3068",
-        "kana": "\u30ca\u30ac\u30c8",
-        "name": "\u9577\u9580",
-        "roma": "nagato"
-    },
-    "930": {
-        "code": "930",
-        "hira": "\u306f\u304e",
-        "kana": "\u30cf\u30ae",
-        "name": "\u306f\u304e",
-        "roma": "hagi"
-    },
-    "955": {
-        "code": "955",
-        "hira": "\u304a\u304a\u3057\u307e",
-        "kana": "\u30aa\u30aa\u30b7\u30de",
-        "name": "\u5927\u5cf6",
-        "roma": "ooshima"
+    "002": {
+        "code": "002",
+        "hira": "\u3055\u304c\u3068\u3046\u304b\u3064",
+        "kana": "\u30b5\u30ac\u30c8\u30a6\u30ab\u30c4",
+        "name": "\u4f50\u8cc0\u7d71\u62ec",
+        "roma": "sagatoukatsu"
+    },
+    "003": {
+        "code": "003",
+        "hira": "\u3042\u308a\u3042\u3051",
+        "kana": "\u30a2\u30ea\u30a2\u30b1",
+        "name": "\u6709\u660e",
+        "roma": "ariake"
+    },
+    "004": {
+        "code": "004",
+        "hira": "\u306a\u304c\u3055\u304d\u3068\u3046\u304b\u3064",
+        "kana": "\u30ca\u30ac\u30b5\u30ad\u30c8\u30a6\u30ab\u30c4",
+        "name": "\u9577\u5d0e\u7d71\u62ec",
+        "roma": "nagasakitoukatsu"
+    },
+    "005": {
+        "code": "005",
+        "hira": "\u307f\u3084\u3056\u304d\u3068\u3046\u304b\u3064",
+        "kana": "\u30df\u30e4\u30b6\u30ad\u30c8\u30a6\u30ab\u30c4",
+        "name": "\u5bae\u5d0e\u7d71\u62ec",
+        "roma": "miyazakitoukatsu"
+    },
+    "006": {
+        "code": "006",
+        "hira": "\u304b\u3054\u3057\u307e\u3068\u3046\u304b\u3064",
+        "kana": "\u30ab\u30b4\u30b7\u30de\u30c8\u30a6\u30ab\u30c4",
+        "name": "\u9e7f\u5150\u5cf6\u7d71\u62ec",
+        "roma": "kagoshimatoukatsu"
+    },
+    "007": {
+        "code": "007",
+        "hira": "\u304a\u304d\u306a\u308f\u3068\u3046\u304b\u3064",
+        "kana": "\u30aa\u30ad\u30ca\u30ef\u30c8\u30a6\u30ab\u30c4",
+        "name": "\u6c96\u7e04\u7d71\u62ec",
+        "roma": "okinawatoukatsu"
+    },
+    "125": {
+        "code": "125",
+        "hira": "\u304d\u305f\u3046\u3089",
+        "kana": "\u30ad\u30bf\u30a6\u30e9",
+        "name": "\u5317\u6d66",
+        "roma": "kitaura"
+    },
+    "127": {
+        "code": "127",
+        "hira": "\u3044\u304a\u308a\u304c\u308f",
+        "kana": "\u30a4\u30aa\u30ea\u30ac\u30ef",
+        "name": "\u5eb5\u5ddd",
+        "roma": "iorigawa"
+    },
+    "133": {
+        "code": "133",
+        "hira": "\u306a\u3093\u3054\u3046",
+        "kana": "\u30ca\u30f3\u30b4\u30a6",
+        "name": "\u5357\u90f7",
+        "roma": "nangou"
+    },
+    "500": {
+        "code": "500",
+        "hira": "\u304b\u3089\u3064",
+        "kana": "\u30ab\u30e9\u30c4",
+        "name": "\u5510\u6d25",
+        "roma": "karatsu"
+    },
+    "505": {
+        "code": "505",
+        "hira": "\u307f\u306a\u307f\u304b\u308f\u305d\u3048",
+        "kana": "\u30df\u30ca\u30df\u30ab\u30ef\u30bd\u30a8",
+        "name": "\u5357\u5ddd\u526f",
+        "roma": "minamikawasoe"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9486.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9486.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9489.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/3590.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.1%*

 * *Differences: {"'002'": "{'name': '千厩', 'kana': 'センマヤ', 'hira': 'せんまや', 'roma': 'semmaya'}",*

 * * "'008'": "OrderedDict([('code', '008'), ('name', '藤沢'), ('kana', 'フジサワ'), ('hira', 'ふじさわ'), "*

 * *          "('roma', 'fujisawa')])",*

 * * "'016'": "OrderedDict([('code', '016'), ('name', '大東'), ('kana', 'ダイトウ'), ('hira', 'だいとう'), "*

 * *          "('roma', 'daitou')])",*

 * * "'021'": "OrderedDict([('code', '021'), ('name', '東山'), ('kana', 'ヒガシヤマ'), ('hira', 'ひがしやま'), "*

 * *          "('roma', 'higashiyama')])",*

 * * "'114'": "OrderedDict([('code', '114 […]*

```diff
@@ -4,83 +4,55 @@
         "hira": "\u307b\u3093\u3066\u3093",
         "kana": "\u30db\u30f3\u30c6\u30f3",
         "name": "\u672c\u5e97",
         "roma": "honten"
     },
     "002": {
         "code": "002",
-        "hira": "\u3055\u304c\u3068\u3046\u304b\u3064",
-        "kana": "\u30b5\u30ac\u30c8\u30a6\u30ab\u30c4",
-        "name": "\u4f50\u8cc0\u7d71\u62ec",
-        "roma": "sagatoukatsu"
-    },
-    "003": {
-        "code": "003",
-        "hira": "\u3042\u308a\u3042\u3051",
-        "kana": "\u30a2\u30ea\u30a2\u30b1",
-        "name": "\u6709\u660e",
-        "roma": "ariake"
-    },
-    "004": {
-        "code": "004",
-        "hira": "\u306a\u304c\u3055\u304d\u3068\u3046\u304b\u3064",
-        "kana": "\u30ca\u30ac\u30b5\u30ad\u30c8\u30a6\u30ab\u30c4",
-        "name": "\u9577\u5d0e\u7d71\u62ec",
-        "roma": "nagasakitoukatsu"
-    },
-    "005": {
-        "code": "005",
-        "hira": "\u307f\u3084\u3056\u304d\u3068\u3046\u304b\u3064",
-        "kana": "\u30df\u30e4\u30b6\u30ad\u30c8\u30a6\u30ab\u30c4",
-        "name": "\u5bae\u5d0e\u7d71\u62ec",
-        "roma": "miyazakitoukatsu"
-    },
-    "006": {
-        "code": "006",
-        "hira": "\u304b\u3054\u3057\u307e\u3068\u3046\u304b\u3064",
-        "kana": "\u30ab\u30b4\u30b7\u30de\u30c8\u30a6\u30ab\u30c4",
-        "name": "\u9e7f\u5150\u5cf6\u7d71\u62ec",
-        "roma": "kagoshimatoukatsu"
-    },
-    "007": {
-        "code": "007",
-        "hira": "\u304a\u304d\u306a\u308f\u3068\u3046\u304b\u3064",
-        "kana": "\u30aa\u30ad\u30ca\u30ef\u30c8\u30a6\u30ab\u30c4",
-        "name": "\u6c96\u7e04\u7d71\u62ec",
-        "roma": "okinawatoukatsu"
-    },
-    "125": {
-        "code": "125",
-        "hira": "\u304d\u305f\u3046\u3089",
-        "kana": "\u30ad\u30bf\u30a6\u30e9",
-        "name": "\u5317\u6d66",
-        "roma": "kitaura"
-    },
-    "127": {
-        "code": "127",
-        "hira": "\u3044\u304a\u308a\u304c\u308f",
-        "kana": "\u30a4\u30aa\u30ea\u30ac\u30ef",
-        "name": "\u5eb5\u5ddd",
-        "roma": "iorigawa"
-    },
-    "133": {
-        "code": "133",
-        "hira": "\u306a\u3093\u3054\u3046",
-        "kana": "\u30ca\u30f3\u30b4\u30a6",
-        "name": "\u5357\u90f7",
-        "roma": "nangou"
-    },
-    "500": {
-        "code": "500",
-        "hira": "\u304b\u3089\u3064",
-        "kana": "\u30ab\u30e9\u30c4",
-        "name": "\u5510\u6d25",
-        "roma": "karatsu"
-    },
-    "505": {
-        "code": "505",
-        "hira": "\u307f\u306a\u307f\u304b\u308f\u305d\u3048",
-        "kana": "\u30df\u30ca\u30df\u30ab\u30ef\u30bd\u30a8",
-        "name": "\u5357\u5ddd\u526f",
-        "roma": "minamikawasoe"
+        "hira": "\u305b\u3093\u307e\u3084",
+        "kana": "\u30bb\u30f3\u30de\u30e4",
+        "name": "\u5343\u53a9",
+        "roma": "semmaya"
+    },
+    "008": {
+        "code": "008",
+        "hira": "\u3075\u3058\u3055\u308f",
+        "kana": "\u30d5\u30b8\u30b5\u30ef",
+        "name": "\u85e4\u6ca2",
+        "roma": "fujisawa"
+    },
+    "016": {
+        "code": "016",
+        "hira": "\u3060\u3044\u3068\u3046",
+        "kana": "\u30c0\u30a4\u30c8\u30a6",
+        "name": "\u5927\u6771",
+        "roma": "daitou"
+    },
+    "021": {
+        "code": "021",
+        "hira": "\u3072\u304c\u3057\u3084\u307e",
+        "kana": "\u30d2\u30ac\u30b7\u30e4\u30de",
+        "name": "\u6771\u5c71",
+        "roma": "higashiyama"
+    },
+    "114": {
+        "code": "114",
+        "hira": "\u3044\u3061\u306e\u305b\u304d\u3061\u3086\u3046\u304a\u3046",
+        "kana": "\u30a4\u30c1\u30ce\u30bb\u30ad\u30c1\u30e6\u30a6\u30aa\u30a6",
+        "name": "\u4e00\u95a2\u4e2d\u592e",
+        "roma": "ichinosekichiyuuou"
+    },
+    "118": {
+        "code": "118",
+        "hira": "\u306f\u306a\u3044\u305a\u307f",
+        "kana": "\u30cf\u30ca\u30a4\u30ba\u30df",
+        "name": "\u82b1\u6cc9",
+        "roma": "hanaizumi"
+    },
+    "124": {
+        "code": "124",
+        "hira": "\u3072\u3089\u3044\u305a\u307f",
+        "kana": "\u30d2\u30e9\u30a4\u30ba\u30df",
+        "name": "\u5e73\u6cc9",
+        "roma": "hiraizumi"
     }
 }
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9490.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9490.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9494.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9494.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code/source-data/data/branches/9900.json` & `zengin_code-1.1.0.20230607/zengin_code/source-data/data/branches/9900.json`

 * *Files identical despite different names*

### Comparing `zengin_code-1.1.0.20230501/zengin_code.egg-info/PKG-INFO` & `zengin_code-1.1.0.20230607/zengin_code.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zengin-code
-Version: 1.1.0.20230501
+Version: 1.1.0.20230607
 Summary: bank codes and branch codes for Japanese.
 Home-page: https://github.com/zengin-code/zengin-py
 Author: Zengin Code
 Author-email: zengin-code@zeny.io
 License: MIT
 Keywords: zengin,bank,japanese
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `zengin_code-1.1.0.20230501/zengin_code.egg-info/SOURCES.txt` & `zengin_code-1.1.0.20230607/zengin_code.egg-info/SOURCES.txt`

 * *Files identical despite different names*

