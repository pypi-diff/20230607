# Comparing `tmp/nrsdk-1.1.1.3.tar.gz` & `tmp/nrsdk-1.1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrsdk-1.1.1.3.tar", last modified: Wed Jun  7 06:11:34 2023, max compression
+gzip compressed data, was "nrsdk-1.1.1.4.tar", last modified: Wed Jun  7 08:44:06 2023, max compression
```

## Comparing `nrsdk-1.1.1.3.tar` & `nrsdk-1.1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.985592 nrsdk-1.1.1.3/
--rw-rw-rw-   0        0        0      199 2023-06-07 06:11:34.985592 nrsdk-1.1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      881 2023-06-01 05:33:10.000000 nrsdk-1.1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.967638 nrsdk-1.1.1.3/nrsdk/
--rw-rw-rw-   0        0        0      119 2023-06-01 03:56:43.000000 nrsdk-1.1.1.3/nrsdk/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-05-16 09:18:13.000000 nrsdk-1.1.1.3/nrsdk/base.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.982601 nrsdk-1.1.1.3/nrsdk/lib/
--rw-rw-rw-   0        0        0  1810944 2023-06-05 08:20:03.000000 nrsdk-1.1.1.3/nrsdk/lib/QLNRSdk.dll
--rw-rw-rw-   0        0        0     1975 2023-06-01 03:59:11.000000 nrsdk-1.1.1.3/nrsdk/mcf_reader.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.984596 nrsdk-1.1.1.3/nrsdk/neuro_recorder/
--rw-rw-rw-   0        0        0     3808 2023-06-07 03:26:39.000000 nrsdk-1.1.1.3/nrsdk/neuro_recorder/__init__.py
--rw-rw-rw-   0        0        0     5594 2023-06-07 05:25:29.000000 nrsdk-1.1.1.3/nrsdk/nrsdk.py
--rw-rw-rw-   0        0        0     1995 2023-06-02 02:35:19.000000 nrsdk-1.1.1.3/nrsdk/paradigm.py
--rw-rw-rw-   0        0        0      136 2023-06-01 03:57:57.000000 nrsdk-1.1.1.3/nrsdk/rsa.py
-drwxrwxrwx   0        0        0        0 2023-06-07 06:11:34.981603 nrsdk-1.1.1.3/nrsdk.egg-info/
--rw-rw-rw-   0        0        0      199 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 06:05:49.000000 nrsdk-1.1.1.3/nrsdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-06-07 06:11:34.000000 nrsdk-1.1.1.3/nrsdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 06:11:34.985592 nrsdk-1.1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      573 2023-06-07 06:11:20.000000 nrsdk-1.1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:06.248084 nrsdk-1.1.1.4/
+-rw-rw-rw-   0        0        0      199 2023-06-07 08:44:06.247083 nrsdk-1.1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      881 2023-06-01 05:33:10.000000 nrsdk-1.1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:06.124178 nrsdk-1.1.1.4/nrsdk/
+-rw-rw-rw-   0        0        0      119 2023-06-01 03:56:43.000000 nrsdk-1.1.1.4/nrsdk/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-05-16 09:18:13.000000 nrsdk-1.1.1.4/nrsdk/base.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:06.146099 nrsdk-1.1.1.4/nrsdk/lib/
+-rw-rw-rw-   0        0        0  1810944 2023-06-05 08:20:03.000000 nrsdk-1.1.1.4/nrsdk/lib/QLNRSdk.dll
+-rw-rw-rw-   0        0        0     1975 2023-06-01 03:59:11.000000 nrsdk-1.1.1.4/nrsdk/mcf_reader.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:06.223803 nrsdk-1.1.1.4/nrsdk/neuro_recorder/
+-rw-rw-rw-   0        0        0     3808 2023-06-07 03:26:39.000000 nrsdk-1.1.1.4/nrsdk/neuro_recorder/__init__.py
+-rw-rw-rw-   0        0        0     5842 2023-06-07 07:38:56.000000 nrsdk-1.1.1.4/nrsdk/nrsdk.py
+-rw-rw-rw-   0        0        0     1995 2023-06-02 02:35:19.000000 nrsdk-1.1.1.4/nrsdk/paradigm.py
+-rw-rw-rw-   0        0        0      136 2023-06-01 03:57:57.000000 nrsdk-1.1.1.4/nrsdk/rsa.py
+drwxrwxrwx   0        0        0        0 2023-06-07 08:44:06.138143 nrsdk-1.1.1.4/nrsdk.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-06-07 08:44:05.000000 nrsdk-1.1.1.4/nrsdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-06-07 08:44:05.000000 nrsdk-1.1.1.4/nrsdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 08:44:05.000000 nrsdk-1.1.1.4/nrsdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-07 06:05:49.000000 nrsdk-1.1.1.4/nrsdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-06-07 08:44:05.000000 nrsdk-1.1.1.4/nrsdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 08:44:06.248084 nrsdk-1.1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      573 2023-06-07 08:43:09.000000 nrsdk-1.1.1.4/setup.py
```

### Comparing `nrsdk-1.1.1.3/README.md` & `nrsdk-1.1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.3/nrsdk/base.py` & `nrsdk-1.1.1.4/nrsdk/base.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.3/nrsdk/lib/QLNRSdk.dll` & `nrsdk-1.1.1.4/nrsdk/lib/QLNRSdk.dll`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.3/nrsdk/mcf_reader.py` & `nrsdk-1.1.1.4/nrsdk/mcf_reader.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.3/nrsdk/neuro_recorder/__init__.py` & `nrsdk-1.1.1.4/nrsdk/neuro_recorder/__init__.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.3/nrsdk/nrsdk.py` & `nrsdk-1.1.1.4/nrsdk/nrsdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,32 +136,36 @@
         p_resp = (c_char * 512)(0)
         len = 512
         res = -1
         p_device = c_char_p(device.encode('utf-8')) if device else c_char_p(None)
 
         ssid = None
         skey = None
+        result = {}
         try:
             res = _api.QLNR_GetDeviceWifiConfigEx(self.login_handle, p_wifi_config, wifi_config_len, p_resp, len, p_device)
             print("get wifi config {} for device[{}]".format(resp_result(res), device))
             if res == _RESP_SUCCESS:
                 wifi_config = p_wifi_config.value.decode("utf-8")
                 print(wifi_config)
-                if wifi_config.find( "currentssid") >= 0:
-                    ssid = wifi_config["currentssid"]
-                if wifi_config.find( "currentpassword") >= 0:
-                    skey = wifi_config["currentpassword"]
+                wifi_config = json.loads(wifi_config)
+                result["ssid"] = wifi_config["configssid"]
+                result["skey"] = wifi_config["configpassword"]
+                result["ssid_default"] = wifi_config["defaultssid"]
+                result["skey_default"] = wifi_config["defaultpassword"]
+                result["ssid_connected"] = wifi_config["currentssid"]
+                result["skey_connected"] = wifi_config["currentpassword"]
 
             else:
                 print(p_resp.value.decode("utf-8"))
             
         except Exception as e:
             print(e)
         
-        return ssid, skey
+        return result
 
 _RESP_SUCCESS = 0
 _SUCCESS = 1
 _FAIL = 0
 
 def resp_result(res):
     return 'success' if res == 0 else 'fail'
```

### Comparing `nrsdk-1.1.1.3/nrsdk/paradigm.py` & `nrsdk-1.1.1.4/nrsdk/paradigm.py`

 * *Files identical despite different names*

### Comparing `nrsdk-1.1.1.3/setup.py` & `nrsdk-1.1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from setuptools import find_packages
 
-VERSION = '1.1.1.3'
+VERSION = '1.1.1.4'
 AUTHOR='eegion'
 EMAIL='hehuajun@eegion.com'
 REQUIRED = [
     'beautifulsoup',
     "lxml"
 ]
```

