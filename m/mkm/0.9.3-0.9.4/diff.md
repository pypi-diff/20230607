# Comparing `tmp/mkm-0.9.3.tar.gz` & `tmp/mkm-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkm-0.9.3.tar", last modified: Mon Apr 13 09:15:48 2020, max compression
+gzip compressed data, was "dist/mkm-0.9.4.tar", last modified: Tue Nov 17 15:57:42 2020, max compression
```

## Comparing `mkm-0.9.3.tar` & `mkm-0.9.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-04-13 09:15:48.000000 mkm-0.9.3/
--rw-r--r--   0 moky       (501) staff       (20)     7871 2020-04-13 09:15:48.000000 mkm-0.9.3/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)     6042 2020-02-06 10:08:59.000000 mkm-0.9.3/README.md
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-04-13 09:15:48.000000 mkm-0.9.3/mkm/
--rw-r--r--   0 moky       (501) staff       (20)     2643 2020-04-09 17:33:41.000000 mkm-0.9.3/mkm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7397 2020-04-08 10:57:39.000000 mkm-0.9.3/mkm/address.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-04-13 09:15:48.000000 mkm-0.9.3/mkm/crypto/
--rw-r--r--   0 moky       (501) staff       (20)     1953 2020-04-09 17:33:41.000000 mkm-0.9.3/mkm/crypto/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     6663 2019-12-25 08:14:53.000000 mkm-0.9.3/mkm/crypto/asymmetric.py
--rw-r--r--   0 moky       (501) staff       (20)     3763 2020-04-08 10:55:49.000000 mkm-0.9.3/mkm/crypto/coder.py
--rw-r--r--   0 moky       (501) staff       (20)     3205 2019-11-21 10:38:12.000000 mkm-0.9.3/mkm/crypto/cryptography.py
--rw-r--r--   0 moky       (501) staff       (20)     3445 2020-04-09 17:33:41.000000 mkm-0.9.3/mkm/crypto/digest.py
--rw-r--r--   0 moky       (501) staff       (20)     3818 2019-12-25 08:14:53.000000 mkm-0.9.3/mkm/crypto/symmetric.py
--rw-r--r--   0 moky       (501) staff       (20)     5519 2019-11-21 10:56:46.000000 mkm-0.9.3/mkm/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     4287 2020-03-03 09:30:18.000000 mkm-0.9.3/mkm/entity.py
--rw-r--r--   0 moky       (501) staff       (20)     2950 2019-11-19 14:50:29.000000 mkm-0.9.3/mkm/group.py
--rw-r--r--   0 moky       (501) staff       (20)     6483 2020-03-03 09:29:04.000000 mkm-0.9.3/mkm/identifier.py
--rw-r--r--   0 moky       (501) staff       (20)    13541 2020-04-08 10:57:34.000000 mkm-0.9.3/mkm/meta.py
--rw-r--r--   0 moky       (501) staff       (20)     9167 2020-04-08 10:57:31.000000 mkm-0.9.3/mkm/profile.py
--rw-r--r--   0 moky       (501) staff       (20)     5276 2019-12-20 14:51:48.000000 mkm-0.9.3/mkm/tai.py
--rw-r--r--   0 moky       (501) staff       (20)     6870 2020-03-10 03:46:22.000000 mkm-0.9.3/mkm/types.py
--rw-r--r--   0 moky       (501) staff       (20)     6812 2019-11-19 15:17:50.000000 mkm-0.9.3/mkm/user.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-04-13 09:15:48.000000 mkm-0.9.3/mkm.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)     7871 2020-04-13 09:15:48.000000 mkm-0.9.3/mkm.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      421 2020-04-13 09:15:48.000000 mkm-0.9.3/mkm.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2020-04-13 09:15:48.000000 mkm-0.9.3/mkm.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2020-04-13 09:15:48.000000 mkm-0.9.3/mkm.egg-info/top_level.txt
--rw-r--r--   0 moky       (501) staff       (20)       38 2020-04-13 09:15:48.000000 mkm-0.9.3/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      876 2020-04-09 17:18:32.000000 mkm-0.9.3/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-11-17 15:57:42.000000 mkm-0.9.4/
+-rw-r--r--   0 moky       (501) staff       (20)     7871 2020-11-17 15:57:42.000000 mkm-0.9.4/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)     6042 2020-02-06 10:08:59.000000 mkm-0.9.4/README.md
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-11-17 15:57:42.000000 mkm-0.9.4/mkm/
+-rw-r--r--   0 moky       (501) staff       (20)     2643 2020-04-09 17:33:41.000000 mkm-0.9.4/mkm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7477 2020-11-17 10:02:44.000000 mkm-0.9.4/mkm/address.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-11-17 15:57:42.000000 mkm-0.9.4/mkm/crypto/
+-rw-r--r--   0 moky       (501) staff       (20)     1953 2020-04-09 17:33:41.000000 mkm-0.9.4/mkm/crypto/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     6663 2019-12-25 08:14:53.000000 mkm-0.9.4/mkm/crypto/asymmetric.py
+-rw-r--r--   0 moky       (501) staff       (20)     3763 2020-04-08 10:55:49.000000 mkm-0.9.4/mkm/crypto/coder.py
+-rw-r--r--   0 moky       (501) staff       (20)     3205 2019-11-21 10:38:12.000000 mkm-0.9.4/mkm/crypto/cryptography.py
+-rw-r--r--   0 moky       (501) staff       (20)     3445 2020-04-09 17:33:41.000000 mkm-0.9.4/mkm/crypto/digest.py
+-rw-r--r--   0 moky       (501) staff       (20)     3818 2019-12-25 08:14:53.000000 mkm-0.9.4/mkm/crypto/symmetric.py
+-rw-r--r--   0 moky       (501) staff       (20)     5519 2019-11-21 10:56:46.000000 mkm-0.9.4/mkm/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4287 2020-03-03 09:30:18.000000 mkm-0.9.4/mkm/entity.py
+-rw-r--r--   0 moky       (501) staff       (20)     2950 2019-11-19 14:50:29.000000 mkm-0.9.4/mkm/group.py
+-rw-r--r--   0 moky       (501) staff       (20)     6483 2020-03-03 09:29:04.000000 mkm-0.9.4/mkm/identifier.py
+-rw-r--r--   0 moky       (501) staff       (20)    13541 2020-04-08 10:57:34.000000 mkm-0.9.4/mkm/meta.py
+-rw-r--r--   0 moky       (501) staff       (20)     9173 2020-11-17 10:43:38.000000 mkm-0.9.4/mkm/profile.py
+-rw-r--r--   0 moky       (501) staff       (20)     5276 2019-12-20 14:51:48.000000 mkm-0.9.4/mkm/tai.py
+-rw-r--r--   0 moky       (501) staff       (20)     6870 2020-03-10 03:46:22.000000 mkm-0.9.4/mkm/types.py
+-rw-r--r--   0 moky       (501) staff       (20)     6812 2019-11-19 15:17:50.000000 mkm-0.9.4/mkm/user.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2020-11-17 15:57:42.000000 mkm-0.9.4/mkm.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)     7871 2020-11-17 15:57:42.000000 mkm-0.9.4/mkm.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      421 2020-11-17 15:57:42.000000 mkm-0.9.4/mkm.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2020-11-17 15:57:42.000000 mkm-0.9.4/mkm.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2020-11-17 15:57:42.000000 mkm-0.9.4/mkm.egg-info/top_level.txt
+-rw-r--r--   0 moky       (501) staff       (20)       38 2020-11-17 15:57:42.000000 mkm-0.9.4/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      876 2020-11-17 10:44:41.000000 mkm-0.9.4/setup.py
```

### Comparing `mkm-0.9.3/PKG-INFO` & `mkm-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkm
-Version: 0.9.3
+Version: 0.9.4
 Summary: A common identity module
 Home-page: https://github.com/dimchat/mkm-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Ming Ke Ming (名可名) -- Account Module (Python)
