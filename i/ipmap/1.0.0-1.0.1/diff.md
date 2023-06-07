# Comparing `tmp/ipmap-1.0.0.tar.gz` & `tmp/ipmap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipmap-1.0.0.tar", max compression
+gzip compressed data, was "ipmap-1.0.1.tar", max compression
```

## Comparing `ipmap-1.0.0.tar` & `ipmap-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1500 2023-06-04 12:28:00.000000 ipmap-1.0.0/LICENSE
--rw-r--r--   0        0        0     3130 2023-06-06 23:03:05.426158 ipmap-1.0.0/README.md
--rw-r--r--   0        0        0     1508 2023-06-04 12:28:00.000000 ipmap-1.0.0/ipmap/__init__.py
--rw-r--r--   0        0        0     4655 2023-06-05 15:56:10.805432 ipmap-1.0.0/ipmap/config.py
--rw-r--r--   0        0        0      706 2023-06-06 23:02:11.704930 ipmap-1.0.0/ipmap/data/settings.json
--rw-r--r--   0        0        0     2215 2023-06-04 12:28:00.000000 ipmap-1.0.0/ipmap/data/templates/map.html
--rw-r--r--   0        0        0     4364 2023-06-06 23:03:05.406158 ipmap-1.0.0/ipmap/ipmap.py
--rw-r--r--   0        0        0     1197 2023-06-06 23:03:05.158152 ipmap-1.0.0/ipmap/main.py
--rw-r--r--   0        0        0     1533 2023-06-06 23:03:10.906280 ipmap-1.0.0/ipmap/utils.py
--rw-r--r--   0        0        0      664 2023-06-06 23:02:11.704930 ipmap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3822 1970-01-01 00:00:00.000000 ipmap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1500 2023-06-07 01:28:04.587199 ipmap-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5752 2023-06-07 01:28:04.591199 ipmap-1.0.1/README.md
+-rw-r--r--   0        0        0     1508 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/__init__.py
+-rw-r--r--   0        0        0     4655 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/config.py
+-rw-r--r--   0        0        0      735 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/data/settings.json
+-rw-r--r--   0        0        0     2215 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/data/templates/map.html
+-rw-r--r--   0        0        0     4364 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/ipmap.py
+-rw-r--r--   0        0        0     1197 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/main.py
+-rw-r--r--   0        0        0     1533 2023-06-07 01:28:04.591199 ipmap-1.0.1/ipmap/utils.py
+-rw-r--r--   0        0        0      920 2023-06-07 01:28:04.591199 ipmap-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6702 1970-01-01 00:00:00.000000 ipmap-1.0.1/PKG-INFO
```

### Comparing `ipmap-1.0.0/LICENSE` & `ipmap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.0/ipmap/__init__.py` & `ipmap-1.0.1/ipmap/__init__.py`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.0/ipmap/config.py` & `ipmap-1.0.1/ipmap/config.py`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.0/ipmap/data/settings.json` & `ipmap-1.0.1/ipmap/data/settings.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.971875%*

 * *Differences: {"'program'": "{'about': 'A cross-platform easy-to-use ip geolocation & mapping tool.', 'version': "*

 * *              "{'patch': '1'}}"}*

```diff
@@ -7,25 +7,25 @@
         "PURPLE": "[purple]",
         "RED": "[red]",
         "RESET": "[/]",
         "WHITE": "[white]",
         "YELLOW": "[yellow]"
     },
     "program": {
-        "about": "IP geolocation & mapping tool.",
+        "about": "A cross-platform easy-to-use ip geolocation & mapping tool.",
         "developer": {
             "about": "https://about.me/rly0nheart",
             "alias": "rly0nheart",
             "github": "https://github.com/rly0nheart",
             "name": "Richard Mwewa",
             "twitter": "https://twitter.com/rly0nheart"
         },
         "license": "BDS-3 Clause",
         "name": "IPMap (IP Mapper)",
         "version": {
             "major": "1",
             "minor": "0",
-            "patch": "0",
+            "patch": "1",
             "suffix": ""
         }
     }
 }
```

### Comparing `ipmap-1.0.0/ipmap/data/templates/map.html` & `ipmap-1.0.1/ipmap/data/templates/map.html`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.0/ipmap/ipmap.py` & `ipmap-1.0.1/ipmap/ipmap.py`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.0/ipmap/main.py` & `ipmap-1.0.1/ipmap/main.py`

 * *Files identical despite different names*

### Comparing `ipmap-1.0.0/ipmap/utils.py` & `ipmap-1.0.1/ipmap/utils.py`

 * *Files identical despite different names*

