# Comparing `tmp/streamlit-qs-0.1.0.tar.gz` & `tmp/streamlit-qs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-qs-0.1.0.tar", last modified: Mon Jun  5 17:43:40 2023, max compression
+gzip compressed data, was "streamlit-qs-0.1.1.tar", last modified: Wed Jun  7 07:20:15 2023, max compression
```

## Comparing `streamlit-qs-0.1.0.tar` & `streamlit-qs-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 17:43:40.913457 streamlit-qs-0.1.0/
--rw-rw-rw-   0        0        0    11357 2023-06-05 05:42:27.000000 streamlit-qs-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2087 2023-06-05 17:43:40.912489 streamlit-qs-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1491 2023-06-05 07:48:47.000000 streamlit-qs-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-05 17:43:40.914458 streamlit-qs-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-06-05 05:52:34.000000 streamlit-qs-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:43:40.879547 streamlit-qs-0.1.0/streamlit_qs/
--rw-rw-rw-   0        0        0    19729 2023-06-05 11:10:41.000000 streamlit-qs-0.1.0/streamlit_qs/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-06-05 06:08:25.000000 streamlit-qs-0.1.0/streamlit_qs/capture.py
-drwxrwxrwx   0        0        0        0 2023-06-05 17:43:40.896533 streamlit-qs-0.1.0/streamlit_qs.egg-info/
--rw-rw-rw-   0        0        0     2087 2023-06-05 17:43:40.000000 streamlit-qs-0.1.0/streamlit_qs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-06-05 17:43:40.000000 streamlit-qs-0.1.0/streamlit_qs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 17:43:40.000000 streamlit-qs-0.1.0/streamlit_qs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-05 17:43:40.000000 streamlit-qs-0.1.0/streamlit_qs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-05 17:43:40.910462 streamlit-qs-0.1.0/tests/
--rw-rw-rw-   0        0        0     3039 2023-06-05 06:06:18.000000 streamlit-qs-0.1.0/tests/test_capture.py
--rw-rw-rw-   0        0        0    15821 2023-06-05 11:10:41.000000 streamlit-qs-0.1.0/tests/test_streamlit_qs.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:20:15.030810 streamlit-qs-0.1.1/
+-rw-rw-rw-   0        0        0    11357 2023-06-05 05:42:27.000000 streamlit-qs-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2087 2023-06-07 07:20:15.029813 streamlit-qs-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1491 2023-06-05 07:48:47.000000 streamlit-qs-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 07:20:15.030810 streamlit-qs-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-06-07 06:45:19.000000 streamlit-qs-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 07:20:15.008899 streamlit-qs-0.1.1/streamlit_qs/
+-rw-rw-rw-   0        0        0    20131 2023-06-07 07:16:26.000000 streamlit-qs-0.1.1/streamlit_qs/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 06:37:36.000000 streamlit-qs-0.1.1/streamlit_qs/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-07 07:20:15.026821 streamlit-qs-0.1.1/streamlit_qs.egg-info/
+-rw-rw-rw-   0        0        0     2087 2023-06-07 07:20:14.000000 streamlit-qs-0.1.1/streamlit_qs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-06-07 07:20:14.000000 streamlit-qs-0.1.1/streamlit_qs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 07:20:14.000000 streamlit-qs-0.1.1/streamlit_qs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-07 07:20:14.000000 streamlit-qs-0.1.1/streamlit_qs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 07:20:15.028845 streamlit-qs-0.1.1/tests/
+-rw-rw-rw-   0        0        0    15897 2023-06-07 07:18:42.000000 streamlit-qs-0.1.1/tests/test_streamlit_qs.py
```

### Comparing `streamlit-qs-0.1.0/LICENSE` & `streamlit-qs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-qs-0.1.0/PKG-INFO` & `streamlit-qs-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-qs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small library to add extra functionality on top of streamlit's experimental_[get/set]_query_string API
 Home-page: https://github.com/Asaurus1/streamlit-qs
 Author: Alexander Martin
 Author-email: fauxjunk-1@yahoo.com
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `streamlit-qs-0.1.0/README.md` & `streamlit-qs-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-qs-0.1.0/setup.py` & `streamlit-qs-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="streamlit-qs",
-    version="0.1.0",
+    version="0.1.1",
     author="Alexander Martin",
     author_email="fauxjunk-1@yahoo.com",
     description="A small library to add extra functionality on top of streamlit's experimental_[get/set]_query_string API",
     license="Apache 2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Asaurus1/streamlit-qs",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
+    package_data={"streamlit_qs": ["py.typed"]},
     install_requires=[],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
```