```

### Comparing `mkm-0.9.3/README.md` & `mkm-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/__init__.py` & `mkm-0.9.4/mkm/__init__.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/address.py` & `mkm-0.9.4/mkm/address.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,18 @@
         if length == len(ANYWHERE) and address.lower() == ANYWHERE:
             return ANYWHERE
         # everywhere
         if length == len(EVERYWHERE) and address.lower() == EVERYWHERE:
             return EVERYWHERE
         # try to create address object
         for clazz in cls.__address_classes:
-            inst = clazz.__new__(clazz, address)
+            try:
+                inst = clazz.__new__(clazz, address)
+            except ValueError:
+                continue
             if inst is not None:
                 return inst
         raise ValueError('unrecognized address: %s' % address)
 
     @property
     @abstractmethod
     def network(self) -> int:
@@ -126,15 +129,15 @@
         """
         Register address class
 
         :param address_class: class for parsing ID.address
         :return: False on error
         """
         if issubclass(address_class, Address):
-            cls.__address_classes.append(address_class)
+            cls.__address_classes.insert(0, address_class)
         else:
             raise TypeError('%s must be subclass of Address' % address_class)
         return True
 
 
 """
     Address like BitCoin
```

### Comparing `mkm-0.9.3/mkm/crypto/__init__.py` & `mkm-0.9.4/mkm/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/crypto/asymmetric.py` & `mkm-0.9.4/mkm/crypto/asymmetric.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/crypto/coder.py` & `mkm-0.9.4/mkm/crypto/coder.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/crypto/cryptography.py` & `mkm-0.9.4/mkm/crypto/cryptography.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/crypto/digest.py` & `mkm-0.9.4/mkm/crypto/digest.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/crypto/symmetric.py` & `mkm-0.9.4/mkm/crypto/symmetric.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/delegate.py` & `mkm-0.9.4/mkm/delegate.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/entity.py` & `mkm-0.9.4/mkm/entity.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/group.py` & `mkm-0.9.4/mkm/group.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/identifier.py` & `mkm-0.9.4/mkm/identifier.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/meta.py` & `mkm-0.9.4/mkm/meta.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/profile.py` & `mkm-0.9.4/mkm/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,17 +215,17 @@
         elif cls is UserProfile:
             # 1. if ID type is user, convert to UserProfile
             # 2. if public key not exists, no need to convert to UserProfile
             identifier = profile.get('ID')
             if isinstance(identifier, ID):
                 if not identifier.is_user:
                     return None
-            elif 'avatar' not in profile and 'key' not in profile:
-                # not a user profile
-                return None
+            # elif 'avatar' not in profile and 'key' not in profile:
+            #     # not a user profile
+            #     return None
         # new UserProfile(dict)
         return super().__new__(cls, profile)
 
     def __init__(self, profile: dict):
         if self is profile:
             # no need to init again
             return
```

### Comparing `mkm-0.9.3/mkm/tai.py` & `mkm-0.9.4/mkm/tai.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/types.py` & `mkm-0.9.4/mkm/types.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm/user.py` & `mkm-0.9.4/mkm/user.py`

 * *Files identical despite different names*

### Comparing `mkm-0.9.3/mkm.egg-info/PKG-INFO` & `mkm-0.9.4/mkm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkm
-Version: 0.9.3
+Version: 0.9.4
 Summary: A common identity module
 Home-page: https://github.com/dimchat/mkm-py
 Author: Albert Moky
 Author-email: albert.moky@gmail.com
 License: MIT
 Description: # Ming Ke Ming (名可名) -- Account Module (Python)
```

### Comparing `mkm-0.9.3/setup.py` & `mkm-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~~~~~~~~~~
 
     Common Identity Module for decentralized user identity authentication
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '0.9.3'
+__version__ = '0.9.4'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
```

