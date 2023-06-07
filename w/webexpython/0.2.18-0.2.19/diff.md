# Comparing `tmp/webexpython-0.2.18.tar.gz` & `tmp/webexpython-0.2.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexpython-0.2.18.tar", last modified: Wed Jun  7 16:46:19 2023, max compression
+gzip compressed data, was "webexpython-0.2.19.tar", last modified: Wed Jun  7 16:54:12 2023, max compression
```

## Comparing `webexpython-0.2.18.tar` & `webexpython-0.2.19.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:46:19.535113 webexpython-0.2.18/
--rw-r--r--   0 josh       (501) staff       (20)      198 2023-06-07 16:46:19.534763 webexpython-0.2.18/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-07 16:46:19.535260 webexpython-0.2.18/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      327 2023-06-07 16:45:33.000000 webexpython-0.2.18/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:46:19.531553 webexpython-0.2.18/webexpython/
--rw-r--r--   0 josh       (501) staff       (20)       20 2022-03-17 16:32:34.000000 webexpython-0.2.18/webexpython/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    22671 2023-06-07 16:45:25.000000 webexpython-0.2.18/webexpython/webex.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:46:19.534121 webexpython-0.2.18/webexpython.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)      198 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)      227 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        9 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       12 2023-06-07 16:46:19.000000 webexpython-0.2.18/webexpython.egg-info/top_level.txt
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:54:12.834872 webexpython-0.2.19/
+-rw-r--r--   0 josh       (501) staff       (20)      198 2023-06-07 16:54:12.834555 webexpython-0.2.19/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-07 16:54:12.834977 webexpython-0.2.19/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      327 2023-06-07 16:53:51.000000 webexpython-0.2.19/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:54:12.832230 webexpython-0.2.19/webexpython/
+-rw-r--r--   0 josh       (501) staff       (20)       20 2022-03-17 16:32:34.000000 webexpython-0.2.19/webexpython/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    22672 2023-06-07 16:53:59.000000 webexpython-0.2.19/webexpython/webex.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-07 16:54:12.834079 webexpython-0.2.19/webexpython.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)      198 2023-06-07 16:54:12.000000 webexpython-0.2.19/webexpython.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)      227 2023-06-07 16:54:12.000000 webexpython-0.2.19/webexpython.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-07 16:54:12.000000 webexpython-0.2.19/webexpython.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        9 2023-06-07 16:54:12.000000 webexpython-0.2.19/webexpython.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       12 2023-06-07 16:54:12.000000 webexpython-0.2.19/webexpython.egg-info/top_level.txt
```

### Comparing `webexpython-0.2.18/webexpython/webex.py` & `webexpython-0.2.19/webexpython/webex.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,15 +381,15 @@
                 "code": code,
                 "description": description
             }
         ]
     }
     httpBodyJSON = json.dumps(API_DATA)
 
-    APIRESPONSE = requests.put(APIURI, headers=APIHEADER, data=httpBodyJSON)
+    APIRESPONSE = requests.post(APIURI, headers=APIHEADER, data=httpBodyJSON)
     results = APIRESPONSE.text
     return results
 
 
 def createVoicemailGroup(accessToken,
                          locationId,
                          orgId,
```