### Comparing `streamlit-qs-0.1.0/streamlit_qs/__init__.py` & `streamlit-qs-0.1.1/streamlit_qs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Callable,
     Collection,
     KeysView,
     List,
     Mapping,
     MutableMapping,
     Sequence,
+    Set,
     Type,
     TypeVar,
     cast,
     overload,
 )
 
 import streamlit as st
@@ -28,15 +29,28 @@
 
 T = TypeVar("T")
 
 
 # A list of query string keys are are not allowed because they are used
 # elsewhere in application backend code. Expected to be set by the user at
 # application initalization
-QS_BLACKLIST_KEYS: List[str] = []
+QS_BLACKLIST_KEYS: Set[str] = set()
+
+
+def blacklist_key(key: str):
+    """Add a key to the list of blacklisted keys that won't show up in the query string."""
+    QS_BLACKLIST_KEYS.add(key)
+
+
+def unblacklist_key(key: str):
+    """Remove a key from the list of blacklisted keys that won't show up in the query string.
+
+    Key is ignored if it isn't already blacklisted.
+    """
+    QS_BLACKLIST_KEYS.discard(key)
 
 
 def selectbox_qs(
     label: str, 
     options: OptionSequence[T], 
     index: int = 0, 
     *,
```

### Comparing `streamlit-qs-0.1.0/streamlit_qs.egg-info/PKG-INFO` & `streamlit-qs-0.1.1/streamlit_qs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-qs
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small library to add extra functionality on top of streamlit's experimental_[get/set]_query_string API
 Home-page: https://github.com/Asaurus1/streamlit-qs
 Author: Alexander Martin
 Author-email: fauxjunk-1@yahoo.com
 License: Apache 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `streamlit-qs-0.1.0/tests/test_streamlit_qs.py` & `streamlit-qs-0.1.1/tests/test_streamlit_qs.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,17 +243,19 @@
         assert stu._qs_intersect(tuple(), tuple()) == {}  # i.e. if the user passes in keys=[]
         assert stu._qs_intersect(["a3", "b3"], tuple()) == {"a3": 1, "b3": 2}
         assert stu._qs_intersect(["a3", "badval"], tuple()) == {"a3": 1}
         assert stu._qs_intersect(None, ["b.$"]) == {"b2": 3, "b3": 2}
         assert stu._qs_intersect(["a3"], ["b.$"]) == {"a3": 1, "b2": 3, "b3": 2}
 
     new_session_state = {"a3": 1, "blacklisted_key": "blacklisted"}
-    with mock.patch("streamlit.session_state", new=new_session_state), \
-        mock.patch.object(stu, "QS_BLACKLIST_KEYS", new=["blacklisted_key"]):
+    with mock.patch("streamlit.session_state", new=new_session_state):
+        stu.blacklist_key("blacklisted_key")
         assert stu._qs_intersect(None, tuple()) == {"a3": 1}
+        stu.unblacklist_key("blacklisted_key")
+        assert "blacklisted_key" not in stu.QS_BLACKLIST_KEYS
 
     with pytest.raises(ValueError, match="Arguments to query string functions must be non-str collections"):
         stu._qs_intersect("foo", tuple())
     with pytest.raises(ValueError, match="Arguments to query string functions must be non-str collections"):
         stu._qs_intersect(None, "foo")
```

